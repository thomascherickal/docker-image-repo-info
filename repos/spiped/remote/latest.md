## `spiped:latest`

```console
$ docker pull spiped@sha256:57a64f2258adde594ef494be06fdbdbbc873d058339d758e6433e483f6b05b10
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
$ docker pull spiped@sha256:446e6d73b8e4f9d6ed3255435d4fd5a0d5cdf8453d37349fac5939ec7096ddde
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.3 MB (36259914 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2d40a43043a984e359c34fd3c040187e8a18bfa5b8fe8392d3553db9442211d1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 10 Sep 2020 00:23:29 GMT
ADD file:e7407f2294ad23634565820b9669b18ff2a2ca0212a7ec84b9c89d8550859954 in / 
# Thu, 10 Sep 2020 00:23:30 GMT
CMD ["bash"]
# Thu, 10 Sep 2020 20:50:35 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Thu, 10 Sep 2020 20:50:41 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Thu, 10 Sep 2020 20:50:41 GMT
ENV SPIPED_VERSION=1.6.1
# Thu, 10 Sep 2020 20:50:41 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Thu, 10 Sep 2020 20:50:41 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 10 Sep 2020 20:51:09 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 10 Sep 2020 20:51:10 GMT
VOLUME [/spiped]
# Thu, 10 Sep 2020 20:51:10 GMT
WORKDIR /spiped
# Thu, 10 Sep 2020 20:51:10 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 10 Sep 2020 20:51:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 10 Sep 2020 20:51:11 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:d121f8d1c4128ebc1e95e5bfad90a0189b84eadbbb2fbaad20cbb26d20b2c8a2`  
		Last Modified: Thu, 10 Sep 2020 00:34:02 GMT  
		Size: 27.1 MB (27092161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5dcb90c804f1c1a4407a7a3511ddf272cb455f0e4df6663cb2a6ca387c07839`  
		Last Modified: Thu, 10 Sep 2020 20:51:25 GMT  
		Size: 1.7 KB (1738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68ea5fe154b21fd7144c56fe18e437e58fcee4aa4a93d9b6dafc2d880ca95eb3`  
		Last Modified: Thu, 10 Sep 2020 20:51:25 GMT  
		Size: 2.1 MB (2128111 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd873a81046041ed0c53eea8499ca1407a2f7f9b326dddb094fea97e9b21f155`  
		Last Modified: Thu, 10 Sep 2020 20:51:26 GMT  
		Size: 7.0 MB (7037469 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8bfe495fdb491566fb6052bbc5ac30d8d68882e68fdf7e939a155ea1dfa481a`  
		Last Modified: Thu, 10 Sep 2020 20:51:25 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a73ec50edd47676d90de885e35ae6c033622e140a9d6e59734a51dd987aeec11`  
		Last Modified: Thu, 10 Sep 2020 20:51:25 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; arm variant v5

```console
$ docker pull spiped@sha256:0ffa7209cfe814b6558ab1e948cc440a965eb77f3af74f0e20e97e346d3b521f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.2 MB (32157276 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a4d6fefca0c0605222f639cdc3d28477e5036c67425fb388f16b2d1d0f3bb3df`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 09 Sep 2020 23:53:49 GMT
ADD file:34835d84d87e3ee1178aa150793d75a4d4a7a28c013ca3495dbcca2b570270bf in / 
# Wed, 09 Sep 2020 23:53:53 GMT
CMD ["bash"]
# Thu, 10 Sep 2020 00:24:20 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Thu, 10 Sep 2020 00:24:31 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Thu, 10 Sep 2020 00:24:32 GMT
ENV SPIPED_VERSION=1.6.1
# Thu, 10 Sep 2020 00:24:33 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Thu, 10 Sep 2020 00:24:34 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 10 Sep 2020 00:25:30 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 10 Sep 2020 00:25:32 GMT
VOLUME [/spiped]
# Thu, 10 Sep 2020 00:25:34 GMT
WORKDIR /spiped
# Thu, 10 Sep 2020 00:25:35 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 10 Sep 2020 00:25:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 10 Sep 2020 00:25:36 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:0a51b5143468e1b44dafa16fea3541e28e369071f6837337ee95e37f0ad81d99`  
		Last Modified: Thu, 10 Sep 2020 00:02:48 GMT  
		Size: 24.8 MB (24835974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c16e60014503eeb6a9de0642540ffe398b65110a92e105ea725fe64050f133c7`  
		Last Modified: Thu, 10 Sep 2020 00:25:57 GMT  
		Size: 1.7 KB (1731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e0bd36d1f55b67f92e906287f170c5ff225fa133082c4ac65bf0b026c8c1c61`  
		Last Modified: Thu, 10 Sep 2020 00:25:58 GMT  
		Size: 1.8 MB (1839179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c8ddea53fb3a57a5e46a257e877538608b0b699eabf62195c6787df35c041c0`  
		Last Modified: Thu, 10 Sep 2020 00:26:00 GMT  
		Size: 5.5 MB (5479920 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6dcc0f7c2e8d86cd9038ca26d518798de530b02f9d6a2625dea4fa37168eaf3f`  
		Last Modified: Thu, 10 Sep 2020 00:25:58 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:416e4e1edd36cc0942d8b1f16299321dcea276b757a77e44a69544b5f2716446`  
		Last Modified: Thu, 10 Sep 2020 00:25:57 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; arm variant v7

```console
$ docker pull spiped@sha256:c59e0e45e0593062d8d86f3c710d7110ad5ccbdc8b2cd3a97da5eb2c00a9c53d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.7 MB (29747113 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f45758e0b37d9d654f80bcce288a0fb1228bef936924d11d94ba5577948f4fb2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 10 Sep 2020 00:08:04 GMT
ADD file:5ec0d2c3043ae64cb72698b0f6fe7387884f4195df962466215ce534d2208327 in / 
# Thu, 10 Sep 2020 00:08:06 GMT
CMD ["bash"]
# Thu, 10 Sep 2020 18:18:03 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Thu, 10 Sep 2020 18:18:46 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Thu, 10 Sep 2020 18:18:57 GMT
ENV SPIPED_VERSION=1.6.1
# Thu, 10 Sep 2020 18:19:05 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Thu, 10 Sep 2020 18:19:12 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 10 Sep 2020 18:20:45 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 10 Sep 2020 18:20:53 GMT
VOLUME [/spiped]
# Thu, 10 Sep 2020 18:21:00 GMT
WORKDIR /spiped
# Thu, 10 Sep 2020 18:21:22 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 10 Sep 2020 18:21:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 10 Sep 2020 18:21:39 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:a7c65856610cb24c46ede2ffe313cbf933c44fa20ba213835af953646f3eb1ed`  
		Last Modified: Thu, 10 Sep 2020 00:17:52 GMT  
		Size: 22.7 MB (22699896 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66fee6c78263ccec9135fc7f2bb28a2de529aff4c5361d3456feea724e427e57`  
		Last Modified: Thu, 10 Sep 2020 18:22:12 GMT  
		Size: 1.7 KB (1732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9656ed70c1e53601a8def851ed70df83a99d6c30a22359856e87915f5dcca43`  
		Last Modified: Thu, 10 Sep 2020 18:22:13 GMT  
		Size: 1.8 MB (1759465 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:befeecd1667ed26f74f6f319f30d191b330e92cf43857823c0b0bafc309526cf`  
		Last Modified: Thu, 10 Sep 2020 18:22:14 GMT  
		Size: 5.3 MB (5285549 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d515d1ec84d005b136fb534dd6cf14b0eeb4096b1b9a0f7c00c9465e018d17a2`  
		Last Modified: Thu, 10 Sep 2020 18:22:12 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f645726760b82f17cd16dd4f97f80c9ad3e26f7218cc2a28619876a0f1314f07`  
		Last Modified: Thu, 10 Sep 2020 18:22:12 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:d0f7a1e94e3574be6205294542315b7366e335a75ae989478f816e828ec28d0d
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.8 MB (33764774 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ba15f48b73d0c01fc8a6207642b4c10acff03aec2ede7b91cd77b8f007eecaaa`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 09 Sep 2020 23:50:54 GMT
ADD file:d870fb0484ea283840d9cc923c9c3fe36d1bb6b3b5ecfefcce06aa26a22c9414 in / 
# Wed, 09 Sep 2020 23:50:57 GMT
CMD ["bash"]
# Thu, 10 Sep 2020 17:46:24 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Thu, 10 Sep 2020 17:46:32 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Thu, 10 Sep 2020 17:46:32 GMT
ENV SPIPED_VERSION=1.6.1
# Thu, 10 Sep 2020 17:46:33 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Thu, 10 Sep 2020 17:46:34 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 10 Sep 2020 17:47:24 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 10 Sep 2020 17:47:25 GMT
VOLUME [/spiped]
# Thu, 10 Sep 2020 17:47:26 GMT
WORKDIR /spiped
# Thu, 10 Sep 2020 17:47:27 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 10 Sep 2020 17:47:28 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 10 Sep 2020 17:47:29 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:a6d76de28f58f3470aff71c934c0fec4e5d0fad788f8b8bcc50601266fc1b34d`  
		Last Modified: Wed, 09 Sep 2020 23:59:09 GMT  
		Size: 25.8 MB (25849325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee1fca8e59138929238924b9500631bea3d7145eb26c2ff5dd838bf0300f2631`  
		Last Modified: Thu, 10 Sep 2020 17:47:53 GMT  
		Size: 1.7 KB (1740 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec65dadd59f387437df5aa1e90e26e6b3c6c7d248e936ddf4ccc9a81cd6facbe`  
		Last Modified: Thu, 10 Sep 2020 17:47:54 GMT  
		Size: 2.0 MB (2007909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd25c3b658895234d7cee37ea8f9d2a2f42664c47e1626093ecc4391ce56b989`  
		Last Modified: Thu, 10 Sep 2020 17:47:56 GMT  
		Size: 5.9 MB (5905328 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce8bb116f4707feafc36880d984f20d59a9ebbbdfcc1f339bb5113e0484b6969`  
		Last Modified: Thu, 10 Sep 2020 17:47:53 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ca039bdab3845640ef458839a0c5540b8e1c885bc2a90aed342b41623b64c7f`  
		Last Modified: Thu, 10 Sep 2020 17:47:53 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; 386

```console
$ docker pull spiped@sha256:7705a0fc3f3476409ebb0bc24d6d37d7fba3e5592d82ee6d2839e364a950456e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.5 MB (41517856 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:989705c9829172d17a6ede941662c041e3cf4cac305a6d4b388b20e91453b1b3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 09 Sep 2020 23:40:19 GMT
ADD file:08dc20c9cd727ebf02cac6e4b287c3009274682174aee9222494491cd6c671b8 in / 
# Wed, 09 Sep 2020 23:40:19 GMT
CMD ["bash"]
# Thu, 10 Sep 2020 00:16:37 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Thu, 10 Sep 2020 00:16:42 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Thu, 10 Sep 2020 00:16:42 GMT
ENV SPIPED_VERSION=1.6.1
# Thu, 10 Sep 2020 00:16:42 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Thu, 10 Sep 2020 00:16:42 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 10 Sep 2020 00:17:11 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 10 Sep 2020 00:17:11 GMT
VOLUME [/spiped]
# Thu, 10 Sep 2020 00:17:11 GMT
WORKDIR /spiped
# Thu, 10 Sep 2020 00:17:12 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 10 Sep 2020 00:17:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 10 Sep 2020 00:17:12 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:31e6582dbd9f9a84903d46339df0c393a63d2cbfb001b06b3204653cceafcc61`  
		Last Modified: Wed, 09 Sep 2020 23:46:30 GMT  
		Size: 27.8 MB (27750334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6860dd30325c96ffc8b96efe07adbb91c1bf07d1fbe88c2cde7cecd89da76d72`  
		Last Modified: Thu, 10 Sep 2020 00:17:26 GMT  
		Size: 1.7 KB (1731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a4331fe8000d00915ae0827ce99d7946202943c5616440cd4fe768d9d7ed71a`  
		Last Modified: Thu, 10 Sep 2020 00:17:27 GMT  
		Size: 2.1 MB (2132352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82c89212a59a8a3b09219d62baf7cfc20311e828bbf52b010ae9db5bc78c5b83`  
		Last Modified: Thu, 10 Sep 2020 00:17:29 GMT  
		Size: 11.6 MB (11633000 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54072dfa562a77a02b96e37ade7b47dfdf8a9a27d4eee6db49dc154a2c89cf0a`  
		Last Modified: Thu, 10 Sep 2020 00:17:27 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bfe5b51ab58e39aa04cbe7d1f927049252d4d7b476925effe2c5e213e905108`  
		Last Modified: Thu, 10 Sep 2020 00:17:26 GMT  
		Size: 344.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; mips64le

```console
$ docker pull spiped@sha256:016da36b9f7998b09d92b6cc8852d341e82ef59a357e95663cf2a912e99bf1c1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.9 MB (33893243 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:195c77f25ce68e53cef2621cd2de83604d84f91dc5bdcebf623cfc31ce8aa130`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 04 Aug 2020 06:42:23 GMT
ADD file:4164c71b841ba2c1f213c9fdc073ec3d4c7d79dadfcd9d771768750a3085d616 in / 
# Tue, 04 Aug 2020 06:42:24 GMT
CMD ["bash"]
# Tue, 04 Aug 2020 11:18:11 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 04 Aug 2020 11:18:23 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 04 Aug 2020 11:18:24 GMT
ENV SPIPED_VERSION=1.6.1
# Tue, 04 Aug 2020 11:18:24 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Tue, 04 Aug 2020 11:18:24 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Tue, 04 Aug 2020 11:19:31 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 04 Aug 2020 11:19:31 GMT
VOLUME [/spiped]
# Tue, 04 Aug 2020 11:19:32 GMT
WORKDIR /spiped
# Tue, 04 Aug 2020 11:19:32 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 04 Aug 2020 11:19:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 04 Aug 2020 11:19:33 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:1333f76e75c0136aa2eb56b14271ef57d1f975f40fe2a56536d99b7c86c3aa29`  
		Last Modified: Tue, 04 Aug 2020 06:48:41 GMT  
		Size: 25.8 MB (25762724 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1d54e34357c9f5fa48267296e6c6c1f76e35953b78ff71274dbf93d620fe713`  
		Last Modified: Tue, 04 Aug 2020 11:19:56 GMT  
		Size: 1.7 KB (1737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:808939bfa0b439c22bc52e424703f683009d54bc7b0e929bb95642a17e4cf346`  
		Last Modified: Tue, 04 Aug 2020 11:19:57 GMT  
		Size: 1.7 MB (1712064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d1430e0259ffd64f678312f8e44b2331f9b36c5dfc010756f03d0b4b1d5278b`  
		Last Modified: Tue, 04 Aug 2020 11:20:02 GMT  
		Size: 6.4 MB (6416279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6160144f3a0adf67512994233d3b27e3cf11991c2929b9ceb5fcbccce56af823`  
		Last Modified: Tue, 04 Aug 2020 11:19:56 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91a1586309f94ae81d1d5501572c464e6cf0b95721f6d0e54fad359886abb713`  
		Last Modified: Tue, 04 Aug 2020 11:19:56 GMT  
		Size: 344.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; ppc64le

```console
$ docker pull spiped@sha256:1a26f6d748b9c6cd0cd3c33bd6326198eac44ee6695d90e32fa92c33d0efab15
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.5 MB (39488256 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dffa18892130ac57caaa0c35c5e223f1f80929f3bca5753dfbbebd98c9d1a1ad`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 04 Aug 2020 04:45:34 GMT
ADD file:3bab6d2b62fe6a548ee28480d9eebf3251e942c4bb66362b87396b73af7aa586 in / 
# Tue, 04 Aug 2020 04:45:40 GMT
CMD ["bash"]
# Tue, 04 Aug 2020 12:44:13 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 04 Aug 2020 12:44:32 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 04 Aug 2020 12:44:36 GMT
ENV SPIPED_VERSION=1.6.1
# Tue, 04 Aug 2020 12:44:39 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Tue, 04 Aug 2020 12:44:44 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Tue, 04 Aug 2020 12:48:01 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 04 Aug 2020 12:48:05 GMT
VOLUME [/spiped]
# Tue, 04 Aug 2020 12:48:08 GMT
WORKDIR /spiped
# Tue, 04 Aug 2020 12:48:11 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 04 Aug 2020 12:48:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 04 Aug 2020 12:48:16 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:0827434caf9c0b71f95b3bcbe29d60f4f887199db59b3994d9315c478def41c3`  
		Last Modified: Tue, 04 Aug 2020 04:53:24 GMT  
		Size: 30.5 MB (30517844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11ec976cf945c4c5a0725ce160b23b8fc7453ab53f7645cb507f81cc8f97ba1f`  
		Last Modified: Tue, 04 Aug 2020 12:48:51 GMT  
		Size: 1.7 KB (1738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42b3868607138d28e33ab153c8f68521f00f2c00ee48d5542c62fef3ee508bcf`  
		Last Modified: Tue, 04 Aug 2020 12:48:52 GMT  
		Size: 2.2 MB (2224970 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bc4d03de8274dc06c34b37b24e819fe01a0d313e538a7a809f519e3a63d9418`  
		Last Modified: Tue, 04 Aug 2020 12:48:53 GMT  
		Size: 6.7 MB (6743232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ff8e76a3ee77f253306f6c4c94eaf5df2e55c449d2a812c3bb843851031bc47`  
		Last Modified: Tue, 04 Aug 2020 12:48:51 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b58b79d7f675a5211c5c171567c5ff5762c0755bef406ed884efd50c9df4a3d1`  
		Last Modified: Tue, 04 Aug 2020 12:48:51 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; s390x

```console
$ docker pull spiped@sha256:3d77e561a1da58512f8944775139df6b4c0837d6f38a3f57a18522f0acc1824e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.5 MB (33474968 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d7e3a3c55ec7ac4f5ce17bb3f14dc3268a611714368d8f3c15bdf715638359f7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 09 Sep 2020 23:42:35 GMT
ADD file:65e860d387f18169ea1783465571eaf0946b51c52e560a06759bbc680752f810 in / 
# Wed, 09 Sep 2020 23:42:37 GMT
CMD ["bash"]
# Thu, 10 Sep 2020 01:42:43 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Thu, 10 Sep 2020 01:42:47 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Thu, 10 Sep 2020 01:42:47 GMT
ENV SPIPED_VERSION=1.6.1
# Thu, 10 Sep 2020 01:42:47 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Thu, 10 Sep 2020 01:42:47 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 10 Sep 2020 01:43:02 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 10 Sep 2020 01:43:02 GMT
VOLUME [/spiped]
# Thu, 10 Sep 2020 01:43:03 GMT
WORKDIR /spiped
# Thu, 10 Sep 2020 01:43:03 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 10 Sep 2020 01:43:03 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 10 Sep 2020 01:43:03 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:07e4a6dbced6eed74bdb331987f95c00aa5b46543570b7adc1575121e66102dd`  
		Last Modified: Wed, 09 Sep 2020 23:46:28 GMT  
		Size: 25.7 MB (25707597 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:814983a66e3ee433d454db4a5b4e1062cf563e9decb8c477bba4cd96bc413ef1`  
		Last Modified: Thu, 10 Sep 2020 01:43:19 GMT  
		Size: 1.7 KB (1742 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47e1d72214ff5a65c75ec20c8756f56e1739f0aa5c8124641f55b46448070adf`  
		Last Modified: Thu, 10 Sep 2020 01:43:19 GMT  
		Size: 1.8 MB (1821787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd27f6e5680762c3bf63ebc1825797061f461bd985220db2634dd60509dfcc7d`  
		Last Modified: Thu, 10 Sep 2020 01:43:20 GMT  
		Size: 5.9 MB (5943372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a566492192d8af2e7358649988f9e50908dbe4afa87c84c6fa890eb6235c6924`  
		Last Modified: Thu, 10 Sep 2020 01:43:19 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3efd28ff600e747098b28280c12af1bfd52c57a500440f4376ba567e79defc6c`  
		Last Modified: Thu, 10 Sep 2020 01:43:19 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
