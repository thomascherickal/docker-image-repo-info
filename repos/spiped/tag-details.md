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
$ docker pull spiped@sha256:d9abc65404acc410b3f94bd812f875d66ad7304604f00ee6464be3ab291d57b3
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
$ docker pull spiped@sha256:dc2c3a3712eacb11a556c86bc2a6b606ba5a0edff87bf3638c159b85a1135448
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.3 MB (37335950 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1d472f594ea8090d6f3cbeb573986f7840e512b983c9def18699f62efe8bcc04`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 26 Jan 2022 01:40:35 GMT
ADD file:90495c24c897ec47982e200f732f8be3109fcd791691ddffae0756898f91024f in / 
# Wed, 26 Jan 2022 01:40:36 GMT
CMD ["bash"]
# Thu, 27 Jan 2022 02:32:24 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Thu, 27 Jan 2022 02:32:27 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Thu, 27 Jan 2022 02:32:28 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 27 Jan 2022 02:32:58 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 27 Jan 2022 02:32:58 GMT
VOLUME [/spiped]
# Thu, 27 Jan 2022 02:32:59 GMT
WORKDIR /spiped
# Thu, 27 Jan 2022 02:33:00 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 27 Jan 2022 02:33:00 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 27 Jan 2022 02:33:01 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:5eb5b503b37671af16371272f9c5313a3e82f1d0756e14506704489ad9900803`  
		Last Modified: Wed, 26 Jan 2022 01:46:39 GMT  
		Size: 31.4 MB (31366257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6a2517caec378bb5ccef0a0d6e52b5e25a629d59a240188bd605cf9f98bc57d`  
		Last Modified: Thu, 27 Jan 2022 02:33:32 GMT  
		Size: 1.7 KB (1734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9824d58dd5193ef98f897a6ac1feb9749d5f2371324023d2ca61dae51fb70e6`  
		Last Modified: Thu, 27 Jan 2022 02:33:32 GMT  
		Size: 1.1 KB (1051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d878a5544ecf1374c1348226765bcdd58a98e4e3d4c98f89ccf5fa10a7ca8ff`  
		Last Modified: Thu, 27 Jan 2022 02:33:34 GMT  
		Size: 6.0 MB (5966436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:754c3acbb4e4a2d6ba3fb19ebf6f464a6af124ca39e832916a9e20959ba6cb46`  
		Last Modified: Thu, 27 Jan 2022 02:33:32 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ddcc8c75157adfeb6f31357486186ad845c90e035dbcc13ad22c90c787c7769`  
		Last Modified: Thu, 27 Jan 2022 02:33:32 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; arm variant v5

```console
$ docker pull spiped@sha256:d35164b325c8b4cebf396e69ccd1cb2f1c7c2c813f1645f3a9d7fa533a214761
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.9 MB (33940215 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7d587f5e0871df03606d30179c325953573c55459a421e180a9ef24904dddb49`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 26 Jan 2022 01:41:57 GMT
ADD file:4ccea3cb033595f7bd9896126e94a8a19199b987bedd87b3c0700d8b29baa1fb in / 
# Wed, 26 Jan 2022 01:41:58 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 13:48:20 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 26 Jan 2022 13:48:29 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 13:48:30 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 26 Jan 2022 13:49:20 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 26 Jan 2022 13:49:21 GMT
VOLUME [/spiped]
# Wed, 26 Jan 2022 13:49:21 GMT
WORKDIR /spiped
# Wed, 26 Jan 2022 13:49:22 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 26 Jan 2022 13:49:23 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 26 Jan 2022 13:49:23 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:247ff78919074ec9db7cccd537dd6eb4d7e2788013b7ef07443e345d91c8a588`  
		Last Modified: Wed, 26 Jan 2022 01:57:36 GMT  
		Size: 28.9 MB (28909638 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cf343e822da1ce4be935758169ff31bce470bf1fe1276540174154bb3f2668d`  
		Last Modified: Wed, 26 Jan 2022 13:49:57 GMT  
		Size: 1.7 KB (1727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c398ac3bf4e12d1412bc45d6f9286f5c1700b12eaa24f0978ff6ab2197fe87d`  
		Last Modified: Wed, 26 Jan 2022 13:49:57 GMT  
		Size: 1.1 KB (1051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:797b9d89af1464c4395401f548e40c856ec3fb4894d839f6f9f420a1e2028f16`  
		Last Modified: Wed, 26 Jan 2022 13:50:02 GMT  
		Size: 5.0 MB (5027326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81ef5c7608dbb1e039ea48a4ffc9bac9710189cf564f106cb68cead03b7e4253`  
		Last Modified: Wed, 26 Jan 2022 13:49:57 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb5277a969518e6a9f8d7485c29504d113db9236a9d49b296bd38c4d422c67ea`  
		Last Modified: Wed, 26 Jan 2022 13:49:57 GMT  
		Size: 344.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; arm variant v7

```console
$ docker pull spiped@sha256:3d916238fd77df17911ab19dc7587e33dd0cada5997bb822a6341b6bc4d22d8e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.3 MB (31315488 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c1f89cc56381f998f2473d68073ecab8c87f42eaa6bc2bfeef9e59d7cffaef6f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 26 Jan 2022 01:42:08 GMT
ADD file:7f27f5b43b7cb04e509fe145266d9bdeacfcacb024cafac32e57ef1c831d5ea7 in / 
# Wed, 26 Jan 2022 01:42:09 GMT
CMD ["bash"]
# Thu, 27 Jan 2022 02:05:29 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Thu, 27 Jan 2022 02:05:36 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Thu, 27 Jan 2022 02:05:37 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 27 Jan 2022 02:06:23 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 27 Jan 2022 02:06:24 GMT
VOLUME [/spiped]
# Thu, 27 Jan 2022 02:06:24 GMT
WORKDIR /spiped
# Thu, 27 Jan 2022 02:06:25 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 27 Jan 2022 02:06:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 27 Jan 2022 02:06:26 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:aaef1f1162ec03e01b5b955d41da400544ec2374093ae3dbc330ab2bb36df3e1`  
		Last Modified: Wed, 26 Jan 2022 01:57:59 GMT  
		Size: 26.6 MB (26564933 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b839df330fe51f570a9646e1b8027ad2653336fbd121c12312e0baddcad0d5cd`  
		Last Modified: Thu, 27 Jan 2022 02:07:27 GMT  
		Size: 1.7 KB (1727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b58b2cda412f0922939bcdd348b6d2e3cd4dccd6036926ca90ec596a1b13fbf2`  
		Last Modified: Thu, 27 Jan 2022 02:07:27 GMT  
		Size: 1.1 KB (1051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3936070b02fda979073a59e440e1fb34695f2a5ab92ee369696afed5e3937b5`  
		Last Modified: Thu, 27 Jan 2022 02:07:32 GMT  
		Size: 4.7 MB (4747305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4dd327a7a9576943baaf60df0bdb6ff237147bcfd0f8ee37cf0a591a60131946`  
		Last Modified: Thu, 27 Jan 2022 02:07:27 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60e3ddb56b8bd24d775b3c0d169d4a1a1e03f18562970b41a9d187bc0b0161d8`  
		Last Modified: Thu, 27 Jan 2022 02:07:27 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:ec801aacab912356ed8782ef99c1d53dea85c30a74b6c982e1c33ab60cf936f5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.3 MB (35329660 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5ec3eef7cdb77d28d34401d13e367b0a1ae12678889d9b3df643c3baf3b58b27`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 26 Jan 2022 01:42:31 GMT
ADD file:0ec6f47a8857bf8e6cef71ed8f864be7ce1790ff6ed04fd4201e7dbde4728d3a in / 
# Wed, 26 Jan 2022 01:42:31 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 09:19:54 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 26 Jan 2022 09:19:57 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 09:19:57 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 26 Jan 2022 09:20:14 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 26 Jan 2022 09:20:15 GMT
VOLUME [/spiped]
# Wed, 26 Jan 2022 09:20:16 GMT
WORKDIR /spiped
# Wed, 26 Jan 2022 09:20:18 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 26 Jan 2022 09:20:18 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 26 Jan 2022 09:20:19 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:8998bd30e6a1204d13403045766edbe14f941b52087465f5d140ab63c8b113bf`  
		Last Modified: Wed, 26 Jan 2022 01:49:04 GMT  
		Size: 30.1 MB (30056774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5c0deb70595215cef3194a8d1bea35a623260a4a537174ac0174e9388d20b66`  
		Last Modified: Wed, 26 Jan 2022 09:20:48 GMT  
		Size: 1.6 KB (1618 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:034b8f66f1f2f1b93a71339b2b1c5e595c4574868f5e7d0f06f2c0bf51174940`  
		Last Modified: Wed, 26 Jan 2022 09:20:48 GMT  
		Size: 923.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b14f060bef623dc32f29a79d5b26a6879c4aa9267e5b87ecf4ce0e10f5dfb170`  
		Last Modified: Wed, 26 Jan 2022 09:20:49 GMT  
		Size: 5.3 MB (5269907 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99a6c1e6b86dbfff40179fb98822e12212a0b2867e6d5240159c942eb3854996`  
		Last Modified: Wed, 26 Jan 2022 09:20:47 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce3566ea2e7139f3188bf62015b6b85e2bb8e4c6c1ad89ef5c389ef067c3c0c2`  
		Last Modified: Wed, 26 Jan 2022 09:20:48 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; 386

```console
$ docker pull spiped@sha256:d62c6f333ea8dc55c74566a02c6966fdb05a5373f946c62e78dc4535e7c6439b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.3 MB (40272052 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:240f8e63cba198164b163f99564af3065d0d08a532f87c59c4fafe8bc87fee95`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 26 Jan 2022 01:39:55 GMT
ADD file:876ebf07c65841f4840842086c883af48e07386964fe6d643ba193895ec2a582 in / 
# Wed, 26 Jan 2022 01:39:56 GMT
CMD ["bash"]
# Thu, 27 Jan 2022 04:50:43 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Thu, 27 Jan 2022 04:50:51 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Thu, 27 Jan 2022 04:50:52 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 27 Jan 2022 04:51:42 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 27 Jan 2022 04:51:43 GMT
VOLUME [/spiped]
# Thu, 27 Jan 2022 04:51:43 GMT
WORKDIR /spiped
# Thu, 27 Jan 2022 04:51:44 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 27 Jan 2022 04:51:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 27 Jan 2022 04:51:45 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:86933886b1754aba091548cf031a9bca88cdce9bb4fc1f28bb38b61594c2c2c7`  
		Last Modified: Wed, 26 Jan 2022 01:48:57 GMT  
		Size: 32.4 MB (32377406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:007b643ac135004248e51a7df9b02d61247a5ace740507e11d1238f5c6559f0a`  
		Last Modified: Thu, 27 Jan 2022 04:52:38 GMT  
		Size: 1.7 KB (1729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe9889a275b3dcd9c9d9380a6b23eff3430e0928931f872c594a56aca75b74a0`  
		Last Modified: Thu, 27 Jan 2022 04:52:37 GMT  
		Size: 1.1 KB (1052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a8f1418eeaf635a0d7c0ff4a2a9200da488617f0d749336ec280dc483d43299`  
		Last Modified: Thu, 27 Jan 2022 04:52:41 GMT  
		Size: 7.9 MB (7891393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edd6784674f4cacc537045d525761932e2f277aa61bb5029896a120518807d30`  
		Last Modified: Thu, 27 Jan 2022 04:52:38 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4489e826d0a9aaec6002d3f886c71d2e729d1a47b745a9a82bbdae810d0345f2`  
		Last Modified: Thu, 27 Jan 2022 04:52:37 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; mips64le

```console
$ docker pull spiped@sha256:5ff06e4c09b7b50640a863ff273ef3b49b36efa00ee15a15bc68e0d0c9c31d4c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.3 MB (35341414 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:13ee9a2841cd7deb5c6e19a80d798eaf34ac36066234c76dd87975bb8adbaa97`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 26 Jan 2022 01:42:45 GMT
ADD file:61767027a5ab46afbcd4079d200abe8d663326adc96fa28ca8c8955a06d9322e in / 
# Wed, 26 Jan 2022 01:42:46 GMT
CMD ["bash"]
# Thu, 27 Jan 2022 14:17:20 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Thu, 27 Jan 2022 14:17:32 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Thu, 27 Jan 2022 14:17:32 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 27 Jan 2022 14:18:22 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 27 Jan 2022 14:18:22 GMT
VOLUME [/spiped]
# Thu, 27 Jan 2022 14:18:23 GMT
WORKDIR /spiped
# Thu, 27 Jan 2022 14:18:23 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 27 Jan 2022 14:18:23 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 27 Jan 2022 14:18:24 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:266e7d2b59483859eaa1711d2afeb25ea4458eeb36b3e909372930db1f834d7f`  
		Last Modified: Wed, 26 Jan 2022 01:51:23 GMT  
		Size: 29.6 MB (29632834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bed329584043834b57b17c1f7fb178849a18c1e185f6a1c3790d7e4f3aabdad`  
		Last Modified: Thu, 27 Jan 2022 14:18:40 GMT  
		Size: 1.7 KB (1732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1221de7514f3a6d44d793ddbb512b55c28feed96691f900bce757c1ad89f2db`  
		Last Modified: Thu, 27 Jan 2022 14:18:41 GMT  
		Size: 1.0 KB (1026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b78ea45f3c4a37e62bd246764fe6840be44718f3a906daf70e4d583cf4aaa6af`  
		Last Modified: Thu, 27 Jan 2022 14:18:46 GMT  
		Size: 5.7 MB (5705384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53d16d14491067074a517e226e1dced4190135104702609415f883fa63d46ee3`  
		Last Modified: Thu, 27 Jan 2022 14:18:41 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2dba9fb9a37e3aafad3abba08e85db2fd96587c52de4e6a2df6ef442c2538a96`  
		Last Modified: Thu, 27 Jan 2022 14:18:40 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; ppc64le

```console
$ docker pull spiped@sha256:f9a8ff652bffe474afdf6cf3da90bcb5fabc4674ad021bc3ddf11100309fcbe7
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.3 MB (41274405 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b89132621e69403b6931ac29ab0fdf93d27e91888256b85a1de6d142d4046a56`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 26 Jan 2022 01:46:51 GMT
ADD file:c03f34c221e57fa5cb625c166d1db9f72d6ba2fa17a3c41a5d04d6875d098949 in / 
# Wed, 26 Jan 2022 01:46:57 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 22:15:10 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 26 Jan 2022 22:15:19 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 22:15:21 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 26 Jan 2022 22:17:04 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 26 Jan 2022 22:17:09 GMT
VOLUME [/spiped]
# Wed, 26 Jan 2022 22:17:12 GMT
WORKDIR /spiped
# Wed, 26 Jan 2022 22:17:14 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 26 Jan 2022 22:17:16 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 26 Jan 2022 22:17:20 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:3149ee4a73508a4c39107d64a3fdc1b021626a22a0ac95e62fa0cea49ab77fba`  
		Last Modified: Wed, 26 Jan 2022 01:57:01 GMT  
		Size: 35.3 MB (35273030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43b54b67a6f99dac2db476b7702d015eb56f81c2d623bc96fd32aae703f0b732`  
		Last Modified: Wed, 26 Jan 2022 22:17:51 GMT  
		Size: 1.7 KB (1739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f1241c00e00d3316ad39effb0518ce815abfcf876ea4efac9de53b2fdc560da`  
		Last Modified: Wed, 26 Jan 2022 22:17:51 GMT  
		Size: 1.1 KB (1054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86ddc628c1bd5eff84e7cb044e5c93444f7e53a189710ec4b2f0213ffc82cb0f`  
		Last Modified: Wed, 26 Jan 2022 22:17:53 GMT  
		Size: 6.0 MB (5998110 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:706174d608bd436d8e8d5fb2c9d2cb2ff6ea71118584ab8a35af39ae43d5d90f`  
		Last Modified: Wed, 26 Jan 2022 22:17:51 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7858b7298d1ed34eff1ac6724d4bce1c8fc696786a68d28c115f2bc843aad9ab`  
		Last Modified: Wed, 26 Jan 2022 22:17:51 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; s390x

```console
$ docker pull spiped@sha256:dc9f30aec35bbc203643e902934a1b5e6140c26c166e0462f571d07f09e3fab5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.8 MB (34836084 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:40e931303d1bd986c9a5293d6f7f2f3dc4a9599d5af26cc8a933a43253c32f21`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 26 Jan 2022 01:41:13 GMT
ADD file:03b224b82f458b08d3b5071e42b67915a3db309332c0fc9229db7cf1148bc1b5 in / 
# Wed, 26 Jan 2022 01:41:15 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 11:27:45 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 26 Jan 2022 11:27:47 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 11:27:48 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 26 Jan 2022 11:28:01 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 26 Jan 2022 11:28:01 GMT
VOLUME [/spiped]
# Wed, 26 Jan 2022 11:28:02 GMT
WORKDIR /spiped
# Wed, 26 Jan 2022 11:28:02 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 26 Jan 2022 11:28:02 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 26 Jan 2022 11:28:02 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:70bed29526f8483937e4d2540d19256d30786007c7c321e717e00d2e74700380`  
		Last Modified: Wed, 26 Jan 2022 01:46:57 GMT  
		Size: 29.6 MB (29647071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87ff2a6a6375f95aac16175fe1a27e34e664c34d69d5ed1efa5d976ad0e7b947`  
		Last Modified: Wed, 26 Jan 2022 11:28:34 GMT  
		Size: 1.7 KB (1736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66b439c0f82c7b1a5745542aedc040eca1c81fae487012b1886220413a47d903`  
		Last Modified: Wed, 26 Jan 2022 11:28:34 GMT  
		Size: 1.1 KB (1052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93908f45004e2f2d6aee48dec977a4e4405bf91858cafb05024b750ca56aa9d7`  
		Last Modified: Wed, 26 Jan 2022 11:28:35 GMT  
		Size: 5.2 MB (5185752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9c094f1ad2a6f023f6f79a11bb9a375b3f52a100501b0d1191d839085802bba`  
		Last Modified: Wed, 26 Jan 2022 11:28:34 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83eccc997a02a9c670eaa7e3d2dfd923453818685f1b2c3ddfff0bf985a890d4`  
		Last Modified: Wed, 26 Jan 2022 11:28:34 GMT  
		Size: 344.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:1-alpine`

```console
$ docker pull spiped@sha256:b1089d3c383de79c5a463d8f6b45c46f804588a33a967ff66469a76a654169f0
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
$ docker pull spiped@sha256:f4aaae543ff5aba181d531aa5504251d883a40559812a85cff78c7526d3f713e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4523758 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d71e35e9a762b19f1a767061f3cf181454d7090d64dec7acef852f68d4c01262`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 24 Nov 2021 20:19:40 GMT
ADD file:9233f6f2237d79659a9521f7e390df217cec49f1a8aa3a12147bbca1956acdb9 in / 
# Wed, 24 Nov 2021 20:19:40 GMT
CMD ["/bin/sh"]
# Mon, 27 Dec 2021 19:10:10 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Mon, 27 Dec 2021 19:10:11 GMT
RUN apk add --no-cache libssl1.1
# Mon, 27 Dec 2021 19:10:11 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Mon, 27 Dec 2021 19:10:22 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Mon, 27 Dec 2021 19:10:22 GMT
VOLUME [/spiped]
# Mon, 27 Dec 2021 19:10:22 GMT
WORKDIR /spiped
# Mon, 27 Dec 2021 19:10:22 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 27 Dec 2021 19:10:23 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 27 Dec 2021 19:10:23 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:59bf1c3509f33515622619af21ed55bbe26d24913cedbca106468a5fb37a50c3`  
		Last Modified: Wed, 24 Nov 2021 20:20:05 GMT  
		Size: 2.8 MB (2818413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50c602680384586a0fe7febde9f529aea001928a6d26e84d9a3f7be94049ef27`  
		Last Modified: Mon, 27 Dec 2021 19:10:53 GMT  
		Size: 1.3 KB (1265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee913a58b01d029ed458f92226b5b52747e0877c39585d9f93ec5dd2ef0a8cf9`  
		Last Modified: Mon, 27 Dec 2021 19:10:53 GMT  
		Size: 7.7 KB (7749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd8bf950f1ef1b7c96ba1781b5a87d4044135ae197871b261e86d74bc35a8bf5`  
		Last Modified: Mon, 27 Dec 2021 19:10:54 GMT  
		Size: 1.7 MB (1695862 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56d41f282509324afd98cc83dab31aee8ba6459973698c8ccaf3978cddc4ede4`  
		Last Modified: Mon, 27 Dec 2021 19:10:53 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8ba766abbc809d26737c9cc94fbe15a6311c603bfd673bd6db553169dd0f141`  
		Last Modified: Mon, 27 Dec 2021 19:10:53 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; arm variant v6

```console
$ docker pull spiped@sha256:b6482b55d0b7700b0393783f0ea8e49e6a4329c07187fdf826b6902d0ccfa3e6
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.1 MB (4080480 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1df9593d1c7a93c5f606ef97c05cc8d86e1a5bce25cd9895c104e2e1a7edbe19`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 24 Nov 2021 21:08:16 GMT
ADD file:61137e0aa49ba06f57ac69466fe2fb116f580b5e6159d56f846b1d72c4a3c814 in / 
# Wed, 24 Nov 2021 21:08:16 GMT
CMD ["/bin/sh"]
# Mon, 27 Dec 2021 17:49:44 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Mon, 27 Dec 2021 17:49:46 GMT
RUN apk add --no-cache libssl1.1
# Mon, 27 Dec 2021 17:49:47 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Mon, 27 Dec 2021 17:50:06 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Mon, 27 Dec 2021 17:50:07 GMT
VOLUME [/spiped]
# Mon, 27 Dec 2021 17:50:07 GMT
WORKDIR /spiped
# Mon, 27 Dec 2021 17:50:08 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 27 Dec 2021 17:50:08 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 27 Dec 2021 17:50:09 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:e4a43de54da9e309482f6762f0c11f5f547cd8fd61a49c5f158453066162023e`  
		Last Modified: Wed, 24 Nov 2021 21:09:46 GMT  
		Size: 2.6 MB (2631421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c04f27a458746dfc1d07b0b03b9b8f205b08ebef9d6060ef92027b709fee313e`  
		Last Modified: Mon, 27 Dec 2021 17:50:41 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fffa3b0ec9bb32d2efab9fa903af078baf37201f4ec2026c0afce9c14156229`  
		Last Modified: Mon, 27 Dec 2021 17:50:41 GMT  
		Size: 7.7 KB (7743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e2344d51f830abe738f710343c04e056b2ec80e33a48522878caa568c9f553c`  
		Last Modified: Mon, 27 Dec 2021 17:50:42 GMT  
		Size: 1.4 MB (1439576 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd3eeeb2545dce6884a99d866ca20bd742d7e133aacf869b4cddbe974bfde627`  
		Last Modified: Mon, 27 Dec 2021 17:50:41 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2681e39729f29c202bc97138be5a28bb84d92220ffe45df47fb643301eef46aa`  
		Last Modified: Mon, 27 Dec 2021 17:50:41 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; arm variant v7

```console
$ docker pull spiped@sha256:277d22d33ab8cd23ff5bf04d4e60841c8a335de8fdb772173601e9a4d4cb00bf
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.8 MB (3802328 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2f94c64b2c706a58b82aa60bafca69c1fd15fb76714e5ca4aae0f1e4a47e3f1d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 24 Nov 2021 21:42:11 GMT
ADD file:ca436da5b0bfc9c0e2fc685533c6628918000c8fff109fe9a8da625b9a798002 in / 
# Wed, 24 Nov 2021 21:42:11 GMT
CMD ["/bin/sh"]
# Mon, 27 Dec 2021 18:00:04 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Mon, 27 Dec 2021 18:00:06 GMT
RUN apk add --no-cache libssl1.1
# Mon, 27 Dec 2021 18:00:06 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Mon, 27 Dec 2021 18:00:25 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Mon, 27 Dec 2021 18:00:26 GMT
VOLUME [/spiped]
# Mon, 27 Dec 2021 18:00:26 GMT
WORKDIR /spiped
# Mon, 27 Dec 2021 18:00:27 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 27 Dec 2021 18:00:27 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 27 Dec 2021 18:00:28 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:5480d2ca1740c20ce17652e01ed2265cdc914458acd41256a2b1ccff28f2762c`  
		Last Modified: Wed, 24 Nov 2021 21:43:40 GMT  
		Size: 2.4 MB (2434764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fca194041621ab40d8e7f24b7f7e82aa07760b2dafcd26472bd7fae96171989a`  
		Last Modified: Mon, 27 Dec 2021 18:01:41 GMT  
		Size: 1.3 KB (1267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7e934f04cb0ca6a107389bcb614eb02143fb079eef09a47a9248e3c4ff07864`  
		Last Modified: Mon, 27 Dec 2021 18:01:41 GMT  
		Size: 7.7 KB (7749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4111e5d44f2316d799c8b9144d8f35765b0bf330b8d596d99e504969cd48e07a`  
		Last Modified: Mon, 27 Dec 2021 18:01:42 GMT  
		Size: 1.4 MB (1358077 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f46d751b026ad913b2a48630c96460959a733e75728d55aafbd389197bf81857`  
		Last Modified: Mon, 27 Dec 2021 18:01:41 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5140561b01c4c6ae8b47c729fd289d7eef4a2b0e9c427a6bd35a86747e966206`  
		Last Modified: Mon, 27 Dec 2021 18:01:41 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:f2401c455a0fde4f25cae4b46bad0721c19ac135bc6efa4e5b3c46c5b04aa1cd
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.3 MB (4289462 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:017a5c1ca8bdf46589e6ab7b72a939d86283ebdb51f63d37bc1c41f07a36600f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 24 Nov 2021 20:39:20 GMT
ADD file:df53811312284306901fdaaff0a357a4bf40d631e662fe9ce6d342442e494b6c in / 
# Wed, 24 Nov 2021 20:39:20 GMT
CMD ["/bin/sh"]
# Mon, 27 Dec 2021 19:39:28 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Mon, 27 Dec 2021 19:39:29 GMT
RUN apk add --no-cache libssl1.1
# Mon, 27 Dec 2021 19:39:30 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Mon, 27 Dec 2021 19:39:41 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Mon, 27 Dec 2021 19:39:42 GMT
VOLUME [/spiped]
# Mon, 27 Dec 2021 19:39:43 GMT
WORKDIR /spiped
# Mon, 27 Dec 2021 19:39:45 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 27 Dec 2021 19:39:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 27 Dec 2021 19:39:46 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:9b3977197b4f2147bdd31e1271f811319dcd5c2fc595f14e81f5351ab6275b99`  
		Last Modified: Wed, 24 Nov 2021 20:39:59 GMT  
		Size: 2.7 MB (2715434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4642588fd355ccb1af1d6dc41cc14b5117bbd4f30adb691aade26686c4d5c116`  
		Last Modified: Mon, 27 Dec 2021 19:40:28 GMT  
		Size: 1.2 KB (1240 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd8e58927c1555e9461b11588b3accaf4b9d1018264a3d1ac75dbd1d03c2212e`  
		Last Modified: Mon, 27 Dec 2021 19:40:28 GMT  
		Size: 7.7 KB (7712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd181fff8bea1f7e317b2af57ee7244e2a0b5226b26df42dc9a9d836cf504dec`  
		Last Modified: Mon, 27 Dec 2021 19:40:28 GMT  
		Size: 1.6 MB (1564638 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f65407c84c38d42d7b099c55334ee34fc2e9f581954ed4e92bab1773599189df`  
		Last Modified: Mon, 27 Dec 2021 19:40:28 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97f56c7d1e54220168de3e0523afd6a69f29f86199d05ee4681c356afaa2e36a`  
		Last Modified: Mon, 27 Dec 2021 19:40:28 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; 386

```console
$ docker pull spiped@sha256:fc962e82018b393667a7d2b43c9bee0b19c4650fadcc16335cf984b44d859d65
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4539662 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:64dc6529164f107ee83f0edafa6bcf506960ffc646e0e9e161cb2640feb90f96`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 24 Nov 2021 20:53:48 GMT
ADD file:b9a17131c440053f2f67e127b447645f25fd7de2d6caca42f569cafab6291855 in / 
# Wed, 24 Nov 2021 20:53:48 GMT
CMD ["/bin/sh"]
# Mon, 27 Dec 2021 18:39:31 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Mon, 27 Dec 2021 18:39:32 GMT
RUN apk add --no-cache libssl1.1
# Mon, 27 Dec 2021 18:39:33 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Mon, 27 Dec 2021 18:39:45 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Mon, 27 Dec 2021 18:39:45 GMT
VOLUME [/spiped]
# Mon, 27 Dec 2021 18:39:45 GMT
WORKDIR /spiped
# Mon, 27 Dec 2021 18:39:46 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 27 Dec 2021 18:39:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 27 Dec 2021 18:39:46 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:e6889e0d66307a4b916fc844f2dcbc03245c63bc4189dd3e88126d9dcf2f9231`  
		Last Modified: Wed, 24 Nov 2021 20:54:48 GMT  
		Size: 2.8 MB (2827117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc39bdf14cf5dcbf704b50f736d82a339b1879574765ef87fbbf5ecb8d7d574e`  
		Last Modified: Mon, 27 Dec 2021 18:40:32 GMT  
		Size: 1.3 KB (1266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7128f9e1b03ce01ba1b51bce7aa1bc585b6c3e6ce1650259721463f363e9aaab`  
		Last Modified: Mon, 27 Dec 2021 18:40:32 GMT  
		Size: 7.8 KB (7750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb2ebf4c9a2525659cebde6ee501a457c4a31d364f3f568be0f076191d96855d`  
		Last Modified: Mon, 27 Dec 2021 18:40:33 GMT  
		Size: 1.7 MB (1703060 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75adf8fe66ad441b9c8e209efcc7d5b68b61c6a33e05b3aed401756e55493d07`  
		Last Modified: Mon, 27 Dec 2021 18:40:32 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99b656b54398310f3a0f295c7737034732b9ee5c7e294ad5df27230309fff8ae`  
		Last Modified: Mon, 27 Dec 2021 18:40:32 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; ppc64le

```console
$ docker pull spiped@sha256:bdb5c0f748fb29dd4c96f71d1eec1c471f348b68e39063a5674e88c6655400ac
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.4 MB (4447359 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c2ab0ba82f0f9badd5246249195a67d4e12bc4f6cfb1822b3454aca1c3dae586`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 24 Nov 2021 20:20:16 GMT
ADD file:57115dca2eb707f46b6301e75174e6aa316fb02ac28643b91429b75be51bd8c8 in / 
# Wed, 24 Nov 2021 20:20:20 GMT
CMD ["/bin/sh"]
# Mon, 27 Dec 2021 18:18:59 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Mon, 27 Dec 2021 18:19:06 GMT
RUN apk add --no-cache libssl1.1
# Mon, 27 Dec 2021 18:19:08 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Mon, 27 Dec 2021 18:19:22 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Mon, 27 Dec 2021 18:19:25 GMT
VOLUME [/spiped]
# Mon, 27 Dec 2021 18:19:28 GMT
WORKDIR /spiped
# Mon, 27 Dec 2021 18:19:28 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 27 Dec 2021 18:19:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 27 Dec 2021 18:19:33 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:159b5dcb1717c815c76ff5ea1db730e18e8609c9090238e43282856db9e71f47`  
		Last Modified: Wed, 24 Nov 2021 20:21:14 GMT  
		Size: 2.8 MB (2814780 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5ef2b17ec4445a63d712289fc62b0e3e30ab15992e0a0d38ab25e290abcb38e`  
		Last Modified: Mon, 27 Dec 2021 18:20:21 GMT  
		Size: 1.3 KB (1274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:210460e69fcfc508eae94f5666c4fc57c0cdf6163c3a6e39710f5da7a2e5ceb6`  
		Last Modified: Mon, 27 Dec 2021 18:20:21 GMT  
		Size: 7.7 KB (7737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0860c3c69dcd2673558f15fc9c46c8447274ce23c207e936804fe5a268e5e7f`  
		Last Modified: Mon, 27 Dec 2021 18:20:22 GMT  
		Size: 1.6 MB (1623097 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13cd96844150db5d01e32349b5f650aafd01dd1789c2a11fee82b6f55bd43560`  
		Last Modified: Mon, 27 Dec 2021 18:20:21 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a52b1de785dfc0bc3d07ee3d3f619d0681bc34b7eeee205db16da01946663a91`  
		Last Modified: Mon, 27 Dec 2021 18:20:21 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; s390x

```console
$ docker pull spiped@sha256:e5972c57d035e42883aca7354deb92cd65a9bbbc8d5d6aaa8b364891cbdba20d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.0 MB (4034365 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6b297cc2c896c2d11d20abe50ce763f606504b9aad55d18a6c8bcf3407db63c8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 24 Nov 2021 20:41:23 GMT
ADD file:cd24c711a2ef431b3ff94f9a02bfc42f159bc60de1d0eceecafea4e8af02441d in / 
# Wed, 24 Nov 2021 20:41:23 GMT
CMD ["/bin/sh"]
# Mon, 27 Dec 2021 18:42:02 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Mon, 27 Dec 2021 18:42:04 GMT
RUN apk add --no-cache libssl1.1
# Mon, 27 Dec 2021 18:42:04 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Mon, 27 Dec 2021 18:42:09 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Mon, 27 Dec 2021 18:42:09 GMT
VOLUME [/spiped]
# Mon, 27 Dec 2021 18:42:09 GMT
WORKDIR /spiped
# Mon, 27 Dec 2021 18:42:10 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 27 Dec 2021 18:42:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 27 Dec 2021 18:42:10 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:d6baca485f3d0f7c77221be60fbef5db014a5ef9d8f53db4a310c947c690d189`  
		Last Modified: Wed, 24 Nov 2021 20:42:15 GMT  
		Size: 2.6 MB (2605944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:631b52683dec736314bc4a995e6d4aa8fe70ccec0ccb0b4f0349543c0b9d315d`  
		Last Modified: Mon, 27 Dec 2021 18:42:54 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8a99397842c922d6589a78e8df8f8b4feac626485047c36e902a2966e19dfe2`  
		Last Modified: Mon, 27 Dec 2021 18:42:54 GMT  
		Size: 7.7 KB (7743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:556dc6882e78ba3518dbab7eaae8412b06f9ad7e09122f6478d9d1cc80b978e4`  
		Last Modified: Mon, 27 Dec 2021 18:42:55 GMT  
		Size: 1.4 MB (1418939 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9680c33180071ffeb1ac5cfe629daff266a5cf86a4072e251e4b0bef70d20b3`  
		Last Modified: Mon, 27 Dec 2021 18:42:54 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2742416115dba0ead2f2dc1f9aa438a1ef9179b4e11cfd9d665c918f92b53c55`  
		Last Modified: Mon, 27 Dec 2021 18:42:54 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:1.6`

```console
$ docker pull spiped@sha256:d9abc65404acc410b3f94bd812f875d66ad7304604f00ee6464be3ab291d57b3
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
$ docker pull spiped@sha256:dc2c3a3712eacb11a556c86bc2a6b606ba5a0edff87bf3638c159b85a1135448
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.3 MB (37335950 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1d472f594ea8090d6f3cbeb573986f7840e512b983c9def18699f62efe8bcc04`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 26 Jan 2022 01:40:35 GMT
ADD file:90495c24c897ec47982e200f732f8be3109fcd791691ddffae0756898f91024f in / 
# Wed, 26 Jan 2022 01:40:36 GMT
CMD ["bash"]
# Thu, 27 Jan 2022 02:32:24 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Thu, 27 Jan 2022 02:32:27 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Thu, 27 Jan 2022 02:32:28 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 27 Jan 2022 02:32:58 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 27 Jan 2022 02:32:58 GMT
VOLUME [/spiped]
# Thu, 27 Jan 2022 02:32:59 GMT
WORKDIR /spiped
# Thu, 27 Jan 2022 02:33:00 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 27 Jan 2022 02:33:00 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 27 Jan 2022 02:33:01 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:5eb5b503b37671af16371272f9c5313a3e82f1d0756e14506704489ad9900803`  
		Last Modified: Wed, 26 Jan 2022 01:46:39 GMT  
		Size: 31.4 MB (31366257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6a2517caec378bb5ccef0a0d6e52b5e25a629d59a240188bd605cf9f98bc57d`  
		Last Modified: Thu, 27 Jan 2022 02:33:32 GMT  
		Size: 1.7 KB (1734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9824d58dd5193ef98f897a6ac1feb9749d5f2371324023d2ca61dae51fb70e6`  
		Last Modified: Thu, 27 Jan 2022 02:33:32 GMT  
		Size: 1.1 KB (1051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d878a5544ecf1374c1348226765bcdd58a98e4e3d4c98f89ccf5fa10a7ca8ff`  
		Last Modified: Thu, 27 Jan 2022 02:33:34 GMT  
		Size: 6.0 MB (5966436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:754c3acbb4e4a2d6ba3fb19ebf6f464a6af124ca39e832916a9e20959ba6cb46`  
		Last Modified: Thu, 27 Jan 2022 02:33:32 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ddcc8c75157adfeb6f31357486186ad845c90e035dbcc13ad22c90c787c7769`  
		Last Modified: Thu, 27 Jan 2022 02:33:32 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; arm variant v5

```console
$ docker pull spiped@sha256:d35164b325c8b4cebf396e69ccd1cb2f1c7c2c813f1645f3a9d7fa533a214761
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.9 MB (33940215 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7d587f5e0871df03606d30179c325953573c55459a421e180a9ef24904dddb49`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 26 Jan 2022 01:41:57 GMT
ADD file:4ccea3cb033595f7bd9896126e94a8a19199b987bedd87b3c0700d8b29baa1fb in / 
# Wed, 26 Jan 2022 01:41:58 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 13:48:20 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 26 Jan 2022 13:48:29 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 13:48:30 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 26 Jan 2022 13:49:20 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 26 Jan 2022 13:49:21 GMT
VOLUME [/spiped]
# Wed, 26 Jan 2022 13:49:21 GMT
WORKDIR /spiped
# Wed, 26 Jan 2022 13:49:22 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 26 Jan 2022 13:49:23 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 26 Jan 2022 13:49:23 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:247ff78919074ec9db7cccd537dd6eb4d7e2788013b7ef07443e345d91c8a588`  
		Last Modified: Wed, 26 Jan 2022 01:57:36 GMT  
		Size: 28.9 MB (28909638 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cf343e822da1ce4be935758169ff31bce470bf1fe1276540174154bb3f2668d`  
		Last Modified: Wed, 26 Jan 2022 13:49:57 GMT  
		Size: 1.7 KB (1727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c398ac3bf4e12d1412bc45d6f9286f5c1700b12eaa24f0978ff6ab2197fe87d`  
		Last Modified: Wed, 26 Jan 2022 13:49:57 GMT  
		Size: 1.1 KB (1051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:797b9d89af1464c4395401f548e40c856ec3fb4894d839f6f9f420a1e2028f16`  
		Last Modified: Wed, 26 Jan 2022 13:50:02 GMT  
		Size: 5.0 MB (5027326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81ef5c7608dbb1e039ea48a4ffc9bac9710189cf564f106cb68cead03b7e4253`  
		Last Modified: Wed, 26 Jan 2022 13:49:57 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb5277a969518e6a9f8d7485c29504d113db9236a9d49b296bd38c4d422c67ea`  
		Last Modified: Wed, 26 Jan 2022 13:49:57 GMT  
		Size: 344.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; arm variant v7

```console
$ docker pull spiped@sha256:3d916238fd77df17911ab19dc7587e33dd0cada5997bb822a6341b6bc4d22d8e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.3 MB (31315488 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c1f89cc56381f998f2473d68073ecab8c87f42eaa6bc2bfeef9e59d7cffaef6f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 26 Jan 2022 01:42:08 GMT
ADD file:7f27f5b43b7cb04e509fe145266d9bdeacfcacb024cafac32e57ef1c831d5ea7 in / 
# Wed, 26 Jan 2022 01:42:09 GMT
CMD ["bash"]
# Thu, 27 Jan 2022 02:05:29 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Thu, 27 Jan 2022 02:05:36 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Thu, 27 Jan 2022 02:05:37 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 27 Jan 2022 02:06:23 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 27 Jan 2022 02:06:24 GMT
VOLUME [/spiped]
# Thu, 27 Jan 2022 02:06:24 GMT
WORKDIR /spiped
# Thu, 27 Jan 2022 02:06:25 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 27 Jan 2022 02:06:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 27 Jan 2022 02:06:26 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:aaef1f1162ec03e01b5b955d41da400544ec2374093ae3dbc330ab2bb36df3e1`  
		Last Modified: Wed, 26 Jan 2022 01:57:59 GMT  
		Size: 26.6 MB (26564933 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b839df330fe51f570a9646e1b8027ad2653336fbd121c12312e0baddcad0d5cd`  
		Last Modified: Thu, 27 Jan 2022 02:07:27 GMT  
		Size: 1.7 KB (1727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b58b2cda412f0922939bcdd348b6d2e3cd4dccd6036926ca90ec596a1b13fbf2`  
		Last Modified: Thu, 27 Jan 2022 02:07:27 GMT  
		Size: 1.1 KB (1051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3936070b02fda979073a59e440e1fb34695f2a5ab92ee369696afed5e3937b5`  
		Last Modified: Thu, 27 Jan 2022 02:07:32 GMT  
		Size: 4.7 MB (4747305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4dd327a7a9576943baaf60df0bdb6ff237147bcfd0f8ee37cf0a591a60131946`  
		Last Modified: Thu, 27 Jan 2022 02:07:27 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60e3ddb56b8bd24d775b3c0d169d4a1a1e03f18562970b41a9d187bc0b0161d8`  
		Last Modified: Thu, 27 Jan 2022 02:07:27 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:ec801aacab912356ed8782ef99c1d53dea85c30a74b6c982e1c33ab60cf936f5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.3 MB (35329660 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5ec3eef7cdb77d28d34401d13e367b0a1ae12678889d9b3df643c3baf3b58b27`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 26 Jan 2022 01:42:31 GMT
ADD file:0ec6f47a8857bf8e6cef71ed8f864be7ce1790ff6ed04fd4201e7dbde4728d3a in / 
# Wed, 26 Jan 2022 01:42:31 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 09:19:54 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 26 Jan 2022 09:19:57 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 09:19:57 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 26 Jan 2022 09:20:14 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 26 Jan 2022 09:20:15 GMT
VOLUME [/spiped]
# Wed, 26 Jan 2022 09:20:16 GMT
WORKDIR /spiped
# Wed, 26 Jan 2022 09:20:18 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 26 Jan 2022 09:20:18 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 26 Jan 2022 09:20:19 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:8998bd30e6a1204d13403045766edbe14f941b52087465f5d140ab63c8b113bf`  
		Last Modified: Wed, 26 Jan 2022 01:49:04 GMT  
		Size: 30.1 MB (30056774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5c0deb70595215cef3194a8d1bea35a623260a4a537174ac0174e9388d20b66`  
		Last Modified: Wed, 26 Jan 2022 09:20:48 GMT  
		Size: 1.6 KB (1618 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:034b8f66f1f2f1b93a71339b2b1c5e595c4574868f5e7d0f06f2c0bf51174940`  
		Last Modified: Wed, 26 Jan 2022 09:20:48 GMT  
		Size: 923.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b14f060bef623dc32f29a79d5b26a6879c4aa9267e5b87ecf4ce0e10f5dfb170`  
		Last Modified: Wed, 26 Jan 2022 09:20:49 GMT  
		Size: 5.3 MB (5269907 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99a6c1e6b86dbfff40179fb98822e12212a0b2867e6d5240159c942eb3854996`  
		Last Modified: Wed, 26 Jan 2022 09:20:47 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce3566ea2e7139f3188bf62015b6b85e2bb8e4c6c1ad89ef5c389ef067c3c0c2`  
		Last Modified: Wed, 26 Jan 2022 09:20:48 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; 386

```console
$ docker pull spiped@sha256:d62c6f333ea8dc55c74566a02c6966fdb05a5373f946c62e78dc4535e7c6439b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.3 MB (40272052 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:240f8e63cba198164b163f99564af3065d0d08a532f87c59c4fafe8bc87fee95`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 26 Jan 2022 01:39:55 GMT
ADD file:876ebf07c65841f4840842086c883af48e07386964fe6d643ba193895ec2a582 in / 
# Wed, 26 Jan 2022 01:39:56 GMT
CMD ["bash"]
# Thu, 27 Jan 2022 04:50:43 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Thu, 27 Jan 2022 04:50:51 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Thu, 27 Jan 2022 04:50:52 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 27 Jan 2022 04:51:42 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 27 Jan 2022 04:51:43 GMT
VOLUME [/spiped]
# Thu, 27 Jan 2022 04:51:43 GMT
WORKDIR /spiped
# Thu, 27 Jan 2022 04:51:44 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 27 Jan 2022 04:51:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 27 Jan 2022 04:51:45 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:86933886b1754aba091548cf031a9bca88cdce9bb4fc1f28bb38b61594c2c2c7`  
		Last Modified: Wed, 26 Jan 2022 01:48:57 GMT  
		Size: 32.4 MB (32377406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:007b643ac135004248e51a7df9b02d61247a5ace740507e11d1238f5c6559f0a`  
		Last Modified: Thu, 27 Jan 2022 04:52:38 GMT  
		Size: 1.7 KB (1729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe9889a275b3dcd9c9d9380a6b23eff3430e0928931f872c594a56aca75b74a0`  
		Last Modified: Thu, 27 Jan 2022 04:52:37 GMT  
		Size: 1.1 KB (1052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a8f1418eeaf635a0d7c0ff4a2a9200da488617f0d749336ec280dc483d43299`  
		Last Modified: Thu, 27 Jan 2022 04:52:41 GMT  
		Size: 7.9 MB (7891393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edd6784674f4cacc537045d525761932e2f277aa61bb5029896a120518807d30`  
		Last Modified: Thu, 27 Jan 2022 04:52:38 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4489e826d0a9aaec6002d3f886c71d2e729d1a47b745a9a82bbdae810d0345f2`  
		Last Modified: Thu, 27 Jan 2022 04:52:37 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; mips64le

```console
$ docker pull spiped@sha256:5ff06e4c09b7b50640a863ff273ef3b49b36efa00ee15a15bc68e0d0c9c31d4c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.3 MB (35341414 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:13ee9a2841cd7deb5c6e19a80d798eaf34ac36066234c76dd87975bb8adbaa97`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 26 Jan 2022 01:42:45 GMT
ADD file:61767027a5ab46afbcd4079d200abe8d663326adc96fa28ca8c8955a06d9322e in / 
# Wed, 26 Jan 2022 01:42:46 GMT
CMD ["bash"]
# Thu, 27 Jan 2022 14:17:20 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Thu, 27 Jan 2022 14:17:32 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Thu, 27 Jan 2022 14:17:32 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 27 Jan 2022 14:18:22 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 27 Jan 2022 14:18:22 GMT
VOLUME [/spiped]
# Thu, 27 Jan 2022 14:18:23 GMT
WORKDIR /spiped
# Thu, 27 Jan 2022 14:18:23 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 27 Jan 2022 14:18:23 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 27 Jan 2022 14:18:24 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:266e7d2b59483859eaa1711d2afeb25ea4458eeb36b3e909372930db1f834d7f`  
		Last Modified: Wed, 26 Jan 2022 01:51:23 GMT  
		Size: 29.6 MB (29632834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bed329584043834b57b17c1f7fb178849a18c1e185f6a1c3790d7e4f3aabdad`  
		Last Modified: Thu, 27 Jan 2022 14:18:40 GMT  
		Size: 1.7 KB (1732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1221de7514f3a6d44d793ddbb512b55c28feed96691f900bce757c1ad89f2db`  
		Last Modified: Thu, 27 Jan 2022 14:18:41 GMT  
		Size: 1.0 KB (1026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b78ea45f3c4a37e62bd246764fe6840be44718f3a906daf70e4d583cf4aaa6af`  
		Last Modified: Thu, 27 Jan 2022 14:18:46 GMT  
		Size: 5.7 MB (5705384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53d16d14491067074a517e226e1dced4190135104702609415f883fa63d46ee3`  
		Last Modified: Thu, 27 Jan 2022 14:18:41 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2dba9fb9a37e3aafad3abba08e85db2fd96587c52de4e6a2df6ef442c2538a96`  
		Last Modified: Thu, 27 Jan 2022 14:18:40 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; ppc64le

```console
$ docker pull spiped@sha256:f9a8ff652bffe474afdf6cf3da90bcb5fabc4674ad021bc3ddf11100309fcbe7
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.3 MB (41274405 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b89132621e69403b6931ac29ab0fdf93d27e91888256b85a1de6d142d4046a56`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 26 Jan 2022 01:46:51 GMT
ADD file:c03f34c221e57fa5cb625c166d1db9f72d6ba2fa17a3c41a5d04d6875d098949 in / 
# Wed, 26 Jan 2022 01:46:57 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 22:15:10 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 26 Jan 2022 22:15:19 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 22:15:21 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 26 Jan 2022 22:17:04 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 26 Jan 2022 22:17:09 GMT
VOLUME [/spiped]
# Wed, 26 Jan 2022 22:17:12 GMT
WORKDIR /spiped
# Wed, 26 Jan 2022 22:17:14 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 26 Jan 2022 22:17:16 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 26 Jan 2022 22:17:20 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:3149ee4a73508a4c39107d64a3fdc1b021626a22a0ac95e62fa0cea49ab77fba`  
		Last Modified: Wed, 26 Jan 2022 01:57:01 GMT  
		Size: 35.3 MB (35273030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43b54b67a6f99dac2db476b7702d015eb56f81c2d623bc96fd32aae703f0b732`  
		Last Modified: Wed, 26 Jan 2022 22:17:51 GMT  
		Size: 1.7 KB (1739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f1241c00e00d3316ad39effb0518ce815abfcf876ea4efac9de53b2fdc560da`  
		Last Modified: Wed, 26 Jan 2022 22:17:51 GMT  
		Size: 1.1 KB (1054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86ddc628c1bd5eff84e7cb044e5c93444f7e53a189710ec4b2f0213ffc82cb0f`  
		Last Modified: Wed, 26 Jan 2022 22:17:53 GMT  
		Size: 6.0 MB (5998110 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:706174d608bd436d8e8d5fb2c9d2cb2ff6ea71118584ab8a35af39ae43d5d90f`  
		Last Modified: Wed, 26 Jan 2022 22:17:51 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7858b7298d1ed34eff1ac6724d4bce1c8fc696786a68d28c115f2bc843aad9ab`  
		Last Modified: Wed, 26 Jan 2022 22:17:51 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; s390x

```console
$ docker pull spiped@sha256:dc9f30aec35bbc203643e902934a1b5e6140c26c166e0462f571d07f09e3fab5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.8 MB (34836084 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:40e931303d1bd986c9a5293d6f7f2f3dc4a9599d5af26cc8a933a43253c32f21`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 26 Jan 2022 01:41:13 GMT
ADD file:03b224b82f458b08d3b5071e42b67915a3db309332c0fc9229db7cf1148bc1b5 in / 
# Wed, 26 Jan 2022 01:41:15 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 11:27:45 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 26 Jan 2022 11:27:47 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 11:27:48 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 26 Jan 2022 11:28:01 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 26 Jan 2022 11:28:01 GMT
VOLUME [/spiped]
# Wed, 26 Jan 2022 11:28:02 GMT
WORKDIR /spiped
# Wed, 26 Jan 2022 11:28:02 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 26 Jan 2022 11:28:02 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 26 Jan 2022 11:28:02 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:70bed29526f8483937e4d2540d19256d30786007c7c321e717e00d2e74700380`  
		Last Modified: Wed, 26 Jan 2022 01:46:57 GMT  
		Size: 29.6 MB (29647071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87ff2a6a6375f95aac16175fe1a27e34e664c34d69d5ed1efa5d976ad0e7b947`  
		Last Modified: Wed, 26 Jan 2022 11:28:34 GMT  
		Size: 1.7 KB (1736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66b439c0f82c7b1a5745542aedc040eca1c81fae487012b1886220413a47d903`  
		Last Modified: Wed, 26 Jan 2022 11:28:34 GMT  
		Size: 1.1 KB (1052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93908f45004e2f2d6aee48dec977a4e4405bf91858cafb05024b750ca56aa9d7`  
		Last Modified: Wed, 26 Jan 2022 11:28:35 GMT  
		Size: 5.2 MB (5185752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9c094f1ad2a6f023f6f79a11bb9a375b3f52a100501b0d1191d839085802bba`  
		Last Modified: Wed, 26 Jan 2022 11:28:34 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83eccc997a02a9c670eaa7e3d2dfd923453818685f1b2c3ddfff0bf985a890d4`  
		Last Modified: Wed, 26 Jan 2022 11:28:34 GMT  
		Size: 344.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:1.6-alpine`

```console
$ docker pull spiped@sha256:b1089d3c383de79c5a463d8f6b45c46f804588a33a967ff66469a76a654169f0
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
$ docker pull spiped@sha256:f4aaae543ff5aba181d531aa5504251d883a40559812a85cff78c7526d3f713e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4523758 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d71e35e9a762b19f1a767061f3cf181454d7090d64dec7acef852f68d4c01262`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 24 Nov 2021 20:19:40 GMT
ADD file:9233f6f2237d79659a9521f7e390df217cec49f1a8aa3a12147bbca1956acdb9 in / 
# Wed, 24 Nov 2021 20:19:40 GMT
CMD ["/bin/sh"]
# Mon, 27 Dec 2021 19:10:10 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Mon, 27 Dec 2021 19:10:11 GMT
RUN apk add --no-cache libssl1.1
# Mon, 27 Dec 2021 19:10:11 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Mon, 27 Dec 2021 19:10:22 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Mon, 27 Dec 2021 19:10:22 GMT
VOLUME [/spiped]
# Mon, 27 Dec 2021 19:10:22 GMT
WORKDIR /spiped
# Mon, 27 Dec 2021 19:10:22 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 27 Dec 2021 19:10:23 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 27 Dec 2021 19:10:23 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:59bf1c3509f33515622619af21ed55bbe26d24913cedbca106468a5fb37a50c3`  
		Last Modified: Wed, 24 Nov 2021 20:20:05 GMT  
		Size: 2.8 MB (2818413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50c602680384586a0fe7febde9f529aea001928a6d26e84d9a3f7be94049ef27`  
		Last Modified: Mon, 27 Dec 2021 19:10:53 GMT  
		Size: 1.3 KB (1265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee913a58b01d029ed458f92226b5b52747e0877c39585d9f93ec5dd2ef0a8cf9`  
		Last Modified: Mon, 27 Dec 2021 19:10:53 GMT  
		Size: 7.7 KB (7749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd8bf950f1ef1b7c96ba1781b5a87d4044135ae197871b261e86d74bc35a8bf5`  
		Last Modified: Mon, 27 Dec 2021 19:10:54 GMT  
		Size: 1.7 MB (1695862 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56d41f282509324afd98cc83dab31aee8ba6459973698c8ccaf3978cddc4ede4`  
		Last Modified: Mon, 27 Dec 2021 19:10:53 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8ba766abbc809d26737c9cc94fbe15a6311c603bfd673bd6db553169dd0f141`  
		Last Modified: Mon, 27 Dec 2021 19:10:53 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; arm variant v6

```console
$ docker pull spiped@sha256:b6482b55d0b7700b0393783f0ea8e49e6a4329c07187fdf826b6902d0ccfa3e6
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.1 MB (4080480 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1df9593d1c7a93c5f606ef97c05cc8d86e1a5bce25cd9895c104e2e1a7edbe19`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 24 Nov 2021 21:08:16 GMT
ADD file:61137e0aa49ba06f57ac69466fe2fb116f580b5e6159d56f846b1d72c4a3c814 in / 
# Wed, 24 Nov 2021 21:08:16 GMT
CMD ["/bin/sh"]
# Mon, 27 Dec 2021 17:49:44 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Mon, 27 Dec 2021 17:49:46 GMT
RUN apk add --no-cache libssl1.1
# Mon, 27 Dec 2021 17:49:47 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Mon, 27 Dec 2021 17:50:06 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Mon, 27 Dec 2021 17:50:07 GMT
VOLUME [/spiped]
# Mon, 27 Dec 2021 17:50:07 GMT
WORKDIR /spiped
# Mon, 27 Dec 2021 17:50:08 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 27 Dec 2021 17:50:08 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 27 Dec 2021 17:50:09 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:e4a43de54da9e309482f6762f0c11f5f547cd8fd61a49c5f158453066162023e`  
		Last Modified: Wed, 24 Nov 2021 21:09:46 GMT  
		Size: 2.6 MB (2631421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c04f27a458746dfc1d07b0b03b9b8f205b08ebef9d6060ef92027b709fee313e`  
		Last Modified: Mon, 27 Dec 2021 17:50:41 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fffa3b0ec9bb32d2efab9fa903af078baf37201f4ec2026c0afce9c14156229`  
		Last Modified: Mon, 27 Dec 2021 17:50:41 GMT  
		Size: 7.7 KB (7743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e2344d51f830abe738f710343c04e056b2ec80e33a48522878caa568c9f553c`  
		Last Modified: Mon, 27 Dec 2021 17:50:42 GMT  
		Size: 1.4 MB (1439576 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd3eeeb2545dce6884a99d866ca20bd742d7e133aacf869b4cddbe974bfde627`  
		Last Modified: Mon, 27 Dec 2021 17:50:41 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2681e39729f29c202bc97138be5a28bb84d92220ffe45df47fb643301eef46aa`  
		Last Modified: Mon, 27 Dec 2021 17:50:41 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; arm variant v7

```console
$ docker pull spiped@sha256:277d22d33ab8cd23ff5bf04d4e60841c8a335de8fdb772173601e9a4d4cb00bf
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.8 MB (3802328 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2f94c64b2c706a58b82aa60bafca69c1fd15fb76714e5ca4aae0f1e4a47e3f1d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 24 Nov 2021 21:42:11 GMT
ADD file:ca436da5b0bfc9c0e2fc685533c6628918000c8fff109fe9a8da625b9a798002 in / 
# Wed, 24 Nov 2021 21:42:11 GMT
CMD ["/bin/sh"]
# Mon, 27 Dec 2021 18:00:04 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Mon, 27 Dec 2021 18:00:06 GMT
RUN apk add --no-cache libssl1.1
# Mon, 27 Dec 2021 18:00:06 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Mon, 27 Dec 2021 18:00:25 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Mon, 27 Dec 2021 18:00:26 GMT
VOLUME [/spiped]
# Mon, 27 Dec 2021 18:00:26 GMT
WORKDIR /spiped
# Mon, 27 Dec 2021 18:00:27 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 27 Dec 2021 18:00:27 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 27 Dec 2021 18:00:28 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:5480d2ca1740c20ce17652e01ed2265cdc914458acd41256a2b1ccff28f2762c`  
		Last Modified: Wed, 24 Nov 2021 21:43:40 GMT  
		Size: 2.4 MB (2434764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fca194041621ab40d8e7f24b7f7e82aa07760b2dafcd26472bd7fae96171989a`  
		Last Modified: Mon, 27 Dec 2021 18:01:41 GMT  
		Size: 1.3 KB (1267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7e934f04cb0ca6a107389bcb614eb02143fb079eef09a47a9248e3c4ff07864`  
		Last Modified: Mon, 27 Dec 2021 18:01:41 GMT  
		Size: 7.7 KB (7749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4111e5d44f2316d799c8b9144d8f35765b0bf330b8d596d99e504969cd48e07a`  
		Last Modified: Mon, 27 Dec 2021 18:01:42 GMT  
		Size: 1.4 MB (1358077 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f46d751b026ad913b2a48630c96460959a733e75728d55aafbd389197bf81857`  
		Last Modified: Mon, 27 Dec 2021 18:01:41 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5140561b01c4c6ae8b47c729fd289d7eef4a2b0e9c427a6bd35a86747e966206`  
		Last Modified: Mon, 27 Dec 2021 18:01:41 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:f2401c455a0fde4f25cae4b46bad0721c19ac135bc6efa4e5b3c46c5b04aa1cd
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.3 MB (4289462 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:017a5c1ca8bdf46589e6ab7b72a939d86283ebdb51f63d37bc1c41f07a36600f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 24 Nov 2021 20:39:20 GMT
ADD file:df53811312284306901fdaaff0a357a4bf40d631e662fe9ce6d342442e494b6c in / 
# Wed, 24 Nov 2021 20:39:20 GMT
CMD ["/bin/sh"]
# Mon, 27 Dec 2021 19:39:28 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Mon, 27 Dec 2021 19:39:29 GMT
RUN apk add --no-cache libssl1.1
# Mon, 27 Dec 2021 19:39:30 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Mon, 27 Dec 2021 19:39:41 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Mon, 27 Dec 2021 19:39:42 GMT
VOLUME [/spiped]
# Mon, 27 Dec 2021 19:39:43 GMT
WORKDIR /spiped
# Mon, 27 Dec 2021 19:39:45 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 27 Dec 2021 19:39:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 27 Dec 2021 19:39:46 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:9b3977197b4f2147bdd31e1271f811319dcd5c2fc595f14e81f5351ab6275b99`  
		Last Modified: Wed, 24 Nov 2021 20:39:59 GMT  
		Size: 2.7 MB (2715434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4642588fd355ccb1af1d6dc41cc14b5117bbd4f30adb691aade26686c4d5c116`  
		Last Modified: Mon, 27 Dec 2021 19:40:28 GMT  
		Size: 1.2 KB (1240 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd8e58927c1555e9461b11588b3accaf4b9d1018264a3d1ac75dbd1d03c2212e`  
		Last Modified: Mon, 27 Dec 2021 19:40:28 GMT  
		Size: 7.7 KB (7712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd181fff8bea1f7e317b2af57ee7244e2a0b5226b26df42dc9a9d836cf504dec`  
		Last Modified: Mon, 27 Dec 2021 19:40:28 GMT  
		Size: 1.6 MB (1564638 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f65407c84c38d42d7b099c55334ee34fc2e9f581954ed4e92bab1773599189df`  
		Last Modified: Mon, 27 Dec 2021 19:40:28 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97f56c7d1e54220168de3e0523afd6a69f29f86199d05ee4681c356afaa2e36a`  
		Last Modified: Mon, 27 Dec 2021 19:40:28 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; 386

```console
$ docker pull spiped@sha256:fc962e82018b393667a7d2b43c9bee0b19c4650fadcc16335cf984b44d859d65
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4539662 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:64dc6529164f107ee83f0edafa6bcf506960ffc646e0e9e161cb2640feb90f96`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 24 Nov 2021 20:53:48 GMT
ADD file:b9a17131c440053f2f67e127b447645f25fd7de2d6caca42f569cafab6291855 in / 
# Wed, 24 Nov 2021 20:53:48 GMT
CMD ["/bin/sh"]
# Mon, 27 Dec 2021 18:39:31 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Mon, 27 Dec 2021 18:39:32 GMT
RUN apk add --no-cache libssl1.1
# Mon, 27 Dec 2021 18:39:33 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Mon, 27 Dec 2021 18:39:45 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Mon, 27 Dec 2021 18:39:45 GMT
VOLUME [/spiped]
# Mon, 27 Dec 2021 18:39:45 GMT
WORKDIR /spiped
# Mon, 27 Dec 2021 18:39:46 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 27 Dec 2021 18:39:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 27 Dec 2021 18:39:46 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:e6889e0d66307a4b916fc844f2dcbc03245c63bc4189dd3e88126d9dcf2f9231`  
		Last Modified: Wed, 24 Nov 2021 20:54:48 GMT  
		Size: 2.8 MB (2827117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc39bdf14cf5dcbf704b50f736d82a339b1879574765ef87fbbf5ecb8d7d574e`  
		Last Modified: Mon, 27 Dec 2021 18:40:32 GMT  
		Size: 1.3 KB (1266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7128f9e1b03ce01ba1b51bce7aa1bc585b6c3e6ce1650259721463f363e9aaab`  
		Last Modified: Mon, 27 Dec 2021 18:40:32 GMT  
		Size: 7.8 KB (7750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb2ebf4c9a2525659cebde6ee501a457c4a31d364f3f568be0f076191d96855d`  
		Last Modified: Mon, 27 Dec 2021 18:40:33 GMT  
		Size: 1.7 MB (1703060 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75adf8fe66ad441b9c8e209efcc7d5b68b61c6a33e05b3aed401756e55493d07`  
		Last Modified: Mon, 27 Dec 2021 18:40:32 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99b656b54398310f3a0f295c7737034732b9ee5c7e294ad5df27230309fff8ae`  
		Last Modified: Mon, 27 Dec 2021 18:40:32 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; ppc64le

```console
$ docker pull spiped@sha256:bdb5c0f748fb29dd4c96f71d1eec1c471f348b68e39063a5674e88c6655400ac
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.4 MB (4447359 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c2ab0ba82f0f9badd5246249195a67d4e12bc4f6cfb1822b3454aca1c3dae586`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 24 Nov 2021 20:20:16 GMT
ADD file:57115dca2eb707f46b6301e75174e6aa316fb02ac28643b91429b75be51bd8c8 in / 
# Wed, 24 Nov 2021 20:20:20 GMT
CMD ["/bin/sh"]
# Mon, 27 Dec 2021 18:18:59 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Mon, 27 Dec 2021 18:19:06 GMT
RUN apk add --no-cache libssl1.1
# Mon, 27 Dec 2021 18:19:08 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Mon, 27 Dec 2021 18:19:22 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Mon, 27 Dec 2021 18:19:25 GMT
VOLUME [/spiped]
# Mon, 27 Dec 2021 18:19:28 GMT
WORKDIR /spiped
# Mon, 27 Dec 2021 18:19:28 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 27 Dec 2021 18:19:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 27 Dec 2021 18:19:33 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:159b5dcb1717c815c76ff5ea1db730e18e8609c9090238e43282856db9e71f47`  
		Last Modified: Wed, 24 Nov 2021 20:21:14 GMT  
		Size: 2.8 MB (2814780 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5ef2b17ec4445a63d712289fc62b0e3e30ab15992e0a0d38ab25e290abcb38e`  
		Last Modified: Mon, 27 Dec 2021 18:20:21 GMT  
		Size: 1.3 KB (1274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:210460e69fcfc508eae94f5666c4fc57c0cdf6163c3a6e39710f5da7a2e5ceb6`  
		Last Modified: Mon, 27 Dec 2021 18:20:21 GMT  
		Size: 7.7 KB (7737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0860c3c69dcd2673558f15fc9c46c8447274ce23c207e936804fe5a268e5e7f`  
		Last Modified: Mon, 27 Dec 2021 18:20:22 GMT  
		Size: 1.6 MB (1623097 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13cd96844150db5d01e32349b5f650aafd01dd1789c2a11fee82b6f55bd43560`  
		Last Modified: Mon, 27 Dec 2021 18:20:21 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a52b1de785dfc0bc3d07ee3d3f619d0681bc34b7eeee205db16da01946663a91`  
		Last Modified: Mon, 27 Dec 2021 18:20:21 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; s390x

```console
$ docker pull spiped@sha256:e5972c57d035e42883aca7354deb92cd65a9bbbc8d5d6aaa8b364891cbdba20d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.0 MB (4034365 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6b297cc2c896c2d11d20abe50ce763f606504b9aad55d18a6c8bcf3407db63c8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 24 Nov 2021 20:41:23 GMT
ADD file:cd24c711a2ef431b3ff94f9a02bfc42f159bc60de1d0eceecafea4e8af02441d in / 
# Wed, 24 Nov 2021 20:41:23 GMT
CMD ["/bin/sh"]
# Mon, 27 Dec 2021 18:42:02 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Mon, 27 Dec 2021 18:42:04 GMT
RUN apk add --no-cache libssl1.1
# Mon, 27 Dec 2021 18:42:04 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Mon, 27 Dec 2021 18:42:09 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Mon, 27 Dec 2021 18:42:09 GMT
VOLUME [/spiped]
# Mon, 27 Dec 2021 18:42:09 GMT
WORKDIR /spiped
# Mon, 27 Dec 2021 18:42:10 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 27 Dec 2021 18:42:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 27 Dec 2021 18:42:10 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:d6baca485f3d0f7c77221be60fbef5db014a5ef9d8f53db4a310c947c690d189`  
		Last Modified: Wed, 24 Nov 2021 20:42:15 GMT  
		Size: 2.6 MB (2605944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:631b52683dec736314bc4a995e6d4aa8fe70ccec0ccb0b4f0349543c0b9d315d`  
		Last Modified: Mon, 27 Dec 2021 18:42:54 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8a99397842c922d6589a78e8df8f8b4feac626485047c36e902a2966e19dfe2`  
		Last Modified: Mon, 27 Dec 2021 18:42:54 GMT  
		Size: 7.7 KB (7743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:556dc6882e78ba3518dbab7eaae8412b06f9ad7e09122f6478d9d1cc80b978e4`  
		Last Modified: Mon, 27 Dec 2021 18:42:55 GMT  
		Size: 1.4 MB (1418939 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9680c33180071ffeb1ac5cfe629daff266a5cf86a4072e251e4b0bef70d20b3`  
		Last Modified: Mon, 27 Dec 2021 18:42:54 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2742416115dba0ead2f2dc1f9aa438a1ef9179b4e11cfd9d665c918f92b53c55`  
		Last Modified: Mon, 27 Dec 2021 18:42:54 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:1.6.2`

```console
$ docker pull spiped@sha256:d9abc65404acc410b3f94bd812f875d66ad7304604f00ee6464be3ab291d57b3
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
$ docker pull spiped@sha256:dc2c3a3712eacb11a556c86bc2a6b606ba5a0edff87bf3638c159b85a1135448
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.3 MB (37335950 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1d472f594ea8090d6f3cbeb573986f7840e512b983c9def18699f62efe8bcc04`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 26 Jan 2022 01:40:35 GMT
ADD file:90495c24c897ec47982e200f732f8be3109fcd791691ddffae0756898f91024f in / 
# Wed, 26 Jan 2022 01:40:36 GMT
CMD ["bash"]
# Thu, 27 Jan 2022 02:32:24 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Thu, 27 Jan 2022 02:32:27 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Thu, 27 Jan 2022 02:32:28 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 27 Jan 2022 02:32:58 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 27 Jan 2022 02:32:58 GMT
VOLUME [/spiped]
# Thu, 27 Jan 2022 02:32:59 GMT
WORKDIR /spiped
# Thu, 27 Jan 2022 02:33:00 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 27 Jan 2022 02:33:00 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 27 Jan 2022 02:33:01 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:5eb5b503b37671af16371272f9c5313a3e82f1d0756e14506704489ad9900803`  
		Last Modified: Wed, 26 Jan 2022 01:46:39 GMT  
		Size: 31.4 MB (31366257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6a2517caec378bb5ccef0a0d6e52b5e25a629d59a240188bd605cf9f98bc57d`  
		Last Modified: Thu, 27 Jan 2022 02:33:32 GMT  
		Size: 1.7 KB (1734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9824d58dd5193ef98f897a6ac1feb9749d5f2371324023d2ca61dae51fb70e6`  
		Last Modified: Thu, 27 Jan 2022 02:33:32 GMT  
		Size: 1.1 KB (1051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d878a5544ecf1374c1348226765bcdd58a98e4e3d4c98f89ccf5fa10a7ca8ff`  
		Last Modified: Thu, 27 Jan 2022 02:33:34 GMT  
		Size: 6.0 MB (5966436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:754c3acbb4e4a2d6ba3fb19ebf6f464a6af124ca39e832916a9e20959ba6cb46`  
		Last Modified: Thu, 27 Jan 2022 02:33:32 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ddcc8c75157adfeb6f31357486186ad845c90e035dbcc13ad22c90c787c7769`  
		Last Modified: Thu, 27 Jan 2022 02:33:32 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.2` - linux; arm variant v5

```console
$ docker pull spiped@sha256:d35164b325c8b4cebf396e69ccd1cb2f1c7c2c813f1645f3a9d7fa533a214761
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.9 MB (33940215 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7d587f5e0871df03606d30179c325953573c55459a421e180a9ef24904dddb49`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 26 Jan 2022 01:41:57 GMT
ADD file:4ccea3cb033595f7bd9896126e94a8a19199b987bedd87b3c0700d8b29baa1fb in / 
# Wed, 26 Jan 2022 01:41:58 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 13:48:20 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 26 Jan 2022 13:48:29 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 13:48:30 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 26 Jan 2022 13:49:20 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 26 Jan 2022 13:49:21 GMT
VOLUME [/spiped]
# Wed, 26 Jan 2022 13:49:21 GMT
WORKDIR /spiped
# Wed, 26 Jan 2022 13:49:22 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 26 Jan 2022 13:49:23 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 26 Jan 2022 13:49:23 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:247ff78919074ec9db7cccd537dd6eb4d7e2788013b7ef07443e345d91c8a588`  
		Last Modified: Wed, 26 Jan 2022 01:57:36 GMT  
		Size: 28.9 MB (28909638 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cf343e822da1ce4be935758169ff31bce470bf1fe1276540174154bb3f2668d`  
		Last Modified: Wed, 26 Jan 2022 13:49:57 GMT  
		Size: 1.7 KB (1727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c398ac3bf4e12d1412bc45d6f9286f5c1700b12eaa24f0978ff6ab2197fe87d`  
		Last Modified: Wed, 26 Jan 2022 13:49:57 GMT  
		Size: 1.1 KB (1051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:797b9d89af1464c4395401f548e40c856ec3fb4894d839f6f9f420a1e2028f16`  
		Last Modified: Wed, 26 Jan 2022 13:50:02 GMT  
		Size: 5.0 MB (5027326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81ef5c7608dbb1e039ea48a4ffc9bac9710189cf564f106cb68cead03b7e4253`  
		Last Modified: Wed, 26 Jan 2022 13:49:57 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb5277a969518e6a9f8d7485c29504d113db9236a9d49b296bd38c4d422c67ea`  
		Last Modified: Wed, 26 Jan 2022 13:49:57 GMT  
		Size: 344.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.2` - linux; arm variant v7

```console
$ docker pull spiped@sha256:3d916238fd77df17911ab19dc7587e33dd0cada5997bb822a6341b6bc4d22d8e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.3 MB (31315488 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c1f89cc56381f998f2473d68073ecab8c87f42eaa6bc2bfeef9e59d7cffaef6f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 26 Jan 2022 01:42:08 GMT
ADD file:7f27f5b43b7cb04e509fe145266d9bdeacfcacb024cafac32e57ef1c831d5ea7 in / 
# Wed, 26 Jan 2022 01:42:09 GMT
CMD ["bash"]
# Thu, 27 Jan 2022 02:05:29 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Thu, 27 Jan 2022 02:05:36 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Thu, 27 Jan 2022 02:05:37 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 27 Jan 2022 02:06:23 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 27 Jan 2022 02:06:24 GMT
VOLUME [/spiped]
# Thu, 27 Jan 2022 02:06:24 GMT
WORKDIR /spiped
# Thu, 27 Jan 2022 02:06:25 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 27 Jan 2022 02:06:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 27 Jan 2022 02:06:26 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:aaef1f1162ec03e01b5b955d41da400544ec2374093ae3dbc330ab2bb36df3e1`  
		Last Modified: Wed, 26 Jan 2022 01:57:59 GMT  
		Size: 26.6 MB (26564933 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b839df330fe51f570a9646e1b8027ad2653336fbd121c12312e0baddcad0d5cd`  
		Last Modified: Thu, 27 Jan 2022 02:07:27 GMT  
		Size: 1.7 KB (1727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b58b2cda412f0922939bcdd348b6d2e3cd4dccd6036926ca90ec596a1b13fbf2`  
		Last Modified: Thu, 27 Jan 2022 02:07:27 GMT  
		Size: 1.1 KB (1051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3936070b02fda979073a59e440e1fb34695f2a5ab92ee369696afed5e3937b5`  
		Last Modified: Thu, 27 Jan 2022 02:07:32 GMT  
		Size: 4.7 MB (4747305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4dd327a7a9576943baaf60df0bdb6ff237147bcfd0f8ee37cf0a591a60131946`  
		Last Modified: Thu, 27 Jan 2022 02:07:27 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60e3ddb56b8bd24d775b3c0d169d4a1a1e03f18562970b41a9d187bc0b0161d8`  
		Last Modified: Thu, 27 Jan 2022 02:07:27 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.2` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:ec801aacab912356ed8782ef99c1d53dea85c30a74b6c982e1c33ab60cf936f5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.3 MB (35329660 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5ec3eef7cdb77d28d34401d13e367b0a1ae12678889d9b3df643c3baf3b58b27`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 26 Jan 2022 01:42:31 GMT
ADD file:0ec6f47a8857bf8e6cef71ed8f864be7ce1790ff6ed04fd4201e7dbde4728d3a in / 
# Wed, 26 Jan 2022 01:42:31 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 09:19:54 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 26 Jan 2022 09:19:57 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 09:19:57 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 26 Jan 2022 09:20:14 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 26 Jan 2022 09:20:15 GMT
VOLUME [/spiped]
# Wed, 26 Jan 2022 09:20:16 GMT
WORKDIR /spiped
# Wed, 26 Jan 2022 09:20:18 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 26 Jan 2022 09:20:18 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 26 Jan 2022 09:20:19 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:8998bd30e6a1204d13403045766edbe14f941b52087465f5d140ab63c8b113bf`  
		Last Modified: Wed, 26 Jan 2022 01:49:04 GMT  
		Size: 30.1 MB (30056774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5c0deb70595215cef3194a8d1bea35a623260a4a537174ac0174e9388d20b66`  
		Last Modified: Wed, 26 Jan 2022 09:20:48 GMT  
		Size: 1.6 KB (1618 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:034b8f66f1f2f1b93a71339b2b1c5e595c4574868f5e7d0f06f2c0bf51174940`  
		Last Modified: Wed, 26 Jan 2022 09:20:48 GMT  
		Size: 923.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b14f060bef623dc32f29a79d5b26a6879c4aa9267e5b87ecf4ce0e10f5dfb170`  
		Last Modified: Wed, 26 Jan 2022 09:20:49 GMT  
		Size: 5.3 MB (5269907 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99a6c1e6b86dbfff40179fb98822e12212a0b2867e6d5240159c942eb3854996`  
		Last Modified: Wed, 26 Jan 2022 09:20:47 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce3566ea2e7139f3188bf62015b6b85e2bb8e4c6c1ad89ef5c389ef067c3c0c2`  
		Last Modified: Wed, 26 Jan 2022 09:20:48 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.2` - linux; 386

```console
$ docker pull spiped@sha256:d62c6f333ea8dc55c74566a02c6966fdb05a5373f946c62e78dc4535e7c6439b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.3 MB (40272052 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:240f8e63cba198164b163f99564af3065d0d08a532f87c59c4fafe8bc87fee95`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 26 Jan 2022 01:39:55 GMT
ADD file:876ebf07c65841f4840842086c883af48e07386964fe6d643ba193895ec2a582 in / 
# Wed, 26 Jan 2022 01:39:56 GMT
CMD ["bash"]
# Thu, 27 Jan 2022 04:50:43 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Thu, 27 Jan 2022 04:50:51 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Thu, 27 Jan 2022 04:50:52 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 27 Jan 2022 04:51:42 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 27 Jan 2022 04:51:43 GMT
VOLUME [/spiped]
# Thu, 27 Jan 2022 04:51:43 GMT
WORKDIR /spiped
# Thu, 27 Jan 2022 04:51:44 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 27 Jan 2022 04:51:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 27 Jan 2022 04:51:45 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:86933886b1754aba091548cf031a9bca88cdce9bb4fc1f28bb38b61594c2c2c7`  
		Last Modified: Wed, 26 Jan 2022 01:48:57 GMT  
		Size: 32.4 MB (32377406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:007b643ac135004248e51a7df9b02d61247a5ace740507e11d1238f5c6559f0a`  
		Last Modified: Thu, 27 Jan 2022 04:52:38 GMT  
		Size: 1.7 KB (1729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe9889a275b3dcd9c9d9380a6b23eff3430e0928931f872c594a56aca75b74a0`  
		Last Modified: Thu, 27 Jan 2022 04:52:37 GMT  
		Size: 1.1 KB (1052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a8f1418eeaf635a0d7c0ff4a2a9200da488617f0d749336ec280dc483d43299`  
		Last Modified: Thu, 27 Jan 2022 04:52:41 GMT  
		Size: 7.9 MB (7891393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edd6784674f4cacc537045d525761932e2f277aa61bb5029896a120518807d30`  
		Last Modified: Thu, 27 Jan 2022 04:52:38 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4489e826d0a9aaec6002d3f886c71d2e729d1a47b745a9a82bbdae810d0345f2`  
		Last Modified: Thu, 27 Jan 2022 04:52:37 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.2` - linux; mips64le

```console
$ docker pull spiped@sha256:5ff06e4c09b7b50640a863ff273ef3b49b36efa00ee15a15bc68e0d0c9c31d4c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.3 MB (35341414 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:13ee9a2841cd7deb5c6e19a80d798eaf34ac36066234c76dd87975bb8adbaa97`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 26 Jan 2022 01:42:45 GMT
ADD file:61767027a5ab46afbcd4079d200abe8d663326adc96fa28ca8c8955a06d9322e in / 
# Wed, 26 Jan 2022 01:42:46 GMT
CMD ["bash"]
# Thu, 27 Jan 2022 14:17:20 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Thu, 27 Jan 2022 14:17:32 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Thu, 27 Jan 2022 14:17:32 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 27 Jan 2022 14:18:22 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 27 Jan 2022 14:18:22 GMT
VOLUME [/spiped]
# Thu, 27 Jan 2022 14:18:23 GMT
WORKDIR /spiped
# Thu, 27 Jan 2022 14:18:23 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 27 Jan 2022 14:18:23 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 27 Jan 2022 14:18:24 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:266e7d2b59483859eaa1711d2afeb25ea4458eeb36b3e909372930db1f834d7f`  
		Last Modified: Wed, 26 Jan 2022 01:51:23 GMT  
		Size: 29.6 MB (29632834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bed329584043834b57b17c1f7fb178849a18c1e185f6a1c3790d7e4f3aabdad`  
		Last Modified: Thu, 27 Jan 2022 14:18:40 GMT  
		Size: 1.7 KB (1732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1221de7514f3a6d44d793ddbb512b55c28feed96691f900bce757c1ad89f2db`  
		Last Modified: Thu, 27 Jan 2022 14:18:41 GMT  
		Size: 1.0 KB (1026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b78ea45f3c4a37e62bd246764fe6840be44718f3a906daf70e4d583cf4aaa6af`  
		Last Modified: Thu, 27 Jan 2022 14:18:46 GMT  
		Size: 5.7 MB (5705384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53d16d14491067074a517e226e1dced4190135104702609415f883fa63d46ee3`  
		Last Modified: Thu, 27 Jan 2022 14:18:41 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2dba9fb9a37e3aafad3abba08e85db2fd96587c52de4e6a2df6ef442c2538a96`  
		Last Modified: Thu, 27 Jan 2022 14:18:40 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.2` - linux; ppc64le

```console
$ docker pull spiped@sha256:f9a8ff652bffe474afdf6cf3da90bcb5fabc4674ad021bc3ddf11100309fcbe7
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.3 MB (41274405 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b89132621e69403b6931ac29ab0fdf93d27e91888256b85a1de6d142d4046a56`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 26 Jan 2022 01:46:51 GMT
ADD file:c03f34c221e57fa5cb625c166d1db9f72d6ba2fa17a3c41a5d04d6875d098949 in / 
# Wed, 26 Jan 2022 01:46:57 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 22:15:10 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 26 Jan 2022 22:15:19 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 22:15:21 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 26 Jan 2022 22:17:04 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 26 Jan 2022 22:17:09 GMT
VOLUME [/spiped]
# Wed, 26 Jan 2022 22:17:12 GMT
WORKDIR /spiped
# Wed, 26 Jan 2022 22:17:14 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 26 Jan 2022 22:17:16 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 26 Jan 2022 22:17:20 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:3149ee4a73508a4c39107d64a3fdc1b021626a22a0ac95e62fa0cea49ab77fba`  
		Last Modified: Wed, 26 Jan 2022 01:57:01 GMT  
		Size: 35.3 MB (35273030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43b54b67a6f99dac2db476b7702d015eb56f81c2d623bc96fd32aae703f0b732`  
		Last Modified: Wed, 26 Jan 2022 22:17:51 GMT  
		Size: 1.7 KB (1739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f1241c00e00d3316ad39effb0518ce815abfcf876ea4efac9de53b2fdc560da`  
		Last Modified: Wed, 26 Jan 2022 22:17:51 GMT  
		Size: 1.1 KB (1054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86ddc628c1bd5eff84e7cb044e5c93444f7e53a189710ec4b2f0213ffc82cb0f`  
		Last Modified: Wed, 26 Jan 2022 22:17:53 GMT  
		Size: 6.0 MB (5998110 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:706174d608bd436d8e8d5fb2c9d2cb2ff6ea71118584ab8a35af39ae43d5d90f`  
		Last Modified: Wed, 26 Jan 2022 22:17:51 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7858b7298d1ed34eff1ac6724d4bce1c8fc696786a68d28c115f2bc843aad9ab`  
		Last Modified: Wed, 26 Jan 2022 22:17:51 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.2` - linux; s390x

```console
$ docker pull spiped@sha256:dc9f30aec35bbc203643e902934a1b5e6140c26c166e0462f571d07f09e3fab5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.8 MB (34836084 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:40e931303d1bd986c9a5293d6f7f2f3dc4a9599d5af26cc8a933a43253c32f21`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 26 Jan 2022 01:41:13 GMT
ADD file:03b224b82f458b08d3b5071e42b67915a3db309332c0fc9229db7cf1148bc1b5 in / 
# Wed, 26 Jan 2022 01:41:15 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 11:27:45 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 26 Jan 2022 11:27:47 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 11:27:48 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 26 Jan 2022 11:28:01 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 26 Jan 2022 11:28:01 GMT
VOLUME [/spiped]
# Wed, 26 Jan 2022 11:28:02 GMT
WORKDIR /spiped
# Wed, 26 Jan 2022 11:28:02 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 26 Jan 2022 11:28:02 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 26 Jan 2022 11:28:02 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:70bed29526f8483937e4d2540d19256d30786007c7c321e717e00d2e74700380`  
		Last Modified: Wed, 26 Jan 2022 01:46:57 GMT  
		Size: 29.6 MB (29647071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87ff2a6a6375f95aac16175fe1a27e34e664c34d69d5ed1efa5d976ad0e7b947`  
		Last Modified: Wed, 26 Jan 2022 11:28:34 GMT  
		Size: 1.7 KB (1736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66b439c0f82c7b1a5745542aedc040eca1c81fae487012b1886220413a47d903`  
		Last Modified: Wed, 26 Jan 2022 11:28:34 GMT  
		Size: 1.1 KB (1052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93908f45004e2f2d6aee48dec977a4e4405bf91858cafb05024b750ca56aa9d7`  
		Last Modified: Wed, 26 Jan 2022 11:28:35 GMT  
		Size: 5.2 MB (5185752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9c094f1ad2a6f023f6f79a11bb9a375b3f52a100501b0d1191d839085802bba`  
		Last Modified: Wed, 26 Jan 2022 11:28:34 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83eccc997a02a9c670eaa7e3d2dfd923453818685f1b2c3ddfff0bf985a890d4`  
		Last Modified: Wed, 26 Jan 2022 11:28:34 GMT  
		Size: 344.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:1.6.2-alpine`

```console
$ docker pull spiped@sha256:b1089d3c383de79c5a463d8f6b45c46f804588a33a967ff66469a76a654169f0
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
$ docker pull spiped@sha256:f4aaae543ff5aba181d531aa5504251d883a40559812a85cff78c7526d3f713e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4523758 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d71e35e9a762b19f1a767061f3cf181454d7090d64dec7acef852f68d4c01262`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 24 Nov 2021 20:19:40 GMT
ADD file:9233f6f2237d79659a9521f7e390df217cec49f1a8aa3a12147bbca1956acdb9 in / 
# Wed, 24 Nov 2021 20:19:40 GMT
CMD ["/bin/sh"]
# Mon, 27 Dec 2021 19:10:10 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Mon, 27 Dec 2021 19:10:11 GMT
RUN apk add --no-cache libssl1.1
# Mon, 27 Dec 2021 19:10:11 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Mon, 27 Dec 2021 19:10:22 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Mon, 27 Dec 2021 19:10:22 GMT
VOLUME [/spiped]
# Mon, 27 Dec 2021 19:10:22 GMT
WORKDIR /spiped
# Mon, 27 Dec 2021 19:10:22 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 27 Dec 2021 19:10:23 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 27 Dec 2021 19:10:23 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:59bf1c3509f33515622619af21ed55bbe26d24913cedbca106468a5fb37a50c3`  
		Last Modified: Wed, 24 Nov 2021 20:20:05 GMT  
		Size: 2.8 MB (2818413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50c602680384586a0fe7febde9f529aea001928a6d26e84d9a3f7be94049ef27`  
		Last Modified: Mon, 27 Dec 2021 19:10:53 GMT  
		Size: 1.3 KB (1265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee913a58b01d029ed458f92226b5b52747e0877c39585d9f93ec5dd2ef0a8cf9`  
		Last Modified: Mon, 27 Dec 2021 19:10:53 GMT  
		Size: 7.7 KB (7749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd8bf950f1ef1b7c96ba1781b5a87d4044135ae197871b261e86d74bc35a8bf5`  
		Last Modified: Mon, 27 Dec 2021 19:10:54 GMT  
		Size: 1.7 MB (1695862 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56d41f282509324afd98cc83dab31aee8ba6459973698c8ccaf3978cddc4ede4`  
		Last Modified: Mon, 27 Dec 2021 19:10:53 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8ba766abbc809d26737c9cc94fbe15a6311c603bfd673bd6db553169dd0f141`  
		Last Modified: Mon, 27 Dec 2021 19:10:53 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.2-alpine` - linux; arm variant v6

```console
$ docker pull spiped@sha256:b6482b55d0b7700b0393783f0ea8e49e6a4329c07187fdf826b6902d0ccfa3e6
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.1 MB (4080480 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1df9593d1c7a93c5f606ef97c05cc8d86e1a5bce25cd9895c104e2e1a7edbe19`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 24 Nov 2021 21:08:16 GMT
ADD file:61137e0aa49ba06f57ac69466fe2fb116f580b5e6159d56f846b1d72c4a3c814 in / 
# Wed, 24 Nov 2021 21:08:16 GMT
CMD ["/bin/sh"]
# Mon, 27 Dec 2021 17:49:44 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Mon, 27 Dec 2021 17:49:46 GMT
RUN apk add --no-cache libssl1.1
# Mon, 27 Dec 2021 17:49:47 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Mon, 27 Dec 2021 17:50:06 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Mon, 27 Dec 2021 17:50:07 GMT
VOLUME [/spiped]
# Mon, 27 Dec 2021 17:50:07 GMT
WORKDIR /spiped
# Mon, 27 Dec 2021 17:50:08 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 27 Dec 2021 17:50:08 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 27 Dec 2021 17:50:09 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:e4a43de54da9e309482f6762f0c11f5f547cd8fd61a49c5f158453066162023e`  
		Last Modified: Wed, 24 Nov 2021 21:09:46 GMT  
		Size: 2.6 MB (2631421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c04f27a458746dfc1d07b0b03b9b8f205b08ebef9d6060ef92027b709fee313e`  
		Last Modified: Mon, 27 Dec 2021 17:50:41 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fffa3b0ec9bb32d2efab9fa903af078baf37201f4ec2026c0afce9c14156229`  
		Last Modified: Mon, 27 Dec 2021 17:50:41 GMT  
		Size: 7.7 KB (7743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e2344d51f830abe738f710343c04e056b2ec80e33a48522878caa568c9f553c`  
		Last Modified: Mon, 27 Dec 2021 17:50:42 GMT  
		Size: 1.4 MB (1439576 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd3eeeb2545dce6884a99d866ca20bd742d7e133aacf869b4cddbe974bfde627`  
		Last Modified: Mon, 27 Dec 2021 17:50:41 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2681e39729f29c202bc97138be5a28bb84d92220ffe45df47fb643301eef46aa`  
		Last Modified: Mon, 27 Dec 2021 17:50:41 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.2-alpine` - linux; arm variant v7

```console
$ docker pull spiped@sha256:277d22d33ab8cd23ff5bf04d4e60841c8a335de8fdb772173601e9a4d4cb00bf
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.8 MB (3802328 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2f94c64b2c706a58b82aa60bafca69c1fd15fb76714e5ca4aae0f1e4a47e3f1d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 24 Nov 2021 21:42:11 GMT
ADD file:ca436da5b0bfc9c0e2fc685533c6628918000c8fff109fe9a8da625b9a798002 in / 
# Wed, 24 Nov 2021 21:42:11 GMT
CMD ["/bin/sh"]
# Mon, 27 Dec 2021 18:00:04 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Mon, 27 Dec 2021 18:00:06 GMT
RUN apk add --no-cache libssl1.1
# Mon, 27 Dec 2021 18:00:06 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Mon, 27 Dec 2021 18:00:25 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Mon, 27 Dec 2021 18:00:26 GMT
VOLUME [/spiped]
# Mon, 27 Dec 2021 18:00:26 GMT
WORKDIR /spiped
# Mon, 27 Dec 2021 18:00:27 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 27 Dec 2021 18:00:27 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 27 Dec 2021 18:00:28 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:5480d2ca1740c20ce17652e01ed2265cdc914458acd41256a2b1ccff28f2762c`  
		Last Modified: Wed, 24 Nov 2021 21:43:40 GMT  
		Size: 2.4 MB (2434764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fca194041621ab40d8e7f24b7f7e82aa07760b2dafcd26472bd7fae96171989a`  
		Last Modified: Mon, 27 Dec 2021 18:01:41 GMT  
		Size: 1.3 KB (1267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7e934f04cb0ca6a107389bcb614eb02143fb079eef09a47a9248e3c4ff07864`  
		Last Modified: Mon, 27 Dec 2021 18:01:41 GMT  
		Size: 7.7 KB (7749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4111e5d44f2316d799c8b9144d8f35765b0bf330b8d596d99e504969cd48e07a`  
		Last Modified: Mon, 27 Dec 2021 18:01:42 GMT  
		Size: 1.4 MB (1358077 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f46d751b026ad913b2a48630c96460959a733e75728d55aafbd389197bf81857`  
		Last Modified: Mon, 27 Dec 2021 18:01:41 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5140561b01c4c6ae8b47c729fd289d7eef4a2b0e9c427a6bd35a86747e966206`  
		Last Modified: Mon, 27 Dec 2021 18:01:41 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.2-alpine` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:f2401c455a0fde4f25cae4b46bad0721c19ac135bc6efa4e5b3c46c5b04aa1cd
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.3 MB (4289462 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:017a5c1ca8bdf46589e6ab7b72a939d86283ebdb51f63d37bc1c41f07a36600f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 24 Nov 2021 20:39:20 GMT
ADD file:df53811312284306901fdaaff0a357a4bf40d631e662fe9ce6d342442e494b6c in / 
# Wed, 24 Nov 2021 20:39:20 GMT
CMD ["/bin/sh"]
# Mon, 27 Dec 2021 19:39:28 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Mon, 27 Dec 2021 19:39:29 GMT
RUN apk add --no-cache libssl1.1
# Mon, 27 Dec 2021 19:39:30 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Mon, 27 Dec 2021 19:39:41 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Mon, 27 Dec 2021 19:39:42 GMT
VOLUME [/spiped]
# Mon, 27 Dec 2021 19:39:43 GMT
WORKDIR /spiped
# Mon, 27 Dec 2021 19:39:45 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 27 Dec 2021 19:39:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 27 Dec 2021 19:39:46 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:9b3977197b4f2147bdd31e1271f811319dcd5c2fc595f14e81f5351ab6275b99`  
		Last Modified: Wed, 24 Nov 2021 20:39:59 GMT  
		Size: 2.7 MB (2715434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4642588fd355ccb1af1d6dc41cc14b5117bbd4f30adb691aade26686c4d5c116`  
		Last Modified: Mon, 27 Dec 2021 19:40:28 GMT  
		Size: 1.2 KB (1240 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd8e58927c1555e9461b11588b3accaf4b9d1018264a3d1ac75dbd1d03c2212e`  
		Last Modified: Mon, 27 Dec 2021 19:40:28 GMT  
		Size: 7.7 KB (7712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd181fff8bea1f7e317b2af57ee7244e2a0b5226b26df42dc9a9d836cf504dec`  
		Last Modified: Mon, 27 Dec 2021 19:40:28 GMT  
		Size: 1.6 MB (1564638 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f65407c84c38d42d7b099c55334ee34fc2e9f581954ed4e92bab1773599189df`  
		Last Modified: Mon, 27 Dec 2021 19:40:28 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97f56c7d1e54220168de3e0523afd6a69f29f86199d05ee4681c356afaa2e36a`  
		Last Modified: Mon, 27 Dec 2021 19:40:28 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.2-alpine` - linux; 386

```console
$ docker pull spiped@sha256:fc962e82018b393667a7d2b43c9bee0b19c4650fadcc16335cf984b44d859d65
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4539662 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:64dc6529164f107ee83f0edafa6bcf506960ffc646e0e9e161cb2640feb90f96`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 24 Nov 2021 20:53:48 GMT
ADD file:b9a17131c440053f2f67e127b447645f25fd7de2d6caca42f569cafab6291855 in / 
# Wed, 24 Nov 2021 20:53:48 GMT
CMD ["/bin/sh"]
# Mon, 27 Dec 2021 18:39:31 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Mon, 27 Dec 2021 18:39:32 GMT
RUN apk add --no-cache libssl1.1
# Mon, 27 Dec 2021 18:39:33 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Mon, 27 Dec 2021 18:39:45 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Mon, 27 Dec 2021 18:39:45 GMT
VOLUME [/spiped]
# Mon, 27 Dec 2021 18:39:45 GMT
WORKDIR /spiped
# Mon, 27 Dec 2021 18:39:46 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 27 Dec 2021 18:39:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 27 Dec 2021 18:39:46 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:e6889e0d66307a4b916fc844f2dcbc03245c63bc4189dd3e88126d9dcf2f9231`  
		Last Modified: Wed, 24 Nov 2021 20:54:48 GMT  
		Size: 2.8 MB (2827117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc39bdf14cf5dcbf704b50f736d82a339b1879574765ef87fbbf5ecb8d7d574e`  
		Last Modified: Mon, 27 Dec 2021 18:40:32 GMT  
		Size: 1.3 KB (1266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7128f9e1b03ce01ba1b51bce7aa1bc585b6c3e6ce1650259721463f363e9aaab`  
		Last Modified: Mon, 27 Dec 2021 18:40:32 GMT  
		Size: 7.8 KB (7750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb2ebf4c9a2525659cebde6ee501a457c4a31d364f3f568be0f076191d96855d`  
		Last Modified: Mon, 27 Dec 2021 18:40:33 GMT  
		Size: 1.7 MB (1703060 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75adf8fe66ad441b9c8e209efcc7d5b68b61c6a33e05b3aed401756e55493d07`  
		Last Modified: Mon, 27 Dec 2021 18:40:32 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99b656b54398310f3a0f295c7737034732b9ee5c7e294ad5df27230309fff8ae`  
		Last Modified: Mon, 27 Dec 2021 18:40:32 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.2-alpine` - linux; ppc64le

```console
$ docker pull spiped@sha256:bdb5c0f748fb29dd4c96f71d1eec1c471f348b68e39063a5674e88c6655400ac
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.4 MB (4447359 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c2ab0ba82f0f9badd5246249195a67d4e12bc4f6cfb1822b3454aca1c3dae586`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 24 Nov 2021 20:20:16 GMT
ADD file:57115dca2eb707f46b6301e75174e6aa316fb02ac28643b91429b75be51bd8c8 in / 
# Wed, 24 Nov 2021 20:20:20 GMT
CMD ["/bin/sh"]
# Mon, 27 Dec 2021 18:18:59 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Mon, 27 Dec 2021 18:19:06 GMT
RUN apk add --no-cache libssl1.1
# Mon, 27 Dec 2021 18:19:08 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Mon, 27 Dec 2021 18:19:22 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Mon, 27 Dec 2021 18:19:25 GMT
VOLUME [/spiped]
# Mon, 27 Dec 2021 18:19:28 GMT
WORKDIR /spiped
# Mon, 27 Dec 2021 18:19:28 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 27 Dec 2021 18:19:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 27 Dec 2021 18:19:33 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:159b5dcb1717c815c76ff5ea1db730e18e8609c9090238e43282856db9e71f47`  
		Last Modified: Wed, 24 Nov 2021 20:21:14 GMT  
		Size: 2.8 MB (2814780 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5ef2b17ec4445a63d712289fc62b0e3e30ab15992e0a0d38ab25e290abcb38e`  
		Last Modified: Mon, 27 Dec 2021 18:20:21 GMT  
		Size: 1.3 KB (1274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:210460e69fcfc508eae94f5666c4fc57c0cdf6163c3a6e39710f5da7a2e5ceb6`  
		Last Modified: Mon, 27 Dec 2021 18:20:21 GMT  
		Size: 7.7 KB (7737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0860c3c69dcd2673558f15fc9c46c8447274ce23c207e936804fe5a268e5e7f`  
		Last Modified: Mon, 27 Dec 2021 18:20:22 GMT  
		Size: 1.6 MB (1623097 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13cd96844150db5d01e32349b5f650aafd01dd1789c2a11fee82b6f55bd43560`  
		Last Modified: Mon, 27 Dec 2021 18:20:21 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a52b1de785dfc0bc3d07ee3d3f619d0681bc34b7eeee205db16da01946663a91`  
		Last Modified: Mon, 27 Dec 2021 18:20:21 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.2-alpine` - linux; s390x

```console
$ docker pull spiped@sha256:e5972c57d035e42883aca7354deb92cd65a9bbbc8d5d6aaa8b364891cbdba20d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.0 MB (4034365 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6b297cc2c896c2d11d20abe50ce763f606504b9aad55d18a6c8bcf3407db63c8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 24 Nov 2021 20:41:23 GMT
ADD file:cd24c711a2ef431b3ff94f9a02bfc42f159bc60de1d0eceecafea4e8af02441d in / 
# Wed, 24 Nov 2021 20:41:23 GMT
CMD ["/bin/sh"]
# Mon, 27 Dec 2021 18:42:02 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Mon, 27 Dec 2021 18:42:04 GMT
RUN apk add --no-cache libssl1.1
# Mon, 27 Dec 2021 18:42:04 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Mon, 27 Dec 2021 18:42:09 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Mon, 27 Dec 2021 18:42:09 GMT
VOLUME [/spiped]
# Mon, 27 Dec 2021 18:42:09 GMT
WORKDIR /spiped
# Mon, 27 Dec 2021 18:42:10 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 27 Dec 2021 18:42:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 27 Dec 2021 18:42:10 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:d6baca485f3d0f7c77221be60fbef5db014a5ef9d8f53db4a310c947c690d189`  
		Last Modified: Wed, 24 Nov 2021 20:42:15 GMT  
		Size: 2.6 MB (2605944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:631b52683dec736314bc4a995e6d4aa8fe70ccec0ccb0b4f0349543c0b9d315d`  
		Last Modified: Mon, 27 Dec 2021 18:42:54 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8a99397842c922d6589a78e8df8f8b4feac626485047c36e902a2966e19dfe2`  
		Last Modified: Mon, 27 Dec 2021 18:42:54 GMT  
		Size: 7.7 KB (7743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:556dc6882e78ba3518dbab7eaae8412b06f9ad7e09122f6478d9d1cc80b978e4`  
		Last Modified: Mon, 27 Dec 2021 18:42:55 GMT  
		Size: 1.4 MB (1418939 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9680c33180071ffeb1ac5cfe629daff266a5cf86a4072e251e4b0bef70d20b3`  
		Last Modified: Mon, 27 Dec 2021 18:42:54 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2742416115dba0ead2f2dc1f9aa438a1ef9179b4e11cfd9d665c918f92b53c55`  
		Last Modified: Mon, 27 Dec 2021 18:42:54 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:alpine`

```console
$ docker pull spiped@sha256:b1089d3c383de79c5a463d8f6b45c46f804588a33a967ff66469a76a654169f0
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
$ docker pull spiped@sha256:f4aaae543ff5aba181d531aa5504251d883a40559812a85cff78c7526d3f713e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4523758 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d71e35e9a762b19f1a767061f3cf181454d7090d64dec7acef852f68d4c01262`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 24 Nov 2021 20:19:40 GMT
ADD file:9233f6f2237d79659a9521f7e390df217cec49f1a8aa3a12147bbca1956acdb9 in / 
# Wed, 24 Nov 2021 20:19:40 GMT
CMD ["/bin/sh"]
# Mon, 27 Dec 2021 19:10:10 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Mon, 27 Dec 2021 19:10:11 GMT
RUN apk add --no-cache libssl1.1
# Mon, 27 Dec 2021 19:10:11 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Mon, 27 Dec 2021 19:10:22 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Mon, 27 Dec 2021 19:10:22 GMT
VOLUME [/spiped]
# Mon, 27 Dec 2021 19:10:22 GMT
WORKDIR /spiped
# Mon, 27 Dec 2021 19:10:22 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 27 Dec 2021 19:10:23 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 27 Dec 2021 19:10:23 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:59bf1c3509f33515622619af21ed55bbe26d24913cedbca106468a5fb37a50c3`  
		Last Modified: Wed, 24 Nov 2021 20:20:05 GMT  
		Size: 2.8 MB (2818413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50c602680384586a0fe7febde9f529aea001928a6d26e84d9a3f7be94049ef27`  
		Last Modified: Mon, 27 Dec 2021 19:10:53 GMT  
		Size: 1.3 KB (1265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee913a58b01d029ed458f92226b5b52747e0877c39585d9f93ec5dd2ef0a8cf9`  
		Last Modified: Mon, 27 Dec 2021 19:10:53 GMT  
		Size: 7.7 KB (7749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd8bf950f1ef1b7c96ba1781b5a87d4044135ae197871b261e86d74bc35a8bf5`  
		Last Modified: Mon, 27 Dec 2021 19:10:54 GMT  
		Size: 1.7 MB (1695862 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56d41f282509324afd98cc83dab31aee8ba6459973698c8ccaf3978cddc4ede4`  
		Last Modified: Mon, 27 Dec 2021 19:10:53 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8ba766abbc809d26737c9cc94fbe15a6311c603bfd673bd6db553169dd0f141`  
		Last Modified: Mon, 27 Dec 2021 19:10:53 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; arm variant v6

```console
$ docker pull spiped@sha256:b6482b55d0b7700b0393783f0ea8e49e6a4329c07187fdf826b6902d0ccfa3e6
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.1 MB (4080480 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1df9593d1c7a93c5f606ef97c05cc8d86e1a5bce25cd9895c104e2e1a7edbe19`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 24 Nov 2021 21:08:16 GMT
ADD file:61137e0aa49ba06f57ac69466fe2fb116f580b5e6159d56f846b1d72c4a3c814 in / 
# Wed, 24 Nov 2021 21:08:16 GMT
CMD ["/bin/sh"]
# Mon, 27 Dec 2021 17:49:44 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Mon, 27 Dec 2021 17:49:46 GMT
RUN apk add --no-cache libssl1.1
# Mon, 27 Dec 2021 17:49:47 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Mon, 27 Dec 2021 17:50:06 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Mon, 27 Dec 2021 17:50:07 GMT
VOLUME [/spiped]
# Mon, 27 Dec 2021 17:50:07 GMT
WORKDIR /spiped
# Mon, 27 Dec 2021 17:50:08 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 27 Dec 2021 17:50:08 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 27 Dec 2021 17:50:09 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:e4a43de54da9e309482f6762f0c11f5f547cd8fd61a49c5f158453066162023e`  
		Last Modified: Wed, 24 Nov 2021 21:09:46 GMT  
		Size: 2.6 MB (2631421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c04f27a458746dfc1d07b0b03b9b8f205b08ebef9d6060ef92027b709fee313e`  
		Last Modified: Mon, 27 Dec 2021 17:50:41 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fffa3b0ec9bb32d2efab9fa903af078baf37201f4ec2026c0afce9c14156229`  
		Last Modified: Mon, 27 Dec 2021 17:50:41 GMT  
		Size: 7.7 KB (7743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e2344d51f830abe738f710343c04e056b2ec80e33a48522878caa568c9f553c`  
		Last Modified: Mon, 27 Dec 2021 17:50:42 GMT  
		Size: 1.4 MB (1439576 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd3eeeb2545dce6884a99d866ca20bd742d7e133aacf869b4cddbe974bfde627`  
		Last Modified: Mon, 27 Dec 2021 17:50:41 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2681e39729f29c202bc97138be5a28bb84d92220ffe45df47fb643301eef46aa`  
		Last Modified: Mon, 27 Dec 2021 17:50:41 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; arm variant v7

```console
$ docker pull spiped@sha256:277d22d33ab8cd23ff5bf04d4e60841c8a335de8fdb772173601e9a4d4cb00bf
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.8 MB (3802328 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2f94c64b2c706a58b82aa60bafca69c1fd15fb76714e5ca4aae0f1e4a47e3f1d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 24 Nov 2021 21:42:11 GMT
ADD file:ca436da5b0bfc9c0e2fc685533c6628918000c8fff109fe9a8da625b9a798002 in / 
# Wed, 24 Nov 2021 21:42:11 GMT
CMD ["/bin/sh"]
# Mon, 27 Dec 2021 18:00:04 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Mon, 27 Dec 2021 18:00:06 GMT
RUN apk add --no-cache libssl1.1
# Mon, 27 Dec 2021 18:00:06 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Mon, 27 Dec 2021 18:00:25 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Mon, 27 Dec 2021 18:00:26 GMT
VOLUME [/spiped]
# Mon, 27 Dec 2021 18:00:26 GMT
WORKDIR /spiped
# Mon, 27 Dec 2021 18:00:27 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 27 Dec 2021 18:00:27 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 27 Dec 2021 18:00:28 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:5480d2ca1740c20ce17652e01ed2265cdc914458acd41256a2b1ccff28f2762c`  
		Last Modified: Wed, 24 Nov 2021 21:43:40 GMT  
		Size: 2.4 MB (2434764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fca194041621ab40d8e7f24b7f7e82aa07760b2dafcd26472bd7fae96171989a`  
		Last Modified: Mon, 27 Dec 2021 18:01:41 GMT  
		Size: 1.3 KB (1267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7e934f04cb0ca6a107389bcb614eb02143fb079eef09a47a9248e3c4ff07864`  
		Last Modified: Mon, 27 Dec 2021 18:01:41 GMT  
		Size: 7.7 KB (7749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4111e5d44f2316d799c8b9144d8f35765b0bf330b8d596d99e504969cd48e07a`  
		Last Modified: Mon, 27 Dec 2021 18:01:42 GMT  
		Size: 1.4 MB (1358077 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f46d751b026ad913b2a48630c96460959a733e75728d55aafbd389197bf81857`  
		Last Modified: Mon, 27 Dec 2021 18:01:41 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5140561b01c4c6ae8b47c729fd289d7eef4a2b0e9c427a6bd35a86747e966206`  
		Last Modified: Mon, 27 Dec 2021 18:01:41 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:f2401c455a0fde4f25cae4b46bad0721c19ac135bc6efa4e5b3c46c5b04aa1cd
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.3 MB (4289462 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:017a5c1ca8bdf46589e6ab7b72a939d86283ebdb51f63d37bc1c41f07a36600f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 24 Nov 2021 20:39:20 GMT
ADD file:df53811312284306901fdaaff0a357a4bf40d631e662fe9ce6d342442e494b6c in / 
# Wed, 24 Nov 2021 20:39:20 GMT
CMD ["/bin/sh"]
# Mon, 27 Dec 2021 19:39:28 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Mon, 27 Dec 2021 19:39:29 GMT
RUN apk add --no-cache libssl1.1
# Mon, 27 Dec 2021 19:39:30 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Mon, 27 Dec 2021 19:39:41 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Mon, 27 Dec 2021 19:39:42 GMT
VOLUME [/spiped]
# Mon, 27 Dec 2021 19:39:43 GMT
WORKDIR /spiped
# Mon, 27 Dec 2021 19:39:45 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 27 Dec 2021 19:39:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 27 Dec 2021 19:39:46 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:9b3977197b4f2147bdd31e1271f811319dcd5c2fc595f14e81f5351ab6275b99`  
		Last Modified: Wed, 24 Nov 2021 20:39:59 GMT  
		Size: 2.7 MB (2715434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4642588fd355ccb1af1d6dc41cc14b5117bbd4f30adb691aade26686c4d5c116`  
		Last Modified: Mon, 27 Dec 2021 19:40:28 GMT  
		Size: 1.2 KB (1240 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd8e58927c1555e9461b11588b3accaf4b9d1018264a3d1ac75dbd1d03c2212e`  
		Last Modified: Mon, 27 Dec 2021 19:40:28 GMT  
		Size: 7.7 KB (7712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd181fff8bea1f7e317b2af57ee7244e2a0b5226b26df42dc9a9d836cf504dec`  
		Last Modified: Mon, 27 Dec 2021 19:40:28 GMT  
		Size: 1.6 MB (1564638 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f65407c84c38d42d7b099c55334ee34fc2e9f581954ed4e92bab1773599189df`  
		Last Modified: Mon, 27 Dec 2021 19:40:28 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97f56c7d1e54220168de3e0523afd6a69f29f86199d05ee4681c356afaa2e36a`  
		Last Modified: Mon, 27 Dec 2021 19:40:28 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; 386

```console
$ docker pull spiped@sha256:fc962e82018b393667a7d2b43c9bee0b19c4650fadcc16335cf984b44d859d65
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4539662 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:64dc6529164f107ee83f0edafa6bcf506960ffc646e0e9e161cb2640feb90f96`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 24 Nov 2021 20:53:48 GMT
ADD file:b9a17131c440053f2f67e127b447645f25fd7de2d6caca42f569cafab6291855 in / 
# Wed, 24 Nov 2021 20:53:48 GMT
CMD ["/bin/sh"]
# Mon, 27 Dec 2021 18:39:31 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Mon, 27 Dec 2021 18:39:32 GMT
RUN apk add --no-cache libssl1.1
# Mon, 27 Dec 2021 18:39:33 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Mon, 27 Dec 2021 18:39:45 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Mon, 27 Dec 2021 18:39:45 GMT
VOLUME [/spiped]
# Mon, 27 Dec 2021 18:39:45 GMT
WORKDIR /spiped
# Mon, 27 Dec 2021 18:39:46 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 27 Dec 2021 18:39:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 27 Dec 2021 18:39:46 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:e6889e0d66307a4b916fc844f2dcbc03245c63bc4189dd3e88126d9dcf2f9231`  
		Last Modified: Wed, 24 Nov 2021 20:54:48 GMT  
		Size: 2.8 MB (2827117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc39bdf14cf5dcbf704b50f736d82a339b1879574765ef87fbbf5ecb8d7d574e`  
		Last Modified: Mon, 27 Dec 2021 18:40:32 GMT  
		Size: 1.3 KB (1266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7128f9e1b03ce01ba1b51bce7aa1bc585b6c3e6ce1650259721463f363e9aaab`  
		Last Modified: Mon, 27 Dec 2021 18:40:32 GMT  
		Size: 7.8 KB (7750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb2ebf4c9a2525659cebde6ee501a457c4a31d364f3f568be0f076191d96855d`  
		Last Modified: Mon, 27 Dec 2021 18:40:33 GMT  
		Size: 1.7 MB (1703060 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75adf8fe66ad441b9c8e209efcc7d5b68b61c6a33e05b3aed401756e55493d07`  
		Last Modified: Mon, 27 Dec 2021 18:40:32 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99b656b54398310f3a0f295c7737034732b9ee5c7e294ad5df27230309fff8ae`  
		Last Modified: Mon, 27 Dec 2021 18:40:32 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; ppc64le

```console
$ docker pull spiped@sha256:bdb5c0f748fb29dd4c96f71d1eec1c471f348b68e39063a5674e88c6655400ac
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.4 MB (4447359 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c2ab0ba82f0f9badd5246249195a67d4e12bc4f6cfb1822b3454aca1c3dae586`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 24 Nov 2021 20:20:16 GMT
ADD file:57115dca2eb707f46b6301e75174e6aa316fb02ac28643b91429b75be51bd8c8 in / 
# Wed, 24 Nov 2021 20:20:20 GMT
CMD ["/bin/sh"]
# Mon, 27 Dec 2021 18:18:59 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Mon, 27 Dec 2021 18:19:06 GMT
RUN apk add --no-cache libssl1.1
# Mon, 27 Dec 2021 18:19:08 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Mon, 27 Dec 2021 18:19:22 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Mon, 27 Dec 2021 18:19:25 GMT
VOLUME [/spiped]
# Mon, 27 Dec 2021 18:19:28 GMT
WORKDIR /spiped
# Mon, 27 Dec 2021 18:19:28 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 27 Dec 2021 18:19:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 27 Dec 2021 18:19:33 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:159b5dcb1717c815c76ff5ea1db730e18e8609c9090238e43282856db9e71f47`  
		Last Modified: Wed, 24 Nov 2021 20:21:14 GMT  
		Size: 2.8 MB (2814780 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5ef2b17ec4445a63d712289fc62b0e3e30ab15992e0a0d38ab25e290abcb38e`  
		Last Modified: Mon, 27 Dec 2021 18:20:21 GMT  
		Size: 1.3 KB (1274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:210460e69fcfc508eae94f5666c4fc57c0cdf6163c3a6e39710f5da7a2e5ceb6`  
		Last Modified: Mon, 27 Dec 2021 18:20:21 GMT  
		Size: 7.7 KB (7737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0860c3c69dcd2673558f15fc9c46c8447274ce23c207e936804fe5a268e5e7f`  
		Last Modified: Mon, 27 Dec 2021 18:20:22 GMT  
		Size: 1.6 MB (1623097 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13cd96844150db5d01e32349b5f650aafd01dd1789c2a11fee82b6f55bd43560`  
		Last Modified: Mon, 27 Dec 2021 18:20:21 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a52b1de785dfc0bc3d07ee3d3f619d0681bc34b7eeee205db16da01946663a91`  
		Last Modified: Mon, 27 Dec 2021 18:20:21 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; s390x

```console
$ docker pull spiped@sha256:e5972c57d035e42883aca7354deb92cd65a9bbbc8d5d6aaa8b364891cbdba20d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.0 MB (4034365 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6b297cc2c896c2d11d20abe50ce763f606504b9aad55d18a6c8bcf3407db63c8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 24 Nov 2021 20:41:23 GMT
ADD file:cd24c711a2ef431b3ff94f9a02bfc42f159bc60de1d0eceecafea4e8af02441d in / 
# Wed, 24 Nov 2021 20:41:23 GMT
CMD ["/bin/sh"]
# Mon, 27 Dec 2021 18:42:02 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Mon, 27 Dec 2021 18:42:04 GMT
RUN apk add --no-cache libssl1.1
# Mon, 27 Dec 2021 18:42:04 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Mon, 27 Dec 2021 18:42:09 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Mon, 27 Dec 2021 18:42:09 GMT
VOLUME [/spiped]
# Mon, 27 Dec 2021 18:42:09 GMT
WORKDIR /spiped
# Mon, 27 Dec 2021 18:42:10 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 27 Dec 2021 18:42:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 27 Dec 2021 18:42:10 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:d6baca485f3d0f7c77221be60fbef5db014a5ef9d8f53db4a310c947c690d189`  
		Last Modified: Wed, 24 Nov 2021 20:42:15 GMT  
		Size: 2.6 MB (2605944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:631b52683dec736314bc4a995e6d4aa8fe70ccec0ccb0b4f0349543c0b9d315d`  
		Last Modified: Mon, 27 Dec 2021 18:42:54 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8a99397842c922d6589a78e8df8f8b4feac626485047c36e902a2966e19dfe2`  
		Last Modified: Mon, 27 Dec 2021 18:42:54 GMT  
		Size: 7.7 KB (7743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:556dc6882e78ba3518dbab7eaae8412b06f9ad7e09122f6478d9d1cc80b978e4`  
		Last Modified: Mon, 27 Dec 2021 18:42:55 GMT  
		Size: 1.4 MB (1418939 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9680c33180071ffeb1ac5cfe629daff266a5cf86a4072e251e4b0bef70d20b3`  
		Last Modified: Mon, 27 Dec 2021 18:42:54 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2742416115dba0ead2f2dc1f9aa438a1ef9179b4e11cfd9d665c918f92b53c55`  
		Last Modified: Mon, 27 Dec 2021 18:42:54 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:latest`

```console
$ docker pull spiped@sha256:d9abc65404acc410b3f94bd812f875d66ad7304604f00ee6464be3ab291d57b3
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
$ docker pull spiped@sha256:dc2c3a3712eacb11a556c86bc2a6b606ba5a0edff87bf3638c159b85a1135448
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.3 MB (37335950 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1d472f594ea8090d6f3cbeb573986f7840e512b983c9def18699f62efe8bcc04`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 26 Jan 2022 01:40:35 GMT
ADD file:90495c24c897ec47982e200f732f8be3109fcd791691ddffae0756898f91024f in / 
# Wed, 26 Jan 2022 01:40:36 GMT
CMD ["bash"]
# Thu, 27 Jan 2022 02:32:24 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Thu, 27 Jan 2022 02:32:27 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Thu, 27 Jan 2022 02:32:28 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 27 Jan 2022 02:32:58 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 27 Jan 2022 02:32:58 GMT
VOLUME [/spiped]
# Thu, 27 Jan 2022 02:32:59 GMT
WORKDIR /spiped
# Thu, 27 Jan 2022 02:33:00 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 27 Jan 2022 02:33:00 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 27 Jan 2022 02:33:01 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:5eb5b503b37671af16371272f9c5313a3e82f1d0756e14506704489ad9900803`  
		Last Modified: Wed, 26 Jan 2022 01:46:39 GMT  
		Size: 31.4 MB (31366257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6a2517caec378bb5ccef0a0d6e52b5e25a629d59a240188bd605cf9f98bc57d`  
		Last Modified: Thu, 27 Jan 2022 02:33:32 GMT  
		Size: 1.7 KB (1734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9824d58dd5193ef98f897a6ac1feb9749d5f2371324023d2ca61dae51fb70e6`  
		Last Modified: Thu, 27 Jan 2022 02:33:32 GMT  
		Size: 1.1 KB (1051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d878a5544ecf1374c1348226765bcdd58a98e4e3d4c98f89ccf5fa10a7ca8ff`  
		Last Modified: Thu, 27 Jan 2022 02:33:34 GMT  
		Size: 6.0 MB (5966436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:754c3acbb4e4a2d6ba3fb19ebf6f464a6af124ca39e832916a9e20959ba6cb46`  
		Last Modified: Thu, 27 Jan 2022 02:33:32 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ddcc8c75157adfeb6f31357486186ad845c90e035dbcc13ad22c90c787c7769`  
		Last Modified: Thu, 27 Jan 2022 02:33:32 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; arm variant v5

```console
$ docker pull spiped@sha256:d35164b325c8b4cebf396e69ccd1cb2f1c7c2c813f1645f3a9d7fa533a214761
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.9 MB (33940215 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7d587f5e0871df03606d30179c325953573c55459a421e180a9ef24904dddb49`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 26 Jan 2022 01:41:57 GMT
ADD file:4ccea3cb033595f7bd9896126e94a8a19199b987bedd87b3c0700d8b29baa1fb in / 
# Wed, 26 Jan 2022 01:41:58 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 13:48:20 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 26 Jan 2022 13:48:29 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 13:48:30 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 26 Jan 2022 13:49:20 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 26 Jan 2022 13:49:21 GMT
VOLUME [/spiped]
# Wed, 26 Jan 2022 13:49:21 GMT
WORKDIR /spiped
# Wed, 26 Jan 2022 13:49:22 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 26 Jan 2022 13:49:23 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 26 Jan 2022 13:49:23 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:247ff78919074ec9db7cccd537dd6eb4d7e2788013b7ef07443e345d91c8a588`  
		Last Modified: Wed, 26 Jan 2022 01:57:36 GMT  
		Size: 28.9 MB (28909638 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cf343e822da1ce4be935758169ff31bce470bf1fe1276540174154bb3f2668d`  
		Last Modified: Wed, 26 Jan 2022 13:49:57 GMT  
		Size: 1.7 KB (1727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c398ac3bf4e12d1412bc45d6f9286f5c1700b12eaa24f0978ff6ab2197fe87d`  
		Last Modified: Wed, 26 Jan 2022 13:49:57 GMT  
		Size: 1.1 KB (1051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:797b9d89af1464c4395401f548e40c856ec3fb4894d839f6f9f420a1e2028f16`  
		Last Modified: Wed, 26 Jan 2022 13:50:02 GMT  
		Size: 5.0 MB (5027326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81ef5c7608dbb1e039ea48a4ffc9bac9710189cf564f106cb68cead03b7e4253`  
		Last Modified: Wed, 26 Jan 2022 13:49:57 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb5277a969518e6a9f8d7485c29504d113db9236a9d49b296bd38c4d422c67ea`  
		Last Modified: Wed, 26 Jan 2022 13:49:57 GMT  
		Size: 344.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; arm variant v7

```console
$ docker pull spiped@sha256:3d916238fd77df17911ab19dc7587e33dd0cada5997bb822a6341b6bc4d22d8e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.3 MB (31315488 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c1f89cc56381f998f2473d68073ecab8c87f42eaa6bc2bfeef9e59d7cffaef6f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 26 Jan 2022 01:42:08 GMT
ADD file:7f27f5b43b7cb04e509fe145266d9bdeacfcacb024cafac32e57ef1c831d5ea7 in / 
# Wed, 26 Jan 2022 01:42:09 GMT
CMD ["bash"]
# Thu, 27 Jan 2022 02:05:29 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Thu, 27 Jan 2022 02:05:36 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Thu, 27 Jan 2022 02:05:37 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 27 Jan 2022 02:06:23 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 27 Jan 2022 02:06:24 GMT
VOLUME [/spiped]
# Thu, 27 Jan 2022 02:06:24 GMT
WORKDIR /spiped
# Thu, 27 Jan 2022 02:06:25 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 27 Jan 2022 02:06:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 27 Jan 2022 02:06:26 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:aaef1f1162ec03e01b5b955d41da400544ec2374093ae3dbc330ab2bb36df3e1`  
		Last Modified: Wed, 26 Jan 2022 01:57:59 GMT  
		Size: 26.6 MB (26564933 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b839df330fe51f570a9646e1b8027ad2653336fbd121c12312e0baddcad0d5cd`  
		Last Modified: Thu, 27 Jan 2022 02:07:27 GMT  
		Size: 1.7 KB (1727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b58b2cda412f0922939bcdd348b6d2e3cd4dccd6036926ca90ec596a1b13fbf2`  
		Last Modified: Thu, 27 Jan 2022 02:07:27 GMT  
		Size: 1.1 KB (1051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3936070b02fda979073a59e440e1fb34695f2a5ab92ee369696afed5e3937b5`  
		Last Modified: Thu, 27 Jan 2022 02:07:32 GMT  
		Size: 4.7 MB (4747305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4dd327a7a9576943baaf60df0bdb6ff237147bcfd0f8ee37cf0a591a60131946`  
		Last Modified: Thu, 27 Jan 2022 02:07:27 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60e3ddb56b8bd24d775b3c0d169d4a1a1e03f18562970b41a9d187bc0b0161d8`  
		Last Modified: Thu, 27 Jan 2022 02:07:27 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:ec801aacab912356ed8782ef99c1d53dea85c30a74b6c982e1c33ab60cf936f5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.3 MB (35329660 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5ec3eef7cdb77d28d34401d13e367b0a1ae12678889d9b3df643c3baf3b58b27`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 26 Jan 2022 01:42:31 GMT
ADD file:0ec6f47a8857bf8e6cef71ed8f864be7ce1790ff6ed04fd4201e7dbde4728d3a in / 
# Wed, 26 Jan 2022 01:42:31 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 09:19:54 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 26 Jan 2022 09:19:57 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 09:19:57 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 26 Jan 2022 09:20:14 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 26 Jan 2022 09:20:15 GMT
VOLUME [/spiped]
# Wed, 26 Jan 2022 09:20:16 GMT
WORKDIR /spiped
# Wed, 26 Jan 2022 09:20:18 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 26 Jan 2022 09:20:18 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 26 Jan 2022 09:20:19 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:8998bd30e6a1204d13403045766edbe14f941b52087465f5d140ab63c8b113bf`  
		Last Modified: Wed, 26 Jan 2022 01:49:04 GMT  
		Size: 30.1 MB (30056774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5c0deb70595215cef3194a8d1bea35a623260a4a537174ac0174e9388d20b66`  
		Last Modified: Wed, 26 Jan 2022 09:20:48 GMT  
		Size: 1.6 KB (1618 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:034b8f66f1f2f1b93a71339b2b1c5e595c4574868f5e7d0f06f2c0bf51174940`  
		Last Modified: Wed, 26 Jan 2022 09:20:48 GMT  
		Size: 923.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b14f060bef623dc32f29a79d5b26a6879c4aa9267e5b87ecf4ce0e10f5dfb170`  
		Last Modified: Wed, 26 Jan 2022 09:20:49 GMT  
		Size: 5.3 MB (5269907 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99a6c1e6b86dbfff40179fb98822e12212a0b2867e6d5240159c942eb3854996`  
		Last Modified: Wed, 26 Jan 2022 09:20:47 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce3566ea2e7139f3188bf62015b6b85e2bb8e4c6c1ad89ef5c389ef067c3c0c2`  
		Last Modified: Wed, 26 Jan 2022 09:20:48 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; 386

```console
$ docker pull spiped@sha256:d62c6f333ea8dc55c74566a02c6966fdb05a5373f946c62e78dc4535e7c6439b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.3 MB (40272052 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:240f8e63cba198164b163f99564af3065d0d08a532f87c59c4fafe8bc87fee95`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 26 Jan 2022 01:39:55 GMT
ADD file:876ebf07c65841f4840842086c883af48e07386964fe6d643ba193895ec2a582 in / 
# Wed, 26 Jan 2022 01:39:56 GMT
CMD ["bash"]
# Thu, 27 Jan 2022 04:50:43 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Thu, 27 Jan 2022 04:50:51 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Thu, 27 Jan 2022 04:50:52 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 27 Jan 2022 04:51:42 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 27 Jan 2022 04:51:43 GMT
VOLUME [/spiped]
# Thu, 27 Jan 2022 04:51:43 GMT
WORKDIR /spiped
# Thu, 27 Jan 2022 04:51:44 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 27 Jan 2022 04:51:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 27 Jan 2022 04:51:45 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:86933886b1754aba091548cf031a9bca88cdce9bb4fc1f28bb38b61594c2c2c7`  
		Last Modified: Wed, 26 Jan 2022 01:48:57 GMT  
		Size: 32.4 MB (32377406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:007b643ac135004248e51a7df9b02d61247a5ace740507e11d1238f5c6559f0a`  
		Last Modified: Thu, 27 Jan 2022 04:52:38 GMT  
		Size: 1.7 KB (1729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe9889a275b3dcd9c9d9380a6b23eff3430e0928931f872c594a56aca75b74a0`  
		Last Modified: Thu, 27 Jan 2022 04:52:37 GMT  
		Size: 1.1 KB (1052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a8f1418eeaf635a0d7c0ff4a2a9200da488617f0d749336ec280dc483d43299`  
		Last Modified: Thu, 27 Jan 2022 04:52:41 GMT  
		Size: 7.9 MB (7891393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edd6784674f4cacc537045d525761932e2f277aa61bb5029896a120518807d30`  
		Last Modified: Thu, 27 Jan 2022 04:52:38 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4489e826d0a9aaec6002d3f886c71d2e729d1a47b745a9a82bbdae810d0345f2`  
		Last Modified: Thu, 27 Jan 2022 04:52:37 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; mips64le

```console
$ docker pull spiped@sha256:5ff06e4c09b7b50640a863ff273ef3b49b36efa00ee15a15bc68e0d0c9c31d4c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.3 MB (35341414 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:13ee9a2841cd7deb5c6e19a80d798eaf34ac36066234c76dd87975bb8adbaa97`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 26 Jan 2022 01:42:45 GMT
ADD file:61767027a5ab46afbcd4079d200abe8d663326adc96fa28ca8c8955a06d9322e in / 
# Wed, 26 Jan 2022 01:42:46 GMT
CMD ["bash"]
# Thu, 27 Jan 2022 14:17:20 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Thu, 27 Jan 2022 14:17:32 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Thu, 27 Jan 2022 14:17:32 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 27 Jan 2022 14:18:22 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 27 Jan 2022 14:18:22 GMT
VOLUME [/spiped]
# Thu, 27 Jan 2022 14:18:23 GMT
WORKDIR /spiped
# Thu, 27 Jan 2022 14:18:23 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 27 Jan 2022 14:18:23 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 27 Jan 2022 14:18:24 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:266e7d2b59483859eaa1711d2afeb25ea4458eeb36b3e909372930db1f834d7f`  
		Last Modified: Wed, 26 Jan 2022 01:51:23 GMT  
		Size: 29.6 MB (29632834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bed329584043834b57b17c1f7fb178849a18c1e185f6a1c3790d7e4f3aabdad`  
		Last Modified: Thu, 27 Jan 2022 14:18:40 GMT  
		Size: 1.7 KB (1732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1221de7514f3a6d44d793ddbb512b55c28feed96691f900bce757c1ad89f2db`  
		Last Modified: Thu, 27 Jan 2022 14:18:41 GMT  
		Size: 1.0 KB (1026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b78ea45f3c4a37e62bd246764fe6840be44718f3a906daf70e4d583cf4aaa6af`  
		Last Modified: Thu, 27 Jan 2022 14:18:46 GMT  
		Size: 5.7 MB (5705384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53d16d14491067074a517e226e1dced4190135104702609415f883fa63d46ee3`  
		Last Modified: Thu, 27 Jan 2022 14:18:41 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2dba9fb9a37e3aafad3abba08e85db2fd96587c52de4e6a2df6ef442c2538a96`  
		Last Modified: Thu, 27 Jan 2022 14:18:40 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; ppc64le

```console
$ docker pull spiped@sha256:f9a8ff652bffe474afdf6cf3da90bcb5fabc4674ad021bc3ddf11100309fcbe7
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.3 MB (41274405 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b89132621e69403b6931ac29ab0fdf93d27e91888256b85a1de6d142d4046a56`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 26 Jan 2022 01:46:51 GMT
ADD file:c03f34c221e57fa5cb625c166d1db9f72d6ba2fa17a3c41a5d04d6875d098949 in / 
# Wed, 26 Jan 2022 01:46:57 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 22:15:10 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 26 Jan 2022 22:15:19 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 22:15:21 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 26 Jan 2022 22:17:04 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 26 Jan 2022 22:17:09 GMT
VOLUME [/spiped]
# Wed, 26 Jan 2022 22:17:12 GMT
WORKDIR /spiped
# Wed, 26 Jan 2022 22:17:14 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 26 Jan 2022 22:17:16 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 26 Jan 2022 22:17:20 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:3149ee4a73508a4c39107d64a3fdc1b021626a22a0ac95e62fa0cea49ab77fba`  
		Last Modified: Wed, 26 Jan 2022 01:57:01 GMT  
		Size: 35.3 MB (35273030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43b54b67a6f99dac2db476b7702d015eb56f81c2d623bc96fd32aae703f0b732`  
		Last Modified: Wed, 26 Jan 2022 22:17:51 GMT  
		Size: 1.7 KB (1739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f1241c00e00d3316ad39effb0518ce815abfcf876ea4efac9de53b2fdc560da`  
		Last Modified: Wed, 26 Jan 2022 22:17:51 GMT  
		Size: 1.1 KB (1054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86ddc628c1bd5eff84e7cb044e5c93444f7e53a189710ec4b2f0213ffc82cb0f`  
		Last Modified: Wed, 26 Jan 2022 22:17:53 GMT  
		Size: 6.0 MB (5998110 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:706174d608bd436d8e8d5fb2c9d2cb2ff6ea71118584ab8a35af39ae43d5d90f`  
		Last Modified: Wed, 26 Jan 2022 22:17:51 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7858b7298d1ed34eff1ac6724d4bce1c8fc696786a68d28c115f2bc843aad9ab`  
		Last Modified: Wed, 26 Jan 2022 22:17:51 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; s390x

```console
$ docker pull spiped@sha256:dc9f30aec35bbc203643e902934a1b5e6140c26c166e0462f571d07f09e3fab5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.8 MB (34836084 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:40e931303d1bd986c9a5293d6f7f2f3dc4a9599d5af26cc8a933a43253c32f21`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 26 Jan 2022 01:41:13 GMT
ADD file:03b224b82f458b08d3b5071e42b67915a3db309332c0fc9229db7cf1148bc1b5 in / 
# Wed, 26 Jan 2022 01:41:15 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 11:27:45 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 26 Jan 2022 11:27:47 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 11:27:48 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 26 Jan 2022 11:28:01 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 26 Jan 2022 11:28:01 GMT
VOLUME [/spiped]
# Wed, 26 Jan 2022 11:28:02 GMT
WORKDIR /spiped
# Wed, 26 Jan 2022 11:28:02 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 26 Jan 2022 11:28:02 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 26 Jan 2022 11:28:02 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:70bed29526f8483937e4d2540d19256d30786007c7c321e717e00d2e74700380`  
		Last Modified: Wed, 26 Jan 2022 01:46:57 GMT  
		Size: 29.6 MB (29647071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87ff2a6a6375f95aac16175fe1a27e34e664c34d69d5ed1efa5d976ad0e7b947`  
		Last Modified: Wed, 26 Jan 2022 11:28:34 GMT  
		Size: 1.7 KB (1736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66b439c0f82c7b1a5745542aedc040eca1c81fae487012b1886220413a47d903`  
		Last Modified: Wed, 26 Jan 2022 11:28:34 GMT  
		Size: 1.1 KB (1052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93908f45004e2f2d6aee48dec977a4e4405bf91858cafb05024b750ca56aa9d7`  
		Last Modified: Wed, 26 Jan 2022 11:28:35 GMT  
		Size: 5.2 MB (5185752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9c094f1ad2a6f023f6f79a11bb9a375b3f52a100501b0d1191d839085802bba`  
		Last Modified: Wed, 26 Jan 2022 11:28:34 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83eccc997a02a9c670eaa7e3d2dfd923453818685f1b2c3ddfff0bf985a890d4`  
		Last Modified: Wed, 26 Jan 2022 11:28:34 GMT  
		Size: 344.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
