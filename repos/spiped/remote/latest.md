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
