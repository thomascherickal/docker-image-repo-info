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
$ docker pull spiped@sha256:f68d4f5a44d55612e4a5fb5ef03f87eb7e370254a26d5db4438a965ca47955b7
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
$ docker pull spiped@sha256:f507b4a86551d14d339abf790dac1c33db18bfb7284170964ee725265e10088d
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.3 MB (36266576 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:45c3b475d023dfa8186a606b7d1371e90494694ca0de5baf5f6e79fe68e66bf2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 15 May 2020 06:28:44 GMT
ADD file:7780c81c33e6cc5b6261af4a6c611cce0f39dec3131009bb297e65f12020c150 in / 
# Fri, 15 May 2020 06:28:44 GMT
CMD ["bash"]
# Sat, 16 May 2020 04:14:42 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Sat, 16 May 2020 04:14:47 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Sat, 16 May 2020 04:14:47 GMT
ENV SPIPED_VERSION=1.6.1
# Sat, 16 May 2020 04:14:47 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Sat, 16 May 2020 04:14:48 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Sat, 16 May 2020 04:15:31 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Sat, 16 May 2020 04:15:31 GMT
VOLUME [/spiped]
# Sat, 16 May 2020 04:15:32 GMT
WORKDIR /spiped
# Sat, 16 May 2020 04:15:32 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 16 May 2020 04:15:33 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 16 May 2020 04:15:33 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:afb6ec6fdc1c3ba04f7a56db32c5ff5ff38962dc4cd0ffdef5beaa0ce2eb77e2`  
		Last Modified: Fri, 15 May 2020 06:37:39 GMT  
		Size: 27.1 MB (27098756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf69e6d5168a8a643db7f3e097762e9a421e550edff25c02d584b76cec2578ce`  
		Last Modified: Sat, 16 May 2020 04:16:01 GMT  
		Size: 1.7 KB (1737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66db3f8998fea45888611f69f9e4fc3dcbff502f19c95bf902ffd7efbbe86966`  
		Last Modified: Sat, 16 May 2020 04:16:03 GMT  
		Size: 2.1 MB (2128102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e90a77d4c614a8407bcb3b077d130d797d0b128b6ad619c6d82573cb5da256ca`  
		Last Modified: Sat, 16 May 2020 04:16:04 GMT  
		Size: 7.0 MB (7037543 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:733772d709b4c96e4a851d79ab6edb5cc26d224468926544f23e40af781b29d8`  
		Last Modified: Sat, 16 May 2020 04:16:01 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11d35645dcf079b19bc3222e62897022743464d26c49ad631c80962369549efb`  
		Last Modified: Sat, 16 May 2020 04:16:01 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; arm variant v5

```console
$ docker pull spiped@sha256:89c0ca163f2aed719b25cfdfed1f04e927c7df87612a3b8249a847320b6b8bce
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.2 MB (32158596 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b151fa5d6a80c8c27152087cd00be0a1c5285e22caba7e411ecdbea1e5c4ce56`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 09 Jun 2020 00:51:58 GMT
ADD file:7fde417d1c70a9ef2b4e468f6e2ee4cbd3f340fb2d5b67ede087c81520c95f4a in / 
# Tue, 09 Jun 2020 00:51:59 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 01:20:07 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 09 Jun 2020 01:20:25 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 01:20:29 GMT
ENV SPIPED_VERSION=1.6.1
# Tue, 09 Jun 2020 01:20:33 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Tue, 09 Jun 2020 01:20:36 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Tue, 09 Jun 2020 01:21:51 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 09 Jun 2020 01:21:52 GMT
VOLUME [/spiped]
# Tue, 09 Jun 2020 01:21:52 GMT
WORKDIR /spiped
# Tue, 09 Jun 2020 01:21:53 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 09 Jun 2020 01:21:54 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 09 Jun 2020 01:21:54 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:5b11fc09c1a26b11a7df7d593adf43baff53c5cdba71cf8a87ae4a6dd17eb52c`  
		Last Modified: Tue, 09 Jun 2020 00:59:24 GMT  
		Size: 24.8 MB (24837249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a472cc54fb3976126466f6e8174720d2861ee99186f056d3aa776e2a94d13ae7`  
		Last Modified: Tue, 09 Jun 2020 01:22:16 GMT  
		Size: 1.7 KB (1725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:199d5cd61848e62c1013cc9a02e846466c14192913c2c3aa2ff178e44e02c53b`  
		Last Modified: Tue, 09 Jun 2020 01:22:16 GMT  
		Size: 1.8 MB (1839189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33ea1498c7e4ec77311232e10f6b24a9a59589d49a801733ae5319fba5aaa110`  
		Last Modified: Tue, 09 Jun 2020 01:22:19 GMT  
		Size: 5.5 MB (5479963 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95d84020e771e6045cb224230b0e3e07d9f77fcaf866dfca9dd82118dc3b39b1`  
		Last Modified: Tue, 09 Jun 2020 01:22:16 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dadc862a28f7f9a00d209adb7e25d470e36693b2f683c3efebc1ae9e8ce8800a`  
		Last Modified: Tue, 09 Jun 2020 01:22:16 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; arm variant v7

```console
$ docker pull spiped@sha256:82810696edb9b9cd3e20c069b4012756e7b42041c9542c8b5f839be38ca817c6
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.8 MB (29752935 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6260ddc16f2f5e54f0471a37563893cee16bbd967a1b1ac677bf3cac97f6a468`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 09 Jun 2020 01:01:24 GMT
ADD file:a35ca31d2a743d6a1738b1652f4f06c789abbca314d120f0e7e748311ac09ed2 in / 
# Tue, 09 Jun 2020 01:01:30 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 14:35:33 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 09 Jun 2020 14:35:42 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 14:35:43 GMT
ENV SPIPED_VERSION=1.6.1
# Tue, 09 Jun 2020 14:35:44 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Tue, 09 Jun 2020 14:35:45 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Tue, 09 Jun 2020 14:36:34 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 09 Jun 2020 14:36:35 GMT
VOLUME [/spiped]
# Tue, 09 Jun 2020 14:36:35 GMT
WORKDIR /spiped
# Tue, 09 Jun 2020 14:36:37 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 09 Jun 2020 14:36:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 09 Jun 2020 14:36:40 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:2dd003996c9ab82cac8112be0a4c04068e666e7a5d0cce3c65fb8f064de284e7`  
		Last Modified: Tue, 09 Jun 2020 01:10:25 GMT  
		Size: 22.7 MB (22705913 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92ddd3a5f3e7321eaaf8f41234d0e80dc3d7999e58c372bb5151417dc02a247c`  
		Last Modified: Tue, 09 Jun 2020 14:37:02 GMT  
		Size: 1.7 KB (1725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51282f9a582694ac89a16f9199036c324e405c496cb903b2691028c6464e2190`  
		Last Modified: Tue, 09 Jun 2020 14:37:02 GMT  
		Size: 1.8 MB (1759442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e51976ffb8ebca3a4d79b8161fb0e929f4cfd107ad09f09b5db452a67321c289`  
		Last Modified: Tue, 09 Jun 2020 14:37:04 GMT  
		Size: 5.3 MB (5285385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4657bf3b61375c1104a52dadec5dbc68c0fd4de727a013b5700db348ba5673b9`  
		Last Modified: Tue, 09 Jun 2020 14:37:02 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccf40741217b741d681454425549dc8910fbd06b638478c8494eeefd8f5d69b9`  
		Last Modified: Tue, 09 Jun 2020 14:37:02 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:cf2d29b06c1d1660698aa9de4dfb42854b60872ee61d9a012ee81240500612cc
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.8 MB (33773090 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ab2bf094b4eb433ebd77cb10ba397c7790ca5548502f326813e537efe5120cf3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 09 Jun 2020 01:52:01 GMT
ADD file:98823648634dfc3af50862b1e2da1028b23996a37adf43b1b0c3c5b29e94b9c7 in / 
# Tue, 09 Jun 2020 01:52:04 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 14:05:51 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 09 Jun 2020 14:05:59 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 14:05:59 GMT
ENV SPIPED_VERSION=1.6.1
# Tue, 09 Jun 2020 14:06:00 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Tue, 09 Jun 2020 14:06:01 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Tue, 09 Jun 2020 14:06:54 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 09 Jun 2020 14:06:55 GMT
VOLUME [/spiped]
# Tue, 09 Jun 2020 14:06:56 GMT
WORKDIR /spiped
# Tue, 09 Jun 2020 14:06:57 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 09 Jun 2020 14:06:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 09 Jun 2020 14:07:01 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:33cc09c9b190539635d7c971301f623d94fda5b4b5647966c6c240902119009f`  
		Last Modified: Tue, 09 Jun 2020 01:58:14 GMT  
		Size: 25.9 MB (25857704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7835e39ac04e97191d3dd883a78d8a2ca93f3b6d48edb467a020ed8aaa1b946c`  
		Last Modified: Tue, 09 Jun 2020 14:07:31 GMT  
		Size: 1.7 KB (1739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee4312c6f96572f3c7d9ba2921a53cf81d20e60ad38a4c67bdd72315940053f4`  
		Last Modified: Tue, 09 Jun 2020 14:07:31 GMT  
		Size: 2.0 MB (2007810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:108dcfd4a32f6e61f1aef4d1ed22a8a2f605529274e35f409d13a193b9a57ed4`  
		Last Modified: Tue, 09 Jun 2020 14:07:33 GMT  
		Size: 5.9 MB (5905367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42a4b05897e656cc187436d888abadd301fd521d43face9f8209586bbc697a7b`  
		Last Modified: Tue, 09 Jun 2020 14:07:31 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01a29dbcea99a23350569144e18f38a4733168c5bcfa9cac0462f663b2372c74`  
		Last Modified: Tue, 09 Jun 2020 14:07:31 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; 386

```console
$ docker pull spiped@sha256:8a7fe6ecb46c7724c5dd6bd2a7baf3094995f1b8edb6303ab0d8c15326f58db0
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.5 MB (41522653 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:713e39173dd25078ab6cc68a487ea2a5d84df4d6edbbcaa33083260d555368a1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 15 May 2020 07:07:55 GMT
ADD file:0c3b44c83914e95e4604999a86af05023cdd2b2f795e71d737e428fae4a7e0ac in / 
# Fri, 15 May 2020 07:07:56 GMT
CMD ["bash"]
# Fri, 15 May 2020 17:47:58 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Fri, 15 May 2020 17:48:04 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 17:48:05 GMT
ENV SPIPED_VERSION=1.6.1
# Fri, 15 May 2020 17:48:05 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Fri, 15 May 2020 17:48:05 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 15 May 2020 17:48:34 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Fri, 15 May 2020 17:48:34 GMT
VOLUME [/spiped]
# Fri, 15 May 2020 17:48:35 GMT
WORKDIR /spiped
# Fri, 15 May 2020 17:48:35 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 15 May 2020 17:48:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 15 May 2020 17:48:35 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:a5695130085a13212b02bf2645a52af5b41dd13e6dc9b29e2d7f357e1525aa48`  
		Last Modified: Fri, 15 May 2020 07:18:14 GMT  
		Size: 27.8 MB (27754922 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e46f1d7c78957f6663bbdcae7eb426e522750e8faf0a4174aed6c870289a058a`  
		Last Modified: Fri, 15 May 2020 17:48:55 GMT  
		Size: 1.7 KB (1731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94e9f3b4ac445b90a62301fd6363399326afdaced0908dfc316fbd74440a1fb2`  
		Last Modified: Fri, 15 May 2020 17:48:54 GMT  
		Size: 2.1 MB (2132373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e4350ab499cd08936f3d1a5c3662216bcbae435f2633319ba851eb2b3d1e00c`  
		Last Modified: Fri, 15 May 2020 17:49:03 GMT  
		Size: 11.6 MB (11633192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7d89781ff63fa52d84afbfa5beb9e63ad4cce6887c070fc07192d8abf85ccdc`  
		Last Modified: Fri, 15 May 2020 17:48:54 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:842d315391120a0e63fdb908daa3bdc3503566f8fa14d97cfcf770d05a50fbcd`  
		Last Modified: Fri, 15 May 2020 17:48:54 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; mips64le

```console
$ docker pull spiped@sha256:4e421f96912b140825f38f5b8b110891bd94b05d2ec75f34db06d6d199c4cd23
```

-	Docker Version: 19.03.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.9 MB (33894402 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d7a5df5ccfcc99a4ea0d50a3c49e81ce52581ff1b5164e4b80e2aa7d30ebc035`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 09 Jun 2020 01:10:06 GMT
ADD file:faf18b832680e98050b98c329add242425904e64c6a5a491c22d33e9417ef323 in / 
# Tue, 09 Jun 2020 01:10:06 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 02:27:39 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 09 Jun 2020 02:27:52 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 02:27:53 GMT
ENV SPIPED_VERSION=1.6.1
# Tue, 09 Jun 2020 02:27:53 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Tue, 09 Jun 2020 02:27:53 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Tue, 09 Jun 2020 02:29:02 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 09 Jun 2020 02:29:02 GMT
VOLUME [/spiped]
# Tue, 09 Jun 2020 02:29:03 GMT
WORKDIR /spiped
# Tue, 09 Jun 2020 02:29:03 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 09 Jun 2020 02:29:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 09 Jun 2020 02:29:04 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:76f2a0c8ea98ebd699a77ced9c677e97cd54b038a8c5e89670af78f38b047b33`  
		Last Modified: Tue, 09 Jun 2020 01:18:14 GMT  
		Size: 25.8 MB (25764040 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b82a47bf90ed455b577c438c12fe80d5fffca13a04f2ca9cec59ab9d64e327e`  
		Last Modified: Tue, 09 Jun 2020 02:29:24 GMT  
		Size: 1.7 KB (1729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbadd9d5a8dc90e2e4dc21414c4a8f4f186c31bde690d68c02d8b6a7b2447424`  
		Last Modified: Tue, 09 Jun 2020 02:29:26 GMT  
		Size: 1.7 MB (1712010 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:185ec9c5c819764b267f21284fed16f6049bac02cfad96abfcaf94cec25b18db`  
		Last Modified: Tue, 09 Jun 2020 02:29:31 GMT  
		Size: 6.4 MB (6416186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96b41dd1f9192b0235e97b93042cd81b32447840f020a5d7cb74b3c2c2c66b47`  
		Last Modified: Tue, 09 Jun 2020 02:29:24 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7c7e5506bf0d6b81418a33b8e3d4dc7c9f3ba1affab0cb6e0472754ed33454c`  
		Last Modified: Tue, 09 Jun 2020 02:29:24 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; ppc64le

```console
$ docker pull spiped@sha256:e0fe7e1f234d59836f3389de1bed55614da9de22f60d4b99c5020395738e16b0
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.5 MB (39494690 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5f5c577483a0496c4220a1c2277b81e7efb989b306fd3b9696971e84a75553ed`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 09 Jun 2020 01:22:34 GMT
ADD file:796aad1a35ba276b8cccc19987c152a713db101b2b65e30923db753f5b7f4b0f in / 
# Tue, 09 Jun 2020 01:22:38 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 03:52:53 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 09 Jun 2020 03:53:15 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 03:53:19 GMT
ENV SPIPED_VERSION=1.6.1
# Tue, 09 Jun 2020 03:53:26 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Tue, 09 Jun 2020 03:53:30 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Tue, 09 Jun 2020 03:55:33 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 09 Jun 2020 03:55:39 GMT
VOLUME [/spiped]
# Tue, 09 Jun 2020 03:55:44 GMT
WORKDIR /spiped
# Tue, 09 Jun 2020 03:55:46 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 09 Jun 2020 03:55:49 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 09 Jun 2020 03:55:52 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:63dbb66c5119bb5086d9e6fb6b154211afc20b44ed136ab7df808f6044cfc6f1`  
		Last Modified: Tue, 09 Jun 2020 01:31:04 GMT  
		Size: 30.5 MB (30524405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cdfd1c0bee0e2e09274162abe2b977b3876128838d43bdc7eded948eec4bf3f`  
		Last Modified: Tue, 09 Jun 2020 03:56:13 GMT  
		Size: 1.7 KB (1734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48279681b065daff73ee3f8ed95b05bdbf278498522ecf1ecc4c88b9fdf37888`  
		Last Modified: Tue, 09 Jun 2020 03:56:13 GMT  
		Size: 2.2 MB (2224949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14a6d252cdc4299f3b8d5819bded4186749b023311b2b9426eace76eb1ae1f09`  
		Last Modified: Tue, 09 Jun 2020 03:56:15 GMT  
		Size: 6.7 MB (6743134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba6c95b5243cf1886f4f17eb961b37932f9d63fa92c3a74bdd80b48424525b67`  
		Last Modified: Tue, 09 Jun 2020 03:56:13 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d86b530154fc517e54378d0142464946d98da0d74a3659f716a9d62f6f958cd5`  
		Last Modified: Tue, 09 Jun 2020 03:56:13 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; s390x

```console
$ docker pull spiped@sha256:e2268b6aea33adcd0e93fa1a60fddc4b589b9145a4400b07beaa756100f6ac54
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.5 MB (33479972 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8b6fc4e4a7364dee9d160cba7e4f9eb1db130b4b86902f49ef7ad7fc117f4f3e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 09 Jun 2020 01:42:37 GMT
ADD file:b21d426de40a194c6c76ed27593f33fb1ea470e15d4d43b00d7601472110de1a in / 
# Tue, 09 Jun 2020 01:42:38 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 02:20:52 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 09 Jun 2020 02:20:55 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 02:20:55 GMT
ENV SPIPED_VERSION=1.6.1
# Tue, 09 Jun 2020 02:20:56 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Tue, 09 Jun 2020 02:20:56 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Tue, 09 Jun 2020 02:21:11 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 09 Jun 2020 02:21:12 GMT
VOLUME [/spiped]
# Tue, 09 Jun 2020 02:21:12 GMT
WORKDIR /spiped
# Tue, 09 Jun 2020 02:21:12 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 09 Jun 2020 02:21:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 09 Jun 2020 02:21:13 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:405e75bf6bb0104d67fcebf58e07cd21bf344589df9c1a41c00354a60ea3a604`  
		Last Modified: Tue, 09 Jun 2020 01:46:30 GMT  
		Size: 25.7 MB (25712668 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17b0d5c87b23ce137e58201b2c08e71d5ea9d83dd59fa3909aa2c53f614d5c10`  
		Last Modified: Tue, 09 Jun 2020 02:21:27 GMT  
		Size: 1.7 KB (1731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eee2a9d7f4f7fcd8891c08e77d7f1994667fd23ca8313160ee58b02eecf8fcfa`  
		Last Modified: Tue, 09 Jun 2020 02:21:27 GMT  
		Size: 1.8 MB (1821769 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f8d4e38f4003d2c47b6f55a0926cdff91a7067c3c76dc4e2c2e2f2daece4c3e`  
		Last Modified: Tue, 09 Jun 2020 02:21:28 GMT  
		Size: 5.9 MB (5943337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77c6f49e3aaa7c6ab24d4a5af33b76359b34b2a1f8cf6d3e6b120651668fe5b6`  
		Last Modified: Tue, 09 Jun 2020 02:21:32 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21942e7c6286b9a4971d968173918ce206fee28d2f17ee9dcb4c551897b53b40`  
		Last Modified: Tue, 09 Jun 2020 02:21:32 GMT  
		Size: 338.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:1.6`

```console
$ docker pull spiped@sha256:f68d4f5a44d55612e4a5fb5ef03f87eb7e370254a26d5db4438a965ca47955b7
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
$ docker pull spiped@sha256:f507b4a86551d14d339abf790dac1c33db18bfb7284170964ee725265e10088d
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.3 MB (36266576 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:45c3b475d023dfa8186a606b7d1371e90494694ca0de5baf5f6e79fe68e66bf2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 15 May 2020 06:28:44 GMT
ADD file:7780c81c33e6cc5b6261af4a6c611cce0f39dec3131009bb297e65f12020c150 in / 
# Fri, 15 May 2020 06:28:44 GMT
CMD ["bash"]
# Sat, 16 May 2020 04:14:42 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Sat, 16 May 2020 04:14:47 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Sat, 16 May 2020 04:14:47 GMT
ENV SPIPED_VERSION=1.6.1
# Sat, 16 May 2020 04:14:47 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Sat, 16 May 2020 04:14:48 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Sat, 16 May 2020 04:15:31 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Sat, 16 May 2020 04:15:31 GMT
VOLUME [/spiped]
# Sat, 16 May 2020 04:15:32 GMT
WORKDIR /spiped
# Sat, 16 May 2020 04:15:32 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 16 May 2020 04:15:33 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 16 May 2020 04:15:33 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:afb6ec6fdc1c3ba04f7a56db32c5ff5ff38962dc4cd0ffdef5beaa0ce2eb77e2`  
		Last Modified: Fri, 15 May 2020 06:37:39 GMT  
		Size: 27.1 MB (27098756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf69e6d5168a8a643db7f3e097762e9a421e550edff25c02d584b76cec2578ce`  
		Last Modified: Sat, 16 May 2020 04:16:01 GMT  
		Size: 1.7 KB (1737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66db3f8998fea45888611f69f9e4fc3dcbff502f19c95bf902ffd7efbbe86966`  
		Last Modified: Sat, 16 May 2020 04:16:03 GMT  
		Size: 2.1 MB (2128102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e90a77d4c614a8407bcb3b077d130d797d0b128b6ad619c6d82573cb5da256ca`  
		Last Modified: Sat, 16 May 2020 04:16:04 GMT  
		Size: 7.0 MB (7037543 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:733772d709b4c96e4a851d79ab6edb5cc26d224468926544f23e40af781b29d8`  
		Last Modified: Sat, 16 May 2020 04:16:01 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11d35645dcf079b19bc3222e62897022743464d26c49ad631c80962369549efb`  
		Last Modified: Sat, 16 May 2020 04:16:01 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; arm variant v5

```console
$ docker pull spiped@sha256:89c0ca163f2aed719b25cfdfed1f04e927c7df87612a3b8249a847320b6b8bce
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.2 MB (32158596 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b151fa5d6a80c8c27152087cd00be0a1c5285e22caba7e411ecdbea1e5c4ce56`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 09 Jun 2020 00:51:58 GMT
ADD file:7fde417d1c70a9ef2b4e468f6e2ee4cbd3f340fb2d5b67ede087c81520c95f4a in / 
# Tue, 09 Jun 2020 00:51:59 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 01:20:07 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 09 Jun 2020 01:20:25 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 01:20:29 GMT
ENV SPIPED_VERSION=1.6.1
# Tue, 09 Jun 2020 01:20:33 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Tue, 09 Jun 2020 01:20:36 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Tue, 09 Jun 2020 01:21:51 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 09 Jun 2020 01:21:52 GMT
VOLUME [/spiped]
# Tue, 09 Jun 2020 01:21:52 GMT
WORKDIR /spiped
# Tue, 09 Jun 2020 01:21:53 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 09 Jun 2020 01:21:54 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 09 Jun 2020 01:21:54 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:5b11fc09c1a26b11a7df7d593adf43baff53c5cdba71cf8a87ae4a6dd17eb52c`  
		Last Modified: Tue, 09 Jun 2020 00:59:24 GMT  
		Size: 24.8 MB (24837249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a472cc54fb3976126466f6e8174720d2861ee99186f056d3aa776e2a94d13ae7`  
		Last Modified: Tue, 09 Jun 2020 01:22:16 GMT  
		Size: 1.7 KB (1725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:199d5cd61848e62c1013cc9a02e846466c14192913c2c3aa2ff178e44e02c53b`  
		Last Modified: Tue, 09 Jun 2020 01:22:16 GMT  
		Size: 1.8 MB (1839189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33ea1498c7e4ec77311232e10f6b24a9a59589d49a801733ae5319fba5aaa110`  
		Last Modified: Tue, 09 Jun 2020 01:22:19 GMT  
		Size: 5.5 MB (5479963 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95d84020e771e6045cb224230b0e3e07d9f77fcaf866dfca9dd82118dc3b39b1`  
		Last Modified: Tue, 09 Jun 2020 01:22:16 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dadc862a28f7f9a00d209adb7e25d470e36693b2f683c3efebc1ae9e8ce8800a`  
		Last Modified: Tue, 09 Jun 2020 01:22:16 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; arm variant v7

```console
$ docker pull spiped@sha256:82810696edb9b9cd3e20c069b4012756e7b42041c9542c8b5f839be38ca817c6
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.8 MB (29752935 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6260ddc16f2f5e54f0471a37563893cee16bbd967a1b1ac677bf3cac97f6a468`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 09 Jun 2020 01:01:24 GMT
ADD file:a35ca31d2a743d6a1738b1652f4f06c789abbca314d120f0e7e748311ac09ed2 in / 
# Tue, 09 Jun 2020 01:01:30 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 14:35:33 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 09 Jun 2020 14:35:42 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 14:35:43 GMT
ENV SPIPED_VERSION=1.6.1
# Tue, 09 Jun 2020 14:35:44 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Tue, 09 Jun 2020 14:35:45 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Tue, 09 Jun 2020 14:36:34 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 09 Jun 2020 14:36:35 GMT
VOLUME [/spiped]
# Tue, 09 Jun 2020 14:36:35 GMT
WORKDIR /spiped
# Tue, 09 Jun 2020 14:36:37 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 09 Jun 2020 14:36:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 09 Jun 2020 14:36:40 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:2dd003996c9ab82cac8112be0a4c04068e666e7a5d0cce3c65fb8f064de284e7`  
		Last Modified: Tue, 09 Jun 2020 01:10:25 GMT  
		Size: 22.7 MB (22705913 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92ddd3a5f3e7321eaaf8f41234d0e80dc3d7999e58c372bb5151417dc02a247c`  
		Last Modified: Tue, 09 Jun 2020 14:37:02 GMT  
		Size: 1.7 KB (1725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51282f9a582694ac89a16f9199036c324e405c496cb903b2691028c6464e2190`  
		Last Modified: Tue, 09 Jun 2020 14:37:02 GMT  
		Size: 1.8 MB (1759442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e51976ffb8ebca3a4d79b8161fb0e929f4cfd107ad09f09b5db452a67321c289`  
		Last Modified: Tue, 09 Jun 2020 14:37:04 GMT  
		Size: 5.3 MB (5285385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4657bf3b61375c1104a52dadec5dbc68c0fd4de727a013b5700db348ba5673b9`  
		Last Modified: Tue, 09 Jun 2020 14:37:02 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccf40741217b741d681454425549dc8910fbd06b638478c8494eeefd8f5d69b9`  
		Last Modified: Tue, 09 Jun 2020 14:37:02 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:cf2d29b06c1d1660698aa9de4dfb42854b60872ee61d9a012ee81240500612cc
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.8 MB (33773090 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ab2bf094b4eb433ebd77cb10ba397c7790ca5548502f326813e537efe5120cf3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 09 Jun 2020 01:52:01 GMT
ADD file:98823648634dfc3af50862b1e2da1028b23996a37adf43b1b0c3c5b29e94b9c7 in / 
# Tue, 09 Jun 2020 01:52:04 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 14:05:51 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 09 Jun 2020 14:05:59 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 14:05:59 GMT
ENV SPIPED_VERSION=1.6.1
# Tue, 09 Jun 2020 14:06:00 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Tue, 09 Jun 2020 14:06:01 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Tue, 09 Jun 2020 14:06:54 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 09 Jun 2020 14:06:55 GMT
VOLUME [/spiped]
# Tue, 09 Jun 2020 14:06:56 GMT
WORKDIR /spiped
# Tue, 09 Jun 2020 14:06:57 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 09 Jun 2020 14:06:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 09 Jun 2020 14:07:01 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:33cc09c9b190539635d7c971301f623d94fda5b4b5647966c6c240902119009f`  
		Last Modified: Tue, 09 Jun 2020 01:58:14 GMT  
		Size: 25.9 MB (25857704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7835e39ac04e97191d3dd883a78d8a2ca93f3b6d48edb467a020ed8aaa1b946c`  
		Last Modified: Tue, 09 Jun 2020 14:07:31 GMT  
		Size: 1.7 KB (1739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee4312c6f96572f3c7d9ba2921a53cf81d20e60ad38a4c67bdd72315940053f4`  
		Last Modified: Tue, 09 Jun 2020 14:07:31 GMT  
		Size: 2.0 MB (2007810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:108dcfd4a32f6e61f1aef4d1ed22a8a2f605529274e35f409d13a193b9a57ed4`  
		Last Modified: Tue, 09 Jun 2020 14:07:33 GMT  
		Size: 5.9 MB (5905367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42a4b05897e656cc187436d888abadd301fd521d43face9f8209586bbc697a7b`  
		Last Modified: Tue, 09 Jun 2020 14:07:31 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01a29dbcea99a23350569144e18f38a4733168c5bcfa9cac0462f663b2372c74`  
		Last Modified: Tue, 09 Jun 2020 14:07:31 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; 386

```console
$ docker pull spiped@sha256:8a7fe6ecb46c7724c5dd6bd2a7baf3094995f1b8edb6303ab0d8c15326f58db0
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.5 MB (41522653 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:713e39173dd25078ab6cc68a487ea2a5d84df4d6edbbcaa33083260d555368a1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 15 May 2020 07:07:55 GMT
ADD file:0c3b44c83914e95e4604999a86af05023cdd2b2f795e71d737e428fae4a7e0ac in / 
# Fri, 15 May 2020 07:07:56 GMT
CMD ["bash"]
# Fri, 15 May 2020 17:47:58 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Fri, 15 May 2020 17:48:04 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 17:48:05 GMT
ENV SPIPED_VERSION=1.6.1
# Fri, 15 May 2020 17:48:05 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Fri, 15 May 2020 17:48:05 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 15 May 2020 17:48:34 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Fri, 15 May 2020 17:48:34 GMT
VOLUME [/spiped]
# Fri, 15 May 2020 17:48:35 GMT
WORKDIR /spiped
# Fri, 15 May 2020 17:48:35 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 15 May 2020 17:48:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 15 May 2020 17:48:35 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:a5695130085a13212b02bf2645a52af5b41dd13e6dc9b29e2d7f357e1525aa48`  
		Last Modified: Fri, 15 May 2020 07:18:14 GMT  
		Size: 27.8 MB (27754922 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e46f1d7c78957f6663bbdcae7eb426e522750e8faf0a4174aed6c870289a058a`  
		Last Modified: Fri, 15 May 2020 17:48:55 GMT  
		Size: 1.7 KB (1731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94e9f3b4ac445b90a62301fd6363399326afdaced0908dfc316fbd74440a1fb2`  
		Last Modified: Fri, 15 May 2020 17:48:54 GMT  
		Size: 2.1 MB (2132373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e4350ab499cd08936f3d1a5c3662216bcbae435f2633319ba851eb2b3d1e00c`  
		Last Modified: Fri, 15 May 2020 17:49:03 GMT  
		Size: 11.6 MB (11633192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7d89781ff63fa52d84afbfa5beb9e63ad4cce6887c070fc07192d8abf85ccdc`  
		Last Modified: Fri, 15 May 2020 17:48:54 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:842d315391120a0e63fdb908daa3bdc3503566f8fa14d97cfcf770d05a50fbcd`  
		Last Modified: Fri, 15 May 2020 17:48:54 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; mips64le

```console
$ docker pull spiped@sha256:4e421f96912b140825f38f5b8b110891bd94b05d2ec75f34db06d6d199c4cd23
```

-	Docker Version: 19.03.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.9 MB (33894402 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d7a5df5ccfcc99a4ea0d50a3c49e81ce52581ff1b5164e4b80e2aa7d30ebc035`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 09 Jun 2020 01:10:06 GMT
ADD file:faf18b832680e98050b98c329add242425904e64c6a5a491c22d33e9417ef323 in / 
# Tue, 09 Jun 2020 01:10:06 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 02:27:39 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 09 Jun 2020 02:27:52 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 02:27:53 GMT
ENV SPIPED_VERSION=1.6.1
# Tue, 09 Jun 2020 02:27:53 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Tue, 09 Jun 2020 02:27:53 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Tue, 09 Jun 2020 02:29:02 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 09 Jun 2020 02:29:02 GMT
VOLUME [/spiped]
# Tue, 09 Jun 2020 02:29:03 GMT
WORKDIR /spiped
# Tue, 09 Jun 2020 02:29:03 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 09 Jun 2020 02:29:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 09 Jun 2020 02:29:04 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:76f2a0c8ea98ebd699a77ced9c677e97cd54b038a8c5e89670af78f38b047b33`  
		Last Modified: Tue, 09 Jun 2020 01:18:14 GMT  
		Size: 25.8 MB (25764040 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b82a47bf90ed455b577c438c12fe80d5fffca13a04f2ca9cec59ab9d64e327e`  
		Last Modified: Tue, 09 Jun 2020 02:29:24 GMT  
		Size: 1.7 KB (1729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbadd9d5a8dc90e2e4dc21414c4a8f4f186c31bde690d68c02d8b6a7b2447424`  
		Last Modified: Tue, 09 Jun 2020 02:29:26 GMT  
		Size: 1.7 MB (1712010 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:185ec9c5c819764b267f21284fed16f6049bac02cfad96abfcaf94cec25b18db`  
		Last Modified: Tue, 09 Jun 2020 02:29:31 GMT  
		Size: 6.4 MB (6416186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96b41dd1f9192b0235e97b93042cd81b32447840f020a5d7cb74b3c2c2c66b47`  
		Last Modified: Tue, 09 Jun 2020 02:29:24 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7c7e5506bf0d6b81418a33b8e3d4dc7c9f3ba1affab0cb6e0472754ed33454c`  
		Last Modified: Tue, 09 Jun 2020 02:29:24 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; ppc64le

```console
$ docker pull spiped@sha256:e0fe7e1f234d59836f3389de1bed55614da9de22f60d4b99c5020395738e16b0
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.5 MB (39494690 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5f5c577483a0496c4220a1c2277b81e7efb989b306fd3b9696971e84a75553ed`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 09 Jun 2020 01:22:34 GMT
ADD file:796aad1a35ba276b8cccc19987c152a713db101b2b65e30923db753f5b7f4b0f in / 
# Tue, 09 Jun 2020 01:22:38 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 03:52:53 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 09 Jun 2020 03:53:15 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 03:53:19 GMT
ENV SPIPED_VERSION=1.6.1
# Tue, 09 Jun 2020 03:53:26 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Tue, 09 Jun 2020 03:53:30 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Tue, 09 Jun 2020 03:55:33 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 09 Jun 2020 03:55:39 GMT
VOLUME [/spiped]
# Tue, 09 Jun 2020 03:55:44 GMT
WORKDIR /spiped
# Tue, 09 Jun 2020 03:55:46 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 09 Jun 2020 03:55:49 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 09 Jun 2020 03:55:52 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:63dbb66c5119bb5086d9e6fb6b154211afc20b44ed136ab7df808f6044cfc6f1`  
		Last Modified: Tue, 09 Jun 2020 01:31:04 GMT  
		Size: 30.5 MB (30524405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cdfd1c0bee0e2e09274162abe2b977b3876128838d43bdc7eded948eec4bf3f`  
		Last Modified: Tue, 09 Jun 2020 03:56:13 GMT  
		Size: 1.7 KB (1734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48279681b065daff73ee3f8ed95b05bdbf278498522ecf1ecc4c88b9fdf37888`  
		Last Modified: Tue, 09 Jun 2020 03:56:13 GMT  
		Size: 2.2 MB (2224949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14a6d252cdc4299f3b8d5819bded4186749b023311b2b9426eace76eb1ae1f09`  
		Last Modified: Tue, 09 Jun 2020 03:56:15 GMT  
		Size: 6.7 MB (6743134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba6c95b5243cf1886f4f17eb961b37932f9d63fa92c3a74bdd80b48424525b67`  
		Last Modified: Tue, 09 Jun 2020 03:56:13 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d86b530154fc517e54378d0142464946d98da0d74a3659f716a9d62f6f958cd5`  
		Last Modified: Tue, 09 Jun 2020 03:56:13 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; s390x

```console
$ docker pull spiped@sha256:e2268b6aea33adcd0e93fa1a60fddc4b589b9145a4400b07beaa756100f6ac54
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.5 MB (33479972 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8b6fc4e4a7364dee9d160cba7e4f9eb1db130b4b86902f49ef7ad7fc117f4f3e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 09 Jun 2020 01:42:37 GMT
ADD file:b21d426de40a194c6c76ed27593f33fb1ea470e15d4d43b00d7601472110de1a in / 
# Tue, 09 Jun 2020 01:42:38 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 02:20:52 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 09 Jun 2020 02:20:55 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 02:20:55 GMT
ENV SPIPED_VERSION=1.6.1
# Tue, 09 Jun 2020 02:20:56 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Tue, 09 Jun 2020 02:20:56 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Tue, 09 Jun 2020 02:21:11 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 09 Jun 2020 02:21:12 GMT
VOLUME [/spiped]
# Tue, 09 Jun 2020 02:21:12 GMT
WORKDIR /spiped
# Tue, 09 Jun 2020 02:21:12 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 09 Jun 2020 02:21:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 09 Jun 2020 02:21:13 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:405e75bf6bb0104d67fcebf58e07cd21bf344589df9c1a41c00354a60ea3a604`  
		Last Modified: Tue, 09 Jun 2020 01:46:30 GMT  
		Size: 25.7 MB (25712668 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17b0d5c87b23ce137e58201b2c08e71d5ea9d83dd59fa3909aa2c53f614d5c10`  
		Last Modified: Tue, 09 Jun 2020 02:21:27 GMT  
		Size: 1.7 KB (1731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eee2a9d7f4f7fcd8891c08e77d7f1994667fd23ca8313160ee58b02eecf8fcfa`  
		Last Modified: Tue, 09 Jun 2020 02:21:27 GMT  
		Size: 1.8 MB (1821769 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f8d4e38f4003d2c47b6f55a0926cdff91a7067c3c76dc4e2c2e2f2daece4c3e`  
		Last Modified: Tue, 09 Jun 2020 02:21:28 GMT  
		Size: 5.9 MB (5943337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77c6f49e3aaa7c6ab24d4a5af33b76359b34b2a1f8cf6d3e6b120651668fe5b6`  
		Last Modified: Tue, 09 Jun 2020 02:21:32 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21942e7c6286b9a4971d968173918ce206fee28d2f17ee9dcb4c551897b53b40`  
		Last Modified: Tue, 09 Jun 2020 02:21:32 GMT  
		Size: 338.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:1.6.1`

```console
$ docker pull spiped@sha256:f68d4f5a44d55612e4a5fb5ef03f87eb7e370254a26d5db4438a965ca47955b7
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
$ docker pull spiped@sha256:f507b4a86551d14d339abf790dac1c33db18bfb7284170964ee725265e10088d
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.3 MB (36266576 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:45c3b475d023dfa8186a606b7d1371e90494694ca0de5baf5f6e79fe68e66bf2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 15 May 2020 06:28:44 GMT
ADD file:7780c81c33e6cc5b6261af4a6c611cce0f39dec3131009bb297e65f12020c150 in / 
# Fri, 15 May 2020 06:28:44 GMT
CMD ["bash"]
# Sat, 16 May 2020 04:14:42 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Sat, 16 May 2020 04:14:47 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Sat, 16 May 2020 04:14:47 GMT
ENV SPIPED_VERSION=1.6.1
# Sat, 16 May 2020 04:14:47 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Sat, 16 May 2020 04:14:48 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Sat, 16 May 2020 04:15:31 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Sat, 16 May 2020 04:15:31 GMT
VOLUME [/spiped]
# Sat, 16 May 2020 04:15:32 GMT
WORKDIR /spiped
# Sat, 16 May 2020 04:15:32 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 16 May 2020 04:15:33 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 16 May 2020 04:15:33 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:afb6ec6fdc1c3ba04f7a56db32c5ff5ff38962dc4cd0ffdef5beaa0ce2eb77e2`  
		Last Modified: Fri, 15 May 2020 06:37:39 GMT  
		Size: 27.1 MB (27098756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf69e6d5168a8a643db7f3e097762e9a421e550edff25c02d584b76cec2578ce`  
		Last Modified: Sat, 16 May 2020 04:16:01 GMT  
		Size: 1.7 KB (1737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66db3f8998fea45888611f69f9e4fc3dcbff502f19c95bf902ffd7efbbe86966`  
		Last Modified: Sat, 16 May 2020 04:16:03 GMT  
		Size: 2.1 MB (2128102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e90a77d4c614a8407bcb3b077d130d797d0b128b6ad619c6d82573cb5da256ca`  
		Last Modified: Sat, 16 May 2020 04:16:04 GMT  
		Size: 7.0 MB (7037543 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:733772d709b4c96e4a851d79ab6edb5cc26d224468926544f23e40af781b29d8`  
		Last Modified: Sat, 16 May 2020 04:16:01 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11d35645dcf079b19bc3222e62897022743464d26c49ad631c80962369549efb`  
		Last Modified: Sat, 16 May 2020 04:16:01 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1` - linux; arm variant v5

```console
$ docker pull spiped@sha256:89c0ca163f2aed719b25cfdfed1f04e927c7df87612a3b8249a847320b6b8bce
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.2 MB (32158596 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b151fa5d6a80c8c27152087cd00be0a1c5285e22caba7e411ecdbea1e5c4ce56`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 09 Jun 2020 00:51:58 GMT
ADD file:7fde417d1c70a9ef2b4e468f6e2ee4cbd3f340fb2d5b67ede087c81520c95f4a in / 
# Tue, 09 Jun 2020 00:51:59 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 01:20:07 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 09 Jun 2020 01:20:25 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 01:20:29 GMT
ENV SPIPED_VERSION=1.6.1
# Tue, 09 Jun 2020 01:20:33 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Tue, 09 Jun 2020 01:20:36 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Tue, 09 Jun 2020 01:21:51 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 09 Jun 2020 01:21:52 GMT
VOLUME [/spiped]
# Tue, 09 Jun 2020 01:21:52 GMT
WORKDIR /spiped
# Tue, 09 Jun 2020 01:21:53 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 09 Jun 2020 01:21:54 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 09 Jun 2020 01:21:54 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:5b11fc09c1a26b11a7df7d593adf43baff53c5cdba71cf8a87ae4a6dd17eb52c`  
		Last Modified: Tue, 09 Jun 2020 00:59:24 GMT  
		Size: 24.8 MB (24837249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a472cc54fb3976126466f6e8174720d2861ee99186f056d3aa776e2a94d13ae7`  
		Last Modified: Tue, 09 Jun 2020 01:22:16 GMT  
		Size: 1.7 KB (1725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:199d5cd61848e62c1013cc9a02e846466c14192913c2c3aa2ff178e44e02c53b`  
		Last Modified: Tue, 09 Jun 2020 01:22:16 GMT  
		Size: 1.8 MB (1839189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33ea1498c7e4ec77311232e10f6b24a9a59589d49a801733ae5319fba5aaa110`  
		Last Modified: Tue, 09 Jun 2020 01:22:19 GMT  
		Size: 5.5 MB (5479963 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95d84020e771e6045cb224230b0e3e07d9f77fcaf866dfca9dd82118dc3b39b1`  
		Last Modified: Tue, 09 Jun 2020 01:22:16 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dadc862a28f7f9a00d209adb7e25d470e36693b2f683c3efebc1ae9e8ce8800a`  
		Last Modified: Tue, 09 Jun 2020 01:22:16 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1` - linux; arm variant v7

```console
$ docker pull spiped@sha256:82810696edb9b9cd3e20c069b4012756e7b42041c9542c8b5f839be38ca817c6
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.8 MB (29752935 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6260ddc16f2f5e54f0471a37563893cee16bbd967a1b1ac677bf3cac97f6a468`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 09 Jun 2020 01:01:24 GMT
ADD file:a35ca31d2a743d6a1738b1652f4f06c789abbca314d120f0e7e748311ac09ed2 in / 
# Tue, 09 Jun 2020 01:01:30 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 14:35:33 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 09 Jun 2020 14:35:42 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 14:35:43 GMT
ENV SPIPED_VERSION=1.6.1
# Tue, 09 Jun 2020 14:35:44 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Tue, 09 Jun 2020 14:35:45 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Tue, 09 Jun 2020 14:36:34 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 09 Jun 2020 14:36:35 GMT
VOLUME [/spiped]
# Tue, 09 Jun 2020 14:36:35 GMT
WORKDIR /spiped
# Tue, 09 Jun 2020 14:36:37 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 09 Jun 2020 14:36:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 09 Jun 2020 14:36:40 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:2dd003996c9ab82cac8112be0a4c04068e666e7a5d0cce3c65fb8f064de284e7`  
		Last Modified: Tue, 09 Jun 2020 01:10:25 GMT  
		Size: 22.7 MB (22705913 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92ddd3a5f3e7321eaaf8f41234d0e80dc3d7999e58c372bb5151417dc02a247c`  
		Last Modified: Tue, 09 Jun 2020 14:37:02 GMT  
		Size: 1.7 KB (1725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51282f9a582694ac89a16f9199036c324e405c496cb903b2691028c6464e2190`  
		Last Modified: Tue, 09 Jun 2020 14:37:02 GMT  
		Size: 1.8 MB (1759442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e51976ffb8ebca3a4d79b8161fb0e929f4cfd107ad09f09b5db452a67321c289`  
		Last Modified: Tue, 09 Jun 2020 14:37:04 GMT  
		Size: 5.3 MB (5285385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4657bf3b61375c1104a52dadec5dbc68c0fd4de727a013b5700db348ba5673b9`  
		Last Modified: Tue, 09 Jun 2020 14:37:02 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccf40741217b741d681454425549dc8910fbd06b638478c8494eeefd8f5d69b9`  
		Last Modified: Tue, 09 Jun 2020 14:37:02 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:cf2d29b06c1d1660698aa9de4dfb42854b60872ee61d9a012ee81240500612cc
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.8 MB (33773090 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ab2bf094b4eb433ebd77cb10ba397c7790ca5548502f326813e537efe5120cf3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 09 Jun 2020 01:52:01 GMT
ADD file:98823648634dfc3af50862b1e2da1028b23996a37adf43b1b0c3c5b29e94b9c7 in / 
# Tue, 09 Jun 2020 01:52:04 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 14:05:51 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 09 Jun 2020 14:05:59 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 14:05:59 GMT
ENV SPIPED_VERSION=1.6.1
# Tue, 09 Jun 2020 14:06:00 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Tue, 09 Jun 2020 14:06:01 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Tue, 09 Jun 2020 14:06:54 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 09 Jun 2020 14:06:55 GMT
VOLUME [/spiped]
# Tue, 09 Jun 2020 14:06:56 GMT
WORKDIR /spiped
# Tue, 09 Jun 2020 14:06:57 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 09 Jun 2020 14:06:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 09 Jun 2020 14:07:01 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:33cc09c9b190539635d7c971301f623d94fda5b4b5647966c6c240902119009f`  
		Last Modified: Tue, 09 Jun 2020 01:58:14 GMT  
		Size: 25.9 MB (25857704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7835e39ac04e97191d3dd883a78d8a2ca93f3b6d48edb467a020ed8aaa1b946c`  
		Last Modified: Tue, 09 Jun 2020 14:07:31 GMT  
		Size: 1.7 KB (1739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee4312c6f96572f3c7d9ba2921a53cf81d20e60ad38a4c67bdd72315940053f4`  
		Last Modified: Tue, 09 Jun 2020 14:07:31 GMT  
		Size: 2.0 MB (2007810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:108dcfd4a32f6e61f1aef4d1ed22a8a2f605529274e35f409d13a193b9a57ed4`  
		Last Modified: Tue, 09 Jun 2020 14:07:33 GMT  
		Size: 5.9 MB (5905367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42a4b05897e656cc187436d888abadd301fd521d43face9f8209586bbc697a7b`  
		Last Modified: Tue, 09 Jun 2020 14:07:31 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01a29dbcea99a23350569144e18f38a4733168c5bcfa9cac0462f663b2372c74`  
		Last Modified: Tue, 09 Jun 2020 14:07:31 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1` - linux; 386

```console
$ docker pull spiped@sha256:8a7fe6ecb46c7724c5dd6bd2a7baf3094995f1b8edb6303ab0d8c15326f58db0
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.5 MB (41522653 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:713e39173dd25078ab6cc68a487ea2a5d84df4d6edbbcaa33083260d555368a1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 15 May 2020 07:07:55 GMT
ADD file:0c3b44c83914e95e4604999a86af05023cdd2b2f795e71d737e428fae4a7e0ac in / 
# Fri, 15 May 2020 07:07:56 GMT
CMD ["bash"]
# Fri, 15 May 2020 17:47:58 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Fri, 15 May 2020 17:48:04 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 17:48:05 GMT
ENV SPIPED_VERSION=1.6.1
# Fri, 15 May 2020 17:48:05 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Fri, 15 May 2020 17:48:05 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 15 May 2020 17:48:34 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Fri, 15 May 2020 17:48:34 GMT
VOLUME [/spiped]
# Fri, 15 May 2020 17:48:35 GMT
WORKDIR /spiped
# Fri, 15 May 2020 17:48:35 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 15 May 2020 17:48:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 15 May 2020 17:48:35 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:a5695130085a13212b02bf2645a52af5b41dd13e6dc9b29e2d7f357e1525aa48`  
		Last Modified: Fri, 15 May 2020 07:18:14 GMT  
		Size: 27.8 MB (27754922 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e46f1d7c78957f6663bbdcae7eb426e522750e8faf0a4174aed6c870289a058a`  
		Last Modified: Fri, 15 May 2020 17:48:55 GMT  
		Size: 1.7 KB (1731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94e9f3b4ac445b90a62301fd6363399326afdaced0908dfc316fbd74440a1fb2`  
		Last Modified: Fri, 15 May 2020 17:48:54 GMT  
		Size: 2.1 MB (2132373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e4350ab499cd08936f3d1a5c3662216bcbae435f2633319ba851eb2b3d1e00c`  
		Last Modified: Fri, 15 May 2020 17:49:03 GMT  
		Size: 11.6 MB (11633192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7d89781ff63fa52d84afbfa5beb9e63ad4cce6887c070fc07192d8abf85ccdc`  
		Last Modified: Fri, 15 May 2020 17:48:54 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:842d315391120a0e63fdb908daa3bdc3503566f8fa14d97cfcf770d05a50fbcd`  
		Last Modified: Fri, 15 May 2020 17:48:54 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1` - linux; mips64le

```console
$ docker pull spiped@sha256:4e421f96912b140825f38f5b8b110891bd94b05d2ec75f34db06d6d199c4cd23
```

-	Docker Version: 19.03.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.9 MB (33894402 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d7a5df5ccfcc99a4ea0d50a3c49e81ce52581ff1b5164e4b80e2aa7d30ebc035`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 09 Jun 2020 01:10:06 GMT
ADD file:faf18b832680e98050b98c329add242425904e64c6a5a491c22d33e9417ef323 in / 
# Tue, 09 Jun 2020 01:10:06 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 02:27:39 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 09 Jun 2020 02:27:52 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 02:27:53 GMT
ENV SPIPED_VERSION=1.6.1
# Tue, 09 Jun 2020 02:27:53 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Tue, 09 Jun 2020 02:27:53 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Tue, 09 Jun 2020 02:29:02 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 09 Jun 2020 02:29:02 GMT
VOLUME [/spiped]
# Tue, 09 Jun 2020 02:29:03 GMT
WORKDIR /spiped
# Tue, 09 Jun 2020 02:29:03 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 09 Jun 2020 02:29:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 09 Jun 2020 02:29:04 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:76f2a0c8ea98ebd699a77ced9c677e97cd54b038a8c5e89670af78f38b047b33`  
		Last Modified: Tue, 09 Jun 2020 01:18:14 GMT  
		Size: 25.8 MB (25764040 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b82a47bf90ed455b577c438c12fe80d5fffca13a04f2ca9cec59ab9d64e327e`  
		Last Modified: Tue, 09 Jun 2020 02:29:24 GMT  
		Size: 1.7 KB (1729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbadd9d5a8dc90e2e4dc21414c4a8f4f186c31bde690d68c02d8b6a7b2447424`  
		Last Modified: Tue, 09 Jun 2020 02:29:26 GMT  
		Size: 1.7 MB (1712010 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:185ec9c5c819764b267f21284fed16f6049bac02cfad96abfcaf94cec25b18db`  
		Last Modified: Tue, 09 Jun 2020 02:29:31 GMT  
		Size: 6.4 MB (6416186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96b41dd1f9192b0235e97b93042cd81b32447840f020a5d7cb74b3c2c2c66b47`  
		Last Modified: Tue, 09 Jun 2020 02:29:24 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7c7e5506bf0d6b81418a33b8e3d4dc7c9f3ba1affab0cb6e0472754ed33454c`  
		Last Modified: Tue, 09 Jun 2020 02:29:24 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1` - linux; ppc64le

```console
$ docker pull spiped@sha256:e0fe7e1f234d59836f3389de1bed55614da9de22f60d4b99c5020395738e16b0
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.5 MB (39494690 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5f5c577483a0496c4220a1c2277b81e7efb989b306fd3b9696971e84a75553ed`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 09 Jun 2020 01:22:34 GMT
ADD file:796aad1a35ba276b8cccc19987c152a713db101b2b65e30923db753f5b7f4b0f in / 
# Tue, 09 Jun 2020 01:22:38 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 03:52:53 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 09 Jun 2020 03:53:15 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 03:53:19 GMT
ENV SPIPED_VERSION=1.6.1
# Tue, 09 Jun 2020 03:53:26 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Tue, 09 Jun 2020 03:53:30 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Tue, 09 Jun 2020 03:55:33 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 09 Jun 2020 03:55:39 GMT
VOLUME [/spiped]
# Tue, 09 Jun 2020 03:55:44 GMT
WORKDIR /spiped
# Tue, 09 Jun 2020 03:55:46 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 09 Jun 2020 03:55:49 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 09 Jun 2020 03:55:52 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:63dbb66c5119bb5086d9e6fb6b154211afc20b44ed136ab7df808f6044cfc6f1`  
		Last Modified: Tue, 09 Jun 2020 01:31:04 GMT  
		Size: 30.5 MB (30524405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cdfd1c0bee0e2e09274162abe2b977b3876128838d43bdc7eded948eec4bf3f`  
		Last Modified: Tue, 09 Jun 2020 03:56:13 GMT  
		Size: 1.7 KB (1734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48279681b065daff73ee3f8ed95b05bdbf278498522ecf1ecc4c88b9fdf37888`  
		Last Modified: Tue, 09 Jun 2020 03:56:13 GMT  
		Size: 2.2 MB (2224949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14a6d252cdc4299f3b8d5819bded4186749b023311b2b9426eace76eb1ae1f09`  
		Last Modified: Tue, 09 Jun 2020 03:56:15 GMT  
		Size: 6.7 MB (6743134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba6c95b5243cf1886f4f17eb961b37932f9d63fa92c3a74bdd80b48424525b67`  
		Last Modified: Tue, 09 Jun 2020 03:56:13 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d86b530154fc517e54378d0142464946d98da0d74a3659f716a9d62f6f958cd5`  
		Last Modified: Tue, 09 Jun 2020 03:56:13 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1` - linux; s390x

```console
$ docker pull spiped@sha256:e2268b6aea33adcd0e93fa1a60fddc4b589b9145a4400b07beaa756100f6ac54
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.5 MB (33479972 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8b6fc4e4a7364dee9d160cba7e4f9eb1db130b4b86902f49ef7ad7fc117f4f3e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 09 Jun 2020 01:42:37 GMT
ADD file:b21d426de40a194c6c76ed27593f33fb1ea470e15d4d43b00d7601472110de1a in / 
# Tue, 09 Jun 2020 01:42:38 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 02:20:52 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 09 Jun 2020 02:20:55 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 02:20:55 GMT
ENV SPIPED_VERSION=1.6.1
# Tue, 09 Jun 2020 02:20:56 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Tue, 09 Jun 2020 02:20:56 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Tue, 09 Jun 2020 02:21:11 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 09 Jun 2020 02:21:12 GMT
VOLUME [/spiped]
# Tue, 09 Jun 2020 02:21:12 GMT
WORKDIR /spiped
# Tue, 09 Jun 2020 02:21:12 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 09 Jun 2020 02:21:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 09 Jun 2020 02:21:13 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:405e75bf6bb0104d67fcebf58e07cd21bf344589df9c1a41c00354a60ea3a604`  
		Last Modified: Tue, 09 Jun 2020 01:46:30 GMT  
		Size: 25.7 MB (25712668 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17b0d5c87b23ce137e58201b2c08e71d5ea9d83dd59fa3909aa2c53f614d5c10`  
		Last Modified: Tue, 09 Jun 2020 02:21:27 GMT  
		Size: 1.7 KB (1731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eee2a9d7f4f7fcd8891c08e77d7f1994667fd23ca8313160ee58b02eecf8fcfa`  
		Last Modified: Tue, 09 Jun 2020 02:21:27 GMT  
		Size: 1.8 MB (1821769 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f8d4e38f4003d2c47b6f55a0926cdff91a7067c3c76dc4e2c2e2f2daece4c3e`  
		Last Modified: Tue, 09 Jun 2020 02:21:28 GMT  
		Size: 5.9 MB (5943337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77c6f49e3aaa7c6ab24d4a5af33b76359b34b2a1f8cf6d3e6b120651668fe5b6`  
		Last Modified: Tue, 09 Jun 2020 02:21:32 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21942e7c6286b9a4971d968173918ce206fee28d2f17ee9dcb4c551897b53b40`  
		Last Modified: Tue, 09 Jun 2020 02:21:32 GMT  
		Size: 338.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:1.6.1-alpine`

```console
$ docker pull spiped@sha256:2c6fe00e5c68d782286286f5ce6e67c5b5d182cdf886ea4fc8e85f1ff5af38e8
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
$ docker pull spiped@sha256:1670c0bedf4cde29b471b07e37cf2ecac7572eab7390e6f319e99a9d518d6c64
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 MB (2892533 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b7388fe097949fecec27fc47569b9454e25d605fa8b3bbad998579bb56613405`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 24 Apr 2020 01:05:21 GMT
ADD file:66a440394c2442570f1f060e25c86613cb2d88a8af0c71c5a4154b3570e9a805 in / 
# Fri, 24 Apr 2020 01:05:21 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 19:24:41 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 24 Apr 2020 19:24:42 GMT
RUN apk add --no-cache libssl1.1
# Fri, 24 Apr 2020 19:24:42 GMT
ENV SPIPED_VERSION=1.6.1
# Fri, 24 Apr 2020 19:24:42 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Fri, 24 Apr 2020 19:24:42 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 24 Apr 2020 19:24:58 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 24 Apr 2020 19:24:58 GMT
VOLUME [/spiped]
# Fri, 24 Apr 2020 19:24:58 GMT
WORKDIR /spiped
# Fri, 24 Apr 2020 19:24:58 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 24 Apr 2020 19:24:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Apr 2020 19:24:59 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:21c83c5242199776c232920ddb58cfa2a46b17e42ed831ca9001c8dbc532d22d`  
		Last Modified: Fri, 24 Apr 2020 01:06:07 GMT  
		Size: 2.8 MB (2795580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89008d600e9081fb81d2d7e8e6aa8507c9687b3dd3e56b2a17403caf42853ce7`  
		Last Modified: Fri, 24 Apr 2020 19:25:11 GMT  
		Size: 1.3 KB (1262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:646675b599220309e2ada934f30d0d976b4cd958316483de7cc5991e055ce61b`  
		Last Modified: Fri, 24 Apr 2020 19:25:12 GMT  
		Size: 6.3 KB (6334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87611a6ca8113a67cc77df7f11722a5925c0fa06ded08127f386d921e262d47d`  
		Last Modified: Fri, 24 Apr 2020 19:25:11 GMT  
		Size: 88.9 KB (88917 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6389f58338eae962a77c80f2c6a0ffd8f52eb490cd1902c8b333da59a1c46faa`  
		Last Modified: Fri, 24 Apr 2020 19:25:11 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b86813460026159fc213df32cdfda9c6bbdcc1e832029ce95c99f30f247e676`  
		Last Modified: Fri, 24 Apr 2020 19:25:12 GMT  
		Size: 345.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1-alpine` - linux; arm variant v6

```console
$ docker pull spiped@sha256:3c0350ac5d5cd7aaf3d93d8f3f7d1e9d1c0888b16731da96a22ccb20b49b531f
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 MB (2655539 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5f2d7b34485f1998f41c45c273be804816dae86f4496e8528867fe3784159e7b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 23 Apr 2020 15:51:35 GMT
ADD file:ef75120295e25a8e67c5ef378df2cf4ce9f7b83b44709452fcaf247b54fabd16 in / 
# Thu, 23 Apr 2020 15:51:36 GMT
CMD ["/bin/sh"]
# Thu, 23 Apr 2020 22:35:07 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 23 Apr 2020 22:35:09 GMT
RUN apk add --no-cache libssl1.1
# Thu, 23 Apr 2020 22:35:10 GMT
ENV SPIPED_VERSION=1.6.1
# Thu, 23 Apr 2020 22:35:10 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Thu, 23 Apr 2020 22:35:11 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 23 Apr 2020 22:35:37 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Thu, 23 Apr 2020 22:35:37 GMT
VOLUME [/spiped]
# Thu, 23 Apr 2020 22:35:38 GMT
WORKDIR /spiped
# Thu, 23 Apr 2020 22:35:39 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 23 Apr 2020 22:35:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Apr 2020 22:35:40 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:e745d1dc1c9e0be26166278da7632765ca98fa1be8179a7cc440b3bdc5671860`  
		Last Modified: Thu, 23 Apr 2020 15:52:15 GMT  
		Size: 2.6 MB (2572512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa1b8c67b45978a638cfe09240ed99c3f92f6ec5ed90fdc3228be33d65aba65e`  
		Last Modified: Thu, 23 Apr 2020 22:35:50 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cc5b5c9a3c98738e9c97f8a355f660e8b630466790fce376b6fa394efa65762`  
		Last Modified: Thu, 23 Apr 2020 22:35:51 GMT  
		Size: 6.3 KB (6326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c13e59f61c9a8509e3813070d46870440778325c0855dfd63a22bd87813428e1`  
		Last Modified: Thu, 23 Apr 2020 22:35:51 GMT  
		Size: 74.9 KB (74941 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c9a0727cd4b0cd75dd888a9ca44cd03adc1969d7e1861ed490045780002ac44`  
		Last Modified: Thu, 23 Apr 2020 22:35:51 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:857bf6c5552222716711317624492f63113effd58dc10e975f74f275444b8baa`  
		Last Modified: Thu, 23 Apr 2020 22:35:50 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1-alpine` - linux; arm variant v7

```console
$ docker pull spiped@sha256:a75d2b4c484e71a83bd1752e91d1d25f30799c3ee1430494e83268154edc9b4f
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 MB (2454828 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2fa554807a467b5e96447049fcb13bc6e7fee126058733f0cc24172beb312732`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 23 Apr 2020 22:04:44 GMT
ADD file:dabd2c1328a46961a58e93557d1039d6b98775cbdfe48ce875c109bb74615cb1 in / 
# Thu, 23 Apr 2020 22:04:45 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 04:14:59 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 24 Apr 2020 04:15:02 GMT
RUN apk add --no-cache libssl1.1
# Fri, 24 Apr 2020 04:15:02 GMT
ENV SPIPED_VERSION=1.6.1
# Fri, 24 Apr 2020 04:15:03 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Fri, 24 Apr 2020 04:15:04 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 24 Apr 2020 04:15:30 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 24 Apr 2020 04:15:30 GMT
VOLUME [/spiped]
# Fri, 24 Apr 2020 04:15:31 GMT
WORKDIR /spiped
# Fri, 24 Apr 2020 04:15:32 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 24 Apr 2020 04:15:33 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Apr 2020 04:15:33 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:ad20c94522902b824bd9ea4e65dc1cba24dca4fdadd5728ed7446c0f4550d1ff`  
		Last Modified: Thu, 23 Apr 2020 22:05:22 GMT  
		Size: 2.4 MB (2378640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5eb1adea1516ec3f4e151236f979a79b04121d2b8fab476668918b0c680a98aa`  
		Last Modified: Fri, 24 Apr 2020 04:15:49 GMT  
		Size: 1.3 KB (1286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72db7e58e30a264f15b4593c5ff6af5481ad577f3da660d4dc16c83b72e77176`  
		Last Modified: Fri, 24 Apr 2020 04:15:49 GMT  
		Size: 6.3 KB (6340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e868fb481151f8f3f73d24c647733c3ecf7b413ced859c1a8fd7a819cc2fdd3`  
		Last Modified: Fri, 24 Apr 2020 04:15:49 GMT  
		Size: 68.1 KB (68094 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a80e3146db25b624154d0900194778383ebdf35898331c684fefe3222eaa9f8`  
		Last Modified: Fri, 24 Apr 2020 04:15:49 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31aa835c2e31ed87aff90e07c38109e24a4e822a0676b4aba91d60519cc17de6`  
		Last Modified: Fri, 24 Apr 2020 04:15:49 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1-alpine` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:8f2a62b811f84b08b1fe7e18a3fb6dcd379bfca73eda2eee53048c7bc3d3553e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 MB (2808833 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bccfc824137404361e6033e1ef17ffc282e128ab855d4f22a8eecf2794b77701`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 24 Apr 2020 00:14:52 GMT
ADD file:75529f7e83edb6d0457a3b8bbfe33d4e3a12f339c5ace517d0f52dbedd9a146b in / 
# Fri, 24 Apr 2020 00:14:53 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 12:13:10 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 24 Apr 2020 12:13:12 GMT
RUN apk add --no-cache libssl1.1
# Fri, 24 Apr 2020 12:13:13 GMT
ENV SPIPED_VERSION=1.6.1
# Fri, 24 Apr 2020 12:13:14 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Fri, 24 Apr 2020 12:13:14 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 24 Apr 2020 12:13:40 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 24 Apr 2020 12:13:40 GMT
VOLUME [/spiped]
# Fri, 24 Apr 2020 12:13:41 GMT
WORKDIR /spiped
# Fri, 24 Apr 2020 12:13:42 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 24 Apr 2020 12:13:43 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Apr 2020 12:13:43 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:b038bcb63e9c8905cc879c957302f686a9b43f24a18dcfc4186ab236ddf04cad`  
		Last Modified: Fri, 24 Apr 2020 00:15:54 GMT  
		Size: 2.7 MB (2718734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbef55dc97b2b7a21b6bf9cf83b991c58c86ad0fe3e1a6f6050253f067e037cc`  
		Last Modified: Fri, 24 Apr 2020 12:14:02 GMT  
		Size: 1.3 KB (1288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7369917525ab29de34f65c7ffb1499470aa078dcb46d280d67175d5693154b5b`  
		Last Modified: Fri, 24 Apr 2020 12:14:02 GMT  
		Size: 6.3 KB (6348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fa4d0a88d2835e26bd5ba1f10e9c032d68f55a971f203ccbb3f95803f0ce216`  
		Last Modified: Fri, 24 Apr 2020 12:14:01 GMT  
		Size: 82.0 KB (81996 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43a1a60fac416a4bcf7dcdc29c6831b93f88e6d89fb9bd982f96f0a8601e14ae`  
		Last Modified: Fri, 24 Apr 2020 12:14:01 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06089ea6b11c1b6c92b6d10715efa2417f03c765cc262a88d1209e14c4eb2790`  
		Last Modified: Fri, 24 Apr 2020 12:14:01 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1-alpine` - linux; 386

```console
$ docker pull spiped@sha256:78999cb8561c2caff3c5846fe237439af72fba5288eed0845c4ce1bad191094c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 MB (2893567 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4b06cf71914272266c98138b1dddfe0971d0e4314ed3f295e8e498c80ab2db9e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 23 Apr 2020 21:16:11 GMT
ADD file:2e9fb162fdd20e7ac6e9edcb9e1ce9ece750f125c93824c5709a2800ae397f89 in / 
# Thu, 23 Apr 2020 21:16:11 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 08:56:34 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 24 Apr 2020 08:56:35 GMT
RUN apk add --no-cache libssl1.1
# Fri, 24 Apr 2020 08:56:35 GMT
ENV SPIPED_VERSION=1.6.1
# Fri, 24 Apr 2020 08:56:35 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Fri, 24 Apr 2020 08:56:35 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 24 Apr 2020 08:56:52 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 24 Apr 2020 08:56:52 GMT
VOLUME [/spiped]
# Fri, 24 Apr 2020 08:56:52 GMT
WORKDIR /spiped
# Fri, 24 Apr 2020 08:56:53 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 24 Apr 2020 08:56:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Apr 2020 08:56:53 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:294658c31053f36b08a64158e37d4fb84478e6fe8f4d5127c51a6334c8a3c36d`  
		Last Modified: Thu, 23 Apr 2020 21:16:37 GMT  
		Size: 2.8 MB (2787128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d99115e03ce3c950e46d67227979c778c7628cde48083cb2af971981006bf941`  
		Last Modified: Fri, 24 Apr 2020 08:57:05 GMT  
		Size: 1.3 KB (1262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c31b4b31c02617aa39baede00c19c62ea202856ecbac0cd402d02254ac730492`  
		Last Modified: Fri, 24 Apr 2020 08:57:05 GMT  
		Size: 6.3 KB (6347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2763a1020ba1dc39a2fe63a92c2a7d3d3db450b78c0003f74c3abd88d2a8690`  
		Last Modified: Fri, 24 Apr 2020 08:57:05 GMT  
		Size: 98.4 KB (98394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfc6e4f386ed41e9ad01c0e5b3e5932a75ad7682805e4aa0799c3415a80ec73a`  
		Last Modified: Fri, 24 Apr 2020 08:57:05 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7579e851392e7efa6fbe6a6a56b04fc171183c31ec1a1f72c1f27658e21286b`  
		Last Modified: Fri, 24 Apr 2020 08:57:05 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1-alpine` - linux; ppc64le

```console
$ docker pull spiped@sha256:9cfed93592b7fe82e50479c7a0822a48b1b5ab400a40cc2f1389ff26010e2411
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 MB (2915588 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b3490b3150b3b9ab6e3a99426c43e465e9bc6270b4eb8b13f9853fcb2b5b6930`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 23 Apr 2020 20:40:45 GMT
ADD file:2b585d18d1fcebf3ed725468d8f9642d2e6e32af8770f87b36d4601cc3a55316 in / 
# Thu, 23 Apr 2020 20:40:47 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 09:08:31 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 24 Apr 2020 09:08:37 GMT
RUN apk add --no-cache libssl1.1
# Fri, 24 Apr 2020 09:08:40 GMT
ENV SPIPED_VERSION=1.6.1
# Fri, 24 Apr 2020 09:08:44 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Fri, 24 Apr 2020 09:08:46 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 24 Apr 2020 09:09:11 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 24 Apr 2020 09:09:14 GMT
VOLUME [/spiped]
# Fri, 24 Apr 2020 09:09:18 GMT
WORKDIR /spiped
# Fri, 24 Apr 2020 09:09:19 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 24 Apr 2020 09:09:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Apr 2020 09:09:24 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:6694fcf3186b2073b4f09e0a2a753df9c8bcd31083e89a8a8f9a7001ad295328`  
		Last Modified: Thu, 23 Apr 2020 20:41:47 GMT  
		Size: 2.8 MB (2809956 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a85914d3a008a1f444b38165ce3fc56d3aa520d88133fdfdf654791a1de71f1a`  
		Last Modified: Fri, 24 Apr 2020 09:09:47 GMT  
		Size: 1.3 KB (1288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ec06a3c07a43eaf655e1f2a0e8576ada754f9af29c18bf3aa94950c92a799a1`  
		Last Modified: Fri, 24 Apr 2020 09:09:47 GMT  
		Size: 6.4 KB (6355 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7c1753650b9ad92aea131b35a681afa866570eb644d3bf8d47c5e2852e6efff`  
		Last Modified: Fri, 24 Apr 2020 09:09:47 GMT  
		Size: 97.5 KB (97519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e7e018c97ddc33d44c99d11c34b2d1601296151ec6f87cdc80cee41bbb6d294`  
		Last Modified: Fri, 24 Apr 2020 09:09:47 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a9dc529e21e37a4f215c5335a3b2a298697829328261d7a279e8dd9f1735fff`  
		Last Modified: Fri, 24 Apr 2020 09:09:47 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1-alpine` - linux; s390x

```console
$ docker pull spiped@sha256:5b9c1d41dd39f4984e651ea4535f43f4100936e674d6c3ae153f21b586a3c16d
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 MB (2663578 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:de69b324a894fbaf9b08ddc70f1ea37eef4e0b5eb83a102ed1689aba74076abe`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 23 Apr 2020 17:51:08 GMT
ADD file:53e1d2e5396547a2d7109e4b73078911bd069ae5d762f816d90e89ec9731ab13 in / 
# Thu, 23 Apr 2020 17:51:08 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 07:33:50 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 24 Apr 2020 07:33:51 GMT
RUN apk add --no-cache libssl1.1
# Fri, 24 Apr 2020 07:33:51 GMT
ENV SPIPED_VERSION=1.6.1
# Fri, 24 Apr 2020 07:33:52 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Fri, 24 Apr 2020 07:33:52 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 24 Apr 2020 07:34:01 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 24 Apr 2020 07:34:01 GMT
VOLUME [/spiped]
# Fri, 24 Apr 2020 07:34:01 GMT
WORKDIR /spiped
# Fri, 24 Apr 2020 07:34:02 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 24 Apr 2020 07:34:02 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Apr 2020 07:34:02 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:ab92bebeb6027138cd65f1f6658fd3428e21c60c95bdc978e0c57bf0b2a53970`  
		Last Modified: Thu, 23 Apr 2020 17:51:46 GMT  
		Size: 2.6 MB (2574478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3feb176fd2b09952c3679317f0be3a9a74423b300047dcb4dc4115d02775dc8`  
		Last Modified: Fri, 24 Apr 2020 07:34:18 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0701f42154bd44f03411750273dbc7f43f557ad52deb5aa079179b76140f5d4`  
		Last Modified: Fri, 24 Apr 2020 07:34:18 GMT  
		Size: 6.3 KB (6344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bcb5dd25d4a0e2547fb965eb04d708124eb3754eaf7fa0fe3a4cfd77ccd1fe3`  
		Last Modified: Fri, 24 Apr 2020 07:34:18 GMT  
		Size: 81.0 KB (80998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96d7e19bd791bc8c8db467add1c84d489de9b8c5c2b2f5b6013c495c35597b8b`  
		Last Modified: Fri, 24 Apr 2020 07:34:24 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:427d930f454293093665a4d2a97377fec8eae8a043e3c5cc97a84a1ec5ce23d5`  
		Last Modified: Fri, 24 Apr 2020 07:34:24 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:1.6-alpine`

```console
$ docker pull spiped@sha256:2c6fe00e5c68d782286286f5ce6e67c5b5d182cdf886ea4fc8e85f1ff5af38e8
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
$ docker pull spiped@sha256:1670c0bedf4cde29b471b07e37cf2ecac7572eab7390e6f319e99a9d518d6c64
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 MB (2892533 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b7388fe097949fecec27fc47569b9454e25d605fa8b3bbad998579bb56613405`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 24 Apr 2020 01:05:21 GMT
ADD file:66a440394c2442570f1f060e25c86613cb2d88a8af0c71c5a4154b3570e9a805 in / 
# Fri, 24 Apr 2020 01:05:21 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 19:24:41 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 24 Apr 2020 19:24:42 GMT
RUN apk add --no-cache libssl1.1
# Fri, 24 Apr 2020 19:24:42 GMT
ENV SPIPED_VERSION=1.6.1
# Fri, 24 Apr 2020 19:24:42 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Fri, 24 Apr 2020 19:24:42 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 24 Apr 2020 19:24:58 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 24 Apr 2020 19:24:58 GMT
VOLUME [/spiped]
# Fri, 24 Apr 2020 19:24:58 GMT
WORKDIR /spiped
# Fri, 24 Apr 2020 19:24:58 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 24 Apr 2020 19:24:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Apr 2020 19:24:59 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:21c83c5242199776c232920ddb58cfa2a46b17e42ed831ca9001c8dbc532d22d`  
		Last Modified: Fri, 24 Apr 2020 01:06:07 GMT  
		Size: 2.8 MB (2795580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89008d600e9081fb81d2d7e8e6aa8507c9687b3dd3e56b2a17403caf42853ce7`  
		Last Modified: Fri, 24 Apr 2020 19:25:11 GMT  
		Size: 1.3 KB (1262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:646675b599220309e2ada934f30d0d976b4cd958316483de7cc5991e055ce61b`  
		Last Modified: Fri, 24 Apr 2020 19:25:12 GMT  
		Size: 6.3 KB (6334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87611a6ca8113a67cc77df7f11722a5925c0fa06ded08127f386d921e262d47d`  
		Last Modified: Fri, 24 Apr 2020 19:25:11 GMT  
		Size: 88.9 KB (88917 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6389f58338eae962a77c80f2c6a0ffd8f52eb490cd1902c8b333da59a1c46faa`  
		Last Modified: Fri, 24 Apr 2020 19:25:11 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b86813460026159fc213df32cdfda9c6bbdcc1e832029ce95c99f30f247e676`  
		Last Modified: Fri, 24 Apr 2020 19:25:12 GMT  
		Size: 345.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; arm variant v6

```console
$ docker pull spiped@sha256:3c0350ac5d5cd7aaf3d93d8f3f7d1e9d1c0888b16731da96a22ccb20b49b531f
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 MB (2655539 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5f2d7b34485f1998f41c45c273be804816dae86f4496e8528867fe3784159e7b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 23 Apr 2020 15:51:35 GMT
ADD file:ef75120295e25a8e67c5ef378df2cf4ce9f7b83b44709452fcaf247b54fabd16 in / 
# Thu, 23 Apr 2020 15:51:36 GMT
CMD ["/bin/sh"]
# Thu, 23 Apr 2020 22:35:07 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 23 Apr 2020 22:35:09 GMT
RUN apk add --no-cache libssl1.1
# Thu, 23 Apr 2020 22:35:10 GMT
ENV SPIPED_VERSION=1.6.1
# Thu, 23 Apr 2020 22:35:10 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Thu, 23 Apr 2020 22:35:11 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 23 Apr 2020 22:35:37 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Thu, 23 Apr 2020 22:35:37 GMT
VOLUME [/spiped]
# Thu, 23 Apr 2020 22:35:38 GMT
WORKDIR /spiped
# Thu, 23 Apr 2020 22:35:39 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 23 Apr 2020 22:35:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Apr 2020 22:35:40 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:e745d1dc1c9e0be26166278da7632765ca98fa1be8179a7cc440b3bdc5671860`  
		Last Modified: Thu, 23 Apr 2020 15:52:15 GMT  
		Size: 2.6 MB (2572512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa1b8c67b45978a638cfe09240ed99c3f92f6ec5ed90fdc3228be33d65aba65e`  
		Last Modified: Thu, 23 Apr 2020 22:35:50 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cc5b5c9a3c98738e9c97f8a355f660e8b630466790fce376b6fa394efa65762`  
		Last Modified: Thu, 23 Apr 2020 22:35:51 GMT  
		Size: 6.3 KB (6326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c13e59f61c9a8509e3813070d46870440778325c0855dfd63a22bd87813428e1`  
		Last Modified: Thu, 23 Apr 2020 22:35:51 GMT  
		Size: 74.9 KB (74941 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c9a0727cd4b0cd75dd888a9ca44cd03adc1969d7e1861ed490045780002ac44`  
		Last Modified: Thu, 23 Apr 2020 22:35:51 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:857bf6c5552222716711317624492f63113effd58dc10e975f74f275444b8baa`  
		Last Modified: Thu, 23 Apr 2020 22:35:50 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; arm variant v7

```console
$ docker pull spiped@sha256:a75d2b4c484e71a83bd1752e91d1d25f30799c3ee1430494e83268154edc9b4f
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 MB (2454828 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2fa554807a467b5e96447049fcb13bc6e7fee126058733f0cc24172beb312732`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 23 Apr 2020 22:04:44 GMT
ADD file:dabd2c1328a46961a58e93557d1039d6b98775cbdfe48ce875c109bb74615cb1 in / 
# Thu, 23 Apr 2020 22:04:45 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 04:14:59 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 24 Apr 2020 04:15:02 GMT
RUN apk add --no-cache libssl1.1
# Fri, 24 Apr 2020 04:15:02 GMT
ENV SPIPED_VERSION=1.6.1
# Fri, 24 Apr 2020 04:15:03 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Fri, 24 Apr 2020 04:15:04 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 24 Apr 2020 04:15:30 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 24 Apr 2020 04:15:30 GMT
VOLUME [/spiped]
# Fri, 24 Apr 2020 04:15:31 GMT
WORKDIR /spiped
# Fri, 24 Apr 2020 04:15:32 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 24 Apr 2020 04:15:33 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Apr 2020 04:15:33 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:ad20c94522902b824bd9ea4e65dc1cba24dca4fdadd5728ed7446c0f4550d1ff`  
		Last Modified: Thu, 23 Apr 2020 22:05:22 GMT  
		Size: 2.4 MB (2378640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5eb1adea1516ec3f4e151236f979a79b04121d2b8fab476668918b0c680a98aa`  
		Last Modified: Fri, 24 Apr 2020 04:15:49 GMT  
		Size: 1.3 KB (1286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72db7e58e30a264f15b4593c5ff6af5481ad577f3da660d4dc16c83b72e77176`  
		Last Modified: Fri, 24 Apr 2020 04:15:49 GMT  
		Size: 6.3 KB (6340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e868fb481151f8f3f73d24c647733c3ecf7b413ced859c1a8fd7a819cc2fdd3`  
		Last Modified: Fri, 24 Apr 2020 04:15:49 GMT  
		Size: 68.1 KB (68094 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a80e3146db25b624154d0900194778383ebdf35898331c684fefe3222eaa9f8`  
		Last Modified: Fri, 24 Apr 2020 04:15:49 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31aa835c2e31ed87aff90e07c38109e24a4e822a0676b4aba91d60519cc17de6`  
		Last Modified: Fri, 24 Apr 2020 04:15:49 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:8f2a62b811f84b08b1fe7e18a3fb6dcd379bfca73eda2eee53048c7bc3d3553e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 MB (2808833 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bccfc824137404361e6033e1ef17ffc282e128ab855d4f22a8eecf2794b77701`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 24 Apr 2020 00:14:52 GMT
ADD file:75529f7e83edb6d0457a3b8bbfe33d4e3a12f339c5ace517d0f52dbedd9a146b in / 
# Fri, 24 Apr 2020 00:14:53 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 12:13:10 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 24 Apr 2020 12:13:12 GMT
RUN apk add --no-cache libssl1.1
# Fri, 24 Apr 2020 12:13:13 GMT
ENV SPIPED_VERSION=1.6.1
# Fri, 24 Apr 2020 12:13:14 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Fri, 24 Apr 2020 12:13:14 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 24 Apr 2020 12:13:40 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 24 Apr 2020 12:13:40 GMT
VOLUME [/spiped]
# Fri, 24 Apr 2020 12:13:41 GMT
WORKDIR /spiped
# Fri, 24 Apr 2020 12:13:42 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 24 Apr 2020 12:13:43 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Apr 2020 12:13:43 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:b038bcb63e9c8905cc879c957302f686a9b43f24a18dcfc4186ab236ddf04cad`  
		Last Modified: Fri, 24 Apr 2020 00:15:54 GMT  
		Size: 2.7 MB (2718734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbef55dc97b2b7a21b6bf9cf83b991c58c86ad0fe3e1a6f6050253f067e037cc`  
		Last Modified: Fri, 24 Apr 2020 12:14:02 GMT  
		Size: 1.3 KB (1288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7369917525ab29de34f65c7ffb1499470aa078dcb46d280d67175d5693154b5b`  
		Last Modified: Fri, 24 Apr 2020 12:14:02 GMT  
		Size: 6.3 KB (6348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fa4d0a88d2835e26bd5ba1f10e9c032d68f55a971f203ccbb3f95803f0ce216`  
		Last Modified: Fri, 24 Apr 2020 12:14:01 GMT  
		Size: 82.0 KB (81996 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43a1a60fac416a4bcf7dcdc29c6831b93f88e6d89fb9bd982f96f0a8601e14ae`  
		Last Modified: Fri, 24 Apr 2020 12:14:01 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06089ea6b11c1b6c92b6d10715efa2417f03c765cc262a88d1209e14c4eb2790`  
		Last Modified: Fri, 24 Apr 2020 12:14:01 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; 386

```console
$ docker pull spiped@sha256:78999cb8561c2caff3c5846fe237439af72fba5288eed0845c4ce1bad191094c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 MB (2893567 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4b06cf71914272266c98138b1dddfe0971d0e4314ed3f295e8e498c80ab2db9e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 23 Apr 2020 21:16:11 GMT
ADD file:2e9fb162fdd20e7ac6e9edcb9e1ce9ece750f125c93824c5709a2800ae397f89 in / 
# Thu, 23 Apr 2020 21:16:11 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 08:56:34 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 24 Apr 2020 08:56:35 GMT
RUN apk add --no-cache libssl1.1
# Fri, 24 Apr 2020 08:56:35 GMT
ENV SPIPED_VERSION=1.6.1
# Fri, 24 Apr 2020 08:56:35 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Fri, 24 Apr 2020 08:56:35 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 24 Apr 2020 08:56:52 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 24 Apr 2020 08:56:52 GMT
VOLUME [/spiped]
# Fri, 24 Apr 2020 08:56:52 GMT
WORKDIR /spiped
# Fri, 24 Apr 2020 08:56:53 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 24 Apr 2020 08:56:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Apr 2020 08:56:53 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:294658c31053f36b08a64158e37d4fb84478e6fe8f4d5127c51a6334c8a3c36d`  
		Last Modified: Thu, 23 Apr 2020 21:16:37 GMT  
		Size: 2.8 MB (2787128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d99115e03ce3c950e46d67227979c778c7628cde48083cb2af971981006bf941`  
		Last Modified: Fri, 24 Apr 2020 08:57:05 GMT  
		Size: 1.3 KB (1262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c31b4b31c02617aa39baede00c19c62ea202856ecbac0cd402d02254ac730492`  
		Last Modified: Fri, 24 Apr 2020 08:57:05 GMT  
		Size: 6.3 KB (6347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2763a1020ba1dc39a2fe63a92c2a7d3d3db450b78c0003f74c3abd88d2a8690`  
		Last Modified: Fri, 24 Apr 2020 08:57:05 GMT  
		Size: 98.4 KB (98394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfc6e4f386ed41e9ad01c0e5b3e5932a75ad7682805e4aa0799c3415a80ec73a`  
		Last Modified: Fri, 24 Apr 2020 08:57:05 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7579e851392e7efa6fbe6a6a56b04fc171183c31ec1a1f72c1f27658e21286b`  
		Last Modified: Fri, 24 Apr 2020 08:57:05 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; ppc64le

```console
$ docker pull spiped@sha256:9cfed93592b7fe82e50479c7a0822a48b1b5ab400a40cc2f1389ff26010e2411
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 MB (2915588 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b3490b3150b3b9ab6e3a99426c43e465e9bc6270b4eb8b13f9853fcb2b5b6930`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 23 Apr 2020 20:40:45 GMT
ADD file:2b585d18d1fcebf3ed725468d8f9642d2e6e32af8770f87b36d4601cc3a55316 in / 
# Thu, 23 Apr 2020 20:40:47 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 09:08:31 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 24 Apr 2020 09:08:37 GMT
RUN apk add --no-cache libssl1.1
# Fri, 24 Apr 2020 09:08:40 GMT
ENV SPIPED_VERSION=1.6.1
# Fri, 24 Apr 2020 09:08:44 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Fri, 24 Apr 2020 09:08:46 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 24 Apr 2020 09:09:11 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 24 Apr 2020 09:09:14 GMT
VOLUME [/spiped]
# Fri, 24 Apr 2020 09:09:18 GMT
WORKDIR /spiped
# Fri, 24 Apr 2020 09:09:19 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 24 Apr 2020 09:09:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Apr 2020 09:09:24 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:6694fcf3186b2073b4f09e0a2a753df9c8bcd31083e89a8a8f9a7001ad295328`  
		Last Modified: Thu, 23 Apr 2020 20:41:47 GMT  
		Size: 2.8 MB (2809956 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a85914d3a008a1f444b38165ce3fc56d3aa520d88133fdfdf654791a1de71f1a`  
		Last Modified: Fri, 24 Apr 2020 09:09:47 GMT  
		Size: 1.3 KB (1288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ec06a3c07a43eaf655e1f2a0e8576ada754f9af29c18bf3aa94950c92a799a1`  
		Last Modified: Fri, 24 Apr 2020 09:09:47 GMT  
		Size: 6.4 KB (6355 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7c1753650b9ad92aea131b35a681afa866570eb644d3bf8d47c5e2852e6efff`  
		Last Modified: Fri, 24 Apr 2020 09:09:47 GMT  
		Size: 97.5 KB (97519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e7e018c97ddc33d44c99d11c34b2d1601296151ec6f87cdc80cee41bbb6d294`  
		Last Modified: Fri, 24 Apr 2020 09:09:47 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a9dc529e21e37a4f215c5335a3b2a298697829328261d7a279e8dd9f1735fff`  
		Last Modified: Fri, 24 Apr 2020 09:09:47 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; s390x

```console
$ docker pull spiped@sha256:5b9c1d41dd39f4984e651ea4535f43f4100936e674d6c3ae153f21b586a3c16d
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 MB (2663578 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:de69b324a894fbaf9b08ddc70f1ea37eef4e0b5eb83a102ed1689aba74076abe`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 23 Apr 2020 17:51:08 GMT
ADD file:53e1d2e5396547a2d7109e4b73078911bd069ae5d762f816d90e89ec9731ab13 in / 
# Thu, 23 Apr 2020 17:51:08 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 07:33:50 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 24 Apr 2020 07:33:51 GMT
RUN apk add --no-cache libssl1.1
# Fri, 24 Apr 2020 07:33:51 GMT
ENV SPIPED_VERSION=1.6.1
# Fri, 24 Apr 2020 07:33:52 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Fri, 24 Apr 2020 07:33:52 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 24 Apr 2020 07:34:01 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 24 Apr 2020 07:34:01 GMT
VOLUME [/spiped]
# Fri, 24 Apr 2020 07:34:01 GMT
WORKDIR /spiped
# Fri, 24 Apr 2020 07:34:02 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 24 Apr 2020 07:34:02 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Apr 2020 07:34:02 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:ab92bebeb6027138cd65f1f6658fd3428e21c60c95bdc978e0c57bf0b2a53970`  
		Last Modified: Thu, 23 Apr 2020 17:51:46 GMT  
		Size: 2.6 MB (2574478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3feb176fd2b09952c3679317f0be3a9a74423b300047dcb4dc4115d02775dc8`  
		Last Modified: Fri, 24 Apr 2020 07:34:18 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0701f42154bd44f03411750273dbc7f43f557ad52deb5aa079179b76140f5d4`  
		Last Modified: Fri, 24 Apr 2020 07:34:18 GMT  
		Size: 6.3 KB (6344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bcb5dd25d4a0e2547fb965eb04d708124eb3754eaf7fa0fe3a4cfd77ccd1fe3`  
		Last Modified: Fri, 24 Apr 2020 07:34:18 GMT  
		Size: 81.0 KB (80998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96d7e19bd791bc8c8db467add1c84d489de9b8c5c2b2f5b6013c495c35597b8b`  
		Last Modified: Fri, 24 Apr 2020 07:34:24 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:427d930f454293093665a4d2a97377fec8eae8a043e3c5cc97a84a1ec5ce23d5`  
		Last Modified: Fri, 24 Apr 2020 07:34:24 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:1-alpine`

```console
$ docker pull spiped@sha256:2c6fe00e5c68d782286286f5ce6e67c5b5d182cdf886ea4fc8e85f1ff5af38e8
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
$ docker pull spiped@sha256:1670c0bedf4cde29b471b07e37cf2ecac7572eab7390e6f319e99a9d518d6c64
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 MB (2892533 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b7388fe097949fecec27fc47569b9454e25d605fa8b3bbad998579bb56613405`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 24 Apr 2020 01:05:21 GMT
ADD file:66a440394c2442570f1f060e25c86613cb2d88a8af0c71c5a4154b3570e9a805 in / 
# Fri, 24 Apr 2020 01:05:21 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 19:24:41 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 24 Apr 2020 19:24:42 GMT
RUN apk add --no-cache libssl1.1
# Fri, 24 Apr 2020 19:24:42 GMT
ENV SPIPED_VERSION=1.6.1
# Fri, 24 Apr 2020 19:24:42 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Fri, 24 Apr 2020 19:24:42 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 24 Apr 2020 19:24:58 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 24 Apr 2020 19:24:58 GMT
VOLUME [/spiped]
# Fri, 24 Apr 2020 19:24:58 GMT
WORKDIR /spiped
# Fri, 24 Apr 2020 19:24:58 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 24 Apr 2020 19:24:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Apr 2020 19:24:59 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:21c83c5242199776c232920ddb58cfa2a46b17e42ed831ca9001c8dbc532d22d`  
		Last Modified: Fri, 24 Apr 2020 01:06:07 GMT  
		Size: 2.8 MB (2795580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89008d600e9081fb81d2d7e8e6aa8507c9687b3dd3e56b2a17403caf42853ce7`  
		Last Modified: Fri, 24 Apr 2020 19:25:11 GMT  
		Size: 1.3 KB (1262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:646675b599220309e2ada934f30d0d976b4cd958316483de7cc5991e055ce61b`  
		Last Modified: Fri, 24 Apr 2020 19:25:12 GMT  
		Size: 6.3 KB (6334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87611a6ca8113a67cc77df7f11722a5925c0fa06ded08127f386d921e262d47d`  
		Last Modified: Fri, 24 Apr 2020 19:25:11 GMT  
		Size: 88.9 KB (88917 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6389f58338eae962a77c80f2c6a0ffd8f52eb490cd1902c8b333da59a1c46faa`  
		Last Modified: Fri, 24 Apr 2020 19:25:11 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b86813460026159fc213df32cdfda9c6bbdcc1e832029ce95c99f30f247e676`  
		Last Modified: Fri, 24 Apr 2020 19:25:12 GMT  
		Size: 345.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; arm variant v6

```console
$ docker pull spiped@sha256:3c0350ac5d5cd7aaf3d93d8f3f7d1e9d1c0888b16731da96a22ccb20b49b531f
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 MB (2655539 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5f2d7b34485f1998f41c45c273be804816dae86f4496e8528867fe3784159e7b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 23 Apr 2020 15:51:35 GMT
ADD file:ef75120295e25a8e67c5ef378df2cf4ce9f7b83b44709452fcaf247b54fabd16 in / 
# Thu, 23 Apr 2020 15:51:36 GMT
CMD ["/bin/sh"]
# Thu, 23 Apr 2020 22:35:07 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 23 Apr 2020 22:35:09 GMT
RUN apk add --no-cache libssl1.1
# Thu, 23 Apr 2020 22:35:10 GMT
ENV SPIPED_VERSION=1.6.1
# Thu, 23 Apr 2020 22:35:10 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Thu, 23 Apr 2020 22:35:11 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 23 Apr 2020 22:35:37 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Thu, 23 Apr 2020 22:35:37 GMT
VOLUME [/spiped]
# Thu, 23 Apr 2020 22:35:38 GMT
WORKDIR /spiped
# Thu, 23 Apr 2020 22:35:39 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 23 Apr 2020 22:35:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Apr 2020 22:35:40 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:e745d1dc1c9e0be26166278da7632765ca98fa1be8179a7cc440b3bdc5671860`  
		Last Modified: Thu, 23 Apr 2020 15:52:15 GMT  
		Size: 2.6 MB (2572512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa1b8c67b45978a638cfe09240ed99c3f92f6ec5ed90fdc3228be33d65aba65e`  
		Last Modified: Thu, 23 Apr 2020 22:35:50 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cc5b5c9a3c98738e9c97f8a355f660e8b630466790fce376b6fa394efa65762`  
		Last Modified: Thu, 23 Apr 2020 22:35:51 GMT  
		Size: 6.3 KB (6326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c13e59f61c9a8509e3813070d46870440778325c0855dfd63a22bd87813428e1`  
		Last Modified: Thu, 23 Apr 2020 22:35:51 GMT  
		Size: 74.9 KB (74941 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c9a0727cd4b0cd75dd888a9ca44cd03adc1969d7e1861ed490045780002ac44`  
		Last Modified: Thu, 23 Apr 2020 22:35:51 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:857bf6c5552222716711317624492f63113effd58dc10e975f74f275444b8baa`  
		Last Modified: Thu, 23 Apr 2020 22:35:50 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; arm variant v7

```console
$ docker pull spiped@sha256:a75d2b4c484e71a83bd1752e91d1d25f30799c3ee1430494e83268154edc9b4f
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 MB (2454828 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2fa554807a467b5e96447049fcb13bc6e7fee126058733f0cc24172beb312732`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 23 Apr 2020 22:04:44 GMT
ADD file:dabd2c1328a46961a58e93557d1039d6b98775cbdfe48ce875c109bb74615cb1 in / 
# Thu, 23 Apr 2020 22:04:45 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 04:14:59 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 24 Apr 2020 04:15:02 GMT
RUN apk add --no-cache libssl1.1
# Fri, 24 Apr 2020 04:15:02 GMT
ENV SPIPED_VERSION=1.6.1
# Fri, 24 Apr 2020 04:15:03 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Fri, 24 Apr 2020 04:15:04 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 24 Apr 2020 04:15:30 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 24 Apr 2020 04:15:30 GMT
VOLUME [/spiped]
# Fri, 24 Apr 2020 04:15:31 GMT
WORKDIR /spiped
# Fri, 24 Apr 2020 04:15:32 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 24 Apr 2020 04:15:33 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Apr 2020 04:15:33 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:ad20c94522902b824bd9ea4e65dc1cba24dca4fdadd5728ed7446c0f4550d1ff`  
		Last Modified: Thu, 23 Apr 2020 22:05:22 GMT  
		Size: 2.4 MB (2378640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5eb1adea1516ec3f4e151236f979a79b04121d2b8fab476668918b0c680a98aa`  
		Last Modified: Fri, 24 Apr 2020 04:15:49 GMT  
		Size: 1.3 KB (1286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72db7e58e30a264f15b4593c5ff6af5481ad577f3da660d4dc16c83b72e77176`  
		Last Modified: Fri, 24 Apr 2020 04:15:49 GMT  
		Size: 6.3 KB (6340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e868fb481151f8f3f73d24c647733c3ecf7b413ced859c1a8fd7a819cc2fdd3`  
		Last Modified: Fri, 24 Apr 2020 04:15:49 GMT  
		Size: 68.1 KB (68094 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a80e3146db25b624154d0900194778383ebdf35898331c684fefe3222eaa9f8`  
		Last Modified: Fri, 24 Apr 2020 04:15:49 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31aa835c2e31ed87aff90e07c38109e24a4e822a0676b4aba91d60519cc17de6`  
		Last Modified: Fri, 24 Apr 2020 04:15:49 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:8f2a62b811f84b08b1fe7e18a3fb6dcd379bfca73eda2eee53048c7bc3d3553e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 MB (2808833 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bccfc824137404361e6033e1ef17ffc282e128ab855d4f22a8eecf2794b77701`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 24 Apr 2020 00:14:52 GMT
ADD file:75529f7e83edb6d0457a3b8bbfe33d4e3a12f339c5ace517d0f52dbedd9a146b in / 
# Fri, 24 Apr 2020 00:14:53 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 12:13:10 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 24 Apr 2020 12:13:12 GMT
RUN apk add --no-cache libssl1.1
# Fri, 24 Apr 2020 12:13:13 GMT
ENV SPIPED_VERSION=1.6.1
# Fri, 24 Apr 2020 12:13:14 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Fri, 24 Apr 2020 12:13:14 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 24 Apr 2020 12:13:40 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 24 Apr 2020 12:13:40 GMT
VOLUME [/spiped]
# Fri, 24 Apr 2020 12:13:41 GMT
WORKDIR /spiped
# Fri, 24 Apr 2020 12:13:42 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 24 Apr 2020 12:13:43 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Apr 2020 12:13:43 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:b038bcb63e9c8905cc879c957302f686a9b43f24a18dcfc4186ab236ddf04cad`  
		Last Modified: Fri, 24 Apr 2020 00:15:54 GMT  
		Size: 2.7 MB (2718734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbef55dc97b2b7a21b6bf9cf83b991c58c86ad0fe3e1a6f6050253f067e037cc`  
		Last Modified: Fri, 24 Apr 2020 12:14:02 GMT  
		Size: 1.3 KB (1288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7369917525ab29de34f65c7ffb1499470aa078dcb46d280d67175d5693154b5b`  
		Last Modified: Fri, 24 Apr 2020 12:14:02 GMT  
		Size: 6.3 KB (6348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fa4d0a88d2835e26bd5ba1f10e9c032d68f55a971f203ccbb3f95803f0ce216`  
		Last Modified: Fri, 24 Apr 2020 12:14:01 GMT  
		Size: 82.0 KB (81996 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43a1a60fac416a4bcf7dcdc29c6831b93f88e6d89fb9bd982f96f0a8601e14ae`  
		Last Modified: Fri, 24 Apr 2020 12:14:01 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06089ea6b11c1b6c92b6d10715efa2417f03c765cc262a88d1209e14c4eb2790`  
		Last Modified: Fri, 24 Apr 2020 12:14:01 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; 386

```console
$ docker pull spiped@sha256:78999cb8561c2caff3c5846fe237439af72fba5288eed0845c4ce1bad191094c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 MB (2893567 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4b06cf71914272266c98138b1dddfe0971d0e4314ed3f295e8e498c80ab2db9e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 23 Apr 2020 21:16:11 GMT
ADD file:2e9fb162fdd20e7ac6e9edcb9e1ce9ece750f125c93824c5709a2800ae397f89 in / 
# Thu, 23 Apr 2020 21:16:11 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 08:56:34 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 24 Apr 2020 08:56:35 GMT
RUN apk add --no-cache libssl1.1
# Fri, 24 Apr 2020 08:56:35 GMT
ENV SPIPED_VERSION=1.6.1
# Fri, 24 Apr 2020 08:56:35 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Fri, 24 Apr 2020 08:56:35 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 24 Apr 2020 08:56:52 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 24 Apr 2020 08:56:52 GMT
VOLUME [/spiped]
# Fri, 24 Apr 2020 08:56:52 GMT
WORKDIR /spiped
# Fri, 24 Apr 2020 08:56:53 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 24 Apr 2020 08:56:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Apr 2020 08:56:53 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:294658c31053f36b08a64158e37d4fb84478e6fe8f4d5127c51a6334c8a3c36d`  
		Last Modified: Thu, 23 Apr 2020 21:16:37 GMT  
		Size: 2.8 MB (2787128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d99115e03ce3c950e46d67227979c778c7628cde48083cb2af971981006bf941`  
		Last Modified: Fri, 24 Apr 2020 08:57:05 GMT  
		Size: 1.3 KB (1262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c31b4b31c02617aa39baede00c19c62ea202856ecbac0cd402d02254ac730492`  
		Last Modified: Fri, 24 Apr 2020 08:57:05 GMT  
		Size: 6.3 KB (6347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2763a1020ba1dc39a2fe63a92c2a7d3d3db450b78c0003f74c3abd88d2a8690`  
		Last Modified: Fri, 24 Apr 2020 08:57:05 GMT  
		Size: 98.4 KB (98394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfc6e4f386ed41e9ad01c0e5b3e5932a75ad7682805e4aa0799c3415a80ec73a`  
		Last Modified: Fri, 24 Apr 2020 08:57:05 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7579e851392e7efa6fbe6a6a56b04fc171183c31ec1a1f72c1f27658e21286b`  
		Last Modified: Fri, 24 Apr 2020 08:57:05 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; ppc64le

```console
$ docker pull spiped@sha256:9cfed93592b7fe82e50479c7a0822a48b1b5ab400a40cc2f1389ff26010e2411
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 MB (2915588 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b3490b3150b3b9ab6e3a99426c43e465e9bc6270b4eb8b13f9853fcb2b5b6930`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 23 Apr 2020 20:40:45 GMT
ADD file:2b585d18d1fcebf3ed725468d8f9642d2e6e32af8770f87b36d4601cc3a55316 in / 
# Thu, 23 Apr 2020 20:40:47 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 09:08:31 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 24 Apr 2020 09:08:37 GMT
RUN apk add --no-cache libssl1.1
# Fri, 24 Apr 2020 09:08:40 GMT
ENV SPIPED_VERSION=1.6.1
# Fri, 24 Apr 2020 09:08:44 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Fri, 24 Apr 2020 09:08:46 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 24 Apr 2020 09:09:11 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 24 Apr 2020 09:09:14 GMT
VOLUME [/spiped]
# Fri, 24 Apr 2020 09:09:18 GMT
WORKDIR /spiped
# Fri, 24 Apr 2020 09:09:19 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 24 Apr 2020 09:09:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Apr 2020 09:09:24 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:6694fcf3186b2073b4f09e0a2a753df9c8bcd31083e89a8a8f9a7001ad295328`  
		Last Modified: Thu, 23 Apr 2020 20:41:47 GMT  
		Size: 2.8 MB (2809956 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a85914d3a008a1f444b38165ce3fc56d3aa520d88133fdfdf654791a1de71f1a`  
		Last Modified: Fri, 24 Apr 2020 09:09:47 GMT  
		Size: 1.3 KB (1288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ec06a3c07a43eaf655e1f2a0e8576ada754f9af29c18bf3aa94950c92a799a1`  
		Last Modified: Fri, 24 Apr 2020 09:09:47 GMT  
		Size: 6.4 KB (6355 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7c1753650b9ad92aea131b35a681afa866570eb644d3bf8d47c5e2852e6efff`  
		Last Modified: Fri, 24 Apr 2020 09:09:47 GMT  
		Size: 97.5 KB (97519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e7e018c97ddc33d44c99d11c34b2d1601296151ec6f87cdc80cee41bbb6d294`  
		Last Modified: Fri, 24 Apr 2020 09:09:47 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a9dc529e21e37a4f215c5335a3b2a298697829328261d7a279e8dd9f1735fff`  
		Last Modified: Fri, 24 Apr 2020 09:09:47 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; s390x

```console
$ docker pull spiped@sha256:5b9c1d41dd39f4984e651ea4535f43f4100936e674d6c3ae153f21b586a3c16d
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 MB (2663578 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:de69b324a894fbaf9b08ddc70f1ea37eef4e0b5eb83a102ed1689aba74076abe`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 23 Apr 2020 17:51:08 GMT
ADD file:53e1d2e5396547a2d7109e4b73078911bd069ae5d762f816d90e89ec9731ab13 in / 
# Thu, 23 Apr 2020 17:51:08 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 07:33:50 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 24 Apr 2020 07:33:51 GMT
RUN apk add --no-cache libssl1.1
# Fri, 24 Apr 2020 07:33:51 GMT
ENV SPIPED_VERSION=1.6.1
# Fri, 24 Apr 2020 07:33:52 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Fri, 24 Apr 2020 07:33:52 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 24 Apr 2020 07:34:01 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 24 Apr 2020 07:34:01 GMT
VOLUME [/spiped]
# Fri, 24 Apr 2020 07:34:01 GMT
WORKDIR /spiped
# Fri, 24 Apr 2020 07:34:02 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 24 Apr 2020 07:34:02 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Apr 2020 07:34:02 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:ab92bebeb6027138cd65f1f6658fd3428e21c60c95bdc978e0c57bf0b2a53970`  
		Last Modified: Thu, 23 Apr 2020 17:51:46 GMT  
		Size: 2.6 MB (2574478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3feb176fd2b09952c3679317f0be3a9a74423b300047dcb4dc4115d02775dc8`  
		Last Modified: Fri, 24 Apr 2020 07:34:18 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0701f42154bd44f03411750273dbc7f43f557ad52deb5aa079179b76140f5d4`  
		Last Modified: Fri, 24 Apr 2020 07:34:18 GMT  
		Size: 6.3 KB (6344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bcb5dd25d4a0e2547fb965eb04d708124eb3754eaf7fa0fe3a4cfd77ccd1fe3`  
		Last Modified: Fri, 24 Apr 2020 07:34:18 GMT  
		Size: 81.0 KB (80998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96d7e19bd791bc8c8db467add1c84d489de9b8c5c2b2f5b6013c495c35597b8b`  
		Last Modified: Fri, 24 Apr 2020 07:34:24 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:427d930f454293093665a4d2a97377fec8eae8a043e3c5cc97a84a1ec5ce23d5`  
		Last Modified: Fri, 24 Apr 2020 07:34:24 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:alpine`

```console
$ docker pull spiped@sha256:2c6fe00e5c68d782286286f5ce6e67c5b5d182cdf886ea4fc8e85f1ff5af38e8
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
$ docker pull spiped@sha256:1670c0bedf4cde29b471b07e37cf2ecac7572eab7390e6f319e99a9d518d6c64
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 MB (2892533 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b7388fe097949fecec27fc47569b9454e25d605fa8b3bbad998579bb56613405`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 24 Apr 2020 01:05:21 GMT
ADD file:66a440394c2442570f1f060e25c86613cb2d88a8af0c71c5a4154b3570e9a805 in / 
# Fri, 24 Apr 2020 01:05:21 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 19:24:41 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 24 Apr 2020 19:24:42 GMT
RUN apk add --no-cache libssl1.1
# Fri, 24 Apr 2020 19:24:42 GMT
ENV SPIPED_VERSION=1.6.1
# Fri, 24 Apr 2020 19:24:42 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Fri, 24 Apr 2020 19:24:42 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 24 Apr 2020 19:24:58 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 24 Apr 2020 19:24:58 GMT
VOLUME [/spiped]
# Fri, 24 Apr 2020 19:24:58 GMT
WORKDIR /spiped
# Fri, 24 Apr 2020 19:24:58 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 24 Apr 2020 19:24:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Apr 2020 19:24:59 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:21c83c5242199776c232920ddb58cfa2a46b17e42ed831ca9001c8dbc532d22d`  
		Last Modified: Fri, 24 Apr 2020 01:06:07 GMT  
		Size: 2.8 MB (2795580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89008d600e9081fb81d2d7e8e6aa8507c9687b3dd3e56b2a17403caf42853ce7`  
		Last Modified: Fri, 24 Apr 2020 19:25:11 GMT  
		Size: 1.3 KB (1262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:646675b599220309e2ada934f30d0d976b4cd958316483de7cc5991e055ce61b`  
		Last Modified: Fri, 24 Apr 2020 19:25:12 GMT  
		Size: 6.3 KB (6334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87611a6ca8113a67cc77df7f11722a5925c0fa06ded08127f386d921e262d47d`  
		Last Modified: Fri, 24 Apr 2020 19:25:11 GMT  
		Size: 88.9 KB (88917 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6389f58338eae962a77c80f2c6a0ffd8f52eb490cd1902c8b333da59a1c46faa`  
		Last Modified: Fri, 24 Apr 2020 19:25:11 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b86813460026159fc213df32cdfda9c6bbdcc1e832029ce95c99f30f247e676`  
		Last Modified: Fri, 24 Apr 2020 19:25:12 GMT  
		Size: 345.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; arm variant v6

```console
$ docker pull spiped@sha256:3c0350ac5d5cd7aaf3d93d8f3f7d1e9d1c0888b16731da96a22ccb20b49b531f
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 MB (2655539 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5f2d7b34485f1998f41c45c273be804816dae86f4496e8528867fe3784159e7b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 23 Apr 2020 15:51:35 GMT
ADD file:ef75120295e25a8e67c5ef378df2cf4ce9f7b83b44709452fcaf247b54fabd16 in / 
# Thu, 23 Apr 2020 15:51:36 GMT
CMD ["/bin/sh"]
# Thu, 23 Apr 2020 22:35:07 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 23 Apr 2020 22:35:09 GMT
RUN apk add --no-cache libssl1.1
# Thu, 23 Apr 2020 22:35:10 GMT
ENV SPIPED_VERSION=1.6.1
# Thu, 23 Apr 2020 22:35:10 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Thu, 23 Apr 2020 22:35:11 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 23 Apr 2020 22:35:37 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Thu, 23 Apr 2020 22:35:37 GMT
VOLUME [/spiped]
# Thu, 23 Apr 2020 22:35:38 GMT
WORKDIR /spiped
# Thu, 23 Apr 2020 22:35:39 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 23 Apr 2020 22:35:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Apr 2020 22:35:40 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:e745d1dc1c9e0be26166278da7632765ca98fa1be8179a7cc440b3bdc5671860`  
		Last Modified: Thu, 23 Apr 2020 15:52:15 GMT  
		Size: 2.6 MB (2572512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa1b8c67b45978a638cfe09240ed99c3f92f6ec5ed90fdc3228be33d65aba65e`  
		Last Modified: Thu, 23 Apr 2020 22:35:50 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cc5b5c9a3c98738e9c97f8a355f660e8b630466790fce376b6fa394efa65762`  
		Last Modified: Thu, 23 Apr 2020 22:35:51 GMT  
		Size: 6.3 KB (6326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c13e59f61c9a8509e3813070d46870440778325c0855dfd63a22bd87813428e1`  
		Last Modified: Thu, 23 Apr 2020 22:35:51 GMT  
		Size: 74.9 KB (74941 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c9a0727cd4b0cd75dd888a9ca44cd03adc1969d7e1861ed490045780002ac44`  
		Last Modified: Thu, 23 Apr 2020 22:35:51 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:857bf6c5552222716711317624492f63113effd58dc10e975f74f275444b8baa`  
		Last Modified: Thu, 23 Apr 2020 22:35:50 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; arm variant v7

```console
$ docker pull spiped@sha256:a75d2b4c484e71a83bd1752e91d1d25f30799c3ee1430494e83268154edc9b4f
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 MB (2454828 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2fa554807a467b5e96447049fcb13bc6e7fee126058733f0cc24172beb312732`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 23 Apr 2020 22:04:44 GMT
ADD file:dabd2c1328a46961a58e93557d1039d6b98775cbdfe48ce875c109bb74615cb1 in / 
# Thu, 23 Apr 2020 22:04:45 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 04:14:59 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 24 Apr 2020 04:15:02 GMT
RUN apk add --no-cache libssl1.1
# Fri, 24 Apr 2020 04:15:02 GMT
ENV SPIPED_VERSION=1.6.1
# Fri, 24 Apr 2020 04:15:03 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Fri, 24 Apr 2020 04:15:04 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 24 Apr 2020 04:15:30 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 24 Apr 2020 04:15:30 GMT
VOLUME [/spiped]
# Fri, 24 Apr 2020 04:15:31 GMT
WORKDIR /spiped
# Fri, 24 Apr 2020 04:15:32 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 24 Apr 2020 04:15:33 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Apr 2020 04:15:33 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:ad20c94522902b824bd9ea4e65dc1cba24dca4fdadd5728ed7446c0f4550d1ff`  
		Last Modified: Thu, 23 Apr 2020 22:05:22 GMT  
		Size: 2.4 MB (2378640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5eb1adea1516ec3f4e151236f979a79b04121d2b8fab476668918b0c680a98aa`  
		Last Modified: Fri, 24 Apr 2020 04:15:49 GMT  
		Size: 1.3 KB (1286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72db7e58e30a264f15b4593c5ff6af5481ad577f3da660d4dc16c83b72e77176`  
		Last Modified: Fri, 24 Apr 2020 04:15:49 GMT  
		Size: 6.3 KB (6340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e868fb481151f8f3f73d24c647733c3ecf7b413ced859c1a8fd7a819cc2fdd3`  
		Last Modified: Fri, 24 Apr 2020 04:15:49 GMT  
		Size: 68.1 KB (68094 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a80e3146db25b624154d0900194778383ebdf35898331c684fefe3222eaa9f8`  
		Last Modified: Fri, 24 Apr 2020 04:15:49 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31aa835c2e31ed87aff90e07c38109e24a4e822a0676b4aba91d60519cc17de6`  
		Last Modified: Fri, 24 Apr 2020 04:15:49 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:8f2a62b811f84b08b1fe7e18a3fb6dcd379bfca73eda2eee53048c7bc3d3553e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 MB (2808833 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bccfc824137404361e6033e1ef17ffc282e128ab855d4f22a8eecf2794b77701`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 24 Apr 2020 00:14:52 GMT
ADD file:75529f7e83edb6d0457a3b8bbfe33d4e3a12f339c5ace517d0f52dbedd9a146b in / 
# Fri, 24 Apr 2020 00:14:53 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 12:13:10 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 24 Apr 2020 12:13:12 GMT
RUN apk add --no-cache libssl1.1
# Fri, 24 Apr 2020 12:13:13 GMT
ENV SPIPED_VERSION=1.6.1
# Fri, 24 Apr 2020 12:13:14 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Fri, 24 Apr 2020 12:13:14 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 24 Apr 2020 12:13:40 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 24 Apr 2020 12:13:40 GMT
VOLUME [/spiped]
# Fri, 24 Apr 2020 12:13:41 GMT
WORKDIR /spiped
# Fri, 24 Apr 2020 12:13:42 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 24 Apr 2020 12:13:43 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Apr 2020 12:13:43 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:b038bcb63e9c8905cc879c957302f686a9b43f24a18dcfc4186ab236ddf04cad`  
		Last Modified: Fri, 24 Apr 2020 00:15:54 GMT  
		Size: 2.7 MB (2718734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbef55dc97b2b7a21b6bf9cf83b991c58c86ad0fe3e1a6f6050253f067e037cc`  
		Last Modified: Fri, 24 Apr 2020 12:14:02 GMT  
		Size: 1.3 KB (1288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7369917525ab29de34f65c7ffb1499470aa078dcb46d280d67175d5693154b5b`  
		Last Modified: Fri, 24 Apr 2020 12:14:02 GMT  
		Size: 6.3 KB (6348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fa4d0a88d2835e26bd5ba1f10e9c032d68f55a971f203ccbb3f95803f0ce216`  
		Last Modified: Fri, 24 Apr 2020 12:14:01 GMT  
		Size: 82.0 KB (81996 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43a1a60fac416a4bcf7dcdc29c6831b93f88e6d89fb9bd982f96f0a8601e14ae`  
		Last Modified: Fri, 24 Apr 2020 12:14:01 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06089ea6b11c1b6c92b6d10715efa2417f03c765cc262a88d1209e14c4eb2790`  
		Last Modified: Fri, 24 Apr 2020 12:14:01 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; 386

```console
$ docker pull spiped@sha256:78999cb8561c2caff3c5846fe237439af72fba5288eed0845c4ce1bad191094c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 MB (2893567 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4b06cf71914272266c98138b1dddfe0971d0e4314ed3f295e8e498c80ab2db9e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 23 Apr 2020 21:16:11 GMT
ADD file:2e9fb162fdd20e7ac6e9edcb9e1ce9ece750f125c93824c5709a2800ae397f89 in / 
# Thu, 23 Apr 2020 21:16:11 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 08:56:34 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 24 Apr 2020 08:56:35 GMT
RUN apk add --no-cache libssl1.1
# Fri, 24 Apr 2020 08:56:35 GMT
ENV SPIPED_VERSION=1.6.1
# Fri, 24 Apr 2020 08:56:35 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Fri, 24 Apr 2020 08:56:35 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 24 Apr 2020 08:56:52 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 24 Apr 2020 08:56:52 GMT
VOLUME [/spiped]
# Fri, 24 Apr 2020 08:56:52 GMT
WORKDIR /spiped
# Fri, 24 Apr 2020 08:56:53 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 24 Apr 2020 08:56:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Apr 2020 08:56:53 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:294658c31053f36b08a64158e37d4fb84478e6fe8f4d5127c51a6334c8a3c36d`  
		Last Modified: Thu, 23 Apr 2020 21:16:37 GMT  
		Size: 2.8 MB (2787128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d99115e03ce3c950e46d67227979c778c7628cde48083cb2af971981006bf941`  
		Last Modified: Fri, 24 Apr 2020 08:57:05 GMT  
		Size: 1.3 KB (1262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c31b4b31c02617aa39baede00c19c62ea202856ecbac0cd402d02254ac730492`  
		Last Modified: Fri, 24 Apr 2020 08:57:05 GMT  
		Size: 6.3 KB (6347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2763a1020ba1dc39a2fe63a92c2a7d3d3db450b78c0003f74c3abd88d2a8690`  
		Last Modified: Fri, 24 Apr 2020 08:57:05 GMT  
		Size: 98.4 KB (98394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfc6e4f386ed41e9ad01c0e5b3e5932a75ad7682805e4aa0799c3415a80ec73a`  
		Last Modified: Fri, 24 Apr 2020 08:57:05 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7579e851392e7efa6fbe6a6a56b04fc171183c31ec1a1f72c1f27658e21286b`  
		Last Modified: Fri, 24 Apr 2020 08:57:05 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; ppc64le

```console
$ docker pull spiped@sha256:9cfed93592b7fe82e50479c7a0822a48b1b5ab400a40cc2f1389ff26010e2411
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 MB (2915588 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b3490b3150b3b9ab6e3a99426c43e465e9bc6270b4eb8b13f9853fcb2b5b6930`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 23 Apr 2020 20:40:45 GMT
ADD file:2b585d18d1fcebf3ed725468d8f9642d2e6e32af8770f87b36d4601cc3a55316 in / 
# Thu, 23 Apr 2020 20:40:47 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 09:08:31 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 24 Apr 2020 09:08:37 GMT
RUN apk add --no-cache libssl1.1
# Fri, 24 Apr 2020 09:08:40 GMT
ENV SPIPED_VERSION=1.6.1
# Fri, 24 Apr 2020 09:08:44 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Fri, 24 Apr 2020 09:08:46 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 24 Apr 2020 09:09:11 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 24 Apr 2020 09:09:14 GMT
VOLUME [/spiped]
# Fri, 24 Apr 2020 09:09:18 GMT
WORKDIR /spiped
# Fri, 24 Apr 2020 09:09:19 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 24 Apr 2020 09:09:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Apr 2020 09:09:24 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:6694fcf3186b2073b4f09e0a2a753df9c8bcd31083e89a8a8f9a7001ad295328`  
		Last Modified: Thu, 23 Apr 2020 20:41:47 GMT  
		Size: 2.8 MB (2809956 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a85914d3a008a1f444b38165ce3fc56d3aa520d88133fdfdf654791a1de71f1a`  
		Last Modified: Fri, 24 Apr 2020 09:09:47 GMT  
		Size: 1.3 KB (1288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ec06a3c07a43eaf655e1f2a0e8576ada754f9af29c18bf3aa94950c92a799a1`  
		Last Modified: Fri, 24 Apr 2020 09:09:47 GMT  
		Size: 6.4 KB (6355 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7c1753650b9ad92aea131b35a681afa866570eb644d3bf8d47c5e2852e6efff`  
		Last Modified: Fri, 24 Apr 2020 09:09:47 GMT  
		Size: 97.5 KB (97519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e7e018c97ddc33d44c99d11c34b2d1601296151ec6f87cdc80cee41bbb6d294`  
		Last Modified: Fri, 24 Apr 2020 09:09:47 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a9dc529e21e37a4f215c5335a3b2a298697829328261d7a279e8dd9f1735fff`  
		Last Modified: Fri, 24 Apr 2020 09:09:47 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; s390x

```console
$ docker pull spiped@sha256:5b9c1d41dd39f4984e651ea4535f43f4100936e674d6c3ae153f21b586a3c16d
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 MB (2663578 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:de69b324a894fbaf9b08ddc70f1ea37eef4e0b5eb83a102ed1689aba74076abe`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 23 Apr 2020 17:51:08 GMT
ADD file:53e1d2e5396547a2d7109e4b73078911bd069ae5d762f816d90e89ec9731ab13 in / 
# Thu, 23 Apr 2020 17:51:08 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 07:33:50 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 24 Apr 2020 07:33:51 GMT
RUN apk add --no-cache libssl1.1
# Fri, 24 Apr 2020 07:33:51 GMT
ENV SPIPED_VERSION=1.6.1
# Fri, 24 Apr 2020 07:33:52 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Fri, 24 Apr 2020 07:33:52 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 24 Apr 2020 07:34:01 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 24 Apr 2020 07:34:01 GMT
VOLUME [/spiped]
# Fri, 24 Apr 2020 07:34:01 GMT
WORKDIR /spiped
# Fri, 24 Apr 2020 07:34:02 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 24 Apr 2020 07:34:02 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Apr 2020 07:34:02 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:ab92bebeb6027138cd65f1f6658fd3428e21c60c95bdc978e0c57bf0b2a53970`  
		Last Modified: Thu, 23 Apr 2020 17:51:46 GMT  
		Size: 2.6 MB (2574478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3feb176fd2b09952c3679317f0be3a9a74423b300047dcb4dc4115d02775dc8`  
		Last Modified: Fri, 24 Apr 2020 07:34:18 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0701f42154bd44f03411750273dbc7f43f557ad52deb5aa079179b76140f5d4`  
		Last Modified: Fri, 24 Apr 2020 07:34:18 GMT  
		Size: 6.3 KB (6344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bcb5dd25d4a0e2547fb965eb04d708124eb3754eaf7fa0fe3a4cfd77ccd1fe3`  
		Last Modified: Fri, 24 Apr 2020 07:34:18 GMT  
		Size: 81.0 KB (80998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96d7e19bd791bc8c8db467add1c84d489de9b8c5c2b2f5b6013c495c35597b8b`  
		Last Modified: Fri, 24 Apr 2020 07:34:24 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:427d930f454293093665a4d2a97377fec8eae8a043e3c5cc97a84a1ec5ce23d5`  
		Last Modified: Fri, 24 Apr 2020 07:34:24 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:latest`

```console
$ docker pull spiped@sha256:f68d4f5a44d55612e4a5fb5ef03f87eb7e370254a26d5db4438a965ca47955b7
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
$ docker pull spiped@sha256:f507b4a86551d14d339abf790dac1c33db18bfb7284170964ee725265e10088d
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.3 MB (36266576 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:45c3b475d023dfa8186a606b7d1371e90494694ca0de5baf5f6e79fe68e66bf2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 15 May 2020 06:28:44 GMT
ADD file:7780c81c33e6cc5b6261af4a6c611cce0f39dec3131009bb297e65f12020c150 in / 
# Fri, 15 May 2020 06:28:44 GMT
CMD ["bash"]
# Sat, 16 May 2020 04:14:42 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Sat, 16 May 2020 04:14:47 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Sat, 16 May 2020 04:14:47 GMT
ENV SPIPED_VERSION=1.6.1
# Sat, 16 May 2020 04:14:47 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Sat, 16 May 2020 04:14:48 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Sat, 16 May 2020 04:15:31 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Sat, 16 May 2020 04:15:31 GMT
VOLUME [/spiped]
# Sat, 16 May 2020 04:15:32 GMT
WORKDIR /spiped
# Sat, 16 May 2020 04:15:32 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 16 May 2020 04:15:33 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 16 May 2020 04:15:33 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:afb6ec6fdc1c3ba04f7a56db32c5ff5ff38962dc4cd0ffdef5beaa0ce2eb77e2`  
		Last Modified: Fri, 15 May 2020 06:37:39 GMT  
		Size: 27.1 MB (27098756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf69e6d5168a8a643db7f3e097762e9a421e550edff25c02d584b76cec2578ce`  
		Last Modified: Sat, 16 May 2020 04:16:01 GMT  
		Size: 1.7 KB (1737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66db3f8998fea45888611f69f9e4fc3dcbff502f19c95bf902ffd7efbbe86966`  
		Last Modified: Sat, 16 May 2020 04:16:03 GMT  
		Size: 2.1 MB (2128102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e90a77d4c614a8407bcb3b077d130d797d0b128b6ad619c6d82573cb5da256ca`  
		Last Modified: Sat, 16 May 2020 04:16:04 GMT  
		Size: 7.0 MB (7037543 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:733772d709b4c96e4a851d79ab6edb5cc26d224468926544f23e40af781b29d8`  
		Last Modified: Sat, 16 May 2020 04:16:01 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11d35645dcf079b19bc3222e62897022743464d26c49ad631c80962369549efb`  
		Last Modified: Sat, 16 May 2020 04:16:01 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; arm variant v5

```console
$ docker pull spiped@sha256:89c0ca163f2aed719b25cfdfed1f04e927c7df87612a3b8249a847320b6b8bce
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.2 MB (32158596 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b151fa5d6a80c8c27152087cd00be0a1c5285e22caba7e411ecdbea1e5c4ce56`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 09 Jun 2020 00:51:58 GMT
ADD file:7fde417d1c70a9ef2b4e468f6e2ee4cbd3f340fb2d5b67ede087c81520c95f4a in / 
# Tue, 09 Jun 2020 00:51:59 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 01:20:07 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 09 Jun 2020 01:20:25 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 01:20:29 GMT
ENV SPIPED_VERSION=1.6.1
# Tue, 09 Jun 2020 01:20:33 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Tue, 09 Jun 2020 01:20:36 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Tue, 09 Jun 2020 01:21:51 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 09 Jun 2020 01:21:52 GMT
VOLUME [/spiped]
# Tue, 09 Jun 2020 01:21:52 GMT
WORKDIR /spiped
# Tue, 09 Jun 2020 01:21:53 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 09 Jun 2020 01:21:54 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 09 Jun 2020 01:21:54 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:5b11fc09c1a26b11a7df7d593adf43baff53c5cdba71cf8a87ae4a6dd17eb52c`  
		Last Modified: Tue, 09 Jun 2020 00:59:24 GMT  
		Size: 24.8 MB (24837249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a472cc54fb3976126466f6e8174720d2861ee99186f056d3aa776e2a94d13ae7`  
		Last Modified: Tue, 09 Jun 2020 01:22:16 GMT  
		Size: 1.7 KB (1725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:199d5cd61848e62c1013cc9a02e846466c14192913c2c3aa2ff178e44e02c53b`  
		Last Modified: Tue, 09 Jun 2020 01:22:16 GMT  
		Size: 1.8 MB (1839189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33ea1498c7e4ec77311232e10f6b24a9a59589d49a801733ae5319fba5aaa110`  
		Last Modified: Tue, 09 Jun 2020 01:22:19 GMT  
		Size: 5.5 MB (5479963 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95d84020e771e6045cb224230b0e3e07d9f77fcaf866dfca9dd82118dc3b39b1`  
		Last Modified: Tue, 09 Jun 2020 01:22:16 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dadc862a28f7f9a00d209adb7e25d470e36693b2f683c3efebc1ae9e8ce8800a`  
		Last Modified: Tue, 09 Jun 2020 01:22:16 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; arm variant v7

```console
$ docker pull spiped@sha256:82810696edb9b9cd3e20c069b4012756e7b42041c9542c8b5f839be38ca817c6
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.8 MB (29752935 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6260ddc16f2f5e54f0471a37563893cee16bbd967a1b1ac677bf3cac97f6a468`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 09 Jun 2020 01:01:24 GMT
ADD file:a35ca31d2a743d6a1738b1652f4f06c789abbca314d120f0e7e748311ac09ed2 in / 
# Tue, 09 Jun 2020 01:01:30 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 14:35:33 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 09 Jun 2020 14:35:42 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 14:35:43 GMT
ENV SPIPED_VERSION=1.6.1
# Tue, 09 Jun 2020 14:35:44 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Tue, 09 Jun 2020 14:35:45 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Tue, 09 Jun 2020 14:36:34 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 09 Jun 2020 14:36:35 GMT
VOLUME [/spiped]
# Tue, 09 Jun 2020 14:36:35 GMT
WORKDIR /spiped
# Tue, 09 Jun 2020 14:36:37 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 09 Jun 2020 14:36:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 09 Jun 2020 14:36:40 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:2dd003996c9ab82cac8112be0a4c04068e666e7a5d0cce3c65fb8f064de284e7`  
		Last Modified: Tue, 09 Jun 2020 01:10:25 GMT  
		Size: 22.7 MB (22705913 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92ddd3a5f3e7321eaaf8f41234d0e80dc3d7999e58c372bb5151417dc02a247c`  
		Last Modified: Tue, 09 Jun 2020 14:37:02 GMT  
		Size: 1.7 KB (1725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51282f9a582694ac89a16f9199036c324e405c496cb903b2691028c6464e2190`  
		Last Modified: Tue, 09 Jun 2020 14:37:02 GMT  
		Size: 1.8 MB (1759442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e51976ffb8ebca3a4d79b8161fb0e929f4cfd107ad09f09b5db452a67321c289`  
		Last Modified: Tue, 09 Jun 2020 14:37:04 GMT  
		Size: 5.3 MB (5285385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4657bf3b61375c1104a52dadec5dbc68c0fd4de727a013b5700db348ba5673b9`  
		Last Modified: Tue, 09 Jun 2020 14:37:02 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccf40741217b741d681454425549dc8910fbd06b638478c8494eeefd8f5d69b9`  
		Last Modified: Tue, 09 Jun 2020 14:37:02 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:cf2d29b06c1d1660698aa9de4dfb42854b60872ee61d9a012ee81240500612cc
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.8 MB (33773090 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ab2bf094b4eb433ebd77cb10ba397c7790ca5548502f326813e537efe5120cf3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 09 Jun 2020 01:52:01 GMT
ADD file:98823648634dfc3af50862b1e2da1028b23996a37adf43b1b0c3c5b29e94b9c7 in / 
# Tue, 09 Jun 2020 01:52:04 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 14:05:51 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 09 Jun 2020 14:05:59 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 14:05:59 GMT
ENV SPIPED_VERSION=1.6.1
# Tue, 09 Jun 2020 14:06:00 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Tue, 09 Jun 2020 14:06:01 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Tue, 09 Jun 2020 14:06:54 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 09 Jun 2020 14:06:55 GMT
VOLUME [/spiped]
# Tue, 09 Jun 2020 14:06:56 GMT
WORKDIR /spiped
# Tue, 09 Jun 2020 14:06:57 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 09 Jun 2020 14:06:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 09 Jun 2020 14:07:01 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:33cc09c9b190539635d7c971301f623d94fda5b4b5647966c6c240902119009f`  
		Last Modified: Tue, 09 Jun 2020 01:58:14 GMT  
		Size: 25.9 MB (25857704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7835e39ac04e97191d3dd883a78d8a2ca93f3b6d48edb467a020ed8aaa1b946c`  
		Last Modified: Tue, 09 Jun 2020 14:07:31 GMT  
		Size: 1.7 KB (1739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee4312c6f96572f3c7d9ba2921a53cf81d20e60ad38a4c67bdd72315940053f4`  
		Last Modified: Tue, 09 Jun 2020 14:07:31 GMT  
		Size: 2.0 MB (2007810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:108dcfd4a32f6e61f1aef4d1ed22a8a2f605529274e35f409d13a193b9a57ed4`  
		Last Modified: Tue, 09 Jun 2020 14:07:33 GMT  
		Size: 5.9 MB (5905367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42a4b05897e656cc187436d888abadd301fd521d43face9f8209586bbc697a7b`  
		Last Modified: Tue, 09 Jun 2020 14:07:31 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01a29dbcea99a23350569144e18f38a4733168c5bcfa9cac0462f663b2372c74`  
		Last Modified: Tue, 09 Jun 2020 14:07:31 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; 386

```console
$ docker pull spiped@sha256:8a7fe6ecb46c7724c5dd6bd2a7baf3094995f1b8edb6303ab0d8c15326f58db0
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.5 MB (41522653 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:713e39173dd25078ab6cc68a487ea2a5d84df4d6edbbcaa33083260d555368a1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 15 May 2020 07:07:55 GMT
ADD file:0c3b44c83914e95e4604999a86af05023cdd2b2f795e71d737e428fae4a7e0ac in / 
# Fri, 15 May 2020 07:07:56 GMT
CMD ["bash"]
# Fri, 15 May 2020 17:47:58 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Fri, 15 May 2020 17:48:04 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 17:48:05 GMT
ENV SPIPED_VERSION=1.6.1
# Fri, 15 May 2020 17:48:05 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Fri, 15 May 2020 17:48:05 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 15 May 2020 17:48:34 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Fri, 15 May 2020 17:48:34 GMT
VOLUME [/spiped]
# Fri, 15 May 2020 17:48:35 GMT
WORKDIR /spiped
# Fri, 15 May 2020 17:48:35 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 15 May 2020 17:48:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 15 May 2020 17:48:35 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:a5695130085a13212b02bf2645a52af5b41dd13e6dc9b29e2d7f357e1525aa48`  
		Last Modified: Fri, 15 May 2020 07:18:14 GMT  
		Size: 27.8 MB (27754922 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e46f1d7c78957f6663bbdcae7eb426e522750e8faf0a4174aed6c870289a058a`  
		Last Modified: Fri, 15 May 2020 17:48:55 GMT  
		Size: 1.7 KB (1731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94e9f3b4ac445b90a62301fd6363399326afdaced0908dfc316fbd74440a1fb2`  
		Last Modified: Fri, 15 May 2020 17:48:54 GMT  
		Size: 2.1 MB (2132373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e4350ab499cd08936f3d1a5c3662216bcbae435f2633319ba851eb2b3d1e00c`  
		Last Modified: Fri, 15 May 2020 17:49:03 GMT  
		Size: 11.6 MB (11633192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7d89781ff63fa52d84afbfa5beb9e63ad4cce6887c070fc07192d8abf85ccdc`  
		Last Modified: Fri, 15 May 2020 17:48:54 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:842d315391120a0e63fdb908daa3bdc3503566f8fa14d97cfcf770d05a50fbcd`  
		Last Modified: Fri, 15 May 2020 17:48:54 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; mips64le

```console
$ docker pull spiped@sha256:4e421f96912b140825f38f5b8b110891bd94b05d2ec75f34db06d6d199c4cd23
```

-	Docker Version: 19.03.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.9 MB (33894402 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d7a5df5ccfcc99a4ea0d50a3c49e81ce52581ff1b5164e4b80e2aa7d30ebc035`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 09 Jun 2020 01:10:06 GMT
ADD file:faf18b832680e98050b98c329add242425904e64c6a5a491c22d33e9417ef323 in / 
# Tue, 09 Jun 2020 01:10:06 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 02:27:39 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 09 Jun 2020 02:27:52 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 02:27:53 GMT
ENV SPIPED_VERSION=1.6.1
# Tue, 09 Jun 2020 02:27:53 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Tue, 09 Jun 2020 02:27:53 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Tue, 09 Jun 2020 02:29:02 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 09 Jun 2020 02:29:02 GMT
VOLUME [/spiped]
# Tue, 09 Jun 2020 02:29:03 GMT
WORKDIR /spiped
# Tue, 09 Jun 2020 02:29:03 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 09 Jun 2020 02:29:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 09 Jun 2020 02:29:04 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:76f2a0c8ea98ebd699a77ced9c677e97cd54b038a8c5e89670af78f38b047b33`  
		Last Modified: Tue, 09 Jun 2020 01:18:14 GMT  
		Size: 25.8 MB (25764040 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b82a47bf90ed455b577c438c12fe80d5fffca13a04f2ca9cec59ab9d64e327e`  
		Last Modified: Tue, 09 Jun 2020 02:29:24 GMT  
		Size: 1.7 KB (1729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbadd9d5a8dc90e2e4dc21414c4a8f4f186c31bde690d68c02d8b6a7b2447424`  
		Last Modified: Tue, 09 Jun 2020 02:29:26 GMT  
		Size: 1.7 MB (1712010 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:185ec9c5c819764b267f21284fed16f6049bac02cfad96abfcaf94cec25b18db`  
		Last Modified: Tue, 09 Jun 2020 02:29:31 GMT  
		Size: 6.4 MB (6416186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96b41dd1f9192b0235e97b93042cd81b32447840f020a5d7cb74b3c2c2c66b47`  
		Last Modified: Tue, 09 Jun 2020 02:29:24 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7c7e5506bf0d6b81418a33b8e3d4dc7c9f3ba1affab0cb6e0472754ed33454c`  
		Last Modified: Tue, 09 Jun 2020 02:29:24 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; ppc64le

```console
$ docker pull spiped@sha256:e0fe7e1f234d59836f3389de1bed55614da9de22f60d4b99c5020395738e16b0
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.5 MB (39494690 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5f5c577483a0496c4220a1c2277b81e7efb989b306fd3b9696971e84a75553ed`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 09 Jun 2020 01:22:34 GMT
ADD file:796aad1a35ba276b8cccc19987c152a713db101b2b65e30923db753f5b7f4b0f in / 
# Tue, 09 Jun 2020 01:22:38 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 03:52:53 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 09 Jun 2020 03:53:15 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 03:53:19 GMT
ENV SPIPED_VERSION=1.6.1
# Tue, 09 Jun 2020 03:53:26 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Tue, 09 Jun 2020 03:53:30 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Tue, 09 Jun 2020 03:55:33 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 09 Jun 2020 03:55:39 GMT
VOLUME [/spiped]
# Tue, 09 Jun 2020 03:55:44 GMT
WORKDIR /spiped
# Tue, 09 Jun 2020 03:55:46 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 09 Jun 2020 03:55:49 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 09 Jun 2020 03:55:52 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:63dbb66c5119bb5086d9e6fb6b154211afc20b44ed136ab7df808f6044cfc6f1`  
		Last Modified: Tue, 09 Jun 2020 01:31:04 GMT  
		Size: 30.5 MB (30524405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cdfd1c0bee0e2e09274162abe2b977b3876128838d43bdc7eded948eec4bf3f`  
		Last Modified: Tue, 09 Jun 2020 03:56:13 GMT  
		Size: 1.7 KB (1734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48279681b065daff73ee3f8ed95b05bdbf278498522ecf1ecc4c88b9fdf37888`  
		Last Modified: Tue, 09 Jun 2020 03:56:13 GMT  
		Size: 2.2 MB (2224949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14a6d252cdc4299f3b8d5819bded4186749b023311b2b9426eace76eb1ae1f09`  
		Last Modified: Tue, 09 Jun 2020 03:56:15 GMT  
		Size: 6.7 MB (6743134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba6c95b5243cf1886f4f17eb961b37932f9d63fa92c3a74bdd80b48424525b67`  
		Last Modified: Tue, 09 Jun 2020 03:56:13 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d86b530154fc517e54378d0142464946d98da0d74a3659f716a9d62f6f958cd5`  
		Last Modified: Tue, 09 Jun 2020 03:56:13 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; s390x

```console
$ docker pull spiped@sha256:e2268b6aea33adcd0e93fa1a60fddc4b589b9145a4400b07beaa756100f6ac54
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.5 MB (33479972 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8b6fc4e4a7364dee9d160cba7e4f9eb1db130b4b86902f49ef7ad7fc117f4f3e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 09 Jun 2020 01:42:37 GMT
ADD file:b21d426de40a194c6c76ed27593f33fb1ea470e15d4d43b00d7601472110de1a in / 
# Tue, 09 Jun 2020 01:42:38 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 02:20:52 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 09 Jun 2020 02:20:55 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 02:20:55 GMT
ENV SPIPED_VERSION=1.6.1
# Tue, 09 Jun 2020 02:20:56 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Tue, 09 Jun 2020 02:20:56 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Tue, 09 Jun 2020 02:21:11 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 09 Jun 2020 02:21:12 GMT
VOLUME [/spiped]
# Tue, 09 Jun 2020 02:21:12 GMT
WORKDIR /spiped
# Tue, 09 Jun 2020 02:21:12 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 09 Jun 2020 02:21:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 09 Jun 2020 02:21:13 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:405e75bf6bb0104d67fcebf58e07cd21bf344589df9c1a41c00354a60ea3a604`  
		Last Modified: Tue, 09 Jun 2020 01:46:30 GMT  
		Size: 25.7 MB (25712668 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17b0d5c87b23ce137e58201b2c08e71d5ea9d83dd59fa3909aa2c53f614d5c10`  
		Last Modified: Tue, 09 Jun 2020 02:21:27 GMT  
		Size: 1.7 KB (1731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eee2a9d7f4f7fcd8891c08e77d7f1994667fd23ca8313160ee58b02eecf8fcfa`  
		Last Modified: Tue, 09 Jun 2020 02:21:27 GMT  
		Size: 1.8 MB (1821769 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f8d4e38f4003d2c47b6f55a0926cdff91a7067c3c76dc4e2c2e2f2daece4c3e`  
		Last Modified: Tue, 09 Jun 2020 02:21:28 GMT  
		Size: 5.9 MB (5943337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77c6f49e3aaa7c6ab24d4a5af33b76359b34b2a1f8cf6d3e6b120651668fe5b6`  
		Last Modified: Tue, 09 Jun 2020 02:21:32 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21942e7c6286b9a4971d968173918ce206fee28d2f17ee9dcb4c551897b53b40`  
		Last Modified: Tue, 09 Jun 2020 02:21:32 GMT  
		Size: 338.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
