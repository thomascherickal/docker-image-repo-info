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
$ docker pull spiped@sha256:3f946d80813d27b67a12c1f37671961b9dafebeaa779ab08875cf6daa5ad8ed2
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
$ docker pull spiped@sha256:027c9e8b16fd5686f2386e10f4efea51d2cf9baf4e7bcdaf3c1fb979d3d6e6c2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.4 MB (37412991 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:803eb276e1835de8624a0705f68be4b52442d62ad95ad7f8933b8a2f1dfe7a40`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 01 Mar 2023 04:09:58 GMT
ADD file:493a5b0c8d2d63a1343258b3f9aa5fcd59a93f44fe26ad9e56b094c3a08fd3be in / 
# Wed, 01 Mar 2023 04:09:59 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 17:55:56 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 01 Mar 2023 17:55:59 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 17:55:59 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 01 Mar 2023 17:56:20 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 01 Mar 2023 17:56:20 GMT
VOLUME [/spiped]
# Wed, 01 Mar 2023 17:56:20 GMT
WORKDIR /spiped
# Wed, 01 Mar 2023 17:56:20 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 01 Mar 2023 17:56:20 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 01 Mar 2023 17:56:20 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:3f9582a2cbe7197f39185419c0ced2c986389f8fc6aa805e1f5c090eea6511e0`  
		Last Modified: Wed, 01 Mar 2023 04:14:23 GMT  
		Size: 31.4 MB (31411403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e97821d2ff040682a3d9356a04d84b72255c563d7603f7219e6ed9e7c0e80e3`  
		Last Modified: Wed, 01 Mar 2023 17:56:35 GMT  
		Size: 1.7 KB (1733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97f3106ca46ab6b0eb674057029e3469fb737549c0e17f93501a7baa91ee7d66`  
		Last Modified: Wed, 01 Mar 2023 17:56:34 GMT  
		Size: 1.1 KB (1054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22be67cd1cbaef6c42eaf8be1eccae8272262dbf3e2ff498e0c4ce7de42750df`  
		Last Modified: Wed, 01 Mar 2023 17:56:36 GMT  
		Size: 6.0 MB (5998329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ededc4cf18635cc66d453c3af24a583d4f300aa916b5d12a5e3622c70bb9a86b`  
		Last Modified: Wed, 01 Mar 2023 17:56:35 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2631603d11fd9110672446c8a343410ea67a502e725c014b4e1f83f522b56904`  
		Last Modified: Wed, 01 Mar 2023 17:56:35 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; arm variant v5

```console
$ docker pull spiped@sha256:528e13ba139adf0768024a80cfc79ab5cb3d0ea5e8f9b9f3bc1511f2d698c215
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.9 MB (33947393 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5a1e48f7b0e65652cca9ca80196c861d383ac1f1b0103cc512be95efd00fc6e9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 01 Mar 2023 01:48:54 GMT
ADD file:b4fb1081f6eb8a0560d56d5781bbcedaac1453615d56e0943245dca784785ea2 in / 
# Wed, 01 Mar 2023 01:48:54 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 07:10:40 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 01 Mar 2023 07:10:44 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 07:10:44 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 01 Mar 2023 07:11:03 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 01 Mar 2023 07:11:03 GMT
VOLUME [/spiped]
# Wed, 01 Mar 2023 07:11:03 GMT
WORKDIR /spiped
# Wed, 01 Mar 2023 07:11:03 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 01 Mar 2023 07:11:03 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 01 Mar 2023 07:11:04 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:3c3af56dbec5913ef8aec0f1ca7112eb5914b4ad346ccd48f836dd7ec0621ba5`  
		Last Modified: Wed, 01 Mar 2023 01:52:57 GMT  
		Size: 28.9 MB (28915776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9aca7d992b566279fbac9ecdeffb9ff2db68cf1ffd6f31a2cce852311c28c5ce`  
		Last Modified: Wed, 01 Mar 2023 07:11:20 GMT  
		Size: 1.7 KB (1728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fc3eb64d155ea643dfc7dde1104693192a95033b812f1cf66e286245705de6f`  
		Last Modified: Wed, 01 Mar 2023 07:11:20 GMT  
		Size: 1.1 KB (1050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9169ad29c4b57b416977f34e4cae1ad9b4efb6110e2a150a7cb43b7eab0da3d3`  
		Last Modified: Wed, 01 Mar 2023 07:11:21 GMT  
		Size: 5.0 MB (5028368 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:742f87e7cb263314cfe9b69a92b5fef45b368e04c178942b699311a03503e14c`  
		Last Modified: Wed, 01 Mar 2023 07:11:20 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0dfe2f008531a4616c872689c583cd0c8468b2fb60b07981fc0e20a80f84497`  
		Last Modified: Wed, 01 Mar 2023 07:11:20 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; arm variant v7

```console
$ docker pull spiped@sha256:627d305c141756ae7f1d3ce8a13ed19b5de3d5e5cc05419c57ca52a7cfad3e38
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.3 MB (31329572 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:80590efa308da9fa53e6713503023d50cdbb6bed46e6565e7a173368c94a3398`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 01 Mar 2023 01:57:55 GMT
ADD file:182fe91b8976a8871aba0d2ff9d4400a60317c8dec282261ba94247500c8d3dc in / 
# Wed, 01 Mar 2023 01:57:55 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 16:59:36 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 01 Mar 2023 16:59:39 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 16:59:39 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 01 Mar 2023 17:00:00 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 01 Mar 2023 17:00:00 GMT
VOLUME [/spiped]
# Wed, 01 Mar 2023 17:00:00 GMT
WORKDIR /spiped
# Wed, 01 Mar 2023 17:00:00 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 01 Mar 2023 17:00:00 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 01 Mar 2023 17:00:00 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:b4770fcf2ef78c1e46693da734476bfaf03cbe1d0b6e0a0f22c2c2e53419e803`  
		Last Modified: Wed, 01 Mar 2023 02:03:02 GMT  
		Size: 26.6 MB (26577290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe9ae4c200b12f57c7a99dbe5cd058c0c8e834ab0e042072df6f3ba0e2ef370b`  
		Last Modified: Wed, 01 Mar 2023 17:00:40 GMT  
		Size: 1.7 KB (1728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5dd24a9c965643a04effdcd9b7b20069af323b31c98f25e7ed41120a81c07cc`  
		Last Modified: Wed, 01 Mar 2023 17:00:40 GMT  
		Size: 1.1 KB (1051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0dba42d16068e44c779a0a9402aca488c2ae655c6d1c8fb07e88c3d68190a68b`  
		Last Modified: Wed, 01 Mar 2023 17:00:41 GMT  
		Size: 4.7 MB (4749033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c895f59fed0503b2299b019d207a580b45874b387ef1a68a3f08902c66676b63`  
		Last Modified: Wed, 01 Mar 2023 17:00:40 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f62eaf16d3dbd860a6214d912a6da95cacab5eaf97a19518ccf6c3ec0c774b0`  
		Last Modified: Wed, 01 Mar 2023 17:00:40 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:c0ee27c170b5818d26dd2679b9f68fbd1717c2b8029be42c1f19b7a9d582c867
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.3 MB (35338707 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f09e879bddede08a1bc165d3efa6587de5e8610534659bd12411ed41795ba246`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 01 Mar 2023 02:20:39 GMT
ADD file:9dc5c6fb6431df80107eddb76fb18256d6f4a06b4b22f9a7c4bcd58476068186 in / 
# Wed, 01 Mar 2023 02:20:39 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 14:07:19 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 01 Mar 2023 14:07:22 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 14:07:22 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 01 Mar 2023 14:07:37 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 01 Mar 2023 14:07:37 GMT
VOLUME [/spiped]
# Wed, 01 Mar 2023 14:07:37 GMT
WORKDIR /spiped
# Wed, 01 Mar 2023 14:07:37 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 01 Mar 2023 14:07:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 01 Mar 2023 14:07:38 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:66dbba0fb1b568cc3ffd53409ba2f9f82995ab7f80e379338f3f36e4dcd223be`  
		Last Modified: Wed, 01 Mar 2023 02:24:17 GMT  
		Size: 30.1 MB (30062814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:261024cf523923721d856c4f6e77a37c041d87ad2d3b4ccd92fb53f3abaab41f`  
		Last Modified: Wed, 01 Mar 2023 14:07:53 GMT  
		Size: 1.7 KB (1738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fe92519b62d1a9b8e2d52510cf1bf885ff477e0383a53bd4ee6a4efb5f3c14e`  
		Last Modified: Wed, 01 Mar 2023 14:07:53 GMT  
		Size: 1.1 KB (1051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a212b6d6d17e0b6cad09fb9cb67db006696d183039d38e32013a5fc3c0afb160`  
		Last Modified: Wed, 01 Mar 2023 14:07:54 GMT  
		Size: 5.3 MB (5272635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa9945ac00fd76d0a06763ef812f442fd4bb8aa3a67db027da1597a25f1e77aa`  
		Last Modified: Wed, 01 Mar 2023 14:07:53 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9fdec150625f76667b7ba6e9417519bf4f6d92c140125d060a1efb39e391342`  
		Last Modified: Wed, 01 Mar 2023 14:07:53 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; 386

```console
$ docker pull spiped@sha256:74d7f5c8f3f3d9c67ac2694a397c85180e9414b6092e41e394b39054f2029c92
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.3 MB (40291472 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cd42d521cfced48016618daf00f5e6976442656bf9c4005a7c8200ef734bcbd4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 23 Mar 2023 00:39:18 GMT
ADD file:315d843eefd4a8bb2345366dcd6bab00a06fca4a7970e220ae8946123d07d7ed in / 
# Thu, 23 Mar 2023 00:39:19 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 12:10:30 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Thu, 23 Mar 2023 12:10:33 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 12:10:33 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 23 Mar 2023 12:10:56 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 23 Mar 2023 12:10:56 GMT
VOLUME [/spiped]
# Thu, 23 Mar 2023 12:10:56 GMT
WORKDIR /spiped
# Thu, 23 Mar 2023 12:10:56 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 23 Mar 2023 12:10:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Mar 2023 12:10:57 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:3e638a975ea99fe8646002726dcb1ccdccc49ad33967b30337b9b2413e0619b5`  
		Last Modified: Thu, 23 Mar 2023 00:43:09 GMT  
		Size: 32.4 MB (32396277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8c70cbb4c8fd8326cfa3a38bcadaebdcf624fcd76381d57288eb687694073d1`  
		Last Modified: Thu, 23 Mar 2023 12:11:11 GMT  
		Size: 1.7 KB (1725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b85e36913d82a6dadb0781c7ab440ef652976cc8995f5f0a0bd0541b9b620373`  
		Last Modified: Thu, 23 Mar 2023 12:11:11 GMT  
		Size: 1.1 KB (1054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bec8a50af228e59f346840b516f8f52a3b22b0be6d31a71d1341b272cc16d2ad`  
		Last Modified: Thu, 23 Mar 2023 12:11:13 GMT  
		Size: 7.9 MB (7891948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af275a5a028f320d08a155a1238d5121d8a0198cebf123d479cfab9a01aafd10`  
		Last Modified: Thu, 23 Mar 2023 12:11:11 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:409fcb43c7b4c77abd48e9757bd49eadd9c1aade55294cd9145e4f451a2a7a75`  
		Last Modified: Thu, 23 Mar 2023 12:11:11 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; mips64le

```console
$ docker pull spiped@sha256:4b768c4a74571ecb307ea7f2c6f0d5444219c4f7701ca7ece08073134a9817c7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.3 MB (35342762 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:60d987426dc913c9b10892ddd45cd5d0cb2f8311fd0e994196056e11189abf9e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 01 Mar 2023 02:10:54 GMT
ADD file:0bcd66a6a099cdb6e018ddc0f00270be93dccd3be6167ce36e9efc99c31549d9 in / 
# Wed, 01 Mar 2023 02:10:59 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 13:56:50 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 01 Mar 2023 13:57:04 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 13:57:07 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 01 Mar 2023 13:58:36 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 01 Mar 2023 13:58:39 GMT
VOLUME [/spiped]
# Wed, 01 Mar 2023 13:58:42 GMT
WORKDIR /spiped
# Wed, 01 Mar 2023 13:58:44 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 01 Mar 2023 13:58:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 01 Mar 2023 13:58:49 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:89f6b45a7afd174bf0d443156831cacd9e6a26c834ad62610b6db53c731d257f`  
		Last Modified: Wed, 01 Mar 2023 02:18:50 GMT  
		Size: 29.6 MB (29634488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d10af42af1cddee9f8d002cb64f604273d7fd56c39403c8ecb2ca86ae445b2ac`  
		Last Modified: Wed, 01 Mar 2023 13:59:02 GMT  
		Size: 1.6 KB (1614 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da6cf49bc572eb473177215ee0a0e9187f04a782706a0d2a362817c62e3e4c1c`  
		Last Modified: Wed, 01 Mar 2023 13:59:03 GMT  
		Size: 928.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:030a52e1972e6a16de35f2c209c9fe8b1b7b677e38894c831863d54f0f1d6cfa`  
		Last Modified: Wed, 01 Mar 2023 13:59:07 GMT  
		Size: 5.7 MB (5705294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8eeca73463248c240d686d1c65ee25f2d27dd86f1920c0ab13f7974cd43b0d51`  
		Last Modified: Wed, 01 Mar 2023 13:59:03 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3867f0e8bddd40c5ae56a42d561c19e9e6c3520d9bb3a19c4ee8e10b5e35a76a`  
		Last Modified: Wed, 01 Mar 2023 13:59:02 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; ppc64le

```console
$ docker pull spiped@sha256:5eeeda056f21e90509214894b25b29c2f077d779e3a9894d7239c7c5b1dde12d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.3 MB (41291034 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2af8e0b52e04e9db1d381ffa1800979e5bb8de9720068f9bb1b0598a7198df6e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 01 Mar 2023 04:47:33 GMT
ADD file:6fdf0b2f8ea4be2d01e25a9d85db8f8c7e3b2a641c9c7665e34f4fad771815e0 in / 
# Wed, 01 Mar 2023 04:47:35 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 14:40:08 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 01 Mar 2023 14:40:14 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 14:40:15 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 01 Mar 2023 14:41:05 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 01 Mar 2023 14:41:06 GMT
VOLUME [/spiped]
# Wed, 01 Mar 2023 14:41:06 GMT
WORKDIR /spiped
# Wed, 01 Mar 2023 14:41:07 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 01 Mar 2023 14:41:07 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 01 Mar 2023 14:41:08 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:93ab3a60c2a8cbc1150cb2bd54222db8b79c525c0243534a10d6294ef7ff83ac`  
		Last Modified: Wed, 01 Mar 2023 04:53:54 GMT  
		Size: 35.3 MB (35288103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0a2080116d00583c373f079b8f40c2fa202cfaa894e5646b928e2f519bc8d0e`  
		Last Modified: Wed, 01 Mar 2023 14:41:39 GMT  
		Size: 1.7 KB (1734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6c05e885d8e0e269f3910fa5c387e4bfe94b5f5844a929e3f2945347c9bc33a`  
		Last Modified: Wed, 01 Mar 2023 14:41:39 GMT  
		Size: 1.1 KB (1055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f9c9a00d487b5d63eb533652fd7c8bbcaf5b4a766b8f50698468f313ea58b31`  
		Last Modified: Wed, 01 Mar 2023 14:41:41 GMT  
		Size: 6.0 MB (5999671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5ffd618016f8cd2101168350b00bdbad7932215a46cddd3c1abc7a1efdf9834`  
		Last Modified: Wed, 01 Mar 2023 14:41:39 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed01129e03be3daf248d482853655a906b1f3e7594b351c1d568f69c46c410ac`  
		Last Modified: Wed, 01 Mar 2023 14:41:39 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; s390x

```console
$ docker pull spiped@sha256:5052a882da69e191760a75d37205ff0a1edd8edf21ae507a22d93c6b1672215a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.8 MB (34837546 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4be5954f5bff77d2a4e04836cc5938d850a56e7ee023f169242f1226e121a558`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 23 Mar 2023 00:44:06 GMT
ADD file:8b6d3f57adaa8af2e0599a6468c50b713d281165b4e61150850bedf587f7ad4f in / 
# Thu, 23 Mar 2023 00:44:08 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 12:15:46 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Thu, 23 Mar 2023 12:15:49 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 12:15:49 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 23 Mar 2023 12:16:07 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 23 Mar 2023 12:16:08 GMT
VOLUME [/spiped]
# Thu, 23 Mar 2023 12:16:08 GMT
WORKDIR /spiped
# Thu, 23 Mar 2023 12:16:08 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 23 Mar 2023 12:16:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Mar 2023 12:16:09 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:25d08e051bb75230bad82e3a7a054083beec6b4f6a46c8345c731582c297a408`  
		Last Modified: Thu, 23 Mar 2023 00:47:20 GMT  
		Size: 29.6 MB (29646820 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3388e32dd1b77d93d6b62ba801fb658ac69c6eebde8b030476caac13f83542be`  
		Last Modified: Thu, 23 Mar 2023 12:16:29 GMT  
		Size: 1.7 KB (1736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a701ac09c5ac118d050e81f6139936da77a346003315c4444e1939a6b9fbf5a`  
		Last Modified: Thu, 23 Mar 2023 12:16:29 GMT  
		Size: 1.1 KB (1050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76c28eecb90a4ce4306f2ee104c3b7a26ed907a1d7b4ffe9ee9f404860df7d2f`  
		Last Modified: Thu, 23 Mar 2023 12:16:30 GMT  
		Size: 5.2 MB (5187470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:851271a85236c408b9e2df7b62a45c37bc5552fb05fc8fb30a87d4f40e207d26`  
		Last Modified: Thu, 23 Mar 2023 12:16:29 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30749340374b1df790439fe4c7b71b610b3d0ae3aef3705de18f2472f5933c06`  
		Last Modified: Thu, 23 Mar 2023 12:16:29 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:1-alpine`

```console
$ docker pull spiped@sha256:dfaf6e7592d4ab323a62d1b401cab7d35cab87afdb70fe94fc8d2c41d99aca33
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
$ docker pull spiped@sha256:b02340eb97482a93ed8c3997880473f27309e7362e27d06bfbdeb686da9f835f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.1 MB (5080754 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1660f13550a5bd6ce0ec142f4dc1325092450163ee42f52b56572854d7e8c1e3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Sat, 11 Feb 2023 04:46:42 GMT
ADD file:40887ab7c06977737e63c215c9bd297c0c74de8d12d16ebdf1c3d40ac392f62d in / 
# Sat, 11 Feb 2023 04:46:42 GMT
CMD ["/bin/sh"]
# Sat, 11 Feb 2023 14:04:29 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Sat, 11 Feb 2023 14:04:30 GMT
RUN apk add --no-cache libssl1.1
# Sat, 11 Feb 2023 14:04:30 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Sat, 11 Feb 2023 14:04:41 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Sat, 11 Feb 2023 14:04:41 GMT
VOLUME [/spiped]
# Sat, 11 Feb 2023 14:04:41 GMT
WORKDIR /spiped
# Sat, 11 Feb 2023 14:04:41 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 11 Feb 2023 14:04:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 11 Feb 2023 14:04:41 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:63b65145d645c1250c391b2d16ebe53b3747c295ca8ba2fcb6b0cf064a4dc21c`  
		Last Modified: Fri, 10 Feb 2023 22:41:31 GMT  
		Size: 3.4 MB (3374446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1567e533de4a753157026d7ef2c42cfa5f9efd21e25cc7370e4c8f1c8f1c8a47`  
		Last Modified: Sat, 11 Feb 2023 14:04:56 GMT  
		Size: 1.3 KB (1267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1a1fcb595374972f69b5a50bd54f62b80c9214b0f891c62726a3fb6853cf855`  
		Last Modified: Sat, 11 Feb 2023 14:04:56 GMT  
		Size: 1.5 MB (1483289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24f4efb6e81c911655772824a287a9f39d90e069841b4fe5601933b9b0ffe154`  
		Last Modified: Sat, 11 Feb 2023 14:04:56 GMT  
		Size: 221.3 KB (221282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:981056191296cd6f887bc7d5e8e078e1cec12690bc7fc8623b868e6b4023e0ea`  
		Last Modified: Sat, 11 Feb 2023 14:04:56 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:577ef58b3b8b045fa02bbbbd599b6c9d4310c0039e442d91e549dad4f7e556fd`  
		Last Modified: Sat, 11 Feb 2023 14:04:56 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; arm variant v6

```console
$ docker pull spiped@sha256:76a36336fb4a148684ae27104022667db149e7b75e602fb0d1fb636cb8277330
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.6 MB (4559988 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8148101a55ef329eee778b51e7674409dd7530f66643e375f5eaf15450e8d364`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Mon, 13 Mar 2023 16:12:44 GMT
ADD file:d825d9aef59df0df23c0140a490998407ee0a62a051699b5c050aef7cb03f042 in / 
# Mon, 13 Mar 2023 16:12:44 GMT
CMD ["/bin/sh"]
# Tue, 14 Mar 2023 01:30:23 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Tue, 14 Mar 2023 01:30:24 GMT
RUN apk add --no-cache libssl1.1
# Tue, 14 Mar 2023 01:30:24 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 14 Mar 2023 01:30:32 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Tue, 14 Mar 2023 01:30:32 GMT
VOLUME [/spiped]
# Tue, 14 Mar 2023 01:30:32 GMT
WORKDIR /spiped
# Tue, 14 Mar 2023 01:30:32 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 14 Mar 2023 01:30:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 14 Mar 2023 01:30:32 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:6a6e4ab63e54442e16400f69d37f662d60cbd67565631eff6bf59b4176e482c3`  
		Last Modified: Fri, 10 Feb 2023 20:50:22 GMT  
		Size: 3.1 MB (3110885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e45faa3e84504ff194d07161781bbb3d65ced006b3559fdd50974ca59bede67b`  
		Last Modified: Tue, 14 Mar 2023 01:30:48 GMT  
		Size: 1.3 KB (1271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a49b678821973054e204d328f8a1abfd5c4d0babdc516e24b56c76cc2adbd596`  
		Last Modified: Tue, 14 Mar 2023 01:30:49 GMT  
		Size: 1.2 MB (1240997 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8dbbba3d131edbec32d7ac2251201ab33e79abc9994b4e0635fac27365f1579f`  
		Last Modified: Tue, 14 Mar 2023 01:30:49 GMT  
		Size: 206.4 KB (206366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f344f34fb34133bb7a416417587f8f9219c749343ba309ab724c2dba1c4653c3`  
		Last Modified: Tue, 14 Mar 2023 01:30:48 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8506930f7b522732a72fca7395d31bb8094739139324468e7ae618b1da4d3cda`  
		Last Modified: Tue, 14 Mar 2023 01:30:48 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; arm variant v7

```console
$ docker pull spiped@sha256:361539f7f9277859ba382de7be4afe676210140f53c3c5cd85d5ae3985f905c0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4237927 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2e899581be5421f50eb7e6339c7512ab16c114d8213f09e8aca52c68f0bcc311`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 10 Feb 2023 21:51:31 GMT
ADD file:143b601fcc6b5d7d95d3e5ccad3fec7081191a47e28d4f9294a7fb2499cab1af in / 
# Fri, 10 Feb 2023 21:51:31 GMT
CMD ["/bin/sh"]
# Wed, 01 Mar 2023 17:00:05 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Wed, 01 Mar 2023 17:00:07 GMT
RUN apk add --no-cache libssl1.1
# Wed, 01 Mar 2023 17:00:07 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 01 Mar 2023 17:00:14 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Wed, 01 Mar 2023 17:00:14 GMT
VOLUME [/spiped]
# Wed, 01 Mar 2023 17:00:14 GMT
WORKDIR /spiped
# Wed, 01 Mar 2023 17:00:14 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 01 Mar 2023 17:00:14 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 01 Mar 2023 17:00:15 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:6fb81ff47bd6d7db0ed86c9b951ad6417ec73ab60af6d22daa604076a902629c`  
		Last Modified: Fri, 10 Feb 2023 21:52:33 GMT  
		Size: 2.9 MB (2868494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bcf9acc5eeca77f6d435380f4f1fea53c3643c4cc9042daf13fdd9b6b72d9f5`  
		Last Modified: Wed, 01 Mar 2023 17:00:57 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f34e65da889251051ec9481b5d6cb0d428c45c8861fb2948b0c38c07470bba59`  
		Last Modified: Wed, 01 Mar 2023 17:00:57 GMT  
		Size: 1.2 MB (1167579 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0412dc4bafb0f9dabcfd28a3c0b4454de2db5c81112fdbb51bf5c883f4a6925`  
		Last Modified: Wed, 01 Mar 2023 17:00:57 GMT  
		Size: 200.1 KB (200120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70011259fd33df6da621cfb9142329c3c7a89b4bc5bfe91a87f7335995930ff9`  
		Last Modified: Wed, 01 Mar 2023 17:00:57 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99d3fd9f335e89a8501d7008f1bbaf813f4a5b26227452ecfc0001613be1ee7f`  
		Last Modified: Wed, 01 Mar 2023 17:00:57 GMT  
		Size: 337.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:b202c4e5897cb771f303b85871c6b7a1fb5f025c51e651b30a4415f0e2e4973d
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.8 MB (4842933 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6c3a0f714da4f343e79de4855fa4cdc4a23892d7fe5654dec6710bc79bb2cc2c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 10 Feb 2023 21:24:08 GMT
ADD file:9bd9ea42a9f3bdc769e80c6b8a4b117d65f73ae68e155a6172a1184e7ac8bcc1 in / 
# Fri, 10 Feb 2023 21:24:08 GMT
CMD ["/bin/sh"]
# Sat, 11 Feb 2023 06:39:43 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Sat, 11 Feb 2023 06:39:44 GMT
RUN apk add --no-cache libssl1.1
# Sat, 11 Feb 2023 06:39:44 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Sat, 11 Feb 2023 06:39:52 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Sat, 11 Feb 2023 06:39:52 GMT
VOLUME [/spiped]
# Sat, 11 Feb 2023 06:39:52 GMT
WORKDIR /spiped
# Sat, 11 Feb 2023 06:39:52 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 11 Feb 2023 06:39:52 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 11 Feb 2023 06:39:52 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:af6eaf76a39c2d3e7e0b8a0420486e3df33c4027d696c076a99a3d0ac09026af`  
		Last Modified: Fri, 10 Feb 2023 21:24:39 GMT  
		Size: 3.3 MB (3261959 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32e706a54c37c1524628e434965039ac738ff48a6f151dd2ef6da2cb49958cc0`  
		Last Modified: Sat, 11 Feb 2023 06:40:07 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e99781ddd302da37630cc491b5190c39c7867e6bd96556fad9f613e3411bca0d`  
		Last Modified: Sat, 11 Feb 2023 06:40:07 GMT  
		Size: 1.4 MB (1363548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:768a1af5c81e5cc877ea8cb330527a3924d5f2b5acfc5dd8239f84fdf091e5ed`  
		Last Modified: Sat, 11 Feb 2023 06:40:07 GMT  
		Size: 215.7 KB (215691 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7567bda17775002440a508f6ff25154cb13c9201175281b80186ce38d44e2b7`  
		Last Modified: Sat, 11 Feb 2023 06:40:07 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba17a7f3c3024db40a3e0b478318d1eb5168af1437c2bd502fb302591b78f95a`  
		Last Modified: Sat, 11 Feb 2023 06:40:07 GMT  
		Size: 338.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; 386

```console
$ docker pull spiped@sha256:1718408d282e2785554de5dd41b1935a8fd740cad6fa42ddeac2fafad4e15148
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.1 MB (5131990 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e81769d87082a52703eb2f30d09dbe3c289d1e6956af04796da66cf8ec2e5a5b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 10 Feb 2023 21:24:23 GMT
ADD file:125f3514520a5cd29df2830a409aa026a2bc06a77a7a5d150133436404b33d41 in / 
# Fri, 10 Feb 2023 21:24:24 GMT
CMD ["/bin/sh"]
# Wed, 01 Mar 2023 20:35:30 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Wed, 01 Mar 2023 20:35:32 GMT
RUN apk add --no-cache libssl1.1
# Wed, 01 Mar 2023 20:35:32 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 01 Mar 2023 20:35:44 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Wed, 01 Mar 2023 20:35:44 GMT
VOLUME [/spiped]
# Wed, 01 Mar 2023 20:35:44 GMT
WORKDIR /spiped
# Wed, 01 Mar 2023 20:35:44 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 01 Mar 2023 20:35:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 01 Mar 2023 20:35:44 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:b3e346c15c2377ec0e75cc9efa98baecd58b0e9bb92f0ec07eeda0bcc7e67fc7`  
		Last Modified: Fri, 10 Feb 2023 21:25:13 GMT  
		Size: 3.4 MB (3412353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9ddea08df82e419c862a82c04a7b6027073e509f79247aaab6fcb9a2d66e4bc`  
		Last Modified: Wed, 01 Mar 2023 20:36:27 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7baff4523d8b5b8d72311936f6b35a74dc61f50af8ceb150e8a464755ed3ff76`  
		Last Modified: Wed, 01 Mar 2023 20:36:27 GMT  
		Size: 1.5 MB (1486288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de00b81755546779184cb3998ef43c5c0445cd5871998c7feb92240ab36aeb5e`  
		Last Modified: Wed, 01 Mar 2023 20:36:27 GMT  
		Size: 231.6 KB (231613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:568814bee4cca693df73f2ed16adcc10335f014f7606b67b33d08c3abf12b51a`  
		Last Modified: Wed, 01 Mar 2023 20:36:27 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da028d97e3da3f51bb23a54f50dc51e00a905208ac487c94ae446e20f926b63c`  
		Last Modified: Wed, 01 Mar 2023 20:36:27 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; ppc64le

```console
$ docker pull spiped@sha256:75c7e8ce27d4c68e8862a8e832409e09dbeb2c47fa2163ac0ac7f4e794b6b14c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.0 MB (5025550 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:523cfab6c09a42cd9174ca6dee237febe2f4a72f0c07628ccddab56278968150`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 10 Feb 2023 21:20:36 GMT
ADD file:ec037a0d4b462d12963ac20d9ec49bb73b4bcaf84d4bc7b364ebf93667e585b0 in / 
# Fri, 10 Feb 2023 21:20:36 GMT
CMD ["/bin/sh"]
# Sat, 11 Feb 2023 09:33:46 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Sat, 11 Feb 2023 09:33:49 GMT
RUN apk add --no-cache libssl1.1
# Sat, 11 Feb 2023 09:33:50 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Sat, 11 Feb 2023 09:34:04 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Sat, 11 Feb 2023 09:34:04 GMT
VOLUME [/spiped]
# Sat, 11 Feb 2023 09:34:05 GMT
WORKDIR /spiped
# Sat, 11 Feb 2023 09:34:05 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 11 Feb 2023 09:34:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 11 Feb 2023 09:34:06 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:aa3c56f9c6f127b6c8f628c95db165741ca400d19bdaef2752d80f093e47451e`  
		Last Modified: Fri, 10 Feb 2023 21:21:37 GMT  
		Size: 3.4 MB (3390750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b5d50df2303841e19f748472d51fac8d0695468f1d50516484905b50450aa48`  
		Last Modified: Sat, 11 Feb 2023 09:34:31 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0b54432b9107e6d87810bd116ab5112e27a1f713d4d2c06525f0ed14f102e3c`  
		Last Modified: Sat, 11 Feb 2023 09:34:32 GMT  
		Size: 1.4 MB (1413040 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4bda8ea646857e9e3d0c92c042261af7dba424338abfc7cc1c58eec7b8985be`  
		Last Modified: Sat, 11 Feb 2023 09:34:32 GMT  
		Size: 220.0 KB (220021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e33bc423b9fd5cc84d66be2c92fc2c78368e9b5553d8c6848fab3570115fb66`  
		Last Modified: Sat, 11 Feb 2023 09:34:31 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53a89c5ec31eae84c318581d292f2fdc24ec49bc7692940d54b3b579b04cd2d6`  
		Last Modified: Sat, 11 Feb 2023 09:34:31 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; s390x

```console
$ docker pull spiped@sha256:c224a59dd171160cb9e3b3be6bac31704ad968f23bed4f4f8ae4d04d938951c6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.6 MB (4608839 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:88032fe647cd1b9c54c93549e3978f1e53d8c0df71f2c0c2660b0545fc0b7ae3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 10 Feb 2023 21:41:25 GMT
ADD file:03b2fb4d732a294329449ff55c5d84f7d2735e6510985718979469994f3a607b in / 
# Fri, 10 Feb 2023 21:41:26 GMT
CMD ["/bin/sh"]
# Sat, 11 Feb 2023 05:20:31 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Sat, 11 Feb 2023 05:20:32 GMT
RUN apk add --no-cache libssl1.1
# Sat, 11 Feb 2023 05:20:33 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Sat, 11 Feb 2023 05:20:38 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Sat, 11 Feb 2023 05:20:38 GMT
VOLUME [/spiped]
# Sat, 11 Feb 2023 05:20:38 GMT
WORKDIR /spiped
# Sat, 11 Feb 2023 05:20:39 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 11 Feb 2023 05:20:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 11 Feb 2023 05:20:39 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:24c4f8de3549a39c64b0edc2cfa68769b373f35138d0f13725100160bb32d4e2`  
		Last Modified: Fri, 10 Feb 2023 21:42:16 GMT  
		Size: 3.2 MB (3175116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdb5c0ff1110b4315355f81e38de10bb31ba9fe44d99d3b7598f20a28f2c98e1`  
		Last Modified: Sat, 11 Feb 2023 05:21:04 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9ac27252903c2b21737926a9cd0721ecfa3aba4f2e52da7f7c114aea4da62df`  
		Last Modified: Sat, 11 Feb 2023 05:21:04 GMT  
		Size: 1.2 MB (1223356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df30f40ce9a4931562f50ea55d6450396fd443fed95a0b2c0ea337f53f22ec25`  
		Last Modified: Sat, 11 Feb 2023 05:21:04 GMT  
		Size: 208.6 KB (208631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d9420167a9c04b73e787d02b0fa09ba21ff8b27917d0406146f9bc5a0df3034`  
		Last Modified: Sat, 11 Feb 2023 05:21:04 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea129f4350d878551c457a2192ea0570f86ca7ee5c193a6b0d8e19727570f05b`  
		Last Modified: Sat, 11 Feb 2023 05:21:04 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:1.6`

```console
$ docker pull spiped@sha256:3f946d80813d27b67a12c1f37671961b9dafebeaa779ab08875cf6daa5ad8ed2
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
$ docker pull spiped@sha256:027c9e8b16fd5686f2386e10f4efea51d2cf9baf4e7bcdaf3c1fb979d3d6e6c2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.4 MB (37412991 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:803eb276e1835de8624a0705f68be4b52442d62ad95ad7f8933b8a2f1dfe7a40`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 01 Mar 2023 04:09:58 GMT
ADD file:493a5b0c8d2d63a1343258b3f9aa5fcd59a93f44fe26ad9e56b094c3a08fd3be in / 
# Wed, 01 Mar 2023 04:09:59 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 17:55:56 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 01 Mar 2023 17:55:59 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 17:55:59 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 01 Mar 2023 17:56:20 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 01 Mar 2023 17:56:20 GMT
VOLUME [/spiped]
# Wed, 01 Mar 2023 17:56:20 GMT
WORKDIR /spiped
# Wed, 01 Mar 2023 17:56:20 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 01 Mar 2023 17:56:20 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 01 Mar 2023 17:56:20 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:3f9582a2cbe7197f39185419c0ced2c986389f8fc6aa805e1f5c090eea6511e0`  
		Last Modified: Wed, 01 Mar 2023 04:14:23 GMT  
		Size: 31.4 MB (31411403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e97821d2ff040682a3d9356a04d84b72255c563d7603f7219e6ed9e7c0e80e3`  
		Last Modified: Wed, 01 Mar 2023 17:56:35 GMT  
		Size: 1.7 KB (1733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97f3106ca46ab6b0eb674057029e3469fb737549c0e17f93501a7baa91ee7d66`  
		Last Modified: Wed, 01 Mar 2023 17:56:34 GMT  
		Size: 1.1 KB (1054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22be67cd1cbaef6c42eaf8be1eccae8272262dbf3e2ff498e0c4ce7de42750df`  
		Last Modified: Wed, 01 Mar 2023 17:56:36 GMT  
		Size: 6.0 MB (5998329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ededc4cf18635cc66d453c3af24a583d4f300aa916b5d12a5e3622c70bb9a86b`  
		Last Modified: Wed, 01 Mar 2023 17:56:35 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2631603d11fd9110672446c8a343410ea67a502e725c014b4e1f83f522b56904`  
		Last Modified: Wed, 01 Mar 2023 17:56:35 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; arm variant v5

```console
$ docker pull spiped@sha256:528e13ba139adf0768024a80cfc79ab5cb3d0ea5e8f9b9f3bc1511f2d698c215
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.9 MB (33947393 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5a1e48f7b0e65652cca9ca80196c861d383ac1f1b0103cc512be95efd00fc6e9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 01 Mar 2023 01:48:54 GMT
ADD file:b4fb1081f6eb8a0560d56d5781bbcedaac1453615d56e0943245dca784785ea2 in / 
# Wed, 01 Mar 2023 01:48:54 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 07:10:40 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 01 Mar 2023 07:10:44 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 07:10:44 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 01 Mar 2023 07:11:03 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 01 Mar 2023 07:11:03 GMT
VOLUME [/spiped]
# Wed, 01 Mar 2023 07:11:03 GMT
WORKDIR /spiped
# Wed, 01 Mar 2023 07:11:03 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 01 Mar 2023 07:11:03 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 01 Mar 2023 07:11:04 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:3c3af56dbec5913ef8aec0f1ca7112eb5914b4ad346ccd48f836dd7ec0621ba5`  
		Last Modified: Wed, 01 Mar 2023 01:52:57 GMT  
		Size: 28.9 MB (28915776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9aca7d992b566279fbac9ecdeffb9ff2db68cf1ffd6f31a2cce852311c28c5ce`  
		Last Modified: Wed, 01 Mar 2023 07:11:20 GMT  
		Size: 1.7 KB (1728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fc3eb64d155ea643dfc7dde1104693192a95033b812f1cf66e286245705de6f`  
		Last Modified: Wed, 01 Mar 2023 07:11:20 GMT  
		Size: 1.1 KB (1050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9169ad29c4b57b416977f34e4cae1ad9b4efb6110e2a150a7cb43b7eab0da3d3`  
		Last Modified: Wed, 01 Mar 2023 07:11:21 GMT  
		Size: 5.0 MB (5028368 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:742f87e7cb263314cfe9b69a92b5fef45b368e04c178942b699311a03503e14c`  
		Last Modified: Wed, 01 Mar 2023 07:11:20 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0dfe2f008531a4616c872689c583cd0c8468b2fb60b07981fc0e20a80f84497`  
		Last Modified: Wed, 01 Mar 2023 07:11:20 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; arm variant v7

```console
$ docker pull spiped@sha256:627d305c141756ae7f1d3ce8a13ed19b5de3d5e5cc05419c57ca52a7cfad3e38
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.3 MB (31329572 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:80590efa308da9fa53e6713503023d50cdbb6bed46e6565e7a173368c94a3398`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 01 Mar 2023 01:57:55 GMT
ADD file:182fe91b8976a8871aba0d2ff9d4400a60317c8dec282261ba94247500c8d3dc in / 
# Wed, 01 Mar 2023 01:57:55 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 16:59:36 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 01 Mar 2023 16:59:39 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 16:59:39 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 01 Mar 2023 17:00:00 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 01 Mar 2023 17:00:00 GMT
VOLUME [/spiped]
# Wed, 01 Mar 2023 17:00:00 GMT
WORKDIR /spiped
# Wed, 01 Mar 2023 17:00:00 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 01 Mar 2023 17:00:00 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 01 Mar 2023 17:00:00 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:b4770fcf2ef78c1e46693da734476bfaf03cbe1d0b6e0a0f22c2c2e53419e803`  
		Last Modified: Wed, 01 Mar 2023 02:03:02 GMT  
		Size: 26.6 MB (26577290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe9ae4c200b12f57c7a99dbe5cd058c0c8e834ab0e042072df6f3ba0e2ef370b`  
		Last Modified: Wed, 01 Mar 2023 17:00:40 GMT  
		Size: 1.7 KB (1728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5dd24a9c965643a04effdcd9b7b20069af323b31c98f25e7ed41120a81c07cc`  
		Last Modified: Wed, 01 Mar 2023 17:00:40 GMT  
		Size: 1.1 KB (1051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0dba42d16068e44c779a0a9402aca488c2ae655c6d1c8fb07e88c3d68190a68b`  
		Last Modified: Wed, 01 Mar 2023 17:00:41 GMT  
		Size: 4.7 MB (4749033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c895f59fed0503b2299b019d207a580b45874b387ef1a68a3f08902c66676b63`  
		Last Modified: Wed, 01 Mar 2023 17:00:40 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f62eaf16d3dbd860a6214d912a6da95cacab5eaf97a19518ccf6c3ec0c774b0`  
		Last Modified: Wed, 01 Mar 2023 17:00:40 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:c0ee27c170b5818d26dd2679b9f68fbd1717c2b8029be42c1f19b7a9d582c867
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.3 MB (35338707 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f09e879bddede08a1bc165d3efa6587de5e8610534659bd12411ed41795ba246`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 01 Mar 2023 02:20:39 GMT
ADD file:9dc5c6fb6431df80107eddb76fb18256d6f4a06b4b22f9a7c4bcd58476068186 in / 
# Wed, 01 Mar 2023 02:20:39 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 14:07:19 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 01 Mar 2023 14:07:22 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 14:07:22 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 01 Mar 2023 14:07:37 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 01 Mar 2023 14:07:37 GMT
VOLUME [/spiped]
# Wed, 01 Mar 2023 14:07:37 GMT
WORKDIR /spiped
# Wed, 01 Mar 2023 14:07:37 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 01 Mar 2023 14:07:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 01 Mar 2023 14:07:38 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:66dbba0fb1b568cc3ffd53409ba2f9f82995ab7f80e379338f3f36e4dcd223be`  
		Last Modified: Wed, 01 Mar 2023 02:24:17 GMT  
		Size: 30.1 MB (30062814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:261024cf523923721d856c4f6e77a37c041d87ad2d3b4ccd92fb53f3abaab41f`  
		Last Modified: Wed, 01 Mar 2023 14:07:53 GMT  
		Size: 1.7 KB (1738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fe92519b62d1a9b8e2d52510cf1bf885ff477e0383a53bd4ee6a4efb5f3c14e`  
		Last Modified: Wed, 01 Mar 2023 14:07:53 GMT  
		Size: 1.1 KB (1051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a212b6d6d17e0b6cad09fb9cb67db006696d183039d38e32013a5fc3c0afb160`  
		Last Modified: Wed, 01 Mar 2023 14:07:54 GMT  
		Size: 5.3 MB (5272635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa9945ac00fd76d0a06763ef812f442fd4bb8aa3a67db027da1597a25f1e77aa`  
		Last Modified: Wed, 01 Mar 2023 14:07:53 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9fdec150625f76667b7ba6e9417519bf4f6d92c140125d060a1efb39e391342`  
		Last Modified: Wed, 01 Mar 2023 14:07:53 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; 386

```console
$ docker pull spiped@sha256:74d7f5c8f3f3d9c67ac2694a397c85180e9414b6092e41e394b39054f2029c92
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.3 MB (40291472 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cd42d521cfced48016618daf00f5e6976442656bf9c4005a7c8200ef734bcbd4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 23 Mar 2023 00:39:18 GMT
ADD file:315d843eefd4a8bb2345366dcd6bab00a06fca4a7970e220ae8946123d07d7ed in / 
# Thu, 23 Mar 2023 00:39:19 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 12:10:30 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Thu, 23 Mar 2023 12:10:33 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 12:10:33 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 23 Mar 2023 12:10:56 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 23 Mar 2023 12:10:56 GMT
VOLUME [/spiped]
# Thu, 23 Mar 2023 12:10:56 GMT
WORKDIR /spiped
# Thu, 23 Mar 2023 12:10:56 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 23 Mar 2023 12:10:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Mar 2023 12:10:57 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:3e638a975ea99fe8646002726dcb1ccdccc49ad33967b30337b9b2413e0619b5`  
		Last Modified: Thu, 23 Mar 2023 00:43:09 GMT  
		Size: 32.4 MB (32396277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8c70cbb4c8fd8326cfa3a38bcadaebdcf624fcd76381d57288eb687694073d1`  
		Last Modified: Thu, 23 Mar 2023 12:11:11 GMT  
		Size: 1.7 KB (1725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b85e36913d82a6dadb0781c7ab440ef652976cc8995f5f0a0bd0541b9b620373`  
		Last Modified: Thu, 23 Mar 2023 12:11:11 GMT  
		Size: 1.1 KB (1054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bec8a50af228e59f346840b516f8f52a3b22b0be6d31a71d1341b272cc16d2ad`  
		Last Modified: Thu, 23 Mar 2023 12:11:13 GMT  
		Size: 7.9 MB (7891948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af275a5a028f320d08a155a1238d5121d8a0198cebf123d479cfab9a01aafd10`  
		Last Modified: Thu, 23 Mar 2023 12:11:11 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:409fcb43c7b4c77abd48e9757bd49eadd9c1aade55294cd9145e4f451a2a7a75`  
		Last Modified: Thu, 23 Mar 2023 12:11:11 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; mips64le

```console
$ docker pull spiped@sha256:4b768c4a74571ecb307ea7f2c6f0d5444219c4f7701ca7ece08073134a9817c7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.3 MB (35342762 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:60d987426dc913c9b10892ddd45cd5d0cb2f8311fd0e994196056e11189abf9e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 01 Mar 2023 02:10:54 GMT
ADD file:0bcd66a6a099cdb6e018ddc0f00270be93dccd3be6167ce36e9efc99c31549d9 in / 
# Wed, 01 Mar 2023 02:10:59 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 13:56:50 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 01 Mar 2023 13:57:04 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 13:57:07 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 01 Mar 2023 13:58:36 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 01 Mar 2023 13:58:39 GMT
VOLUME [/spiped]
# Wed, 01 Mar 2023 13:58:42 GMT
WORKDIR /spiped
# Wed, 01 Mar 2023 13:58:44 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 01 Mar 2023 13:58:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 01 Mar 2023 13:58:49 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:89f6b45a7afd174bf0d443156831cacd9e6a26c834ad62610b6db53c731d257f`  
		Last Modified: Wed, 01 Mar 2023 02:18:50 GMT  
		Size: 29.6 MB (29634488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d10af42af1cddee9f8d002cb64f604273d7fd56c39403c8ecb2ca86ae445b2ac`  
		Last Modified: Wed, 01 Mar 2023 13:59:02 GMT  
		Size: 1.6 KB (1614 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da6cf49bc572eb473177215ee0a0e9187f04a782706a0d2a362817c62e3e4c1c`  
		Last Modified: Wed, 01 Mar 2023 13:59:03 GMT  
		Size: 928.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:030a52e1972e6a16de35f2c209c9fe8b1b7b677e38894c831863d54f0f1d6cfa`  
		Last Modified: Wed, 01 Mar 2023 13:59:07 GMT  
		Size: 5.7 MB (5705294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8eeca73463248c240d686d1c65ee25f2d27dd86f1920c0ab13f7974cd43b0d51`  
		Last Modified: Wed, 01 Mar 2023 13:59:03 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3867f0e8bddd40c5ae56a42d561c19e9e6c3520d9bb3a19c4ee8e10b5e35a76a`  
		Last Modified: Wed, 01 Mar 2023 13:59:02 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; ppc64le

```console
$ docker pull spiped@sha256:5eeeda056f21e90509214894b25b29c2f077d779e3a9894d7239c7c5b1dde12d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.3 MB (41291034 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2af8e0b52e04e9db1d381ffa1800979e5bb8de9720068f9bb1b0598a7198df6e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 01 Mar 2023 04:47:33 GMT
ADD file:6fdf0b2f8ea4be2d01e25a9d85db8f8c7e3b2a641c9c7665e34f4fad771815e0 in / 
# Wed, 01 Mar 2023 04:47:35 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 14:40:08 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 01 Mar 2023 14:40:14 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 14:40:15 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 01 Mar 2023 14:41:05 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 01 Mar 2023 14:41:06 GMT
VOLUME [/spiped]
# Wed, 01 Mar 2023 14:41:06 GMT
WORKDIR /spiped
# Wed, 01 Mar 2023 14:41:07 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 01 Mar 2023 14:41:07 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 01 Mar 2023 14:41:08 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:93ab3a60c2a8cbc1150cb2bd54222db8b79c525c0243534a10d6294ef7ff83ac`  
		Last Modified: Wed, 01 Mar 2023 04:53:54 GMT  
		Size: 35.3 MB (35288103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0a2080116d00583c373f079b8f40c2fa202cfaa894e5646b928e2f519bc8d0e`  
		Last Modified: Wed, 01 Mar 2023 14:41:39 GMT  
		Size: 1.7 KB (1734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6c05e885d8e0e269f3910fa5c387e4bfe94b5f5844a929e3f2945347c9bc33a`  
		Last Modified: Wed, 01 Mar 2023 14:41:39 GMT  
		Size: 1.1 KB (1055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f9c9a00d487b5d63eb533652fd7c8bbcaf5b4a766b8f50698468f313ea58b31`  
		Last Modified: Wed, 01 Mar 2023 14:41:41 GMT  
		Size: 6.0 MB (5999671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5ffd618016f8cd2101168350b00bdbad7932215a46cddd3c1abc7a1efdf9834`  
		Last Modified: Wed, 01 Mar 2023 14:41:39 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed01129e03be3daf248d482853655a906b1f3e7594b351c1d568f69c46c410ac`  
		Last Modified: Wed, 01 Mar 2023 14:41:39 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; s390x

```console
$ docker pull spiped@sha256:5052a882da69e191760a75d37205ff0a1edd8edf21ae507a22d93c6b1672215a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.8 MB (34837546 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4be5954f5bff77d2a4e04836cc5938d850a56e7ee023f169242f1226e121a558`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 23 Mar 2023 00:44:06 GMT
ADD file:8b6d3f57adaa8af2e0599a6468c50b713d281165b4e61150850bedf587f7ad4f in / 
# Thu, 23 Mar 2023 00:44:08 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 12:15:46 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Thu, 23 Mar 2023 12:15:49 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 12:15:49 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 23 Mar 2023 12:16:07 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 23 Mar 2023 12:16:08 GMT
VOLUME [/spiped]
# Thu, 23 Mar 2023 12:16:08 GMT
WORKDIR /spiped
# Thu, 23 Mar 2023 12:16:08 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 23 Mar 2023 12:16:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Mar 2023 12:16:09 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:25d08e051bb75230bad82e3a7a054083beec6b4f6a46c8345c731582c297a408`  
		Last Modified: Thu, 23 Mar 2023 00:47:20 GMT  
		Size: 29.6 MB (29646820 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3388e32dd1b77d93d6b62ba801fb658ac69c6eebde8b030476caac13f83542be`  
		Last Modified: Thu, 23 Mar 2023 12:16:29 GMT  
		Size: 1.7 KB (1736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a701ac09c5ac118d050e81f6139936da77a346003315c4444e1939a6b9fbf5a`  
		Last Modified: Thu, 23 Mar 2023 12:16:29 GMT  
		Size: 1.1 KB (1050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76c28eecb90a4ce4306f2ee104c3b7a26ed907a1d7b4ffe9ee9f404860df7d2f`  
		Last Modified: Thu, 23 Mar 2023 12:16:30 GMT  
		Size: 5.2 MB (5187470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:851271a85236c408b9e2df7b62a45c37bc5552fb05fc8fb30a87d4f40e207d26`  
		Last Modified: Thu, 23 Mar 2023 12:16:29 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30749340374b1df790439fe4c7b71b610b3d0ae3aef3705de18f2472f5933c06`  
		Last Modified: Thu, 23 Mar 2023 12:16:29 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:1.6-alpine`

```console
$ docker pull spiped@sha256:dfaf6e7592d4ab323a62d1b401cab7d35cab87afdb70fe94fc8d2c41d99aca33
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
$ docker pull spiped@sha256:b02340eb97482a93ed8c3997880473f27309e7362e27d06bfbdeb686da9f835f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.1 MB (5080754 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1660f13550a5bd6ce0ec142f4dc1325092450163ee42f52b56572854d7e8c1e3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Sat, 11 Feb 2023 04:46:42 GMT
ADD file:40887ab7c06977737e63c215c9bd297c0c74de8d12d16ebdf1c3d40ac392f62d in / 
# Sat, 11 Feb 2023 04:46:42 GMT
CMD ["/bin/sh"]
# Sat, 11 Feb 2023 14:04:29 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Sat, 11 Feb 2023 14:04:30 GMT
RUN apk add --no-cache libssl1.1
# Sat, 11 Feb 2023 14:04:30 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Sat, 11 Feb 2023 14:04:41 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Sat, 11 Feb 2023 14:04:41 GMT
VOLUME [/spiped]
# Sat, 11 Feb 2023 14:04:41 GMT
WORKDIR /spiped
# Sat, 11 Feb 2023 14:04:41 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 11 Feb 2023 14:04:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 11 Feb 2023 14:04:41 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:63b65145d645c1250c391b2d16ebe53b3747c295ca8ba2fcb6b0cf064a4dc21c`  
		Last Modified: Fri, 10 Feb 2023 22:41:31 GMT  
		Size: 3.4 MB (3374446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1567e533de4a753157026d7ef2c42cfa5f9efd21e25cc7370e4c8f1c8f1c8a47`  
		Last Modified: Sat, 11 Feb 2023 14:04:56 GMT  
		Size: 1.3 KB (1267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1a1fcb595374972f69b5a50bd54f62b80c9214b0f891c62726a3fb6853cf855`  
		Last Modified: Sat, 11 Feb 2023 14:04:56 GMT  
		Size: 1.5 MB (1483289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24f4efb6e81c911655772824a287a9f39d90e069841b4fe5601933b9b0ffe154`  
		Last Modified: Sat, 11 Feb 2023 14:04:56 GMT  
		Size: 221.3 KB (221282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:981056191296cd6f887bc7d5e8e078e1cec12690bc7fc8623b868e6b4023e0ea`  
		Last Modified: Sat, 11 Feb 2023 14:04:56 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:577ef58b3b8b045fa02bbbbd599b6c9d4310c0039e442d91e549dad4f7e556fd`  
		Last Modified: Sat, 11 Feb 2023 14:04:56 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; arm variant v6

```console
$ docker pull spiped@sha256:76a36336fb4a148684ae27104022667db149e7b75e602fb0d1fb636cb8277330
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.6 MB (4559988 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8148101a55ef329eee778b51e7674409dd7530f66643e375f5eaf15450e8d364`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Mon, 13 Mar 2023 16:12:44 GMT
ADD file:d825d9aef59df0df23c0140a490998407ee0a62a051699b5c050aef7cb03f042 in / 
# Mon, 13 Mar 2023 16:12:44 GMT
CMD ["/bin/sh"]
# Tue, 14 Mar 2023 01:30:23 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Tue, 14 Mar 2023 01:30:24 GMT
RUN apk add --no-cache libssl1.1
# Tue, 14 Mar 2023 01:30:24 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 14 Mar 2023 01:30:32 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Tue, 14 Mar 2023 01:30:32 GMT
VOLUME [/spiped]
# Tue, 14 Mar 2023 01:30:32 GMT
WORKDIR /spiped
# Tue, 14 Mar 2023 01:30:32 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 14 Mar 2023 01:30:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 14 Mar 2023 01:30:32 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:6a6e4ab63e54442e16400f69d37f662d60cbd67565631eff6bf59b4176e482c3`  
		Last Modified: Fri, 10 Feb 2023 20:50:22 GMT  
		Size: 3.1 MB (3110885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e45faa3e84504ff194d07161781bbb3d65ced006b3559fdd50974ca59bede67b`  
		Last Modified: Tue, 14 Mar 2023 01:30:48 GMT  
		Size: 1.3 KB (1271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a49b678821973054e204d328f8a1abfd5c4d0babdc516e24b56c76cc2adbd596`  
		Last Modified: Tue, 14 Mar 2023 01:30:49 GMT  
		Size: 1.2 MB (1240997 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8dbbba3d131edbec32d7ac2251201ab33e79abc9994b4e0635fac27365f1579f`  
		Last Modified: Tue, 14 Mar 2023 01:30:49 GMT  
		Size: 206.4 KB (206366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f344f34fb34133bb7a416417587f8f9219c749343ba309ab724c2dba1c4653c3`  
		Last Modified: Tue, 14 Mar 2023 01:30:48 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8506930f7b522732a72fca7395d31bb8094739139324468e7ae618b1da4d3cda`  
		Last Modified: Tue, 14 Mar 2023 01:30:48 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; arm variant v7

```console
$ docker pull spiped@sha256:361539f7f9277859ba382de7be4afe676210140f53c3c5cd85d5ae3985f905c0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4237927 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2e899581be5421f50eb7e6339c7512ab16c114d8213f09e8aca52c68f0bcc311`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 10 Feb 2023 21:51:31 GMT
ADD file:143b601fcc6b5d7d95d3e5ccad3fec7081191a47e28d4f9294a7fb2499cab1af in / 
# Fri, 10 Feb 2023 21:51:31 GMT
CMD ["/bin/sh"]
# Wed, 01 Mar 2023 17:00:05 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Wed, 01 Mar 2023 17:00:07 GMT
RUN apk add --no-cache libssl1.1
# Wed, 01 Mar 2023 17:00:07 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 01 Mar 2023 17:00:14 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Wed, 01 Mar 2023 17:00:14 GMT
VOLUME [/spiped]
# Wed, 01 Mar 2023 17:00:14 GMT
WORKDIR /spiped
# Wed, 01 Mar 2023 17:00:14 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 01 Mar 2023 17:00:14 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 01 Mar 2023 17:00:15 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:6fb81ff47bd6d7db0ed86c9b951ad6417ec73ab60af6d22daa604076a902629c`  
		Last Modified: Fri, 10 Feb 2023 21:52:33 GMT  
		Size: 2.9 MB (2868494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bcf9acc5eeca77f6d435380f4f1fea53c3643c4cc9042daf13fdd9b6b72d9f5`  
		Last Modified: Wed, 01 Mar 2023 17:00:57 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f34e65da889251051ec9481b5d6cb0d428c45c8861fb2948b0c38c07470bba59`  
		Last Modified: Wed, 01 Mar 2023 17:00:57 GMT  
		Size: 1.2 MB (1167579 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0412dc4bafb0f9dabcfd28a3c0b4454de2db5c81112fdbb51bf5c883f4a6925`  
		Last Modified: Wed, 01 Mar 2023 17:00:57 GMT  
		Size: 200.1 KB (200120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70011259fd33df6da621cfb9142329c3c7a89b4bc5bfe91a87f7335995930ff9`  
		Last Modified: Wed, 01 Mar 2023 17:00:57 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99d3fd9f335e89a8501d7008f1bbaf813f4a5b26227452ecfc0001613be1ee7f`  
		Last Modified: Wed, 01 Mar 2023 17:00:57 GMT  
		Size: 337.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:b202c4e5897cb771f303b85871c6b7a1fb5f025c51e651b30a4415f0e2e4973d
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.8 MB (4842933 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6c3a0f714da4f343e79de4855fa4cdc4a23892d7fe5654dec6710bc79bb2cc2c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 10 Feb 2023 21:24:08 GMT
ADD file:9bd9ea42a9f3bdc769e80c6b8a4b117d65f73ae68e155a6172a1184e7ac8bcc1 in / 
# Fri, 10 Feb 2023 21:24:08 GMT
CMD ["/bin/sh"]
# Sat, 11 Feb 2023 06:39:43 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Sat, 11 Feb 2023 06:39:44 GMT
RUN apk add --no-cache libssl1.1
# Sat, 11 Feb 2023 06:39:44 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Sat, 11 Feb 2023 06:39:52 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Sat, 11 Feb 2023 06:39:52 GMT
VOLUME [/spiped]
# Sat, 11 Feb 2023 06:39:52 GMT
WORKDIR /spiped
# Sat, 11 Feb 2023 06:39:52 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 11 Feb 2023 06:39:52 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 11 Feb 2023 06:39:52 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:af6eaf76a39c2d3e7e0b8a0420486e3df33c4027d696c076a99a3d0ac09026af`  
		Last Modified: Fri, 10 Feb 2023 21:24:39 GMT  
		Size: 3.3 MB (3261959 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32e706a54c37c1524628e434965039ac738ff48a6f151dd2ef6da2cb49958cc0`  
		Last Modified: Sat, 11 Feb 2023 06:40:07 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e99781ddd302da37630cc491b5190c39c7867e6bd96556fad9f613e3411bca0d`  
		Last Modified: Sat, 11 Feb 2023 06:40:07 GMT  
		Size: 1.4 MB (1363548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:768a1af5c81e5cc877ea8cb330527a3924d5f2b5acfc5dd8239f84fdf091e5ed`  
		Last Modified: Sat, 11 Feb 2023 06:40:07 GMT  
		Size: 215.7 KB (215691 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7567bda17775002440a508f6ff25154cb13c9201175281b80186ce38d44e2b7`  
		Last Modified: Sat, 11 Feb 2023 06:40:07 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba17a7f3c3024db40a3e0b478318d1eb5168af1437c2bd502fb302591b78f95a`  
		Last Modified: Sat, 11 Feb 2023 06:40:07 GMT  
		Size: 338.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; 386

```console
$ docker pull spiped@sha256:1718408d282e2785554de5dd41b1935a8fd740cad6fa42ddeac2fafad4e15148
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.1 MB (5131990 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e81769d87082a52703eb2f30d09dbe3c289d1e6956af04796da66cf8ec2e5a5b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 10 Feb 2023 21:24:23 GMT
ADD file:125f3514520a5cd29df2830a409aa026a2bc06a77a7a5d150133436404b33d41 in / 
# Fri, 10 Feb 2023 21:24:24 GMT
CMD ["/bin/sh"]
# Wed, 01 Mar 2023 20:35:30 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Wed, 01 Mar 2023 20:35:32 GMT
RUN apk add --no-cache libssl1.1
# Wed, 01 Mar 2023 20:35:32 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 01 Mar 2023 20:35:44 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Wed, 01 Mar 2023 20:35:44 GMT
VOLUME [/spiped]
# Wed, 01 Mar 2023 20:35:44 GMT
WORKDIR /spiped
# Wed, 01 Mar 2023 20:35:44 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 01 Mar 2023 20:35:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 01 Mar 2023 20:35:44 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:b3e346c15c2377ec0e75cc9efa98baecd58b0e9bb92f0ec07eeda0bcc7e67fc7`  
		Last Modified: Fri, 10 Feb 2023 21:25:13 GMT  
		Size: 3.4 MB (3412353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9ddea08df82e419c862a82c04a7b6027073e509f79247aaab6fcb9a2d66e4bc`  
		Last Modified: Wed, 01 Mar 2023 20:36:27 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7baff4523d8b5b8d72311936f6b35a74dc61f50af8ceb150e8a464755ed3ff76`  
		Last Modified: Wed, 01 Mar 2023 20:36:27 GMT  
		Size: 1.5 MB (1486288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de00b81755546779184cb3998ef43c5c0445cd5871998c7feb92240ab36aeb5e`  
		Last Modified: Wed, 01 Mar 2023 20:36:27 GMT  
		Size: 231.6 KB (231613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:568814bee4cca693df73f2ed16adcc10335f014f7606b67b33d08c3abf12b51a`  
		Last Modified: Wed, 01 Mar 2023 20:36:27 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da028d97e3da3f51bb23a54f50dc51e00a905208ac487c94ae446e20f926b63c`  
		Last Modified: Wed, 01 Mar 2023 20:36:27 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; ppc64le

```console
$ docker pull spiped@sha256:75c7e8ce27d4c68e8862a8e832409e09dbeb2c47fa2163ac0ac7f4e794b6b14c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.0 MB (5025550 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:523cfab6c09a42cd9174ca6dee237febe2f4a72f0c07628ccddab56278968150`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 10 Feb 2023 21:20:36 GMT
ADD file:ec037a0d4b462d12963ac20d9ec49bb73b4bcaf84d4bc7b364ebf93667e585b0 in / 
# Fri, 10 Feb 2023 21:20:36 GMT
CMD ["/bin/sh"]
# Sat, 11 Feb 2023 09:33:46 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Sat, 11 Feb 2023 09:33:49 GMT
RUN apk add --no-cache libssl1.1
# Sat, 11 Feb 2023 09:33:50 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Sat, 11 Feb 2023 09:34:04 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Sat, 11 Feb 2023 09:34:04 GMT
VOLUME [/spiped]
# Sat, 11 Feb 2023 09:34:05 GMT
WORKDIR /spiped
# Sat, 11 Feb 2023 09:34:05 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 11 Feb 2023 09:34:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 11 Feb 2023 09:34:06 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:aa3c56f9c6f127b6c8f628c95db165741ca400d19bdaef2752d80f093e47451e`  
		Last Modified: Fri, 10 Feb 2023 21:21:37 GMT  
		Size: 3.4 MB (3390750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b5d50df2303841e19f748472d51fac8d0695468f1d50516484905b50450aa48`  
		Last Modified: Sat, 11 Feb 2023 09:34:31 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0b54432b9107e6d87810bd116ab5112e27a1f713d4d2c06525f0ed14f102e3c`  
		Last Modified: Sat, 11 Feb 2023 09:34:32 GMT  
		Size: 1.4 MB (1413040 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4bda8ea646857e9e3d0c92c042261af7dba424338abfc7cc1c58eec7b8985be`  
		Last Modified: Sat, 11 Feb 2023 09:34:32 GMT  
		Size: 220.0 KB (220021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e33bc423b9fd5cc84d66be2c92fc2c78368e9b5553d8c6848fab3570115fb66`  
		Last Modified: Sat, 11 Feb 2023 09:34:31 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53a89c5ec31eae84c318581d292f2fdc24ec49bc7692940d54b3b579b04cd2d6`  
		Last Modified: Sat, 11 Feb 2023 09:34:31 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; s390x

```console
$ docker pull spiped@sha256:c224a59dd171160cb9e3b3be6bac31704ad968f23bed4f4f8ae4d04d938951c6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.6 MB (4608839 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:88032fe647cd1b9c54c93549e3978f1e53d8c0df71f2c0c2660b0545fc0b7ae3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 10 Feb 2023 21:41:25 GMT
ADD file:03b2fb4d732a294329449ff55c5d84f7d2735e6510985718979469994f3a607b in / 
# Fri, 10 Feb 2023 21:41:26 GMT
CMD ["/bin/sh"]
# Sat, 11 Feb 2023 05:20:31 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Sat, 11 Feb 2023 05:20:32 GMT
RUN apk add --no-cache libssl1.1
# Sat, 11 Feb 2023 05:20:33 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Sat, 11 Feb 2023 05:20:38 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Sat, 11 Feb 2023 05:20:38 GMT
VOLUME [/spiped]
# Sat, 11 Feb 2023 05:20:38 GMT
WORKDIR /spiped
# Sat, 11 Feb 2023 05:20:39 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 11 Feb 2023 05:20:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 11 Feb 2023 05:20:39 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:24c4f8de3549a39c64b0edc2cfa68769b373f35138d0f13725100160bb32d4e2`  
		Last Modified: Fri, 10 Feb 2023 21:42:16 GMT  
		Size: 3.2 MB (3175116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdb5c0ff1110b4315355f81e38de10bb31ba9fe44d99d3b7598f20a28f2c98e1`  
		Last Modified: Sat, 11 Feb 2023 05:21:04 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9ac27252903c2b21737926a9cd0721ecfa3aba4f2e52da7f7c114aea4da62df`  
		Last Modified: Sat, 11 Feb 2023 05:21:04 GMT  
		Size: 1.2 MB (1223356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df30f40ce9a4931562f50ea55d6450396fd443fed95a0b2c0ea337f53f22ec25`  
		Last Modified: Sat, 11 Feb 2023 05:21:04 GMT  
		Size: 208.6 KB (208631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d9420167a9c04b73e787d02b0fa09ba21ff8b27917d0406146f9bc5a0df3034`  
		Last Modified: Sat, 11 Feb 2023 05:21:04 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea129f4350d878551c457a2192ea0570f86ca7ee5c193a6b0d8e19727570f05b`  
		Last Modified: Sat, 11 Feb 2023 05:21:04 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:1.6.2`

```console
$ docker pull spiped@sha256:3f946d80813d27b67a12c1f37671961b9dafebeaa779ab08875cf6daa5ad8ed2
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
$ docker pull spiped@sha256:027c9e8b16fd5686f2386e10f4efea51d2cf9baf4e7bcdaf3c1fb979d3d6e6c2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.4 MB (37412991 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:803eb276e1835de8624a0705f68be4b52442d62ad95ad7f8933b8a2f1dfe7a40`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 01 Mar 2023 04:09:58 GMT
ADD file:493a5b0c8d2d63a1343258b3f9aa5fcd59a93f44fe26ad9e56b094c3a08fd3be in / 
# Wed, 01 Mar 2023 04:09:59 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 17:55:56 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 01 Mar 2023 17:55:59 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 17:55:59 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 01 Mar 2023 17:56:20 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 01 Mar 2023 17:56:20 GMT
VOLUME [/spiped]
# Wed, 01 Mar 2023 17:56:20 GMT
WORKDIR /spiped
# Wed, 01 Mar 2023 17:56:20 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 01 Mar 2023 17:56:20 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 01 Mar 2023 17:56:20 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:3f9582a2cbe7197f39185419c0ced2c986389f8fc6aa805e1f5c090eea6511e0`  
		Last Modified: Wed, 01 Mar 2023 04:14:23 GMT  
		Size: 31.4 MB (31411403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e97821d2ff040682a3d9356a04d84b72255c563d7603f7219e6ed9e7c0e80e3`  
		Last Modified: Wed, 01 Mar 2023 17:56:35 GMT  
		Size: 1.7 KB (1733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97f3106ca46ab6b0eb674057029e3469fb737549c0e17f93501a7baa91ee7d66`  
		Last Modified: Wed, 01 Mar 2023 17:56:34 GMT  
		Size: 1.1 KB (1054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22be67cd1cbaef6c42eaf8be1eccae8272262dbf3e2ff498e0c4ce7de42750df`  
		Last Modified: Wed, 01 Mar 2023 17:56:36 GMT  
		Size: 6.0 MB (5998329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ededc4cf18635cc66d453c3af24a583d4f300aa916b5d12a5e3622c70bb9a86b`  
		Last Modified: Wed, 01 Mar 2023 17:56:35 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2631603d11fd9110672446c8a343410ea67a502e725c014b4e1f83f522b56904`  
		Last Modified: Wed, 01 Mar 2023 17:56:35 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.2` - linux; arm variant v5

```console
$ docker pull spiped@sha256:528e13ba139adf0768024a80cfc79ab5cb3d0ea5e8f9b9f3bc1511f2d698c215
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.9 MB (33947393 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5a1e48f7b0e65652cca9ca80196c861d383ac1f1b0103cc512be95efd00fc6e9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 01 Mar 2023 01:48:54 GMT
ADD file:b4fb1081f6eb8a0560d56d5781bbcedaac1453615d56e0943245dca784785ea2 in / 
# Wed, 01 Mar 2023 01:48:54 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 07:10:40 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 01 Mar 2023 07:10:44 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 07:10:44 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 01 Mar 2023 07:11:03 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 01 Mar 2023 07:11:03 GMT
VOLUME [/spiped]
# Wed, 01 Mar 2023 07:11:03 GMT
WORKDIR /spiped
# Wed, 01 Mar 2023 07:11:03 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 01 Mar 2023 07:11:03 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 01 Mar 2023 07:11:04 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:3c3af56dbec5913ef8aec0f1ca7112eb5914b4ad346ccd48f836dd7ec0621ba5`  
		Last Modified: Wed, 01 Mar 2023 01:52:57 GMT  
		Size: 28.9 MB (28915776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9aca7d992b566279fbac9ecdeffb9ff2db68cf1ffd6f31a2cce852311c28c5ce`  
		Last Modified: Wed, 01 Mar 2023 07:11:20 GMT  
		Size: 1.7 KB (1728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fc3eb64d155ea643dfc7dde1104693192a95033b812f1cf66e286245705de6f`  
		Last Modified: Wed, 01 Mar 2023 07:11:20 GMT  
		Size: 1.1 KB (1050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9169ad29c4b57b416977f34e4cae1ad9b4efb6110e2a150a7cb43b7eab0da3d3`  
		Last Modified: Wed, 01 Mar 2023 07:11:21 GMT  
		Size: 5.0 MB (5028368 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:742f87e7cb263314cfe9b69a92b5fef45b368e04c178942b699311a03503e14c`  
		Last Modified: Wed, 01 Mar 2023 07:11:20 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0dfe2f008531a4616c872689c583cd0c8468b2fb60b07981fc0e20a80f84497`  
		Last Modified: Wed, 01 Mar 2023 07:11:20 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.2` - linux; arm variant v7

```console
$ docker pull spiped@sha256:627d305c141756ae7f1d3ce8a13ed19b5de3d5e5cc05419c57ca52a7cfad3e38
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.3 MB (31329572 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:80590efa308da9fa53e6713503023d50cdbb6bed46e6565e7a173368c94a3398`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 01 Mar 2023 01:57:55 GMT
ADD file:182fe91b8976a8871aba0d2ff9d4400a60317c8dec282261ba94247500c8d3dc in / 
# Wed, 01 Mar 2023 01:57:55 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 16:59:36 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 01 Mar 2023 16:59:39 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 16:59:39 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 01 Mar 2023 17:00:00 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 01 Mar 2023 17:00:00 GMT
VOLUME [/spiped]
# Wed, 01 Mar 2023 17:00:00 GMT
WORKDIR /spiped
# Wed, 01 Mar 2023 17:00:00 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 01 Mar 2023 17:00:00 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 01 Mar 2023 17:00:00 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:b4770fcf2ef78c1e46693da734476bfaf03cbe1d0b6e0a0f22c2c2e53419e803`  
		Last Modified: Wed, 01 Mar 2023 02:03:02 GMT  
		Size: 26.6 MB (26577290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe9ae4c200b12f57c7a99dbe5cd058c0c8e834ab0e042072df6f3ba0e2ef370b`  
		Last Modified: Wed, 01 Mar 2023 17:00:40 GMT  
		Size: 1.7 KB (1728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5dd24a9c965643a04effdcd9b7b20069af323b31c98f25e7ed41120a81c07cc`  
		Last Modified: Wed, 01 Mar 2023 17:00:40 GMT  
		Size: 1.1 KB (1051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0dba42d16068e44c779a0a9402aca488c2ae655c6d1c8fb07e88c3d68190a68b`  
		Last Modified: Wed, 01 Mar 2023 17:00:41 GMT  
		Size: 4.7 MB (4749033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c895f59fed0503b2299b019d207a580b45874b387ef1a68a3f08902c66676b63`  
		Last Modified: Wed, 01 Mar 2023 17:00:40 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f62eaf16d3dbd860a6214d912a6da95cacab5eaf97a19518ccf6c3ec0c774b0`  
		Last Modified: Wed, 01 Mar 2023 17:00:40 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.2` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:c0ee27c170b5818d26dd2679b9f68fbd1717c2b8029be42c1f19b7a9d582c867
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.3 MB (35338707 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f09e879bddede08a1bc165d3efa6587de5e8610534659bd12411ed41795ba246`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 01 Mar 2023 02:20:39 GMT
ADD file:9dc5c6fb6431df80107eddb76fb18256d6f4a06b4b22f9a7c4bcd58476068186 in / 
# Wed, 01 Mar 2023 02:20:39 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 14:07:19 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 01 Mar 2023 14:07:22 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 14:07:22 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 01 Mar 2023 14:07:37 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 01 Mar 2023 14:07:37 GMT
VOLUME [/spiped]
# Wed, 01 Mar 2023 14:07:37 GMT
WORKDIR /spiped
# Wed, 01 Mar 2023 14:07:37 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 01 Mar 2023 14:07:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 01 Mar 2023 14:07:38 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:66dbba0fb1b568cc3ffd53409ba2f9f82995ab7f80e379338f3f36e4dcd223be`  
		Last Modified: Wed, 01 Mar 2023 02:24:17 GMT  
		Size: 30.1 MB (30062814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:261024cf523923721d856c4f6e77a37c041d87ad2d3b4ccd92fb53f3abaab41f`  
		Last Modified: Wed, 01 Mar 2023 14:07:53 GMT  
		Size: 1.7 KB (1738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fe92519b62d1a9b8e2d52510cf1bf885ff477e0383a53bd4ee6a4efb5f3c14e`  
		Last Modified: Wed, 01 Mar 2023 14:07:53 GMT  
		Size: 1.1 KB (1051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a212b6d6d17e0b6cad09fb9cb67db006696d183039d38e32013a5fc3c0afb160`  
		Last Modified: Wed, 01 Mar 2023 14:07:54 GMT  
		Size: 5.3 MB (5272635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa9945ac00fd76d0a06763ef812f442fd4bb8aa3a67db027da1597a25f1e77aa`  
		Last Modified: Wed, 01 Mar 2023 14:07:53 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9fdec150625f76667b7ba6e9417519bf4f6d92c140125d060a1efb39e391342`  
		Last Modified: Wed, 01 Mar 2023 14:07:53 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.2` - linux; 386

```console
$ docker pull spiped@sha256:74d7f5c8f3f3d9c67ac2694a397c85180e9414b6092e41e394b39054f2029c92
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.3 MB (40291472 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cd42d521cfced48016618daf00f5e6976442656bf9c4005a7c8200ef734bcbd4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 23 Mar 2023 00:39:18 GMT
ADD file:315d843eefd4a8bb2345366dcd6bab00a06fca4a7970e220ae8946123d07d7ed in / 
# Thu, 23 Mar 2023 00:39:19 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 12:10:30 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Thu, 23 Mar 2023 12:10:33 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 12:10:33 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 23 Mar 2023 12:10:56 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 23 Mar 2023 12:10:56 GMT
VOLUME [/spiped]
# Thu, 23 Mar 2023 12:10:56 GMT
WORKDIR /spiped
# Thu, 23 Mar 2023 12:10:56 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 23 Mar 2023 12:10:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Mar 2023 12:10:57 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:3e638a975ea99fe8646002726dcb1ccdccc49ad33967b30337b9b2413e0619b5`  
		Last Modified: Thu, 23 Mar 2023 00:43:09 GMT  
		Size: 32.4 MB (32396277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8c70cbb4c8fd8326cfa3a38bcadaebdcf624fcd76381d57288eb687694073d1`  
		Last Modified: Thu, 23 Mar 2023 12:11:11 GMT  
		Size: 1.7 KB (1725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b85e36913d82a6dadb0781c7ab440ef652976cc8995f5f0a0bd0541b9b620373`  
		Last Modified: Thu, 23 Mar 2023 12:11:11 GMT  
		Size: 1.1 KB (1054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bec8a50af228e59f346840b516f8f52a3b22b0be6d31a71d1341b272cc16d2ad`  
		Last Modified: Thu, 23 Mar 2023 12:11:13 GMT  
		Size: 7.9 MB (7891948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af275a5a028f320d08a155a1238d5121d8a0198cebf123d479cfab9a01aafd10`  
		Last Modified: Thu, 23 Mar 2023 12:11:11 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:409fcb43c7b4c77abd48e9757bd49eadd9c1aade55294cd9145e4f451a2a7a75`  
		Last Modified: Thu, 23 Mar 2023 12:11:11 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.2` - linux; mips64le

```console
$ docker pull spiped@sha256:4b768c4a74571ecb307ea7f2c6f0d5444219c4f7701ca7ece08073134a9817c7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.3 MB (35342762 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:60d987426dc913c9b10892ddd45cd5d0cb2f8311fd0e994196056e11189abf9e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 01 Mar 2023 02:10:54 GMT
ADD file:0bcd66a6a099cdb6e018ddc0f00270be93dccd3be6167ce36e9efc99c31549d9 in / 
# Wed, 01 Mar 2023 02:10:59 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 13:56:50 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 01 Mar 2023 13:57:04 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 13:57:07 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 01 Mar 2023 13:58:36 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 01 Mar 2023 13:58:39 GMT
VOLUME [/spiped]
# Wed, 01 Mar 2023 13:58:42 GMT
WORKDIR /spiped
# Wed, 01 Mar 2023 13:58:44 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 01 Mar 2023 13:58:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 01 Mar 2023 13:58:49 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:89f6b45a7afd174bf0d443156831cacd9e6a26c834ad62610b6db53c731d257f`  
		Last Modified: Wed, 01 Mar 2023 02:18:50 GMT  
		Size: 29.6 MB (29634488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d10af42af1cddee9f8d002cb64f604273d7fd56c39403c8ecb2ca86ae445b2ac`  
		Last Modified: Wed, 01 Mar 2023 13:59:02 GMT  
		Size: 1.6 KB (1614 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da6cf49bc572eb473177215ee0a0e9187f04a782706a0d2a362817c62e3e4c1c`  
		Last Modified: Wed, 01 Mar 2023 13:59:03 GMT  
		Size: 928.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:030a52e1972e6a16de35f2c209c9fe8b1b7b677e38894c831863d54f0f1d6cfa`  
		Last Modified: Wed, 01 Mar 2023 13:59:07 GMT  
		Size: 5.7 MB (5705294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8eeca73463248c240d686d1c65ee25f2d27dd86f1920c0ab13f7974cd43b0d51`  
		Last Modified: Wed, 01 Mar 2023 13:59:03 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3867f0e8bddd40c5ae56a42d561c19e9e6c3520d9bb3a19c4ee8e10b5e35a76a`  
		Last Modified: Wed, 01 Mar 2023 13:59:02 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.2` - linux; ppc64le

```console
$ docker pull spiped@sha256:5eeeda056f21e90509214894b25b29c2f077d779e3a9894d7239c7c5b1dde12d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.3 MB (41291034 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2af8e0b52e04e9db1d381ffa1800979e5bb8de9720068f9bb1b0598a7198df6e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 01 Mar 2023 04:47:33 GMT
ADD file:6fdf0b2f8ea4be2d01e25a9d85db8f8c7e3b2a641c9c7665e34f4fad771815e0 in / 
# Wed, 01 Mar 2023 04:47:35 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 14:40:08 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 01 Mar 2023 14:40:14 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 14:40:15 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 01 Mar 2023 14:41:05 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 01 Mar 2023 14:41:06 GMT
VOLUME [/spiped]
# Wed, 01 Mar 2023 14:41:06 GMT
WORKDIR /spiped
# Wed, 01 Mar 2023 14:41:07 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 01 Mar 2023 14:41:07 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 01 Mar 2023 14:41:08 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:93ab3a60c2a8cbc1150cb2bd54222db8b79c525c0243534a10d6294ef7ff83ac`  
		Last Modified: Wed, 01 Mar 2023 04:53:54 GMT  
		Size: 35.3 MB (35288103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0a2080116d00583c373f079b8f40c2fa202cfaa894e5646b928e2f519bc8d0e`  
		Last Modified: Wed, 01 Mar 2023 14:41:39 GMT  
		Size: 1.7 KB (1734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6c05e885d8e0e269f3910fa5c387e4bfe94b5f5844a929e3f2945347c9bc33a`  
		Last Modified: Wed, 01 Mar 2023 14:41:39 GMT  
		Size: 1.1 KB (1055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f9c9a00d487b5d63eb533652fd7c8bbcaf5b4a766b8f50698468f313ea58b31`  
		Last Modified: Wed, 01 Mar 2023 14:41:41 GMT  
		Size: 6.0 MB (5999671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5ffd618016f8cd2101168350b00bdbad7932215a46cddd3c1abc7a1efdf9834`  
		Last Modified: Wed, 01 Mar 2023 14:41:39 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed01129e03be3daf248d482853655a906b1f3e7594b351c1d568f69c46c410ac`  
		Last Modified: Wed, 01 Mar 2023 14:41:39 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.2` - linux; s390x

```console
$ docker pull spiped@sha256:5052a882da69e191760a75d37205ff0a1edd8edf21ae507a22d93c6b1672215a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.8 MB (34837546 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4be5954f5bff77d2a4e04836cc5938d850a56e7ee023f169242f1226e121a558`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 23 Mar 2023 00:44:06 GMT
ADD file:8b6d3f57adaa8af2e0599a6468c50b713d281165b4e61150850bedf587f7ad4f in / 
# Thu, 23 Mar 2023 00:44:08 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 12:15:46 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Thu, 23 Mar 2023 12:15:49 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 12:15:49 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 23 Mar 2023 12:16:07 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 23 Mar 2023 12:16:08 GMT
VOLUME [/spiped]
# Thu, 23 Mar 2023 12:16:08 GMT
WORKDIR /spiped
# Thu, 23 Mar 2023 12:16:08 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 23 Mar 2023 12:16:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Mar 2023 12:16:09 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:25d08e051bb75230bad82e3a7a054083beec6b4f6a46c8345c731582c297a408`  
		Last Modified: Thu, 23 Mar 2023 00:47:20 GMT  
		Size: 29.6 MB (29646820 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3388e32dd1b77d93d6b62ba801fb658ac69c6eebde8b030476caac13f83542be`  
		Last Modified: Thu, 23 Mar 2023 12:16:29 GMT  
		Size: 1.7 KB (1736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a701ac09c5ac118d050e81f6139936da77a346003315c4444e1939a6b9fbf5a`  
		Last Modified: Thu, 23 Mar 2023 12:16:29 GMT  
		Size: 1.1 KB (1050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76c28eecb90a4ce4306f2ee104c3b7a26ed907a1d7b4ffe9ee9f404860df7d2f`  
		Last Modified: Thu, 23 Mar 2023 12:16:30 GMT  
		Size: 5.2 MB (5187470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:851271a85236c408b9e2df7b62a45c37bc5552fb05fc8fb30a87d4f40e207d26`  
		Last Modified: Thu, 23 Mar 2023 12:16:29 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30749340374b1df790439fe4c7b71b610b3d0ae3aef3705de18f2472f5933c06`  
		Last Modified: Thu, 23 Mar 2023 12:16:29 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:1.6.2-alpine`

```console
$ docker pull spiped@sha256:dfaf6e7592d4ab323a62d1b401cab7d35cab87afdb70fe94fc8d2c41d99aca33
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
$ docker pull spiped@sha256:b02340eb97482a93ed8c3997880473f27309e7362e27d06bfbdeb686da9f835f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.1 MB (5080754 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1660f13550a5bd6ce0ec142f4dc1325092450163ee42f52b56572854d7e8c1e3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Sat, 11 Feb 2023 04:46:42 GMT
ADD file:40887ab7c06977737e63c215c9bd297c0c74de8d12d16ebdf1c3d40ac392f62d in / 
# Sat, 11 Feb 2023 04:46:42 GMT
CMD ["/bin/sh"]
# Sat, 11 Feb 2023 14:04:29 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Sat, 11 Feb 2023 14:04:30 GMT
RUN apk add --no-cache libssl1.1
# Sat, 11 Feb 2023 14:04:30 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Sat, 11 Feb 2023 14:04:41 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Sat, 11 Feb 2023 14:04:41 GMT
VOLUME [/spiped]
# Sat, 11 Feb 2023 14:04:41 GMT
WORKDIR /spiped
# Sat, 11 Feb 2023 14:04:41 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 11 Feb 2023 14:04:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 11 Feb 2023 14:04:41 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:63b65145d645c1250c391b2d16ebe53b3747c295ca8ba2fcb6b0cf064a4dc21c`  
		Last Modified: Fri, 10 Feb 2023 22:41:31 GMT  
		Size: 3.4 MB (3374446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1567e533de4a753157026d7ef2c42cfa5f9efd21e25cc7370e4c8f1c8f1c8a47`  
		Last Modified: Sat, 11 Feb 2023 14:04:56 GMT  
		Size: 1.3 KB (1267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1a1fcb595374972f69b5a50bd54f62b80c9214b0f891c62726a3fb6853cf855`  
		Last Modified: Sat, 11 Feb 2023 14:04:56 GMT  
		Size: 1.5 MB (1483289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24f4efb6e81c911655772824a287a9f39d90e069841b4fe5601933b9b0ffe154`  
		Last Modified: Sat, 11 Feb 2023 14:04:56 GMT  
		Size: 221.3 KB (221282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:981056191296cd6f887bc7d5e8e078e1cec12690bc7fc8623b868e6b4023e0ea`  
		Last Modified: Sat, 11 Feb 2023 14:04:56 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:577ef58b3b8b045fa02bbbbd599b6c9d4310c0039e442d91e549dad4f7e556fd`  
		Last Modified: Sat, 11 Feb 2023 14:04:56 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.2-alpine` - linux; arm variant v6

```console
$ docker pull spiped@sha256:76a36336fb4a148684ae27104022667db149e7b75e602fb0d1fb636cb8277330
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.6 MB (4559988 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8148101a55ef329eee778b51e7674409dd7530f66643e375f5eaf15450e8d364`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Mon, 13 Mar 2023 16:12:44 GMT
ADD file:d825d9aef59df0df23c0140a490998407ee0a62a051699b5c050aef7cb03f042 in / 
# Mon, 13 Mar 2023 16:12:44 GMT
CMD ["/bin/sh"]
# Tue, 14 Mar 2023 01:30:23 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Tue, 14 Mar 2023 01:30:24 GMT
RUN apk add --no-cache libssl1.1
# Tue, 14 Mar 2023 01:30:24 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 14 Mar 2023 01:30:32 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Tue, 14 Mar 2023 01:30:32 GMT
VOLUME [/spiped]
# Tue, 14 Mar 2023 01:30:32 GMT
WORKDIR /spiped
# Tue, 14 Mar 2023 01:30:32 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 14 Mar 2023 01:30:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 14 Mar 2023 01:30:32 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:6a6e4ab63e54442e16400f69d37f662d60cbd67565631eff6bf59b4176e482c3`  
		Last Modified: Fri, 10 Feb 2023 20:50:22 GMT  
		Size: 3.1 MB (3110885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e45faa3e84504ff194d07161781bbb3d65ced006b3559fdd50974ca59bede67b`  
		Last Modified: Tue, 14 Mar 2023 01:30:48 GMT  
		Size: 1.3 KB (1271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a49b678821973054e204d328f8a1abfd5c4d0babdc516e24b56c76cc2adbd596`  
		Last Modified: Tue, 14 Mar 2023 01:30:49 GMT  
		Size: 1.2 MB (1240997 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8dbbba3d131edbec32d7ac2251201ab33e79abc9994b4e0635fac27365f1579f`  
		Last Modified: Tue, 14 Mar 2023 01:30:49 GMT  
		Size: 206.4 KB (206366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f344f34fb34133bb7a416417587f8f9219c749343ba309ab724c2dba1c4653c3`  
		Last Modified: Tue, 14 Mar 2023 01:30:48 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8506930f7b522732a72fca7395d31bb8094739139324468e7ae618b1da4d3cda`  
		Last Modified: Tue, 14 Mar 2023 01:30:48 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.2-alpine` - linux; arm variant v7

```console
$ docker pull spiped@sha256:361539f7f9277859ba382de7be4afe676210140f53c3c5cd85d5ae3985f905c0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4237927 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2e899581be5421f50eb7e6339c7512ab16c114d8213f09e8aca52c68f0bcc311`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 10 Feb 2023 21:51:31 GMT
ADD file:143b601fcc6b5d7d95d3e5ccad3fec7081191a47e28d4f9294a7fb2499cab1af in / 
# Fri, 10 Feb 2023 21:51:31 GMT
CMD ["/bin/sh"]
# Wed, 01 Mar 2023 17:00:05 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Wed, 01 Mar 2023 17:00:07 GMT
RUN apk add --no-cache libssl1.1
# Wed, 01 Mar 2023 17:00:07 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 01 Mar 2023 17:00:14 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Wed, 01 Mar 2023 17:00:14 GMT
VOLUME [/spiped]
# Wed, 01 Mar 2023 17:00:14 GMT
WORKDIR /spiped
# Wed, 01 Mar 2023 17:00:14 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 01 Mar 2023 17:00:14 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 01 Mar 2023 17:00:15 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:6fb81ff47bd6d7db0ed86c9b951ad6417ec73ab60af6d22daa604076a902629c`  
		Last Modified: Fri, 10 Feb 2023 21:52:33 GMT  
		Size: 2.9 MB (2868494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bcf9acc5eeca77f6d435380f4f1fea53c3643c4cc9042daf13fdd9b6b72d9f5`  
		Last Modified: Wed, 01 Mar 2023 17:00:57 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f34e65da889251051ec9481b5d6cb0d428c45c8861fb2948b0c38c07470bba59`  
		Last Modified: Wed, 01 Mar 2023 17:00:57 GMT  
		Size: 1.2 MB (1167579 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0412dc4bafb0f9dabcfd28a3c0b4454de2db5c81112fdbb51bf5c883f4a6925`  
		Last Modified: Wed, 01 Mar 2023 17:00:57 GMT  
		Size: 200.1 KB (200120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70011259fd33df6da621cfb9142329c3c7a89b4bc5bfe91a87f7335995930ff9`  
		Last Modified: Wed, 01 Mar 2023 17:00:57 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99d3fd9f335e89a8501d7008f1bbaf813f4a5b26227452ecfc0001613be1ee7f`  
		Last Modified: Wed, 01 Mar 2023 17:00:57 GMT  
		Size: 337.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.2-alpine` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:b202c4e5897cb771f303b85871c6b7a1fb5f025c51e651b30a4415f0e2e4973d
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.8 MB (4842933 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6c3a0f714da4f343e79de4855fa4cdc4a23892d7fe5654dec6710bc79bb2cc2c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 10 Feb 2023 21:24:08 GMT
ADD file:9bd9ea42a9f3bdc769e80c6b8a4b117d65f73ae68e155a6172a1184e7ac8bcc1 in / 
# Fri, 10 Feb 2023 21:24:08 GMT
CMD ["/bin/sh"]
# Sat, 11 Feb 2023 06:39:43 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Sat, 11 Feb 2023 06:39:44 GMT
RUN apk add --no-cache libssl1.1
# Sat, 11 Feb 2023 06:39:44 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Sat, 11 Feb 2023 06:39:52 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Sat, 11 Feb 2023 06:39:52 GMT
VOLUME [/spiped]
# Sat, 11 Feb 2023 06:39:52 GMT
WORKDIR /spiped
# Sat, 11 Feb 2023 06:39:52 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 11 Feb 2023 06:39:52 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 11 Feb 2023 06:39:52 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:af6eaf76a39c2d3e7e0b8a0420486e3df33c4027d696c076a99a3d0ac09026af`  
		Last Modified: Fri, 10 Feb 2023 21:24:39 GMT  
		Size: 3.3 MB (3261959 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32e706a54c37c1524628e434965039ac738ff48a6f151dd2ef6da2cb49958cc0`  
		Last Modified: Sat, 11 Feb 2023 06:40:07 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e99781ddd302da37630cc491b5190c39c7867e6bd96556fad9f613e3411bca0d`  
		Last Modified: Sat, 11 Feb 2023 06:40:07 GMT  
		Size: 1.4 MB (1363548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:768a1af5c81e5cc877ea8cb330527a3924d5f2b5acfc5dd8239f84fdf091e5ed`  
		Last Modified: Sat, 11 Feb 2023 06:40:07 GMT  
		Size: 215.7 KB (215691 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7567bda17775002440a508f6ff25154cb13c9201175281b80186ce38d44e2b7`  
		Last Modified: Sat, 11 Feb 2023 06:40:07 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba17a7f3c3024db40a3e0b478318d1eb5168af1437c2bd502fb302591b78f95a`  
		Last Modified: Sat, 11 Feb 2023 06:40:07 GMT  
		Size: 338.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.2-alpine` - linux; 386

```console
$ docker pull spiped@sha256:1718408d282e2785554de5dd41b1935a8fd740cad6fa42ddeac2fafad4e15148
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.1 MB (5131990 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e81769d87082a52703eb2f30d09dbe3c289d1e6956af04796da66cf8ec2e5a5b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 10 Feb 2023 21:24:23 GMT
ADD file:125f3514520a5cd29df2830a409aa026a2bc06a77a7a5d150133436404b33d41 in / 
# Fri, 10 Feb 2023 21:24:24 GMT
CMD ["/bin/sh"]
# Wed, 01 Mar 2023 20:35:30 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Wed, 01 Mar 2023 20:35:32 GMT
RUN apk add --no-cache libssl1.1
# Wed, 01 Mar 2023 20:35:32 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 01 Mar 2023 20:35:44 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Wed, 01 Mar 2023 20:35:44 GMT
VOLUME [/spiped]
# Wed, 01 Mar 2023 20:35:44 GMT
WORKDIR /spiped
# Wed, 01 Mar 2023 20:35:44 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 01 Mar 2023 20:35:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 01 Mar 2023 20:35:44 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:b3e346c15c2377ec0e75cc9efa98baecd58b0e9bb92f0ec07eeda0bcc7e67fc7`  
		Last Modified: Fri, 10 Feb 2023 21:25:13 GMT  
		Size: 3.4 MB (3412353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9ddea08df82e419c862a82c04a7b6027073e509f79247aaab6fcb9a2d66e4bc`  
		Last Modified: Wed, 01 Mar 2023 20:36:27 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7baff4523d8b5b8d72311936f6b35a74dc61f50af8ceb150e8a464755ed3ff76`  
		Last Modified: Wed, 01 Mar 2023 20:36:27 GMT  
		Size: 1.5 MB (1486288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de00b81755546779184cb3998ef43c5c0445cd5871998c7feb92240ab36aeb5e`  
		Last Modified: Wed, 01 Mar 2023 20:36:27 GMT  
		Size: 231.6 KB (231613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:568814bee4cca693df73f2ed16adcc10335f014f7606b67b33d08c3abf12b51a`  
		Last Modified: Wed, 01 Mar 2023 20:36:27 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da028d97e3da3f51bb23a54f50dc51e00a905208ac487c94ae446e20f926b63c`  
		Last Modified: Wed, 01 Mar 2023 20:36:27 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.2-alpine` - linux; ppc64le

```console
$ docker pull spiped@sha256:75c7e8ce27d4c68e8862a8e832409e09dbeb2c47fa2163ac0ac7f4e794b6b14c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.0 MB (5025550 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:523cfab6c09a42cd9174ca6dee237febe2f4a72f0c07628ccddab56278968150`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 10 Feb 2023 21:20:36 GMT
ADD file:ec037a0d4b462d12963ac20d9ec49bb73b4bcaf84d4bc7b364ebf93667e585b0 in / 
# Fri, 10 Feb 2023 21:20:36 GMT
CMD ["/bin/sh"]
# Sat, 11 Feb 2023 09:33:46 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Sat, 11 Feb 2023 09:33:49 GMT
RUN apk add --no-cache libssl1.1
# Sat, 11 Feb 2023 09:33:50 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Sat, 11 Feb 2023 09:34:04 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Sat, 11 Feb 2023 09:34:04 GMT
VOLUME [/spiped]
# Sat, 11 Feb 2023 09:34:05 GMT
WORKDIR /spiped
# Sat, 11 Feb 2023 09:34:05 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 11 Feb 2023 09:34:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 11 Feb 2023 09:34:06 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:aa3c56f9c6f127b6c8f628c95db165741ca400d19bdaef2752d80f093e47451e`  
		Last Modified: Fri, 10 Feb 2023 21:21:37 GMT  
		Size: 3.4 MB (3390750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b5d50df2303841e19f748472d51fac8d0695468f1d50516484905b50450aa48`  
		Last Modified: Sat, 11 Feb 2023 09:34:31 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0b54432b9107e6d87810bd116ab5112e27a1f713d4d2c06525f0ed14f102e3c`  
		Last Modified: Sat, 11 Feb 2023 09:34:32 GMT  
		Size: 1.4 MB (1413040 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4bda8ea646857e9e3d0c92c042261af7dba424338abfc7cc1c58eec7b8985be`  
		Last Modified: Sat, 11 Feb 2023 09:34:32 GMT  
		Size: 220.0 KB (220021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e33bc423b9fd5cc84d66be2c92fc2c78368e9b5553d8c6848fab3570115fb66`  
		Last Modified: Sat, 11 Feb 2023 09:34:31 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53a89c5ec31eae84c318581d292f2fdc24ec49bc7692940d54b3b579b04cd2d6`  
		Last Modified: Sat, 11 Feb 2023 09:34:31 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.2-alpine` - linux; s390x

```console
$ docker pull spiped@sha256:c224a59dd171160cb9e3b3be6bac31704ad968f23bed4f4f8ae4d04d938951c6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.6 MB (4608839 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:88032fe647cd1b9c54c93549e3978f1e53d8c0df71f2c0c2660b0545fc0b7ae3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 10 Feb 2023 21:41:25 GMT
ADD file:03b2fb4d732a294329449ff55c5d84f7d2735e6510985718979469994f3a607b in / 
# Fri, 10 Feb 2023 21:41:26 GMT
CMD ["/bin/sh"]
# Sat, 11 Feb 2023 05:20:31 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Sat, 11 Feb 2023 05:20:32 GMT
RUN apk add --no-cache libssl1.1
# Sat, 11 Feb 2023 05:20:33 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Sat, 11 Feb 2023 05:20:38 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Sat, 11 Feb 2023 05:20:38 GMT
VOLUME [/spiped]
# Sat, 11 Feb 2023 05:20:38 GMT
WORKDIR /spiped
# Sat, 11 Feb 2023 05:20:39 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 11 Feb 2023 05:20:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 11 Feb 2023 05:20:39 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:24c4f8de3549a39c64b0edc2cfa68769b373f35138d0f13725100160bb32d4e2`  
		Last Modified: Fri, 10 Feb 2023 21:42:16 GMT  
		Size: 3.2 MB (3175116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdb5c0ff1110b4315355f81e38de10bb31ba9fe44d99d3b7598f20a28f2c98e1`  
		Last Modified: Sat, 11 Feb 2023 05:21:04 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9ac27252903c2b21737926a9cd0721ecfa3aba4f2e52da7f7c114aea4da62df`  
		Last Modified: Sat, 11 Feb 2023 05:21:04 GMT  
		Size: 1.2 MB (1223356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df30f40ce9a4931562f50ea55d6450396fd443fed95a0b2c0ea337f53f22ec25`  
		Last Modified: Sat, 11 Feb 2023 05:21:04 GMT  
		Size: 208.6 KB (208631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d9420167a9c04b73e787d02b0fa09ba21ff8b27917d0406146f9bc5a0df3034`  
		Last Modified: Sat, 11 Feb 2023 05:21:04 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea129f4350d878551c457a2192ea0570f86ca7ee5c193a6b0d8e19727570f05b`  
		Last Modified: Sat, 11 Feb 2023 05:21:04 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:alpine`

```console
$ docker pull spiped@sha256:dfaf6e7592d4ab323a62d1b401cab7d35cab87afdb70fe94fc8d2c41d99aca33
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
$ docker pull spiped@sha256:b02340eb97482a93ed8c3997880473f27309e7362e27d06bfbdeb686da9f835f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.1 MB (5080754 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1660f13550a5bd6ce0ec142f4dc1325092450163ee42f52b56572854d7e8c1e3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Sat, 11 Feb 2023 04:46:42 GMT
ADD file:40887ab7c06977737e63c215c9bd297c0c74de8d12d16ebdf1c3d40ac392f62d in / 
# Sat, 11 Feb 2023 04:46:42 GMT
CMD ["/bin/sh"]
# Sat, 11 Feb 2023 14:04:29 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Sat, 11 Feb 2023 14:04:30 GMT
RUN apk add --no-cache libssl1.1
# Sat, 11 Feb 2023 14:04:30 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Sat, 11 Feb 2023 14:04:41 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Sat, 11 Feb 2023 14:04:41 GMT
VOLUME [/spiped]
# Sat, 11 Feb 2023 14:04:41 GMT
WORKDIR /spiped
# Sat, 11 Feb 2023 14:04:41 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 11 Feb 2023 14:04:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 11 Feb 2023 14:04:41 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:63b65145d645c1250c391b2d16ebe53b3747c295ca8ba2fcb6b0cf064a4dc21c`  
		Last Modified: Fri, 10 Feb 2023 22:41:31 GMT  
		Size: 3.4 MB (3374446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1567e533de4a753157026d7ef2c42cfa5f9efd21e25cc7370e4c8f1c8f1c8a47`  
		Last Modified: Sat, 11 Feb 2023 14:04:56 GMT  
		Size: 1.3 KB (1267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1a1fcb595374972f69b5a50bd54f62b80c9214b0f891c62726a3fb6853cf855`  
		Last Modified: Sat, 11 Feb 2023 14:04:56 GMT  
		Size: 1.5 MB (1483289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24f4efb6e81c911655772824a287a9f39d90e069841b4fe5601933b9b0ffe154`  
		Last Modified: Sat, 11 Feb 2023 14:04:56 GMT  
		Size: 221.3 KB (221282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:981056191296cd6f887bc7d5e8e078e1cec12690bc7fc8623b868e6b4023e0ea`  
		Last Modified: Sat, 11 Feb 2023 14:04:56 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:577ef58b3b8b045fa02bbbbd599b6c9d4310c0039e442d91e549dad4f7e556fd`  
		Last Modified: Sat, 11 Feb 2023 14:04:56 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; arm variant v6

```console
$ docker pull spiped@sha256:76a36336fb4a148684ae27104022667db149e7b75e602fb0d1fb636cb8277330
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.6 MB (4559988 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8148101a55ef329eee778b51e7674409dd7530f66643e375f5eaf15450e8d364`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Mon, 13 Mar 2023 16:12:44 GMT
ADD file:d825d9aef59df0df23c0140a490998407ee0a62a051699b5c050aef7cb03f042 in / 
# Mon, 13 Mar 2023 16:12:44 GMT
CMD ["/bin/sh"]
# Tue, 14 Mar 2023 01:30:23 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Tue, 14 Mar 2023 01:30:24 GMT
RUN apk add --no-cache libssl1.1
# Tue, 14 Mar 2023 01:30:24 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 14 Mar 2023 01:30:32 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Tue, 14 Mar 2023 01:30:32 GMT
VOLUME [/spiped]
# Tue, 14 Mar 2023 01:30:32 GMT
WORKDIR /spiped
# Tue, 14 Mar 2023 01:30:32 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 14 Mar 2023 01:30:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 14 Mar 2023 01:30:32 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:6a6e4ab63e54442e16400f69d37f662d60cbd67565631eff6bf59b4176e482c3`  
		Last Modified: Fri, 10 Feb 2023 20:50:22 GMT  
		Size: 3.1 MB (3110885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e45faa3e84504ff194d07161781bbb3d65ced006b3559fdd50974ca59bede67b`  
		Last Modified: Tue, 14 Mar 2023 01:30:48 GMT  
		Size: 1.3 KB (1271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a49b678821973054e204d328f8a1abfd5c4d0babdc516e24b56c76cc2adbd596`  
		Last Modified: Tue, 14 Mar 2023 01:30:49 GMT  
		Size: 1.2 MB (1240997 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8dbbba3d131edbec32d7ac2251201ab33e79abc9994b4e0635fac27365f1579f`  
		Last Modified: Tue, 14 Mar 2023 01:30:49 GMT  
		Size: 206.4 KB (206366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f344f34fb34133bb7a416417587f8f9219c749343ba309ab724c2dba1c4653c3`  
		Last Modified: Tue, 14 Mar 2023 01:30:48 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8506930f7b522732a72fca7395d31bb8094739139324468e7ae618b1da4d3cda`  
		Last Modified: Tue, 14 Mar 2023 01:30:48 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; arm variant v7

```console
$ docker pull spiped@sha256:361539f7f9277859ba382de7be4afe676210140f53c3c5cd85d5ae3985f905c0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4237927 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2e899581be5421f50eb7e6339c7512ab16c114d8213f09e8aca52c68f0bcc311`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 10 Feb 2023 21:51:31 GMT
ADD file:143b601fcc6b5d7d95d3e5ccad3fec7081191a47e28d4f9294a7fb2499cab1af in / 
# Fri, 10 Feb 2023 21:51:31 GMT
CMD ["/bin/sh"]
# Wed, 01 Mar 2023 17:00:05 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Wed, 01 Mar 2023 17:00:07 GMT
RUN apk add --no-cache libssl1.1
# Wed, 01 Mar 2023 17:00:07 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 01 Mar 2023 17:00:14 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Wed, 01 Mar 2023 17:00:14 GMT
VOLUME [/spiped]
# Wed, 01 Mar 2023 17:00:14 GMT
WORKDIR /spiped
# Wed, 01 Mar 2023 17:00:14 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 01 Mar 2023 17:00:14 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 01 Mar 2023 17:00:15 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:6fb81ff47bd6d7db0ed86c9b951ad6417ec73ab60af6d22daa604076a902629c`  
		Last Modified: Fri, 10 Feb 2023 21:52:33 GMT  
		Size: 2.9 MB (2868494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bcf9acc5eeca77f6d435380f4f1fea53c3643c4cc9042daf13fdd9b6b72d9f5`  
		Last Modified: Wed, 01 Mar 2023 17:00:57 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f34e65da889251051ec9481b5d6cb0d428c45c8861fb2948b0c38c07470bba59`  
		Last Modified: Wed, 01 Mar 2023 17:00:57 GMT  
		Size: 1.2 MB (1167579 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0412dc4bafb0f9dabcfd28a3c0b4454de2db5c81112fdbb51bf5c883f4a6925`  
		Last Modified: Wed, 01 Mar 2023 17:00:57 GMT  
		Size: 200.1 KB (200120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70011259fd33df6da621cfb9142329c3c7a89b4bc5bfe91a87f7335995930ff9`  
		Last Modified: Wed, 01 Mar 2023 17:00:57 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99d3fd9f335e89a8501d7008f1bbaf813f4a5b26227452ecfc0001613be1ee7f`  
		Last Modified: Wed, 01 Mar 2023 17:00:57 GMT  
		Size: 337.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:b202c4e5897cb771f303b85871c6b7a1fb5f025c51e651b30a4415f0e2e4973d
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.8 MB (4842933 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6c3a0f714da4f343e79de4855fa4cdc4a23892d7fe5654dec6710bc79bb2cc2c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 10 Feb 2023 21:24:08 GMT
ADD file:9bd9ea42a9f3bdc769e80c6b8a4b117d65f73ae68e155a6172a1184e7ac8bcc1 in / 
# Fri, 10 Feb 2023 21:24:08 GMT
CMD ["/bin/sh"]
# Sat, 11 Feb 2023 06:39:43 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Sat, 11 Feb 2023 06:39:44 GMT
RUN apk add --no-cache libssl1.1
# Sat, 11 Feb 2023 06:39:44 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Sat, 11 Feb 2023 06:39:52 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Sat, 11 Feb 2023 06:39:52 GMT
VOLUME [/spiped]
# Sat, 11 Feb 2023 06:39:52 GMT
WORKDIR /spiped
# Sat, 11 Feb 2023 06:39:52 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 11 Feb 2023 06:39:52 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 11 Feb 2023 06:39:52 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:af6eaf76a39c2d3e7e0b8a0420486e3df33c4027d696c076a99a3d0ac09026af`  
		Last Modified: Fri, 10 Feb 2023 21:24:39 GMT  
		Size: 3.3 MB (3261959 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32e706a54c37c1524628e434965039ac738ff48a6f151dd2ef6da2cb49958cc0`  
		Last Modified: Sat, 11 Feb 2023 06:40:07 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e99781ddd302da37630cc491b5190c39c7867e6bd96556fad9f613e3411bca0d`  
		Last Modified: Sat, 11 Feb 2023 06:40:07 GMT  
		Size: 1.4 MB (1363548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:768a1af5c81e5cc877ea8cb330527a3924d5f2b5acfc5dd8239f84fdf091e5ed`  
		Last Modified: Sat, 11 Feb 2023 06:40:07 GMT  
		Size: 215.7 KB (215691 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7567bda17775002440a508f6ff25154cb13c9201175281b80186ce38d44e2b7`  
		Last Modified: Sat, 11 Feb 2023 06:40:07 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba17a7f3c3024db40a3e0b478318d1eb5168af1437c2bd502fb302591b78f95a`  
		Last Modified: Sat, 11 Feb 2023 06:40:07 GMT  
		Size: 338.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; 386

```console
$ docker pull spiped@sha256:1718408d282e2785554de5dd41b1935a8fd740cad6fa42ddeac2fafad4e15148
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.1 MB (5131990 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e81769d87082a52703eb2f30d09dbe3c289d1e6956af04796da66cf8ec2e5a5b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 10 Feb 2023 21:24:23 GMT
ADD file:125f3514520a5cd29df2830a409aa026a2bc06a77a7a5d150133436404b33d41 in / 
# Fri, 10 Feb 2023 21:24:24 GMT
CMD ["/bin/sh"]
# Wed, 01 Mar 2023 20:35:30 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Wed, 01 Mar 2023 20:35:32 GMT
RUN apk add --no-cache libssl1.1
# Wed, 01 Mar 2023 20:35:32 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 01 Mar 2023 20:35:44 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Wed, 01 Mar 2023 20:35:44 GMT
VOLUME [/spiped]
# Wed, 01 Mar 2023 20:35:44 GMT
WORKDIR /spiped
# Wed, 01 Mar 2023 20:35:44 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 01 Mar 2023 20:35:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 01 Mar 2023 20:35:44 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:b3e346c15c2377ec0e75cc9efa98baecd58b0e9bb92f0ec07eeda0bcc7e67fc7`  
		Last Modified: Fri, 10 Feb 2023 21:25:13 GMT  
		Size: 3.4 MB (3412353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9ddea08df82e419c862a82c04a7b6027073e509f79247aaab6fcb9a2d66e4bc`  
		Last Modified: Wed, 01 Mar 2023 20:36:27 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7baff4523d8b5b8d72311936f6b35a74dc61f50af8ceb150e8a464755ed3ff76`  
		Last Modified: Wed, 01 Mar 2023 20:36:27 GMT  
		Size: 1.5 MB (1486288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de00b81755546779184cb3998ef43c5c0445cd5871998c7feb92240ab36aeb5e`  
		Last Modified: Wed, 01 Mar 2023 20:36:27 GMT  
		Size: 231.6 KB (231613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:568814bee4cca693df73f2ed16adcc10335f014f7606b67b33d08c3abf12b51a`  
		Last Modified: Wed, 01 Mar 2023 20:36:27 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da028d97e3da3f51bb23a54f50dc51e00a905208ac487c94ae446e20f926b63c`  
		Last Modified: Wed, 01 Mar 2023 20:36:27 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; ppc64le

```console
$ docker pull spiped@sha256:75c7e8ce27d4c68e8862a8e832409e09dbeb2c47fa2163ac0ac7f4e794b6b14c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.0 MB (5025550 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:523cfab6c09a42cd9174ca6dee237febe2f4a72f0c07628ccddab56278968150`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 10 Feb 2023 21:20:36 GMT
ADD file:ec037a0d4b462d12963ac20d9ec49bb73b4bcaf84d4bc7b364ebf93667e585b0 in / 
# Fri, 10 Feb 2023 21:20:36 GMT
CMD ["/bin/sh"]
# Sat, 11 Feb 2023 09:33:46 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Sat, 11 Feb 2023 09:33:49 GMT
RUN apk add --no-cache libssl1.1
# Sat, 11 Feb 2023 09:33:50 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Sat, 11 Feb 2023 09:34:04 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Sat, 11 Feb 2023 09:34:04 GMT
VOLUME [/spiped]
# Sat, 11 Feb 2023 09:34:05 GMT
WORKDIR /spiped
# Sat, 11 Feb 2023 09:34:05 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 11 Feb 2023 09:34:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 11 Feb 2023 09:34:06 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:aa3c56f9c6f127b6c8f628c95db165741ca400d19bdaef2752d80f093e47451e`  
		Last Modified: Fri, 10 Feb 2023 21:21:37 GMT  
		Size: 3.4 MB (3390750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b5d50df2303841e19f748472d51fac8d0695468f1d50516484905b50450aa48`  
		Last Modified: Sat, 11 Feb 2023 09:34:31 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0b54432b9107e6d87810bd116ab5112e27a1f713d4d2c06525f0ed14f102e3c`  
		Last Modified: Sat, 11 Feb 2023 09:34:32 GMT  
		Size: 1.4 MB (1413040 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4bda8ea646857e9e3d0c92c042261af7dba424338abfc7cc1c58eec7b8985be`  
		Last Modified: Sat, 11 Feb 2023 09:34:32 GMT  
		Size: 220.0 KB (220021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e33bc423b9fd5cc84d66be2c92fc2c78368e9b5553d8c6848fab3570115fb66`  
		Last Modified: Sat, 11 Feb 2023 09:34:31 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53a89c5ec31eae84c318581d292f2fdc24ec49bc7692940d54b3b579b04cd2d6`  
		Last Modified: Sat, 11 Feb 2023 09:34:31 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; s390x

```console
$ docker pull spiped@sha256:c224a59dd171160cb9e3b3be6bac31704ad968f23bed4f4f8ae4d04d938951c6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.6 MB (4608839 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:88032fe647cd1b9c54c93549e3978f1e53d8c0df71f2c0c2660b0545fc0b7ae3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 10 Feb 2023 21:41:25 GMT
ADD file:03b2fb4d732a294329449ff55c5d84f7d2735e6510985718979469994f3a607b in / 
# Fri, 10 Feb 2023 21:41:26 GMT
CMD ["/bin/sh"]
# Sat, 11 Feb 2023 05:20:31 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Sat, 11 Feb 2023 05:20:32 GMT
RUN apk add --no-cache libssl1.1
# Sat, 11 Feb 2023 05:20:33 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Sat, 11 Feb 2023 05:20:38 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Sat, 11 Feb 2023 05:20:38 GMT
VOLUME [/spiped]
# Sat, 11 Feb 2023 05:20:38 GMT
WORKDIR /spiped
# Sat, 11 Feb 2023 05:20:39 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 11 Feb 2023 05:20:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 11 Feb 2023 05:20:39 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:24c4f8de3549a39c64b0edc2cfa68769b373f35138d0f13725100160bb32d4e2`  
		Last Modified: Fri, 10 Feb 2023 21:42:16 GMT  
		Size: 3.2 MB (3175116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdb5c0ff1110b4315355f81e38de10bb31ba9fe44d99d3b7598f20a28f2c98e1`  
		Last Modified: Sat, 11 Feb 2023 05:21:04 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9ac27252903c2b21737926a9cd0721ecfa3aba4f2e52da7f7c114aea4da62df`  
		Last Modified: Sat, 11 Feb 2023 05:21:04 GMT  
		Size: 1.2 MB (1223356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df30f40ce9a4931562f50ea55d6450396fd443fed95a0b2c0ea337f53f22ec25`  
		Last Modified: Sat, 11 Feb 2023 05:21:04 GMT  
		Size: 208.6 KB (208631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d9420167a9c04b73e787d02b0fa09ba21ff8b27917d0406146f9bc5a0df3034`  
		Last Modified: Sat, 11 Feb 2023 05:21:04 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea129f4350d878551c457a2192ea0570f86ca7ee5c193a6b0d8e19727570f05b`  
		Last Modified: Sat, 11 Feb 2023 05:21:04 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:latest`

```console
$ docker pull spiped@sha256:3f946d80813d27b67a12c1f37671961b9dafebeaa779ab08875cf6daa5ad8ed2
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
$ docker pull spiped@sha256:027c9e8b16fd5686f2386e10f4efea51d2cf9baf4e7bcdaf3c1fb979d3d6e6c2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.4 MB (37412991 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:803eb276e1835de8624a0705f68be4b52442d62ad95ad7f8933b8a2f1dfe7a40`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 01 Mar 2023 04:09:58 GMT
ADD file:493a5b0c8d2d63a1343258b3f9aa5fcd59a93f44fe26ad9e56b094c3a08fd3be in / 
# Wed, 01 Mar 2023 04:09:59 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 17:55:56 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 01 Mar 2023 17:55:59 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 17:55:59 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 01 Mar 2023 17:56:20 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 01 Mar 2023 17:56:20 GMT
VOLUME [/spiped]
# Wed, 01 Mar 2023 17:56:20 GMT
WORKDIR /spiped
# Wed, 01 Mar 2023 17:56:20 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 01 Mar 2023 17:56:20 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 01 Mar 2023 17:56:20 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:3f9582a2cbe7197f39185419c0ced2c986389f8fc6aa805e1f5c090eea6511e0`  
		Last Modified: Wed, 01 Mar 2023 04:14:23 GMT  
		Size: 31.4 MB (31411403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e97821d2ff040682a3d9356a04d84b72255c563d7603f7219e6ed9e7c0e80e3`  
		Last Modified: Wed, 01 Mar 2023 17:56:35 GMT  
		Size: 1.7 KB (1733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97f3106ca46ab6b0eb674057029e3469fb737549c0e17f93501a7baa91ee7d66`  
		Last Modified: Wed, 01 Mar 2023 17:56:34 GMT  
		Size: 1.1 KB (1054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22be67cd1cbaef6c42eaf8be1eccae8272262dbf3e2ff498e0c4ce7de42750df`  
		Last Modified: Wed, 01 Mar 2023 17:56:36 GMT  
		Size: 6.0 MB (5998329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ededc4cf18635cc66d453c3af24a583d4f300aa916b5d12a5e3622c70bb9a86b`  
		Last Modified: Wed, 01 Mar 2023 17:56:35 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2631603d11fd9110672446c8a343410ea67a502e725c014b4e1f83f522b56904`  
		Last Modified: Wed, 01 Mar 2023 17:56:35 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; arm variant v5

```console
$ docker pull spiped@sha256:528e13ba139adf0768024a80cfc79ab5cb3d0ea5e8f9b9f3bc1511f2d698c215
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.9 MB (33947393 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5a1e48f7b0e65652cca9ca80196c861d383ac1f1b0103cc512be95efd00fc6e9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 01 Mar 2023 01:48:54 GMT
ADD file:b4fb1081f6eb8a0560d56d5781bbcedaac1453615d56e0943245dca784785ea2 in / 
# Wed, 01 Mar 2023 01:48:54 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 07:10:40 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 01 Mar 2023 07:10:44 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 07:10:44 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 01 Mar 2023 07:11:03 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 01 Mar 2023 07:11:03 GMT
VOLUME [/spiped]
# Wed, 01 Mar 2023 07:11:03 GMT
WORKDIR /spiped
# Wed, 01 Mar 2023 07:11:03 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 01 Mar 2023 07:11:03 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 01 Mar 2023 07:11:04 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:3c3af56dbec5913ef8aec0f1ca7112eb5914b4ad346ccd48f836dd7ec0621ba5`  
		Last Modified: Wed, 01 Mar 2023 01:52:57 GMT  
		Size: 28.9 MB (28915776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9aca7d992b566279fbac9ecdeffb9ff2db68cf1ffd6f31a2cce852311c28c5ce`  
		Last Modified: Wed, 01 Mar 2023 07:11:20 GMT  
		Size: 1.7 KB (1728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fc3eb64d155ea643dfc7dde1104693192a95033b812f1cf66e286245705de6f`  
		Last Modified: Wed, 01 Mar 2023 07:11:20 GMT  
		Size: 1.1 KB (1050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9169ad29c4b57b416977f34e4cae1ad9b4efb6110e2a150a7cb43b7eab0da3d3`  
		Last Modified: Wed, 01 Mar 2023 07:11:21 GMT  
		Size: 5.0 MB (5028368 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:742f87e7cb263314cfe9b69a92b5fef45b368e04c178942b699311a03503e14c`  
		Last Modified: Wed, 01 Mar 2023 07:11:20 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0dfe2f008531a4616c872689c583cd0c8468b2fb60b07981fc0e20a80f84497`  
		Last Modified: Wed, 01 Mar 2023 07:11:20 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; arm variant v7

```console
$ docker pull spiped@sha256:627d305c141756ae7f1d3ce8a13ed19b5de3d5e5cc05419c57ca52a7cfad3e38
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.3 MB (31329572 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:80590efa308da9fa53e6713503023d50cdbb6bed46e6565e7a173368c94a3398`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 01 Mar 2023 01:57:55 GMT
ADD file:182fe91b8976a8871aba0d2ff9d4400a60317c8dec282261ba94247500c8d3dc in / 
# Wed, 01 Mar 2023 01:57:55 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 16:59:36 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 01 Mar 2023 16:59:39 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 16:59:39 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 01 Mar 2023 17:00:00 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 01 Mar 2023 17:00:00 GMT
VOLUME [/spiped]
# Wed, 01 Mar 2023 17:00:00 GMT
WORKDIR /spiped
# Wed, 01 Mar 2023 17:00:00 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 01 Mar 2023 17:00:00 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 01 Mar 2023 17:00:00 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:b4770fcf2ef78c1e46693da734476bfaf03cbe1d0b6e0a0f22c2c2e53419e803`  
		Last Modified: Wed, 01 Mar 2023 02:03:02 GMT  
		Size: 26.6 MB (26577290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe9ae4c200b12f57c7a99dbe5cd058c0c8e834ab0e042072df6f3ba0e2ef370b`  
		Last Modified: Wed, 01 Mar 2023 17:00:40 GMT  
		Size: 1.7 KB (1728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5dd24a9c965643a04effdcd9b7b20069af323b31c98f25e7ed41120a81c07cc`  
		Last Modified: Wed, 01 Mar 2023 17:00:40 GMT  
		Size: 1.1 KB (1051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0dba42d16068e44c779a0a9402aca488c2ae655c6d1c8fb07e88c3d68190a68b`  
		Last Modified: Wed, 01 Mar 2023 17:00:41 GMT  
		Size: 4.7 MB (4749033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c895f59fed0503b2299b019d207a580b45874b387ef1a68a3f08902c66676b63`  
		Last Modified: Wed, 01 Mar 2023 17:00:40 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f62eaf16d3dbd860a6214d912a6da95cacab5eaf97a19518ccf6c3ec0c774b0`  
		Last Modified: Wed, 01 Mar 2023 17:00:40 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:c0ee27c170b5818d26dd2679b9f68fbd1717c2b8029be42c1f19b7a9d582c867
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.3 MB (35338707 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f09e879bddede08a1bc165d3efa6587de5e8610534659bd12411ed41795ba246`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 01 Mar 2023 02:20:39 GMT
ADD file:9dc5c6fb6431df80107eddb76fb18256d6f4a06b4b22f9a7c4bcd58476068186 in / 
# Wed, 01 Mar 2023 02:20:39 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 14:07:19 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 01 Mar 2023 14:07:22 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 14:07:22 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 01 Mar 2023 14:07:37 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 01 Mar 2023 14:07:37 GMT
VOLUME [/spiped]
# Wed, 01 Mar 2023 14:07:37 GMT
WORKDIR /spiped
# Wed, 01 Mar 2023 14:07:37 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 01 Mar 2023 14:07:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 01 Mar 2023 14:07:38 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:66dbba0fb1b568cc3ffd53409ba2f9f82995ab7f80e379338f3f36e4dcd223be`  
		Last Modified: Wed, 01 Mar 2023 02:24:17 GMT  
		Size: 30.1 MB (30062814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:261024cf523923721d856c4f6e77a37c041d87ad2d3b4ccd92fb53f3abaab41f`  
		Last Modified: Wed, 01 Mar 2023 14:07:53 GMT  
		Size: 1.7 KB (1738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fe92519b62d1a9b8e2d52510cf1bf885ff477e0383a53bd4ee6a4efb5f3c14e`  
		Last Modified: Wed, 01 Mar 2023 14:07:53 GMT  
		Size: 1.1 KB (1051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a212b6d6d17e0b6cad09fb9cb67db006696d183039d38e32013a5fc3c0afb160`  
		Last Modified: Wed, 01 Mar 2023 14:07:54 GMT  
		Size: 5.3 MB (5272635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa9945ac00fd76d0a06763ef812f442fd4bb8aa3a67db027da1597a25f1e77aa`  
		Last Modified: Wed, 01 Mar 2023 14:07:53 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9fdec150625f76667b7ba6e9417519bf4f6d92c140125d060a1efb39e391342`  
		Last Modified: Wed, 01 Mar 2023 14:07:53 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; 386

```console
$ docker pull spiped@sha256:74d7f5c8f3f3d9c67ac2694a397c85180e9414b6092e41e394b39054f2029c92
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.3 MB (40291472 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cd42d521cfced48016618daf00f5e6976442656bf9c4005a7c8200ef734bcbd4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 23 Mar 2023 00:39:18 GMT
ADD file:315d843eefd4a8bb2345366dcd6bab00a06fca4a7970e220ae8946123d07d7ed in / 
# Thu, 23 Mar 2023 00:39:19 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 12:10:30 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Thu, 23 Mar 2023 12:10:33 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 12:10:33 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 23 Mar 2023 12:10:56 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 23 Mar 2023 12:10:56 GMT
VOLUME [/spiped]
# Thu, 23 Mar 2023 12:10:56 GMT
WORKDIR /spiped
# Thu, 23 Mar 2023 12:10:56 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 23 Mar 2023 12:10:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Mar 2023 12:10:57 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:3e638a975ea99fe8646002726dcb1ccdccc49ad33967b30337b9b2413e0619b5`  
		Last Modified: Thu, 23 Mar 2023 00:43:09 GMT  
		Size: 32.4 MB (32396277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8c70cbb4c8fd8326cfa3a38bcadaebdcf624fcd76381d57288eb687694073d1`  
		Last Modified: Thu, 23 Mar 2023 12:11:11 GMT  
		Size: 1.7 KB (1725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b85e36913d82a6dadb0781c7ab440ef652976cc8995f5f0a0bd0541b9b620373`  
		Last Modified: Thu, 23 Mar 2023 12:11:11 GMT  
		Size: 1.1 KB (1054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bec8a50af228e59f346840b516f8f52a3b22b0be6d31a71d1341b272cc16d2ad`  
		Last Modified: Thu, 23 Mar 2023 12:11:13 GMT  
		Size: 7.9 MB (7891948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af275a5a028f320d08a155a1238d5121d8a0198cebf123d479cfab9a01aafd10`  
		Last Modified: Thu, 23 Mar 2023 12:11:11 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:409fcb43c7b4c77abd48e9757bd49eadd9c1aade55294cd9145e4f451a2a7a75`  
		Last Modified: Thu, 23 Mar 2023 12:11:11 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; mips64le

```console
$ docker pull spiped@sha256:4b768c4a74571ecb307ea7f2c6f0d5444219c4f7701ca7ece08073134a9817c7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.3 MB (35342762 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:60d987426dc913c9b10892ddd45cd5d0cb2f8311fd0e994196056e11189abf9e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 01 Mar 2023 02:10:54 GMT
ADD file:0bcd66a6a099cdb6e018ddc0f00270be93dccd3be6167ce36e9efc99c31549d9 in / 
# Wed, 01 Mar 2023 02:10:59 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 13:56:50 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 01 Mar 2023 13:57:04 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 13:57:07 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 01 Mar 2023 13:58:36 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 01 Mar 2023 13:58:39 GMT
VOLUME [/spiped]
# Wed, 01 Mar 2023 13:58:42 GMT
WORKDIR /spiped
# Wed, 01 Mar 2023 13:58:44 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 01 Mar 2023 13:58:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 01 Mar 2023 13:58:49 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:89f6b45a7afd174bf0d443156831cacd9e6a26c834ad62610b6db53c731d257f`  
		Last Modified: Wed, 01 Mar 2023 02:18:50 GMT  
		Size: 29.6 MB (29634488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d10af42af1cddee9f8d002cb64f604273d7fd56c39403c8ecb2ca86ae445b2ac`  
		Last Modified: Wed, 01 Mar 2023 13:59:02 GMT  
		Size: 1.6 KB (1614 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da6cf49bc572eb473177215ee0a0e9187f04a782706a0d2a362817c62e3e4c1c`  
		Last Modified: Wed, 01 Mar 2023 13:59:03 GMT  
		Size: 928.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:030a52e1972e6a16de35f2c209c9fe8b1b7b677e38894c831863d54f0f1d6cfa`  
		Last Modified: Wed, 01 Mar 2023 13:59:07 GMT  
		Size: 5.7 MB (5705294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8eeca73463248c240d686d1c65ee25f2d27dd86f1920c0ab13f7974cd43b0d51`  
		Last Modified: Wed, 01 Mar 2023 13:59:03 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3867f0e8bddd40c5ae56a42d561c19e9e6c3520d9bb3a19c4ee8e10b5e35a76a`  
		Last Modified: Wed, 01 Mar 2023 13:59:02 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; ppc64le

```console
$ docker pull spiped@sha256:5eeeda056f21e90509214894b25b29c2f077d779e3a9894d7239c7c5b1dde12d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.3 MB (41291034 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2af8e0b52e04e9db1d381ffa1800979e5bb8de9720068f9bb1b0598a7198df6e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 01 Mar 2023 04:47:33 GMT
ADD file:6fdf0b2f8ea4be2d01e25a9d85db8f8c7e3b2a641c9c7665e34f4fad771815e0 in / 
# Wed, 01 Mar 2023 04:47:35 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 14:40:08 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 01 Mar 2023 14:40:14 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 14:40:15 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 01 Mar 2023 14:41:05 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 01 Mar 2023 14:41:06 GMT
VOLUME [/spiped]
# Wed, 01 Mar 2023 14:41:06 GMT
WORKDIR /spiped
# Wed, 01 Mar 2023 14:41:07 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 01 Mar 2023 14:41:07 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 01 Mar 2023 14:41:08 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:93ab3a60c2a8cbc1150cb2bd54222db8b79c525c0243534a10d6294ef7ff83ac`  
		Last Modified: Wed, 01 Mar 2023 04:53:54 GMT  
		Size: 35.3 MB (35288103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0a2080116d00583c373f079b8f40c2fa202cfaa894e5646b928e2f519bc8d0e`  
		Last Modified: Wed, 01 Mar 2023 14:41:39 GMT  
		Size: 1.7 KB (1734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6c05e885d8e0e269f3910fa5c387e4bfe94b5f5844a929e3f2945347c9bc33a`  
		Last Modified: Wed, 01 Mar 2023 14:41:39 GMT  
		Size: 1.1 KB (1055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f9c9a00d487b5d63eb533652fd7c8bbcaf5b4a766b8f50698468f313ea58b31`  
		Last Modified: Wed, 01 Mar 2023 14:41:41 GMT  
		Size: 6.0 MB (5999671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5ffd618016f8cd2101168350b00bdbad7932215a46cddd3c1abc7a1efdf9834`  
		Last Modified: Wed, 01 Mar 2023 14:41:39 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed01129e03be3daf248d482853655a906b1f3e7594b351c1d568f69c46c410ac`  
		Last Modified: Wed, 01 Mar 2023 14:41:39 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; s390x

```console
$ docker pull spiped@sha256:5052a882da69e191760a75d37205ff0a1edd8edf21ae507a22d93c6b1672215a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.8 MB (34837546 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4be5954f5bff77d2a4e04836cc5938d850a56e7ee023f169242f1226e121a558`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 23 Mar 2023 00:44:06 GMT
ADD file:8b6d3f57adaa8af2e0599a6468c50b713d281165b4e61150850bedf587f7ad4f in / 
# Thu, 23 Mar 2023 00:44:08 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 12:15:46 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Thu, 23 Mar 2023 12:15:49 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 12:15:49 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 23 Mar 2023 12:16:07 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 23 Mar 2023 12:16:08 GMT
VOLUME [/spiped]
# Thu, 23 Mar 2023 12:16:08 GMT
WORKDIR /spiped
# Thu, 23 Mar 2023 12:16:08 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 23 Mar 2023 12:16:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Mar 2023 12:16:09 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:25d08e051bb75230bad82e3a7a054083beec6b4f6a46c8345c731582c297a408`  
		Last Modified: Thu, 23 Mar 2023 00:47:20 GMT  
		Size: 29.6 MB (29646820 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3388e32dd1b77d93d6b62ba801fb658ac69c6eebde8b030476caac13f83542be`  
		Last Modified: Thu, 23 Mar 2023 12:16:29 GMT  
		Size: 1.7 KB (1736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a701ac09c5ac118d050e81f6139936da77a346003315c4444e1939a6b9fbf5a`  
		Last Modified: Thu, 23 Mar 2023 12:16:29 GMT  
		Size: 1.1 KB (1050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76c28eecb90a4ce4306f2ee104c3b7a26ed907a1d7b4ffe9ee9f404860df7d2f`  
		Last Modified: Thu, 23 Mar 2023 12:16:30 GMT  
		Size: 5.2 MB (5187470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:851271a85236c408b9e2df7b62a45c37bc5552fb05fc8fb30a87d4f40e207d26`  
		Last Modified: Thu, 23 Mar 2023 12:16:29 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30749340374b1df790439fe4c7b71b610b3d0ae3aef3705de18f2472f5933c06`  
		Last Modified: Thu, 23 Mar 2023 12:16:29 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
