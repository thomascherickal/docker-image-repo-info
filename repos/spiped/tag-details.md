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
$ docker pull spiped@sha256:ff3003949cdd1ced212cbb6bea1509e64d4fc152923eda3c284abfb51342637f
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
$ docker pull spiped@sha256:a696ea93d50ac968bc64ce5ab01eaf4ff13ae39fa9f099b9cd19a8e7a9d07aee
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.3 MB (37320955 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:683078eccb0851809c92a9dfdb1dcdd47c187bd8a7a5cc960a8fa55b1ece7e86`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 12 Oct 2021 01:20:42 GMT
ADD file:16dc2c6d1932194edec28d730b004fd6deca3d0f0e1a07bc5b8b6e8a1662f7af in / 
# Tue, 12 Oct 2021 01:20:42 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 16:21:25 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 12 Oct 2021 16:21:29 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 16:21:29 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Tue, 12 Oct 2021 16:21:56 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 12 Oct 2021 16:21:56 GMT
VOLUME [/spiped]
# Tue, 12 Oct 2021 16:21:56 GMT
WORKDIR /spiped
# Tue, 12 Oct 2021 16:21:57 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 12 Oct 2021 16:21:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 12 Oct 2021 16:21:57 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:7d63c13d9b9b6ec5f05a2b07daadacaa9c610d01102a662ae9b1d082105f1ffa`  
		Last Modified: Tue, 12 Oct 2021 01:26:05 GMT  
		Size: 31.4 MB (31357311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c825e91f209a1656f91feea4a2861373b55da8c1c3eb72e742c7f31c3d367918`  
		Last Modified: Tue, 12 Oct 2021 16:22:19 GMT  
		Size: 1.7 KB (1735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bba3f6cb28bad6f7f95e8be3b815465b3d5585c01a7cde8e6c561a81fd08d8e7`  
		Last Modified: Tue, 12 Oct 2021 16:22:19 GMT  
		Size: 1.1 KB (1051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbac5321939b951af500d72dc338b30ccdc61d354b3a466ce698a006ca3f4999`  
		Last Modified: Tue, 12 Oct 2021 16:22:20 GMT  
		Size: 6.0 MB (5960389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e58545b0e832a28e4b2fe9fe327f35158f38ccc204ce2c8fe1597803e860c0c2`  
		Last Modified: Tue, 12 Oct 2021 16:22:19 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c1557262dbc7e84098fd29719562170e4c257f980350cf3e68318ecd07a8956`  
		Last Modified: Tue, 12 Oct 2021 16:22:19 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; arm variant v5

```console
$ docker pull spiped@sha256:470773bf2dac565adf268ce74a10c0ca68c421d0de4192c4f6f29f15e8663e54
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.9 MB (33928107 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bee42cb8fa181c28acac6a722b80b4ea34b101698e1d8886a77f8323f3dbc1d2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 12 Oct 2021 00:50:30 GMT
ADD file:fb1afabdc1f93b4866b4c4d696f272b4888519cb5bf35eb7ed1a4c021d1a04c8 in / 
# Tue, 12 Oct 2021 00:50:30 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 11:33:43 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 12 Oct 2021 11:33:53 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 11:33:53 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Tue, 12 Oct 2021 11:34:54 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 12 Oct 2021 11:34:55 GMT
VOLUME [/spiped]
# Tue, 12 Oct 2021 11:34:55 GMT
WORKDIR /spiped
# Tue, 12 Oct 2021 11:34:56 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 12 Oct 2021 11:34:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 12 Oct 2021 11:34:57 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:5c9bab66abc5c53391435f6fd66e0ff3571295d568f45ac7d2dc480bcbfd56e8`  
		Last Modified: Tue, 12 Oct 2021 01:06:07 GMT  
		Size: 28.9 MB (28899715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b29fa5bfe046f908c4024b12760d6a235703129cf889a6b12fe9cb3c909e50ea`  
		Last Modified: Tue, 12 Oct 2021 11:35:35 GMT  
		Size: 1.7 KB (1725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f15e6ebdfdcc8907dc36ff08f672c463d0fbb6c59b0bb232ff1a229f64e4ea34`  
		Last Modified: Tue, 12 Oct 2021 11:35:35 GMT  
		Size: 1.1 KB (1053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0030f062ce13c3eb3f6f0020460e01e4beebed73ca735660e5fe74df98d62119`  
		Last Modified: Tue, 12 Oct 2021 11:35:40 GMT  
		Size: 5.0 MB (5025142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9edc074a3eb9dffdb9440831266c18299dcccc42834d767fc489b92ca7f2a48`  
		Last Modified: Tue, 12 Oct 2021 11:35:35 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ef7dd4a1c957efda249f4568cd568c8671c526848a4b9f57ffc9783bf81cef3`  
		Last Modified: Tue, 12 Oct 2021 11:35:35 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; arm variant v7

```console
$ docker pull spiped@sha256:958d2e76bb92a4709c36123b6553d179419227b06b733ec19cf1a4899da20853
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.3 MB (31309843 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9c0880cb9c6c234ff2fe6a3c163710a28845c22e1207ecd0b31cd8887cb77d26`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 12 Oct 2021 01:28:36 GMT
ADD file:89eac94007ac04f9168737686fa0a6c737f2c28fc9e5918d4d512924fe1973be in / 
# Tue, 12 Oct 2021 01:28:37 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 03:43:34 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 12 Oct 2021 03:43:41 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 03:43:42 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Tue, 12 Oct 2021 03:44:37 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 12 Oct 2021 03:44:37 GMT
VOLUME [/spiped]
# Tue, 12 Oct 2021 03:44:38 GMT
WORKDIR /spiped
# Tue, 12 Oct 2021 03:44:39 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 12 Oct 2021 03:44:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 12 Oct 2021 03:44:40 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:4e5300249f84466df4dc73ea0ce09938ca00c1718bb12619c4f26bd936162331`  
		Last Modified: Tue, 12 Oct 2021 01:44:28 GMT  
		Size: 26.6 MB (26561058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6ecc7e48d063e5bf0a086847e03c73699a183e8a9129e1b8ee3cab1482dde2d`  
		Last Modified: Tue, 12 Oct 2021 03:45:39 GMT  
		Size: 1.7 KB (1735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:584009012f86b47c7e4e6d1fd99c2d00976e77d0c5c66f0179ed3c7ea7c54725`  
		Last Modified: Tue, 12 Oct 2021 03:45:39 GMT  
		Size: 1.1 KB (1051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aae397080ab7f297afe0c2760bc744f5c6ab5ff8f88b8e0830bc8ae8d97b565f`  
		Last Modified: Tue, 12 Oct 2021 03:45:44 GMT  
		Size: 4.7 MB (4745527 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c697bb38b9e3862762d00df70d8a431fd891e25b33a03308c9e1cf59a02c712`  
		Last Modified: Tue, 12 Oct 2021 03:45:39 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0c305948d80dae9d7e0b495eba60d890696dba8079d33af0619bb473c03c079`  
		Last Modified: Tue, 12 Oct 2021 03:45:39 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:ddea46bf094678e8d8a63419789e3ff6b8df43ce2463fe054b2c6873958a7ed6
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.3 MB (35323019 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c62eeb5b4d9a5249368c594ef830ee32d99656d7accef9dec9afa2117c116bd4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 17 Nov 2021 02:40:15 GMT
ADD file:4203242b2b09a65239092c4780b59181da7b861b3c0be40810b3588aa200f72c in / 
# Wed, 17 Nov 2021 02:40:16 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 10:13:37 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 17 Nov 2021 10:13:41 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 10:13:42 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Wed, 17 Nov 2021 10:14:05 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 17 Nov 2021 10:14:06 GMT
VOLUME [/spiped]
# Wed, 17 Nov 2021 10:14:07 GMT
WORKDIR /spiped
# Wed, 17 Nov 2021 10:14:09 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 17 Nov 2021 10:14:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 17 Nov 2021 10:14:10 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:eb9a2845ed124d072b117aba4f0508e00c1ecd0d147dc324d14b00d24092046c`  
		Last Modified: Wed, 17 Nov 2021 02:47:17 GMT  
		Size: 30.1 MB (30056521 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b433167df10525b1b963a099589e5afac7d2b0fb31ccdd12d08134a7f543066`  
		Last Modified: Wed, 17 Nov 2021 10:14:43 GMT  
		Size: 1.6 KB (1616 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e176f2d91c6ad8f6d7ec824e8ecb1f7fc106c426f4717846a45154a39dcd214`  
		Last Modified: Wed, 17 Nov 2021 10:14:43 GMT  
		Size: 922.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99b725a99707e19e9152425097352ac163c18e25fdfdc11408f1b24926d88e21`  
		Last Modified: Wed, 17 Nov 2021 10:14:45 GMT  
		Size: 5.3 MB (5263526 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c46663b1e9b74612d1f081a80b43411d46c40cca2ca919d85b3e5651330d0e9`  
		Last Modified: Wed, 17 Nov 2021 10:14:44 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa44bd73d20d05c58e00bfff946eb6cab9b43fab597595cb74d0dcf53ab375c5`  
		Last Modified: Wed, 17 Nov 2021 10:14:43 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; 386

```console
$ docker pull spiped@sha256:1a250bf744242fee28c1506fa0085cd2e9f9467a0112a9497e7b6c5c7eda827b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.3 MB (40268237 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7f13080f172f1d6f15013062e14fd652880f18a736ef807504f9efeba0451496`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 17 Nov 2021 02:39:53 GMT
ADD file:ff018048717c0f5aa1730480d0bfea1c2bf94d6e2dae2d7cef46d05ffb0d93e1 in / 
# Wed, 17 Nov 2021 02:39:53 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 19:21:10 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 17 Nov 2021 19:21:18 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 19:21:18 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Wed, 17 Nov 2021 19:22:03 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 17 Nov 2021 19:22:04 GMT
VOLUME [/spiped]
# Wed, 17 Nov 2021 19:22:04 GMT
WORKDIR /spiped
# Wed, 17 Nov 2021 19:22:05 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 17 Nov 2021 19:22:05 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 17 Nov 2021 19:22:05 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:0bae0e1d4cb1d56ffeb9d05de7a097d3157267eef07b6d8131344d99bd97c431`  
		Last Modified: Wed, 17 Nov 2021 02:47:49 GMT  
		Size: 32.4 MB (32380683 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f71fd8d5c5711c96e84b1ce61114fe587d1427bf8042ef8ebf82882aa6b272a6`  
		Last Modified: Wed, 17 Nov 2021 19:23:02 GMT  
		Size: 1.7 KB (1734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c9611950dec2f42e40638d36289e1eef041b09d67ce4432d06ab76df0b5ace2`  
		Last Modified: Wed, 17 Nov 2021 19:23:03 GMT  
		Size: 1.1 KB (1055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:518b93d7db88cd296006861d6bca16590713db92325202daf9f4b7ebea46c840`  
		Last Modified: Wed, 17 Nov 2021 19:23:06 GMT  
		Size: 7.9 MB (7884295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd63e5a1b92185ac3ee583071d18f2c066670b2d466f8d18b888ba29e63ed182`  
		Last Modified: Wed, 17 Nov 2021 19:23:02 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc11c755ca357e2015909562f541b58552c232be20964fbba165a30990d5ebe1`  
		Last Modified: Wed, 17 Nov 2021 19:23:02 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; mips64le

```console
$ docker pull spiped@sha256:450f58414b6d98b4327999d964acbdfd088a4876c793662af1e6612a3c22e4f4
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.3 MB (35339707 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7fce297eacc4add3406390459583f251fc83bd3ae97b51328694b22fa7fe7772`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 17 Nov 2021 02:10:13 GMT
ADD file:10bc783d286d0a800f59d5009e87ecb4651659c82cae1325132756c7c8b1dec0 in / 
# Wed, 17 Nov 2021 02:10:13 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 08:27:05 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 17 Nov 2021 08:27:17 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 08:27:17 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Wed, 17 Nov 2021 08:28:30 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 17 Nov 2021 08:28:31 GMT
VOLUME [/spiped]
# Wed, 17 Nov 2021 08:28:31 GMT
WORKDIR /spiped
# Wed, 17 Nov 2021 08:28:32 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 17 Nov 2021 08:28:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 17 Nov 2021 08:28:32 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:08bca22fbffb4e58224e9e4f6a56f1ca5099c002b1aeb6181df63af308a3da58`  
		Last Modified: Wed, 17 Nov 2021 02:19:09 GMT  
		Size: 29.6 MB (29630388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac0800f7325d28791d9fbe530a7eef215f778350ecaf8ea10233b5921e861a07`  
		Last Modified: Wed, 17 Nov 2021 08:28:54 GMT  
		Size: 1.7 KB (1735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:566002f949cf54396dcd4f4732f10bb92a05a233c5e1ab60f79bff5a0fd57f63`  
		Last Modified: Wed, 17 Nov 2021 08:28:54 GMT  
		Size: 1.0 KB (1026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0339485e14c68084894399e67ee3e846ae570dd31af17ff0c7b996e2240cc8af`  
		Last Modified: Wed, 17 Nov 2021 08:29:00 GMT  
		Size: 5.7 MB (5706120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41d70628022717b6810fe3b62132cabe088e4c72a562033f04f332cd196b72c9`  
		Last Modified: Wed, 17 Nov 2021 08:28:54 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd86da81696b1bd0c2d983b7561e6bfa1c71b05b50c6e31685145ffc68ac067d`  
		Last Modified: Wed, 17 Nov 2021 08:28:54 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; ppc64le

```console
$ docker pull spiped@sha256:44b13757ab959642c428cd66c8a503318b7916932e88ee0f686aff3c40b6f88e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.3 MB (41263678 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aadb76166ced7d8733fac685c49d5b3e6c4e0ca8713e0c26fa2829ab87bb9172`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 12 Oct 2021 01:25:45 GMT
ADD file:d8794fadf16c9948c3574ba28740d08393eca57766340333ad91f9c2a33eb719 in / 
# Tue, 12 Oct 2021 01:25:53 GMT
CMD ["bash"]
# Wed, 13 Oct 2021 08:03:47 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 13 Oct 2021 08:03:59 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 13 Oct 2021 08:04:02 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Wed, 13 Oct 2021 08:07:07 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 13 Oct 2021 08:07:16 GMT
VOLUME [/spiped]
# Wed, 13 Oct 2021 08:07:24 GMT
WORKDIR /spiped
# Wed, 13 Oct 2021 08:07:26 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 13 Oct 2021 08:07:28 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 13 Oct 2021 08:07:32 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:6c28c1405c677dd809094d06190225b38cee3d24f18da38d287ef5bcc67884d6`  
		Last Modified: Tue, 12 Oct 2021 01:37:00 GMT  
		Size: 35.3 MB (35258729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44c02b2acecad78932397dca6224b551528ccaf70fed1c60da8884b1ee077de8`  
		Last Modified: Wed, 13 Oct 2021 08:08:15 GMT  
		Size: 1.7 KB (1745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1e5dcbe4d07e13aa9f6162d201034eb2b26b9f69987315148425a39102ba3df`  
		Last Modified: Wed, 13 Oct 2021 08:08:15 GMT  
		Size: 1.1 KB (1056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d805dc3af7457dd0105eca804e08afa7eed7d23d36613d054713cef0cd7f301a`  
		Last Modified: Wed, 13 Oct 2021 08:08:16 GMT  
		Size: 6.0 MB (6001677 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c36c3789c72419dd7c04f766b8ef090133dd4afbffd43366f439be9bdcb7d88`  
		Last Modified: Wed, 13 Oct 2021 08:08:15 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1414313671940f5f943d32775bed04903cb0d2af90ece5729859bf3a6284b292`  
		Last Modified: Wed, 13 Oct 2021 08:08:15 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; s390x

```console
$ docker pull spiped@sha256:bbdf535a02054a6706cd99a1fafde9724dd2417cfe9cbe59bb51a6a86fcdedfc
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.8 MB (34838172 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b0334f4bf3851c59d807ecc784fbf754bcc015f78bc339af17c7452c71ee0450`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 17 Nov 2021 02:42:27 GMT
ADD file:42f73dac307a6a5232e3100f3d3b36e8125f73a4ca504b106e60e2b66d242b2f in / 
# Wed, 17 Nov 2021 02:42:28 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 09:51:42 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 17 Nov 2021 09:51:44 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 09:51:44 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Wed, 17 Nov 2021 09:51:59 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 17 Nov 2021 09:52:00 GMT
VOLUME [/spiped]
# Wed, 17 Nov 2021 09:52:00 GMT
WORKDIR /spiped
# Wed, 17 Nov 2021 09:52:00 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 17 Nov 2021 09:52:00 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 17 Nov 2021 09:52:00 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:8d71e885edf612b507bbdcc48a970548d436b8709eeedfc2c98f6843a214b5e2`  
		Last Modified: Wed, 17 Nov 2021 02:48:25 GMT  
		Size: 29.7 MB (29650960 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b4e3a0c91da007baa099ab7d28b8282d97a1d427f8c3bfb6fa661fea558f431`  
		Last Modified: Wed, 17 Nov 2021 09:52:31 GMT  
		Size: 1.7 KB (1737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ea434878158c3e70134c052033e411e6633b141bdafd5fc45465e919790f3c9`  
		Last Modified: Wed, 17 Nov 2021 09:52:31 GMT  
		Size: 1.1 KB (1051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1680a353eb5f9bbeb5fa65bb02c66d997e5e0211cdf62ea04996f568f3a34af2`  
		Last Modified: Wed, 17 Nov 2021 09:52:32 GMT  
		Size: 5.2 MB (5183957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92981a4dda6befd75588ea56b9eb907cd8ab9daae831a0fb3b18c2dc37e4d7fe`  
		Last Modified: Wed, 17 Nov 2021 09:52:31 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76ef547fabd115d65e325e62fac7260ef1ce418b3c8ac5e5b8ca8b4efac73ed9`  
		Last Modified: Wed, 17 Nov 2021 09:52:31 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:1-alpine`

```console
$ docker pull spiped@sha256:1447fc83864d467400e6d1b2a87532955de7649123545804894c2a8c86d6a34a
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
$ docker pull spiped@sha256:5759c6e68d7e93789c7fc574722f42f3d3bafcaab2c4a8aeeeac5bb4772012a7
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (3045597 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1cc3e3a8422cee08ac18b30d97939a3a6bd28e94a61d0caaaa96ff86dd8f425c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 12 Nov 2021 17:19:44 GMT
ADD file:762c899ec0505d1a32930ee804c5b008825f41611161be104076cba33b7e5b2b in / 
# Fri, 12 Nov 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Sat, 13 Nov 2021 07:30:36 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Sat, 13 Nov 2021 07:30:37 GMT
RUN apk add --no-cache libssl1.1
# Sat, 13 Nov 2021 07:30:37 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Sat, 13 Nov 2021 07:31:02 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Sat, 13 Nov 2021 07:31:02 GMT
VOLUME [/spiped]
# Sat, 13 Nov 2021 07:31:03 GMT
WORKDIR /spiped
# Sat, 13 Nov 2021 07:31:03 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 13 Nov 2021 07:31:03 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 13 Nov 2021 07:31:04 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:97518928ae5f3d52d4164b314a7e73654eb686ecd8aafa0b79acd980773a740d`  
		Last Modified: Fri, 12 Nov 2021 17:20:39 GMT  
		Size: 2.8 MB (2822981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d272f2608cb29aaf56aaa58c4e8245793833d52257971c0a4a90c1445945548`  
		Last Modified: Sat, 13 Nov 2021 07:31:25 GMT  
		Size: 1.3 KB (1267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:588bebf547583661fb31be182d777849262971941c241f7b072c041f54e3c4ff`  
		Last Modified: Sat, 13 Nov 2021 07:31:25 GMT  
		Size: 7.8 KB (7767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:687f41a1ab4447065d651caf78075639eb1027290f0756c4d489a10c43a745af`  
		Last Modified: Sat, 13 Nov 2021 07:31:25 GMT  
		Size: 213.1 KB (213113 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0d7a22ad75e07e938780270586c7d97ddd070bf6b70ee31e6fbe14b6c79cda6`  
		Last Modified: Sat, 13 Nov 2021 07:31:25 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b484100590c35b883633e127830518528f9cc47bce7f4b864394b4bd85acb54`  
		Last Modified: Sat, 13 Nov 2021 07:31:25 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; arm variant v6

```console
$ docker pull spiped@sha256:e54c9ae8aa1651b3704440b6b74cbdd5ac80086e8fa25252df5ffbe44591eade
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 MB (2847905 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c6b358d015e8acc6b6eac3e79c5fc5302785d8bce806dc4640e51e684fc73495`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 12 Nov 2021 16:49:42 GMT
ADD file:6daf1fe862c00673bf9cf4d7e20b0bf253a56e7fb8ed5e730a4466ab9186e18a in / 
# Fri, 12 Nov 2021 16:49:44 GMT
CMD ["/bin/sh"]
# Sat, 13 Nov 2021 06:56:43 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Sat, 13 Nov 2021 06:56:48 GMT
RUN apk add --no-cache libssl1.1
# Sat, 13 Nov 2021 06:56:49 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Sat, 13 Nov 2021 06:57:26 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Sat, 13 Nov 2021 06:57:27 GMT
VOLUME [/spiped]
# Sat, 13 Nov 2021 06:57:27 GMT
WORKDIR /spiped
# Sat, 13 Nov 2021 06:57:28 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 13 Nov 2021 06:57:28 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 13 Nov 2021 06:57:29 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:56afcfda5d78cc243287acbaad250c5e8c0f47aae620dd7c51985b0d3c9b2728`  
		Last Modified: Fri, 12 Nov 2021 16:51:32 GMT  
		Size: 2.6 MB (2635392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbee8633a3e2da897713dd8453113fc924e1ad102e43bc673e5aa4e72a3c5ff6`  
		Last Modified: Sat, 13 Nov 2021 06:58:02 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b421d84dfbecebc99f29f801626a8781142421b8affb55b6dac49de522afdd86`  
		Last Modified: Sat, 13 Nov 2021 06:58:02 GMT  
		Size: 7.8 KB (7780 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c67a331696441ca0da524281edcd53ee4b8d52a24b4fdaab4f5b2e3833ab74a`  
		Last Modified: Sat, 13 Nov 2021 06:58:02 GMT  
		Size: 203.0 KB (202993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52ab514374a45d9fd16341748dc013e94fd9ddf0b15c2f3666bea84a2c2db7dd`  
		Last Modified: Sat, 13 Nov 2021 06:58:02 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:526ec51047ed2d4267785d4387f46cebef6e388cb755c73b640a73e44db871b6`  
		Last Modified: Sat, 13 Nov 2021 06:58:02 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; arm variant v7

```console
$ docker pull spiped@sha256:8b3e418343ca28cc6af7c79a9c92f500d16214863644d56f2e6a6c6a66f457d8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 MB (2644452 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3edd8179550b7c42a3827056d11ba4da9c0f384e1b5ac66177b911a1a9f75acc`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 12 Nov 2021 16:57:35 GMT
ADD file:03e0720458c3475758bf4394afa56f2165198eb91e6e9581f7768e433744dd9b in / 
# Fri, 12 Nov 2021 16:57:36 GMT
CMD ["/bin/sh"]
# Fri, 12 Nov 2021 19:09:19 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 12 Nov 2021 19:09:21 GMT
RUN apk add --no-cache libssl1.1
# Fri, 12 Nov 2021 19:09:22 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 12 Nov 2021 19:09:55 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 12 Nov 2021 19:09:55 GMT
VOLUME [/spiped]
# Fri, 12 Nov 2021 19:09:56 GMT
WORKDIR /spiped
# Fri, 12 Nov 2021 19:09:56 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 12 Nov 2021 19:09:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 12 Nov 2021 19:09:57 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:764d2e53e1a607f2d8261522185d5b9021ade3ec1a595664ee90308c00176899`  
		Last Modified: Fri, 12 Nov 2021 16:59:33 GMT  
		Size: 2.4 MB (2438618 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2462c3e2387f9df1b6daae812a3674ccd49db10b9b7251881ea1a034a39185b`  
		Last Modified: Fri, 12 Nov 2021 19:10:52 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9e4892bdd8b9be427ec2794ea13c95ec6cca78353d3c032d0fd2ba5acf9bae3`  
		Last Modified: Fri, 12 Nov 2021 19:10:52 GMT  
		Size: 7.8 KB (7791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:624ff05273c8a204e1361bc188430fe618799c3ec5471284aa49a1f9bd365020`  
		Last Modified: Fri, 12 Nov 2021 19:10:52 GMT  
		Size: 196.3 KB (196302 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f127d56c30dd5e8a58309b3d42c9c4f974256b6b1f1f9ff32b0ff78d8c372b3b`  
		Last Modified: Fri, 12 Nov 2021 19:10:52 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aab7e0d291c6010513c0721d4abf0cd1f407a631c23f515859004dddf983c5f5`  
		Last Modified: Fri, 12 Nov 2021 19:10:52 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:cbaa0533059fb17c768fe05790c3675b5b5cecf35f0b461e5347d763b1322af8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 MB (2932006 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a49787cc7861893f9d6020342db1639e60d7af6850ca4866d08840d8438a2b0c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 12 Nov 2021 16:39:58 GMT
ADD file:400c0466b29ccad54e0f6c0acef22542992828678c96693ef1f9f4d0551935d8 in / 
# Fri, 12 Nov 2021 16:39:58 GMT
CMD ["/bin/sh"]
# Fri, 12 Nov 2021 18:19:31 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 12 Nov 2021 18:19:33 GMT
RUN apk add --no-cache libssl1.1
# Fri, 12 Nov 2021 18:19:34 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 12 Nov 2021 18:19:54 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 12 Nov 2021 18:19:55 GMT
VOLUME [/spiped]
# Fri, 12 Nov 2021 18:19:56 GMT
WORKDIR /spiped
# Fri, 12 Nov 2021 18:19:58 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 12 Nov 2021 18:19:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 12 Nov 2021 18:19:59 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:be307f383ecc62b27a29b599c3fc9d3129693a798e7fcce614f09174cfe2d354`  
		Last Modified: Fri, 12 Nov 2021 16:40:59 GMT  
		Size: 2.7 MB (2717700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffbcce6bf922e4817964b0a9575d547fbb39004874a87c290658dcbb8939209e`  
		Last Modified: Fri, 12 Nov 2021 18:20:41 GMT  
		Size: 1.2 KB (1239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b342172a90f6f6a837eeb8f0025e02facad5a97fdd12c0aeac68c2411928d16f`  
		Last Modified: Fri, 12 Nov 2021 18:20:41 GMT  
		Size: 7.8 KB (7751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd8a670bc36ab2f74e650d7cb573c4c3542673b9488e2659efbc0d6b9db67529`  
		Last Modified: Fri, 12 Nov 2021 18:20:41 GMT  
		Size: 204.9 KB (204879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:698de19c09a4c9763fb04c4946f3bffafe6556fcfe73a3d55bbb4255f65bd458`  
		Last Modified: Fri, 12 Nov 2021 18:20:41 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1d1aa9a890181cdc95e60ea01849306cb72c967e13716722baa68c7bca76fdb`  
		Last Modified: Fri, 12 Nov 2021 18:20:42 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; 386

```console
$ docker pull spiped@sha256:ed9db1b4a0c65f0ca88573ca4e82bafaedde5032f465971dba93432ddcf67f67
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.1 MB (3064332 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:04afce967f7cf45ad1faa0b6e1d955f2bad9d1aff37c3659db5e809170762140`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 12 Nov 2021 16:38:42 GMT
ADD file:403428c2903dd9dea10d069185873cb2c2c3149c553797807c69f22aa3d12fe3 in / 
# Fri, 12 Nov 2021 16:38:42 GMT
CMD ["/bin/sh"]
# Fri, 12 Nov 2021 20:40:39 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 12 Nov 2021 20:40:41 GMT
RUN apk add --no-cache libssl1.1
# Fri, 12 Nov 2021 20:40:41 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 12 Nov 2021 20:41:13 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 12 Nov 2021 20:41:14 GMT
VOLUME [/spiped]
# Fri, 12 Nov 2021 20:41:14 GMT
WORKDIR /spiped
# Fri, 12 Nov 2021 20:41:15 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 12 Nov 2021 20:41:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 12 Nov 2021 20:41:16 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:5420e0d28c84ecb16748cb90cc6acf8e2a81dab10cb1f674f3eee8533e53c62a`  
		Last Modified: Fri, 12 Nov 2021 16:39:36 GMT  
		Size: 2.8 MB (2830948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9abea20678ed9ffc78867f8fc9674162184169da3d7c198cd24ec6b7439e0c88`  
		Last Modified: Fri, 12 Nov 2021 20:41:51 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f04cc4ba71752a6b9075421e6b0b7f08625406fb105f85e23547c4eb23b25f3`  
		Last Modified: Fri, 12 Nov 2021 20:41:51 GMT  
		Size: 7.8 KB (7770 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae957cbfbd7f9f36494cb3954e91d1ead35e68d61bbddf48904c4b6133c4c878`  
		Last Modified: Fri, 12 Nov 2021 20:41:51 GMT  
		Size: 223.9 KB (223875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:911b8888c5d7d41e887ed34d5f9c93d1d3241ad814e69f4d7def6b5debc96ae8`  
		Last Modified: Fri, 12 Nov 2021 20:41:51 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74d46a3df042754e1b8e655e102bf789f899a1f3758442759be66fe90573dbd2`  
		Last Modified: Fri, 12 Nov 2021 20:41:52 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; ppc64le

```console
$ docker pull spiped@sha256:892b50ba6b7bed8e6253a2577dcb2c38d0e60b1ae71968d978a808094e610768
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (3048694 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f7522decac983b5c7f6951cee379a5207bdbe044c9371a89a784e025923deb04`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 12 Nov 2021 21:18:00 GMT
ADD file:4d45063079cb28a34f1e382fddb22f156ac99d5449aa05ed37cb653c1f7b80f2 in / 
# Fri, 12 Nov 2021 21:18:01 GMT
CMD ["/bin/sh"]
# Sat, 13 Nov 2021 15:29:42 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Sat, 13 Nov 2021 15:29:55 GMT
RUN apk add --no-cache libssl1.1
# Sat, 13 Nov 2021 15:29:58 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Sat, 13 Nov 2021 15:30:26 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Sat, 13 Nov 2021 15:30:32 GMT
VOLUME [/spiped]
# Sat, 13 Nov 2021 15:30:34 GMT
WORKDIR /spiped
# Sat, 13 Nov 2021 15:30:37 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 13 Nov 2021 15:30:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 13 Nov 2021 15:30:45 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:72940440c1ab65eca4d38846164719ffde4b147543cc658d041407a925b13368`  
		Last Modified: Fri, 12 Nov 2021 21:19:32 GMT  
		Size: 2.8 MB (2817467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63441839c077959763f01da2aec624ff02d5765af3e923419046fe79761bf71d`  
		Last Modified: Sat, 13 Nov 2021 15:31:20 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:907f83f2fcbfe22132bde253d7c486b65870dc9635bc53461fab20a90a87ad73`  
		Last Modified: Sat, 13 Nov 2021 15:31:20 GMT  
		Size: 7.8 KB (7777 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6096cf0d6847df2dfecdd48192e3922a4bbc85ed08ddfab7f33b335ffb6dc77`  
		Last Modified: Sat, 13 Nov 2021 15:31:20 GMT  
		Size: 221.7 KB (221712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e51da854d577591f12d32b8d52aeb0c4576b7254377303693f07d6a4854ef5f`  
		Last Modified: Sat, 13 Nov 2021 15:31:20 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e1d81a9ee14a2ec2938cd589d2bda48191378ac5f8717102a0203b9d37df9ff`  
		Last Modified: Sat, 13 Nov 2021 15:31:20 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; s390x

```console
$ docker pull spiped@sha256:118a8c071df238ccc4affa6c1ad90ecaa58fd6f20861ee190449b34b1f5734bd
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 MB (2824562 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a068554fae2e46941a18261fe2601c6c40df867a7b227b9bf154694451ba5390`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 12 Nov 2021 16:41:35 GMT
ADD file:7e0cf02b3f015b1a0f867c03b2902b85f2140be1cee7af63c23f367a487e4577 in / 
# Fri, 12 Nov 2021 16:41:36 GMT
CMD ["/bin/sh"]
# Fri, 12 Nov 2021 19:55:55 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 12 Nov 2021 19:55:56 GMT
RUN apk add --no-cache libssl1.1
# Fri, 12 Nov 2021 19:55:56 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 12 Nov 2021 19:56:06 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 12 Nov 2021 19:56:06 GMT
VOLUME [/spiped]
# Fri, 12 Nov 2021 19:56:06 GMT
WORKDIR /spiped
# Fri, 12 Nov 2021 19:56:06 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 12 Nov 2021 19:56:07 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 12 Nov 2021 19:56:07 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:817a13b0e05928f7491adbf1d2cf261ec35079112247bd03469bbe31156aca7c`  
		Last Modified: Fri, 12 Nov 2021 16:42:44 GMT  
		Size: 2.6 MB (2609278 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc797db23a37010d6b83bb8a9eaa1336ed352043857e5a44d68a4b8efad9e0b5`  
		Last Modified: Fri, 12 Nov 2021 19:56:35 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f44e810eed7330856c73daba855bc8adf50fdde87ccab6697c3416ee314886ca`  
		Last Modified: Fri, 12 Nov 2021 19:56:35 GMT  
		Size: 7.8 KB (7775 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f95a425358f95dbc88c89aac4c0c745bacaceb3d4598a051af18b0df4a28d76e`  
		Last Modified: Fri, 12 Nov 2021 19:56:35 GMT  
		Size: 205.8 KB (205773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc9c7009eddad4f11d690d41e57f47828edf66b3f5113d35cf2a68eee8beed75`  
		Last Modified: Fri, 12 Nov 2021 19:56:35 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5522513383757fa4cc180054c6b6b641c302050e0dce5ddfdd2a8881e7efcfa2`  
		Last Modified: Fri, 12 Nov 2021 19:56:35 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:1.6`

```console
$ docker pull spiped@sha256:ff3003949cdd1ced212cbb6bea1509e64d4fc152923eda3c284abfb51342637f
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
$ docker pull spiped@sha256:a696ea93d50ac968bc64ce5ab01eaf4ff13ae39fa9f099b9cd19a8e7a9d07aee
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.3 MB (37320955 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:683078eccb0851809c92a9dfdb1dcdd47c187bd8a7a5cc960a8fa55b1ece7e86`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 12 Oct 2021 01:20:42 GMT
ADD file:16dc2c6d1932194edec28d730b004fd6deca3d0f0e1a07bc5b8b6e8a1662f7af in / 
# Tue, 12 Oct 2021 01:20:42 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 16:21:25 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 12 Oct 2021 16:21:29 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 16:21:29 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Tue, 12 Oct 2021 16:21:56 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 12 Oct 2021 16:21:56 GMT
VOLUME [/spiped]
# Tue, 12 Oct 2021 16:21:56 GMT
WORKDIR /spiped
# Tue, 12 Oct 2021 16:21:57 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 12 Oct 2021 16:21:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 12 Oct 2021 16:21:57 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:7d63c13d9b9b6ec5f05a2b07daadacaa9c610d01102a662ae9b1d082105f1ffa`  
		Last Modified: Tue, 12 Oct 2021 01:26:05 GMT  
		Size: 31.4 MB (31357311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c825e91f209a1656f91feea4a2861373b55da8c1c3eb72e742c7f31c3d367918`  
		Last Modified: Tue, 12 Oct 2021 16:22:19 GMT  
		Size: 1.7 KB (1735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bba3f6cb28bad6f7f95e8be3b815465b3d5585c01a7cde8e6c561a81fd08d8e7`  
		Last Modified: Tue, 12 Oct 2021 16:22:19 GMT  
		Size: 1.1 KB (1051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbac5321939b951af500d72dc338b30ccdc61d354b3a466ce698a006ca3f4999`  
		Last Modified: Tue, 12 Oct 2021 16:22:20 GMT  
		Size: 6.0 MB (5960389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e58545b0e832a28e4b2fe9fe327f35158f38ccc204ce2c8fe1597803e860c0c2`  
		Last Modified: Tue, 12 Oct 2021 16:22:19 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c1557262dbc7e84098fd29719562170e4c257f980350cf3e68318ecd07a8956`  
		Last Modified: Tue, 12 Oct 2021 16:22:19 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; arm variant v5

```console
$ docker pull spiped@sha256:470773bf2dac565adf268ce74a10c0ca68c421d0de4192c4f6f29f15e8663e54
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.9 MB (33928107 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bee42cb8fa181c28acac6a722b80b4ea34b101698e1d8886a77f8323f3dbc1d2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 12 Oct 2021 00:50:30 GMT
ADD file:fb1afabdc1f93b4866b4c4d696f272b4888519cb5bf35eb7ed1a4c021d1a04c8 in / 
# Tue, 12 Oct 2021 00:50:30 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 11:33:43 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 12 Oct 2021 11:33:53 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 11:33:53 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Tue, 12 Oct 2021 11:34:54 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 12 Oct 2021 11:34:55 GMT
VOLUME [/spiped]
# Tue, 12 Oct 2021 11:34:55 GMT
WORKDIR /spiped
# Tue, 12 Oct 2021 11:34:56 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 12 Oct 2021 11:34:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 12 Oct 2021 11:34:57 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:5c9bab66abc5c53391435f6fd66e0ff3571295d568f45ac7d2dc480bcbfd56e8`  
		Last Modified: Tue, 12 Oct 2021 01:06:07 GMT  
		Size: 28.9 MB (28899715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b29fa5bfe046f908c4024b12760d6a235703129cf889a6b12fe9cb3c909e50ea`  
		Last Modified: Tue, 12 Oct 2021 11:35:35 GMT  
		Size: 1.7 KB (1725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f15e6ebdfdcc8907dc36ff08f672c463d0fbb6c59b0bb232ff1a229f64e4ea34`  
		Last Modified: Tue, 12 Oct 2021 11:35:35 GMT  
		Size: 1.1 KB (1053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0030f062ce13c3eb3f6f0020460e01e4beebed73ca735660e5fe74df98d62119`  
		Last Modified: Tue, 12 Oct 2021 11:35:40 GMT  
		Size: 5.0 MB (5025142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9edc074a3eb9dffdb9440831266c18299dcccc42834d767fc489b92ca7f2a48`  
		Last Modified: Tue, 12 Oct 2021 11:35:35 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ef7dd4a1c957efda249f4568cd568c8671c526848a4b9f57ffc9783bf81cef3`  
		Last Modified: Tue, 12 Oct 2021 11:35:35 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; arm variant v7

```console
$ docker pull spiped@sha256:958d2e76bb92a4709c36123b6553d179419227b06b733ec19cf1a4899da20853
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.3 MB (31309843 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9c0880cb9c6c234ff2fe6a3c163710a28845c22e1207ecd0b31cd8887cb77d26`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 12 Oct 2021 01:28:36 GMT
ADD file:89eac94007ac04f9168737686fa0a6c737f2c28fc9e5918d4d512924fe1973be in / 
# Tue, 12 Oct 2021 01:28:37 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 03:43:34 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 12 Oct 2021 03:43:41 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 03:43:42 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Tue, 12 Oct 2021 03:44:37 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 12 Oct 2021 03:44:37 GMT
VOLUME [/spiped]
# Tue, 12 Oct 2021 03:44:38 GMT
WORKDIR /spiped
# Tue, 12 Oct 2021 03:44:39 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 12 Oct 2021 03:44:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 12 Oct 2021 03:44:40 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:4e5300249f84466df4dc73ea0ce09938ca00c1718bb12619c4f26bd936162331`  
		Last Modified: Tue, 12 Oct 2021 01:44:28 GMT  
		Size: 26.6 MB (26561058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6ecc7e48d063e5bf0a086847e03c73699a183e8a9129e1b8ee3cab1482dde2d`  
		Last Modified: Tue, 12 Oct 2021 03:45:39 GMT  
		Size: 1.7 KB (1735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:584009012f86b47c7e4e6d1fd99c2d00976e77d0c5c66f0179ed3c7ea7c54725`  
		Last Modified: Tue, 12 Oct 2021 03:45:39 GMT  
		Size: 1.1 KB (1051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aae397080ab7f297afe0c2760bc744f5c6ab5ff8f88b8e0830bc8ae8d97b565f`  
		Last Modified: Tue, 12 Oct 2021 03:45:44 GMT  
		Size: 4.7 MB (4745527 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c697bb38b9e3862762d00df70d8a431fd891e25b33a03308c9e1cf59a02c712`  
		Last Modified: Tue, 12 Oct 2021 03:45:39 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0c305948d80dae9d7e0b495eba60d890696dba8079d33af0619bb473c03c079`  
		Last Modified: Tue, 12 Oct 2021 03:45:39 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:ddea46bf094678e8d8a63419789e3ff6b8df43ce2463fe054b2c6873958a7ed6
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.3 MB (35323019 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c62eeb5b4d9a5249368c594ef830ee32d99656d7accef9dec9afa2117c116bd4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 17 Nov 2021 02:40:15 GMT
ADD file:4203242b2b09a65239092c4780b59181da7b861b3c0be40810b3588aa200f72c in / 
# Wed, 17 Nov 2021 02:40:16 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 10:13:37 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 17 Nov 2021 10:13:41 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 10:13:42 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Wed, 17 Nov 2021 10:14:05 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 17 Nov 2021 10:14:06 GMT
VOLUME [/spiped]
# Wed, 17 Nov 2021 10:14:07 GMT
WORKDIR /spiped
# Wed, 17 Nov 2021 10:14:09 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 17 Nov 2021 10:14:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 17 Nov 2021 10:14:10 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:eb9a2845ed124d072b117aba4f0508e00c1ecd0d147dc324d14b00d24092046c`  
		Last Modified: Wed, 17 Nov 2021 02:47:17 GMT  
		Size: 30.1 MB (30056521 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b433167df10525b1b963a099589e5afac7d2b0fb31ccdd12d08134a7f543066`  
		Last Modified: Wed, 17 Nov 2021 10:14:43 GMT  
		Size: 1.6 KB (1616 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e176f2d91c6ad8f6d7ec824e8ecb1f7fc106c426f4717846a45154a39dcd214`  
		Last Modified: Wed, 17 Nov 2021 10:14:43 GMT  
		Size: 922.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99b725a99707e19e9152425097352ac163c18e25fdfdc11408f1b24926d88e21`  
		Last Modified: Wed, 17 Nov 2021 10:14:45 GMT  
		Size: 5.3 MB (5263526 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c46663b1e9b74612d1f081a80b43411d46c40cca2ca919d85b3e5651330d0e9`  
		Last Modified: Wed, 17 Nov 2021 10:14:44 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa44bd73d20d05c58e00bfff946eb6cab9b43fab597595cb74d0dcf53ab375c5`  
		Last Modified: Wed, 17 Nov 2021 10:14:43 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; 386

```console
$ docker pull spiped@sha256:1a250bf744242fee28c1506fa0085cd2e9f9467a0112a9497e7b6c5c7eda827b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.3 MB (40268237 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7f13080f172f1d6f15013062e14fd652880f18a736ef807504f9efeba0451496`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 17 Nov 2021 02:39:53 GMT
ADD file:ff018048717c0f5aa1730480d0bfea1c2bf94d6e2dae2d7cef46d05ffb0d93e1 in / 
# Wed, 17 Nov 2021 02:39:53 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 19:21:10 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 17 Nov 2021 19:21:18 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 19:21:18 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Wed, 17 Nov 2021 19:22:03 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 17 Nov 2021 19:22:04 GMT
VOLUME [/spiped]
# Wed, 17 Nov 2021 19:22:04 GMT
WORKDIR /spiped
# Wed, 17 Nov 2021 19:22:05 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 17 Nov 2021 19:22:05 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 17 Nov 2021 19:22:05 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:0bae0e1d4cb1d56ffeb9d05de7a097d3157267eef07b6d8131344d99bd97c431`  
		Last Modified: Wed, 17 Nov 2021 02:47:49 GMT  
		Size: 32.4 MB (32380683 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f71fd8d5c5711c96e84b1ce61114fe587d1427bf8042ef8ebf82882aa6b272a6`  
		Last Modified: Wed, 17 Nov 2021 19:23:02 GMT  
		Size: 1.7 KB (1734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c9611950dec2f42e40638d36289e1eef041b09d67ce4432d06ab76df0b5ace2`  
		Last Modified: Wed, 17 Nov 2021 19:23:03 GMT  
		Size: 1.1 KB (1055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:518b93d7db88cd296006861d6bca16590713db92325202daf9f4b7ebea46c840`  
		Last Modified: Wed, 17 Nov 2021 19:23:06 GMT  
		Size: 7.9 MB (7884295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd63e5a1b92185ac3ee583071d18f2c066670b2d466f8d18b888ba29e63ed182`  
		Last Modified: Wed, 17 Nov 2021 19:23:02 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc11c755ca357e2015909562f541b58552c232be20964fbba165a30990d5ebe1`  
		Last Modified: Wed, 17 Nov 2021 19:23:02 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; mips64le

```console
$ docker pull spiped@sha256:450f58414b6d98b4327999d964acbdfd088a4876c793662af1e6612a3c22e4f4
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.3 MB (35339707 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7fce297eacc4add3406390459583f251fc83bd3ae97b51328694b22fa7fe7772`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 17 Nov 2021 02:10:13 GMT
ADD file:10bc783d286d0a800f59d5009e87ecb4651659c82cae1325132756c7c8b1dec0 in / 
# Wed, 17 Nov 2021 02:10:13 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 08:27:05 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 17 Nov 2021 08:27:17 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 08:27:17 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Wed, 17 Nov 2021 08:28:30 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 17 Nov 2021 08:28:31 GMT
VOLUME [/spiped]
# Wed, 17 Nov 2021 08:28:31 GMT
WORKDIR /spiped
# Wed, 17 Nov 2021 08:28:32 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 17 Nov 2021 08:28:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 17 Nov 2021 08:28:32 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:08bca22fbffb4e58224e9e4f6a56f1ca5099c002b1aeb6181df63af308a3da58`  
		Last Modified: Wed, 17 Nov 2021 02:19:09 GMT  
		Size: 29.6 MB (29630388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac0800f7325d28791d9fbe530a7eef215f778350ecaf8ea10233b5921e861a07`  
		Last Modified: Wed, 17 Nov 2021 08:28:54 GMT  
		Size: 1.7 KB (1735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:566002f949cf54396dcd4f4732f10bb92a05a233c5e1ab60f79bff5a0fd57f63`  
		Last Modified: Wed, 17 Nov 2021 08:28:54 GMT  
		Size: 1.0 KB (1026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0339485e14c68084894399e67ee3e846ae570dd31af17ff0c7b996e2240cc8af`  
		Last Modified: Wed, 17 Nov 2021 08:29:00 GMT  
		Size: 5.7 MB (5706120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41d70628022717b6810fe3b62132cabe088e4c72a562033f04f332cd196b72c9`  
		Last Modified: Wed, 17 Nov 2021 08:28:54 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd86da81696b1bd0c2d983b7561e6bfa1c71b05b50c6e31685145ffc68ac067d`  
		Last Modified: Wed, 17 Nov 2021 08:28:54 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; ppc64le

```console
$ docker pull spiped@sha256:44b13757ab959642c428cd66c8a503318b7916932e88ee0f686aff3c40b6f88e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.3 MB (41263678 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aadb76166ced7d8733fac685c49d5b3e6c4e0ca8713e0c26fa2829ab87bb9172`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 12 Oct 2021 01:25:45 GMT
ADD file:d8794fadf16c9948c3574ba28740d08393eca57766340333ad91f9c2a33eb719 in / 
# Tue, 12 Oct 2021 01:25:53 GMT
CMD ["bash"]
# Wed, 13 Oct 2021 08:03:47 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 13 Oct 2021 08:03:59 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 13 Oct 2021 08:04:02 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Wed, 13 Oct 2021 08:07:07 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 13 Oct 2021 08:07:16 GMT
VOLUME [/spiped]
# Wed, 13 Oct 2021 08:07:24 GMT
WORKDIR /spiped
# Wed, 13 Oct 2021 08:07:26 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 13 Oct 2021 08:07:28 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 13 Oct 2021 08:07:32 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:6c28c1405c677dd809094d06190225b38cee3d24f18da38d287ef5bcc67884d6`  
		Last Modified: Tue, 12 Oct 2021 01:37:00 GMT  
		Size: 35.3 MB (35258729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44c02b2acecad78932397dca6224b551528ccaf70fed1c60da8884b1ee077de8`  
		Last Modified: Wed, 13 Oct 2021 08:08:15 GMT  
		Size: 1.7 KB (1745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1e5dcbe4d07e13aa9f6162d201034eb2b26b9f69987315148425a39102ba3df`  
		Last Modified: Wed, 13 Oct 2021 08:08:15 GMT  
		Size: 1.1 KB (1056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d805dc3af7457dd0105eca804e08afa7eed7d23d36613d054713cef0cd7f301a`  
		Last Modified: Wed, 13 Oct 2021 08:08:16 GMT  
		Size: 6.0 MB (6001677 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c36c3789c72419dd7c04f766b8ef090133dd4afbffd43366f439be9bdcb7d88`  
		Last Modified: Wed, 13 Oct 2021 08:08:15 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1414313671940f5f943d32775bed04903cb0d2af90ece5729859bf3a6284b292`  
		Last Modified: Wed, 13 Oct 2021 08:08:15 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; s390x

```console
$ docker pull spiped@sha256:bbdf535a02054a6706cd99a1fafde9724dd2417cfe9cbe59bb51a6a86fcdedfc
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.8 MB (34838172 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b0334f4bf3851c59d807ecc784fbf754bcc015f78bc339af17c7452c71ee0450`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 17 Nov 2021 02:42:27 GMT
ADD file:42f73dac307a6a5232e3100f3d3b36e8125f73a4ca504b106e60e2b66d242b2f in / 
# Wed, 17 Nov 2021 02:42:28 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 09:51:42 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 17 Nov 2021 09:51:44 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 09:51:44 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Wed, 17 Nov 2021 09:51:59 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 17 Nov 2021 09:52:00 GMT
VOLUME [/spiped]
# Wed, 17 Nov 2021 09:52:00 GMT
WORKDIR /spiped
# Wed, 17 Nov 2021 09:52:00 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 17 Nov 2021 09:52:00 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 17 Nov 2021 09:52:00 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:8d71e885edf612b507bbdcc48a970548d436b8709eeedfc2c98f6843a214b5e2`  
		Last Modified: Wed, 17 Nov 2021 02:48:25 GMT  
		Size: 29.7 MB (29650960 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b4e3a0c91da007baa099ab7d28b8282d97a1d427f8c3bfb6fa661fea558f431`  
		Last Modified: Wed, 17 Nov 2021 09:52:31 GMT  
		Size: 1.7 KB (1737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ea434878158c3e70134c052033e411e6633b141bdafd5fc45465e919790f3c9`  
		Last Modified: Wed, 17 Nov 2021 09:52:31 GMT  
		Size: 1.1 KB (1051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1680a353eb5f9bbeb5fa65bb02c66d997e5e0211cdf62ea04996f568f3a34af2`  
		Last Modified: Wed, 17 Nov 2021 09:52:32 GMT  
		Size: 5.2 MB (5183957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92981a4dda6befd75588ea56b9eb907cd8ab9daae831a0fb3b18c2dc37e4d7fe`  
		Last Modified: Wed, 17 Nov 2021 09:52:31 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76ef547fabd115d65e325e62fac7260ef1ce418b3c8ac5e5b8ca8b4efac73ed9`  
		Last Modified: Wed, 17 Nov 2021 09:52:31 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:1.6-alpine`

```console
$ docker pull spiped@sha256:1447fc83864d467400e6d1b2a87532955de7649123545804894c2a8c86d6a34a
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
$ docker pull spiped@sha256:5759c6e68d7e93789c7fc574722f42f3d3bafcaab2c4a8aeeeac5bb4772012a7
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (3045597 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1cc3e3a8422cee08ac18b30d97939a3a6bd28e94a61d0caaaa96ff86dd8f425c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 12 Nov 2021 17:19:44 GMT
ADD file:762c899ec0505d1a32930ee804c5b008825f41611161be104076cba33b7e5b2b in / 
# Fri, 12 Nov 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Sat, 13 Nov 2021 07:30:36 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Sat, 13 Nov 2021 07:30:37 GMT
RUN apk add --no-cache libssl1.1
# Sat, 13 Nov 2021 07:30:37 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Sat, 13 Nov 2021 07:31:02 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Sat, 13 Nov 2021 07:31:02 GMT
VOLUME [/spiped]
# Sat, 13 Nov 2021 07:31:03 GMT
WORKDIR /spiped
# Sat, 13 Nov 2021 07:31:03 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 13 Nov 2021 07:31:03 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 13 Nov 2021 07:31:04 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:97518928ae5f3d52d4164b314a7e73654eb686ecd8aafa0b79acd980773a740d`  
		Last Modified: Fri, 12 Nov 2021 17:20:39 GMT  
		Size: 2.8 MB (2822981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d272f2608cb29aaf56aaa58c4e8245793833d52257971c0a4a90c1445945548`  
		Last Modified: Sat, 13 Nov 2021 07:31:25 GMT  
		Size: 1.3 KB (1267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:588bebf547583661fb31be182d777849262971941c241f7b072c041f54e3c4ff`  
		Last Modified: Sat, 13 Nov 2021 07:31:25 GMT  
		Size: 7.8 KB (7767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:687f41a1ab4447065d651caf78075639eb1027290f0756c4d489a10c43a745af`  
		Last Modified: Sat, 13 Nov 2021 07:31:25 GMT  
		Size: 213.1 KB (213113 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0d7a22ad75e07e938780270586c7d97ddd070bf6b70ee31e6fbe14b6c79cda6`  
		Last Modified: Sat, 13 Nov 2021 07:31:25 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b484100590c35b883633e127830518528f9cc47bce7f4b864394b4bd85acb54`  
		Last Modified: Sat, 13 Nov 2021 07:31:25 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; arm variant v6

```console
$ docker pull spiped@sha256:e54c9ae8aa1651b3704440b6b74cbdd5ac80086e8fa25252df5ffbe44591eade
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 MB (2847905 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c6b358d015e8acc6b6eac3e79c5fc5302785d8bce806dc4640e51e684fc73495`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 12 Nov 2021 16:49:42 GMT
ADD file:6daf1fe862c00673bf9cf4d7e20b0bf253a56e7fb8ed5e730a4466ab9186e18a in / 
# Fri, 12 Nov 2021 16:49:44 GMT
CMD ["/bin/sh"]
# Sat, 13 Nov 2021 06:56:43 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Sat, 13 Nov 2021 06:56:48 GMT
RUN apk add --no-cache libssl1.1
# Sat, 13 Nov 2021 06:56:49 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Sat, 13 Nov 2021 06:57:26 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Sat, 13 Nov 2021 06:57:27 GMT
VOLUME [/spiped]
# Sat, 13 Nov 2021 06:57:27 GMT
WORKDIR /spiped
# Sat, 13 Nov 2021 06:57:28 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 13 Nov 2021 06:57:28 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 13 Nov 2021 06:57:29 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:56afcfda5d78cc243287acbaad250c5e8c0f47aae620dd7c51985b0d3c9b2728`  
		Last Modified: Fri, 12 Nov 2021 16:51:32 GMT  
		Size: 2.6 MB (2635392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbee8633a3e2da897713dd8453113fc924e1ad102e43bc673e5aa4e72a3c5ff6`  
		Last Modified: Sat, 13 Nov 2021 06:58:02 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b421d84dfbecebc99f29f801626a8781142421b8affb55b6dac49de522afdd86`  
		Last Modified: Sat, 13 Nov 2021 06:58:02 GMT  
		Size: 7.8 KB (7780 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c67a331696441ca0da524281edcd53ee4b8d52a24b4fdaab4f5b2e3833ab74a`  
		Last Modified: Sat, 13 Nov 2021 06:58:02 GMT  
		Size: 203.0 KB (202993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52ab514374a45d9fd16341748dc013e94fd9ddf0b15c2f3666bea84a2c2db7dd`  
		Last Modified: Sat, 13 Nov 2021 06:58:02 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:526ec51047ed2d4267785d4387f46cebef6e388cb755c73b640a73e44db871b6`  
		Last Modified: Sat, 13 Nov 2021 06:58:02 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; arm variant v7

```console
$ docker pull spiped@sha256:8b3e418343ca28cc6af7c79a9c92f500d16214863644d56f2e6a6c6a66f457d8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 MB (2644452 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3edd8179550b7c42a3827056d11ba4da9c0f384e1b5ac66177b911a1a9f75acc`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 12 Nov 2021 16:57:35 GMT
ADD file:03e0720458c3475758bf4394afa56f2165198eb91e6e9581f7768e433744dd9b in / 
# Fri, 12 Nov 2021 16:57:36 GMT
CMD ["/bin/sh"]
# Fri, 12 Nov 2021 19:09:19 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 12 Nov 2021 19:09:21 GMT
RUN apk add --no-cache libssl1.1
# Fri, 12 Nov 2021 19:09:22 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 12 Nov 2021 19:09:55 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 12 Nov 2021 19:09:55 GMT
VOLUME [/spiped]
# Fri, 12 Nov 2021 19:09:56 GMT
WORKDIR /spiped
# Fri, 12 Nov 2021 19:09:56 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 12 Nov 2021 19:09:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 12 Nov 2021 19:09:57 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:764d2e53e1a607f2d8261522185d5b9021ade3ec1a595664ee90308c00176899`  
		Last Modified: Fri, 12 Nov 2021 16:59:33 GMT  
		Size: 2.4 MB (2438618 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2462c3e2387f9df1b6daae812a3674ccd49db10b9b7251881ea1a034a39185b`  
		Last Modified: Fri, 12 Nov 2021 19:10:52 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9e4892bdd8b9be427ec2794ea13c95ec6cca78353d3c032d0fd2ba5acf9bae3`  
		Last Modified: Fri, 12 Nov 2021 19:10:52 GMT  
		Size: 7.8 KB (7791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:624ff05273c8a204e1361bc188430fe618799c3ec5471284aa49a1f9bd365020`  
		Last Modified: Fri, 12 Nov 2021 19:10:52 GMT  
		Size: 196.3 KB (196302 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f127d56c30dd5e8a58309b3d42c9c4f974256b6b1f1f9ff32b0ff78d8c372b3b`  
		Last Modified: Fri, 12 Nov 2021 19:10:52 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aab7e0d291c6010513c0721d4abf0cd1f407a631c23f515859004dddf983c5f5`  
		Last Modified: Fri, 12 Nov 2021 19:10:52 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:cbaa0533059fb17c768fe05790c3675b5b5cecf35f0b461e5347d763b1322af8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 MB (2932006 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a49787cc7861893f9d6020342db1639e60d7af6850ca4866d08840d8438a2b0c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 12 Nov 2021 16:39:58 GMT
ADD file:400c0466b29ccad54e0f6c0acef22542992828678c96693ef1f9f4d0551935d8 in / 
# Fri, 12 Nov 2021 16:39:58 GMT
CMD ["/bin/sh"]
# Fri, 12 Nov 2021 18:19:31 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 12 Nov 2021 18:19:33 GMT
RUN apk add --no-cache libssl1.1
# Fri, 12 Nov 2021 18:19:34 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 12 Nov 2021 18:19:54 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 12 Nov 2021 18:19:55 GMT
VOLUME [/spiped]
# Fri, 12 Nov 2021 18:19:56 GMT
WORKDIR /spiped
# Fri, 12 Nov 2021 18:19:58 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 12 Nov 2021 18:19:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 12 Nov 2021 18:19:59 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:be307f383ecc62b27a29b599c3fc9d3129693a798e7fcce614f09174cfe2d354`  
		Last Modified: Fri, 12 Nov 2021 16:40:59 GMT  
		Size: 2.7 MB (2717700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffbcce6bf922e4817964b0a9575d547fbb39004874a87c290658dcbb8939209e`  
		Last Modified: Fri, 12 Nov 2021 18:20:41 GMT  
		Size: 1.2 KB (1239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b342172a90f6f6a837eeb8f0025e02facad5a97fdd12c0aeac68c2411928d16f`  
		Last Modified: Fri, 12 Nov 2021 18:20:41 GMT  
		Size: 7.8 KB (7751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd8a670bc36ab2f74e650d7cb573c4c3542673b9488e2659efbc0d6b9db67529`  
		Last Modified: Fri, 12 Nov 2021 18:20:41 GMT  
		Size: 204.9 KB (204879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:698de19c09a4c9763fb04c4946f3bffafe6556fcfe73a3d55bbb4255f65bd458`  
		Last Modified: Fri, 12 Nov 2021 18:20:41 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1d1aa9a890181cdc95e60ea01849306cb72c967e13716722baa68c7bca76fdb`  
		Last Modified: Fri, 12 Nov 2021 18:20:42 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; 386

```console
$ docker pull spiped@sha256:ed9db1b4a0c65f0ca88573ca4e82bafaedde5032f465971dba93432ddcf67f67
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.1 MB (3064332 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:04afce967f7cf45ad1faa0b6e1d955f2bad9d1aff37c3659db5e809170762140`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 12 Nov 2021 16:38:42 GMT
ADD file:403428c2903dd9dea10d069185873cb2c2c3149c553797807c69f22aa3d12fe3 in / 
# Fri, 12 Nov 2021 16:38:42 GMT
CMD ["/bin/sh"]
# Fri, 12 Nov 2021 20:40:39 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 12 Nov 2021 20:40:41 GMT
RUN apk add --no-cache libssl1.1
# Fri, 12 Nov 2021 20:40:41 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 12 Nov 2021 20:41:13 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 12 Nov 2021 20:41:14 GMT
VOLUME [/spiped]
# Fri, 12 Nov 2021 20:41:14 GMT
WORKDIR /spiped
# Fri, 12 Nov 2021 20:41:15 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 12 Nov 2021 20:41:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 12 Nov 2021 20:41:16 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:5420e0d28c84ecb16748cb90cc6acf8e2a81dab10cb1f674f3eee8533e53c62a`  
		Last Modified: Fri, 12 Nov 2021 16:39:36 GMT  
		Size: 2.8 MB (2830948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9abea20678ed9ffc78867f8fc9674162184169da3d7c198cd24ec6b7439e0c88`  
		Last Modified: Fri, 12 Nov 2021 20:41:51 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f04cc4ba71752a6b9075421e6b0b7f08625406fb105f85e23547c4eb23b25f3`  
		Last Modified: Fri, 12 Nov 2021 20:41:51 GMT  
		Size: 7.8 KB (7770 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae957cbfbd7f9f36494cb3954e91d1ead35e68d61bbddf48904c4b6133c4c878`  
		Last Modified: Fri, 12 Nov 2021 20:41:51 GMT  
		Size: 223.9 KB (223875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:911b8888c5d7d41e887ed34d5f9c93d1d3241ad814e69f4d7def6b5debc96ae8`  
		Last Modified: Fri, 12 Nov 2021 20:41:51 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74d46a3df042754e1b8e655e102bf789f899a1f3758442759be66fe90573dbd2`  
		Last Modified: Fri, 12 Nov 2021 20:41:52 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; ppc64le

```console
$ docker pull spiped@sha256:892b50ba6b7bed8e6253a2577dcb2c38d0e60b1ae71968d978a808094e610768
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (3048694 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f7522decac983b5c7f6951cee379a5207bdbe044c9371a89a784e025923deb04`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 12 Nov 2021 21:18:00 GMT
ADD file:4d45063079cb28a34f1e382fddb22f156ac99d5449aa05ed37cb653c1f7b80f2 in / 
# Fri, 12 Nov 2021 21:18:01 GMT
CMD ["/bin/sh"]
# Sat, 13 Nov 2021 15:29:42 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Sat, 13 Nov 2021 15:29:55 GMT
RUN apk add --no-cache libssl1.1
# Sat, 13 Nov 2021 15:29:58 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Sat, 13 Nov 2021 15:30:26 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Sat, 13 Nov 2021 15:30:32 GMT
VOLUME [/spiped]
# Sat, 13 Nov 2021 15:30:34 GMT
WORKDIR /spiped
# Sat, 13 Nov 2021 15:30:37 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 13 Nov 2021 15:30:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 13 Nov 2021 15:30:45 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:72940440c1ab65eca4d38846164719ffde4b147543cc658d041407a925b13368`  
		Last Modified: Fri, 12 Nov 2021 21:19:32 GMT  
		Size: 2.8 MB (2817467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63441839c077959763f01da2aec624ff02d5765af3e923419046fe79761bf71d`  
		Last Modified: Sat, 13 Nov 2021 15:31:20 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:907f83f2fcbfe22132bde253d7c486b65870dc9635bc53461fab20a90a87ad73`  
		Last Modified: Sat, 13 Nov 2021 15:31:20 GMT  
		Size: 7.8 KB (7777 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6096cf0d6847df2dfecdd48192e3922a4bbc85ed08ddfab7f33b335ffb6dc77`  
		Last Modified: Sat, 13 Nov 2021 15:31:20 GMT  
		Size: 221.7 KB (221712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e51da854d577591f12d32b8d52aeb0c4576b7254377303693f07d6a4854ef5f`  
		Last Modified: Sat, 13 Nov 2021 15:31:20 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e1d81a9ee14a2ec2938cd589d2bda48191378ac5f8717102a0203b9d37df9ff`  
		Last Modified: Sat, 13 Nov 2021 15:31:20 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; s390x

```console
$ docker pull spiped@sha256:118a8c071df238ccc4affa6c1ad90ecaa58fd6f20861ee190449b34b1f5734bd
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 MB (2824562 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a068554fae2e46941a18261fe2601c6c40df867a7b227b9bf154694451ba5390`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 12 Nov 2021 16:41:35 GMT
ADD file:7e0cf02b3f015b1a0f867c03b2902b85f2140be1cee7af63c23f367a487e4577 in / 
# Fri, 12 Nov 2021 16:41:36 GMT
CMD ["/bin/sh"]
# Fri, 12 Nov 2021 19:55:55 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 12 Nov 2021 19:55:56 GMT
RUN apk add --no-cache libssl1.1
# Fri, 12 Nov 2021 19:55:56 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 12 Nov 2021 19:56:06 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 12 Nov 2021 19:56:06 GMT
VOLUME [/spiped]
# Fri, 12 Nov 2021 19:56:06 GMT
WORKDIR /spiped
# Fri, 12 Nov 2021 19:56:06 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 12 Nov 2021 19:56:07 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 12 Nov 2021 19:56:07 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:817a13b0e05928f7491adbf1d2cf261ec35079112247bd03469bbe31156aca7c`  
		Last Modified: Fri, 12 Nov 2021 16:42:44 GMT  
		Size: 2.6 MB (2609278 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc797db23a37010d6b83bb8a9eaa1336ed352043857e5a44d68a4b8efad9e0b5`  
		Last Modified: Fri, 12 Nov 2021 19:56:35 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f44e810eed7330856c73daba855bc8adf50fdde87ccab6697c3416ee314886ca`  
		Last Modified: Fri, 12 Nov 2021 19:56:35 GMT  
		Size: 7.8 KB (7775 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f95a425358f95dbc88c89aac4c0c745bacaceb3d4598a051af18b0df4a28d76e`  
		Last Modified: Fri, 12 Nov 2021 19:56:35 GMT  
		Size: 205.8 KB (205773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc9c7009eddad4f11d690d41e57f47828edf66b3f5113d35cf2a68eee8beed75`  
		Last Modified: Fri, 12 Nov 2021 19:56:35 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5522513383757fa4cc180054c6b6b641c302050e0dce5ddfdd2a8881e7efcfa2`  
		Last Modified: Fri, 12 Nov 2021 19:56:35 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:1.6.1`

```console
$ docker pull spiped@sha256:ff3003949cdd1ced212cbb6bea1509e64d4fc152923eda3c284abfb51342637f
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

### `spiped:1.6.1` - linux; amd64

```console
$ docker pull spiped@sha256:a696ea93d50ac968bc64ce5ab01eaf4ff13ae39fa9f099b9cd19a8e7a9d07aee
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.3 MB (37320955 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:683078eccb0851809c92a9dfdb1dcdd47c187bd8a7a5cc960a8fa55b1ece7e86`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 12 Oct 2021 01:20:42 GMT
ADD file:16dc2c6d1932194edec28d730b004fd6deca3d0f0e1a07bc5b8b6e8a1662f7af in / 
# Tue, 12 Oct 2021 01:20:42 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 16:21:25 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 12 Oct 2021 16:21:29 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 16:21:29 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Tue, 12 Oct 2021 16:21:56 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 12 Oct 2021 16:21:56 GMT
VOLUME [/spiped]
# Tue, 12 Oct 2021 16:21:56 GMT
WORKDIR /spiped
# Tue, 12 Oct 2021 16:21:57 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 12 Oct 2021 16:21:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 12 Oct 2021 16:21:57 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:7d63c13d9b9b6ec5f05a2b07daadacaa9c610d01102a662ae9b1d082105f1ffa`  
		Last Modified: Tue, 12 Oct 2021 01:26:05 GMT  
		Size: 31.4 MB (31357311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c825e91f209a1656f91feea4a2861373b55da8c1c3eb72e742c7f31c3d367918`  
		Last Modified: Tue, 12 Oct 2021 16:22:19 GMT  
		Size: 1.7 KB (1735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bba3f6cb28bad6f7f95e8be3b815465b3d5585c01a7cde8e6c561a81fd08d8e7`  
		Last Modified: Tue, 12 Oct 2021 16:22:19 GMT  
		Size: 1.1 KB (1051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbac5321939b951af500d72dc338b30ccdc61d354b3a466ce698a006ca3f4999`  
		Last Modified: Tue, 12 Oct 2021 16:22:20 GMT  
		Size: 6.0 MB (5960389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e58545b0e832a28e4b2fe9fe327f35158f38ccc204ce2c8fe1597803e860c0c2`  
		Last Modified: Tue, 12 Oct 2021 16:22:19 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c1557262dbc7e84098fd29719562170e4c257f980350cf3e68318ecd07a8956`  
		Last Modified: Tue, 12 Oct 2021 16:22:19 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1` - linux; arm variant v5

```console
$ docker pull spiped@sha256:470773bf2dac565adf268ce74a10c0ca68c421d0de4192c4f6f29f15e8663e54
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.9 MB (33928107 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bee42cb8fa181c28acac6a722b80b4ea34b101698e1d8886a77f8323f3dbc1d2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 12 Oct 2021 00:50:30 GMT
ADD file:fb1afabdc1f93b4866b4c4d696f272b4888519cb5bf35eb7ed1a4c021d1a04c8 in / 
# Tue, 12 Oct 2021 00:50:30 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 11:33:43 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 12 Oct 2021 11:33:53 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 11:33:53 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Tue, 12 Oct 2021 11:34:54 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 12 Oct 2021 11:34:55 GMT
VOLUME [/spiped]
# Tue, 12 Oct 2021 11:34:55 GMT
WORKDIR /spiped
# Tue, 12 Oct 2021 11:34:56 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 12 Oct 2021 11:34:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 12 Oct 2021 11:34:57 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:5c9bab66abc5c53391435f6fd66e0ff3571295d568f45ac7d2dc480bcbfd56e8`  
		Last Modified: Tue, 12 Oct 2021 01:06:07 GMT  
		Size: 28.9 MB (28899715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b29fa5bfe046f908c4024b12760d6a235703129cf889a6b12fe9cb3c909e50ea`  
		Last Modified: Tue, 12 Oct 2021 11:35:35 GMT  
		Size: 1.7 KB (1725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f15e6ebdfdcc8907dc36ff08f672c463d0fbb6c59b0bb232ff1a229f64e4ea34`  
		Last Modified: Tue, 12 Oct 2021 11:35:35 GMT  
		Size: 1.1 KB (1053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0030f062ce13c3eb3f6f0020460e01e4beebed73ca735660e5fe74df98d62119`  
		Last Modified: Tue, 12 Oct 2021 11:35:40 GMT  
		Size: 5.0 MB (5025142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9edc074a3eb9dffdb9440831266c18299dcccc42834d767fc489b92ca7f2a48`  
		Last Modified: Tue, 12 Oct 2021 11:35:35 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ef7dd4a1c957efda249f4568cd568c8671c526848a4b9f57ffc9783bf81cef3`  
		Last Modified: Tue, 12 Oct 2021 11:35:35 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1` - linux; arm variant v7

```console
$ docker pull spiped@sha256:958d2e76bb92a4709c36123b6553d179419227b06b733ec19cf1a4899da20853
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.3 MB (31309843 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9c0880cb9c6c234ff2fe6a3c163710a28845c22e1207ecd0b31cd8887cb77d26`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 12 Oct 2021 01:28:36 GMT
ADD file:89eac94007ac04f9168737686fa0a6c737f2c28fc9e5918d4d512924fe1973be in / 
# Tue, 12 Oct 2021 01:28:37 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 03:43:34 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 12 Oct 2021 03:43:41 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 03:43:42 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Tue, 12 Oct 2021 03:44:37 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 12 Oct 2021 03:44:37 GMT
VOLUME [/spiped]
# Tue, 12 Oct 2021 03:44:38 GMT
WORKDIR /spiped
# Tue, 12 Oct 2021 03:44:39 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 12 Oct 2021 03:44:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 12 Oct 2021 03:44:40 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:4e5300249f84466df4dc73ea0ce09938ca00c1718bb12619c4f26bd936162331`  
		Last Modified: Tue, 12 Oct 2021 01:44:28 GMT  
		Size: 26.6 MB (26561058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6ecc7e48d063e5bf0a086847e03c73699a183e8a9129e1b8ee3cab1482dde2d`  
		Last Modified: Tue, 12 Oct 2021 03:45:39 GMT  
		Size: 1.7 KB (1735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:584009012f86b47c7e4e6d1fd99c2d00976e77d0c5c66f0179ed3c7ea7c54725`  
		Last Modified: Tue, 12 Oct 2021 03:45:39 GMT  
		Size: 1.1 KB (1051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aae397080ab7f297afe0c2760bc744f5c6ab5ff8f88b8e0830bc8ae8d97b565f`  
		Last Modified: Tue, 12 Oct 2021 03:45:44 GMT  
		Size: 4.7 MB (4745527 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c697bb38b9e3862762d00df70d8a431fd891e25b33a03308c9e1cf59a02c712`  
		Last Modified: Tue, 12 Oct 2021 03:45:39 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0c305948d80dae9d7e0b495eba60d890696dba8079d33af0619bb473c03c079`  
		Last Modified: Tue, 12 Oct 2021 03:45:39 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:ddea46bf094678e8d8a63419789e3ff6b8df43ce2463fe054b2c6873958a7ed6
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.3 MB (35323019 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c62eeb5b4d9a5249368c594ef830ee32d99656d7accef9dec9afa2117c116bd4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 17 Nov 2021 02:40:15 GMT
ADD file:4203242b2b09a65239092c4780b59181da7b861b3c0be40810b3588aa200f72c in / 
# Wed, 17 Nov 2021 02:40:16 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 10:13:37 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 17 Nov 2021 10:13:41 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 10:13:42 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Wed, 17 Nov 2021 10:14:05 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 17 Nov 2021 10:14:06 GMT
VOLUME [/spiped]
# Wed, 17 Nov 2021 10:14:07 GMT
WORKDIR /spiped
# Wed, 17 Nov 2021 10:14:09 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 17 Nov 2021 10:14:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 17 Nov 2021 10:14:10 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:eb9a2845ed124d072b117aba4f0508e00c1ecd0d147dc324d14b00d24092046c`  
		Last Modified: Wed, 17 Nov 2021 02:47:17 GMT  
		Size: 30.1 MB (30056521 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b433167df10525b1b963a099589e5afac7d2b0fb31ccdd12d08134a7f543066`  
		Last Modified: Wed, 17 Nov 2021 10:14:43 GMT  
		Size: 1.6 KB (1616 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e176f2d91c6ad8f6d7ec824e8ecb1f7fc106c426f4717846a45154a39dcd214`  
		Last Modified: Wed, 17 Nov 2021 10:14:43 GMT  
		Size: 922.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99b725a99707e19e9152425097352ac163c18e25fdfdc11408f1b24926d88e21`  
		Last Modified: Wed, 17 Nov 2021 10:14:45 GMT  
		Size: 5.3 MB (5263526 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c46663b1e9b74612d1f081a80b43411d46c40cca2ca919d85b3e5651330d0e9`  
		Last Modified: Wed, 17 Nov 2021 10:14:44 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa44bd73d20d05c58e00bfff946eb6cab9b43fab597595cb74d0dcf53ab375c5`  
		Last Modified: Wed, 17 Nov 2021 10:14:43 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1` - linux; 386

```console
$ docker pull spiped@sha256:1a250bf744242fee28c1506fa0085cd2e9f9467a0112a9497e7b6c5c7eda827b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.3 MB (40268237 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7f13080f172f1d6f15013062e14fd652880f18a736ef807504f9efeba0451496`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 17 Nov 2021 02:39:53 GMT
ADD file:ff018048717c0f5aa1730480d0bfea1c2bf94d6e2dae2d7cef46d05ffb0d93e1 in / 
# Wed, 17 Nov 2021 02:39:53 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 19:21:10 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 17 Nov 2021 19:21:18 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 19:21:18 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Wed, 17 Nov 2021 19:22:03 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 17 Nov 2021 19:22:04 GMT
VOLUME [/spiped]
# Wed, 17 Nov 2021 19:22:04 GMT
WORKDIR /spiped
# Wed, 17 Nov 2021 19:22:05 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 17 Nov 2021 19:22:05 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 17 Nov 2021 19:22:05 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:0bae0e1d4cb1d56ffeb9d05de7a097d3157267eef07b6d8131344d99bd97c431`  
		Last Modified: Wed, 17 Nov 2021 02:47:49 GMT  
		Size: 32.4 MB (32380683 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f71fd8d5c5711c96e84b1ce61114fe587d1427bf8042ef8ebf82882aa6b272a6`  
		Last Modified: Wed, 17 Nov 2021 19:23:02 GMT  
		Size: 1.7 KB (1734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c9611950dec2f42e40638d36289e1eef041b09d67ce4432d06ab76df0b5ace2`  
		Last Modified: Wed, 17 Nov 2021 19:23:03 GMT  
		Size: 1.1 KB (1055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:518b93d7db88cd296006861d6bca16590713db92325202daf9f4b7ebea46c840`  
		Last Modified: Wed, 17 Nov 2021 19:23:06 GMT  
		Size: 7.9 MB (7884295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd63e5a1b92185ac3ee583071d18f2c066670b2d466f8d18b888ba29e63ed182`  
		Last Modified: Wed, 17 Nov 2021 19:23:02 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc11c755ca357e2015909562f541b58552c232be20964fbba165a30990d5ebe1`  
		Last Modified: Wed, 17 Nov 2021 19:23:02 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1` - linux; mips64le

```console
$ docker pull spiped@sha256:450f58414b6d98b4327999d964acbdfd088a4876c793662af1e6612a3c22e4f4
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.3 MB (35339707 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7fce297eacc4add3406390459583f251fc83bd3ae97b51328694b22fa7fe7772`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 17 Nov 2021 02:10:13 GMT
ADD file:10bc783d286d0a800f59d5009e87ecb4651659c82cae1325132756c7c8b1dec0 in / 
# Wed, 17 Nov 2021 02:10:13 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 08:27:05 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 17 Nov 2021 08:27:17 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 08:27:17 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Wed, 17 Nov 2021 08:28:30 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 17 Nov 2021 08:28:31 GMT
VOLUME [/spiped]
# Wed, 17 Nov 2021 08:28:31 GMT
WORKDIR /spiped
# Wed, 17 Nov 2021 08:28:32 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 17 Nov 2021 08:28:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 17 Nov 2021 08:28:32 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:08bca22fbffb4e58224e9e4f6a56f1ca5099c002b1aeb6181df63af308a3da58`  
		Last Modified: Wed, 17 Nov 2021 02:19:09 GMT  
		Size: 29.6 MB (29630388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac0800f7325d28791d9fbe530a7eef215f778350ecaf8ea10233b5921e861a07`  
		Last Modified: Wed, 17 Nov 2021 08:28:54 GMT  
		Size: 1.7 KB (1735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:566002f949cf54396dcd4f4732f10bb92a05a233c5e1ab60f79bff5a0fd57f63`  
		Last Modified: Wed, 17 Nov 2021 08:28:54 GMT  
		Size: 1.0 KB (1026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0339485e14c68084894399e67ee3e846ae570dd31af17ff0c7b996e2240cc8af`  
		Last Modified: Wed, 17 Nov 2021 08:29:00 GMT  
		Size: 5.7 MB (5706120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41d70628022717b6810fe3b62132cabe088e4c72a562033f04f332cd196b72c9`  
		Last Modified: Wed, 17 Nov 2021 08:28:54 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd86da81696b1bd0c2d983b7561e6bfa1c71b05b50c6e31685145ffc68ac067d`  
		Last Modified: Wed, 17 Nov 2021 08:28:54 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1` - linux; ppc64le

```console
$ docker pull spiped@sha256:44b13757ab959642c428cd66c8a503318b7916932e88ee0f686aff3c40b6f88e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.3 MB (41263678 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aadb76166ced7d8733fac685c49d5b3e6c4e0ca8713e0c26fa2829ab87bb9172`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 12 Oct 2021 01:25:45 GMT
ADD file:d8794fadf16c9948c3574ba28740d08393eca57766340333ad91f9c2a33eb719 in / 
# Tue, 12 Oct 2021 01:25:53 GMT
CMD ["bash"]
# Wed, 13 Oct 2021 08:03:47 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 13 Oct 2021 08:03:59 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 13 Oct 2021 08:04:02 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Wed, 13 Oct 2021 08:07:07 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 13 Oct 2021 08:07:16 GMT
VOLUME [/spiped]
# Wed, 13 Oct 2021 08:07:24 GMT
WORKDIR /spiped
# Wed, 13 Oct 2021 08:07:26 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 13 Oct 2021 08:07:28 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 13 Oct 2021 08:07:32 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:6c28c1405c677dd809094d06190225b38cee3d24f18da38d287ef5bcc67884d6`  
		Last Modified: Tue, 12 Oct 2021 01:37:00 GMT  
		Size: 35.3 MB (35258729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44c02b2acecad78932397dca6224b551528ccaf70fed1c60da8884b1ee077de8`  
		Last Modified: Wed, 13 Oct 2021 08:08:15 GMT  
		Size: 1.7 KB (1745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1e5dcbe4d07e13aa9f6162d201034eb2b26b9f69987315148425a39102ba3df`  
		Last Modified: Wed, 13 Oct 2021 08:08:15 GMT  
		Size: 1.1 KB (1056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d805dc3af7457dd0105eca804e08afa7eed7d23d36613d054713cef0cd7f301a`  
		Last Modified: Wed, 13 Oct 2021 08:08:16 GMT  
		Size: 6.0 MB (6001677 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c36c3789c72419dd7c04f766b8ef090133dd4afbffd43366f439be9bdcb7d88`  
		Last Modified: Wed, 13 Oct 2021 08:08:15 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1414313671940f5f943d32775bed04903cb0d2af90ece5729859bf3a6284b292`  
		Last Modified: Wed, 13 Oct 2021 08:08:15 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1` - linux; s390x

```console
$ docker pull spiped@sha256:bbdf535a02054a6706cd99a1fafde9724dd2417cfe9cbe59bb51a6a86fcdedfc
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.8 MB (34838172 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b0334f4bf3851c59d807ecc784fbf754bcc015f78bc339af17c7452c71ee0450`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 17 Nov 2021 02:42:27 GMT
ADD file:42f73dac307a6a5232e3100f3d3b36e8125f73a4ca504b106e60e2b66d242b2f in / 
# Wed, 17 Nov 2021 02:42:28 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 09:51:42 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 17 Nov 2021 09:51:44 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 09:51:44 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Wed, 17 Nov 2021 09:51:59 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 17 Nov 2021 09:52:00 GMT
VOLUME [/spiped]
# Wed, 17 Nov 2021 09:52:00 GMT
WORKDIR /spiped
# Wed, 17 Nov 2021 09:52:00 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 17 Nov 2021 09:52:00 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 17 Nov 2021 09:52:00 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:8d71e885edf612b507bbdcc48a970548d436b8709eeedfc2c98f6843a214b5e2`  
		Last Modified: Wed, 17 Nov 2021 02:48:25 GMT  
		Size: 29.7 MB (29650960 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b4e3a0c91da007baa099ab7d28b8282d97a1d427f8c3bfb6fa661fea558f431`  
		Last Modified: Wed, 17 Nov 2021 09:52:31 GMT  
		Size: 1.7 KB (1737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ea434878158c3e70134c052033e411e6633b141bdafd5fc45465e919790f3c9`  
		Last Modified: Wed, 17 Nov 2021 09:52:31 GMT  
		Size: 1.1 KB (1051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1680a353eb5f9bbeb5fa65bb02c66d997e5e0211cdf62ea04996f568f3a34af2`  
		Last Modified: Wed, 17 Nov 2021 09:52:32 GMT  
		Size: 5.2 MB (5183957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92981a4dda6befd75588ea56b9eb907cd8ab9daae831a0fb3b18c2dc37e4d7fe`  
		Last Modified: Wed, 17 Nov 2021 09:52:31 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76ef547fabd115d65e325e62fac7260ef1ce418b3c8ac5e5b8ca8b4efac73ed9`  
		Last Modified: Wed, 17 Nov 2021 09:52:31 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:1.6.1-alpine`

```console
$ docker pull spiped@sha256:1447fc83864d467400e6d1b2a87532955de7649123545804894c2a8c86d6a34a
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

### `spiped:1.6.1-alpine` - linux; amd64

```console
$ docker pull spiped@sha256:5759c6e68d7e93789c7fc574722f42f3d3bafcaab2c4a8aeeeac5bb4772012a7
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (3045597 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1cc3e3a8422cee08ac18b30d97939a3a6bd28e94a61d0caaaa96ff86dd8f425c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 12 Nov 2021 17:19:44 GMT
ADD file:762c899ec0505d1a32930ee804c5b008825f41611161be104076cba33b7e5b2b in / 
# Fri, 12 Nov 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Sat, 13 Nov 2021 07:30:36 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Sat, 13 Nov 2021 07:30:37 GMT
RUN apk add --no-cache libssl1.1
# Sat, 13 Nov 2021 07:30:37 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Sat, 13 Nov 2021 07:31:02 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Sat, 13 Nov 2021 07:31:02 GMT
VOLUME [/spiped]
# Sat, 13 Nov 2021 07:31:03 GMT
WORKDIR /spiped
# Sat, 13 Nov 2021 07:31:03 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 13 Nov 2021 07:31:03 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 13 Nov 2021 07:31:04 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:97518928ae5f3d52d4164b314a7e73654eb686ecd8aafa0b79acd980773a740d`  
		Last Modified: Fri, 12 Nov 2021 17:20:39 GMT  
		Size: 2.8 MB (2822981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d272f2608cb29aaf56aaa58c4e8245793833d52257971c0a4a90c1445945548`  
		Last Modified: Sat, 13 Nov 2021 07:31:25 GMT  
		Size: 1.3 KB (1267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:588bebf547583661fb31be182d777849262971941c241f7b072c041f54e3c4ff`  
		Last Modified: Sat, 13 Nov 2021 07:31:25 GMT  
		Size: 7.8 KB (7767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:687f41a1ab4447065d651caf78075639eb1027290f0756c4d489a10c43a745af`  
		Last Modified: Sat, 13 Nov 2021 07:31:25 GMT  
		Size: 213.1 KB (213113 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0d7a22ad75e07e938780270586c7d97ddd070bf6b70ee31e6fbe14b6c79cda6`  
		Last Modified: Sat, 13 Nov 2021 07:31:25 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b484100590c35b883633e127830518528f9cc47bce7f4b864394b4bd85acb54`  
		Last Modified: Sat, 13 Nov 2021 07:31:25 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1-alpine` - linux; arm variant v6

```console
$ docker pull spiped@sha256:e54c9ae8aa1651b3704440b6b74cbdd5ac80086e8fa25252df5ffbe44591eade
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 MB (2847905 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c6b358d015e8acc6b6eac3e79c5fc5302785d8bce806dc4640e51e684fc73495`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 12 Nov 2021 16:49:42 GMT
ADD file:6daf1fe862c00673bf9cf4d7e20b0bf253a56e7fb8ed5e730a4466ab9186e18a in / 
# Fri, 12 Nov 2021 16:49:44 GMT
CMD ["/bin/sh"]
# Sat, 13 Nov 2021 06:56:43 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Sat, 13 Nov 2021 06:56:48 GMT
RUN apk add --no-cache libssl1.1
# Sat, 13 Nov 2021 06:56:49 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Sat, 13 Nov 2021 06:57:26 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Sat, 13 Nov 2021 06:57:27 GMT
VOLUME [/spiped]
# Sat, 13 Nov 2021 06:57:27 GMT
WORKDIR /spiped
# Sat, 13 Nov 2021 06:57:28 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 13 Nov 2021 06:57:28 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 13 Nov 2021 06:57:29 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:56afcfda5d78cc243287acbaad250c5e8c0f47aae620dd7c51985b0d3c9b2728`  
		Last Modified: Fri, 12 Nov 2021 16:51:32 GMT  
		Size: 2.6 MB (2635392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbee8633a3e2da897713dd8453113fc924e1ad102e43bc673e5aa4e72a3c5ff6`  
		Last Modified: Sat, 13 Nov 2021 06:58:02 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b421d84dfbecebc99f29f801626a8781142421b8affb55b6dac49de522afdd86`  
		Last Modified: Sat, 13 Nov 2021 06:58:02 GMT  
		Size: 7.8 KB (7780 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c67a331696441ca0da524281edcd53ee4b8d52a24b4fdaab4f5b2e3833ab74a`  
		Last Modified: Sat, 13 Nov 2021 06:58:02 GMT  
		Size: 203.0 KB (202993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52ab514374a45d9fd16341748dc013e94fd9ddf0b15c2f3666bea84a2c2db7dd`  
		Last Modified: Sat, 13 Nov 2021 06:58:02 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:526ec51047ed2d4267785d4387f46cebef6e388cb755c73b640a73e44db871b6`  
		Last Modified: Sat, 13 Nov 2021 06:58:02 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1-alpine` - linux; arm variant v7

```console
$ docker pull spiped@sha256:8b3e418343ca28cc6af7c79a9c92f500d16214863644d56f2e6a6c6a66f457d8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 MB (2644452 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3edd8179550b7c42a3827056d11ba4da9c0f384e1b5ac66177b911a1a9f75acc`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 12 Nov 2021 16:57:35 GMT
ADD file:03e0720458c3475758bf4394afa56f2165198eb91e6e9581f7768e433744dd9b in / 
# Fri, 12 Nov 2021 16:57:36 GMT
CMD ["/bin/sh"]
# Fri, 12 Nov 2021 19:09:19 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 12 Nov 2021 19:09:21 GMT
RUN apk add --no-cache libssl1.1
# Fri, 12 Nov 2021 19:09:22 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 12 Nov 2021 19:09:55 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 12 Nov 2021 19:09:55 GMT
VOLUME [/spiped]
# Fri, 12 Nov 2021 19:09:56 GMT
WORKDIR /spiped
# Fri, 12 Nov 2021 19:09:56 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 12 Nov 2021 19:09:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 12 Nov 2021 19:09:57 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:764d2e53e1a607f2d8261522185d5b9021ade3ec1a595664ee90308c00176899`  
		Last Modified: Fri, 12 Nov 2021 16:59:33 GMT  
		Size: 2.4 MB (2438618 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2462c3e2387f9df1b6daae812a3674ccd49db10b9b7251881ea1a034a39185b`  
		Last Modified: Fri, 12 Nov 2021 19:10:52 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9e4892bdd8b9be427ec2794ea13c95ec6cca78353d3c032d0fd2ba5acf9bae3`  
		Last Modified: Fri, 12 Nov 2021 19:10:52 GMT  
		Size: 7.8 KB (7791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:624ff05273c8a204e1361bc188430fe618799c3ec5471284aa49a1f9bd365020`  
		Last Modified: Fri, 12 Nov 2021 19:10:52 GMT  
		Size: 196.3 KB (196302 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f127d56c30dd5e8a58309b3d42c9c4f974256b6b1f1f9ff32b0ff78d8c372b3b`  
		Last Modified: Fri, 12 Nov 2021 19:10:52 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aab7e0d291c6010513c0721d4abf0cd1f407a631c23f515859004dddf983c5f5`  
		Last Modified: Fri, 12 Nov 2021 19:10:52 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1-alpine` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:cbaa0533059fb17c768fe05790c3675b5b5cecf35f0b461e5347d763b1322af8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 MB (2932006 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a49787cc7861893f9d6020342db1639e60d7af6850ca4866d08840d8438a2b0c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 12 Nov 2021 16:39:58 GMT
ADD file:400c0466b29ccad54e0f6c0acef22542992828678c96693ef1f9f4d0551935d8 in / 
# Fri, 12 Nov 2021 16:39:58 GMT
CMD ["/bin/sh"]
# Fri, 12 Nov 2021 18:19:31 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 12 Nov 2021 18:19:33 GMT
RUN apk add --no-cache libssl1.1
# Fri, 12 Nov 2021 18:19:34 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 12 Nov 2021 18:19:54 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 12 Nov 2021 18:19:55 GMT
VOLUME [/spiped]
# Fri, 12 Nov 2021 18:19:56 GMT
WORKDIR /spiped
# Fri, 12 Nov 2021 18:19:58 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 12 Nov 2021 18:19:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 12 Nov 2021 18:19:59 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:be307f383ecc62b27a29b599c3fc9d3129693a798e7fcce614f09174cfe2d354`  
		Last Modified: Fri, 12 Nov 2021 16:40:59 GMT  
		Size: 2.7 MB (2717700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffbcce6bf922e4817964b0a9575d547fbb39004874a87c290658dcbb8939209e`  
		Last Modified: Fri, 12 Nov 2021 18:20:41 GMT  
		Size: 1.2 KB (1239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b342172a90f6f6a837eeb8f0025e02facad5a97fdd12c0aeac68c2411928d16f`  
		Last Modified: Fri, 12 Nov 2021 18:20:41 GMT  
		Size: 7.8 KB (7751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd8a670bc36ab2f74e650d7cb573c4c3542673b9488e2659efbc0d6b9db67529`  
		Last Modified: Fri, 12 Nov 2021 18:20:41 GMT  
		Size: 204.9 KB (204879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:698de19c09a4c9763fb04c4946f3bffafe6556fcfe73a3d55bbb4255f65bd458`  
		Last Modified: Fri, 12 Nov 2021 18:20:41 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1d1aa9a890181cdc95e60ea01849306cb72c967e13716722baa68c7bca76fdb`  
		Last Modified: Fri, 12 Nov 2021 18:20:42 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1-alpine` - linux; 386

```console
$ docker pull spiped@sha256:ed9db1b4a0c65f0ca88573ca4e82bafaedde5032f465971dba93432ddcf67f67
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.1 MB (3064332 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:04afce967f7cf45ad1faa0b6e1d955f2bad9d1aff37c3659db5e809170762140`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 12 Nov 2021 16:38:42 GMT
ADD file:403428c2903dd9dea10d069185873cb2c2c3149c553797807c69f22aa3d12fe3 in / 
# Fri, 12 Nov 2021 16:38:42 GMT
CMD ["/bin/sh"]
# Fri, 12 Nov 2021 20:40:39 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 12 Nov 2021 20:40:41 GMT
RUN apk add --no-cache libssl1.1
# Fri, 12 Nov 2021 20:40:41 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 12 Nov 2021 20:41:13 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 12 Nov 2021 20:41:14 GMT
VOLUME [/spiped]
# Fri, 12 Nov 2021 20:41:14 GMT
WORKDIR /spiped
# Fri, 12 Nov 2021 20:41:15 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 12 Nov 2021 20:41:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 12 Nov 2021 20:41:16 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:5420e0d28c84ecb16748cb90cc6acf8e2a81dab10cb1f674f3eee8533e53c62a`  
		Last Modified: Fri, 12 Nov 2021 16:39:36 GMT  
		Size: 2.8 MB (2830948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9abea20678ed9ffc78867f8fc9674162184169da3d7c198cd24ec6b7439e0c88`  
		Last Modified: Fri, 12 Nov 2021 20:41:51 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f04cc4ba71752a6b9075421e6b0b7f08625406fb105f85e23547c4eb23b25f3`  
		Last Modified: Fri, 12 Nov 2021 20:41:51 GMT  
		Size: 7.8 KB (7770 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae957cbfbd7f9f36494cb3954e91d1ead35e68d61bbddf48904c4b6133c4c878`  
		Last Modified: Fri, 12 Nov 2021 20:41:51 GMT  
		Size: 223.9 KB (223875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:911b8888c5d7d41e887ed34d5f9c93d1d3241ad814e69f4d7def6b5debc96ae8`  
		Last Modified: Fri, 12 Nov 2021 20:41:51 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74d46a3df042754e1b8e655e102bf789f899a1f3758442759be66fe90573dbd2`  
		Last Modified: Fri, 12 Nov 2021 20:41:52 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1-alpine` - linux; ppc64le

```console
$ docker pull spiped@sha256:892b50ba6b7bed8e6253a2577dcb2c38d0e60b1ae71968d978a808094e610768
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (3048694 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f7522decac983b5c7f6951cee379a5207bdbe044c9371a89a784e025923deb04`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 12 Nov 2021 21:18:00 GMT
ADD file:4d45063079cb28a34f1e382fddb22f156ac99d5449aa05ed37cb653c1f7b80f2 in / 
# Fri, 12 Nov 2021 21:18:01 GMT
CMD ["/bin/sh"]
# Sat, 13 Nov 2021 15:29:42 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Sat, 13 Nov 2021 15:29:55 GMT
RUN apk add --no-cache libssl1.1
# Sat, 13 Nov 2021 15:29:58 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Sat, 13 Nov 2021 15:30:26 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Sat, 13 Nov 2021 15:30:32 GMT
VOLUME [/spiped]
# Sat, 13 Nov 2021 15:30:34 GMT
WORKDIR /spiped
# Sat, 13 Nov 2021 15:30:37 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 13 Nov 2021 15:30:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 13 Nov 2021 15:30:45 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:72940440c1ab65eca4d38846164719ffde4b147543cc658d041407a925b13368`  
		Last Modified: Fri, 12 Nov 2021 21:19:32 GMT  
		Size: 2.8 MB (2817467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63441839c077959763f01da2aec624ff02d5765af3e923419046fe79761bf71d`  
		Last Modified: Sat, 13 Nov 2021 15:31:20 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:907f83f2fcbfe22132bde253d7c486b65870dc9635bc53461fab20a90a87ad73`  
		Last Modified: Sat, 13 Nov 2021 15:31:20 GMT  
		Size: 7.8 KB (7777 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6096cf0d6847df2dfecdd48192e3922a4bbc85ed08ddfab7f33b335ffb6dc77`  
		Last Modified: Sat, 13 Nov 2021 15:31:20 GMT  
		Size: 221.7 KB (221712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e51da854d577591f12d32b8d52aeb0c4576b7254377303693f07d6a4854ef5f`  
		Last Modified: Sat, 13 Nov 2021 15:31:20 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e1d81a9ee14a2ec2938cd589d2bda48191378ac5f8717102a0203b9d37df9ff`  
		Last Modified: Sat, 13 Nov 2021 15:31:20 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1-alpine` - linux; s390x

```console
$ docker pull spiped@sha256:118a8c071df238ccc4affa6c1ad90ecaa58fd6f20861ee190449b34b1f5734bd
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 MB (2824562 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a068554fae2e46941a18261fe2601c6c40df867a7b227b9bf154694451ba5390`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 12 Nov 2021 16:41:35 GMT
ADD file:7e0cf02b3f015b1a0f867c03b2902b85f2140be1cee7af63c23f367a487e4577 in / 
# Fri, 12 Nov 2021 16:41:36 GMT
CMD ["/bin/sh"]
# Fri, 12 Nov 2021 19:55:55 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 12 Nov 2021 19:55:56 GMT
RUN apk add --no-cache libssl1.1
# Fri, 12 Nov 2021 19:55:56 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 12 Nov 2021 19:56:06 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 12 Nov 2021 19:56:06 GMT
VOLUME [/spiped]
# Fri, 12 Nov 2021 19:56:06 GMT
WORKDIR /spiped
# Fri, 12 Nov 2021 19:56:06 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 12 Nov 2021 19:56:07 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 12 Nov 2021 19:56:07 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:817a13b0e05928f7491adbf1d2cf261ec35079112247bd03469bbe31156aca7c`  
		Last Modified: Fri, 12 Nov 2021 16:42:44 GMT  
		Size: 2.6 MB (2609278 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc797db23a37010d6b83bb8a9eaa1336ed352043857e5a44d68a4b8efad9e0b5`  
		Last Modified: Fri, 12 Nov 2021 19:56:35 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f44e810eed7330856c73daba855bc8adf50fdde87ccab6697c3416ee314886ca`  
		Last Modified: Fri, 12 Nov 2021 19:56:35 GMT  
		Size: 7.8 KB (7775 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f95a425358f95dbc88c89aac4c0c745bacaceb3d4598a051af18b0df4a28d76e`  
		Last Modified: Fri, 12 Nov 2021 19:56:35 GMT  
		Size: 205.8 KB (205773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc9c7009eddad4f11d690d41e57f47828edf66b3f5113d35cf2a68eee8beed75`  
		Last Modified: Fri, 12 Nov 2021 19:56:35 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5522513383757fa4cc180054c6b6b641c302050e0dce5ddfdd2a8881e7efcfa2`  
		Last Modified: Fri, 12 Nov 2021 19:56:35 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:alpine`

```console
$ docker pull spiped@sha256:1447fc83864d467400e6d1b2a87532955de7649123545804894c2a8c86d6a34a
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
$ docker pull spiped@sha256:5759c6e68d7e93789c7fc574722f42f3d3bafcaab2c4a8aeeeac5bb4772012a7
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (3045597 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1cc3e3a8422cee08ac18b30d97939a3a6bd28e94a61d0caaaa96ff86dd8f425c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 12 Nov 2021 17:19:44 GMT
ADD file:762c899ec0505d1a32930ee804c5b008825f41611161be104076cba33b7e5b2b in / 
# Fri, 12 Nov 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Sat, 13 Nov 2021 07:30:36 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Sat, 13 Nov 2021 07:30:37 GMT
RUN apk add --no-cache libssl1.1
# Sat, 13 Nov 2021 07:30:37 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Sat, 13 Nov 2021 07:31:02 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Sat, 13 Nov 2021 07:31:02 GMT
VOLUME [/spiped]
# Sat, 13 Nov 2021 07:31:03 GMT
WORKDIR /spiped
# Sat, 13 Nov 2021 07:31:03 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 13 Nov 2021 07:31:03 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 13 Nov 2021 07:31:04 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:97518928ae5f3d52d4164b314a7e73654eb686ecd8aafa0b79acd980773a740d`  
		Last Modified: Fri, 12 Nov 2021 17:20:39 GMT  
		Size: 2.8 MB (2822981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d272f2608cb29aaf56aaa58c4e8245793833d52257971c0a4a90c1445945548`  
		Last Modified: Sat, 13 Nov 2021 07:31:25 GMT  
		Size: 1.3 KB (1267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:588bebf547583661fb31be182d777849262971941c241f7b072c041f54e3c4ff`  
		Last Modified: Sat, 13 Nov 2021 07:31:25 GMT  
		Size: 7.8 KB (7767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:687f41a1ab4447065d651caf78075639eb1027290f0756c4d489a10c43a745af`  
		Last Modified: Sat, 13 Nov 2021 07:31:25 GMT  
		Size: 213.1 KB (213113 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0d7a22ad75e07e938780270586c7d97ddd070bf6b70ee31e6fbe14b6c79cda6`  
		Last Modified: Sat, 13 Nov 2021 07:31:25 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b484100590c35b883633e127830518528f9cc47bce7f4b864394b4bd85acb54`  
		Last Modified: Sat, 13 Nov 2021 07:31:25 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; arm variant v6

```console
$ docker pull spiped@sha256:e54c9ae8aa1651b3704440b6b74cbdd5ac80086e8fa25252df5ffbe44591eade
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 MB (2847905 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c6b358d015e8acc6b6eac3e79c5fc5302785d8bce806dc4640e51e684fc73495`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 12 Nov 2021 16:49:42 GMT
ADD file:6daf1fe862c00673bf9cf4d7e20b0bf253a56e7fb8ed5e730a4466ab9186e18a in / 
# Fri, 12 Nov 2021 16:49:44 GMT
CMD ["/bin/sh"]
# Sat, 13 Nov 2021 06:56:43 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Sat, 13 Nov 2021 06:56:48 GMT
RUN apk add --no-cache libssl1.1
# Sat, 13 Nov 2021 06:56:49 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Sat, 13 Nov 2021 06:57:26 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Sat, 13 Nov 2021 06:57:27 GMT
VOLUME [/spiped]
# Sat, 13 Nov 2021 06:57:27 GMT
WORKDIR /spiped
# Sat, 13 Nov 2021 06:57:28 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 13 Nov 2021 06:57:28 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 13 Nov 2021 06:57:29 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:56afcfda5d78cc243287acbaad250c5e8c0f47aae620dd7c51985b0d3c9b2728`  
		Last Modified: Fri, 12 Nov 2021 16:51:32 GMT  
		Size: 2.6 MB (2635392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbee8633a3e2da897713dd8453113fc924e1ad102e43bc673e5aa4e72a3c5ff6`  
		Last Modified: Sat, 13 Nov 2021 06:58:02 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b421d84dfbecebc99f29f801626a8781142421b8affb55b6dac49de522afdd86`  
		Last Modified: Sat, 13 Nov 2021 06:58:02 GMT  
		Size: 7.8 KB (7780 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c67a331696441ca0da524281edcd53ee4b8d52a24b4fdaab4f5b2e3833ab74a`  
		Last Modified: Sat, 13 Nov 2021 06:58:02 GMT  
		Size: 203.0 KB (202993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52ab514374a45d9fd16341748dc013e94fd9ddf0b15c2f3666bea84a2c2db7dd`  
		Last Modified: Sat, 13 Nov 2021 06:58:02 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:526ec51047ed2d4267785d4387f46cebef6e388cb755c73b640a73e44db871b6`  
		Last Modified: Sat, 13 Nov 2021 06:58:02 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; arm variant v7

```console
$ docker pull spiped@sha256:8b3e418343ca28cc6af7c79a9c92f500d16214863644d56f2e6a6c6a66f457d8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 MB (2644452 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3edd8179550b7c42a3827056d11ba4da9c0f384e1b5ac66177b911a1a9f75acc`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 12 Nov 2021 16:57:35 GMT
ADD file:03e0720458c3475758bf4394afa56f2165198eb91e6e9581f7768e433744dd9b in / 
# Fri, 12 Nov 2021 16:57:36 GMT
CMD ["/bin/sh"]
# Fri, 12 Nov 2021 19:09:19 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 12 Nov 2021 19:09:21 GMT
RUN apk add --no-cache libssl1.1
# Fri, 12 Nov 2021 19:09:22 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 12 Nov 2021 19:09:55 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 12 Nov 2021 19:09:55 GMT
VOLUME [/spiped]
# Fri, 12 Nov 2021 19:09:56 GMT
WORKDIR /spiped
# Fri, 12 Nov 2021 19:09:56 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 12 Nov 2021 19:09:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 12 Nov 2021 19:09:57 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:764d2e53e1a607f2d8261522185d5b9021ade3ec1a595664ee90308c00176899`  
		Last Modified: Fri, 12 Nov 2021 16:59:33 GMT  
		Size: 2.4 MB (2438618 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2462c3e2387f9df1b6daae812a3674ccd49db10b9b7251881ea1a034a39185b`  
		Last Modified: Fri, 12 Nov 2021 19:10:52 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9e4892bdd8b9be427ec2794ea13c95ec6cca78353d3c032d0fd2ba5acf9bae3`  
		Last Modified: Fri, 12 Nov 2021 19:10:52 GMT  
		Size: 7.8 KB (7791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:624ff05273c8a204e1361bc188430fe618799c3ec5471284aa49a1f9bd365020`  
		Last Modified: Fri, 12 Nov 2021 19:10:52 GMT  
		Size: 196.3 KB (196302 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f127d56c30dd5e8a58309b3d42c9c4f974256b6b1f1f9ff32b0ff78d8c372b3b`  
		Last Modified: Fri, 12 Nov 2021 19:10:52 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aab7e0d291c6010513c0721d4abf0cd1f407a631c23f515859004dddf983c5f5`  
		Last Modified: Fri, 12 Nov 2021 19:10:52 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:cbaa0533059fb17c768fe05790c3675b5b5cecf35f0b461e5347d763b1322af8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 MB (2932006 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a49787cc7861893f9d6020342db1639e60d7af6850ca4866d08840d8438a2b0c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 12 Nov 2021 16:39:58 GMT
ADD file:400c0466b29ccad54e0f6c0acef22542992828678c96693ef1f9f4d0551935d8 in / 
# Fri, 12 Nov 2021 16:39:58 GMT
CMD ["/bin/sh"]
# Fri, 12 Nov 2021 18:19:31 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 12 Nov 2021 18:19:33 GMT
RUN apk add --no-cache libssl1.1
# Fri, 12 Nov 2021 18:19:34 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 12 Nov 2021 18:19:54 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 12 Nov 2021 18:19:55 GMT
VOLUME [/spiped]
# Fri, 12 Nov 2021 18:19:56 GMT
WORKDIR /spiped
# Fri, 12 Nov 2021 18:19:58 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 12 Nov 2021 18:19:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 12 Nov 2021 18:19:59 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:be307f383ecc62b27a29b599c3fc9d3129693a798e7fcce614f09174cfe2d354`  
		Last Modified: Fri, 12 Nov 2021 16:40:59 GMT  
		Size: 2.7 MB (2717700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffbcce6bf922e4817964b0a9575d547fbb39004874a87c290658dcbb8939209e`  
		Last Modified: Fri, 12 Nov 2021 18:20:41 GMT  
		Size: 1.2 KB (1239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b342172a90f6f6a837eeb8f0025e02facad5a97fdd12c0aeac68c2411928d16f`  
		Last Modified: Fri, 12 Nov 2021 18:20:41 GMT  
		Size: 7.8 KB (7751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd8a670bc36ab2f74e650d7cb573c4c3542673b9488e2659efbc0d6b9db67529`  
		Last Modified: Fri, 12 Nov 2021 18:20:41 GMT  
		Size: 204.9 KB (204879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:698de19c09a4c9763fb04c4946f3bffafe6556fcfe73a3d55bbb4255f65bd458`  
		Last Modified: Fri, 12 Nov 2021 18:20:41 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1d1aa9a890181cdc95e60ea01849306cb72c967e13716722baa68c7bca76fdb`  
		Last Modified: Fri, 12 Nov 2021 18:20:42 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; 386

```console
$ docker pull spiped@sha256:ed9db1b4a0c65f0ca88573ca4e82bafaedde5032f465971dba93432ddcf67f67
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.1 MB (3064332 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:04afce967f7cf45ad1faa0b6e1d955f2bad9d1aff37c3659db5e809170762140`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 12 Nov 2021 16:38:42 GMT
ADD file:403428c2903dd9dea10d069185873cb2c2c3149c553797807c69f22aa3d12fe3 in / 
# Fri, 12 Nov 2021 16:38:42 GMT
CMD ["/bin/sh"]
# Fri, 12 Nov 2021 20:40:39 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 12 Nov 2021 20:40:41 GMT
RUN apk add --no-cache libssl1.1
# Fri, 12 Nov 2021 20:40:41 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 12 Nov 2021 20:41:13 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 12 Nov 2021 20:41:14 GMT
VOLUME [/spiped]
# Fri, 12 Nov 2021 20:41:14 GMT
WORKDIR /spiped
# Fri, 12 Nov 2021 20:41:15 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 12 Nov 2021 20:41:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 12 Nov 2021 20:41:16 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:5420e0d28c84ecb16748cb90cc6acf8e2a81dab10cb1f674f3eee8533e53c62a`  
		Last Modified: Fri, 12 Nov 2021 16:39:36 GMT  
		Size: 2.8 MB (2830948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9abea20678ed9ffc78867f8fc9674162184169da3d7c198cd24ec6b7439e0c88`  
		Last Modified: Fri, 12 Nov 2021 20:41:51 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f04cc4ba71752a6b9075421e6b0b7f08625406fb105f85e23547c4eb23b25f3`  
		Last Modified: Fri, 12 Nov 2021 20:41:51 GMT  
		Size: 7.8 KB (7770 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae957cbfbd7f9f36494cb3954e91d1ead35e68d61bbddf48904c4b6133c4c878`  
		Last Modified: Fri, 12 Nov 2021 20:41:51 GMT  
		Size: 223.9 KB (223875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:911b8888c5d7d41e887ed34d5f9c93d1d3241ad814e69f4d7def6b5debc96ae8`  
		Last Modified: Fri, 12 Nov 2021 20:41:51 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74d46a3df042754e1b8e655e102bf789f899a1f3758442759be66fe90573dbd2`  
		Last Modified: Fri, 12 Nov 2021 20:41:52 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; ppc64le

```console
$ docker pull spiped@sha256:892b50ba6b7bed8e6253a2577dcb2c38d0e60b1ae71968d978a808094e610768
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (3048694 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f7522decac983b5c7f6951cee379a5207bdbe044c9371a89a784e025923deb04`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 12 Nov 2021 21:18:00 GMT
ADD file:4d45063079cb28a34f1e382fddb22f156ac99d5449aa05ed37cb653c1f7b80f2 in / 
# Fri, 12 Nov 2021 21:18:01 GMT
CMD ["/bin/sh"]
# Sat, 13 Nov 2021 15:29:42 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Sat, 13 Nov 2021 15:29:55 GMT
RUN apk add --no-cache libssl1.1
# Sat, 13 Nov 2021 15:29:58 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Sat, 13 Nov 2021 15:30:26 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Sat, 13 Nov 2021 15:30:32 GMT
VOLUME [/spiped]
# Sat, 13 Nov 2021 15:30:34 GMT
WORKDIR /spiped
# Sat, 13 Nov 2021 15:30:37 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 13 Nov 2021 15:30:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 13 Nov 2021 15:30:45 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:72940440c1ab65eca4d38846164719ffde4b147543cc658d041407a925b13368`  
		Last Modified: Fri, 12 Nov 2021 21:19:32 GMT  
		Size: 2.8 MB (2817467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63441839c077959763f01da2aec624ff02d5765af3e923419046fe79761bf71d`  
		Last Modified: Sat, 13 Nov 2021 15:31:20 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:907f83f2fcbfe22132bde253d7c486b65870dc9635bc53461fab20a90a87ad73`  
		Last Modified: Sat, 13 Nov 2021 15:31:20 GMT  
		Size: 7.8 KB (7777 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6096cf0d6847df2dfecdd48192e3922a4bbc85ed08ddfab7f33b335ffb6dc77`  
		Last Modified: Sat, 13 Nov 2021 15:31:20 GMT  
		Size: 221.7 KB (221712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e51da854d577591f12d32b8d52aeb0c4576b7254377303693f07d6a4854ef5f`  
		Last Modified: Sat, 13 Nov 2021 15:31:20 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e1d81a9ee14a2ec2938cd589d2bda48191378ac5f8717102a0203b9d37df9ff`  
		Last Modified: Sat, 13 Nov 2021 15:31:20 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; s390x

```console
$ docker pull spiped@sha256:118a8c071df238ccc4affa6c1ad90ecaa58fd6f20861ee190449b34b1f5734bd
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 MB (2824562 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a068554fae2e46941a18261fe2601c6c40df867a7b227b9bf154694451ba5390`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 12 Nov 2021 16:41:35 GMT
ADD file:7e0cf02b3f015b1a0f867c03b2902b85f2140be1cee7af63c23f367a487e4577 in / 
# Fri, 12 Nov 2021 16:41:36 GMT
CMD ["/bin/sh"]
# Fri, 12 Nov 2021 19:55:55 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 12 Nov 2021 19:55:56 GMT
RUN apk add --no-cache libssl1.1
# Fri, 12 Nov 2021 19:55:56 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 12 Nov 2021 19:56:06 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 12 Nov 2021 19:56:06 GMT
VOLUME [/spiped]
# Fri, 12 Nov 2021 19:56:06 GMT
WORKDIR /spiped
# Fri, 12 Nov 2021 19:56:06 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 12 Nov 2021 19:56:07 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 12 Nov 2021 19:56:07 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:817a13b0e05928f7491adbf1d2cf261ec35079112247bd03469bbe31156aca7c`  
		Last Modified: Fri, 12 Nov 2021 16:42:44 GMT  
		Size: 2.6 MB (2609278 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc797db23a37010d6b83bb8a9eaa1336ed352043857e5a44d68a4b8efad9e0b5`  
		Last Modified: Fri, 12 Nov 2021 19:56:35 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f44e810eed7330856c73daba855bc8adf50fdde87ccab6697c3416ee314886ca`  
		Last Modified: Fri, 12 Nov 2021 19:56:35 GMT  
		Size: 7.8 KB (7775 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f95a425358f95dbc88c89aac4c0c745bacaceb3d4598a051af18b0df4a28d76e`  
		Last Modified: Fri, 12 Nov 2021 19:56:35 GMT  
		Size: 205.8 KB (205773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc9c7009eddad4f11d690d41e57f47828edf66b3f5113d35cf2a68eee8beed75`  
		Last Modified: Fri, 12 Nov 2021 19:56:35 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5522513383757fa4cc180054c6b6b641c302050e0dce5ddfdd2a8881e7efcfa2`  
		Last Modified: Fri, 12 Nov 2021 19:56:35 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:latest`

```console
$ docker pull spiped@sha256:ff3003949cdd1ced212cbb6bea1509e64d4fc152923eda3c284abfb51342637f
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
$ docker pull spiped@sha256:a696ea93d50ac968bc64ce5ab01eaf4ff13ae39fa9f099b9cd19a8e7a9d07aee
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.3 MB (37320955 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:683078eccb0851809c92a9dfdb1dcdd47c187bd8a7a5cc960a8fa55b1ece7e86`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 12 Oct 2021 01:20:42 GMT
ADD file:16dc2c6d1932194edec28d730b004fd6deca3d0f0e1a07bc5b8b6e8a1662f7af in / 
# Tue, 12 Oct 2021 01:20:42 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 16:21:25 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 12 Oct 2021 16:21:29 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 16:21:29 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Tue, 12 Oct 2021 16:21:56 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 12 Oct 2021 16:21:56 GMT
VOLUME [/spiped]
# Tue, 12 Oct 2021 16:21:56 GMT
WORKDIR /spiped
# Tue, 12 Oct 2021 16:21:57 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 12 Oct 2021 16:21:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 12 Oct 2021 16:21:57 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:7d63c13d9b9b6ec5f05a2b07daadacaa9c610d01102a662ae9b1d082105f1ffa`  
		Last Modified: Tue, 12 Oct 2021 01:26:05 GMT  
		Size: 31.4 MB (31357311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c825e91f209a1656f91feea4a2861373b55da8c1c3eb72e742c7f31c3d367918`  
		Last Modified: Tue, 12 Oct 2021 16:22:19 GMT  
		Size: 1.7 KB (1735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bba3f6cb28bad6f7f95e8be3b815465b3d5585c01a7cde8e6c561a81fd08d8e7`  
		Last Modified: Tue, 12 Oct 2021 16:22:19 GMT  
		Size: 1.1 KB (1051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbac5321939b951af500d72dc338b30ccdc61d354b3a466ce698a006ca3f4999`  
		Last Modified: Tue, 12 Oct 2021 16:22:20 GMT  
		Size: 6.0 MB (5960389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e58545b0e832a28e4b2fe9fe327f35158f38ccc204ce2c8fe1597803e860c0c2`  
		Last Modified: Tue, 12 Oct 2021 16:22:19 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c1557262dbc7e84098fd29719562170e4c257f980350cf3e68318ecd07a8956`  
		Last Modified: Tue, 12 Oct 2021 16:22:19 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; arm variant v5

```console
$ docker pull spiped@sha256:470773bf2dac565adf268ce74a10c0ca68c421d0de4192c4f6f29f15e8663e54
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.9 MB (33928107 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bee42cb8fa181c28acac6a722b80b4ea34b101698e1d8886a77f8323f3dbc1d2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 12 Oct 2021 00:50:30 GMT
ADD file:fb1afabdc1f93b4866b4c4d696f272b4888519cb5bf35eb7ed1a4c021d1a04c8 in / 
# Tue, 12 Oct 2021 00:50:30 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 11:33:43 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 12 Oct 2021 11:33:53 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 11:33:53 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Tue, 12 Oct 2021 11:34:54 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 12 Oct 2021 11:34:55 GMT
VOLUME [/spiped]
# Tue, 12 Oct 2021 11:34:55 GMT
WORKDIR /spiped
# Tue, 12 Oct 2021 11:34:56 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 12 Oct 2021 11:34:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 12 Oct 2021 11:34:57 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:5c9bab66abc5c53391435f6fd66e0ff3571295d568f45ac7d2dc480bcbfd56e8`  
		Last Modified: Tue, 12 Oct 2021 01:06:07 GMT  
		Size: 28.9 MB (28899715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b29fa5bfe046f908c4024b12760d6a235703129cf889a6b12fe9cb3c909e50ea`  
		Last Modified: Tue, 12 Oct 2021 11:35:35 GMT  
		Size: 1.7 KB (1725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f15e6ebdfdcc8907dc36ff08f672c463d0fbb6c59b0bb232ff1a229f64e4ea34`  
		Last Modified: Tue, 12 Oct 2021 11:35:35 GMT  
		Size: 1.1 KB (1053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0030f062ce13c3eb3f6f0020460e01e4beebed73ca735660e5fe74df98d62119`  
		Last Modified: Tue, 12 Oct 2021 11:35:40 GMT  
		Size: 5.0 MB (5025142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9edc074a3eb9dffdb9440831266c18299dcccc42834d767fc489b92ca7f2a48`  
		Last Modified: Tue, 12 Oct 2021 11:35:35 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ef7dd4a1c957efda249f4568cd568c8671c526848a4b9f57ffc9783bf81cef3`  
		Last Modified: Tue, 12 Oct 2021 11:35:35 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; arm variant v7

```console
$ docker pull spiped@sha256:958d2e76bb92a4709c36123b6553d179419227b06b733ec19cf1a4899da20853
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.3 MB (31309843 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9c0880cb9c6c234ff2fe6a3c163710a28845c22e1207ecd0b31cd8887cb77d26`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 12 Oct 2021 01:28:36 GMT
ADD file:89eac94007ac04f9168737686fa0a6c737f2c28fc9e5918d4d512924fe1973be in / 
# Tue, 12 Oct 2021 01:28:37 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 03:43:34 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 12 Oct 2021 03:43:41 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 03:43:42 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Tue, 12 Oct 2021 03:44:37 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 12 Oct 2021 03:44:37 GMT
VOLUME [/spiped]
# Tue, 12 Oct 2021 03:44:38 GMT
WORKDIR /spiped
# Tue, 12 Oct 2021 03:44:39 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 12 Oct 2021 03:44:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 12 Oct 2021 03:44:40 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:4e5300249f84466df4dc73ea0ce09938ca00c1718bb12619c4f26bd936162331`  
		Last Modified: Tue, 12 Oct 2021 01:44:28 GMT  
		Size: 26.6 MB (26561058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6ecc7e48d063e5bf0a086847e03c73699a183e8a9129e1b8ee3cab1482dde2d`  
		Last Modified: Tue, 12 Oct 2021 03:45:39 GMT  
		Size: 1.7 KB (1735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:584009012f86b47c7e4e6d1fd99c2d00976e77d0c5c66f0179ed3c7ea7c54725`  
		Last Modified: Tue, 12 Oct 2021 03:45:39 GMT  
		Size: 1.1 KB (1051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aae397080ab7f297afe0c2760bc744f5c6ab5ff8f88b8e0830bc8ae8d97b565f`  
		Last Modified: Tue, 12 Oct 2021 03:45:44 GMT  
		Size: 4.7 MB (4745527 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c697bb38b9e3862762d00df70d8a431fd891e25b33a03308c9e1cf59a02c712`  
		Last Modified: Tue, 12 Oct 2021 03:45:39 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0c305948d80dae9d7e0b495eba60d890696dba8079d33af0619bb473c03c079`  
		Last Modified: Tue, 12 Oct 2021 03:45:39 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:ddea46bf094678e8d8a63419789e3ff6b8df43ce2463fe054b2c6873958a7ed6
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.3 MB (35323019 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c62eeb5b4d9a5249368c594ef830ee32d99656d7accef9dec9afa2117c116bd4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 17 Nov 2021 02:40:15 GMT
ADD file:4203242b2b09a65239092c4780b59181da7b861b3c0be40810b3588aa200f72c in / 
# Wed, 17 Nov 2021 02:40:16 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 10:13:37 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 17 Nov 2021 10:13:41 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 10:13:42 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Wed, 17 Nov 2021 10:14:05 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 17 Nov 2021 10:14:06 GMT
VOLUME [/spiped]
# Wed, 17 Nov 2021 10:14:07 GMT
WORKDIR /spiped
# Wed, 17 Nov 2021 10:14:09 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 17 Nov 2021 10:14:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 17 Nov 2021 10:14:10 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:eb9a2845ed124d072b117aba4f0508e00c1ecd0d147dc324d14b00d24092046c`  
		Last Modified: Wed, 17 Nov 2021 02:47:17 GMT  
		Size: 30.1 MB (30056521 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b433167df10525b1b963a099589e5afac7d2b0fb31ccdd12d08134a7f543066`  
		Last Modified: Wed, 17 Nov 2021 10:14:43 GMT  
		Size: 1.6 KB (1616 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e176f2d91c6ad8f6d7ec824e8ecb1f7fc106c426f4717846a45154a39dcd214`  
		Last Modified: Wed, 17 Nov 2021 10:14:43 GMT  
		Size: 922.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99b725a99707e19e9152425097352ac163c18e25fdfdc11408f1b24926d88e21`  
		Last Modified: Wed, 17 Nov 2021 10:14:45 GMT  
		Size: 5.3 MB (5263526 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c46663b1e9b74612d1f081a80b43411d46c40cca2ca919d85b3e5651330d0e9`  
		Last Modified: Wed, 17 Nov 2021 10:14:44 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa44bd73d20d05c58e00bfff946eb6cab9b43fab597595cb74d0dcf53ab375c5`  
		Last Modified: Wed, 17 Nov 2021 10:14:43 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; 386

```console
$ docker pull spiped@sha256:1a250bf744242fee28c1506fa0085cd2e9f9467a0112a9497e7b6c5c7eda827b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.3 MB (40268237 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7f13080f172f1d6f15013062e14fd652880f18a736ef807504f9efeba0451496`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 17 Nov 2021 02:39:53 GMT
ADD file:ff018048717c0f5aa1730480d0bfea1c2bf94d6e2dae2d7cef46d05ffb0d93e1 in / 
# Wed, 17 Nov 2021 02:39:53 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 19:21:10 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 17 Nov 2021 19:21:18 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 19:21:18 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Wed, 17 Nov 2021 19:22:03 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 17 Nov 2021 19:22:04 GMT
VOLUME [/spiped]
# Wed, 17 Nov 2021 19:22:04 GMT
WORKDIR /spiped
# Wed, 17 Nov 2021 19:22:05 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 17 Nov 2021 19:22:05 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 17 Nov 2021 19:22:05 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:0bae0e1d4cb1d56ffeb9d05de7a097d3157267eef07b6d8131344d99bd97c431`  
		Last Modified: Wed, 17 Nov 2021 02:47:49 GMT  
		Size: 32.4 MB (32380683 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f71fd8d5c5711c96e84b1ce61114fe587d1427bf8042ef8ebf82882aa6b272a6`  
		Last Modified: Wed, 17 Nov 2021 19:23:02 GMT  
		Size: 1.7 KB (1734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c9611950dec2f42e40638d36289e1eef041b09d67ce4432d06ab76df0b5ace2`  
		Last Modified: Wed, 17 Nov 2021 19:23:03 GMT  
		Size: 1.1 KB (1055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:518b93d7db88cd296006861d6bca16590713db92325202daf9f4b7ebea46c840`  
		Last Modified: Wed, 17 Nov 2021 19:23:06 GMT  
		Size: 7.9 MB (7884295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd63e5a1b92185ac3ee583071d18f2c066670b2d466f8d18b888ba29e63ed182`  
		Last Modified: Wed, 17 Nov 2021 19:23:02 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc11c755ca357e2015909562f541b58552c232be20964fbba165a30990d5ebe1`  
		Last Modified: Wed, 17 Nov 2021 19:23:02 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; mips64le

```console
$ docker pull spiped@sha256:450f58414b6d98b4327999d964acbdfd088a4876c793662af1e6612a3c22e4f4
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.3 MB (35339707 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7fce297eacc4add3406390459583f251fc83bd3ae97b51328694b22fa7fe7772`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 17 Nov 2021 02:10:13 GMT
ADD file:10bc783d286d0a800f59d5009e87ecb4651659c82cae1325132756c7c8b1dec0 in / 
# Wed, 17 Nov 2021 02:10:13 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 08:27:05 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 17 Nov 2021 08:27:17 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 08:27:17 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Wed, 17 Nov 2021 08:28:30 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 17 Nov 2021 08:28:31 GMT
VOLUME [/spiped]
# Wed, 17 Nov 2021 08:28:31 GMT
WORKDIR /spiped
# Wed, 17 Nov 2021 08:28:32 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 17 Nov 2021 08:28:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 17 Nov 2021 08:28:32 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:08bca22fbffb4e58224e9e4f6a56f1ca5099c002b1aeb6181df63af308a3da58`  
		Last Modified: Wed, 17 Nov 2021 02:19:09 GMT  
		Size: 29.6 MB (29630388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac0800f7325d28791d9fbe530a7eef215f778350ecaf8ea10233b5921e861a07`  
		Last Modified: Wed, 17 Nov 2021 08:28:54 GMT  
		Size: 1.7 KB (1735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:566002f949cf54396dcd4f4732f10bb92a05a233c5e1ab60f79bff5a0fd57f63`  
		Last Modified: Wed, 17 Nov 2021 08:28:54 GMT  
		Size: 1.0 KB (1026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0339485e14c68084894399e67ee3e846ae570dd31af17ff0c7b996e2240cc8af`  
		Last Modified: Wed, 17 Nov 2021 08:29:00 GMT  
		Size: 5.7 MB (5706120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41d70628022717b6810fe3b62132cabe088e4c72a562033f04f332cd196b72c9`  
		Last Modified: Wed, 17 Nov 2021 08:28:54 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd86da81696b1bd0c2d983b7561e6bfa1c71b05b50c6e31685145ffc68ac067d`  
		Last Modified: Wed, 17 Nov 2021 08:28:54 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; ppc64le

```console
$ docker pull spiped@sha256:44b13757ab959642c428cd66c8a503318b7916932e88ee0f686aff3c40b6f88e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.3 MB (41263678 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aadb76166ced7d8733fac685c49d5b3e6c4e0ca8713e0c26fa2829ab87bb9172`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 12 Oct 2021 01:25:45 GMT
ADD file:d8794fadf16c9948c3574ba28740d08393eca57766340333ad91f9c2a33eb719 in / 
# Tue, 12 Oct 2021 01:25:53 GMT
CMD ["bash"]
# Wed, 13 Oct 2021 08:03:47 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 13 Oct 2021 08:03:59 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 13 Oct 2021 08:04:02 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Wed, 13 Oct 2021 08:07:07 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 13 Oct 2021 08:07:16 GMT
VOLUME [/spiped]
# Wed, 13 Oct 2021 08:07:24 GMT
WORKDIR /spiped
# Wed, 13 Oct 2021 08:07:26 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 13 Oct 2021 08:07:28 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 13 Oct 2021 08:07:32 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:6c28c1405c677dd809094d06190225b38cee3d24f18da38d287ef5bcc67884d6`  
		Last Modified: Tue, 12 Oct 2021 01:37:00 GMT  
		Size: 35.3 MB (35258729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44c02b2acecad78932397dca6224b551528ccaf70fed1c60da8884b1ee077de8`  
		Last Modified: Wed, 13 Oct 2021 08:08:15 GMT  
		Size: 1.7 KB (1745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1e5dcbe4d07e13aa9f6162d201034eb2b26b9f69987315148425a39102ba3df`  
		Last Modified: Wed, 13 Oct 2021 08:08:15 GMT  
		Size: 1.1 KB (1056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d805dc3af7457dd0105eca804e08afa7eed7d23d36613d054713cef0cd7f301a`  
		Last Modified: Wed, 13 Oct 2021 08:08:16 GMT  
		Size: 6.0 MB (6001677 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c36c3789c72419dd7c04f766b8ef090133dd4afbffd43366f439be9bdcb7d88`  
		Last Modified: Wed, 13 Oct 2021 08:08:15 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1414313671940f5f943d32775bed04903cb0d2af90ece5729859bf3a6284b292`  
		Last Modified: Wed, 13 Oct 2021 08:08:15 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; s390x

```console
$ docker pull spiped@sha256:bbdf535a02054a6706cd99a1fafde9724dd2417cfe9cbe59bb51a6a86fcdedfc
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.8 MB (34838172 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b0334f4bf3851c59d807ecc784fbf754bcc015f78bc339af17c7452c71ee0450`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 17 Nov 2021 02:42:27 GMT
ADD file:42f73dac307a6a5232e3100f3d3b36e8125f73a4ca504b106e60e2b66d242b2f in / 
# Wed, 17 Nov 2021 02:42:28 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 09:51:42 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 17 Nov 2021 09:51:44 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 09:51:44 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Wed, 17 Nov 2021 09:51:59 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 17 Nov 2021 09:52:00 GMT
VOLUME [/spiped]
# Wed, 17 Nov 2021 09:52:00 GMT
WORKDIR /spiped
# Wed, 17 Nov 2021 09:52:00 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 17 Nov 2021 09:52:00 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 17 Nov 2021 09:52:00 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:8d71e885edf612b507bbdcc48a970548d436b8709eeedfc2c98f6843a214b5e2`  
		Last Modified: Wed, 17 Nov 2021 02:48:25 GMT  
		Size: 29.7 MB (29650960 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b4e3a0c91da007baa099ab7d28b8282d97a1d427f8c3bfb6fa661fea558f431`  
		Last Modified: Wed, 17 Nov 2021 09:52:31 GMT  
		Size: 1.7 KB (1737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ea434878158c3e70134c052033e411e6633b141bdafd5fc45465e919790f3c9`  
		Last Modified: Wed, 17 Nov 2021 09:52:31 GMT  
		Size: 1.1 KB (1051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1680a353eb5f9bbeb5fa65bb02c66d997e5e0211cdf62ea04996f568f3a34af2`  
		Last Modified: Wed, 17 Nov 2021 09:52:32 GMT  
		Size: 5.2 MB (5183957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92981a4dda6befd75588ea56b9eb907cd8ab9daae831a0fb3b18c2dc37e4d7fe`  
		Last Modified: Wed, 17 Nov 2021 09:52:31 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76ef547fabd115d65e325e62fac7260ef1ce418b3c8ac5e5b8ca8b4efac73ed9`  
		Last Modified: Wed, 17 Nov 2021 09:52:31 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
