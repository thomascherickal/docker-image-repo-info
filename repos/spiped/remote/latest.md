## `spiped:latest`

```console
$ docker pull spiped@sha256:e38334cb8a3058ff5c9de5d7bf7f86ad99393b8094f76013c42d23f698c35a16
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
$ docker pull spiped@sha256:515eeff0790a66d6f804a47e6066d0dc088ebce04e8b14f9d25c1907ae717db2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.4 MB (37414538 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ac8398d3028b7e7e89842d7546b1b809800bb5fdaf11ae1a3eb9ea880c93fc6b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 06 Dec 2022 01:20:54 GMT
ADD file:1f1efd56601ebc26a041a7b994a380ef68112b91a078e225753bee7b3196d22c in / 
# Tue, 06 Dec 2022 01:20:54 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 08:03:32 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 06 Dec 2022 08:03:35 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 06 Dec 2022 08:03:35 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 06 Dec 2022 08:03:55 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 06 Dec 2022 08:03:56 GMT
VOLUME [/spiped]
# Tue, 06 Dec 2022 08:03:56 GMT
WORKDIR /spiped
# Tue, 06 Dec 2022 08:03:56 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 06 Dec 2022 08:03:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 06 Dec 2022 08:03:56 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:025c56f98b679f70b7a54241917e56da7b59ab9d2defecc6ebdb0bf2750484bb`  
		Last Modified: Tue, 06 Dec 2022 01:25:12 GMT  
		Size: 31.4 MB (31412852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec62ed2a44d78c21ab72e8eee1fbc27cb1392fa8cf508574175d315ea02cc2b0`  
		Last Modified: Tue, 06 Dec 2022 08:04:14 GMT  
		Size: 1.7 KB (1733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c75e86d7e6035b646443c975a02019d31e645279762165d8a50f2c67f932c079`  
		Last Modified: Tue, 06 Dec 2022 08:04:14 GMT  
		Size: 1.1 KB (1055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee2a87693b0022c3ad8f9fab9c55b79e7493e4f5f6bfe661963a18bcf230ad13`  
		Last Modified: Tue, 06 Dec 2022 08:04:15 GMT  
		Size: 6.0 MB (5998429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02692279b0822562e0d73effc9e6e2658002863fa714173db9d3c646773ad1df`  
		Last Modified: Tue, 06 Dec 2022 08:04:14 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:454f02843045aeaf0a03708f693de0cd7996b5ad9880831a2bcad1532f6baf19`  
		Last Modified: Tue, 06 Dec 2022 08:04:14 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; arm variant v5

```console
$ docker pull spiped@sha256:4c7d2251d333f8d0431820c3b578f7ae41917ca1093c5935c2388b147706ae15
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.9 MB (33946847 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f7aa0014abccf756d84170e4ca178cb8a05c991898f66e6fb02fe20b62f8d0df`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 06 Dec 2022 01:49:26 GMT
ADD file:3333e32449573e158be62ea6948788daec95a151f49035d65db8d7cb72b42c53 in / 
# Tue, 06 Dec 2022 01:49:27 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 08:43:55 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 06 Dec 2022 08:44:00 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 06 Dec 2022 08:44:00 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 06 Dec 2022 08:44:21 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 06 Dec 2022 08:44:21 GMT
VOLUME [/spiped]
# Tue, 06 Dec 2022 08:44:21 GMT
WORKDIR /spiped
# Tue, 06 Dec 2022 08:44:21 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 06 Dec 2022 08:44:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 06 Dec 2022 08:44:22 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:98c2ef299f89748b9c6075c728521ba8fe6e236fa46f50c465894cdb0ce69b35`  
		Last Modified: Tue, 06 Dec 2022 01:54:34 GMT  
		Size: 28.9 MB (28914353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc0ea1113a1be6fc2a9627ef082e720ff371fc45d6716fe7f722ca707538c7b1`  
		Last Modified: Tue, 06 Dec 2022 08:44:43 GMT  
		Size: 1.7 KB (1727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3887c862b2195ae4cc2a426d5f5da6cc1a1eb1aeb3a9cda029ab716e93d0a4c8`  
		Last Modified: Tue, 06 Dec 2022 08:44:43 GMT  
		Size: 1.0 KB (1023 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50d3fd5451d1949d361ab4448641dae3c1482c3b583f689519a217b67e38dc17`  
		Last Modified: Tue, 06 Dec 2022 08:44:44 GMT  
		Size: 5.0 MB (5029310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ecf2c8c904629c3af4f6d49c73ef023d6a3578840593d5c4b34d1fb74127e11`  
		Last Modified: Tue, 06 Dec 2022 08:44:43 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e19dee5dfc587991ed9321301a47c108d9e1bcd7bb2fc6f545c025b18ad05b2`  
		Last Modified: Tue, 06 Dec 2022 08:44:43 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; arm variant v7

```console
$ docker pull spiped@sha256:40b754b0ea2e65a750e0ca29e975bb772e33487bff62b443d2d3a52383d1f856
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.3 MB (31328552 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:665b2cb1f145cf0fe91e25c0b3bfc3f426e923bf58b844f0a566c36f00cbdd15`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 06 Dec 2022 00:58:51 GMT
ADD file:cb354f875d5631d5d4542ab57d0b9b323a261f5c631d5917127504d6eb54d85a in / 
# Tue, 06 Dec 2022 00:58:52 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 09:44:49 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 06 Dec 2022 09:44:52 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 06 Dec 2022 09:44:52 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 06 Dec 2022 09:45:11 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 06 Dec 2022 09:45:11 GMT
VOLUME [/spiped]
# Tue, 06 Dec 2022 09:45:11 GMT
WORKDIR /spiped
# Tue, 06 Dec 2022 09:45:12 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 06 Dec 2022 09:45:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 06 Dec 2022 09:45:12 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:4f32a98d14d26603bb8e8cf9bda992e24606d2fe00101767049a01d5176929e1`  
		Last Modified: Tue, 06 Dec 2022 01:06:05 GMT  
		Size: 26.6 MB (26576348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31137077cb0a083a399832c97ab11acd4066178e346b5813f3ad88e22a0565de`  
		Last Modified: Tue, 06 Dec 2022 09:45:49 GMT  
		Size: 1.7 KB (1729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b77617815911ed6c386761a2b71808839da34856eb521da23c158122c5dc681c`  
		Last Modified: Tue, 06 Dec 2022 09:45:49 GMT  
		Size: 1.0 KB (1021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:147b8da531098fead18d0722a7917658b99135017faf865e63f16660a7651b2c`  
		Last Modified: Tue, 06 Dec 2022 09:45:50 GMT  
		Size: 4.7 MB (4749020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49fc380b3e32f8df7a1f5caf7c53ade9e62badfc4b800cde9f8d6cac51d680ea`  
		Last Modified: Tue, 06 Dec 2022 09:45:48 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40dad1f3cce34a30fa25661aae54c80af7db819079b217cd779e7f27b025fada`  
		Last Modified: Tue, 06 Dec 2022 09:45:49 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:31d2c74a0140b5ff5c4ac410868ab4e933c8fd4074b898f4f90f2b7115d320d5
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.3 MB (35335991 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a9e5c42236284f6ec20094f338bf351249ecc7f86a22321f73b1d77ad606aaab`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 06 Dec 2022 01:40:17 GMT
ADD file:379d6ac56afdb6e02d71fa0faebc13b8a2554fc6ae76c5f5bbdb5b8e475135d6 in / 
# Tue, 06 Dec 2022 01:40:17 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 10:35:08 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 06 Dec 2022 10:35:11 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 06 Dec 2022 10:35:11 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 06 Dec 2022 10:35:25 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 06 Dec 2022 10:35:25 GMT
VOLUME [/spiped]
# Tue, 06 Dec 2022 10:35:25 GMT
WORKDIR /spiped
# Tue, 06 Dec 2022 10:35:25 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 06 Dec 2022 10:35:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 06 Dec 2022 10:35:25 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:6064e7e5b6afa4dc711228eddfd250aebac271830dc184c400ce640020bc2cb0`  
		Last Modified: Tue, 06 Dec 2022 01:43:56 GMT  
		Size: 30.1 MB (30060320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07ceaf30e109e8e4905e43890b83c26829fd61fa10f17e13462ee8790b4468b8`  
		Last Modified: Tue, 06 Dec 2022 10:35:41 GMT  
		Size: 1.7 KB (1734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfec2a36ae512de467eae80692b0847767fcc2b7aec528063f2b6d41bb85baa4`  
		Last Modified: Tue, 06 Dec 2022 10:35:41 GMT  
		Size: 1.1 KB (1052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1ad1673176eebc504a201540453eeaee3186931383a394a3e546a276d55ef41`  
		Last Modified: Tue, 06 Dec 2022 10:35:42 GMT  
		Size: 5.3 MB (5272419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3062f7c67c493a547b2454cf88fa51cab1cc38c8df1f504ecf30d28076ead221`  
		Last Modified: Tue, 06 Dec 2022 10:35:41 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e29a78cb947b3e22331e5dab5bbd5b0a972a02304c8d4a269d4f140e5a2b6ffb`  
		Last Modified: Tue, 06 Dec 2022 10:35:41 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; 386

```console
$ docker pull spiped@sha256:bc3034ea433bc46dd8c0b1f375517e13ebce3786f7ecbfffdb7edc99af6185f1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.3 MB (40286524 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fe71f396ab173d0e7a95d9be87cd921b46ab02f959c0cbf70a4d5b39250f548e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 15 Nov 2022 01:41:27 GMT
ADD file:608bec4ba3e2543714da4c5158f3c46a168f63ee69ac3f48bff54474ba9a6f27 in / 
# Tue, 15 Nov 2022 01:41:27 GMT
CMD ["bash"]
# Tue, 15 Nov 2022 17:51:33 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 15 Nov 2022 17:51:37 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 17:51:38 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 15 Nov 2022 17:51:59 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 15 Nov 2022 17:51:59 GMT
VOLUME [/spiped]
# Tue, 15 Nov 2022 17:52:00 GMT
WORKDIR /spiped
# Tue, 15 Nov 2022 17:52:02 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 15 Nov 2022 17:52:02 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 15 Nov 2022 17:52:03 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:f6a1e975b34444ecb7c6a2b537403fd6b94d2ff3225944ac2ac3b292466e4078`  
		Last Modified: Tue, 15 Nov 2022 01:47:05 GMT  
		Size: 32.4 MB (32392982 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43fbdc019d80d6a30ab90868896498a28c5e819659f22bb2894d5fc2e7d6bb3f`  
		Last Modified: Tue, 15 Nov 2022 17:52:32 GMT  
		Size: 1.6 KB (1614 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19d64fbdfcaf79efbaf8da0d679f65709cf4066699e35b9fbb0029f30317bbf9`  
		Last Modified: Tue, 15 Nov 2022 17:52:32 GMT  
		Size: 924.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1159f60b8a31090685214f0ae08d84535c724e5e92a2f79c4684a8af8435bdb`  
		Last Modified: Tue, 15 Nov 2022 17:52:34 GMT  
		Size: 7.9 MB (7890569 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd48a2b4bd1d2bd7ea1b36aea4ae7e36171af6be414a64513fdab695cf409fd0`  
		Last Modified: Tue, 15 Nov 2022 17:52:32 GMT  
		Size: 93.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0abba44a7b8700f9ac9dd0dba12b7983ecdc4c918ba4f8129e912828bd9b529`  
		Last Modified: Tue, 15 Nov 2022 17:52:32 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; mips64le

```console
$ docker pull spiped@sha256:aac80a4c64529fa60afc110d64d0c85b6a568df1b7cb5a5a9ca9d5ac966ca456
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.3 MB (35344851 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b04dad9d417652d7dc5fa4f1473c6a4076a1d44506ae13e748b502ed478db269`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 15 Nov 2022 04:13:42 GMT
ADD file:da7bed758c1e8c14583d53792170b6f4133a408ce2966e22ce52905f5c0d55a4 in / 
# Tue, 15 Nov 2022 04:13:46 GMT
CMD ["bash"]
# Wed, 16 Nov 2022 00:04:26 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 16 Nov 2022 00:04:40 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 16 Nov 2022 00:04:43 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 16 Nov 2022 00:06:07 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 16 Nov 2022 00:06:10 GMT
VOLUME [/spiped]
# Wed, 16 Nov 2022 00:06:13 GMT
WORKDIR /spiped
# Wed, 16 Nov 2022 00:06:15 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 16 Nov 2022 00:06:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 16 Nov 2022 00:06:20 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:27e2cdb4ebe2b6ee11014db328a4a8a055e3dcee2e275bf3aca6f03b39a09ad5`  
		Last Modified: Tue, 15 Nov 2022 04:21:14 GMT  
		Size: 29.6 MB (29635497 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3423cc689eb0f49221096b6d78f2f88cde0b37b5c1b49367ebff22a6e1ee33ba`  
		Last Modified: Wed, 16 Nov 2022 00:06:45 GMT  
		Size: 1.6 KB (1615 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff778c8a78825f7845b585d8dae3024757f98b009043b391253b9555d1bd3ee2`  
		Last Modified: Wed, 16 Nov 2022 00:06:45 GMT  
		Size: 925.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9787dc2ceb548759ff582e8606939f449df9a0dd7ce05dc5d1722c52cb9feb0c`  
		Last Modified: Wed, 16 Nov 2022 00:06:51 GMT  
		Size: 5.7 MB (5706376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1e18e00bc8e5f5bd8ded0d5c9a2d7e7ef1eddc72b6c9594971ecc6a5cd62c3d`  
		Last Modified: Wed, 16 Nov 2022 00:06:45 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c867e28a7d951478254c55c58be169d8812eaa99008aa6b11248a5c9046ae2f3`  
		Last Modified: Wed, 16 Nov 2022 00:06:45 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; ppc64le

```console
$ docker pull spiped@sha256:7dc6c63cf3a5c782ff8771d4fc8cdb70c66a6431370a50f4ed21e8de4e72c62e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.3 MB (41288342 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:adb1038b04ea2f70d259f739f5db46a604ebc27dce654270a95b8bb1bf072c43`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 06 Dec 2022 01:18:04 GMT
ADD file:2231a44ea52d93df58e23883ba6b6911d4c554f4c1d172d80fb21c751ddcbbfc in / 
# Tue, 06 Dec 2022 01:18:06 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 08:46:38 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 06 Dec 2022 08:46:44 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 06 Dec 2022 08:46:44 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 06 Dec 2022 08:47:23 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 06 Dec 2022 08:47:23 GMT
VOLUME [/spiped]
# Tue, 06 Dec 2022 08:47:24 GMT
WORKDIR /spiped
# Tue, 06 Dec 2022 08:47:24 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 06 Dec 2022 08:47:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 06 Dec 2022 08:47:25 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:1f72e1168976861c676bf86a6c149129baba7e13200e8b70e6f24dc2ac2797df`  
		Last Modified: Tue, 06 Dec 2022 01:24:18 GMT  
		Size: 35.3 MB (35285293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9bcd78f9b26ad833839cd08fb046f430437fd8d32e1bc5ecd748ede40c46f38`  
		Last Modified: Tue, 06 Dec 2022 08:48:00 GMT  
		Size: 1.7 KB (1732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20e30172f52bc26550dbd4c93f5279187368a3e481306d39c13b4b2028c85b48`  
		Last Modified: Tue, 06 Dec 2022 08:48:00 GMT  
		Size: 1.1 KB (1054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80a63688c8b5e78f3b418ecf36a67c6aa74de5018a1779b4fd3fd591630ad5b5`  
		Last Modified: Tue, 06 Dec 2022 08:48:02 GMT  
		Size: 6.0 MB (5999792 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6435887ede215333bcadcb79291fdc78590675fb277cfc74a82e59e86bdd7810`  
		Last Modified: Tue, 06 Dec 2022 08:48:00 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8711be9812e0b91d8c132be82304a099526684f5ef3ad39ff68e68e23206a2c6`  
		Last Modified: Tue, 06 Dec 2022 08:48:00 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; s390x

```console
$ docker pull spiped@sha256:dabf67b68c578220856eae3d1aa6e259e705dccdf5cdf67bf94231a7386985ef
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.8 MB (34835208 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:07220f39cb55897edd960624e94261bf233db44df4f80922a81668b1a269f18f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 06 Dec 2022 01:43:03 GMT
ADD file:f9243ad65309c3c458bf646b21aced55c055f7601340b3bda80ec30ff2f62159 in / 
# Tue, 06 Dec 2022 01:43:06 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 09:30:36 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 06 Dec 2022 09:30:40 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 06 Dec 2022 09:30:41 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 06 Dec 2022 09:31:14 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 06 Dec 2022 09:31:16 GMT
VOLUME [/spiped]
# Tue, 06 Dec 2022 09:31:17 GMT
WORKDIR /spiped
# Tue, 06 Dec 2022 09:31:17 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 06 Dec 2022 09:31:18 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 06 Dec 2022 09:31:19 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:66bc250ceea32b3e395aec7bb63aad4ac079791df67a2732692841e8dfacac94`  
		Last Modified: Tue, 06 Dec 2022 01:48:46 GMT  
		Size: 29.6 MB (29643886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:993125537188e3ea3515bbe7e54d76f4ffc24e5c5474ab91a4cff3b9f46e3fef`  
		Last Modified: Tue, 06 Dec 2022 09:32:00 GMT  
		Size: 1.7 KB (1735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c24621fa0a7df7b3d38b83959bca65e9c73c5fda9d37fa4f47d47a3d9689f73`  
		Last Modified: Tue, 06 Dec 2022 09:32:00 GMT  
		Size: 1.1 KB (1051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:156a325b8e0aad84615bca1bf738ec6e4b90c59878446cc5e3c396b38b9f294f`  
		Last Modified: Tue, 06 Dec 2022 09:32:01 GMT  
		Size: 5.2 MB (5188064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:412db3e471810a565457df0caac8b5a3316d99d9086b660612fea84953773282`  
		Last Modified: Tue, 06 Dec 2022 09:32:00 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66ea7d77964979ec04e96d7b369b49c2e0cbbf2004d37a40bbace3c7e21f1c9b`  
		Last Modified: Tue, 06 Dec 2022 09:32:00 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
