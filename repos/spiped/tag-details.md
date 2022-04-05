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
$ docker pull spiped@sha256:1096e8cf1ee57825fa381a290095d3d42ebddf1e22f54edb53f96109d8466d0d
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
$ docker pull spiped@sha256:f236fca971a0526aa22ab4aa69709d302210d7e1f5bd42902bde2803ec0495bd
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.3 MB (37348627 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0ab54c336e542bbe2bacf29196b05876f18889ca6f79cd1c223af52a9bcf3241`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 29 Mar 2022 00:22:18 GMT
ADD file:966d3669b40f5fbaecee1ecbeb58debe19001076da5d94717080d55efbc25971 in / 
# Tue, 29 Mar 2022 00:22:19 GMT
CMD ["bash"]
# Tue, 29 Mar 2022 12:05:44 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 29 Mar 2022 12:05:47 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 29 Mar 2022 12:05:47 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 29 Mar 2022 12:06:06 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 29 Mar 2022 12:06:07 GMT
VOLUME [/spiped]
# Tue, 29 Mar 2022 12:06:07 GMT
WORKDIR /spiped
# Tue, 29 Mar 2022 12:06:07 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 29 Mar 2022 12:06:07 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 29 Mar 2022 12:06:07 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:c229119241af7b23b121052a1cae4c03e0a477a72ea6a7f463ad7623ff8f274b`  
		Last Modified: Tue, 29 Mar 2022 00:27:16 GMT  
		Size: 31.4 MB (31378457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fda024001dd8419f652d3fde717d37b32c648032cc3f92d00978db9268a65b97`  
		Last Modified: Tue, 29 Mar 2022 12:06:37 GMT  
		Size: 1.7 KB (1736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b55c823e9d54047194e3c5cef477607293ed02e6d1b77f8f6f834f50fe2e9d05`  
		Last Modified: Tue, 29 Mar 2022 12:06:37 GMT  
		Size: 1.1 KB (1052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55ae1339c87c4e759ff4a439ee8561a8481ea3131678ac5e2f58795506cb67fc`  
		Last Modified: Tue, 29 Mar 2022 12:06:38 GMT  
		Size: 6.0 MB (5966913 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eda9f112e9f42cfee9c6890693553b623bf2dd540c36f29ad14276acb22e044e`  
		Last Modified: Tue, 29 Mar 2022 12:06:37 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad6ba00100ccbdece1902154d0d0d33ee3d70d4e184a6524a97b6ab7e2e53192`  
		Last Modified: Tue, 29 Mar 2022 12:06:37 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; arm variant v5

```console
$ docker pull spiped@sha256:94736a8efc0da3dd2c4c38b0a356b70873aee616c541dbccdfa95068dc6c0cb6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.0 MB (33951476 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cfb46d52c65a3d3391adc84884f180419a0f9437774a897d2ba90ecff46cb1cb`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 29 Mar 2022 00:50:37 GMT
ADD file:6b9a30e6ef50a46e87cf9d7f5a491c7951fdb6dd6fab3c9d4a9c3c40f92b8db4 in / 
# Tue, 29 Mar 2022 00:50:38 GMT
CMD ["bash"]
# Wed, 30 Mar 2022 01:08:33 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 30 Mar 2022 01:08:43 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 30 Mar 2022 01:08:43 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 30 Mar 2022 01:09:31 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 30 Mar 2022 01:09:32 GMT
VOLUME [/spiped]
# Wed, 30 Mar 2022 01:09:32 GMT
WORKDIR /spiped
# Wed, 30 Mar 2022 01:09:33 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 30 Mar 2022 01:09:33 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 30 Mar 2022 01:09:34 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:9a41aba0a099ec129c20f41f6370b97daa4c3d4d3edc76ea1863bc5f76f9e5e5`  
		Last Modified: Tue, 29 Mar 2022 01:05:21 GMT  
		Size: 28.9 MB (28920513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afcd77f21f54e947717641dc9eb4a3c32a321dd3df6f615e082da0d916f9c6ca`  
		Last Modified: Wed, 30 Mar 2022 01:10:09 GMT  
		Size: 1.7 KB (1729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96e6a8e69828bdad8405be855d17ef3331b8093c3773b6a6ed726e8788cc3fe1`  
		Last Modified: Wed, 30 Mar 2022 01:10:09 GMT  
		Size: 1.1 KB (1053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e672a3f91acf51a5b4252fc7a5e23c4bd9539029d819fafe90af13149b18a97`  
		Last Modified: Wed, 30 Mar 2022 01:10:12 GMT  
		Size: 5.0 MB (5027710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11475c4da412af9a0208f5a0962e32a7bd674a732fc2cb1bd58a16deb9aac2e4`  
		Last Modified: Wed, 30 Mar 2022 01:10:09 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2adba7e3a404697c9d1e15fe08cfbb357d8dd16b877a299ca347781afd782675`  
		Last Modified: Wed, 30 Mar 2022 01:10:09 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; arm variant v7

```console
$ docker pull spiped@sha256:2dbc8de74b30a303a09ce36ac401dbbc2edd6a659c643579a43d0243250acd0b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.3 MB (31326537 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:04bbd512c51b4df932d3725ab91fe61a2eecb9b729392297a9634c096f37e9aa`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 29 Mar 2022 02:18:34 GMT
ADD file:e1835d1a0c70a0335757f211893e5d12ddf797e489e10434c0982bdf9b234f67 in / 
# Tue, 29 Mar 2022 02:18:36 GMT
CMD ["bash"]
# Wed, 30 Mar 2022 16:37:08 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 30 Mar 2022 16:37:15 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 30 Mar 2022 16:37:16 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 30 Mar 2022 16:38:00 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 30 Mar 2022 16:38:01 GMT
VOLUME [/spiped]
# Wed, 30 Mar 2022 16:38:01 GMT
WORKDIR /spiped
# Wed, 30 Mar 2022 16:38:02 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 30 Mar 2022 16:38:02 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 30 Mar 2022 16:38:03 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:f98812e1a494a683a5b3dea593dd2ef305f5f732193044c147f22e44b00164bc`  
		Last Modified: Tue, 29 Mar 2022 02:34:13 GMT  
		Size: 26.6 MB (26575370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b566a0eb6f50a4d3076e96e1230218651c8e3409f1e36b78720641ddcf02fe67`  
		Last Modified: Wed, 30 Mar 2022 16:39:28 GMT  
		Size: 1.7 KB (1730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3653f9517ce7a66aa5b26388c993e6803d010dd10becbc1141166b19d0575c20`  
		Last Modified: Wed, 30 Mar 2022 16:39:28 GMT  
		Size: 1.1 KB (1055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bef73e1c106acd2821aea52e999a0ab3dc8a102d38cf18f931ff036fc5cdde29`  
		Last Modified: Wed, 30 Mar 2022 16:39:32 GMT  
		Size: 4.7 MB (4747910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1eb71618098b05bae1eef477c77b1abb4846fb9cb147e36318ec26d12542a9db`  
		Last Modified: Wed, 30 Mar 2022 16:39:28 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4742b0162d23f2f2a3f504f4d0eded391b6c812f26030eca3f9137563d7d44fc`  
		Last Modified: Wed, 30 Mar 2022 16:39:28 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:489251bdbc8f5a1d43cb461dba8917af4fb58142240f15e7d2c7c31f7d859b2b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.3 MB (35337814 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bead5c7928697f7d3aded01a859186f595bedcb48737aebb29d40d92c78230e5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 29 Mar 2022 00:43:17 GMT
ADD file:e95289cd39de0f389d09cda9edf8476d5da371bc68d76e820c5e1c310dc54baf in / 
# Tue, 29 Mar 2022 00:43:17 GMT
CMD ["bash"]
# Wed, 30 Mar 2022 01:01:29 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 30 Mar 2022 01:01:33 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 30 Mar 2022 01:01:34 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 30 Mar 2022 01:01:58 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 30 Mar 2022 01:01:58 GMT
VOLUME [/spiped]
# Wed, 30 Mar 2022 01:01:59 GMT
WORKDIR /spiped
# Wed, 30 Mar 2022 01:02:01 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 30 Mar 2022 01:02:01 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 30 Mar 2022 01:02:02 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:2203022c5aa978ec114a15a7cdc2c323c65922d3b0a8eab11d50811bb9ae1cfb`  
		Last Modified: Tue, 29 Mar 2022 00:50:04 GMT  
		Size: 30.1 MB (30064311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c1c5ff6bd12cad4539ef42aba72b9e2a79fd5e03cf703d178e9179cf3ca28d3`  
		Last Modified: Wed, 30 Mar 2022 01:03:05 GMT  
		Size: 1.6 KB (1619 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d32807b7cfbcaf6c5dda896ed26a7d5b103161f8237a6f762874f9d2e713509`  
		Last Modified: Wed, 30 Mar 2022 01:03:04 GMT  
		Size: 923.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbc810f776215aefbbbcac36475250c8768eea0d0fdb5cdeceb3a2ed84c8dbb8`  
		Last Modified: Wed, 30 Mar 2022 01:03:06 GMT  
		Size: 5.3 MB (5270525 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d1419d96420314f5d538869ef6bf4d3e349c952c254f754fba1e39a0ba1a36c`  
		Last Modified: Wed, 30 Mar 2022 01:03:04 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:533163ce32b9d79dc658ade7a26d7f71cece5b9bf114cc7b7dc3596ba66609ba`  
		Last Modified: Wed, 30 Mar 2022 01:03:04 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; 386

```console
$ docker pull spiped@sha256:7bf4cc6d7160264b61ad5339a1b254c94c216125bf624adbb4a44b1a484a71b1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.3 MB (40283723 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e193db912bc32b089a793405a8541f1cb6d938b1dad5dc81b749bdb791619efa`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 29 Mar 2022 00:42:01 GMT
ADD file:d093057c080a13cc4370d0e786857751004b8cd3c93368742512abbee4f1de83 in / 
# Tue, 29 Mar 2022 00:42:01 GMT
CMD ["bash"]
# Tue, 29 Mar 2022 10:43:59 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 29 Mar 2022 10:44:03 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 29 Mar 2022 10:44:04 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 29 Mar 2022 10:44:24 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 29 Mar 2022 10:44:25 GMT
VOLUME [/spiped]
# Tue, 29 Mar 2022 10:44:26 GMT
WORKDIR /spiped
# Tue, 29 Mar 2022 10:44:28 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 29 Mar 2022 10:44:28 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 29 Mar 2022 10:44:29 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:fec59da75229f638ca2878278d3859a1a8b73a20d5c0c043354eb37129ebb8bf`  
		Last Modified: Tue, 29 Mar 2022 00:49:10 GMT  
		Size: 32.4 MB (32389518 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:559c323dcf632c3e6c78229ea96b201cd5c6a73598a208ba2fd88a55a2e53f6a`  
		Last Modified: Tue, 29 Mar 2022 10:45:19 GMT  
		Size: 1.6 KB (1611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7b0c52bcbc80dacdfd452f5135ca2e640ab57050b38fbf5890ca41339ce8cbf`  
		Last Modified: Tue, 29 Mar 2022 10:45:19 GMT  
		Size: 924.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0e273d1baff760d787e4bf5a3e20801cf5a8e2625eada853a4d7cdd86c1e25f`  
		Last Modified: Tue, 29 Mar 2022 10:45:20 GMT  
		Size: 7.9 MB (7891233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd7f99497ff10c89ef5d937c4f127f94bcc0391017c3fa45d587bab079706dea`  
		Last Modified: Tue, 29 Mar 2022 10:45:19 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61bb3d200b36c323a0edaaa6ceb5990790f17562ef9d5e5c63d7fab6d1978d51`  
		Last Modified: Tue, 29 Mar 2022 10:45:19 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; mips64le

```console
$ docker pull spiped@sha256:616f8531e23b941b90c8d1293b641771b4c758475fff50f5f6f50bdceae91f2c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.3 MB (35349463 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e57ad4c68f94212319101e900c6737ad74d321485f03cf0cf7522b7259c35ac0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 29 Mar 2022 07:42:27 GMT
ADD file:32aa9fd7ee5c64e4bd49459e801e3e5dc50138590bbfca671e336a197aa7fa92 in / 
# Tue, 29 Mar 2022 07:42:31 GMT
CMD ["bash"]
# Wed, 30 Mar 2022 05:36:13 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 30 Mar 2022 05:36:28 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 30 Mar 2022 05:36:31 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 30 Mar 2022 05:38:04 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 30 Mar 2022 05:38:06 GMT
VOLUME [/spiped]
# Wed, 30 Mar 2022 05:38:09 GMT
WORKDIR /spiped
# Wed, 30 Mar 2022 05:38:12 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 30 Mar 2022 05:38:14 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 30 Mar 2022 05:38:17 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:5c2a8045f9de06328ab3d0ff505d990892219b7faee393bc9ac342347fc83d04`  
		Last Modified: Tue, 29 Mar 2022 07:52:59 GMT  
		Size: 29.6 MB (29641474 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28d11336cbfa9f2c1e6c22eef2096c37397f6a0058407687dc007bf7384a3e79`  
		Last Modified: Wed, 30 Mar 2022 05:38:29 GMT  
		Size: 1.6 KB (1629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd53cadc47175f65d5df3546949d7f0a90aec5d75b5fe538a9a9b4fe2ebeefd2`  
		Last Modified: Wed, 30 Mar 2022 05:38:29 GMT  
		Size: 924.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcdf8956bed67848aaf6e2f1456d79a9db2efc0f6986df8eb00feb2d30de9389`  
		Last Modified: Wed, 30 Mar 2022 05:38:34 GMT  
		Size: 5.7 MB (5704999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6a3ca7ecd16ef5159abf00ec43e34fbe1b528c2416e3b0eb94806b1d5445e5d`  
		Last Modified: Wed, 30 Mar 2022 05:38:29 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:109d3b9867a03e8499cbf83271d977a1bbf8550acb992fce7348de6047db039f`  
		Last Modified: Wed, 30 Mar 2022 05:38:29 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; ppc64le

```console
$ docker pull spiped@sha256:20cc9df235f7239597ba6e9f0da45b8a2476c6020795502aa68f0b7275799a6d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.3 MB (41284580 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a9d0a0f307401e56e3c154076006ae5b0585b5124c0ad643d5fc5305effea55c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 29 Mar 2022 00:22:08 GMT
ADD file:e7ae113c10f322a9cffc46b62ba12820e270caaadaee3c5b907c801a37e1632c in / 
# Tue, 29 Mar 2022 00:22:11 GMT
CMD ["bash"]
# Wed, 30 Mar 2022 05:21:11 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 30 Mar 2022 05:21:26 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 30 Mar 2022 05:21:30 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 30 Mar 2022 05:24:47 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 30 Mar 2022 05:24:55 GMT
VOLUME [/spiped]
# Wed, 30 Mar 2022 05:25:01 GMT
WORKDIR /spiped
# Wed, 30 Mar 2022 05:25:04 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 30 Mar 2022 05:25:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 30 Mar 2022 05:25:15 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:ecc74bb8af5a048e1123af0e17d88ef3da1d10951ada79e8e1cc9c0a694245d3`  
		Last Modified: Tue, 29 Mar 2022 00:32:57 GMT  
		Size: 35.3 MB (35282506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89e50c6a3f6bfe8c939d3f4cf697d6972444715b3e29bbe8ba3a8503b2d47744`  
		Last Modified: Wed, 30 Mar 2022 05:27:29 GMT  
		Size: 1.7 KB (1748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06d13b3a37c65e9f1e8f7d06ea8947895095e24e8766405225cfb8a7a68897fd`  
		Last Modified: Wed, 30 Mar 2022 05:27:29 GMT  
		Size: 1.1 KB (1056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bf7cfaec929baf5dd2ec1c286ff49084391ed126f695c76cc847467adb4b808`  
		Last Modified: Wed, 30 Mar 2022 05:27:31 GMT  
		Size: 6.0 MB (5998799 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0d18fb763428d4908c4dccb28dd79a1ef28deee5b1869dd026f99019b274d04`  
		Last Modified: Wed, 30 Mar 2022 05:27:29 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17b9492405cf9ecc040958db5b6363eb0b2a3fb3a3113526b3c94ebbe352ec9c`  
		Last Modified: Wed, 30 Mar 2022 05:27:29 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; s390x

```console
$ docker pull spiped@sha256:bc909d5eeee60c7823173755c87467307f944145474e127199afc7d15643b99c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.8 MB (34845094 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2c0bcec57634c726f934b24b28bf162da99aacbf72dd089108346ddd627e4284`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 29 Mar 2022 00:51:57 GMT
ADD file:39c5e0d7a686abd19448ab3e6237d50955ae2187fc2b64289a08c2549352b8f1 in / 
# Tue, 29 Mar 2022 00:51:58 GMT
CMD ["bash"]
# Wed, 30 Mar 2022 02:17:13 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 30 Mar 2022 02:17:16 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 30 Mar 2022 02:17:16 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 30 Mar 2022 02:17:28 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 30 Mar 2022 02:17:29 GMT
VOLUME [/spiped]
# Wed, 30 Mar 2022 02:17:29 GMT
WORKDIR /spiped
# Wed, 30 Mar 2022 02:17:29 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 30 Mar 2022 02:17:29 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 30 Mar 2022 02:17:29 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:ffb22bcde95509bb75f6dd2d69f3fdb5c7471727e4d720b31d92cd297582865c`  
		Last Modified: Tue, 29 Mar 2022 01:04:43 GMT  
		Size: 29.7 MB (29655426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9488a45de61a7c26b2a863c250a52839737d409c8bac0426e2161131489985d3`  
		Last Modified: Wed, 30 Mar 2022 02:18:10 GMT  
		Size: 1.7 KB (1735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abedbd8409757c2b32910d965e11e1ba2d29a16105361932d6d8bd82b611d64d`  
		Last Modified: Wed, 30 Mar 2022 02:18:10 GMT  
		Size: 1.1 KB (1053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0eb1d8925fb8e4d0edc85c85b1f0d782db61bdf479a93bc6a0ccd97410d5a81`  
		Last Modified: Wed, 30 Mar 2022 02:18:10 GMT  
		Size: 5.2 MB (5186412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7987418a0dc4bd8525c7ad87f10f5f7ca2fdd8060ac0807f66714351df3d27cc`  
		Last Modified: Wed, 30 Mar 2022 02:18:10 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3647b49ea4318215c86c777031179b0cacb01790a04d0208a9d80a7962bb5768`  
		Last Modified: Wed, 30 Mar 2022 02:18:10 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:1-alpine`

```console
$ docker pull spiped@sha256:df67424ae1b5f50fe62e3c8f7584a176cef62ba9d479ccd376f70587ae42ca61
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
$ docker pull spiped@sha256:b1000f43786f16a20a805fa353f6e29da279735ce16fc397001fde0e351cadab
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (3038963 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:319549bf17a1c296f365e261889f2573a629fda0ca36fa2dac3efc79c233dc4d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 05 Apr 2022 00:19:59 GMT
ADD file:5d673d25da3a14ce1f6cf66e4c7fd4f4b85a3759a9d93efb3fd9ff852b5b56e4 in / 
# Tue, 05 Apr 2022 00:19:59 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 09:41:12 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Tue, 05 Apr 2022 09:41:13 GMT
RUN apk add --no-cache libssl1.1
# Tue, 05 Apr 2022 09:41:13 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 05 Apr 2022 09:41:22 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Tue, 05 Apr 2022 09:41:22 GMT
VOLUME [/spiped]
# Tue, 05 Apr 2022 09:41:23 GMT
WORKDIR /spiped
# Tue, 05 Apr 2022 09:41:23 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 05 Apr 2022 09:41:23 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 05 Apr 2022 09:41:23 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:df9b9388f04ad6279a7410b85cedfdcb2208c0a003da7ab5613af71079148139`  
		Last Modified: Mon, 04 Apr 2022 19:10:16 GMT  
		Size: 2.8 MB (2814559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:735044c06e8b73c2bb88467804d54b359bfc8226cf975772cc666adc9f029f5c`  
		Last Modified: Tue, 05 Apr 2022 09:41:38 GMT  
		Size: 1.3 KB (1271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd8b16fcaec70a3de42b4e850be4a851eaffa96a04fb49668b0d55b15bdf9675`  
		Last Modified: Tue, 05 Apr 2022 09:41:38 GMT  
		Size: 7.8 KB (7783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79236b25532d68c328b81af71a0f8c4eca102b7030a98d650ffc9a7e35d113be`  
		Last Modified: Tue, 05 Apr 2022 09:41:38 GMT  
		Size: 214.9 KB (214880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f429bef29fed68fb012179a10893c62fd5167934a7d62e7d3db15361601d47e9`  
		Last Modified: Tue, 05 Apr 2022 09:41:38 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1703108ce26f514d42179cf03051a6082b57e184d89f7bab08377819025c74d9`  
		Last Modified: Tue, 05 Apr 2022 09:41:38 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; arm variant v6

```console
$ docker pull spiped@sha256:ae66fb10272b529530524084a214a11e65777dff6517d5a90d71357e60416246
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 MB (2830615 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aae9a0570520cf722d24d3a84685d936a04a06d1b8e35de44be52daca29219ea`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 29 Mar 2022 00:49:32 GMT
ADD file:44acf536d487bec7f7bf16561f4ec90e60d4447b3cbabfeca66953c4491aabeb in / 
# Tue, 29 Mar 2022 00:49:33 GMT
CMD ["/bin/sh"]
# Tue, 29 Mar 2022 08:24:39 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Tue, 29 Mar 2022 08:24:41 GMT
RUN apk add --no-cache libssl1.1
# Tue, 29 Mar 2022 08:24:41 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 29 Mar 2022 08:25:01 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Tue, 29 Mar 2022 08:25:01 GMT
VOLUME [/spiped]
# Tue, 29 Mar 2022 08:25:02 GMT
WORKDIR /spiped
# Tue, 29 Mar 2022 08:25:03 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 29 Mar 2022 08:25:03 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 29 Mar 2022 08:25:04 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:84f033dabe5013c0dfae4263abd951011719d0a15adc3c7312c5be994deff030`  
		Last Modified: Tue, 29 Mar 2022 00:51:25 GMT  
		Size: 2.6 MB (2621943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdc4ea1012b3262fa7706463586c4d41a0cf0a329238cbe52ea6d03bfbc07fae`  
		Last Modified: Tue, 29 Mar 2022 08:25:35 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5659ae5d68adc8e4012f07c665ea352c4068ee821e83350f8bc165b6aea5583`  
		Last Modified: Tue, 29 Mar 2022 08:25:35 GMT  
		Size: 7.8 KB (7774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bf4925cebf49f63997a8c7389e423c3623dc4cd2e6c701e4282c664293e789b`  
		Last Modified: Tue, 29 Mar 2022 08:25:35 GMT  
		Size: 199.2 KB (199158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6eac1b140b33266f585c96310939c5cdbac7bde1fcbc0bd4e8cde9f9f0dd5171`  
		Last Modified: Tue, 29 Mar 2022 08:25:35 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11b13e602bdbc874391ee6aee0f8abffe1e74ee57061d9e1faed46aa76ad44a0`  
		Last Modified: Tue, 29 Mar 2022 08:25:35 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; arm variant v7

```console
$ docker pull spiped@sha256:1533669bdce5be15027cb96650fabea206274558c0195f437de5245079d89f0f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 MB (2626515 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:52a32db31d94e7ea2f1af7b835d809d1b42c16deff1071fe4b3f2e720bc3688c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 29 Mar 2022 02:13:28 GMT
ADD file:8c959b80e3661beea7b3468017b88897d981bf52ed43c074e7c87ecb753e9059 in / 
# Tue, 29 Mar 2022 02:13:28 GMT
CMD ["/bin/sh"]
# Wed, 30 Mar 2022 16:38:17 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Wed, 30 Mar 2022 16:38:19 GMT
RUN apk add --no-cache libssl1.1
# Wed, 30 Mar 2022 16:38:20 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 30 Mar 2022 16:38:38 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Wed, 30 Mar 2022 16:38:38 GMT
VOLUME [/spiped]
# Wed, 30 Mar 2022 16:38:39 GMT
WORKDIR /spiped
# Wed, 30 Mar 2022 16:38:40 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 30 Mar 2022 16:38:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 30 Mar 2022 16:38:40 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:22b1e5a07a97d7af6fdc335e3b3a975b73908fa19b084289c408a00814da0398`  
		Last Modified: Tue, 29 Mar 2022 02:15:28 GMT  
		Size: 2.4 MB (2424303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1b864dcb6ac61a275d83b41f5e533000faf52fae810b4fc0513796337285828`  
		Last Modified: Wed, 30 Mar 2022 16:39:51 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3aed778a3d8f2984cc57d3cbd49d0974e4d48f31a548da40051a676285fcb98`  
		Last Modified: Wed, 30 Mar 2022 16:39:51 GMT  
		Size: 7.8 KB (7781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23bc58fbe93b76dec15870d5507d4377afa5e3cd4e9ddd68e1117ed5fb9b1953`  
		Last Modified: Wed, 30 Mar 2022 16:39:52 GMT  
		Size: 192.7 KB (192691 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1f1a66e69919430ccc221d6a8b42a90a4ebdee7a41b426b4cabbd472c3d62a3`  
		Last Modified: Wed, 30 Mar 2022 16:39:51 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6342a8067391971e5056968d5d26841d53aeaab30109c42bb6c53a227f694cab`  
		Last Modified: Wed, 30 Mar 2022 16:39:51 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:c0d28956af21c9ad7d0e3d4cf972b301ea28efa0c8755d1ee62841b09754b0ab
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 MB (2933013 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a11675ed63f0f0f4c5e2d5175c06bade440268d204f7a4b104eba50db3f998da`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 29 Mar 2022 00:40:05 GMT
ADD file:24e8b04304ef91bbf949674909ccaf2c66e3dcd096c3c307a0510569eadf576f in / 
# Tue, 29 Mar 2022 00:40:05 GMT
CMD ["/bin/sh"]
# Wed, 30 Mar 2022 01:02:13 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Wed, 30 Mar 2022 01:02:15 GMT
RUN apk add --no-cache libssl1.1
# Wed, 30 Mar 2022 01:02:16 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 30 Mar 2022 01:02:34 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Wed, 30 Mar 2022 01:02:35 GMT
VOLUME [/spiped]
# Wed, 30 Mar 2022 01:02:36 GMT
WORKDIR /spiped
# Wed, 30 Mar 2022 01:02:38 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 30 Mar 2022 01:02:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 30 Mar 2022 01:02:39 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:80fa7f07ec7b717ec5f8e2717b91e3d659e129052ec3def2570a5674322688d9`  
		Last Modified: Tue, 29 Mar 2022 00:41:08 GMT  
		Size: 2.7 MB (2716347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ef7ee2c7f3dc7bcaf9752a844248d8127145ffd675ae5de72b4be177fc37cd5`  
		Last Modified: Wed, 30 Mar 2022 01:03:39 GMT  
		Size: 1.2 KB (1240 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47c53830f06d1a108ac255dbff68c71fabc58723d0a42943fec7681cbebe653a`  
		Last Modified: Wed, 30 Mar 2022 01:03:38 GMT  
		Size: 7.8 KB (7751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e1f94f19caf7b781c37e261530b5861447ecd5ab33d55ad4d2f12a932db1cf8`  
		Last Modified: Wed, 30 Mar 2022 01:03:39 GMT  
		Size: 207.2 KB (207237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b259955a7b787ff533a05f42050e5172ba829db902cac41506236e30a45be04e`  
		Last Modified: Wed, 30 Mar 2022 01:03:38 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29db0547b8fb18568f5c6616a8622211952741a2a93da0e86cb506b1ee4c941c`  
		Last Modified: Wed, 30 Mar 2022 01:03:39 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; 386

```console
$ docker pull spiped@sha256:dcbb93128deb3206337ac10573e41e27b4a95816cd3f931412c655201fef2396
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.1 MB (3053817 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fdb9526919356b65e45d7bc9a9bd2aaddd7da8a1e62f023b9511a320a431df64`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Mon, 04 Apr 2022 23:38:25 GMT
ADD file:7d51a0f8691eb78c9062fd31984423a93d276a67b4ed5d1a706e1c2cd9fea23a in / 
# Mon, 04 Apr 2022 23:38:25 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 06:51:23 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Tue, 05 Apr 2022 06:51:24 GMT
RUN apk add --no-cache libssl1.1
# Tue, 05 Apr 2022 06:51:24 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 05 Apr 2022 06:51:34 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Tue, 05 Apr 2022 06:51:35 GMT
VOLUME [/spiped]
# Tue, 05 Apr 2022 06:51:36 GMT
WORKDIR /spiped
# Tue, 05 Apr 2022 06:51:38 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 05 Apr 2022 06:51:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 05 Apr 2022 06:51:39 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:73b28a5955ec7fb46f2cf0434e4901a889f7dda3f8c9ec496300feb256c7eda8`  
		Last Modified: Mon, 04 Apr 2022 19:10:03 GMT  
		Size: 2.8 MB (2818974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5043c44edf55100d2df153f657912b53abf987ef0c6286b113dcef298998f359`  
		Last Modified: Tue, 05 Apr 2022 06:52:09 GMT  
		Size: 1.2 KB (1240 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfc9d36e654ea336dd74dc00574768a6502edd5ef5cd785b695e516f6254be55`  
		Last Modified: Tue, 05 Apr 2022 06:52:08 GMT  
		Size: 7.8 KB (7750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0401735f1a5cdc5a0248a778049579b8858a6f7cc0fc6fdcdaea211930d4a386`  
		Last Modified: Tue, 05 Apr 2022 06:52:08 GMT  
		Size: 225.4 KB (225416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5a85e3f263e110e3fa50aada2a3ca6314a5a6e67e8f211881a826585a5db409`  
		Last Modified: Tue, 05 Apr 2022 06:52:08 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a0f113efbe13d3511b57cb0428e99f2725a51cb3980e75b1f1be3fc0d715b19`  
		Last Modified: Tue, 05 Apr 2022 06:52:08 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; ppc64le

```console
$ docker pull spiped@sha256:d27c5eb0ad348fe2a50b65e808e4b825f0f479572187d81757b9a82ce2ad9e50
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (3033662 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1853309ab0785a26d0b48053b424c5b8c4ffd6367504032c68e3377b9fc92eba`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 29 Mar 2022 00:16:52 GMT
ADD file:9e7b65a431d59070abaadae56d9c3fc59c899af881939e4353b1f524b2bd5185 in / 
# Tue, 29 Mar 2022 00:16:55 GMT
CMD ["/bin/sh"]
# Wed, 30 Mar 2022 05:25:40 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Wed, 30 Mar 2022 05:25:50 GMT
RUN apk add --no-cache libssl1.1
# Wed, 30 Mar 2022 05:25:53 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 30 Mar 2022 05:26:20 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Wed, 30 Mar 2022 05:26:24 GMT
VOLUME [/spiped]
# Wed, 30 Mar 2022 05:26:28 GMT
WORKDIR /spiped
# Wed, 30 Mar 2022 05:26:35 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 30 Mar 2022 05:26:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 30 Mar 2022 05:26:46 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:1c611bca4fa49cac5bc1e3826ad53fee85ed659d24bffcccd86c3f04be07339a`  
		Last Modified: Tue, 29 Mar 2022 00:18:26 GMT  
		Size: 2.8 MB (2811009 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b61e9d70cfabe50a7554945008b067920fffa673936b1b8c50f29cdbc07fad93`  
		Last Modified: Wed, 30 Mar 2022 05:27:51 GMT  
		Size: 1.3 KB (1263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd9a458bb0005f54d005e938aa01a6aeeb1d7c48486de6811d1c16a9846b1239`  
		Last Modified: Wed, 30 Mar 2022 05:27:51 GMT  
		Size: 7.8 KB (7774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be8c858ba1f6886855b0312ec6b3618c916bea4577c858d028e6709d67f05939`  
		Last Modified: Wed, 30 Mar 2022 05:27:51 GMT  
		Size: 213.1 KB (213149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1d4e4cb20d1bd858c134eae12aac2cab24001fbae386ee7f84b1e8dc6c6ef76`  
		Last Modified: Wed, 30 Mar 2022 05:27:51 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20cb5033835d271b66d87c37a113ae41ee09c6b1c5b462196462cb06687e3352`  
		Last Modified: Wed, 30 Mar 2022 05:27:51 GMT  
		Size: 338.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; s390x

```console
$ docker pull spiped@sha256:851d4d1e8b82de6d455e9a562bd6b75539fe737213c9f3cf01ce7b44e11abeb4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 MB (2811594 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e240f56e6000d053b4d3e20632b54b88daaa8dad76ecda720ce9f76c82bfe394`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Mon, 04 Apr 2022 23:41:39 GMT
ADD file:f22e4b2be87d3c59c8c609acf79015938dc1fba0b26d7c1b59bd0fc36d63a906 in / 
# Mon, 04 Apr 2022 23:41:39 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 06:09:44 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Tue, 05 Apr 2022 06:09:45 GMT
RUN apk add --no-cache libssl1.1
# Tue, 05 Apr 2022 06:09:45 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 05 Apr 2022 06:09:50 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Tue, 05 Apr 2022 06:09:50 GMT
VOLUME [/spiped]
# Tue, 05 Apr 2022 06:09:51 GMT
WORKDIR /spiped
# Tue, 05 Apr 2022 06:09:51 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 05 Apr 2022 06:09:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 05 Apr 2022 06:09:51 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:a27b630f446c3da376a30cf610e4bfa6847f8b87c83702c29e72b986f4e52d28`  
		Last Modified: Mon, 04 Apr 2022 23:42:37 GMT  
		Size: 2.6 MB (2600375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ffc8ec477cbe2d575e99a9232e9328db8cc40109dbe067d93c2033302576850`  
		Last Modified: Tue, 05 Apr 2022 06:10:22 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ee008c7ec71319091cda7b7cbf1063414ee758f739581409a2e7089e90882c9`  
		Last Modified: Tue, 05 Apr 2022 06:10:21 GMT  
		Size: 7.8 KB (7788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3edcb5212f084eabfd1bad6e332d8b53bd7756099c4da3e410ee23f869a701b`  
		Last Modified: Tue, 05 Apr 2022 06:10:21 GMT  
		Size: 201.7 KB (201693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd099e1efb05ce5fa06c5e18ba7d057b5df318c462022f1ac443f45e86fdc809`  
		Last Modified: Tue, 05 Apr 2022 06:10:21 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afbab95e29c022d6828d869e5e4442b139373571c747f8fc6470b8bd257337a4`  
		Last Modified: Tue, 05 Apr 2022 06:10:21 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:1.6`

```console
$ docker pull spiped@sha256:1096e8cf1ee57825fa381a290095d3d42ebddf1e22f54edb53f96109d8466d0d
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
$ docker pull spiped@sha256:f236fca971a0526aa22ab4aa69709d302210d7e1f5bd42902bde2803ec0495bd
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.3 MB (37348627 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0ab54c336e542bbe2bacf29196b05876f18889ca6f79cd1c223af52a9bcf3241`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 29 Mar 2022 00:22:18 GMT
ADD file:966d3669b40f5fbaecee1ecbeb58debe19001076da5d94717080d55efbc25971 in / 
# Tue, 29 Mar 2022 00:22:19 GMT
CMD ["bash"]
# Tue, 29 Mar 2022 12:05:44 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 29 Mar 2022 12:05:47 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 29 Mar 2022 12:05:47 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 29 Mar 2022 12:06:06 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 29 Mar 2022 12:06:07 GMT
VOLUME [/spiped]
# Tue, 29 Mar 2022 12:06:07 GMT
WORKDIR /spiped
# Tue, 29 Mar 2022 12:06:07 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 29 Mar 2022 12:06:07 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 29 Mar 2022 12:06:07 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:c229119241af7b23b121052a1cae4c03e0a477a72ea6a7f463ad7623ff8f274b`  
		Last Modified: Tue, 29 Mar 2022 00:27:16 GMT  
		Size: 31.4 MB (31378457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fda024001dd8419f652d3fde717d37b32c648032cc3f92d00978db9268a65b97`  
		Last Modified: Tue, 29 Mar 2022 12:06:37 GMT  
		Size: 1.7 KB (1736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b55c823e9d54047194e3c5cef477607293ed02e6d1b77f8f6f834f50fe2e9d05`  
		Last Modified: Tue, 29 Mar 2022 12:06:37 GMT  
		Size: 1.1 KB (1052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55ae1339c87c4e759ff4a439ee8561a8481ea3131678ac5e2f58795506cb67fc`  
		Last Modified: Tue, 29 Mar 2022 12:06:38 GMT  
		Size: 6.0 MB (5966913 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eda9f112e9f42cfee9c6890693553b623bf2dd540c36f29ad14276acb22e044e`  
		Last Modified: Tue, 29 Mar 2022 12:06:37 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad6ba00100ccbdece1902154d0d0d33ee3d70d4e184a6524a97b6ab7e2e53192`  
		Last Modified: Tue, 29 Mar 2022 12:06:37 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; arm variant v5

```console
$ docker pull spiped@sha256:94736a8efc0da3dd2c4c38b0a356b70873aee616c541dbccdfa95068dc6c0cb6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.0 MB (33951476 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cfb46d52c65a3d3391adc84884f180419a0f9437774a897d2ba90ecff46cb1cb`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 29 Mar 2022 00:50:37 GMT
ADD file:6b9a30e6ef50a46e87cf9d7f5a491c7951fdb6dd6fab3c9d4a9c3c40f92b8db4 in / 
# Tue, 29 Mar 2022 00:50:38 GMT
CMD ["bash"]
# Wed, 30 Mar 2022 01:08:33 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 30 Mar 2022 01:08:43 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 30 Mar 2022 01:08:43 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 30 Mar 2022 01:09:31 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 30 Mar 2022 01:09:32 GMT
VOLUME [/spiped]
# Wed, 30 Mar 2022 01:09:32 GMT
WORKDIR /spiped
# Wed, 30 Mar 2022 01:09:33 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 30 Mar 2022 01:09:33 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 30 Mar 2022 01:09:34 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:9a41aba0a099ec129c20f41f6370b97daa4c3d4d3edc76ea1863bc5f76f9e5e5`  
		Last Modified: Tue, 29 Mar 2022 01:05:21 GMT  
		Size: 28.9 MB (28920513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afcd77f21f54e947717641dc9eb4a3c32a321dd3df6f615e082da0d916f9c6ca`  
		Last Modified: Wed, 30 Mar 2022 01:10:09 GMT  
		Size: 1.7 KB (1729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96e6a8e69828bdad8405be855d17ef3331b8093c3773b6a6ed726e8788cc3fe1`  
		Last Modified: Wed, 30 Mar 2022 01:10:09 GMT  
		Size: 1.1 KB (1053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e672a3f91acf51a5b4252fc7a5e23c4bd9539029d819fafe90af13149b18a97`  
		Last Modified: Wed, 30 Mar 2022 01:10:12 GMT  
		Size: 5.0 MB (5027710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11475c4da412af9a0208f5a0962e32a7bd674a732fc2cb1bd58a16deb9aac2e4`  
		Last Modified: Wed, 30 Mar 2022 01:10:09 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2adba7e3a404697c9d1e15fe08cfbb357d8dd16b877a299ca347781afd782675`  
		Last Modified: Wed, 30 Mar 2022 01:10:09 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; arm variant v7

```console
$ docker pull spiped@sha256:2dbc8de74b30a303a09ce36ac401dbbc2edd6a659c643579a43d0243250acd0b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.3 MB (31326537 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:04bbd512c51b4df932d3725ab91fe61a2eecb9b729392297a9634c096f37e9aa`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 29 Mar 2022 02:18:34 GMT
ADD file:e1835d1a0c70a0335757f211893e5d12ddf797e489e10434c0982bdf9b234f67 in / 
# Tue, 29 Mar 2022 02:18:36 GMT
CMD ["bash"]
# Wed, 30 Mar 2022 16:37:08 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 30 Mar 2022 16:37:15 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 30 Mar 2022 16:37:16 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 30 Mar 2022 16:38:00 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 30 Mar 2022 16:38:01 GMT
VOLUME [/spiped]
# Wed, 30 Mar 2022 16:38:01 GMT
WORKDIR /spiped
# Wed, 30 Mar 2022 16:38:02 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 30 Mar 2022 16:38:02 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 30 Mar 2022 16:38:03 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:f98812e1a494a683a5b3dea593dd2ef305f5f732193044c147f22e44b00164bc`  
		Last Modified: Tue, 29 Mar 2022 02:34:13 GMT  
		Size: 26.6 MB (26575370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b566a0eb6f50a4d3076e96e1230218651c8e3409f1e36b78720641ddcf02fe67`  
		Last Modified: Wed, 30 Mar 2022 16:39:28 GMT  
		Size: 1.7 KB (1730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3653f9517ce7a66aa5b26388c993e6803d010dd10becbc1141166b19d0575c20`  
		Last Modified: Wed, 30 Mar 2022 16:39:28 GMT  
		Size: 1.1 KB (1055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bef73e1c106acd2821aea52e999a0ab3dc8a102d38cf18f931ff036fc5cdde29`  
		Last Modified: Wed, 30 Mar 2022 16:39:32 GMT  
		Size: 4.7 MB (4747910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1eb71618098b05bae1eef477c77b1abb4846fb9cb147e36318ec26d12542a9db`  
		Last Modified: Wed, 30 Mar 2022 16:39:28 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4742b0162d23f2f2a3f504f4d0eded391b6c812f26030eca3f9137563d7d44fc`  
		Last Modified: Wed, 30 Mar 2022 16:39:28 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:489251bdbc8f5a1d43cb461dba8917af4fb58142240f15e7d2c7c31f7d859b2b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.3 MB (35337814 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bead5c7928697f7d3aded01a859186f595bedcb48737aebb29d40d92c78230e5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 29 Mar 2022 00:43:17 GMT
ADD file:e95289cd39de0f389d09cda9edf8476d5da371bc68d76e820c5e1c310dc54baf in / 
# Tue, 29 Mar 2022 00:43:17 GMT
CMD ["bash"]
# Wed, 30 Mar 2022 01:01:29 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 30 Mar 2022 01:01:33 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 30 Mar 2022 01:01:34 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 30 Mar 2022 01:01:58 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 30 Mar 2022 01:01:58 GMT
VOLUME [/spiped]
# Wed, 30 Mar 2022 01:01:59 GMT
WORKDIR /spiped
# Wed, 30 Mar 2022 01:02:01 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 30 Mar 2022 01:02:01 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 30 Mar 2022 01:02:02 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:2203022c5aa978ec114a15a7cdc2c323c65922d3b0a8eab11d50811bb9ae1cfb`  
		Last Modified: Tue, 29 Mar 2022 00:50:04 GMT  
		Size: 30.1 MB (30064311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c1c5ff6bd12cad4539ef42aba72b9e2a79fd5e03cf703d178e9179cf3ca28d3`  
		Last Modified: Wed, 30 Mar 2022 01:03:05 GMT  
		Size: 1.6 KB (1619 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d32807b7cfbcaf6c5dda896ed26a7d5b103161f8237a6f762874f9d2e713509`  
		Last Modified: Wed, 30 Mar 2022 01:03:04 GMT  
		Size: 923.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbc810f776215aefbbbcac36475250c8768eea0d0fdb5cdeceb3a2ed84c8dbb8`  
		Last Modified: Wed, 30 Mar 2022 01:03:06 GMT  
		Size: 5.3 MB (5270525 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d1419d96420314f5d538869ef6bf4d3e349c952c254f754fba1e39a0ba1a36c`  
		Last Modified: Wed, 30 Mar 2022 01:03:04 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:533163ce32b9d79dc658ade7a26d7f71cece5b9bf114cc7b7dc3596ba66609ba`  
		Last Modified: Wed, 30 Mar 2022 01:03:04 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; 386

```console
$ docker pull spiped@sha256:7bf4cc6d7160264b61ad5339a1b254c94c216125bf624adbb4a44b1a484a71b1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.3 MB (40283723 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e193db912bc32b089a793405a8541f1cb6d938b1dad5dc81b749bdb791619efa`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 29 Mar 2022 00:42:01 GMT
ADD file:d093057c080a13cc4370d0e786857751004b8cd3c93368742512abbee4f1de83 in / 
# Tue, 29 Mar 2022 00:42:01 GMT
CMD ["bash"]
# Tue, 29 Mar 2022 10:43:59 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 29 Mar 2022 10:44:03 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 29 Mar 2022 10:44:04 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 29 Mar 2022 10:44:24 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 29 Mar 2022 10:44:25 GMT
VOLUME [/spiped]
# Tue, 29 Mar 2022 10:44:26 GMT
WORKDIR /spiped
# Tue, 29 Mar 2022 10:44:28 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 29 Mar 2022 10:44:28 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 29 Mar 2022 10:44:29 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:fec59da75229f638ca2878278d3859a1a8b73a20d5c0c043354eb37129ebb8bf`  
		Last Modified: Tue, 29 Mar 2022 00:49:10 GMT  
		Size: 32.4 MB (32389518 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:559c323dcf632c3e6c78229ea96b201cd5c6a73598a208ba2fd88a55a2e53f6a`  
		Last Modified: Tue, 29 Mar 2022 10:45:19 GMT  
		Size: 1.6 KB (1611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7b0c52bcbc80dacdfd452f5135ca2e640ab57050b38fbf5890ca41339ce8cbf`  
		Last Modified: Tue, 29 Mar 2022 10:45:19 GMT  
		Size: 924.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0e273d1baff760d787e4bf5a3e20801cf5a8e2625eada853a4d7cdd86c1e25f`  
		Last Modified: Tue, 29 Mar 2022 10:45:20 GMT  
		Size: 7.9 MB (7891233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd7f99497ff10c89ef5d937c4f127f94bcc0391017c3fa45d587bab079706dea`  
		Last Modified: Tue, 29 Mar 2022 10:45:19 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61bb3d200b36c323a0edaaa6ceb5990790f17562ef9d5e5c63d7fab6d1978d51`  
		Last Modified: Tue, 29 Mar 2022 10:45:19 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; mips64le

```console
$ docker pull spiped@sha256:616f8531e23b941b90c8d1293b641771b4c758475fff50f5f6f50bdceae91f2c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.3 MB (35349463 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e57ad4c68f94212319101e900c6737ad74d321485f03cf0cf7522b7259c35ac0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 29 Mar 2022 07:42:27 GMT
ADD file:32aa9fd7ee5c64e4bd49459e801e3e5dc50138590bbfca671e336a197aa7fa92 in / 
# Tue, 29 Mar 2022 07:42:31 GMT
CMD ["bash"]
# Wed, 30 Mar 2022 05:36:13 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 30 Mar 2022 05:36:28 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 30 Mar 2022 05:36:31 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 30 Mar 2022 05:38:04 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 30 Mar 2022 05:38:06 GMT
VOLUME [/spiped]
# Wed, 30 Mar 2022 05:38:09 GMT
WORKDIR /spiped
# Wed, 30 Mar 2022 05:38:12 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 30 Mar 2022 05:38:14 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 30 Mar 2022 05:38:17 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:5c2a8045f9de06328ab3d0ff505d990892219b7faee393bc9ac342347fc83d04`  
		Last Modified: Tue, 29 Mar 2022 07:52:59 GMT  
		Size: 29.6 MB (29641474 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28d11336cbfa9f2c1e6c22eef2096c37397f6a0058407687dc007bf7384a3e79`  
		Last Modified: Wed, 30 Mar 2022 05:38:29 GMT  
		Size: 1.6 KB (1629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd53cadc47175f65d5df3546949d7f0a90aec5d75b5fe538a9a9b4fe2ebeefd2`  
		Last Modified: Wed, 30 Mar 2022 05:38:29 GMT  
		Size: 924.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcdf8956bed67848aaf6e2f1456d79a9db2efc0f6986df8eb00feb2d30de9389`  
		Last Modified: Wed, 30 Mar 2022 05:38:34 GMT  
		Size: 5.7 MB (5704999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6a3ca7ecd16ef5159abf00ec43e34fbe1b528c2416e3b0eb94806b1d5445e5d`  
		Last Modified: Wed, 30 Mar 2022 05:38:29 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:109d3b9867a03e8499cbf83271d977a1bbf8550acb992fce7348de6047db039f`  
		Last Modified: Wed, 30 Mar 2022 05:38:29 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; ppc64le

```console
$ docker pull spiped@sha256:20cc9df235f7239597ba6e9f0da45b8a2476c6020795502aa68f0b7275799a6d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.3 MB (41284580 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a9d0a0f307401e56e3c154076006ae5b0585b5124c0ad643d5fc5305effea55c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 29 Mar 2022 00:22:08 GMT
ADD file:e7ae113c10f322a9cffc46b62ba12820e270caaadaee3c5b907c801a37e1632c in / 
# Tue, 29 Mar 2022 00:22:11 GMT
CMD ["bash"]
# Wed, 30 Mar 2022 05:21:11 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 30 Mar 2022 05:21:26 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 30 Mar 2022 05:21:30 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 30 Mar 2022 05:24:47 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 30 Mar 2022 05:24:55 GMT
VOLUME [/spiped]
# Wed, 30 Mar 2022 05:25:01 GMT
WORKDIR /spiped
# Wed, 30 Mar 2022 05:25:04 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 30 Mar 2022 05:25:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 30 Mar 2022 05:25:15 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:ecc74bb8af5a048e1123af0e17d88ef3da1d10951ada79e8e1cc9c0a694245d3`  
		Last Modified: Tue, 29 Mar 2022 00:32:57 GMT  
		Size: 35.3 MB (35282506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89e50c6a3f6bfe8c939d3f4cf697d6972444715b3e29bbe8ba3a8503b2d47744`  
		Last Modified: Wed, 30 Mar 2022 05:27:29 GMT  
		Size: 1.7 KB (1748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06d13b3a37c65e9f1e8f7d06ea8947895095e24e8766405225cfb8a7a68897fd`  
		Last Modified: Wed, 30 Mar 2022 05:27:29 GMT  
		Size: 1.1 KB (1056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bf7cfaec929baf5dd2ec1c286ff49084391ed126f695c76cc847467adb4b808`  
		Last Modified: Wed, 30 Mar 2022 05:27:31 GMT  
		Size: 6.0 MB (5998799 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0d18fb763428d4908c4dccb28dd79a1ef28deee5b1869dd026f99019b274d04`  
		Last Modified: Wed, 30 Mar 2022 05:27:29 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17b9492405cf9ecc040958db5b6363eb0b2a3fb3a3113526b3c94ebbe352ec9c`  
		Last Modified: Wed, 30 Mar 2022 05:27:29 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; s390x

```console
$ docker pull spiped@sha256:bc909d5eeee60c7823173755c87467307f944145474e127199afc7d15643b99c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.8 MB (34845094 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2c0bcec57634c726f934b24b28bf162da99aacbf72dd089108346ddd627e4284`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 29 Mar 2022 00:51:57 GMT
ADD file:39c5e0d7a686abd19448ab3e6237d50955ae2187fc2b64289a08c2549352b8f1 in / 
# Tue, 29 Mar 2022 00:51:58 GMT
CMD ["bash"]
# Wed, 30 Mar 2022 02:17:13 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 30 Mar 2022 02:17:16 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 30 Mar 2022 02:17:16 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 30 Mar 2022 02:17:28 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 30 Mar 2022 02:17:29 GMT
VOLUME [/spiped]
# Wed, 30 Mar 2022 02:17:29 GMT
WORKDIR /spiped
# Wed, 30 Mar 2022 02:17:29 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 30 Mar 2022 02:17:29 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 30 Mar 2022 02:17:29 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:ffb22bcde95509bb75f6dd2d69f3fdb5c7471727e4d720b31d92cd297582865c`  
		Last Modified: Tue, 29 Mar 2022 01:04:43 GMT  
		Size: 29.7 MB (29655426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9488a45de61a7c26b2a863c250a52839737d409c8bac0426e2161131489985d3`  
		Last Modified: Wed, 30 Mar 2022 02:18:10 GMT  
		Size: 1.7 KB (1735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abedbd8409757c2b32910d965e11e1ba2d29a16105361932d6d8bd82b611d64d`  
		Last Modified: Wed, 30 Mar 2022 02:18:10 GMT  
		Size: 1.1 KB (1053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0eb1d8925fb8e4d0edc85c85b1f0d782db61bdf479a93bc6a0ccd97410d5a81`  
		Last Modified: Wed, 30 Mar 2022 02:18:10 GMT  
		Size: 5.2 MB (5186412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7987418a0dc4bd8525c7ad87f10f5f7ca2fdd8060ac0807f66714351df3d27cc`  
		Last Modified: Wed, 30 Mar 2022 02:18:10 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3647b49ea4318215c86c777031179b0cacb01790a04d0208a9d80a7962bb5768`  
		Last Modified: Wed, 30 Mar 2022 02:18:10 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:1.6-alpine`

```console
$ docker pull spiped@sha256:df67424ae1b5f50fe62e3c8f7584a176cef62ba9d479ccd376f70587ae42ca61
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
$ docker pull spiped@sha256:b1000f43786f16a20a805fa353f6e29da279735ce16fc397001fde0e351cadab
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (3038963 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:319549bf17a1c296f365e261889f2573a629fda0ca36fa2dac3efc79c233dc4d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 05 Apr 2022 00:19:59 GMT
ADD file:5d673d25da3a14ce1f6cf66e4c7fd4f4b85a3759a9d93efb3fd9ff852b5b56e4 in / 
# Tue, 05 Apr 2022 00:19:59 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 09:41:12 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Tue, 05 Apr 2022 09:41:13 GMT
RUN apk add --no-cache libssl1.1
# Tue, 05 Apr 2022 09:41:13 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 05 Apr 2022 09:41:22 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Tue, 05 Apr 2022 09:41:22 GMT
VOLUME [/spiped]
# Tue, 05 Apr 2022 09:41:23 GMT
WORKDIR /spiped
# Tue, 05 Apr 2022 09:41:23 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 05 Apr 2022 09:41:23 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 05 Apr 2022 09:41:23 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:df9b9388f04ad6279a7410b85cedfdcb2208c0a003da7ab5613af71079148139`  
		Last Modified: Mon, 04 Apr 2022 19:10:16 GMT  
		Size: 2.8 MB (2814559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:735044c06e8b73c2bb88467804d54b359bfc8226cf975772cc666adc9f029f5c`  
		Last Modified: Tue, 05 Apr 2022 09:41:38 GMT  
		Size: 1.3 KB (1271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd8b16fcaec70a3de42b4e850be4a851eaffa96a04fb49668b0d55b15bdf9675`  
		Last Modified: Tue, 05 Apr 2022 09:41:38 GMT  
		Size: 7.8 KB (7783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79236b25532d68c328b81af71a0f8c4eca102b7030a98d650ffc9a7e35d113be`  
		Last Modified: Tue, 05 Apr 2022 09:41:38 GMT  
		Size: 214.9 KB (214880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f429bef29fed68fb012179a10893c62fd5167934a7d62e7d3db15361601d47e9`  
		Last Modified: Tue, 05 Apr 2022 09:41:38 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1703108ce26f514d42179cf03051a6082b57e184d89f7bab08377819025c74d9`  
		Last Modified: Tue, 05 Apr 2022 09:41:38 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; arm variant v6

```console
$ docker pull spiped@sha256:ae66fb10272b529530524084a214a11e65777dff6517d5a90d71357e60416246
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 MB (2830615 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aae9a0570520cf722d24d3a84685d936a04a06d1b8e35de44be52daca29219ea`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 29 Mar 2022 00:49:32 GMT
ADD file:44acf536d487bec7f7bf16561f4ec90e60d4447b3cbabfeca66953c4491aabeb in / 
# Tue, 29 Mar 2022 00:49:33 GMT
CMD ["/bin/sh"]
# Tue, 29 Mar 2022 08:24:39 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Tue, 29 Mar 2022 08:24:41 GMT
RUN apk add --no-cache libssl1.1
# Tue, 29 Mar 2022 08:24:41 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 29 Mar 2022 08:25:01 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Tue, 29 Mar 2022 08:25:01 GMT
VOLUME [/spiped]
# Tue, 29 Mar 2022 08:25:02 GMT
WORKDIR /spiped
# Tue, 29 Mar 2022 08:25:03 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 29 Mar 2022 08:25:03 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 29 Mar 2022 08:25:04 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:84f033dabe5013c0dfae4263abd951011719d0a15adc3c7312c5be994deff030`  
		Last Modified: Tue, 29 Mar 2022 00:51:25 GMT  
		Size: 2.6 MB (2621943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdc4ea1012b3262fa7706463586c4d41a0cf0a329238cbe52ea6d03bfbc07fae`  
		Last Modified: Tue, 29 Mar 2022 08:25:35 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5659ae5d68adc8e4012f07c665ea352c4068ee821e83350f8bc165b6aea5583`  
		Last Modified: Tue, 29 Mar 2022 08:25:35 GMT  
		Size: 7.8 KB (7774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bf4925cebf49f63997a8c7389e423c3623dc4cd2e6c701e4282c664293e789b`  
		Last Modified: Tue, 29 Mar 2022 08:25:35 GMT  
		Size: 199.2 KB (199158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6eac1b140b33266f585c96310939c5cdbac7bde1fcbc0bd4e8cde9f9f0dd5171`  
		Last Modified: Tue, 29 Mar 2022 08:25:35 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11b13e602bdbc874391ee6aee0f8abffe1e74ee57061d9e1faed46aa76ad44a0`  
		Last Modified: Tue, 29 Mar 2022 08:25:35 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; arm variant v7

```console
$ docker pull spiped@sha256:1533669bdce5be15027cb96650fabea206274558c0195f437de5245079d89f0f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 MB (2626515 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:52a32db31d94e7ea2f1af7b835d809d1b42c16deff1071fe4b3f2e720bc3688c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 29 Mar 2022 02:13:28 GMT
ADD file:8c959b80e3661beea7b3468017b88897d981bf52ed43c074e7c87ecb753e9059 in / 
# Tue, 29 Mar 2022 02:13:28 GMT
CMD ["/bin/sh"]
# Wed, 30 Mar 2022 16:38:17 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Wed, 30 Mar 2022 16:38:19 GMT
RUN apk add --no-cache libssl1.1
# Wed, 30 Mar 2022 16:38:20 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 30 Mar 2022 16:38:38 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Wed, 30 Mar 2022 16:38:38 GMT
VOLUME [/spiped]
# Wed, 30 Mar 2022 16:38:39 GMT
WORKDIR /spiped
# Wed, 30 Mar 2022 16:38:40 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 30 Mar 2022 16:38:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 30 Mar 2022 16:38:40 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:22b1e5a07a97d7af6fdc335e3b3a975b73908fa19b084289c408a00814da0398`  
		Last Modified: Tue, 29 Mar 2022 02:15:28 GMT  
		Size: 2.4 MB (2424303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1b864dcb6ac61a275d83b41f5e533000faf52fae810b4fc0513796337285828`  
		Last Modified: Wed, 30 Mar 2022 16:39:51 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3aed778a3d8f2984cc57d3cbd49d0974e4d48f31a548da40051a676285fcb98`  
		Last Modified: Wed, 30 Mar 2022 16:39:51 GMT  
		Size: 7.8 KB (7781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23bc58fbe93b76dec15870d5507d4377afa5e3cd4e9ddd68e1117ed5fb9b1953`  
		Last Modified: Wed, 30 Mar 2022 16:39:52 GMT  
		Size: 192.7 KB (192691 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1f1a66e69919430ccc221d6a8b42a90a4ebdee7a41b426b4cabbd472c3d62a3`  
		Last Modified: Wed, 30 Mar 2022 16:39:51 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6342a8067391971e5056968d5d26841d53aeaab30109c42bb6c53a227f694cab`  
		Last Modified: Wed, 30 Mar 2022 16:39:51 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:c0d28956af21c9ad7d0e3d4cf972b301ea28efa0c8755d1ee62841b09754b0ab
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 MB (2933013 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a11675ed63f0f0f4c5e2d5175c06bade440268d204f7a4b104eba50db3f998da`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 29 Mar 2022 00:40:05 GMT
ADD file:24e8b04304ef91bbf949674909ccaf2c66e3dcd096c3c307a0510569eadf576f in / 
# Tue, 29 Mar 2022 00:40:05 GMT
CMD ["/bin/sh"]
# Wed, 30 Mar 2022 01:02:13 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Wed, 30 Mar 2022 01:02:15 GMT
RUN apk add --no-cache libssl1.1
# Wed, 30 Mar 2022 01:02:16 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 30 Mar 2022 01:02:34 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Wed, 30 Mar 2022 01:02:35 GMT
VOLUME [/spiped]
# Wed, 30 Mar 2022 01:02:36 GMT
WORKDIR /spiped
# Wed, 30 Mar 2022 01:02:38 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 30 Mar 2022 01:02:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 30 Mar 2022 01:02:39 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:80fa7f07ec7b717ec5f8e2717b91e3d659e129052ec3def2570a5674322688d9`  
		Last Modified: Tue, 29 Mar 2022 00:41:08 GMT  
		Size: 2.7 MB (2716347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ef7ee2c7f3dc7bcaf9752a844248d8127145ffd675ae5de72b4be177fc37cd5`  
		Last Modified: Wed, 30 Mar 2022 01:03:39 GMT  
		Size: 1.2 KB (1240 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47c53830f06d1a108ac255dbff68c71fabc58723d0a42943fec7681cbebe653a`  
		Last Modified: Wed, 30 Mar 2022 01:03:38 GMT  
		Size: 7.8 KB (7751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e1f94f19caf7b781c37e261530b5861447ecd5ab33d55ad4d2f12a932db1cf8`  
		Last Modified: Wed, 30 Mar 2022 01:03:39 GMT  
		Size: 207.2 KB (207237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b259955a7b787ff533a05f42050e5172ba829db902cac41506236e30a45be04e`  
		Last Modified: Wed, 30 Mar 2022 01:03:38 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29db0547b8fb18568f5c6616a8622211952741a2a93da0e86cb506b1ee4c941c`  
		Last Modified: Wed, 30 Mar 2022 01:03:39 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; 386

```console
$ docker pull spiped@sha256:dcbb93128deb3206337ac10573e41e27b4a95816cd3f931412c655201fef2396
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.1 MB (3053817 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fdb9526919356b65e45d7bc9a9bd2aaddd7da8a1e62f023b9511a320a431df64`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Mon, 04 Apr 2022 23:38:25 GMT
ADD file:7d51a0f8691eb78c9062fd31984423a93d276a67b4ed5d1a706e1c2cd9fea23a in / 
# Mon, 04 Apr 2022 23:38:25 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 06:51:23 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Tue, 05 Apr 2022 06:51:24 GMT
RUN apk add --no-cache libssl1.1
# Tue, 05 Apr 2022 06:51:24 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 05 Apr 2022 06:51:34 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Tue, 05 Apr 2022 06:51:35 GMT
VOLUME [/spiped]
# Tue, 05 Apr 2022 06:51:36 GMT
WORKDIR /spiped
# Tue, 05 Apr 2022 06:51:38 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 05 Apr 2022 06:51:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 05 Apr 2022 06:51:39 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:73b28a5955ec7fb46f2cf0434e4901a889f7dda3f8c9ec496300feb256c7eda8`  
		Last Modified: Mon, 04 Apr 2022 19:10:03 GMT  
		Size: 2.8 MB (2818974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5043c44edf55100d2df153f657912b53abf987ef0c6286b113dcef298998f359`  
		Last Modified: Tue, 05 Apr 2022 06:52:09 GMT  
		Size: 1.2 KB (1240 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfc9d36e654ea336dd74dc00574768a6502edd5ef5cd785b695e516f6254be55`  
		Last Modified: Tue, 05 Apr 2022 06:52:08 GMT  
		Size: 7.8 KB (7750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0401735f1a5cdc5a0248a778049579b8858a6f7cc0fc6fdcdaea211930d4a386`  
		Last Modified: Tue, 05 Apr 2022 06:52:08 GMT  
		Size: 225.4 KB (225416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5a85e3f263e110e3fa50aada2a3ca6314a5a6e67e8f211881a826585a5db409`  
		Last Modified: Tue, 05 Apr 2022 06:52:08 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a0f113efbe13d3511b57cb0428e99f2725a51cb3980e75b1f1be3fc0d715b19`  
		Last Modified: Tue, 05 Apr 2022 06:52:08 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; ppc64le

```console
$ docker pull spiped@sha256:d27c5eb0ad348fe2a50b65e808e4b825f0f479572187d81757b9a82ce2ad9e50
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (3033662 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1853309ab0785a26d0b48053b424c5b8c4ffd6367504032c68e3377b9fc92eba`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 29 Mar 2022 00:16:52 GMT
ADD file:9e7b65a431d59070abaadae56d9c3fc59c899af881939e4353b1f524b2bd5185 in / 
# Tue, 29 Mar 2022 00:16:55 GMT
CMD ["/bin/sh"]
# Wed, 30 Mar 2022 05:25:40 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Wed, 30 Mar 2022 05:25:50 GMT
RUN apk add --no-cache libssl1.1
# Wed, 30 Mar 2022 05:25:53 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 30 Mar 2022 05:26:20 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Wed, 30 Mar 2022 05:26:24 GMT
VOLUME [/spiped]
# Wed, 30 Mar 2022 05:26:28 GMT
WORKDIR /spiped
# Wed, 30 Mar 2022 05:26:35 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 30 Mar 2022 05:26:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 30 Mar 2022 05:26:46 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:1c611bca4fa49cac5bc1e3826ad53fee85ed659d24bffcccd86c3f04be07339a`  
		Last Modified: Tue, 29 Mar 2022 00:18:26 GMT  
		Size: 2.8 MB (2811009 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b61e9d70cfabe50a7554945008b067920fffa673936b1b8c50f29cdbc07fad93`  
		Last Modified: Wed, 30 Mar 2022 05:27:51 GMT  
		Size: 1.3 KB (1263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd9a458bb0005f54d005e938aa01a6aeeb1d7c48486de6811d1c16a9846b1239`  
		Last Modified: Wed, 30 Mar 2022 05:27:51 GMT  
		Size: 7.8 KB (7774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be8c858ba1f6886855b0312ec6b3618c916bea4577c858d028e6709d67f05939`  
		Last Modified: Wed, 30 Mar 2022 05:27:51 GMT  
		Size: 213.1 KB (213149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1d4e4cb20d1bd858c134eae12aac2cab24001fbae386ee7f84b1e8dc6c6ef76`  
		Last Modified: Wed, 30 Mar 2022 05:27:51 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20cb5033835d271b66d87c37a113ae41ee09c6b1c5b462196462cb06687e3352`  
		Last Modified: Wed, 30 Mar 2022 05:27:51 GMT  
		Size: 338.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; s390x

```console
$ docker pull spiped@sha256:851d4d1e8b82de6d455e9a562bd6b75539fe737213c9f3cf01ce7b44e11abeb4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 MB (2811594 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e240f56e6000d053b4d3e20632b54b88daaa8dad76ecda720ce9f76c82bfe394`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Mon, 04 Apr 2022 23:41:39 GMT
ADD file:f22e4b2be87d3c59c8c609acf79015938dc1fba0b26d7c1b59bd0fc36d63a906 in / 
# Mon, 04 Apr 2022 23:41:39 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 06:09:44 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Tue, 05 Apr 2022 06:09:45 GMT
RUN apk add --no-cache libssl1.1
# Tue, 05 Apr 2022 06:09:45 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 05 Apr 2022 06:09:50 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Tue, 05 Apr 2022 06:09:50 GMT
VOLUME [/spiped]
# Tue, 05 Apr 2022 06:09:51 GMT
WORKDIR /spiped
# Tue, 05 Apr 2022 06:09:51 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 05 Apr 2022 06:09:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 05 Apr 2022 06:09:51 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:a27b630f446c3da376a30cf610e4bfa6847f8b87c83702c29e72b986f4e52d28`  
		Last Modified: Mon, 04 Apr 2022 23:42:37 GMT  
		Size: 2.6 MB (2600375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ffc8ec477cbe2d575e99a9232e9328db8cc40109dbe067d93c2033302576850`  
		Last Modified: Tue, 05 Apr 2022 06:10:22 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ee008c7ec71319091cda7b7cbf1063414ee758f739581409a2e7089e90882c9`  
		Last Modified: Tue, 05 Apr 2022 06:10:21 GMT  
		Size: 7.8 KB (7788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3edcb5212f084eabfd1bad6e332d8b53bd7756099c4da3e410ee23f869a701b`  
		Last Modified: Tue, 05 Apr 2022 06:10:21 GMT  
		Size: 201.7 KB (201693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd099e1efb05ce5fa06c5e18ba7d057b5df318c462022f1ac443f45e86fdc809`  
		Last Modified: Tue, 05 Apr 2022 06:10:21 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afbab95e29c022d6828d869e5e4442b139373571c747f8fc6470b8bd257337a4`  
		Last Modified: Tue, 05 Apr 2022 06:10:21 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:1.6.2`

```console
$ docker pull spiped@sha256:1096e8cf1ee57825fa381a290095d3d42ebddf1e22f54edb53f96109d8466d0d
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
$ docker pull spiped@sha256:f236fca971a0526aa22ab4aa69709d302210d7e1f5bd42902bde2803ec0495bd
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.3 MB (37348627 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0ab54c336e542bbe2bacf29196b05876f18889ca6f79cd1c223af52a9bcf3241`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 29 Mar 2022 00:22:18 GMT
ADD file:966d3669b40f5fbaecee1ecbeb58debe19001076da5d94717080d55efbc25971 in / 
# Tue, 29 Mar 2022 00:22:19 GMT
CMD ["bash"]
# Tue, 29 Mar 2022 12:05:44 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 29 Mar 2022 12:05:47 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 29 Mar 2022 12:05:47 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 29 Mar 2022 12:06:06 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 29 Mar 2022 12:06:07 GMT
VOLUME [/spiped]
# Tue, 29 Mar 2022 12:06:07 GMT
WORKDIR /spiped
# Tue, 29 Mar 2022 12:06:07 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 29 Mar 2022 12:06:07 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 29 Mar 2022 12:06:07 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:c229119241af7b23b121052a1cae4c03e0a477a72ea6a7f463ad7623ff8f274b`  
		Last Modified: Tue, 29 Mar 2022 00:27:16 GMT  
		Size: 31.4 MB (31378457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fda024001dd8419f652d3fde717d37b32c648032cc3f92d00978db9268a65b97`  
		Last Modified: Tue, 29 Mar 2022 12:06:37 GMT  
		Size: 1.7 KB (1736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b55c823e9d54047194e3c5cef477607293ed02e6d1b77f8f6f834f50fe2e9d05`  
		Last Modified: Tue, 29 Mar 2022 12:06:37 GMT  
		Size: 1.1 KB (1052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55ae1339c87c4e759ff4a439ee8561a8481ea3131678ac5e2f58795506cb67fc`  
		Last Modified: Tue, 29 Mar 2022 12:06:38 GMT  
		Size: 6.0 MB (5966913 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eda9f112e9f42cfee9c6890693553b623bf2dd540c36f29ad14276acb22e044e`  
		Last Modified: Tue, 29 Mar 2022 12:06:37 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad6ba00100ccbdece1902154d0d0d33ee3d70d4e184a6524a97b6ab7e2e53192`  
		Last Modified: Tue, 29 Mar 2022 12:06:37 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.2` - linux; arm variant v5

```console
$ docker pull spiped@sha256:94736a8efc0da3dd2c4c38b0a356b70873aee616c541dbccdfa95068dc6c0cb6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.0 MB (33951476 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cfb46d52c65a3d3391adc84884f180419a0f9437774a897d2ba90ecff46cb1cb`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 29 Mar 2022 00:50:37 GMT
ADD file:6b9a30e6ef50a46e87cf9d7f5a491c7951fdb6dd6fab3c9d4a9c3c40f92b8db4 in / 
# Tue, 29 Mar 2022 00:50:38 GMT
CMD ["bash"]
# Wed, 30 Mar 2022 01:08:33 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 30 Mar 2022 01:08:43 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 30 Mar 2022 01:08:43 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 30 Mar 2022 01:09:31 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 30 Mar 2022 01:09:32 GMT
VOLUME [/spiped]
# Wed, 30 Mar 2022 01:09:32 GMT
WORKDIR /spiped
# Wed, 30 Mar 2022 01:09:33 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 30 Mar 2022 01:09:33 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 30 Mar 2022 01:09:34 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:9a41aba0a099ec129c20f41f6370b97daa4c3d4d3edc76ea1863bc5f76f9e5e5`  
		Last Modified: Tue, 29 Mar 2022 01:05:21 GMT  
		Size: 28.9 MB (28920513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afcd77f21f54e947717641dc9eb4a3c32a321dd3df6f615e082da0d916f9c6ca`  
		Last Modified: Wed, 30 Mar 2022 01:10:09 GMT  
		Size: 1.7 KB (1729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96e6a8e69828bdad8405be855d17ef3331b8093c3773b6a6ed726e8788cc3fe1`  
		Last Modified: Wed, 30 Mar 2022 01:10:09 GMT  
		Size: 1.1 KB (1053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e672a3f91acf51a5b4252fc7a5e23c4bd9539029d819fafe90af13149b18a97`  
		Last Modified: Wed, 30 Mar 2022 01:10:12 GMT  
		Size: 5.0 MB (5027710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11475c4da412af9a0208f5a0962e32a7bd674a732fc2cb1bd58a16deb9aac2e4`  
		Last Modified: Wed, 30 Mar 2022 01:10:09 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2adba7e3a404697c9d1e15fe08cfbb357d8dd16b877a299ca347781afd782675`  
		Last Modified: Wed, 30 Mar 2022 01:10:09 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.2` - linux; arm variant v7

```console
$ docker pull spiped@sha256:2dbc8de74b30a303a09ce36ac401dbbc2edd6a659c643579a43d0243250acd0b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.3 MB (31326537 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:04bbd512c51b4df932d3725ab91fe61a2eecb9b729392297a9634c096f37e9aa`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 29 Mar 2022 02:18:34 GMT
ADD file:e1835d1a0c70a0335757f211893e5d12ddf797e489e10434c0982bdf9b234f67 in / 
# Tue, 29 Mar 2022 02:18:36 GMT
CMD ["bash"]
# Wed, 30 Mar 2022 16:37:08 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 30 Mar 2022 16:37:15 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 30 Mar 2022 16:37:16 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 30 Mar 2022 16:38:00 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 30 Mar 2022 16:38:01 GMT
VOLUME [/spiped]
# Wed, 30 Mar 2022 16:38:01 GMT
WORKDIR /spiped
# Wed, 30 Mar 2022 16:38:02 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 30 Mar 2022 16:38:02 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 30 Mar 2022 16:38:03 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:f98812e1a494a683a5b3dea593dd2ef305f5f732193044c147f22e44b00164bc`  
		Last Modified: Tue, 29 Mar 2022 02:34:13 GMT  
		Size: 26.6 MB (26575370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b566a0eb6f50a4d3076e96e1230218651c8e3409f1e36b78720641ddcf02fe67`  
		Last Modified: Wed, 30 Mar 2022 16:39:28 GMT  
		Size: 1.7 KB (1730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3653f9517ce7a66aa5b26388c993e6803d010dd10becbc1141166b19d0575c20`  
		Last Modified: Wed, 30 Mar 2022 16:39:28 GMT  
		Size: 1.1 KB (1055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bef73e1c106acd2821aea52e999a0ab3dc8a102d38cf18f931ff036fc5cdde29`  
		Last Modified: Wed, 30 Mar 2022 16:39:32 GMT  
		Size: 4.7 MB (4747910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1eb71618098b05bae1eef477c77b1abb4846fb9cb147e36318ec26d12542a9db`  
		Last Modified: Wed, 30 Mar 2022 16:39:28 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4742b0162d23f2f2a3f504f4d0eded391b6c812f26030eca3f9137563d7d44fc`  
		Last Modified: Wed, 30 Mar 2022 16:39:28 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.2` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:489251bdbc8f5a1d43cb461dba8917af4fb58142240f15e7d2c7c31f7d859b2b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.3 MB (35337814 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bead5c7928697f7d3aded01a859186f595bedcb48737aebb29d40d92c78230e5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 29 Mar 2022 00:43:17 GMT
ADD file:e95289cd39de0f389d09cda9edf8476d5da371bc68d76e820c5e1c310dc54baf in / 
# Tue, 29 Mar 2022 00:43:17 GMT
CMD ["bash"]
# Wed, 30 Mar 2022 01:01:29 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 30 Mar 2022 01:01:33 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 30 Mar 2022 01:01:34 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 30 Mar 2022 01:01:58 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 30 Mar 2022 01:01:58 GMT
VOLUME [/spiped]
# Wed, 30 Mar 2022 01:01:59 GMT
WORKDIR /spiped
# Wed, 30 Mar 2022 01:02:01 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 30 Mar 2022 01:02:01 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 30 Mar 2022 01:02:02 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:2203022c5aa978ec114a15a7cdc2c323c65922d3b0a8eab11d50811bb9ae1cfb`  
		Last Modified: Tue, 29 Mar 2022 00:50:04 GMT  
		Size: 30.1 MB (30064311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c1c5ff6bd12cad4539ef42aba72b9e2a79fd5e03cf703d178e9179cf3ca28d3`  
		Last Modified: Wed, 30 Mar 2022 01:03:05 GMT  
		Size: 1.6 KB (1619 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d32807b7cfbcaf6c5dda896ed26a7d5b103161f8237a6f762874f9d2e713509`  
		Last Modified: Wed, 30 Mar 2022 01:03:04 GMT  
		Size: 923.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbc810f776215aefbbbcac36475250c8768eea0d0fdb5cdeceb3a2ed84c8dbb8`  
		Last Modified: Wed, 30 Mar 2022 01:03:06 GMT  
		Size: 5.3 MB (5270525 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d1419d96420314f5d538869ef6bf4d3e349c952c254f754fba1e39a0ba1a36c`  
		Last Modified: Wed, 30 Mar 2022 01:03:04 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:533163ce32b9d79dc658ade7a26d7f71cece5b9bf114cc7b7dc3596ba66609ba`  
		Last Modified: Wed, 30 Mar 2022 01:03:04 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.2` - linux; 386

```console
$ docker pull spiped@sha256:7bf4cc6d7160264b61ad5339a1b254c94c216125bf624adbb4a44b1a484a71b1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.3 MB (40283723 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e193db912bc32b089a793405a8541f1cb6d938b1dad5dc81b749bdb791619efa`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 29 Mar 2022 00:42:01 GMT
ADD file:d093057c080a13cc4370d0e786857751004b8cd3c93368742512abbee4f1de83 in / 
# Tue, 29 Mar 2022 00:42:01 GMT
CMD ["bash"]
# Tue, 29 Mar 2022 10:43:59 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 29 Mar 2022 10:44:03 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 29 Mar 2022 10:44:04 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 29 Mar 2022 10:44:24 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 29 Mar 2022 10:44:25 GMT
VOLUME [/spiped]
# Tue, 29 Mar 2022 10:44:26 GMT
WORKDIR /spiped
# Tue, 29 Mar 2022 10:44:28 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 29 Mar 2022 10:44:28 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 29 Mar 2022 10:44:29 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:fec59da75229f638ca2878278d3859a1a8b73a20d5c0c043354eb37129ebb8bf`  
		Last Modified: Tue, 29 Mar 2022 00:49:10 GMT  
		Size: 32.4 MB (32389518 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:559c323dcf632c3e6c78229ea96b201cd5c6a73598a208ba2fd88a55a2e53f6a`  
		Last Modified: Tue, 29 Mar 2022 10:45:19 GMT  
		Size: 1.6 KB (1611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7b0c52bcbc80dacdfd452f5135ca2e640ab57050b38fbf5890ca41339ce8cbf`  
		Last Modified: Tue, 29 Mar 2022 10:45:19 GMT  
		Size: 924.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0e273d1baff760d787e4bf5a3e20801cf5a8e2625eada853a4d7cdd86c1e25f`  
		Last Modified: Tue, 29 Mar 2022 10:45:20 GMT  
		Size: 7.9 MB (7891233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd7f99497ff10c89ef5d937c4f127f94bcc0391017c3fa45d587bab079706dea`  
		Last Modified: Tue, 29 Mar 2022 10:45:19 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61bb3d200b36c323a0edaaa6ceb5990790f17562ef9d5e5c63d7fab6d1978d51`  
		Last Modified: Tue, 29 Mar 2022 10:45:19 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.2` - linux; mips64le

```console
$ docker pull spiped@sha256:616f8531e23b941b90c8d1293b641771b4c758475fff50f5f6f50bdceae91f2c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.3 MB (35349463 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e57ad4c68f94212319101e900c6737ad74d321485f03cf0cf7522b7259c35ac0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 29 Mar 2022 07:42:27 GMT
ADD file:32aa9fd7ee5c64e4bd49459e801e3e5dc50138590bbfca671e336a197aa7fa92 in / 
# Tue, 29 Mar 2022 07:42:31 GMT
CMD ["bash"]
# Wed, 30 Mar 2022 05:36:13 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 30 Mar 2022 05:36:28 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 30 Mar 2022 05:36:31 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 30 Mar 2022 05:38:04 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 30 Mar 2022 05:38:06 GMT
VOLUME [/spiped]
# Wed, 30 Mar 2022 05:38:09 GMT
WORKDIR /spiped
# Wed, 30 Mar 2022 05:38:12 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 30 Mar 2022 05:38:14 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 30 Mar 2022 05:38:17 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:5c2a8045f9de06328ab3d0ff505d990892219b7faee393bc9ac342347fc83d04`  
		Last Modified: Tue, 29 Mar 2022 07:52:59 GMT  
		Size: 29.6 MB (29641474 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28d11336cbfa9f2c1e6c22eef2096c37397f6a0058407687dc007bf7384a3e79`  
		Last Modified: Wed, 30 Mar 2022 05:38:29 GMT  
		Size: 1.6 KB (1629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd53cadc47175f65d5df3546949d7f0a90aec5d75b5fe538a9a9b4fe2ebeefd2`  
		Last Modified: Wed, 30 Mar 2022 05:38:29 GMT  
		Size: 924.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcdf8956bed67848aaf6e2f1456d79a9db2efc0f6986df8eb00feb2d30de9389`  
		Last Modified: Wed, 30 Mar 2022 05:38:34 GMT  
		Size: 5.7 MB (5704999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6a3ca7ecd16ef5159abf00ec43e34fbe1b528c2416e3b0eb94806b1d5445e5d`  
		Last Modified: Wed, 30 Mar 2022 05:38:29 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:109d3b9867a03e8499cbf83271d977a1bbf8550acb992fce7348de6047db039f`  
		Last Modified: Wed, 30 Mar 2022 05:38:29 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.2` - linux; ppc64le

```console
$ docker pull spiped@sha256:20cc9df235f7239597ba6e9f0da45b8a2476c6020795502aa68f0b7275799a6d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.3 MB (41284580 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a9d0a0f307401e56e3c154076006ae5b0585b5124c0ad643d5fc5305effea55c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 29 Mar 2022 00:22:08 GMT
ADD file:e7ae113c10f322a9cffc46b62ba12820e270caaadaee3c5b907c801a37e1632c in / 
# Tue, 29 Mar 2022 00:22:11 GMT
CMD ["bash"]
# Wed, 30 Mar 2022 05:21:11 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 30 Mar 2022 05:21:26 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 30 Mar 2022 05:21:30 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 30 Mar 2022 05:24:47 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 30 Mar 2022 05:24:55 GMT
VOLUME [/spiped]
# Wed, 30 Mar 2022 05:25:01 GMT
WORKDIR /spiped
# Wed, 30 Mar 2022 05:25:04 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 30 Mar 2022 05:25:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 30 Mar 2022 05:25:15 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:ecc74bb8af5a048e1123af0e17d88ef3da1d10951ada79e8e1cc9c0a694245d3`  
		Last Modified: Tue, 29 Mar 2022 00:32:57 GMT  
		Size: 35.3 MB (35282506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89e50c6a3f6bfe8c939d3f4cf697d6972444715b3e29bbe8ba3a8503b2d47744`  
		Last Modified: Wed, 30 Mar 2022 05:27:29 GMT  
		Size: 1.7 KB (1748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06d13b3a37c65e9f1e8f7d06ea8947895095e24e8766405225cfb8a7a68897fd`  
		Last Modified: Wed, 30 Mar 2022 05:27:29 GMT  
		Size: 1.1 KB (1056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bf7cfaec929baf5dd2ec1c286ff49084391ed126f695c76cc847467adb4b808`  
		Last Modified: Wed, 30 Mar 2022 05:27:31 GMT  
		Size: 6.0 MB (5998799 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0d18fb763428d4908c4dccb28dd79a1ef28deee5b1869dd026f99019b274d04`  
		Last Modified: Wed, 30 Mar 2022 05:27:29 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17b9492405cf9ecc040958db5b6363eb0b2a3fb3a3113526b3c94ebbe352ec9c`  
		Last Modified: Wed, 30 Mar 2022 05:27:29 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.2` - linux; s390x

```console
$ docker pull spiped@sha256:bc909d5eeee60c7823173755c87467307f944145474e127199afc7d15643b99c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.8 MB (34845094 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2c0bcec57634c726f934b24b28bf162da99aacbf72dd089108346ddd627e4284`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 29 Mar 2022 00:51:57 GMT
ADD file:39c5e0d7a686abd19448ab3e6237d50955ae2187fc2b64289a08c2549352b8f1 in / 
# Tue, 29 Mar 2022 00:51:58 GMT
CMD ["bash"]
# Wed, 30 Mar 2022 02:17:13 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 30 Mar 2022 02:17:16 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 30 Mar 2022 02:17:16 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 30 Mar 2022 02:17:28 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 30 Mar 2022 02:17:29 GMT
VOLUME [/spiped]
# Wed, 30 Mar 2022 02:17:29 GMT
WORKDIR /spiped
# Wed, 30 Mar 2022 02:17:29 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 30 Mar 2022 02:17:29 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 30 Mar 2022 02:17:29 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:ffb22bcde95509bb75f6dd2d69f3fdb5c7471727e4d720b31d92cd297582865c`  
		Last Modified: Tue, 29 Mar 2022 01:04:43 GMT  
		Size: 29.7 MB (29655426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9488a45de61a7c26b2a863c250a52839737d409c8bac0426e2161131489985d3`  
		Last Modified: Wed, 30 Mar 2022 02:18:10 GMT  
		Size: 1.7 KB (1735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abedbd8409757c2b32910d965e11e1ba2d29a16105361932d6d8bd82b611d64d`  
		Last Modified: Wed, 30 Mar 2022 02:18:10 GMT  
		Size: 1.1 KB (1053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0eb1d8925fb8e4d0edc85c85b1f0d782db61bdf479a93bc6a0ccd97410d5a81`  
		Last Modified: Wed, 30 Mar 2022 02:18:10 GMT  
		Size: 5.2 MB (5186412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7987418a0dc4bd8525c7ad87f10f5f7ca2fdd8060ac0807f66714351df3d27cc`  
		Last Modified: Wed, 30 Mar 2022 02:18:10 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3647b49ea4318215c86c777031179b0cacb01790a04d0208a9d80a7962bb5768`  
		Last Modified: Wed, 30 Mar 2022 02:18:10 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:1.6.2-alpine`

```console
$ docker pull spiped@sha256:df67424ae1b5f50fe62e3c8f7584a176cef62ba9d479ccd376f70587ae42ca61
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
$ docker pull spiped@sha256:b1000f43786f16a20a805fa353f6e29da279735ce16fc397001fde0e351cadab
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (3038963 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:319549bf17a1c296f365e261889f2573a629fda0ca36fa2dac3efc79c233dc4d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 05 Apr 2022 00:19:59 GMT
ADD file:5d673d25da3a14ce1f6cf66e4c7fd4f4b85a3759a9d93efb3fd9ff852b5b56e4 in / 
# Tue, 05 Apr 2022 00:19:59 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 09:41:12 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Tue, 05 Apr 2022 09:41:13 GMT
RUN apk add --no-cache libssl1.1
# Tue, 05 Apr 2022 09:41:13 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 05 Apr 2022 09:41:22 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Tue, 05 Apr 2022 09:41:22 GMT
VOLUME [/spiped]
# Tue, 05 Apr 2022 09:41:23 GMT
WORKDIR /spiped
# Tue, 05 Apr 2022 09:41:23 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 05 Apr 2022 09:41:23 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 05 Apr 2022 09:41:23 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:df9b9388f04ad6279a7410b85cedfdcb2208c0a003da7ab5613af71079148139`  
		Last Modified: Mon, 04 Apr 2022 19:10:16 GMT  
		Size: 2.8 MB (2814559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:735044c06e8b73c2bb88467804d54b359bfc8226cf975772cc666adc9f029f5c`  
		Last Modified: Tue, 05 Apr 2022 09:41:38 GMT  
		Size: 1.3 KB (1271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd8b16fcaec70a3de42b4e850be4a851eaffa96a04fb49668b0d55b15bdf9675`  
		Last Modified: Tue, 05 Apr 2022 09:41:38 GMT  
		Size: 7.8 KB (7783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79236b25532d68c328b81af71a0f8c4eca102b7030a98d650ffc9a7e35d113be`  
		Last Modified: Tue, 05 Apr 2022 09:41:38 GMT  
		Size: 214.9 KB (214880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f429bef29fed68fb012179a10893c62fd5167934a7d62e7d3db15361601d47e9`  
		Last Modified: Tue, 05 Apr 2022 09:41:38 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1703108ce26f514d42179cf03051a6082b57e184d89f7bab08377819025c74d9`  
		Last Modified: Tue, 05 Apr 2022 09:41:38 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.2-alpine` - linux; arm variant v6

```console
$ docker pull spiped@sha256:ae66fb10272b529530524084a214a11e65777dff6517d5a90d71357e60416246
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 MB (2830615 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aae9a0570520cf722d24d3a84685d936a04a06d1b8e35de44be52daca29219ea`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 29 Mar 2022 00:49:32 GMT
ADD file:44acf536d487bec7f7bf16561f4ec90e60d4447b3cbabfeca66953c4491aabeb in / 
# Tue, 29 Mar 2022 00:49:33 GMT
CMD ["/bin/sh"]
# Tue, 29 Mar 2022 08:24:39 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Tue, 29 Mar 2022 08:24:41 GMT
RUN apk add --no-cache libssl1.1
# Tue, 29 Mar 2022 08:24:41 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 29 Mar 2022 08:25:01 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Tue, 29 Mar 2022 08:25:01 GMT
VOLUME [/spiped]
# Tue, 29 Mar 2022 08:25:02 GMT
WORKDIR /spiped
# Tue, 29 Mar 2022 08:25:03 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 29 Mar 2022 08:25:03 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 29 Mar 2022 08:25:04 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:84f033dabe5013c0dfae4263abd951011719d0a15adc3c7312c5be994deff030`  
		Last Modified: Tue, 29 Mar 2022 00:51:25 GMT  
		Size: 2.6 MB (2621943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdc4ea1012b3262fa7706463586c4d41a0cf0a329238cbe52ea6d03bfbc07fae`  
		Last Modified: Tue, 29 Mar 2022 08:25:35 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5659ae5d68adc8e4012f07c665ea352c4068ee821e83350f8bc165b6aea5583`  
		Last Modified: Tue, 29 Mar 2022 08:25:35 GMT  
		Size: 7.8 KB (7774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bf4925cebf49f63997a8c7389e423c3623dc4cd2e6c701e4282c664293e789b`  
		Last Modified: Tue, 29 Mar 2022 08:25:35 GMT  
		Size: 199.2 KB (199158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6eac1b140b33266f585c96310939c5cdbac7bde1fcbc0bd4e8cde9f9f0dd5171`  
		Last Modified: Tue, 29 Mar 2022 08:25:35 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11b13e602bdbc874391ee6aee0f8abffe1e74ee57061d9e1faed46aa76ad44a0`  
		Last Modified: Tue, 29 Mar 2022 08:25:35 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.2-alpine` - linux; arm variant v7

```console
$ docker pull spiped@sha256:1533669bdce5be15027cb96650fabea206274558c0195f437de5245079d89f0f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 MB (2626515 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:52a32db31d94e7ea2f1af7b835d809d1b42c16deff1071fe4b3f2e720bc3688c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 29 Mar 2022 02:13:28 GMT
ADD file:8c959b80e3661beea7b3468017b88897d981bf52ed43c074e7c87ecb753e9059 in / 
# Tue, 29 Mar 2022 02:13:28 GMT
CMD ["/bin/sh"]
# Wed, 30 Mar 2022 16:38:17 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Wed, 30 Mar 2022 16:38:19 GMT
RUN apk add --no-cache libssl1.1
# Wed, 30 Mar 2022 16:38:20 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 30 Mar 2022 16:38:38 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Wed, 30 Mar 2022 16:38:38 GMT
VOLUME [/spiped]
# Wed, 30 Mar 2022 16:38:39 GMT
WORKDIR /spiped
# Wed, 30 Mar 2022 16:38:40 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 30 Mar 2022 16:38:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 30 Mar 2022 16:38:40 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:22b1e5a07a97d7af6fdc335e3b3a975b73908fa19b084289c408a00814da0398`  
		Last Modified: Tue, 29 Mar 2022 02:15:28 GMT  
		Size: 2.4 MB (2424303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1b864dcb6ac61a275d83b41f5e533000faf52fae810b4fc0513796337285828`  
		Last Modified: Wed, 30 Mar 2022 16:39:51 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3aed778a3d8f2984cc57d3cbd49d0974e4d48f31a548da40051a676285fcb98`  
		Last Modified: Wed, 30 Mar 2022 16:39:51 GMT  
		Size: 7.8 KB (7781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23bc58fbe93b76dec15870d5507d4377afa5e3cd4e9ddd68e1117ed5fb9b1953`  
		Last Modified: Wed, 30 Mar 2022 16:39:52 GMT  
		Size: 192.7 KB (192691 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1f1a66e69919430ccc221d6a8b42a90a4ebdee7a41b426b4cabbd472c3d62a3`  
		Last Modified: Wed, 30 Mar 2022 16:39:51 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6342a8067391971e5056968d5d26841d53aeaab30109c42bb6c53a227f694cab`  
		Last Modified: Wed, 30 Mar 2022 16:39:51 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.2-alpine` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:c0d28956af21c9ad7d0e3d4cf972b301ea28efa0c8755d1ee62841b09754b0ab
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 MB (2933013 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a11675ed63f0f0f4c5e2d5175c06bade440268d204f7a4b104eba50db3f998da`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 29 Mar 2022 00:40:05 GMT
ADD file:24e8b04304ef91bbf949674909ccaf2c66e3dcd096c3c307a0510569eadf576f in / 
# Tue, 29 Mar 2022 00:40:05 GMT
CMD ["/bin/sh"]
# Wed, 30 Mar 2022 01:02:13 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Wed, 30 Mar 2022 01:02:15 GMT
RUN apk add --no-cache libssl1.1
# Wed, 30 Mar 2022 01:02:16 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 30 Mar 2022 01:02:34 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Wed, 30 Mar 2022 01:02:35 GMT
VOLUME [/spiped]
# Wed, 30 Mar 2022 01:02:36 GMT
WORKDIR /spiped
# Wed, 30 Mar 2022 01:02:38 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 30 Mar 2022 01:02:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 30 Mar 2022 01:02:39 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:80fa7f07ec7b717ec5f8e2717b91e3d659e129052ec3def2570a5674322688d9`  
		Last Modified: Tue, 29 Mar 2022 00:41:08 GMT  
		Size: 2.7 MB (2716347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ef7ee2c7f3dc7bcaf9752a844248d8127145ffd675ae5de72b4be177fc37cd5`  
		Last Modified: Wed, 30 Mar 2022 01:03:39 GMT  
		Size: 1.2 KB (1240 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47c53830f06d1a108ac255dbff68c71fabc58723d0a42943fec7681cbebe653a`  
		Last Modified: Wed, 30 Mar 2022 01:03:38 GMT  
		Size: 7.8 KB (7751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e1f94f19caf7b781c37e261530b5861447ecd5ab33d55ad4d2f12a932db1cf8`  
		Last Modified: Wed, 30 Mar 2022 01:03:39 GMT  
		Size: 207.2 KB (207237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b259955a7b787ff533a05f42050e5172ba829db902cac41506236e30a45be04e`  
		Last Modified: Wed, 30 Mar 2022 01:03:38 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29db0547b8fb18568f5c6616a8622211952741a2a93da0e86cb506b1ee4c941c`  
		Last Modified: Wed, 30 Mar 2022 01:03:39 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.2-alpine` - linux; 386

```console
$ docker pull spiped@sha256:dcbb93128deb3206337ac10573e41e27b4a95816cd3f931412c655201fef2396
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.1 MB (3053817 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fdb9526919356b65e45d7bc9a9bd2aaddd7da8a1e62f023b9511a320a431df64`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Mon, 04 Apr 2022 23:38:25 GMT
ADD file:7d51a0f8691eb78c9062fd31984423a93d276a67b4ed5d1a706e1c2cd9fea23a in / 
# Mon, 04 Apr 2022 23:38:25 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 06:51:23 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Tue, 05 Apr 2022 06:51:24 GMT
RUN apk add --no-cache libssl1.1
# Tue, 05 Apr 2022 06:51:24 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 05 Apr 2022 06:51:34 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Tue, 05 Apr 2022 06:51:35 GMT
VOLUME [/spiped]
# Tue, 05 Apr 2022 06:51:36 GMT
WORKDIR /spiped
# Tue, 05 Apr 2022 06:51:38 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 05 Apr 2022 06:51:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 05 Apr 2022 06:51:39 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:73b28a5955ec7fb46f2cf0434e4901a889f7dda3f8c9ec496300feb256c7eda8`  
		Last Modified: Mon, 04 Apr 2022 19:10:03 GMT  
		Size: 2.8 MB (2818974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5043c44edf55100d2df153f657912b53abf987ef0c6286b113dcef298998f359`  
		Last Modified: Tue, 05 Apr 2022 06:52:09 GMT  
		Size: 1.2 KB (1240 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfc9d36e654ea336dd74dc00574768a6502edd5ef5cd785b695e516f6254be55`  
		Last Modified: Tue, 05 Apr 2022 06:52:08 GMT  
		Size: 7.8 KB (7750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0401735f1a5cdc5a0248a778049579b8858a6f7cc0fc6fdcdaea211930d4a386`  
		Last Modified: Tue, 05 Apr 2022 06:52:08 GMT  
		Size: 225.4 KB (225416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5a85e3f263e110e3fa50aada2a3ca6314a5a6e67e8f211881a826585a5db409`  
		Last Modified: Tue, 05 Apr 2022 06:52:08 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a0f113efbe13d3511b57cb0428e99f2725a51cb3980e75b1f1be3fc0d715b19`  
		Last Modified: Tue, 05 Apr 2022 06:52:08 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.2-alpine` - linux; ppc64le

```console
$ docker pull spiped@sha256:d27c5eb0ad348fe2a50b65e808e4b825f0f479572187d81757b9a82ce2ad9e50
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (3033662 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1853309ab0785a26d0b48053b424c5b8c4ffd6367504032c68e3377b9fc92eba`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 29 Mar 2022 00:16:52 GMT
ADD file:9e7b65a431d59070abaadae56d9c3fc59c899af881939e4353b1f524b2bd5185 in / 
# Tue, 29 Mar 2022 00:16:55 GMT
CMD ["/bin/sh"]
# Wed, 30 Mar 2022 05:25:40 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Wed, 30 Mar 2022 05:25:50 GMT
RUN apk add --no-cache libssl1.1
# Wed, 30 Mar 2022 05:25:53 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 30 Mar 2022 05:26:20 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Wed, 30 Mar 2022 05:26:24 GMT
VOLUME [/spiped]
# Wed, 30 Mar 2022 05:26:28 GMT
WORKDIR /spiped
# Wed, 30 Mar 2022 05:26:35 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 30 Mar 2022 05:26:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 30 Mar 2022 05:26:46 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:1c611bca4fa49cac5bc1e3826ad53fee85ed659d24bffcccd86c3f04be07339a`  
		Last Modified: Tue, 29 Mar 2022 00:18:26 GMT  
		Size: 2.8 MB (2811009 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b61e9d70cfabe50a7554945008b067920fffa673936b1b8c50f29cdbc07fad93`  
		Last Modified: Wed, 30 Mar 2022 05:27:51 GMT  
		Size: 1.3 KB (1263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd9a458bb0005f54d005e938aa01a6aeeb1d7c48486de6811d1c16a9846b1239`  
		Last Modified: Wed, 30 Mar 2022 05:27:51 GMT  
		Size: 7.8 KB (7774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be8c858ba1f6886855b0312ec6b3618c916bea4577c858d028e6709d67f05939`  
		Last Modified: Wed, 30 Mar 2022 05:27:51 GMT  
		Size: 213.1 KB (213149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1d4e4cb20d1bd858c134eae12aac2cab24001fbae386ee7f84b1e8dc6c6ef76`  
		Last Modified: Wed, 30 Mar 2022 05:27:51 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20cb5033835d271b66d87c37a113ae41ee09c6b1c5b462196462cb06687e3352`  
		Last Modified: Wed, 30 Mar 2022 05:27:51 GMT  
		Size: 338.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.2-alpine` - linux; s390x

```console
$ docker pull spiped@sha256:851d4d1e8b82de6d455e9a562bd6b75539fe737213c9f3cf01ce7b44e11abeb4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 MB (2811594 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e240f56e6000d053b4d3e20632b54b88daaa8dad76ecda720ce9f76c82bfe394`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Mon, 04 Apr 2022 23:41:39 GMT
ADD file:f22e4b2be87d3c59c8c609acf79015938dc1fba0b26d7c1b59bd0fc36d63a906 in / 
# Mon, 04 Apr 2022 23:41:39 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 06:09:44 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Tue, 05 Apr 2022 06:09:45 GMT
RUN apk add --no-cache libssl1.1
# Tue, 05 Apr 2022 06:09:45 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 05 Apr 2022 06:09:50 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Tue, 05 Apr 2022 06:09:50 GMT
VOLUME [/spiped]
# Tue, 05 Apr 2022 06:09:51 GMT
WORKDIR /spiped
# Tue, 05 Apr 2022 06:09:51 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 05 Apr 2022 06:09:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 05 Apr 2022 06:09:51 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:a27b630f446c3da376a30cf610e4bfa6847f8b87c83702c29e72b986f4e52d28`  
		Last Modified: Mon, 04 Apr 2022 23:42:37 GMT  
		Size: 2.6 MB (2600375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ffc8ec477cbe2d575e99a9232e9328db8cc40109dbe067d93c2033302576850`  
		Last Modified: Tue, 05 Apr 2022 06:10:22 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ee008c7ec71319091cda7b7cbf1063414ee758f739581409a2e7089e90882c9`  
		Last Modified: Tue, 05 Apr 2022 06:10:21 GMT  
		Size: 7.8 KB (7788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3edcb5212f084eabfd1bad6e332d8b53bd7756099c4da3e410ee23f869a701b`  
		Last Modified: Tue, 05 Apr 2022 06:10:21 GMT  
		Size: 201.7 KB (201693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd099e1efb05ce5fa06c5e18ba7d057b5df318c462022f1ac443f45e86fdc809`  
		Last Modified: Tue, 05 Apr 2022 06:10:21 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afbab95e29c022d6828d869e5e4442b139373571c747f8fc6470b8bd257337a4`  
		Last Modified: Tue, 05 Apr 2022 06:10:21 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:alpine`

```console
$ docker pull spiped@sha256:df67424ae1b5f50fe62e3c8f7584a176cef62ba9d479ccd376f70587ae42ca61
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
$ docker pull spiped@sha256:b1000f43786f16a20a805fa353f6e29da279735ce16fc397001fde0e351cadab
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (3038963 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:319549bf17a1c296f365e261889f2573a629fda0ca36fa2dac3efc79c233dc4d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 05 Apr 2022 00:19:59 GMT
ADD file:5d673d25da3a14ce1f6cf66e4c7fd4f4b85a3759a9d93efb3fd9ff852b5b56e4 in / 
# Tue, 05 Apr 2022 00:19:59 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 09:41:12 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Tue, 05 Apr 2022 09:41:13 GMT
RUN apk add --no-cache libssl1.1
# Tue, 05 Apr 2022 09:41:13 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 05 Apr 2022 09:41:22 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Tue, 05 Apr 2022 09:41:22 GMT
VOLUME [/spiped]
# Tue, 05 Apr 2022 09:41:23 GMT
WORKDIR /spiped
# Tue, 05 Apr 2022 09:41:23 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 05 Apr 2022 09:41:23 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 05 Apr 2022 09:41:23 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:df9b9388f04ad6279a7410b85cedfdcb2208c0a003da7ab5613af71079148139`  
		Last Modified: Mon, 04 Apr 2022 19:10:16 GMT  
		Size: 2.8 MB (2814559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:735044c06e8b73c2bb88467804d54b359bfc8226cf975772cc666adc9f029f5c`  
		Last Modified: Tue, 05 Apr 2022 09:41:38 GMT  
		Size: 1.3 KB (1271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd8b16fcaec70a3de42b4e850be4a851eaffa96a04fb49668b0d55b15bdf9675`  
		Last Modified: Tue, 05 Apr 2022 09:41:38 GMT  
		Size: 7.8 KB (7783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79236b25532d68c328b81af71a0f8c4eca102b7030a98d650ffc9a7e35d113be`  
		Last Modified: Tue, 05 Apr 2022 09:41:38 GMT  
		Size: 214.9 KB (214880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f429bef29fed68fb012179a10893c62fd5167934a7d62e7d3db15361601d47e9`  
		Last Modified: Tue, 05 Apr 2022 09:41:38 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1703108ce26f514d42179cf03051a6082b57e184d89f7bab08377819025c74d9`  
		Last Modified: Tue, 05 Apr 2022 09:41:38 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; arm variant v6

```console
$ docker pull spiped@sha256:ae66fb10272b529530524084a214a11e65777dff6517d5a90d71357e60416246
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 MB (2830615 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aae9a0570520cf722d24d3a84685d936a04a06d1b8e35de44be52daca29219ea`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 29 Mar 2022 00:49:32 GMT
ADD file:44acf536d487bec7f7bf16561f4ec90e60d4447b3cbabfeca66953c4491aabeb in / 
# Tue, 29 Mar 2022 00:49:33 GMT
CMD ["/bin/sh"]
# Tue, 29 Mar 2022 08:24:39 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Tue, 29 Mar 2022 08:24:41 GMT
RUN apk add --no-cache libssl1.1
# Tue, 29 Mar 2022 08:24:41 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 29 Mar 2022 08:25:01 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Tue, 29 Mar 2022 08:25:01 GMT
VOLUME [/spiped]
# Tue, 29 Mar 2022 08:25:02 GMT
WORKDIR /spiped
# Tue, 29 Mar 2022 08:25:03 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 29 Mar 2022 08:25:03 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 29 Mar 2022 08:25:04 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:84f033dabe5013c0dfae4263abd951011719d0a15adc3c7312c5be994deff030`  
		Last Modified: Tue, 29 Mar 2022 00:51:25 GMT  
		Size: 2.6 MB (2621943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdc4ea1012b3262fa7706463586c4d41a0cf0a329238cbe52ea6d03bfbc07fae`  
		Last Modified: Tue, 29 Mar 2022 08:25:35 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5659ae5d68adc8e4012f07c665ea352c4068ee821e83350f8bc165b6aea5583`  
		Last Modified: Tue, 29 Mar 2022 08:25:35 GMT  
		Size: 7.8 KB (7774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bf4925cebf49f63997a8c7389e423c3623dc4cd2e6c701e4282c664293e789b`  
		Last Modified: Tue, 29 Mar 2022 08:25:35 GMT  
		Size: 199.2 KB (199158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6eac1b140b33266f585c96310939c5cdbac7bde1fcbc0bd4e8cde9f9f0dd5171`  
		Last Modified: Tue, 29 Mar 2022 08:25:35 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11b13e602bdbc874391ee6aee0f8abffe1e74ee57061d9e1faed46aa76ad44a0`  
		Last Modified: Tue, 29 Mar 2022 08:25:35 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; arm variant v7

```console
$ docker pull spiped@sha256:1533669bdce5be15027cb96650fabea206274558c0195f437de5245079d89f0f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 MB (2626515 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:52a32db31d94e7ea2f1af7b835d809d1b42c16deff1071fe4b3f2e720bc3688c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 29 Mar 2022 02:13:28 GMT
ADD file:8c959b80e3661beea7b3468017b88897d981bf52ed43c074e7c87ecb753e9059 in / 
# Tue, 29 Mar 2022 02:13:28 GMT
CMD ["/bin/sh"]
# Wed, 30 Mar 2022 16:38:17 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Wed, 30 Mar 2022 16:38:19 GMT
RUN apk add --no-cache libssl1.1
# Wed, 30 Mar 2022 16:38:20 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 30 Mar 2022 16:38:38 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Wed, 30 Mar 2022 16:38:38 GMT
VOLUME [/spiped]
# Wed, 30 Mar 2022 16:38:39 GMT
WORKDIR /spiped
# Wed, 30 Mar 2022 16:38:40 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 30 Mar 2022 16:38:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 30 Mar 2022 16:38:40 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:22b1e5a07a97d7af6fdc335e3b3a975b73908fa19b084289c408a00814da0398`  
		Last Modified: Tue, 29 Mar 2022 02:15:28 GMT  
		Size: 2.4 MB (2424303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1b864dcb6ac61a275d83b41f5e533000faf52fae810b4fc0513796337285828`  
		Last Modified: Wed, 30 Mar 2022 16:39:51 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3aed778a3d8f2984cc57d3cbd49d0974e4d48f31a548da40051a676285fcb98`  
		Last Modified: Wed, 30 Mar 2022 16:39:51 GMT  
		Size: 7.8 KB (7781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23bc58fbe93b76dec15870d5507d4377afa5e3cd4e9ddd68e1117ed5fb9b1953`  
		Last Modified: Wed, 30 Mar 2022 16:39:52 GMT  
		Size: 192.7 KB (192691 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1f1a66e69919430ccc221d6a8b42a90a4ebdee7a41b426b4cabbd472c3d62a3`  
		Last Modified: Wed, 30 Mar 2022 16:39:51 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6342a8067391971e5056968d5d26841d53aeaab30109c42bb6c53a227f694cab`  
		Last Modified: Wed, 30 Mar 2022 16:39:51 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:c0d28956af21c9ad7d0e3d4cf972b301ea28efa0c8755d1ee62841b09754b0ab
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 MB (2933013 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a11675ed63f0f0f4c5e2d5175c06bade440268d204f7a4b104eba50db3f998da`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 29 Mar 2022 00:40:05 GMT
ADD file:24e8b04304ef91bbf949674909ccaf2c66e3dcd096c3c307a0510569eadf576f in / 
# Tue, 29 Mar 2022 00:40:05 GMT
CMD ["/bin/sh"]
# Wed, 30 Mar 2022 01:02:13 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Wed, 30 Mar 2022 01:02:15 GMT
RUN apk add --no-cache libssl1.1
# Wed, 30 Mar 2022 01:02:16 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 30 Mar 2022 01:02:34 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Wed, 30 Mar 2022 01:02:35 GMT
VOLUME [/spiped]
# Wed, 30 Mar 2022 01:02:36 GMT
WORKDIR /spiped
# Wed, 30 Mar 2022 01:02:38 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 30 Mar 2022 01:02:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 30 Mar 2022 01:02:39 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:80fa7f07ec7b717ec5f8e2717b91e3d659e129052ec3def2570a5674322688d9`  
		Last Modified: Tue, 29 Mar 2022 00:41:08 GMT  
		Size: 2.7 MB (2716347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ef7ee2c7f3dc7bcaf9752a844248d8127145ffd675ae5de72b4be177fc37cd5`  
		Last Modified: Wed, 30 Mar 2022 01:03:39 GMT  
		Size: 1.2 KB (1240 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47c53830f06d1a108ac255dbff68c71fabc58723d0a42943fec7681cbebe653a`  
		Last Modified: Wed, 30 Mar 2022 01:03:38 GMT  
		Size: 7.8 KB (7751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e1f94f19caf7b781c37e261530b5861447ecd5ab33d55ad4d2f12a932db1cf8`  
		Last Modified: Wed, 30 Mar 2022 01:03:39 GMT  
		Size: 207.2 KB (207237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b259955a7b787ff533a05f42050e5172ba829db902cac41506236e30a45be04e`  
		Last Modified: Wed, 30 Mar 2022 01:03:38 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29db0547b8fb18568f5c6616a8622211952741a2a93da0e86cb506b1ee4c941c`  
		Last Modified: Wed, 30 Mar 2022 01:03:39 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; 386

```console
$ docker pull spiped@sha256:dcbb93128deb3206337ac10573e41e27b4a95816cd3f931412c655201fef2396
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.1 MB (3053817 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fdb9526919356b65e45d7bc9a9bd2aaddd7da8a1e62f023b9511a320a431df64`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Mon, 04 Apr 2022 23:38:25 GMT
ADD file:7d51a0f8691eb78c9062fd31984423a93d276a67b4ed5d1a706e1c2cd9fea23a in / 
# Mon, 04 Apr 2022 23:38:25 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 06:51:23 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Tue, 05 Apr 2022 06:51:24 GMT
RUN apk add --no-cache libssl1.1
# Tue, 05 Apr 2022 06:51:24 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 05 Apr 2022 06:51:34 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Tue, 05 Apr 2022 06:51:35 GMT
VOLUME [/spiped]
# Tue, 05 Apr 2022 06:51:36 GMT
WORKDIR /spiped
# Tue, 05 Apr 2022 06:51:38 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 05 Apr 2022 06:51:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 05 Apr 2022 06:51:39 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:73b28a5955ec7fb46f2cf0434e4901a889f7dda3f8c9ec496300feb256c7eda8`  
		Last Modified: Mon, 04 Apr 2022 19:10:03 GMT  
		Size: 2.8 MB (2818974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5043c44edf55100d2df153f657912b53abf987ef0c6286b113dcef298998f359`  
		Last Modified: Tue, 05 Apr 2022 06:52:09 GMT  
		Size: 1.2 KB (1240 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfc9d36e654ea336dd74dc00574768a6502edd5ef5cd785b695e516f6254be55`  
		Last Modified: Tue, 05 Apr 2022 06:52:08 GMT  
		Size: 7.8 KB (7750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0401735f1a5cdc5a0248a778049579b8858a6f7cc0fc6fdcdaea211930d4a386`  
		Last Modified: Tue, 05 Apr 2022 06:52:08 GMT  
		Size: 225.4 KB (225416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5a85e3f263e110e3fa50aada2a3ca6314a5a6e67e8f211881a826585a5db409`  
		Last Modified: Tue, 05 Apr 2022 06:52:08 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a0f113efbe13d3511b57cb0428e99f2725a51cb3980e75b1f1be3fc0d715b19`  
		Last Modified: Tue, 05 Apr 2022 06:52:08 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; ppc64le

```console
$ docker pull spiped@sha256:d27c5eb0ad348fe2a50b65e808e4b825f0f479572187d81757b9a82ce2ad9e50
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (3033662 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1853309ab0785a26d0b48053b424c5b8c4ffd6367504032c68e3377b9fc92eba`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 29 Mar 2022 00:16:52 GMT
ADD file:9e7b65a431d59070abaadae56d9c3fc59c899af881939e4353b1f524b2bd5185 in / 
# Tue, 29 Mar 2022 00:16:55 GMT
CMD ["/bin/sh"]
# Wed, 30 Mar 2022 05:25:40 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Wed, 30 Mar 2022 05:25:50 GMT
RUN apk add --no-cache libssl1.1
# Wed, 30 Mar 2022 05:25:53 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 30 Mar 2022 05:26:20 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Wed, 30 Mar 2022 05:26:24 GMT
VOLUME [/spiped]
# Wed, 30 Mar 2022 05:26:28 GMT
WORKDIR /spiped
# Wed, 30 Mar 2022 05:26:35 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 30 Mar 2022 05:26:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 30 Mar 2022 05:26:46 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:1c611bca4fa49cac5bc1e3826ad53fee85ed659d24bffcccd86c3f04be07339a`  
		Last Modified: Tue, 29 Mar 2022 00:18:26 GMT  
		Size: 2.8 MB (2811009 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b61e9d70cfabe50a7554945008b067920fffa673936b1b8c50f29cdbc07fad93`  
		Last Modified: Wed, 30 Mar 2022 05:27:51 GMT  
		Size: 1.3 KB (1263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd9a458bb0005f54d005e938aa01a6aeeb1d7c48486de6811d1c16a9846b1239`  
		Last Modified: Wed, 30 Mar 2022 05:27:51 GMT  
		Size: 7.8 KB (7774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be8c858ba1f6886855b0312ec6b3618c916bea4577c858d028e6709d67f05939`  
		Last Modified: Wed, 30 Mar 2022 05:27:51 GMT  
		Size: 213.1 KB (213149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1d4e4cb20d1bd858c134eae12aac2cab24001fbae386ee7f84b1e8dc6c6ef76`  
		Last Modified: Wed, 30 Mar 2022 05:27:51 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20cb5033835d271b66d87c37a113ae41ee09c6b1c5b462196462cb06687e3352`  
		Last Modified: Wed, 30 Mar 2022 05:27:51 GMT  
		Size: 338.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; s390x

```console
$ docker pull spiped@sha256:851d4d1e8b82de6d455e9a562bd6b75539fe737213c9f3cf01ce7b44e11abeb4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 MB (2811594 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e240f56e6000d053b4d3e20632b54b88daaa8dad76ecda720ce9f76c82bfe394`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Mon, 04 Apr 2022 23:41:39 GMT
ADD file:f22e4b2be87d3c59c8c609acf79015938dc1fba0b26d7c1b59bd0fc36d63a906 in / 
# Mon, 04 Apr 2022 23:41:39 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 06:09:44 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Tue, 05 Apr 2022 06:09:45 GMT
RUN apk add --no-cache libssl1.1
# Tue, 05 Apr 2022 06:09:45 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 05 Apr 2022 06:09:50 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Tue, 05 Apr 2022 06:09:50 GMT
VOLUME [/spiped]
# Tue, 05 Apr 2022 06:09:51 GMT
WORKDIR /spiped
# Tue, 05 Apr 2022 06:09:51 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 05 Apr 2022 06:09:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 05 Apr 2022 06:09:51 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:a27b630f446c3da376a30cf610e4bfa6847f8b87c83702c29e72b986f4e52d28`  
		Last Modified: Mon, 04 Apr 2022 23:42:37 GMT  
		Size: 2.6 MB (2600375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ffc8ec477cbe2d575e99a9232e9328db8cc40109dbe067d93c2033302576850`  
		Last Modified: Tue, 05 Apr 2022 06:10:22 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ee008c7ec71319091cda7b7cbf1063414ee758f739581409a2e7089e90882c9`  
		Last Modified: Tue, 05 Apr 2022 06:10:21 GMT  
		Size: 7.8 KB (7788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3edcb5212f084eabfd1bad6e332d8b53bd7756099c4da3e410ee23f869a701b`  
		Last Modified: Tue, 05 Apr 2022 06:10:21 GMT  
		Size: 201.7 KB (201693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd099e1efb05ce5fa06c5e18ba7d057b5df318c462022f1ac443f45e86fdc809`  
		Last Modified: Tue, 05 Apr 2022 06:10:21 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afbab95e29c022d6828d869e5e4442b139373571c747f8fc6470b8bd257337a4`  
		Last Modified: Tue, 05 Apr 2022 06:10:21 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:latest`

```console
$ docker pull spiped@sha256:1096e8cf1ee57825fa381a290095d3d42ebddf1e22f54edb53f96109d8466d0d
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
$ docker pull spiped@sha256:f236fca971a0526aa22ab4aa69709d302210d7e1f5bd42902bde2803ec0495bd
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.3 MB (37348627 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0ab54c336e542bbe2bacf29196b05876f18889ca6f79cd1c223af52a9bcf3241`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 29 Mar 2022 00:22:18 GMT
ADD file:966d3669b40f5fbaecee1ecbeb58debe19001076da5d94717080d55efbc25971 in / 
# Tue, 29 Mar 2022 00:22:19 GMT
CMD ["bash"]
# Tue, 29 Mar 2022 12:05:44 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 29 Mar 2022 12:05:47 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 29 Mar 2022 12:05:47 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 29 Mar 2022 12:06:06 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 29 Mar 2022 12:06:07 GMT
VOLUME [/spiped]
# Tue, 29 Mar 2022 12:06:07 GMT
WORKDIR /spiped
# Tue, 29 Mar 2022 12:06:07 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 29 Mar 2022 12:06:07 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 29 Mar 2022 12:06:07 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:c229119241af7b23b121052a1cae4c03e0a477a72ea6a7f463ad7623ff8f274b`  
		Last Modified: Tue, 29 Mar 2022 00:27:16 GMT  
		Size: 31.4 MB (31378457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fda024001dd8419f652d3fde717d37b32c648032cc3f92d00978db9268a65b97`  
		Last Modified: Tue, 29 Mar 2022 12:06:37 GMT  
		Size: 1.7 KB (1736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b55c823e9d54047194e3c5cef477607293ed02e6d1b77f8f6f834f50fe2e9d05`  
		Last Modified: Tue, 29 Mar 2022 12:06:37 GMT  
		Size: 1.1 KB (1052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55ae1339c87c4e759ff4a439ee8561a8481ea3131678ac5e2f58795506cb67fc`  
		Last Modified: Tue, 29 Mar 2022 12:06:38 GMT  
		Size: 6.0 MB (5966913 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eda9f112e9f42cfee9c6890693553b623bf2dd540c36f29ad14276acb22e044e`  
		Last Modified: Tue, 29 Mar 2022 12:06:37 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad6ba00100ccbdece1902154d0d0d33ee3d70d4e184a6524a97b6ab7e2e53192`  
		Last Modified: Tue, 29 Mar 2022 12:06:37 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; arm variant v5

```console
$ docker pull spiped@sha256:94736a8efc0da3dd2c4c38b0a356b70873aee616c541dbccdfa95068dc6c0cb6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.0 MB (33951476 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cfb46d52c65a3d3391adc84884f180419a0f9437774a897d2ba90ecff46cb1cb`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 29 Mar 2022 00:50:37 GMT
ADD file:6b9a30e6ef50a46e87cf9d7f5a491c7951fdb6dd6fab3c9d4a9c3c40f92b8db4 in / 
# Tue, 29 Mar 2022 00:50:38 GMT
CMD ["bash"]
# Wed, 30 Mar 2022 01:08:33 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 30 Mar 2022 01:08:43 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 30 Mar 2022 01:08:43 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 30 Mar 2022 01:09:31 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 30 Mar 2022 01:09:32 GMT
VOLUME [/spiped]
# Wed, 30 Mar 2022 01:09:32 GMT
WORKDIR /spiped
# Wed, 30 Mar 2022 01:09:33 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 30 Mar 2022 01:09:33 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 30 Mar 2022 01:09:34 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:9a41aba0a099ec129c20f41f6370b97daa4c3d4d3edc76ea1863bc5f76f9e5e5`  
		Last Modified: Tue, 29 Mar 2022 01:05:21 GMT  
		Size: 28.9 MB (28920513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afcd77f21f54e947717641dc9eb4a3c32a321dd3df6f615e082da0d916f9c6ca`  
		Last Modified: Wed, 30 Mar 2022 01:10:09 GMT  
		Size: 1.7 KB (1729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96e6a8e69828bdad8405be855d17ef3331b8093c3773b6a6ed726e8788cc3fe1`  
		Last Modified: Wed, 30 Mar 2022 01:10:09 GMT  
		Size: 1.1 KB (1053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e672a3f91acf51a5b4252fc7a5e23c4bd9539029d819fafe90af13149b18a97`  
		Last Modified: Wed, 30 Mar 2022 01:10:12 GMT  
		Size: 5.0 MB (5027710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11475c4da412af9a0208f5a0962e32a7bd674a732fc2cb1bd58a16deb9aac2e4`  
		Last Modified: Wed, 30 Mar 2022 01:10:09 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2adba7e3a404697c9d1e15fe08cfbb357d8dd16b877a299ca347781afd782675`  
		Last Modified: Wed, 30 Mar 2022 01:10:09 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; arm variant v7

```console
$ docker pull spiped@sha256:2dbc8de74b30a303a09ce36ac401dbbc2edd6a659c643579a43d0243250acd0b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.3 MB (31326537 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:04bbd512c51b4df932d3725ab91fe61a2eecb9b729392297a9634c096f37e9aa`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 29 Mar 2022 02:18:34 GMT
ADD file:e1835d1a0c70a0335757f211893e5d12ddf797e489e10434c0982bdf9b234f67 in / 
# Tue, 29 Mar 2022 02:18:36 GMT
CMD ["bash"]
# Wed, 30 Mar 2022 16:37:08 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 30 Mar 2022 16:37:15 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 30 Mar 2022 16:37:16 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 30 Mar 2022 16:38:00 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 30 Mar 2022 16:38:01 GMT
VOLUME [/spiped]
# Wed, 30 Mar 2022 16:38:01 GMT
WORKDIR /spiped
# Wed, 30 Mar 2022 16:38:02 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 30 Mar 2022 16:38:02 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 30 Mar 2022 16:38:03 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:f98812e1a494a683a5b3dea593dd2ef305f5f732193044c147f22e44b00164bc`  
		Last Modified: Tue, 29 Mar 2022 02:34:13 GMT  
		Size: 26.6 MB (26575370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b566a0eb6f50a4d3076e96e1230218651c8e3409f1e36b78720641ddcf02fe67`  
		Last Modified: Wed, 30 Mar 2022 16:39:28 GMT  
		Size: 1.7 KB (1730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3653f9517ce7a66aa5b26388c993e6803d010dd10becbc1141166b19d0575c20`  
		Last Modified: Wed, 30 Mar 2022 16:39:28 GMT  
		Size: 1.1 KB (1055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bef73e1c106acd2821aea52e999a0ab3dc8a102d38cf18f931ff036fc5cdde29`  
		Last Modified: Wed, 30 Mar 2022 16:39:32 GMT  
		Size: 4.7 MB (4747910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1eb71618098b05bae1eef477c77b1abb4846fb9cb147e36318ec26d12542a9db`  
		Last Modified: Wed, 30 Mar 2022 16:39:28 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4742b0162d23f2f2a3f504f4d0eded391b6c812f26030eca3f9137563d7d44fc`  
		Last Modified: Wed, 30 Mar 2022 16:39:28 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:489251bdbc8f5a1d43cb461dba8917af4fb58142240f15e7d2c7c31f7d859b2b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.3 MB (35337814 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bead5c7928697f7d3aded01a859186f595bedcb48737aebb29d40d92c78230e5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 29 Mar 2022 00:43:17 GMT
ADD file:e95289cd39de0f389d09cda9edf8476d5da371bc68d76e820c5e1c310dc54baf in / 
# Tue, 29 Mar 2022 00:43:17 GMT
CMD ["bash"]
# Wed, 30 Mar 2022 01:01:29 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 30 Mar 2022 01:01:33 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 30 Mar 2022 01:01:34 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 30 Mar 2022 01:01:58 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 30 Mar 2022 01:01:58 GMT
VOLUME [/spiped]
# Wed, 30 Mar 2022 01:01:59 GMT
WORKDIR /spiped
# Wed, 30 Mar 2022 01:02:01 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 30 Mar 2022 01:02:01 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 30 Mar 2022 01:02:02 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:2203022c5aa978ec114a15a7cdc2c323c65922d3b0a8eab11d50811bb9ae1cfb`  
		Last Modified: Tue, 29 Mar 2022 00:50:04 GMT  
		Size: 30.1 MB (30064311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c1c5ff6bd12cad4539ef42aba72b9e2a79fd5e03cf703d178e9179cf3ca28d3`  
		Last Modified: Wed, 30 Mar 2022 01:03:05 GMT  
		Size: 1.6 KB (1619 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d32807b7cfbcaf6c5dda896ed26a7d5b103161f8237a6f762874f9d2e713509`  
		Last Modified: Wed, 30 Mar 2022 01:03:04 GMT  
		Size: 923.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbc810f776215aefbbbcac36475250c8768eea0d0fdb5cdeceb3a2ed84c8dbb8`  
		Last Modified: Wed, 30 Mar 2022 01:03:06 GMT  
		Size: 5.3 MB (5270525 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d1419d96420314f5d538869ef6bf4d3e349c952c254f754fba1e39a0ba1a36c`  
		Last Modified: Wed, 30 Mar 2022 01:03:04 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:533163ce32b9d79dc658ade7a26d7f71cece5b9bf114cc7b7dc3596ba66609ba`  
		Last Modified: Wed, 30 Mar 2022 01:03:04 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; 386

```console
$ docker pull spiped@sha256:7bf4cc6d7160264b61ad5339a1b254c94c216125bf624adbb4a44b1a484a71b1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.3 MB (40283723 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e193db912bc32b089a793405a8541f1cb6d938b1dad5dc81b749bdb791619efa`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 29 Mar 2022 00:42:01 GMT
ADD file:d093057c080a13cc4370d0e786857751004b8cd3c93368742512abbee4f1de83 in / 
# Tue, 29 Mar 2022 00:42:01 GMT
CMD ["bash"]
# Tue, 29 Mar 2022 10:43:59 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 29 Mar 2022 10:44:03 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 29 Mar 2022 10:44:04 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 29 Mar 2022 10:44:24 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 29 Mar 2022 10:44:25 GMT
VOLUME [/spiped]
# Tue, 29 Mar 2022 10:44:26 GMT
WORKDIR /spiped
# Tue, 29 Mar 2022 10:44:28 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 29 Mar 2022 10:44:28 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 29 Mar 2022 10:44:29 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:fec59da75229f638ca2878278d3859a1a8b73a20d5c0c043354eb37129ebb8bf`  
		Last Modified: Tue, 29 Mar 2022 00:49:10 GMT  
		Size: 32.4 MB (32389518 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:559c323dcf632c3e6c78229ea96b201cd5c6a73598a208ba2fd88a55a2e53f6a`  
		Last Modified: Tue, 29 Mar 2022 10:45:19 GMT  
		Size: 1.6 KB (1611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7b0c52bcbc80dacdfd452f5135ca2e640ab57050b38fbf5890ca41339ce8cbf`  
		Last Modified: Tue, 29 Mar 2022 10:45:19 GMT  
		Size: 924.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0e273d1baff760d787e4bf5a3e20801cf5a8e2625eada853a4d7cdd86c1e25f`  
		Last Modified: Tue, 29 Mar 2022 10:45:20 GMT  
		Size: 7.9 MB (7891233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd7f99497ff10c89ef5d937c4f127f94bcc0391017c3fa45d587bab079706dea`  
		Last Modified: Tue, 29 Mar 2022 10:45:19 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61bb3d200b36c323a0edaaa6ceb5990790f17562ef9d5e5c63d7fab6d1978d51`  
		Last Modified: Tue, 29 Mar 2022 10:45:19 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; mips64le

```console
$ docker pull spiped@sha256:616f8531e23b941b90c8d1293b641771b4c758475fff50f5f6f50bdceae91f2c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.3 MB (35349463 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e57ad4c68f94212319101e900c6737ad74d321485f03cf0cf7522b7259c35ac0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 29 Mar 2022 07:42:27 GMT
ADD file:32aa9fd7ee5c64e4bd49459e801e3e5dc50138590bbfca671e336a197aa7fa92 in / 
# Tue, 29 Mar 2022 07:42:31 GMT
CMD ["bash"]
# Wed, 30 Mar 2022 05:36:13 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 30 Mar 2022 05:36:28 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 30 Mar 2022 05:36:31 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 30 Mar 2022 05:38:04 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 30 Mar 2022 05:38:06 GMT
VOLUME [/spiped]
# Wed, 30 Mar 2022 05:38:09 GMT
WORKDIR /spiped
# Wed, 30 Mar 2022 05:38:12 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 30 Mar 2022 05:38:14 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 30 Mar 2022 05:38:17 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:5c2a8045f9de06328ab3d0ff505d990892219b7faee393bc9ac342347fc83d04`  
		Last Modified: Tue, 29 Mar 2022 07:52:59 GMT  
		Size: 29.6 MB (29641474 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28d11336cbfa9f2c1e6c22eef2096c37397f6a0058407687dc007bf7384a3e79`  
		Last Modified: Wed, 30 Mar 2022 05:38:29 GMT  
		Size: 1.6 KB (1629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd53cadc47175f65d5df3546949d7f0a90aec5d75b5fe538a9a9b4fe2ebeefd2`  
		Last Modified: Wed, 30 Mar 2022 05:38:29 GMT  
		Size: 924.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcdf8956bed67848aaf6e2f1456d79a9db2efc0f6986df8eb00feb2d30de9389`  
		Last Modified: Wed, 30 Mar 2022 05:38:34 GMT  
		Size: 5.7 MB (5704999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6a3ca7ecd16ef5159abf00ec43e34fbe1b528c2416e3b0eb94806b1d5445e5d`  
		Last Modified: Wed, 30 Mar 2022 05:38:29 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:109d3b9867a03e8499cbf83271d977a1bbf8550acb992fce7348de6047db039f`  
		Last Modified: Wed, 30 Mar 2022 05:38:29 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; ppc64le

```console
$ docker pull spiped@sha256:20cc9df235f7239597ba6e9f0da45b8a2476c6020795502aa68f0b7275799a6d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.3 MB (41284580 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a9d0a0f307401e56e3c154076006ae5b0585b5124c0ad643d5fc5305effea55c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 29 Mar 2022 00:22:08 GMT
ADD file:e7ae113c10f322a9cffc46b62ba12820e270caaadaee3c5b907c801a37e1632c in / 
# Tue, 29 Mar 2022 00:22:11 GMT
CMD ["bash"]
# Wed, 30 Mar 2022 05:21:11 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 30 Mar 2022 05:21:26 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 30 Mar 2022 05:21:30 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 30 Mar 2022 05:24:47 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 30 Mar 2022 05:24:55 GMT
VOLUME [/spiped]
# Wed, 30 Mar 2022 05:25:01 GMT
WORKDIR /spiped
# Wed, 30 Mar 2022 05:25:04 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 30 Mar 2022 05:25:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 30 Mar 2022 05:25:15 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:ecc74bb8af5a048e1123af0e17d88ef3da1d10951ada79e8e1cc9c0a694245d3`  
		Last Modified: Tue, 29 Mar 2022 00:32:57 GMT  
		Size: 35.3 MB (35282506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89e50c6a3f6bfe8c939d3f4cf697d6972444715b3e29bbe8ba3a8503b2d47744`  
		Last Modified: Wed, 30 Mar 2022 05:27:29 GMT  
		Size: 1.7 KB (1748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06d13b3a37c65e9f1e8f7d06ea8947895095e24e8766405225cfb8a7a68897fd`  
		Last Modified: Wed, 30 Mar 2022 05:27:29 GMT  
		Size: 1.1 KB (1056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bf7cfaec929baf5dd2ec1c286ff49084391ed126f695c76cc847467adb4b808`  
		Last Modified: Wed, 30 Mar 2022 05:27:31 GMT  
		Size: 6.0 MB (5998799 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0d18fb763428d4908c4dccb28dd79a1ef28deee5b1869dd026f99019b274d04`  
		Last Modified: Wed, 30 Mar 2022 05:27:29 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17b9492405cf9ecc040958db5b6363eb0b2a3fb3a3113526b3c94ebbe352ec9c`  
		Last Modified: Wed, 30 Mar 2022 05:27:29 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; s390x

```console
$ docker pull spiped@sha256:bc909d5eeee60c7823173755c87467307f944145474e127199afc7d15643b99c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.8 MB (34845094 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2c0bcec57634c726f934b24b28bf162da99aacbf72dd089108346ddd627e4284`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 29 Mar 2022 00:51:57 GMT
ADD file:39c5e0d7a686abd19448ab3e6237d50955ae2187fc2b64289a08c2549352b8f1 in / 
# Tue, 29 Mar 2022 00:51:58 GMT
CMD ["bash"]
# Wed, 30 Mar 2022 02:17:13 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 30 Mar 2022 02:17:16 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 30 Mar 2022 02:17:16 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 30 Mar 2022 02:17:28 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 30 Mar 2022 02:17:29 GMT
VOLUME [/spiped]
# Wed, 30 Mar 2022 02:17:29 GMT
WORKDIR /spiped
# Wed, 30 Mar 2022 02:17:29 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 30 Mar 2022 02:17:29 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 30 Mar 2022 02:17:29 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:ffb22bcde95509bb75f6dd2d69f3fdb5c7471727e4d720b31d92cd297582865c`  
		Last Modified: Tue, 29 Mar 2022 01:04:43 GMT  
		Size: 29.7 MB (29655426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9488a45de61a7c26b2a863c250a52839737d409c8bac0426e2161131489985d3`  
		Last Modified: Wed, 30 Mar 2022 02:18:10 GMT  
		Size: 1.7 KB (1735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abedbd8409757c2b32910d965e11e1ba2d29a16105361932d6d8bd82b611d64d`  
		Last Modified: Wed, 30 Mar 2022 02:18:10 GMT  
		Size: 1.1 KB (1053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0eb1d8925fb8e4d0edc85c85b1f0d782db61bdf479a93bc6a0ccd97410d5a81`  
		Last Modified: Wed, 30 Mar 2022 02:18:10 GMT  
		Size: 5.2 MB (5186412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7987418a0dc4bd8525c7ad87f10f5f7ca2fdd8060ac0807f66714351df3d27cc`  
		Last Modified: Wed, 30 Mar 2022 02:18:10 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3647b49ea4318215c86c777031179b0cacb01790a04d0208a9d80a7962bb5768`  
		Last Modified: Wed, 30 Mar 2022 02:18:10 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
