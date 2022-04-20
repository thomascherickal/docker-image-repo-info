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
$ docker pull spiped@sha256:e41d72055c192ba15be28273bd2527bec1287049aa45503a6ae35843aaf1e7f0
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
$ docker pull spiped@sha256:16dc6e9c7cc546dd93b3277b671e27c1f626381772450d34aca4fe57204d4133
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.3 MB (37349089 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:936295bd1770ae3d06a781883aaf0402285a3ca230376de9c3e66805404bafd2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 20 Apr 2022 04:43:27 GMT
ADD file:8b1e79f91081eb527b455431af58e823d8b84d9d0c8e5c47cb7bda7507954ae4 in / 
# Wed, 20 Apr 2022 04:43:27 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 14:42:13 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 20 Apr 2022 14:42:16 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 14:42:17 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 20 Apr 2022 14:42:36 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 20 Apr 2022 14:42:36 GMT
VOLUME [/spiped]
# Wed, 20 Apr 2022 14:42:36 GMT
WORKDIR /spiped
# Wed, 20 Apr 2022 14:42:36 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 20 Apr 2022 14:42:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 20 Apr 2022 14:42:37 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:1fe172e4850f03bb45d41a20174112bc119fbfec42a650edbbd8491aee32e3c3`  
		Last Modified: Wed, 20 Apr 2022 04:48:27 GMT  
		Size: 31.4 MB (31378979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b928d6a0541674b585ea92d20767b83422feb13d6fbc1abaa28a7826bb06248`  
		Last Modified: Wed, 20 Apr 2022 14:42:55 GMT  
		Size: 1.7 KB (1733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66b378d15273f2509a64b2226cba3a808959f15b27da55a7d76e5c65f9eba0b3`  
		Last Modified: Wed, 20 Apr 2022 14:42:54 GMT  
		Size: 1.1 KB (1051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42cafcb442c712c0e3e55bd8f3b333a2017004ee9b8cfc91b8db9f785da03f20`  
		Last Modified: Wed, 20 Apr 2022 14:42:55 GMT  
		Size: 6.0 MB (5966859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74d34e46b75a94b87d6f0e6244d621ca65062e16482ab72da03c043c47b92fb7`  
		Last Modified: Wed, 20 Apr 2022 14:42:53 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:829867eb8d44007081e54aa2f2d2c95672a8d637ada17d287d61ee015deb07c9`  
		Last Modified: Wed, 20 Apr 2022 14:42:54 GMT  
		Size: 338.0 B  
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
$ docker pull spiped@sha256:c77b8dcee965e718c75a675e3a54836064db87b3b5c58ba037d2a6c55d8df2a8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.3 MB (35339282 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ab11032d60954d0b8efe030e933f75c0fe37bc1e065a04d430b561ead73447cf`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 20 Apr 2022 04:29:10 GMT
ADD file:84523b5820128293b713ef35d8db618921162250da1e4c72bf9923f34ad7d87d in / 
# Wed, 20 Apr 2022 04:29:11 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 13:23:17 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 20 Apr 2022 13:23:20 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 13:23:21 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 20 Apr 2022 13:23:40 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 20 Apr 2022 13:23:40 GMT
VOLUME [/spiped]
# Wed, 20 Apr 2022 13:23:41 GMT
WORKDIR /spiped
# Wed, 20 Apr 2022 13:23:43 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 20 Apr 2022 13:23:43 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 20 Apr 2022 13:23:44 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:6d4a449ac69c579312443ded09f57c4894e7adb42f7406abd364f95982fafc59`  
		Last Modified: Wed, 20 Apr 2022 04:35:49 GMT  
		Size: 30.1 MB (30065801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42dc04924f7bc70b614cd605748ff30771d2512c072c23ee447a97913fb8fcac`  
		Last Modified: Wed, 20 Apr 2022 13:24:16 GMT  
		Size: 1.6 KB (1617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fc7419a408efd2adf7d6262aba45bf723a68c82f6fed03a452ed435d056a2ea`  
		Last Modified: Wed, 20 Apr 2022 13:24:16 GMT  
		Size: 923.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ed1890998ade1d071e1c0a83385b099cf5a2c90cf3c07aed336df959c389566`  
		Last Modified: Wed, 20 Apr 2022 13:24:17 GMT  
		Size: 5.3 MB (5270506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f49fd39484937ac9d29d7115f083632a23430e844508db5f87ca3242623ec5a3`  
		Last Modified: Wed, 20 Apr 2022 13:24:16 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e88e88b2bc326b3bd7b854635b99e68b9221a9681011eab185be6cd5a25c3997`  
		Last Modified: Wed, 20 Apr 2022 13:24:17 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; 386

```console
$ docker pull spiped@sha256:638aec173289dc36b5cb473a6a2c56bb663a242dbf686b59570afe0545ad78b4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.3 MB (40283724 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a1b75d157a7b3804959f6312294fa5d73153d8b9bdb132528b65a8d1621c1962`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 20 Apr 2022 07:37:35 GMT
ADD file:460761e2baaea91893a907ce122ff7d585ef5704f48c03454835986028a1d842 in / 
# Wed, 20 Apr 2022 07:37:35 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 17:17:55 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 20 Apr 2022 17:17:58 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 17:17:59 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 20 Apr 2022 17:18:20 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 20 Apr 2022 17:18:20 GMT
VOLUME [/spiped]
# Wed, 20 Apr 2022 17:18:21 GMT
WORKDIR /spiped
# Wed, 20 Apr 2022 17:18:23 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 20 Apr 2022 17:18:23 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 20 Apr 2022 17:18:24 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:6e5c4eb151e267d273883db6e9aee3ff01be07e098ca33f0d1d65bb0e0416921`  
		Last Modified: Wed, 20 Apr 2022 07:44:54 GMT  
		Size: 32.4 MB (32389597 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f028933eb426fbb298139a1dca2725fb0eafb946f569b992df24bd34162a48b3`  
		Last Modified: Wed, 20 Apr 2022 17:18:55 GMT  
		Size: 1.6 KB (1607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67f360e1d9530b3648bdcf5c7326926ff5baa64e92bda4a4a0728b5c9ccc6ff4`  
		Last Modified: Wed, 20 Apr 2022 17:18:55 GMT  
		Size: 924.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ffdaa6a1838fae07117537f9592ff6d6ff9fb9e606e49ef07d7fa284f8e4fec`  
		Last Modified: Wed, 20 Apr 2022 17:18:58 GMT  
		Size: 7.9 MB (7891164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e2dcefeb0e2e0da58f1e84d51883255fdb16534020498300dc17b9be99fddaa`  
		Last Modified: Wed, 20 Apr 2022 17:18:55 GMT  
		Size: 93.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b096bbf0c1da11d62385da1f32accd5cdca77bdf49211090df69c4c01fbb36bf`  
		Last Modified: Wed, 20 Apr 2022 17:18:55 GMT  
		Size: 339.0 B  
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
$ docker pull spiped@sha256:bf075f42da62ca883587f9728ba830188d24ee2945ee2696ae7eb3a34fb93a5b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.8 MB (34844651 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:07ef13537cd5b4d11ab787b82be9cc057080d956e800fc47b9ee29a41e12cc55`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 20 Apr 2022 08:39:37 GMT
ADD file:c3381330644d6d9fc585301395580b564cdf7c880fb2dc2d8e48992673184f7d in / 
# Wed, 20 Apr 2022 08:39:42 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 19:26:58 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 20 Apr 2022 19:27:03 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 19:27:03 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 20 Apr 2022 19:27:40 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 20 Apr 2022 19:27:41 GMT
VOLUME [/spiped]
# Wed, 20 Apr 2022 19:27:42 GMT
WORKDIR /spiped
# Wed, 20 Apr 2022 19:27:43 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 20 Apr 2022 19:27:43 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 20 Apr 2022 19:27:44 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:3179e1eccb473ae22a70e8ac3e9ddb4660ebdfd977989d115bd4d322ecc12b89`  
		Last Modified: Wed, 20 Apr 2022 08:49:39 GMT  
		Size: 29.7 MB (29654805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d754de8e8834cac9eb69a9928cc0308eb7cc27e2f6179a47006dd83eb79efe8`  
		Last Modified: Wed, 20 Apr 2022 19:28:25 GMT  
		Size: 1.7 KB (1738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:614b1cc169aee0108e5bd1ffc58bfdf24837336e51383305d18cc65a2fe0b39d`  
		Last Modified: Wed, 20 Apr 2022 19:28:25 GMT  
		Size: 1.1 KB (1053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c0ad428027cd8d71d60220f87669bda68ddc3c7a16a841848a3074ecdc45c00`  
		Last Modified: Wed, 20 Apr 2022 19:28:26 GMT  
		Size: 5.2 MB (5186587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:928adbd6d308eae2f0dd4159d224497e8b7b98bb8cadf312090af2224a17f0fa`  
		Last Modified: Wed, 20 Apr 2022 19:28:25 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5136bd5ecd9f140deaae6471ebdb42dceb9269b5ae767360d52e426758aaee31`  
		Last Modified: Wed, 20 Apr 2022 19:28:25 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:1-alpine`

```console
$ docker pull spiped@sha256:e803772f3cd77bd5eb74c25cebf7dbe58c1490172affec2756736f01297e2ad6
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
$ docker pull spiped@sha256:44fa18e7d3af978bedc72ce9110a2217004554deec585dfcdafffb4c761a1661
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 MB (2830637 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b21bdc008b33d69d3d83d8292f28384b56c4166b1ef0c3f5c05eac33a48df2a7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Mon, 04 Apr 2022 23:49:42 GMT
ADD file:159dcddaab900372df882a4e94615ed84250e9cea3e74bc0479d98280342f596 in / 
# Mon, 04 Apr 2022 23:49:42 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 11:42:28 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Tue, 05 Apr 2022 11:42:30 GMT
RUN apk add --no-cache libssl1.1
# Tue, 05 Apr 2022 11:42:30 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 05 Apr 2022 11:42:49 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Tue, 05 Apr 2022 11:42:50 GMT
VOLUME [/spiped]
# Tue, 05 Apr 2022 11:42:50 GMT
WORKDIR /spiped
# Tue, 05 Apr 2022 11:42:51 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 05 Apr 2022 11:42:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 05 Apr 2022 11:42:52 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:c319b1fc4ed70b8241a7ce6ac0c4015d354bf5cf8c01eb73c50b6709c0c46e49`  
		Last Modified: Mon, 04 Apr 2022 19:09:22 GMT  
		Size: 2.6 MB (2621972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b279880cad38890c6b22622a3cecb67733556ec9965319ffa327afec8900ad3`  
		Last Modified: Tue, 05 Apr 2022 11:43:27 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27045425770040b89c6aeadebc232d3bd49690ccc505ec5a20336cbfa650b899`  
		Last Modified: Tue, 05 Apr 2022 11:43:27 GMT  
		Size: 7.8 KB (7767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfe17e03d9a44e0c737a4484821d473ab6476046270059fab5ebad88fdbfcce7`  
		Last Modified: Tue, 05 Apr 2022 11:43:27 GMT  
		Size: 199.2 KB (199161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2979a2148a9f161c6f6ae02c8bdc6b41f1f18da7a66d2db5addec2e19752388b`  
		Last Modified: Tue, 05 Apr 2022 11:43:26 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5863282bd4052a3bc2b39bb2d4cc46b864b2e4214edba85c572e7f55f95d7ee1`  
		Last Modified: Tue, 05 Apr 2022 11:43:26 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; arm variant v7

```console
$ docker pull spiped@sha256:41ea58744c279880bd672731168c41728c367a5558010a8b15109a53651aed8b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 MB (2626540 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fa3a26053023e3df6fe0ab2fdfc9b5c0e7806a837bdf8aeeebed934566092f5f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Mon, 04 Apr 2022 23:57:34 GMT
ADD file:20f8cdddc53a4a8bd78945fc32fe08e9f80ab3b16dc20a9aa4ba73b79f2bc71c in / 
# Mon, 04 Apr 2022 23:57:35 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 15:38:30 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Tue, 05 Apr 2022 15:38:32 GMT
RUN apk add --no-cache libssl1.1
# Tue, 05 Apr 2022 15:38:33 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 05 Apr 2022 15:38:51 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Tue, 05 Apr 2022 15:38:51 GMT
VOLUME [/spiped]
# Tue, 05 Apr 2022 15:38:52 GMT
WORKDIR /spiped
# Tue, 05 Apr 2022 15:38:52 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 05 Apr 2022 15:38:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 05 Apr 2022 15:38:53 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:57fb4b5f1a47c953ca5703f0f81ce14e5d01cf23aa79558b5adb961cc526e320`  
		Last Modified: Mon, 04 Apr 2022 19:09:36 GMT  
		Size: 2.4 MB (2424323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c34bb3a817bf019eff75e990b3ee9f75b0d33a5070d140d69adcd81bc3c61d4`  
		Last Modified: Tue, 05 Apr 2022 15:39:47 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50ddc3edc7d50bace02b581239b3d2096bbdd43b8d5cca77199c023788b7bab9`  
		Last Modified: Tue, 05 Apr 2022 15:39:47 GMT  
		Size: 7.8 KB (7779 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e4b14e7f868497bf35a981b97fa3d6c40d44c373e6207c0e73aa3292319b6e8`  
		Last Modified: Tue, 05 Apr 2022 15:39:47 GMT  
		Size: 192.7 KB (192698 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c22a92e8f54240f73e546662dc34d0aa6b83ec1617f18fa8e178c93138c0b72e`  
		Last Modified: Tue, 05 Apr 2022 15:39:47 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98ad3607e9857b6fb1bb4fbf10d6e9ed9e787343edd64901dc0ecaadd3ff55db`  
		Last Modified: Tue, 05 Apr 2022 15:39:47 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:6b7fd2442f6dcd71561982dfb157122343a4c720493a891274c64d2c577ce4ab
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 MB (2933135 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8dc39b7901f2654c939cb1c1d44ff3a6e036a4bcf2cef396786768da4de2f658`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Mon, 04 Apr 2022 23:39:31 GMT
ADD file:90e56af13188c7f0283d244a0d70b853d8bef8587a41f1da8eac3a2aba8964ef in / 
# Mon, 04 Apr 2022 23:39:31 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 14:38:03 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Tue, 05 Apr 2022 14:38:04 GMT
RUN apk add --no-cache libssl1.1
# Tue, 05 Apr 2022 14:38:05 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 05 Apr 2022 14:38:15 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Tue, 05 Apr 2022 14:38:16 GMT
VOLUME [/spiped]
# Tue, 05 Apr 2022 14:38:17 GMT
WORKDIR /spiped
# Tue, 05 Apr 2022 14:38:19 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 05 Apr 2022 14:38:19 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 05 Apr 2022 14:38:20 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:9981e73032c8833e387a8f96986e560edbed12c38119e0edb0439c9c2234eac9`  
		Last Modified: Mon, 04 Apr 2022 19:09:10 GMT  
		Size: 2.7 MB (2716477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe4c0758a179cd25e16e078f253517cd4f315287416c3ce781a852e456da3093`  
		Last Modified: Tue, 05 Apr 2022 14:38:47 GMT  
		Size: 1.2 KB (1240 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ad68b994955132db089d9decfe3c1abb1e0d937a743641a82ff97b1ad0de230`  
		Last Modified: Tue, 05 Apr 2022 14:38:47 GMT  
		Size: 7.7 KB (7749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2412b85fbb446b18863d0276c285a9f15c5506327e253be647ba7c7e323d01e0`  
		Last Modified: Tue, 05 Apr 2022 14:38:47 GMT  
		Size: 207.2 KB (207235 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff9b28798cece086f58205831a8c06e9be4d79eb185eb2a5566b692c6bb0aa1f`  
		Last Modified: Tue, 05 Apr 2022 14:38:47 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9aa51b8e1739c24bc53b08bbda05fba07af4b69550a9c5ac36ea5be1bb7d5b1`  
		Last Modified: Tue, 05 Apr 2022 14:38:47 GMT  
		Size: 339.0 B  
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
$ docker pull spiped@sha256:6d1206f429c5113ac4fbd6820b913ec32aa3cb826c65e5446d05eb57c3bfd7f4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (3033860 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:64a17da88fc17c158a4b17b8a85a6b534482d5b9fe198bee0a961886519d4811`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 05 Apr 2022 00:23:30 GMT
ADD file:960cf6f9d3d1cfcb36c2d67dd4c3eaba7db1d0c7afe97968512248d7f234ad47 in / 
# Tue, 05 Apr 2022 00:23:32 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 20:07:37 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Tue, 05 Apr 2022 20:08:01 GMT
RUN apk add --no-cache libssl1.1
# Tue, 05 Apr 2022 20:08:06 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 05 Apr 2022 20:08:35 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Tue, 05 Apr 2022 20:08:41 GMT
VOLUME [/spiped]
# Tue, 05 Apr 2022 20:08:46 GMT
WORKDIR /spiped
# Tue, 05 Apr 2022 20:08:48 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 05 Apr 2022 20:08:49 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 05 Apr 2022 20:08:52 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:1877acf2d48ed8bcb5bd9756a95aca0c077457be7cf4fcef25807f4e9be88db1`  
		Last Modified: Mon, 04 Apr 2022 19:09:49 GMT  
		Size: 2.8 MB (2811186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:898122ed2d1fcbc53be831191766c1b47d98b8cb2251d70dcc91e5ecad3bf34e`  
		Last Modified: Tue, 05 Apr 2022 20:09:25 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0cdc12b8854b22d6407eaece31ad74f6d0d2f322236c0d02a0074aef7944b93`  
		Last Modified: Tue, 05 Apr 2022 20:09:25 GMT  
		Size: 7.8 KB (7771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc1f84e0deee708d9995b37beb5b3923a9091dcc0ee670f7d784de701af40e2e`  
		Last Modified: Tue, 05 Apr 2022 20:09:25 GMT  
		Size: 213.2 KB (213160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67c77cab4a7338ba5a131c568ed153eb1fd0151dbb6108fae4fd3234a699f6ac`  
		Last Modified: Tue, 05 Apr 2022 20:09:25 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e03666b6f800b3362553b44e783b6eff051c84c4ae25bdb3d1da279626fc8bb9`  
		Last Modified: Tue, 05 Apr 2022 20:09:25 GMT  
		Size: 345.0 B  
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
$ docker pull spiped@sha256:e41d72055c192ba15be28273bd2527bec1287049aa45503a6ae35843aaf1e7f0
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
$ docker pull spiped@sha256:16dc6e9c7cc546dd93b3277b671e27c1f626381772450d34aca4fe57204d4133
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.3 MB (37349089 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:936295bd1770ae3d06a781883aaf0402285a3ca230376de9c3e66805404bafd2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 20 Apr 2022 04:43:27 GMT
ADD file:8b1e79f91081eb527b455431af58e823d8b84d9d0c8e5c47cb7bda7507954ae4 in / 
# Wed, 20 Apr 2022 04:43:27 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 14:42:13 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 20 Apr 2022 14:42:16 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 14:42:17 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 20 Apr 2022 14:42:36 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 20 Apr 2022 14:42:36 GMT
VOLUME [/spiped]
# Wed, 20 Apr 2022 14:42:36 GMT
WORKDIR /spiped
# Wed, 20 Apr 2022 14:42:36 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 20 Apr 2022 14:42:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 20 Apr 2022 14:42:37 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:1fe172e4850f03bb45d41a20174112bc119fbfec42a650edbbd8491aee32e3c3`  
		Last Modified: Wed, 20 Apr 2022 04:48:27 GMT  
		Size: 31.4 MB (31378979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b928d6a0541674b585ea92d20767b83422feb13d6fbc1abaa28a7826bb06248`  
		Last Modified: Wed, 20 Apr 2022 14:42:55 GMT  
		Size: 1.7 KB (1733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66b378d15273f2509a64b2226cba3a808959f15b27da55a7d76e5c65f9eba0b3`  
		Last Modified: Wed, 20 Apr 2022 14:42:54 GMT  
		Size: 1.1 KB (1051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42cafcb442c712c0e3e55bd8f3b333a2017004ee9b8cfc91b8db9f785da03f20`  
		Last Modified: Wed, 20 Apr 2022 14:42:55 GMT  
		Size: 6.0 MB (5966859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74d34e46b75a94b87d6f0e6244d621ca65062e16482ab72da03c043c47b92fb7`  
		Last Modified: Wed, 20 Apr 2022 14:42:53 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:829867eb8d44007081e54aa2f2d2c95672a8d637ada17d287d61ee015deb07c9`  
		Last Modified: Wed, 20 Apr 2022 14:42:54 GMT  
		Size: 338.0 B  
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
$ docker pull spiped@sha256:c77b8dcee965e718c75a675e3a54836064db87b3b5c58ba037d2a6c55d8df2a8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.3 MB (35339282 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ab11032d60954d0b8efe030e933f75c0fe37bc1e065a04d430b561ead73447cf`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 20 Apr 2022 04:29:10 GMT
ADD file:84523b5820128293b713ef35d8db618921162250da1e4c72bf9923f34ad7d87d in / 
# Wed, 20 Apr 2022 04:29:11 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 13:23:17 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 20 Apr 2022 13:23:20 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 13:23:21 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 20 Apr 2022 13:23:40 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 20 Apr 2022 13:23:40 GMT
VOLUME [/spiped]
# Wed, 20 Apr 2022 13:23:41 GMT
WORKDIR /spiped
# Wed, 20 Apr 2022 13:23:43 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 20 Apr 2022 13:23:43 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 20 Apr 2022 13:23:44 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:6d4a449ac69c579312443ded09f57c4894e7adb42f7406abd364f95982fafc59`  
		Last Modified: Wed, 20 Apr 2022 04:35:49 GMT  
		Size: 30.1 MB (30065801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42dc04924f7bc70b614cd605748ff30771d2512c072c23ee447a97913fb8fcac`  
		Last Modified: Wed, 20 Apr 2022 13:24:16 GMT  
		Size: 1.6 KB (1617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fc7419a408efd2adf7d6262aba45bf723a68c82f6fed03a452ed435d056a2ea`  
		Last Modified: Wed, 20 Apr 2022 13:24:16 GMT  
		Size: 923.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ed1890998ade1d071e1c0a83385b099cf5a2c90cf3c07aed336df959c389566`  
		Last Modified: Wed, 20 Apr 2022 13:24:17 GMT  
		Size: 5.3 MB (5270506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f49fd39484937ac9d29d7115f083632a23430e844508db5f87ca3242623ec5a3`  
		Last Modified: Wed, 20 Apr 2022 13:24:16 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e88e88b2bc326b3bd7b854635b99e68b9221a9681011eab185be6cd5a25c3997`  
		Last Modified: Wed, 20 Apr 2022 13:24:17 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; 386

```console
$ docker pull spiped@sha256:638aec173289dc36b5cb473a6a2c56bb663a242dbf686b59570afe0545ad78b4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.3 MB (40283724 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a1b75d157a7b3804959f6312294fa5d73153d8b9bdb132528b65a8d1621c1962`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 20 Apr 2022 07:37:35 GMT
ADD file:460761e2baaea91893a907ce122ff7d585ef5704f48c03454835986028a1d842 in / 
# Wed, 20 Apr 2022 07:37:35 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 17:17:55 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 20 Apr 2022 17:17:58 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 17:17:59 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 20 Apr 2022 17:18:20 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 20 Apr 2022 17:18:20 GMT
VOLUME [/spiped]
# Wed, 20 Apr 2022 17:18:21 GMT
WORKDIR /spiped
# Wed, 20 Apr 2022 17:18:23 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 20 Apr 2022 17:18:23 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 20 Apr 2022 17:18:24 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:6e5c4eb151e267d273883db6e9aee3ff01be07e098ca33f0d1d65bb0e0416921`  
		Last Modified: Wed, 20 Apr 2022 07:44:54 GMT  
		Size: 32.4 MB (32389597 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f028933eb426fbb298139a1dca2725fb0eafb946f569b992df24bd34162a48b3`  
		Last Modified: Wed, 20 Apr 2022 17:18:55 GMT  
		Size: 1.6 KB (1607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67f360e1d9530b3648bdcf5c7326926ff5baa64e92bda4a4a0728b5c9ccc6ff4`  
		Last Modified: Wed, 20 Apr 2022 17:18:55 GMT  
		Size: 924.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ffdaa6a1838fae07117537f9592ff6d6ff9fb9e606e49ef07d7fa284f8e4fec`  
		Last Modified: Wed, 20 Apr 2022 17:18:58 GMT  
		Size: 7.9 MB (7891164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e2dcefeb0e2e0da58f1e84d51883255fdb16534020498300dc17b9be99fddaa`  
		Last Modified: Wed, 20 Apr 2022 17:18:55 GMT  
		Size: 93.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b096bbf0c1da11d62385da1f32accd5cdca77bdf49211090df69c4c01fbb36bf`  
		Last Modified: Wed, 20 Apr 2022 17:18:55 GMT  
		Size: 339.0 B  
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
$ docker pull spiped@sha256:bf075f42da62ca883587f9728ba830188d24ee2945ee2696ae7eb3a34fb93a5b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.8 MB (34844651 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:07ef13537cd5b4d11ab787b82be9cc057080d956e800fc47b9ee29a41e12cc55`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 20 Apr 2022 08:39:37 GMT
ADD file:c3381330644d6d9fc585301395580b564cdf7c880fb2dc2d8e48992673184f7d in / 
# Wed, 20 Apr 2022 08:39:42 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 19:26:58 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 20 Apr 2022 19:27:03 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 19:27:03 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 20 Apr 2022 19:27:40 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 20 Apr 2022 19:27:41 GMT
VOLUME [/spiped]
# Wed, 20 Apr 2022 19:27:42 GMT
WORKDIR /spiped
# Wed, 20 Apr 2022 19:27:43 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 20 Apr 2022 19:27:43 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 20 Apr 2022 19:27:44 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:3179e1eccb473ae22a70e8ac3e9ddb4660ebdfd977989d115bd4d322ecc12b89`  
		Last Modified: Wed, 20 Apr 2022 08:49:39 GMT  
		Size: 29.7 MB (29654805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d754de8e8834cac9eb69a9928cc0308eb7cc27e2f6179a47006dd83eb79efe8`  
		Last Modified: Wed, 20 Apr 2022 19:28:25 GMT  
		Size: 1.7 KB (1738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:614b1cc169aee0108e5bd1ffc58bfdf24837336e51383305d18cc65a2fe0b39d`  
		Last Modified: Wed, 20 Apr 2022 19:28:25 GMT  
		Size: 1.1 KB (1053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c0ad428027cd8d71d60220f87669bda68ddc3c7a16a841848a3074ecdc45c00`  
		Last Modified: Wed, 20 Apr 2022 19:28:26 GMT  
		Size: 5.2 MB (5186587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:928adbd6d308eae2f0dd4159d224497e8b7b98bb8cadf312090af2224a17f0fa`  
		Last Modified: Wed, 20 Apr 2022 19:28:25 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5136bd5ecd9f140deaae6471ebdb42dceb9269b5ae767360d52e426758aaee31`  
		Last Modified: Wed, 20 Apr 2022 19:28:25 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:1.6-alpine`

```console
$ docker pull spiped@sha256:e803772f3cd77bd5eb74c25cebf7dbe58c1490172affec2756736f01297e2ad6
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
$ docker pull spiped@sha256:44fa18e7d3af978bedc72ce9110a2217004554deec585dfcdafffb4c761a1661
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 MB (2830637 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b21bdc008b33d69d3d83d8292f28384b56c4166b1ef0c3f5c05eac33a48df2a7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Mon, 04 Apr 2022 23:49:42 GMT
ADD file:159dcddaab900372df882a4e94615ed84250e9cea3e74bc0479d98280342f596 in / 
# Mon, 04 Apr 2022 23:49:42 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 11:42:28 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Tue, 05 Apr 2022 11:42:30 GMT
RUN apk add --no-cache libssl1.1
# Tue, 05 Apr 2022 11:42:30 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 05 Apr 2022 11:42:49 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Tue, 05 Apr 2022 11:42:50 GMT
VOLUME [/spiped]
# Tue, 05 Apr 2022 11:42:50 GMT
WORKDIR /spiped
# Tue, 05 Apr 2022 11:42:51 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 05 Apr 2022 11:42:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 05 Apr 2022 11:42:52 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:c319b1fc4ed70b8241a7ce6ac0c4015d354bf5cf8c01eb73c50b6709c0c46e49`  
		Last Modified: Mon, 04 Apr 2022 19:09:22 GMT  
		Size: 2.6 MB (2621972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b279880cad38890c6b22622a3cecb67733556ec9965319ffa327afec8900ad3`  
		Last Modified: Tue, 05 Apr 2022 11:43:27 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27045425770040b89c6aeadebc232d3bd49690ccc505ec5a20336cbfa650b899`  
		Last Modified: Tue, 05 Apr 2022 11:43:27 GMT  
		Size: 7.8 KB (7767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfe17e03d9a44e0c737a4484821d473ab6476046270059fab5ebad88fdbfcce7`  
		Last Modified: Tue, 05 Apr 2022 11:43:27 GMT  
		Size: 199.2 KB (199161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2979a2148a9f161c6f6ae02c8bdc6b41f1f18da7a66d2db5addec2e19752388b`  
		Last Modified: Tue, 05 Apr 2022 11:43:26 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5863282bd4052a3bc2b39bb2d4cc46b864b2e4214edba85c572e7f55f95d7ee1`  
		Last Modified: Tue, 05 Apr 2022 11:43:26 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; arm variant v7

```console
$ docker pull spiped@sha256:41ea58744c279880bd672731168c41728c367a5558010a8b15109a53651aed8b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 MB (2626540 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fa3a26053023e3df6fe0ab2fdfc9b5c0e7806a837bdf8aeeebed934566092f5f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Mon, 04 Apr 2022 23:57:34 GMT
ADD file:20f8cdddc53a4a8bd78945fc32fe08e9f80ab3b16dc20a9aa4ba73b79f2bc71c in / 
# Mon, 04 Apr 2022 23:57:35 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 15:38:30 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Tue, 05 Apr 2022 15:38:32 GMT
RUN apk add --no-cache libssl1.1
# Tue, 05 Apr 2022 15:38:33 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 05 Apr 2022 15:38:51 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Tue, 05 Apr 2022 15:38:51 GMT
VOLUME [/spiped]
# Tue, 05 Apr 2022 15:38:52 GMT
WORKDIR /spiped
# Tue, 05 Apr 2022 15:38:52 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 05 Apr 2022 15:38:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 05 Apr 2022 15:38:53 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:57fb4b5f1a47c953ca5703f0f81ce14e5d01cf23aa79558b5adb961cc526e320`  
		Last Modified: Mon, 04 Apr 2022 19:09:36 GMT  
		Size: 2.4 MB (2424323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c34bb3a817bf019eff75e990b3ee9f75b0d33a5070d140d69adcd81bc3c61d4`  
		Last Modified: Tue, 05 Apr 2022 15:39:47 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50ddc3edc7d50bace02b581239b3d2096bbdd43b8d5cca77199c023788b7bab9`  
		Last Modified: Tue, 05 Apr 2022 15:39:47 GMT  
		Size: 7.8 KB (7779 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e4b14e7f868497bf35a981b97fa3d6c40d44c373e6207c0e73aa3292319b6e8`  
		Last Modified: Tue, 05 Apr 2022 15:39:47 GMT  
		Size: 192.7 KB (192698 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c22a92e8f54240f73e546662dc34d0aa6b83ec1617f18fa8e178c93138c0b72e`  
		Last Modified: Tue, 05 Apr 2022 15:39:47 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98ad3607e9857b6fb1bb4fbf10d6e9ed9e787343edd64901dc0ecaadd3ff55db`  
		Last Modified: Tue, 05 Apr 2022 15:39:47 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:6b7fd2442f6dcd71561982dfb157122343a4c720493a891274c64d2c577ce4ab
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 MB (2933135 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8dc39b7901f2654c939cb1c1d44ff3a6e036a4bcf2cef396786768da4de2f658`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Mon, 04 Apr 2022 23:39:31 GMT
ADD file:90e56af13188c7f0283d244a0d70b853d8bef8587a41f1da8eac3a2aba8964ef in / 
# Mon, 04 Apr 2022 23:39:31 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 14:38:03 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Tue, 05 Apr 2022 14:38:04 GMT
RUN apk add --no-cache libssl1.1
# Tue, 05 Apr 2022 14:38:05 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 05 Apr 2022 14:38:15 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Tue, 05 Apr 2022 14:38:16 GMT
VOLUME [/spiped]
# Tue, 05 Apr 2022 14:38:17 GMT
WORKDIR /spiped
# Tue, 05 Apr 2022 14:38:19 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 05 Apr 2022 14:38:19 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 05 Apr 2022 14:38:20 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:9981e73032c8833e387a8f96986e560edbed12c38119e0edb0439c9c2234eac9`  
		Last Modified: Mon, 04 Apr 2022 19:09:10 GMT  
		Size: 2.7 MB (2716477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe4c0758a179cd25e16e078f253517cd4f315287416c3ce781a852e456da3093`  
		Last Modified: Tue, 05 Apr 2022 14:38:47 GMT  
		Size: 1.2 KB (1240 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ad68b994955132db089d9decfe3c1abb1e0d937a743641a82ff97b1ad0de230`  
		Last Modified: Tue, 05 Apr 2022 14:38:47 GMT  
		Size: 7.7 KB (7749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2412b85fbb446b18863d0276c285a9f15c5506327e253be647ba7c7e323d01e0`  
		Last Modified: Tue, 05 Apr 2022 14:38:47 GMT  
		Size: 207.2 KB (207235 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff9b28798cece086f58205831a8c06e9be4d79eb185eb2a5566b692c6bb0aa1f`  
		Last Modified: Tue, 05 Apr 2022 14:38:47 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9aa51b8e1739c24bc53b08bbda05fba07af4b69550a9c5ac36ea5be1bb7d5b1`  
		Last Modified: Tue, 05 Apr 2022 14:38:47 GMT  
		Size: 339.0 B  
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
$ docker pull spiped@sha256:6d1206f429c5113ac4fbd6820b913ec32aa3cb826c65e5446d05eb57c3bfd7f4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (3033860 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:64a17da88fc17c158a4b17b8a85a6b534482d5b9fe198bee0a961886519d4811`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 05 Apr 2022 00:23:30 GMT
ADD file:960cf6f9d3d1cfcb36c2d67dd4c3eaba7db1d0c7afe97968512248d7f234ad47 in / 
# Tue, 05 Apr 2022 00:23:32 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 20:07:37 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Tue, 05 Apr 2022 20:08:01 GMT
RUN apk add --no-cache libssl1.1
# Tue, 05 Apr 2022 20:08:06 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 05 Apr 2022 20:08:35 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Tue, 05 Apr 2022 20:08:41 GMT
VOLUME [/spiped]
# Tue, 05 Apr 2022 20:08:46 GMT
WORKDIR /spiped
# Tue, 05 Apr 2022 20:08:48 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 05 Apr 2022 20:08:49 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 05 Apr 2022 20:08:52 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:1877acf2d48ed8bcb5bd9756a95aca0c077457be7cf4fcef25807f4e9be88db1`  
		Last Modified: Mon, 04 Apr 2022 19:09:49 GMT  
		Size: 2.8 MB (2811186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:898122ed2d1fcbc53be831191766c1b47d98b8cb2251d70dcc91e5ecad3bf34e`  
		Last Modified: Tue, 05 Apr 2022 20:09:25 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0cdc12b8854b22d6407eaece31ad74f6d0d2f322236c0d02a0074aef7944b93`  
		Last Modified: Tue, 05 Apr 2022 20:09:25 GMT  
		Size: 7.8 KB (7771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc1f84e0deee708d9995b37beb5b3923a9091dcc0ee670f7d784de701af40e2e`  
		Last Modified: Tue, 05 Apr 2022 20:09:25 GMT  
		Size: 213.2 KB (213160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67c77cab4a7338ba5a131c568ed153eb1fd0151dbb6108fae4fd3234a699f6ac`  
		Last Modified: Tue, 05 Apr 2022 20:09:25 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e03666b6f800b3362553b44e783b6eff051c84c4ae25bdb3d1da279626fc8bb9`  
		Last Modified: Tue, 05 Apr 2022 20:09:25 GMT  
		Size: 345.0 B  
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
$ docker pull spiped@sha256:e41d72055c192ba15be28273bd2527bec1287049aa45503a6ae35843aaf1e7f0
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
$ docker pull spiped@sha256:16dc6e9c7cc546dd93b3277b671e27c1f626381772450d34aca4fe57204d4133
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.3 MB (37349089 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:936295bd1770ae3d06a781883aaf0402285a3ca230376de9c3e66805404bafd2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 20 Apr 2022 04:43:27 GMT
ADD file:8b1e79f91081eb527b455431af58e823d8b84d9d0c8e5c47cb7bda7507954ae4 in / 
# Wed, 20 Apr 2022 04:43:27 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 14:42:13 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 20 Apr 2022 14:42:16 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 14:42:17 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 20 Apr 2022 14:42:36 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 20 Apr 2022 14:42:36 GMT
VOLUME [/spiped]
# Wed, 20 Apr 2022 14:42:36 GMT
WORKDIR /spiped
# Wed, 20 Apr 2022 14:42:36 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 20 Apr 2022 14:42:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 20 Apr 2022 14:42:37 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:1fe172e4850f03bb45d41a20174112bc119fbfec42a650edbbd8491aee32e3c3`  
		Last Modified: Wed, 20 Apr 2022 04:48:27 GMT  
		Size: 31.4 MB (31378979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b928d6a0541674b585ea92d20767b83422feb13d6fbc1abaa28a7826bb06248`  
		Last Modified: Wed, 20 Apr 2022 14:42:55 GMT  
		Size: 1.7 KB (1733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66b378d15273f2509a64b2226cba3a808959f15b27da55a7d76e5c65f9eba0b3`  
		Last Modified: Wed, 20 Apr 2022 14:42:54 GMT  
		Size: 1.1 KB (1051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42cafcb442c712c0e3e55bd8f3b333a2017004ee9b8cfc91b8db9f785da03f20`  
		Last Modified: Wed, 20 Apr 2022 14:42:55 GMT  
		Size: 6.0 MB (5966859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74d34e46b75a94b87d6f0e6244d621ca65062e16482ab72da03c043c47b92fb7`  
		Last Modified: Wed, 20 Apr 2022 14:42:53 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:829867eb8d44007081e54aa2f2d2c95672a8d637ada17d287d61ee015deb07c9`  
		Last Modified: Wed, 20 Apr 2022 14:42:54 GMT  
		Size: 338.0 B  
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
$ docker pull spiped@sha256:c77b8dcee965e718c75a675e3a54836064db87b3b5c58ba037d2a6c55d8df2a8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.3 MB (35339282 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ab11032d60954d0b8efe030e933f75c0fe37bc1e065a04d430b561ead73447cf`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 20 Apr 2022 04:29:10 GMT
ADD file:84523b5820128293b713ef35d8db618921162250da1e4c72bf9923f34ad7d87d in / 
# Wed, 20 Apr 2022 04:29:11 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 13:23:17 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 20 Apr 2022 13:23:20 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 13:23:21 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 20 Apr 2022 13:23:40 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 20 Apr 2022 13:23:40 GMT
VOLUME [/spiped]
# Wed, 20 Apr 2022 13:23:41 GMT
WORKDIR /spiped
# Wed, 20 Apr 2022 13:23:43 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 20 Apr 2022 13:23:43 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 20 Apr 2022 13:23:44 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:6d4a449ac69c579312443ded09f57c4894e7adb42f7406abd364f95982fafc59`  
		Last Modified: Wed, 20 Apr 2022 04:35:49 GMT  
		Size: 30.1 MB (30065801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42dc04924f7bc70b614cd605748ff30771d2512c072c23ee447a97913fb8fcac`  
		Last Modified: Wed, 20 Apr 2022 13:24:16 GMT  
		Size: 1.6 KB (1617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fc7419a408efd2adf7d6262aba45bf723a68c82f6fed03a452ed435d056a2ea`  
		Last Modified: Wed, 20 Apr 2022 13:24:16 GMT  
		Size: 923.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ed1890998ade1d071e1c0a83385b099cf5a2c90cf3c07aed336df959c389566`  
		Last Modified: Wed, 20 Apr 2022 13:24:17 GMT  
		Size: 5.3 MB (5270506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f49fd39484937ac9d29d7115f083632a23430e844508db5f87ca3242623ec5a3`  
		Last Modified: Wed, 20 Apr 2022 13:24:16 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e88e88b2bc326b3bd7b854635b99e68b9221a9681011eab185be6cd5a25c3997`  
		Last Modified: Wed, 20 Apr 2022 13:24:17 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.2` - linux; 386

```console
$ docker pull spiped@sha256:638aec173289dc36b5cb473a6a2c56bb663a242dbf686b59570afe0545ad78b4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.3 MB (40283724 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a1b75d157a7b3804959f6312294fa5d73153d8b9bdb132528b65a8d1621c1962`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 20 Apr 2022 07:37:35 GMT
ADD file:460761e2baaea91893a907ce122ff7d585ef5704f48c03454835986028a1d842 in / 
# Wed, 20 Apr 2022 07:37:35 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 17:17:55 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 20 Apr 2022 17:17:58 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 17:17:59 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 20 Apr 2022 17:18:20 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 20 Apr 2022 17:18:20 GMT
VOLUME [/spiped]
# Wed, 20 Apr 2022 17:18:21 GMT
WORKDIR /spiped
# Wed, 20 Apr 2022 17:18:23 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 20 Apr 2022 17:18:23 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 20 Apr 2022 17:18:24 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:6e5c4eb151e267d273883db6e9aee3ff01be07e098ca33f0d1d65bb0e0416921`  
		Last Modified: Wed, 20 Apr 2022 07:44:54 GMT  
		Size: 32.4 MB (32389597 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f028933eb426fbb298139a1dca2725fb0eafb946f569b992df24bd34162a48b3`  
		Last Modified: Wed, 20 Apr 2022 17:18:55 GMT  
		Size: 1.6 KB (1607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67f360e1d9530b3648bdcf5c7326926ff5baa64e92bda4a4a0728b5c9ccc6ff4`  
		Last Modified: Wed, 20 Apr 2022 17:18:55 GMT  
		Size: 924.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ffdaa6a1838fae07117537f9592ff6d6ff9fb9e606e49ef07d7fa284f8e4fec`  
		Last Modified: Wed, 20 Apr 2022 17:18:58 GMT  
		Size: 7.9 MB (7891164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e2dcefeb0e2e0da58f1e84d51883255fdb16534020498300dc17b9be99fddaa`  
		Last Modified: Wed, 20 Apr 2022 17:18:55 GMT  
		Size: 93.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b096bbf0c1da11d62385da1f32accd5cdca77bdf49211090df69c4c01fbb36bf`  
		Last Modified: Wed, 20 Apr 2022 17:18:55 GMT  
		Size: 339.0 B  
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
$ docker pull spiped@sha256:bf075f42da62ca883587f9728ba830188d24ee2945ee2696ae7eb3a34fb93a5b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.8 MB (34844651 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:07ef13537cd5b4d11ab787b82be9cc057080d956e800fc47b9ee29a41e12cc55`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 20 Apr 2022 08:39:37 GMT
ADD file:c3381330644d6d9fc585301395580b564cdf7c880fb2dc2d8e48992673184f7d in / 
# Wed, 20 Apr 2022 08:39:42 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 19:26:58 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 20 Apr 2022 19:27:03 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 19:27:03 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 20 Apr 2022 19:27:40 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 20 Apr 2022 19:27:41 GMT
VOLUME [/spiped]
# Wed, 20 Apr 2022 19:27:42 GMT
WORKDIR /spiped
# Wed, 20 Apr 2022 19:27:43 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 20 Apr 2022 19:27:43 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 20 Apr 2022 19:27:44 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:3179e1eccb473ae22a70e8ac3e9ddb4660ebdfd977989d115bd4d322ecc12b89`  
		Last Modified: Wed, 20 Apr 2022 08:49:39 GMT  
		Size: 29.7 MB (29654805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d754de8e8834cac9eb69a9928cc0308eb7cc27e2f6179a47006dd83eb79efe8`  
		Last Modified: Wed, 20 Apr 2022 19:28:25 GMT  
		Size: 1.7 KB (1738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:614b1cc169aee0108e5bd1ffc58bfdf24837336e51383305d18cc65a2fe0b39d`  
		Last Modified: Wed, 20 Apr 2022 19:28:25 GMT  
		Size: 1.1 KB (1053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c0ad428027cd8d71d60220f87669bda68ddc3c7a16a841848a3074ecdc45c00`  
		Last Modified: Wed, 20 Apr 2022 19:28:26 GMT  
		Size: 5.2 MB (5186587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:928adbd6d308eae2f0dd4159d224497e8b7b98bb8cadf312090af2224a17f0fa`  
		Last Modified: Wed, 20 Apr 2022 19:28:25 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5136bd5ecd9f140deaae6471ebdb42dceb9269b5ae767360d52e426758aaee31`  
		Last Modified: Wed, 20 Apr 2022 19:28:25 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:1.6.2-alpine`

```console
$ docker pull spiped@sha256:e803772f3cd77bd5eb74c25cebf7dbe58c1490172affec2756736f01297e2ad6
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
$ docker pull spiped@sha256:44fa18e7d3af978bedc72ce9110a2217004554deec585dfcdafffb4c761a1661
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 MB (2830637 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b21bdc008b33d69d3d83d8292f28384b56c4166b1ef0c3f5c05eac33a48df2a7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Mon, 04 Apr 2022 23:49:42 GMT
ADD file:159dcddaab900372df882a4e94615ed84250e9cea3e74bc0479d98280342f596 in / 
# Mon, 04 Apr 2022 23:49:42 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 11:42:28 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Tue, 05 Apr 2022 11:42:30 GMT
RUN apk add --no-cache libssl1.1
# Tue, 05 Apr 2022 11:42:30 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 05 Apr 2022 11:42:49 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Tue, 05 Apr 2022 11:42:50 GMT
VOLUME [/spiped]
# Tue, 05 Apr 2022 11:42:50 GMT
WORKDIR /spiped
# Tue, 05 Apr 2022 11:42:51 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 05 Apr 2022 11:42:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 05 Apr 2022 11:42:52 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:c319b1fc4ed70b8241a7ce6ac0c4015d354bf5cf8c01eb73c50b6709c0c46e49`  
		Last Modified: Mon, 04 Apr 2022 19:09:22 GMT  
		Size: 2.6 MB (2621972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b279880cad38890c6b22622a3cecb67733556ec9965319ffa327afec8900ad3`  
		Last Modified: Tue, 05 Apr 2022 11:43:27 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27045425770040b89c6aeadebc232d3bd49690ccc505ec5a20336cbfa650b899`  
		Last Modified: Tue, 05 Apr 2022 11:43:27 GMT  
		Size: 7.8 KB (7767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfe17e03d9a44e0c737a4484821d473ab6476046270059fab5ebad88fdbfcce7`  
		Last Modified: Tue, 05 Apr 2022 11:43:27 GMT  
		Size: 199.2 KB (199161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2979a2148a9f161c6f6ae02c8bdc6b41f1f18da7a66d2db5addec2e19752388b`  
		Last Modified: Tue, 05 Apr 2022 11:43:26 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5863282bd4052a3bc2b39bb2d4cc46b864b2e4214edba85c572e7f55f95d7ee1`  
		Last Modified: Tue, 05 Apr 2022 11:43:26 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.2-alpine` - linux; arm variant v7

```console
$ docker pull spiped@sha256:41ea58744c279880bd672731168c41728c367a5558010a8b15109a53651aed8b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 MB (2626540 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fa3a26053023e3df6fe0ab2fdfc9b5c0e7806a837bdf8aeeebed934566092f5f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Mon, 04 Apr 2022 23:57:34 GMT
ADD file:20f8cdddc53a4a8bd78945fc32fe08e9f80ab3b16dc20a9aa4ba73b79f2bc71c in / 
# Mon, 04 Apr 2022 23:57:35 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 15:38:30 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Tue, 05 Apr 2022 15:38:32 GMT
RUN apk add --no-cache libssl1.1
# Tue, 05 Apr 2022 15:38:33 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 05 Apr 2022 15:38:51 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Tue, 05 Apr 2022 15:38:51 GMT
VOLUME [/spiped]
# Tue, 05 Apr 2022 15:38:52 GMT
WORKDIR /spiped
# Tue, 05 Apr 2022 15:38:52 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 05 Apr 2022 15:38:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 05 Apr 2022 15:38:53 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:57fb4b5f1a47c953ca5703f0f81ce14e5d01cf23aa79558b5adb961cc526e320`  
		Last Modified: Mon, 04 Apr 2022 19:09:36 GMT  
		Size: 2.4 MB (2424323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c34bb3a817bf019eff75e990b3ee9f75b0d33a5070d140d69adcd81bc3c61d4`  
		Last Modified: Tue, 05 Apr 2022 15:39:47 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50ddc3edc7d50bace02b581239b3d2096bbdd43b8d5cca77199c023788b7bab9`  
		Last Modified: Tue, 05 Apr 2022 15:39:47 GMT  
		Size: 7.8 KB (7779 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e4b14e7f868497bf35a981b97fa3d6c40d44c373e6207c0e73aa3292319b6e8`  
		Last Modified: Tue, 05 Apr 2022 15:39:47 GMT  
		Size: 192.7 KB (192698 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c22a92e8f54240f73e546662dc34d0aa6b83ec1617f18fa8e178c93138c0b72e`  
		Last Modified: Tue, 05 Apr 2022 15:39:47 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98ad3607e9857b6fb1bb4fbf10d6e9ed9e787343edd64901dc0ecaadd3ff55db`  
		Last Modified: Tue, 05 Apr 2022 15:39:47 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.2-alpine` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:6b7fd2442f6dcd71561982dfb157122343a4c720493a891274c64d2c577ce4ab
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 MB (2933135 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8dc39b7901f2654c939cb1c1d44ff3a6e036a4bcf2cef396786768da4de2f658`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Mon, 04 Apr 2022 23:39:31 GMT
ADD file:90e56af13188c7f0283d244a0d70b853d8bef8587a41f1da8eac3a2aba8964ef in / 
# Mon, 04 Apr 2022 23:39:31 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 14:38:03 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Tue, 05 Apr 2022 14:38:04 GMT
RUN apk add --no-cache libssl1.1
# Tue, 05 Apr 2022 14:38:05 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 05 Apr 2022 14:38:15 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Tue, 05 Apr 2022 14:38:16 GMT
VOLUME [/spiped]
# Tue, 05 Apr 2022 14:38:17 GMT
WORKDIR /spiped
# Tue, 05 Apr 2022 14:38:19 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 05 Apr 2022 14:38:19 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 05 Apr 2022 14:38:20 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:9981e73032c8833e387a8f96986e560edbed12c38119e0edb0439c9c2234eac9`  
		Last Modified: Mon, 04 Apr 2022 19:09:10 GMT  
		Size: 2.7 MB (2716477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe4c0758a179cd25e16e078f253517cd4f315287416c3ce781a852e456da3093`  
		Last Modified: Tue, 05 Apr 2022 14:38:47 GMT  
		Size: 1.2 KB (1240 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ad68b994955132db089d9decfe3c1abb1e0d937a743641a82ff97b1ad0de230`  
		Last Modified: Tue, 05 Apr 2022 14:38:47 GMT  
		Size: 7.7 KB (7749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2412b85fbb446b18863d0276c285a9f15c5506327e253be647ba7c7e323d01e0`  
		Last Modified: Tue, 05 Apr 2022 14:38:47 GMT  
		Size: 207.2 KB (207235 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff9b28798cece086f58205831a8c06e9be4d79eb185eb2a5566b692c6bb0aa1f`  
		Last Modified: Tue, 05 Apr 2022 14:38:47 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9aa51b8e1739c24bc53b08bbda05fba07af4b69550a9c5ac36ea5be1bb7d5b1`  
		Last Modified: Tue, 05 Apr 2022 14:38:47 GMT  
		Size: 339.0 B  
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
$ docker pull spiped@sha256:6d1206f429c5113ac4fbd6820b913ec32aa3cb826c65e5446d05eb57c3bfd7f4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (3033860 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:64a17da88fc17c158a4b17b8a85a6b534482d5b9fe198bee0a961886519d4811`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 05 Apr 2022 00:23:30 GMT
ADD file:960cf6f9d3d1cfcb36c2d67dd4c3eaba7db1d0c7afe97968512248d7f234ad47 in / 
# Tue, 05 Apr 2022 00:23:32 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 20:07:37 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Tue, 05 Apr 2022 20:08:01 GMT
RUN apk add --no-cache libssl1.1
# Tue, 05 Apr 2022 20:08:06 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 05 Apr 2022 20:08:35 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Tue, 05 Apr 2022 20:08:41 GMT
VOLUME [/spiped]
# Tue, 05 Apr 2022 20:08:46 GMT
WORKDIR /spiped
# Tue, 05 Apr 2022 20:08:48 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 05 Apr 2022 20:08:49 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 05 Apr 2022 20:08:52 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:1877acf2d48ed8bcb5bd9756a95aca0c077457be7cf4fcef25807f4e9be88db1`  
		Last Modified: Mon, 04 Apr 2022 19:09:49 GMT  
		Size: 2.8 MB (2811186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:898122ed2d1fcbc53be831191766c1b47d98b8cb2251d70dcc91e5ecad3bf34e`  
		Last Modified: Tue, 05 Apr 2022 20:09:25 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0cdc12b8854b22d6407eaece31ad74f6d0d2f322236c0d02a0074aef7944b93`  
		Last Modified: Tue, 05 Apr 2022 20:09:25 GMT  
		Size: 7.8 KB (7771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc1f84e0deee708d9995b37beb5b3923a9091dcc0ee670f7d784de701af40e2e`  
		Last Modified: Tue, 05 Apr 2022 20:09:25 GMT  
		Size: 213.2 KB (213160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67c77cab4a7338ba5a131c568ed153eb1fd0151dbb6108fae4fd3234a699f6ac`  
		Last Modified: Tue, 05 Apr 2022 20:09:25 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e03666b6f800b3362553b44e783b6eff051c84c4ae25bdb3d1da279626fc8bb9`  
		Last Modified: Tue, 05 Apr 2022 20:09:25 GMT  
		Size: 345.0 B  
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
$ docker pull spiped@sha256:e803772f3cd77bd5eb74c25cebf7dbe58c1490172affec2756736f01297e2ad6
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
$ docker pull spiped@sha256:44fa18e7d3af978bedc72ce9110a2217004554deec585dfcdafffb4c761a1661
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 MB (2830637 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b21bdc008b33d69d3d83d8292f28384b56c4166b1ef0c3f5c05eac33a48df2a7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Mon, 04 Apr 2022 23:49:42 GMT
ADD file:159dcddaab900372df882a4e94615ed84250e9cea3e74bc0479d98280342f596 in / 
# Mon, 04 Apr 2022 23:49:42 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 11:42:28 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Tue, 05 Apr 2022 11:42:30 GMT
RUN apk add --no-cache libssl1.1
# Tue, 05 Apr 2022 11:42:30 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 05 Apr 2022 11:42:49 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Tue, 05 Apr 2022 11:42:50 GMT
VOLUME [/spiped]
# Tue, 05 Apr 2022 11:42:50 GMT
WORKDIR /spiped
# Tue, 05 Apr 2022 11:42:51 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 05 Apr 2022 11:42:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 05 Apr 2022 11:42:52 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:c319b1fc4ed70b8241a7ce6ac0c4015d354bf5cf8c01eb73c50b6709c0c46e49`  
		Last Modified: Mon, 04 Apr 2022 19:09:22 GMT  
		Size: 2.6 MB (2621972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b279880cad38890c6b22622a3cecb67733556ec9965319ffa327afec8900ad3`  
		Last Modified: Tue, 05 Apr 2022 11:43:27 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27045425770040b89c6aeadebc232d3bd49690ccc505ec5a20336cbfa650b899`  
		Last Modified: Tue, 05 Apr 2022 11:43:27 GMT  
		Size: 7.8 KB (7767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfe17e03d9a44e0c737a4484821d473ab6476046270059fab5ebad88fdbfcce7`  
		Last Modified: Tue, 05 Apr 2022 11:43:27 GMT  
		Size: 199.2 KB (199161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2979a2148a9f161c6f6ae02c8bdc6b41f1f18da7a66d2db5addec2e19752388b`  
		Last Modified: Tue, 05 Apr 2022 11:43:26 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5863282bd4052a3bc2b39bb2d4cc46b864b2e4214edba85c572e7f55f95d7ee1`  
		Last Modified: Tue, 05 Apr 2022 11:43:26 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; arm variant v7

```console
$ docker pull spiped@sha256:41ea58744c279880bd672731168c41728c367a5558010a8b15109a53651aed8b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 MB (2626540 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fa3a26053023e3df6fe0ab2fdfc9b5c0e7806a837bdf8aeeebed934566092f5f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Mon, 04 Apr 2022 23:57:34 GMT
ADD file:20f8cdddc53a4a8bd78945fc32fe08e9f80ab3b16dc20a9aa4ba73b79f2bc71c in / 
# Mon, 04 Apr 2022 23:57:35 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 15:38:30 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Tue, 05 Apr 2022 15:38:32 GMT
RUN apk add --no-cache libssl1.1
# Tue, 05 Apr 2022 15:38:33 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 05 Apr 2022 15:38:51 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Tue, 05 Apr 2022 15:38:51 GMT
VOLUME [/spiped]
# Tue, 05 Apr 2022 15:38:52 GMT
WORKDIR /spiped
# Tue, 05 Apr 2022 15:38:52 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 05 Apr 2022 15:38:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 05 Apr 2022 15:38:53 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:57fb4b5f1a47c953ca5703f0f81ce14e5d01cf23aa79558b5adb961cc526e320`  
		Last Modified: Mon, 04 Apr 2022 19:09:36 GMT  
		Size: 2.4 MB (2424323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c34bb3a817bf019eff75e990b3ee9f75b0d33a5070d140d69adcd81bc3c61d4`  
		Last Modified: Tue, 05 Apr 2022 15:39:47 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50ddc3edc7d50bace02b581239b3d2096bbdd43b8d5cca77199c023788b7bab9`  
		Last Modified: Tue, 05 Apr 2022 15:39:47 GMT  
		Size: 7.8 KB (7779 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e4b14e7f868497bf35a981b97fa3d6c40d44c373e6207c0e73aa3292319b6e8`  
		Last Modified: Tue, 05 Apr 2022 15:39:47 GMT  
		Size: 192.7 KB (192698 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c22a92e8f54240f73e546662dc34d0aa6b83ec1617f18fa8e178c93138c0b72e`  
		Last Modified: Tue, 05 Apr 2022 15:39:47 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98ad3607e9857b6fb1bb4fbf10d6e9ed9e787343edd64901dc0ecaadd3ff55db`  
		Last Modified: Tue, 05 Apr 2022 15:39:47 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:6b7fd2442f6dcd71561982dfb157122343a4c720493a891274c64d2c577ce4ab
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 MB (2933135 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8dc39b7901f2654c939cb1c1d44ff3a6e036a4bcf2cef396786768da4de2f658`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Mon, 04 Apr 2022 23:39:31 GMT
ADD file:90e56af13188c7f0283d244a0d70b853d8bef8587a41f1da8eac3a2aba8964ef in / 
# Mon, 04 Apr 2022 23:39:31 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 14:38:03 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Tue, 05 Apr 2022 14:38:04 GMT
RUN apk add --no-cache libssl1.1
# Tue, 05 Apr 2022 14:38:05 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 05 Apr 2022 14:38:15 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Tue, 05 Apr 2022 14:38:16 GMT
VOLUME [/spiped]
# Tue, 05 Apr 2022 14:38:17 GMT
WORKDIR /spiped
# Tue, 05 Apr 2022 14:38:19 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 05 Apr 2022 14:38:19 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 05 Apr 2022 14:38:20 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:9981e73032c8833e387a8f96986e560edbed12c38119e0edb0439c9c2234eac9`  
		Last Modified: Mon, 04 Apr 2022 19:09:10 GMT  
		Size: 2.7 MB (2716477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe4c0758a179cd25e16e078f253517cd4f315287416c3ce781a852e456da3093`  
		Last Modified: Tue, 05 Apr 2022 14:38:47 GMT  
		Size: 1.2 KB (1240 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ad68b994955132db089d9decfe3c1abb1e0d937a743641a82ff97b1ad0de230`  
		Last Modified: Tue, 05 Apr 2022 14:38:47 GMT  
		Size: 7.7 KB (7749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2412b85fbb446b18863d0276c285a9f15c5506327e253be647ba7c7e323d01e0`  
		Last Modified: Tue, 05 Apr 2022 14:38:47 GMT  
		Size: 207.2 KB (207235 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff9b28798cece086f58205831a8c06e9be4d79eb185eb2a5566b692c6bb0aa1f`  
		Last Modified: Tue, 05 Apr 2022 14:38:47 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9aa51b8e1739c24bc53b08bbda05fba07af4b69550a9c5ac36ea5be1bb7d5b1`  
		Last Modified: Tue, 05 Apr 2022 14:38:47 GMT  
		Size: 339.0 B  
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
$ docker pull spiped@sha256:6d1206f429c5113ac4fbd6820b913ec32aa3cb826c65e5446d05eb57c3bfd7f4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (3033860 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:64a17da88fc17c158a4b17b8a85a6b534482d5b9fe198bee0a961886519d4811`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 05 Apr 2022 00:23:30 GMT
ADD file:960cf6f9d3d1cfcb36c2d67dd4c3eaba7db1d0c7afe97968512248d7f234ad47 in / 
# Tue, 05 Apr 2022 00:23:32 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 20:07:37 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Tue, 05 Apr 2022 20:08:01 GMT
RUN apk add --no-cache libssl1.1
# Tue, 05 Apr 2022 20:08:06 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 05 Apr 2022 20:08:35 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Tue, 05 Apr 2022 20:08:41 GMT
VOLUME [/spiped]
# Tue, 05 Apr 2022 20:08:46 GMT
WORKDIR /spiped
# Tue, 05 Apr 2022 20:08:48 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 05 Apr 2022 20:08:49 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 05 Apr 2022 20:08:52 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:1877acf2d48ed8bcb5bd9756a95aca0c077457be7cf4fcef25807f4e9be88db1`  
		Last Modified: Mon, 04 Apr 2022 19:09:49 GMT  
		Size: 2.8 MB (2811186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:898122ed2d1fcbc53be831191766c1b47d98b8cb2251d70dcc91e5ecad3bf34e`  
		Last Modified: Tue, 05 Apr 2022 20:09:25 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0cdc12b8854b22d6407eaece31ad74f6d0d2f322236c0d02a0074aef7944b93`  
		Last Modified: Tue, 05 Apr 2022 20:09:25 GMT  
		Size: 7.8 KB (7771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc1f84e0deee708d9995b37beb5b3923a9091dcc0ee670f7d784de701af40e2e`  
		Last Modified: Tue, 05 Apr 2022 20:09:25 GMT  
		Size: 213.2 KB (213160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67c77cab4a7338ba5a131c568ed153eb1fd0151dbb6108fae4fd3234a699f6ac`  
		Last Modified: Tue, 05 Apr 2022 20:09:25 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e03666b6f800b3362553b44e783b6eff051c84c4ae25bdb3d1da279626fc8bb9`  
		Last Modified: Tue, 05 Apr 2022 20:09:25 GMT  
		Size: 345.0 B  
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
$ docker pull spiped@sha256:e41d72055c192ba15be28273bd2527bec1287049aa45503a6ae35843aaf1e7f0
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
$ docker pull spiped@sha256:16dc6e9c7cc546dd93b3277b671e27c1f626381772450d34aca4fe57204d4133
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.3 MB (37349089 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:936295bd1770ae3d06a781883aaf0402285a3ca230376de9c3e66805404bafd2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 20 Apr 2022 04:43:27 GMT
ADD file:8b1e79f91081eb527b455431af58e823d8b84d9d0c8e5c47cb7bda7507954ae4 in / 
# Wed, 20 Apr 2022 04:43:27 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 14:42:13 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 20 Apr 2022 14:42:16 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 14:42:17 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 20 Apr 2022 14:42:36 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 20 Apr 2022 14:42:36 GMT
VOLUME [/spiped]
# Wed, 20 Apr 2022 14:42:36 GMT
WORKDIR /spiped
# Wed, 20 Apr 2022 14:42:36 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 20 Apr 2022 14:42:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 20 Apr 2022 14:42:37 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:1fe172e4850f03bb45d41a20174112bc119fbfec42a650edbbd8491aee32e3c3`  
		Last Modified: Wed, 20 Apr 2022 04:48:27 GMT  
		Size: 31.4 MB (31378979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b928d6a0541674b585ea92d20767b83422feb13d6fbc1abaa28a7826bb06248`  
		Last Modified: Wed, 20 Apr 2022 14:42:55 GMT  
		Size: 1.7 KB (1733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66b378d15273f2509a64b2226cba3a808959f15b27da55a7d76e5c65f9eba0b3`  
		Last Modified: Wed, 20 Apr 2022 14:42:54 GMT  
		Size: 1.1 KB (1051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42cafcb442c712c0e3e55bd8f3b333a2017004ee9b8cfc91b8db9f785da03f20`  
		Last Modified: Wed, 20 Apr 2022 14:42:55 GMT  
		Size: 6.0 MB (5966859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74d34e46b75a94b87d6f0e6244d621ca65062e16482ab72da03c043c47b92fb7`  
		Last Modified: Wed, 20 Apr 2022 14:42:53 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:829867eb8d44007081e54aa2f2d2c95672a8d637ada17d287d61ee015deb07c9`  
		Last Modified: Wed, 20 Apr 2022 14:42:54 GMT  
		Size: 338.0 B  
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
$ docker pull spiped@sha256:c77b8dcee965e718c75a675e3a54836064db87b3b5c58ba037d2a6c55d8df2a8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.3 MB (35339282 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ab11032d60954d0b8efe030e933f75c0fe37bc1e065a04d430b561ead73447cf`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 20 Apr 2022 04:29:10 GMT
ADD file:84523b5820128293b713ef35d8db618921162250da1e4c72bf9923f34ad7d87d in / 
# Wed, 20 Apr 2022 04:29:11 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 13:23:17 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 20 Apr 2022 13:23:20 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 13:23:21 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 20 Apr 2022 13:23:40 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 20 Apr 2022 13:23:40 GMT
VOLUME [/spiped]
# Wed, 20 Apr 2022 13:23:41 GMT
WORKDIR /spiped
# Wed, 20 Apr 2022 13:23:43 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 20 Apr 2022 13:23:43 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 20 Apr 2022 13:23:44 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:6d4a449ac69c579312443ded09f57c4894e7adb42f7406abd364f95982fafc59`  
		Last Modified: Wed, 20 Apr 2022 04:35:49 GMT  
		Size: 30.1 MB (30065801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42dc04924f7bc70b614cd605748ff30771d2512c072c23ee447a97913fb8fcac`  
		Last Modified: Wed, 20 Apr 2022 13:24:16 GMT  
		Size: 1.6 KB (1617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fc7419a408efd2adf7d6262aba45bf723a68c82f6fed03a452ed435d056a2ea`  
		Last Modified: Wed, 20 Apr 2022 13:24:16 GMT  
		Size: 923.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ed1890998ade1d071e1c0a83385b099cf5a2c90cf3c07aed336df959c389566`  
		Last Modified: Wed, 20 Apr 2022 13:24:17 GMT  
		Size: 5.3 MB (5270506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f49fd39484937ac9d29d7115f083632a23430e844508db5f87ca3242623ec5a3`  
		Last Modified: Wed, 20 Apr 2022 13:24:16 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e88e88b2bc326b3bd7b854635b99e68b9221a9681011eab185be6cd5a25c3997`  
		Last Modified: Wed, 20 Apr 2022 13:24:17 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; 386

```console
$ docker pull spiped@sha256:638aec173289dc36b5cb473a6a2c56bb663a242dbf686b59570afe0545ad78b4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.3 MB (40283724 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a1b75d157a7b3804959f6312294fa5d73153d8b9bdb132528b65a8d1621c1962`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 20 Apr 2022 07:37:35 GMT
ADD file:460761e2baaea91893a907ce122ff7d585ef5704f48c03454835986028a1d842 in / 
# Wed, 20 Apr 2022 07:37:35 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 17:17:55 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 20 Apr 2022 17:17:58 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 17:17:59 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 20 Apr 2022 17:18:20 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 20 Apr 2022 17:18:20 GMT
VOLUME [/spiped]
# Wed, 20 Apr 2022 17:18:21 GMT
WORKDIR /spiped
# Wed, 20 Apr 2022 17:18:23 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 20 Apr 2022 17:18:23 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 20 Apr 2022 17:18:24 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:6e5c4eb151e267d273883db6e9aee3ff01be07e098ca33f0d1d65bb0e0416921`  
		Last Modified: Wed, 20 Apr 2022 07:44:54 GMT  
		Size: 32.4 MB (32389597 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f028933eb426fbb298139a1dca2725fb0eafb946f569b992df24bd34162a48b3`  
		Last Modified: Wed, 20 Apr 2022 17:18:55 GMT  
		Size: 1.6 KB (1607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67f360e1d9530b3648bdcf5c7326926ff5baa64e92bda4a4a0728b5c9ccc6ff4`  
		Last Modified: Wed, 20 Apr 2022 17:18:55 GMT  
		Size: 924.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ffdaa6a1838fae07117537f9592ff6d6ff9fb9e606e49ef07d7fa284f8e4fec`  
		Last Modified: Wed, 20 Apr 2022 17:18:58 GMT  
		Size: 7.9 MB (7891164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e2dcefeb0e2e0da58f1e84d51883255fdb16534020498300dc17b9be99fddaa`  
		Last Modified: Wed, 20 Apr 2022 17:18:55 GMT  
		Size: 93.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b096bbf0c1da11d62385da1f32accd5cdca77bdf49211090df69c4c01fbb36bf`  
		Last Modified: Wed, 20 Apr 2022 17:18:55 GMT  
		Size: 339.0 B  
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
$ docker pull spiped@sha256:bf075f42da62ca883587f9728ba830188d24ee2945ee2696ae7eb3a34fb93a5b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.8 MB (34844651 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:07ef13537cd5b4d11ab787b82be9cc057080d956e800fc47b9ee29a41e12cc55`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 20 Apr 2022 08:39:37 GMT
ADD file:c3381330644d6d9fc585301395580b564cdf7c880fb2dc2d8e48992673184f7d in / 
# Wed, 20 Apr 2022 08:39:42 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 19:26:58 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 20 Apr 2022 19:27:03 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 19:27:03 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 20 Apr 2022 19:27:40 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 20 Apr 2022 19:27:41 GMT
VOLUME [/spiped]
# Wed, 20 Apr 2022 19:27:42 GMT
WORKDIR /spiped
# Wed, 20 Apr 2022 19:27:43 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 20 Apr 2022 19:27:43 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 20 Apr 2022 19:27:44 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:3179e1eccb473ae22a70e8ac3e9ddb4660ebdfd977989d115bd4d322ecc12b89`  
		Last Modified: Wed, 20 Apr 2022 08:49:39 GMT  
		Size: 29.7 MB (29654805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d754de8e8834cac9eb69a9928cc0308eb7cc27e2f6179a47006dd83eb79efe8`  
		Last Modified: Wed, 20 Apr 2022 19:28:25 GMT  
		Size: 1.7 KB (1738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:614b1cc169aee0108e5bd1ffc58bfdf24837336e51383305d18cc65a2fe0b39d`  
		Last Modified: Wed, 20 Apr 2022 19:28:25 GMT  
		Size: 1.1 KB (1053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c0ad428027cd8d71d60220f87669bda68ddc3c7a16a841848a3074ecdc45c00`  
		Last Modified: Wed, 20 Apr 2022 19:28:26 GMT  
		Size: 5.2 MB (5186587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:928adbd6d308eae2f0dd4159d224497e8b7b98bb8cadf312090af2224a17f0fa`  
		Last Modified: Wed, 20 Apr 2022 19:28:25 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5136bd5ecd9f140deaae6471ebdb42dceb9269b5ae767360d52e426758aaee31`  
		Last Modified: Wed, 20 Apr 2022 19:28:25 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
