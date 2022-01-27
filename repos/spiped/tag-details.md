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
$ docker pull spiped@sha256:695728df46d9899ea5caf49d16190d360575886d18bf0948f55bd1d82e81ec80
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
$ docker pull spiped@sha256:27655c03e38daa8aa4afed06a3d4c9f6127f971fe9ed16b98c8f48cc902ef314
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.3 MB (37327359 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:03b1412c46e8325a0589c93bac2d1990523e7e07b13698c2a9cb573fed4960bd`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 21 Dec 2021 01:22:43 GMT
ADD file:09675d11695f65c55efdc393ff0cd32f30194cd7d0fbef4631eebfed4414ac97 in / 
# Tue, 21 Dec 2021 01:22:43 GMT
CMD ["bash"]
# Mon, 27 Dec 2021 19:09:37 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Mon, 27 Dec 2021 19:09:40 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Mon, 27 Dec 2021 19:09:40 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Mon, 27 Dec 2021 19:10:01 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Mon, 27 Dec 2021 19:10:01 GMT
VOLUME [/spiped]
# Mon, 27 Dec 2021 19:10:01 GMT
WORKDIR /spiped
# Mon, 27 Dec 2021 19:10:02 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 27 Dec 2021 19:10:02 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 27 Dec 2021 19:10:02 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:a2abf6c4d29d43a4bf9fbb769f524d0fb36a2edab49819c1bf3e76f409f953ea`  
		Last Modified: Tue, 21 Dec 2021 01:27:48 GMT  
		Size: 31.4 MB (31357624 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d547106b69c042e6267b4030a20ff577bcfc9917ebf0a49d697c1d2819992416`  
		Last Modified: Mon, 27 Dec 2021 19:10:37 GMT  
		Size: 1.7 KB (1733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eda7224a790705cc7b53c6c57deb18f74ceeddf1a6a748cb1c59dd1d4f8b7c03`  
		Last Modified: Mon, 27 Dec 2021 19:10:37 GMT  
		Size: 1.1 KB (1055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7082f5785f33700aa63be5c0b314767d2b6039850a3dfcba2547dc823a464fff`  
		Last Modified: Mon, 27 Dec 2021 19:10:38 GMT  
		Size: 6.0 MB (5966475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8ceb17a2971caaf21db95998adb68b036ca18a5890dede0280840f93e2dabcb`  
		Last Modified: Mon, 27 Dec 2021 19:10:37 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7aed5299a2faa639446a4fc16f9364a4b444cae0a4c9855837063682ec7e4a88`  
		Last Modified: Mon, 27 Dec 2021 19:10:37 GMT  
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
$ docker pull spiped@sha256:126609a7885028d241e5a5879a81db1e409324ad4299d35fa13d8cb81db7741b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.3 MB (40265566 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e63888bbd27971f057151d0bfa298298857717efa83c94412e8ccc0a77dd65d5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 21 Dec 2021 01:40:06 GMT
ADD file:6b67a0d4d176747cc8cefbd105facde82f1795467bf02eb45e8385c91cdc9c41 in / 
# Tue, 21 Dec 2021 01:40:09 GMT
CMD ["bash"]
# Mon, 27 Dec 2021 18:38:49 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Mon, 27 Dec 2021 18:38:53 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Mon, 27 Dec 2021 18:38:53 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Mon, 27 Dec 2021 18:39:18 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Mon, 27 Dec 2021 18:39:19 GMT
VOLUME [/spiped]
# Mon, 27 Dec 2021 18:39:19 GMT
WORKDIR /spiped
# Mon, 27 Dec 2021 18:39:19 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 27 Dec 2021 18:39:20 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 27 Dec 2021 18:39:20 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:9b9a100d632569e96aeb2d7b0bc45bc436609bb61335815f207994f3b557f0f7`  
		Last Modified: Tue, 21 Dec 2021 01:48:45 GMT  
		Size: 32.4 MB (32370850 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bacb6a90485f91c14c0461997a7afe3993a50f138c22f09ce39f21024c2062b8`  
		Last Modified: Mon, 27 Dec 2021 18:40:12 GMT  
		Size: 1.7 KB (1730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15dd5efb02f26ea602aaebe8f67a9f3a6947dad763a495fef3a9318f12fface9`  
		Last Modified: Mon, 27 Dec 2021 18:40:12 GMT  
		Size: 1.1 KB (1058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82f0e51dee85e4dcfc46978558a24091bc87a2559c3f2a36c3543893184a4c43`  
		Last Modified: Mon, 27 Dec 2021 18:40:14 GMT  
		Size: 7.9 MB (7891457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8925f3c59859f8e255f517eb2391360847148d17eb2715caa30753707600716`  
		Last Modified: Mon, 27 Dec 2021 18:40:12 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce7c6638e6c8f4a87a2847736b51b3093f589a601733574eb08c60e0c4707d43`  
		Last Modified: Mon, 27 Dec 2021 18:40:12 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; mips64le

```console
$ docker pull spiped@sha256:130c01d2a02859608af1ff69b512e606c6b0afab129f4f55f3b214e4439a961e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.3 MB (35327767 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8059d8a507f312d8d77dc186576b8b33cbc65306a9ff8fd918ca17b2b9163198`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 21 Dec 2021 02:09:07 GMT
ADD file:9e5931d5ed32a23b2e93bd8846258c647613637c581b6813bbc7d7e6b86bbdf5 in / 
# Tue, 21 Dec 2021 02:09:08 GMT
CMD ["bash"]
# Mon, 27 Dec 2021 18:07:30 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Mon, 27 Dec 2021 18:07:41 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Mon, 27 Dec 2021 18:07:41 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Mon, 27 Dec 2021 18:08:36 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Mon, 27 Dec 2021 18:08:36 GMT
VOLUME [/spiped]
# Mon, 27 Dec 2021 18:08:37 GMT
WORKDIR /spiped
# Mon, 27 Dec 2021 18:08:37 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 27 Dec 2021 18:08:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 27 Dec 2021 18:08:38 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:6a6edb95e2485a5b9b3c44b27b7ebad16384c0e08a3d61b7e48c65d7278763cf`  
		Last Modified: Tue, 21 Dec 2021 02:18:14 GMT  
		Size: 29.6 MB (29619177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffc41050c10fb28c363303084d216e4a84358c365e0c0c3ea780e76094ac5b62`  
		Last Modified: Mon, 27 Dec 2021 18:08:50 GMT  
		Size: 1.7 KB (1735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ccfed374e34e3e33bb1dac88ddd7d7bd1e7f5274368492e37c693a71768d15b`  
		Last Modified: Mon, 27 Dec 2021 18:08:50 GMT  
		Size: 1.0 KB (1028 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13d7546f5c1590f88787a1fc6a1c2e0d48c67af85dd4b7e8249ff573bee2daad`  
		Last Modified: Mon, 27 Dec 2021 18:08:55 GMT  
		Size: 5.7 MB (5705389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e85af9afd2d869bd928b4990f6fd908f635c5421d1dc8083fc5fd377b8bbd90`  
		Last Modified: Mon, 27 Dec 2021 18:08:50 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:870f16daf77f715fb9dc96eccb5b8d4af6d8b166fa70454d7fab605bd39d022b`  
		Last Modified: Mon, 27 Dec 2021 18:08:50 GMT  
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
$ docker pull spiped@sha256:695728df46d9899ea5caf49d16190d360575886d18bf0948f55bd1d82e81ec80
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
$ docker pull spiped@sha256:27655c03e38daa8aa4afed06a3d4c9f6127f971fe9ed16b98c8f48cc902ef314
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.3 MB (37327359 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:03b1412c46e8325a0589c93bac2d1990523e7e07b13698c2a9cb573fed4960bd`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 21 Dec 2021 01:22:43 GMT
ADD file:09675d11695f65c55efdc393ff0cd32f30194cd7d0fbef4631eebfed4414ac97 in / 
# Tue, 21 Dec 2021 01:22:43 GMT
CMD ["bash"]
# Mon, 27 Dec 2021 19:09:37 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Mon, 27 Dec 2021 19:09:40 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Mon, 27 Dec 2021 19:09:40 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Mon, 27 Dec 2021 19:10:01 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Mon, 27 Dec 2021 19:10:01 GMT
VOLUME [/spiped]
# Mon, 27 Dec 2021 19:10:01 GMT
WORKDIR /spiped
# Mon, 27 Dec 2021 19:10:02 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 27 Dec 2021 19:10:02 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 27 Dec 2021 19:10:02 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:a2abf6c4d29d43a4bf9fbb769f524d0fb36a2edab49819c1bf3e76f409f953ea`  
		Last Modified: Tue, 21 Dec 2021 01:27:48 GMT  
		Size: 31.4 MB (31357624 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d547106b69c042e6267b4030a20ff577bcfc9917ebf0a49d697c1d2819992416`  
		Last Modified: Mon, 27 Dec 2021 19:10:37 GMT  
		Size: 1.7 KB (1733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eda7224a790705cc7b53c6c57deb18f74ceeddf1a6a748cb1c59dd1d4f8b7c03`  
		Last Modified: Mon, 27 Dec 2021 19:10:37 GMT  
		Size: 1.1 KB (1055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7082f5785f33700aa63be5c0b314767d2b6039850a3dfcba2547dc823a464fff`  
		Last Modified: Mon, 27 Dec 2021 19:10:38 GMT  
		Size: 6.0 MB (5966475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8ceb17a2971caaf21db95998adb68b036ca18a5890dede0280840f93e2dabcb`  
		Last Modified: Mon, 27 Dec 2021 19:10:37 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7aed5299a2faa639446a4fc16f9364a4b444cae0a4c9855837063682ec7e4a88`  
		Last Modified: Mon, 27 Dec 2021 19:10:37 GMT  
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
$ docker pull spiped@sha256:126609a7885028d241e5a5879a81db1e409324ad4299d35fa13d8cb81db7741b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.3 MB (40265566 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e63888bbd27971f057151d0bfa298298857717efa83c94412e8ccc0a77dd65d5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 21 Dec 2021 01:40:06 GMT
ADD file:6b67a0d4d176747cc8cefbd105facde82f1795467bf02eb45e8385c91cdc9c41 in / 
# Tue, 21 Dec 2021 01:40:09 GMT
CMD ["bash"]
# Mon, 27 Dec 2021 18:38:49 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Mon, 27 Dec 2021 18:38:53 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Mon, 27 Dec 2021 18:38:53 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Mon, 27 Dec 2021 18:39:18 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Mon, 27 Dec 2021 18:39:19 GMT
VOLUME [/spiped]
# Mon, 27 Dec 2021 18:39:19 GMT
WORKDIR /spiped
# Mon, 27 Dec 2021 18:39:19 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 27 Dec 2021 18:39:20 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 27 Dec 2021 18:39:20 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:9b9a100d632569e96aeb2d7b0bc45bc436609bb61335815f207994f3b557f0f7`  
		Last Modified: Tue, 21 Dec 2021 01:48:45 GMT  
		Size: 32.4 MB (32370850 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bacb6a90485f91c14c0461997a7afe3993a50f138c22f09ce39f21024c2062b8`  
		Last Modified: Mon, 27 Dec 2021 18:40:12 GMT  
		Size: 1.7 KB (1730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15dd5efb02f26ea602aaebe8f67a9f3a6947dad763a495fef3a9318f12fface9`  
		Last Modified: Mon, 27 Dec 2021 18:40:12 GMT  
		Size: 1.1 KB (1058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82f0e51dee85e4dcfc46978558a24091bc87a2559c3f2a36c3543893184a4c43`  
		Last Modified: Mon, 27 Dec 2021 18:40:14 GMT  
		Size: 7.9 MB (7891457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8925f3c59859f8e255f517eb2391360847148d17eb2715caa30753707600716`  
		Last Modified: Mon, 27 Dec 2021 18:40:12 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce7c6638e6c8f4a87a2847736b51b3093f589a601733574eb08c60e0c4707d43`  
		Last Modified: Mon, 27 Dec 2021 18:40:12 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; mips64le

```console
$ docker pull spiped@sha256:130c01d2a02859608af1ff69b512e606c6b0afab129f4f55f3b214e4439a961e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.3 MB (35327767 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8059d8a507f312d8d77dc186576b8b33cbc65306a9ff8fd918ca17b2b9163198`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 21 Dec 2021 02:09:07 GMT
ADD file:9e5931d5ed32a23b2e93bd8846258c647613637c581b6813bbc7d7e6b86bbdf5 in / 
# Tue, 21 Dec 2021 02:09:08 GMT
CMD ["bash"]
# Mon, 27 Dec 2021 18:07:30 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Mon, 27 Dec 2021 18:07:41 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Mon, 27 Dec 2021 18:07:41 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Mon, 27 Dec 2021 18:08:36 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Mon, 27 Dec 2021 18:08:36 GMT
VOLUME [/spiped]
# Mon, 27 Dec 2021 18:08:37 GMT
WORKDIR /spiped
# Mon, 27 Dec 2021 18:08:37 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 27 Dec 2021 18:08:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 27 Dec 2021 18:08:38 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:6a6edb95e2485a5b9b3c44b27b7ebad16384c0e08a3d61b7e48c65d7278763cf`  
		Last Modified: Tue, 21 Dec 2021 02:18:14 GMT  
		Size: 29.6 MB (29619177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffc41050c10fb28c363303084d216e4a84358c365e0c0c3ea780e76094ac5b62`  
		Last Modified: Mon, 27 Dec 2021 18:08:50 GMT  
		Size: 1.7 KB (1735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ccfed374e34e3e33bb1dac88ddd7d7bd1e7f5274368492e37c693a71768d15b`  
		Last Modified: Mon, 27 Dec 2021 18:08:50 GMT  
		Size: 1.0 KB (1028 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13d7546f5c1590f88787a1fc6a1c2e0d48c67af85dd4b7e8249ff573bee2daad`  
		Last Modified: Mon, 27 Dec 2021 18:08:55 GMT  
		Size: 5.7 MB (5705389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e85af9afd2d869bd928b4990f6fd908f635c5421d1dc8083fc5fd377b8bbd90`  
		Last Modified: Mon, 27 Dec 2021 18:08:50 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:870f16daf77f715fb9dc96eccb5b8d4af6d8b166fa70454d7fab605bd39d022b`  
		Last Modified: Mon, 27 Dec 2021 18:08:50 GMT  
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
$ docker pull spiped@sha256:695728df46d9899ea5caf49d16190d360575886d18bf0948f55bd1d82e81ec80
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
$ docker pull spiped@sha256:27655c03e38daa8aa4afed06a3d4c9f6127f971fe9ed16b98c8f48cc902ef314
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.3 MB (37327359 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:03b1412c46e8325a0589c93bac2d1990523e7e07b13698c2a9cb573fed4960bd`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 21 Dec 2021 01:22:43 GMT
ADD file:09675d11695f65c55efdc393ff0cd32f30194cd7d0fbef4631eebfed4414ac97 in / 
# Tue, 21 Dec 2021 01:22:43 GMT
CMD ["bash"]
# Mon, 27 Dec 2021 19:09:37 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Mon, 27 Dec 2021 19:09:40 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Mon, 27 Dec 2021 19:09:40 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Mon, 27 Dec 2021 19:10:01 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Mon, 27 Dec 2021 19:10:01 GMT
VOLUME [/spiped]
# Mon, 27 Dec 2021 19:10:01 GMT
WORKDIR /spiped
# Mon, 27 Dec 2021 19:10:02 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 27 Dec 2021 19:10:02 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 27 Dec 2021 19:10:02 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:a2abf6c4d29d43a4bf9fbb769f524d0fb36a2edab49819c1bf3e76f409f953ea`  
		Last Modified: Tue, 21 Dec 2021 01:27:48 GMT  
		Size: 31.4 MB (31357624 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d547106b69c042e6267b4030a20ff577bcfc9917ebf0a49d697c1d2819992416`  
		Last Modified: Mon, 27 Dec 2021 19:10:37 GMT  
		Size: 1.7 KB (1733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eda7224a790705cc7b53c6c57deb18f74ceeddf1a6a748cb1c59dd1d4f8b7c03`  
		Last Modified: Mon, 27 Dec 2021 19:10:37 GMT  
		Size: 1.1 KB (1055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7082f5785f33700aa63be5c0b314767d2b6039850a3dfcba2547dc823a464fff`  
		Last Modified: Mon, 27 Dec 2021 19:10:38 GMT  
		Size: 6.0 MB (5966475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8ceb17a2971caaf21db95998adb68b036ca18a5890dede0280840f93e2dabcb`  
		Last Modified: Mon, 27 Dec 2021 19:10:37 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7aed5299a2faa639446a4fc16f9364a4b444cae0a4c9855837063682ec7e4a88`  
		Last Modified: Mon, 27 Dec 2021 19:10:37 GMT  
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
$ docker pull spiped@sha256:126609a7885028d241e5a5879a81db1e409324ad4299d35fa13d8cb81db7741b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.3 MB (40265566 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e63888bbd27971f057151d0bfa298298857717efa83c94412e8ccc0a77dd65d5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 21 Dec 2021 01:40:06 GMT
ADD file:6b67a0d4d176747cc8cefbd105facde82f1795467bf02eb45e8385c91cdc9c41 in / 
# Tue, 21 Dec 2021 01:40:09 GMT
CMD ["bash"]
# Mon, 27 Dec 2021 18:38:49 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Mon, 27 Dec 2021 18:38:53 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Mon, 27 Dec 2021 18:38:53 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Mon, 27 Dec 2021 18:39:18 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Mon, 27 Dec 2021 18:39:19 GMT
VOLUME [/spiped]
# Mon, 27 Dec 2021 18:39:19 GMT
WORKDIR /spiped
# Mon, 27 Dec 2021 18:39:19 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 27 Dec 2021 18:39:20 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 27 Dec 2021 18:39:20 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:9b9a100d632569e96aeb2d7b0bc45bc436609bb61335815f207994f3b557f0f7`  
		Last Modified: Tue, 21 Dec 2021 01:48:45 GMT  
		Size: 32.4 MB (32370850 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bacb6a90485f91c14c0461997a7afe3993a50f138c22f09ce39f21024c2062b8`  
		Last Modified: Mon, 27 Dec 2021 18:40:12 GMT  
		Size: 1.7 KB (1730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15dd5efb02f26ea602aaebe8f67a9f3a6947dad763a495fef3a9318f12fface9`  
		Last Modified: Mon, 27 Dec 2021 18:40:12 GMT  
		Size: 1.1 KB (1058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82f0e51dee85e4dcfc46978558a24091bc87a2559c3f2a36c3543893184a4c43`  
		Last Modified: Mon, 27 Dec 2021 18:40:14 GMT  
		Size: 7.9 MB (7891457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8925f3c59859f8e255f517eb2391360847148d17eb2715caa30753707600716`  
		Last Modified: Mon, 27 Dec 2021 18:40:12 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce7c6638e6c8f4a87a2847736b51b3093f589a601733574eb08c60e0c4707d43`  
		Last Modified: Mon, 27 Dec 2021 18:40:12 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.2` - linux; mips64le

```console
$ docker pull spiped@sha256:130c01d2a02859608af1ff69b512e606c6b0afab129f4f55f3b214e4439a961e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.3 MB (35327767 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8059d8a507f312d8d77dc186576b8b33cbc65306a9ff8fd918ca17b2b9163198`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 21 Dec 2021 02:09:07 GMT
ADD file:9e5931d5ed32a23b2e93bd8846258c647613637c581b6813bbc7d7e6b86bbdf5 in / 
# Tue, 21 Dec 2021 02:09:08 GMT
CMD ["bash"]
# Mon, 27 Dec 2021 18:07:30 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Mon, 27 Dec 2021 18:07:41 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Mon, 27 Dec 2021 18:07:41 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Mon, 27 Dec 2021 18:08:36 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Mon, 27 Dec 2021 18:08:36 GMT
VOLUME [/spiped]
# Mon, 27 Dec 2021 18:08:37 GMT
WORKDIR /spiped
# Mon, 27 Dec 2021 18:08:37 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 27 Dec 2021 18:08:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 27 Dec 2021 18:08:38 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:6a6edb95e2485a5b9b3c44b27b7ebad16384c0e08a3d61b7e48c65d7278763cf`  
		Last Modified: Tue, 21 Dec 2021 02:18:14 GMT  
		Size: 29.6 MB (29619177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffc41050c10fb28c363303084d216e4a84358c365e0c0c3ea780e76094ac5b62`  
		Last Modified: Mon, 27 Dec 2021 18:08:50 GMT  
		Size: 1.7 KB (1735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ccfed374e34e3e33bb1dac88ddd7d7bd1e7f5274368492e37c693a71768d15b`  
		Last Modified: Mon, 27 Dec 2021 18:08:50 GMT  
		Size: 1.0 KB (1028 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13d7546f5c1590f88787a1fc6a1c2e0d48c67af85dd4b7e8249ff573bee2daad`  
		Last Modified: Mon, 27 Dec 2021 18:08:55 GMT  
		Size: 5.7 MB (5705389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e85af9afd2d869bd928b4990f6fd908f635c5421d1dc8083fc5fd377b8bbd90`  
		Last Modified: Mon, 27 Dec 2021 18:08:50 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:870f16daf77f715fb9dc96eccb5b8d4af6d8b166fa70454d7fab605bd39d022b`  
		Last Modified: Mon, 27 Dec 2021 18:08:50 GMT  
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
$ docker pull spiped@sha256:695728df46d9899ea5caf49d16190d360575886d18bf0948f55bd1d82e81ec80
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
$ docker pull spiped@sha256:27655c03e38daa8aa4afed06a3d4c9f6127f971fe9ed16b98c8f48cc902ef314
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.3 MB (37327359 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:03b1412c46e8325a0589c93bac2d1990523e7e07b13698c2a9cb573fed4960bd`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 21 Dec 2021 01:22:43 GMT
ADD file:09675d11695f65c55efdc393ff0cd32f30194cd7d0fbef4631eebfed4414ac97 in / 
# Tue, 21 Dec 2021 01:22:43 GMT
CMD ["bash"]
# Mon, 27 Dec 2021 19:09:37 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Mon, 27 Dec 2021 19:09:40 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Mon, 27 Dec 2021 19:09:40 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Mon, 27 Dec 2021 19:10:01 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Mon, 27 Dec 2021 19:10:01 GMT
VOLUME [/spiped]
# Mon, 27 Dec 2021 19:10:01 GMT
WORKDIR /spiped
# Mon, 27 Dec 2021 19:10:02 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 27 Dec 2021 19:10:02 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 27 Dec 2021 19:10:02 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:a2abf6c4d29d43a4bf9fbb769f524d0fb36a2edab49819c1bf3e76f409f953ea`  
		Last Modified: Tue, 21 Dec 2021 01:27:48 GMT  
		Size: 31.4 MB (31357624 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d547106b69c042e6267b4030a20ff577bcfc9917ebf0a49d697c1d2819992416`  
		Last Modified: Mon, 27 Dec 2021 19:10:37 GMT  
		Size: 1.7 KB (1733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eda7224a790705cc7b53c6c57deb18f74ceeddf1a6a748cb1c59dd1d4f8b7c03`  
		Last Modified: Mon, 27 Dec 2021 19:10:37 GMT  
		Size: 1.1 KB (1055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7082f5785f33700aa63be5c0b314767d2b6039850a3dfcba2547dc823a464fff`  
		Last Modified: Mon, 27 Dec 2021 19:10:38 GMT  
		Size: 6.0 MB (5966475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8ceb17a2971caaf21db95998adb68b036ca18a5890dede0280840f93e2dabcb`  
		Last Modified: Mon, 27 Dec 2021 19:10:37 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7aed5299a2faa639446a4fc16f9364a4b444cae0a4c9855837063682ec7e4a88`  
		Last Modified: Mon, 27 Dec 2021 19:10:37 GMT  
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
$ docker pull spiped@sha256:126609a7885028d241e5a5879a81db1e409324ad4299d35fa13d8cb81db7741b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.3 MB (40265566 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e63888bbd27971f057151d0bfa298298857717efa83c94412e8ccc0a77dd65d5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 21 Dec 2021 01:40:06 GMT
ADD file:6b67a0d4d176747cc8cefbd105facde82f1795467bf02eb45e8385c91cdc9c41 in / 
# Tue, 21 Dec 2021 01:40:09 GMT
CMD ["bash"]
# Mon, 27 Dec 2021 18:38:49 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Mon, 27 Dec 2021 18:38:53 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Mon, 27 Dec 2021 18:38:53 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Mon, 27 Dec 2021 18:39:18 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Mon, 27 Dec 2021 18:39:19 GMT
VOLUME [/spiped]
# Mon, 27 Dec 2021 18:39:19 GMT
WORKDIR /spiped
# Mon, 27 Dec 2021 18:39:19 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 27 Dec 2021 18:39:20 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 27 Dec 2021 18:39:20 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:9b9a100d632569e96aeb2d7b0bc45bc436609bb61335815f207994f3b557f0f7`  
		Last Modified: Tue, 21 Dec 2021 01:48:45 GMT  
		Size: 32.4 MB (32370850 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bacb6a90485f91c14c0461997a7afe3993a50f138c22f09ce39f21024c2062b8`  
		Last Modified: Mon, 27 Dec 2021 18:40:12 GMT  
		Size: 1.7 KB (1730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15dd5efb02f26ea602aaebe8f67a9f3a6947dad763a495fef3a9318f12fface9`  
		Last Modified: Mon, 27 Dec 2021 18:40:12 GMT  
		Size: 1.1 KB (1058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82f0e51dee85e4dcfc46978558a24091bc87a2559c3f2a36c3543893184a4c43`  
		Last Modified: Mon, 27 Dec 2021 18:40:14 GMT  
		Size: 7.9 MB (7891457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8925f3c59859f8e255f517eb2391360847148d17eb2715caa30753707600716`  
		Last Modified: Mon, 27 Dec 2021 18:40:12 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce7c6638e6c8f4a87a2847736b51b3093f589a601733574eb08c60e0c4707d43`  
		Last Modified: Mon, 27 Dec 2021 18:40:12 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; mips64le

```console
$ docker pull spiped@sha256:130c01d2a02859608af1ff69b512e606c6b0afab129f4f55f3b214e4439a961e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.3 MB (35327767 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8059d8a507f312d8d77dc186576b8b33cbc65306a9ff8fd918ca17b2b9163198`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 21 Dec 2021 02:09:07 GMT
ADD file:9e5931d5ed32a23b2e93bd8846258c647613637c581b6813bbc7d7e6b86bbdf5 in / 
# Tue, 21 Dec 2021 02:09:08 GMT
CMD ["bash"]
# Mon, 27 Dec 2021 18:07:30 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Mon, 27 Dec 2021 18:07:41 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Mon, 27 Dec 2021 18:07:41 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Mon, 27 Dec 2021 18:08:36 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Mon, 27 Dec 2021 18:08:36 GMT
VOLUME [/spiped]
# Mon, 27 Dec 2021 18:08:37 GMT
WORKDIR /spiped
# Mon, 27 Dec 2021 18:08:37 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 27 Dec 2021 18:08:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 27 Dec 2021 18:08:38 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:6a6edb95e2485a5b9b3c44b27b7ebad16384c0e08a3d61b7e48c65d7278763cf`  
		Last Modified: Tue, 21 Dec 2021 02:18:14 GMT  
		Size: 29.6 MB (29619177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffc41050c10fb28c363303084d216e4a84358c365e0c0c3ea780e76094ac5b62`  
		Last Modified: Mon, 27 Dec 2021 18:08:50 GMT  
		Size: 1.7 KB (1735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ccfed374e34e3e33bb1dac88ddd7d7bd1e7f5274368492e37c693a71768d15b`  
		Last Modified: Mon, 27 Dec 2021 18:08:50 GMT  
		Size: 1.0 KB (1028 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13d7546f5c1590f88787a1fc6a1c2e0d48c67af85dd4b7e8249ff573bee2daad`  
		Last Modified: Mon, 27 Dec 2021 18:08:55 GMT  
		Size: 5.7 MB (5705389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e85af9afd2d869bd928b4990f6fd908f635c5421d1dc8083fc5fd377b8bbd90`  
		Last Modified: Mon, 27 Dec 2021 18:08:50 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:870f16daf77f715fb9dc96eccb5b8d4af6d8b166fa70454d7fab605bd39d022b`  
		Last Modified: Mon, 27 Dec 2021 18:08:50 GMT  
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
