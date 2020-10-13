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
$ docker pull spiped@sha256:79df51f975875356a7b20bd3eeab8678f6d57e36bfd0f02566fd46e7c03e7b8b
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
$ docker pull spiped@sha256:cbcdcae2145e7f1c5b4c4e2ec9926e8f7cf2741c2edd41e74eb1a5ca85431c6a
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.3 MB (36260010 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ff3a3a8321db5126e2cfa970d9cabeafcbc493ae611c56ac1b7f3bc9c1877287`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 13 Oct 2020 01:39:05 GMT
ADD file:0dc53e7886c35bc21ae6c4f6cedda54d56ae9c9e9cd367678f1a72e68b3c43d4 in / 
# Tue, 13 Oct 2020 01:39:05 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 02:36:30 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 13 Oct 2020 02:36:35 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 13 Oct 2020 02:36:35 GMT
ENV SPIPED_VERSION=1.6.1
# Tue, 13 Oct 2020 02:36:36 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Tue, 13 Oct 2020 02:36:36 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Tue, 13 Oct 2020 02:37:05 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 13 Oct 2020 02:37:06 GMT
VOLUME [/spiped]
# Tue, 13 Oct 2020 02:37:06 GMT
WORKDIR /spiped
# Tue, 13 Oct 2020 02:37:06 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 13 Oct 2020 02:37:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 13 Oct 2020 02:37:07 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:bb79b6b2107fea8e8a47133a660b78e3a546998fcf0427be39ac9a0af4a97e90`  
		Last Modified: Tue, 13 Oct 2020 01:48:17 GMT  
		Size: 27.1 MB (27092228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e7e552308a9a7e56787eb8f2ee2cd0e5ae1bcd3e6e70767a3f1f63d04df1043`  
		Last Modified: Tue, 13 Oct 2020 02:37:24 GMT  
		Size: 1.7 KB (1738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fae3cfef5f840d90ca6a31c452db1ff437bc80f30c34bfe95e60a73d26faa39a`  
		Last Modified: Tue, 13 Oct 2020 02:37:25 GMT  
		Size: 2.1 MB (2128094 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3b92b058cf5a162f3e9e9c1b57e6ea521b98cfbdfe95c64e96543614c0aa889`  
		Last Modified: Tue, 13 Oct 2020 02:37:26 GMT  
		Size: 7.0 MB (7037515 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43e07e79b0faf86dec01bde507101fa39b284b027b0a16dcc2e0385b2711b7d7`  
		Last Modified: Tue, 13 Oct 2020 02:37:25 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2774b42f92e50846c6909f7c57a4559f4e39365596961f3cc60c181fd5ff02f7`  
		Last Modified: Tue, 13 Oct 2020 02:37:24 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; arm variant v5

```console
$ docker pull spiped@sha256:672edee7237da76ba6de9367e734a27d7f8f8562c11afcb03f3b145d6d260015
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.2 MB (32157300 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:17e88bd24524f59d6103fec000e35dde5b823055a634e55e935d247d8ac5444a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 13 Oct 2020 01:52:17 GMT
ADD file:b71c0fa4957d6b65af37231a105f3d17cdbafe5c7d6c37b5843ebf619c608aaa in / 
# Tue, 13 Oct 2020 01:52:27 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 03:19:47 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 13 Oct 2020 03:20:02 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 13 Oct 2020 03:20:03 GMT
ENV SPIPED_VERSION=1.6.1
# Tue, 13 Oct 2020 03:20:04 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Tue, 13 Oct 2020 03:20:05 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Tue, 13 Oct 2020 03:21:05 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 13 Oct 2020 03:21:10 GMT
VOLUME [/spiped]
# Tue, 13 Oct 2020 03:21:11 GMT
WORKDIR /spiped
# Tue, 13 Oct 2020 03:21:12 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 13 Oct 2020 03:21:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 13 Oct 2020 03:21:14 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:f991c1e1ee2c48f16625b6b61310bf3c0616c0dbda4762019117e86fd29cf9ce`  
		Last Modified: Tue, 13 Oct 2020 02:01:27 GMT  
		Size: 24.8 MB (24835992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bfc2a4609d9b5232a9e51a28b5db91ffc8c66f8660df9bcf2f5d1e3bceccec0`  
		Last Modified: Tue, 13 Oct 2020 03:21:36 GMT  
		Size: 1.7 KB (1737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:098bc9c2699c25d745dbdf0cb778c6194789b2d87ee75581c62527cc53f62a01`  
		Last Modified: Tue, 13 Oct 2020 03:21:37 GMT  
		Size: 1.8 MB (1839142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f23ff5b2f49dbf01bbcabfe3c39e09035f01987cdb3987c44dd29b8e562c9c79`  
		Last Modified: Tue, 13 Oct 2020 03:21:38 GMT  
		Size: 5.5 MB (5479959 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6783146d326266ff3b29ec06b968d70f4c9d910ed3b3d4b90a52adce04f6a4f2`  
		Last Modified: Tue, 13 Oct 2020 03:21:36 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e71a40b93164b5b86c29eae7931a993d7a6b035139e1d330fcaa7bb9f1663d30`  
		Last Modified: Tue, 13 Oct 2020 03:21:37 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; arm variant v7

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

### `spiped:1` - linux; arm64 variant v8

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

### `spiped:1` - linux; 386

```console
$ docker pull spiped@sha256:020927c2bce85e0a6153b9e3fba53483f1ca59bec55e71c09bfb448087264273
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.5 MB (41517895 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:faa5ea3e409fa66afb6ac2267b51c0db7a950a67d5efd32aa7094a082bd8ac57`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 13 Oct 2020 01:41:03 GMT
ADD file:51108b89c70ce0773c897be520c84454660f38b84ba556da49c7fe77e5d52416 in / 
# Tue, 13 Oct 2020 01:41:03 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 07:08:37 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 13 Oct 2020 07:08:42 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 13 Oct 2020 07:08:43 GMT
ENV SPIPED_VERSION=1.6.1
# Tue, 13 Oct 2020 07:08:43 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Tue, 13 Oct 2020 07:08:43 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Tue, 13 Oct 2020 07:09:13 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 13 Oct 2020 07:09:14 GMT
VOLUME [/spiped]
# Tue, 13 Oct 2020 07:09:14 GMT
WORKDIR /spiped
# Tue, 13 Oct 2020 07:09:14 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 13 Oct 2020 07:09:14 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 13 Oct 2020 07:09:15 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:97e4efec21eea92209464547d0f52a0f773c505cf4ea9d8090cef667bde145b8`  
		Last Modified: Tue, 13 Oct 2020 01:48:54 GMT  
		Size: 27.8 MB (27750243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:745fb22bef9b177604b68c486de51931377440e01812132d536beb88d70a5d21`  
		Last Modified: Tue, 13 Oct 2020 07:09:32 GMT  
		Size: 1.7 KB (1730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82d19eade6c6a313dc1c60e86222d6bafb19b6a105b28092bbd0cc98b4c0070f`  
		Last Modified: Tue, 13 Oct 2020 07:09:33 GMT  
		Size: 2.1 MB (2132324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:532cde1db9018cf5bdfd3b40054c0ad417b669d165c66aca9a994bc452d3c4fa`  
		Last Modified: Tue, 13 Oct 2020 07:09:36 GMT  
		Size: 11.6 MB (11633161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1dca20ce2d893f37dacd76615c6eacb8d643d74c3989b598ab4e4158b6bfc4e`  
		Last Modified: Tue, 13 Oct 2020 07:09:32 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:216b5ffd9d325d221945ae36ab00beed34a9aaea74f6118052db2fcba2c563ea`  
		Last Modified: Tue, 13 Oct 2020 07:09:32 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; mips64le

```console
$ docker pull spiped@sha256:bfe5c974767b865a68adb72cce4848ecaa36cab8992abfaff529176fc18ed961
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.9 MB (33893051 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0f86dfdfdd1df8f189c47811b193797f1bd21f709ec9849d5b71fb83d64fc0f8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 13 Oct 2020 01:09:50 GMT
ADD file:c2ad270f70511601478158cfe3854499c0b4887f049b78b66903412a811a428a in / 
# Tue, 13 Oct 2020 01:09:50 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 02:30:03 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 13 Oct 2020 02:30:16 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 13 Oct 2020 02:30:16 GMT
ENV SPIPED_VERSION=1.6.1
# Tue, 13 Oct 2020 02:30:16 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Tue, 13 Oct 2020 02:30:17 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Tue, 13 Oct 2020 02:31:24 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 13 Oct 2020 02:31:24 GMT
VOLUME [/spiped]
# Tue, 13 Oct 2020 02:31:24 GMT
WORKDIR /spiped
# Tue, 13 Oct 2020 02:31:25 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 13 Oct 2020 02:31:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 13 Oct 2020 02:31:26 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:9bc77d453b2242ec513032b61e23061712b79c3ba0c60114232d743e5ab4e4fa`  
		Last Modified: Tue, 13 Oct 2020 01:16:41 GMT  
		Size: 25.8 MB (25762577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5be50d34e573637b833f398c4bb03213fdc0e39948eb67673d4e6090fd69a86b`  
		Last Modified: Tue, 13 Oct 2020 02:31:50 GMT  
		Size: 1.7 KB (1740 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56986f62a854f267f51d23dcdfce8ed543e5c3f7ecaa67057a60aeba849366ae`  
		Last Modified: Tue, 13 Oct 2020 02:31:51 GMT  
		Size: 1.7 MB (1712061 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8827c190f0eb33937717d762d6cd11a35e2a49ba62d7af225998650be849266d`  
		Last Modified: Tue, 13 Oct 2020 02:31:56 GMT  
		Size: 6.4 MB (6416237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a38c49421fb63af5186fbe4e32552de9ad359f4d9611ca42956e2bce8ce49a98`  
		Last Modified: Tue, 13 Oct 2020 02:31:50 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74f89d8674f8700037b86df03ef1fd4e5e40b04138c1deb95601e7e1723050bb`  
		Last Modified: Tue, 13 Oct 2020 02:31:50 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; ppc64le

```console
$ docker pull spiped@sha256:11f9c1dbc68d2bcdd7a7f524027219a963ce523b201e71ae83c7052e635b27c1
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.5 MB (39488625 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cc337b8be5274e46ce4e2892582058be9fe426dc646660aa407e845573321c32`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 13 Oct 2020 01:38:54 GMT
ADD file:9992867f855c9bed54df6d26f3d8076689aff8a51e808fefba7d3b66dab250e5 in / 
# Tue, 13 Oct 2020 01:38:59 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 08:32:35 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 13 Oct 2020 08:33:10 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 13 Oct 2020 08:33:18 GMT
ENV SPIPED_VERSION=1.6.1
# Tue, 13 Oct 2020 08:33:25 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Tue, 13 Oct 2020 08:33:33 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Tue, 13 Oct 2020 08:40:10 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 13 Oct 2020 08:40:16 GMT
VOLUME [/spiped]
# Tue, 13 Oct 2020 08:40:29 GMT
WORKDIR /spiped
# Tue, 13 Oct 2020 08:40:33 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 13 Oct 2020 08:40:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 13 Oct 2020 08:40:44 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:523555c6877c72cfcdec912b4d0053c298b1c97835efc7c6b0211585a06bd563`  
		Last Modified: Tue, 13 Oct 2020 01:50:10 GMT  
		Size: 30.5 MB (30517878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e1d07b98a86b2674f96635104e41916c1e547434cb7d561cd85492408607281`  
		Last Modified: Tue, 13 Oct 2020 08:41:22 GMT  
		Size: 1.7 KB (1745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d2c21d3c72f09a47ee5eaa7be57ecda6468c5095c72c0ae090abfab50a53f17`  
		Last Modified: Tue, 13 Oct 2020 08:41:22 GMT  
		Size: 2.2 MB (2225018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b4a219f1f2d5be3ad0b26293fc2b817c1bb804bb21197d100b7dd072101f007`  
		Last Modified: Tue, 13 Oct 2020 08:41:22 GMT  
		Size: 6.7 MB (6743513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a3cacc68fbff4f9b9f07d0bb78c5b34216d92ff73ee186cbac165f8ee0cc552`  
		Last Modified: Tue, 13 Oct 2020 08:41:18 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:809a6e602fa91081254fd3482a446e8d14916d389cda086023515709324d584b`  
		Last Modified: Tue, 13 Oct 2020 08:41:18 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; s390x

```console
$ docker pull spiped@sha256:3feac6ba4263f960d8481dee734f70e1f4b0daea3436dcc444e6d37616e90f81
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.5 MB (33475004 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:239e569a133e1fb83824c9c12873d8c897d84bc87265b777b3b39e179c31d516`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 13 Oct 2020 01:42:26 GMT
ADD file:f932c1176fdc9bf45ced816290f83e6231df3dffa3b7f8de1a3bb0adcff1588b in / 
# Tue, 13 Oct 2020 01:42:27 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 06:29:14 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 13 Oct 2020 06:29:19 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 13 Oct 2020 06:29:20 GMT
ENV SPIPED_VERSION=1.6.1
# Tue, 13 Oct 2020 06:29:20 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Tue, 13 Oct 2020 06:29:20 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Tue, 13 Oct 2020 06:29:47 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 13 Oct 2020 06:29:48 GMT
VOLUME [/spiped]
# Tue, 13 Oct 2020 06:29:49 GMT
WORKDIR /spiped
# Tue, 13 Oct 2020 06:29:49 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 13 Oct 2020 06:29:49 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 13 Oct 2020 06:29:50 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:2a4f9dc00d797c86c4ffce3b50bea9037c2eb4637f045ad3fd68cf151577b639`  
		Last Modified: Tue, 13 Oct 2020 01:45:45 GMT  
		Size: 25.7 MB (25707519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8de0e34331f0b780854c48224e0de248e8951e70d8846ff0fe303e83d4425c38`  
		Last Modified: Tue, 13 Oct 2020 06:30:07 GMT  
		Size: 1.7 KB (1739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e4244b6ed8088d52ab38a21af88c52cfb32af480c91f3ebb8b84cdb807fe209`  
		Last Modified: Tue, 13 Oct 2020 06:30:07 GMT  
		Size: 1.8 MB (1821803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edbf619e3fe12a6407295c6f4a1cd8379ef1e9b588b41999d1fd99578395bf09`  
		Last Modified: Tue, 13 Oct 2020 06:30:08 GMT  
		Size: 5.9 MB (5943472 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4daaafe9626c1495df1df7db30d89e5f7a3e3e451f17cfe519a205fcd9e900c9`  
		Last Modified: Tue, 13 Oct 2020 06:30:07 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d3ebfbb7e7b045ea63889ea6b91bf081c0ba9ac7d0e7b7ca274a841059f6b31`  
		Last Modified: Tue, 13 Oct 2020 06:30:06 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:1.6`

```console
$ docker pull spiped@sha256:79df51f975875356a7b20bd3eeab8678f6d57e36bfd0f02566fd46e7c03e7b8b
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
$ docker pull spiped@sha256:cbcdcae2145e7f1c5b4c4e2ec9926e8f7cf2741c2edd41e74eb1a5ca85431c6a
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.3 MB (36260010 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ff3a3a8321db5126e2cfa970d9cabeafcbc493ae611c56ac1b7f3bc9c1877287`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 13 Oct 2020 01:39:05 GMT
ADD file:0dc53e7886c35bc21ae6c4f6cedda54d56ae9c9e9cd367678f1a72e68b3c43d4 in / 
# Tue, 13 Oct 2020 01:39:05 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 02:36:30 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 13 Oct 2020 02:36:35 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 13 Oct 2020 02:36:35 GMT
ENV SPIPED_VERSION=1.6.1
# Tue, 13 Oct 2020 02:36:36 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Tue, 13 Oct 2020 02:36:36 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Tue, 13 Oct 2020 02:37:05 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 13 Oct 2020 02:37:06 GMT
VOLUME [/spiped]
# Tue, 13 Oct 2020 02:37:06 GMT
WORKDIR /spiped
# Tue, 13 Oct 2020 02:37:06 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 13 Oct 2020 02:37:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 13 Oct 2020 02:37:07 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:bb79b6b2107fea8e8a47133a660b78e3a546998fcf0427be39ac9a0af4a97e90`  
		Last Modified: Tue, 13 Oct 2020 01:48:17 GMT  
		Size: 27.1 MB (27092228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e7e552308a9a7e56787eb8f2ee2cd0e5ae1bcd3e6e70767a3f1f63d04df1043`  
		Last Modified: Tue, 13 Oct 2020 02:37:24 GMT  
		Size: 1.7 KB (1738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fae3cfef5f840d90ca6a31c452db1ff437bc80f30c34bfe95e60a73d26faa39a`  
		Last Modified: Tue, 13 Oct 2020 02:37:25 GMT  
		Size: 2.1 MB (2128094 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3b92b058cf5a162f3e9e9c1b57e6ea521b98cfbdfe95c64e96543614c0aa889`  
		Last Modified: Tue, 13 Oct 2020 02:37:26 GMT  
		Size: 7.0 MB (7037515 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43e07e79b0faf86dec01bde507101fa39b284b027b0a16dcc2e0385b2711b7d7`  
		Last Modified: Tue, 13 Oct 2020 02:37:25 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2774b42f92e50846c6909f7c57a4559f4e39365596961f3cc60c181fd5ff02f7`  
		Last Modified: Tue, 13 Oct 2020 02:37:24 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; arm variant v5

```console
$ docker pull spiped@sha256:672edee7237da76ba6de9367e734a27d7f8f8562c11afcb03f3b145d6d260015
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.2 MB (32157300 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:17e88bd24524f59d6103fec000e35dde5b823055a634e55e935d247d8ac5444a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 13 Oct 2020 01:52:17 GMT
ADD file:b71c0fa4957d6b65af37231a105f3d17cdbafe5c7d6c37b5843ebf619c608aaa in / 
# Tue, 13 Oct 2020 01:52:27 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 03:19:47 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 13 Oct 2020 03:20:02 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 13 Oct 2020 03:20:03 GMT
ENV SPIPED_VERSION=1.6.1
# Tue, 13 Oct 2020 03:20:04 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Tue, 13 Oct 2020 03:20:05 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Tue, 13 Oct 2020 03:21:05 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 13 Oct 2020 03:21:10 GMT
VOLUME [/spiped]
# Tue, 13 Oct 2020 03:21:11 GMT
WORKDIR /spiped
# Tue, 13 Oct 2020 03:21:12 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 13 Oct 2020 03:21:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 13 Oct 2020 03:21:14 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:f991c1e1ee2c48f16625b6b61310bf3c0616c0dbda4762019117e86fd29cf9ce`  
		Last Modified: Tue, 13 Oct 2020 02:01:27 GMT  
		Size: 24.8 MB (24835992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bfc2a4609d9b5232a9e51a28b5db91ffc8c66f8660df9bcf2f5d1e3bceccec0`  
		Last Modified: Tue, 13 Oct 2020 03:21:36 GMT  
		Size: 1.7 KB (1737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:098bc9c2699c25d745dbdf0cb778c6194789b2d87ee75581c62527cc53f62a01`  
		Last Modified: Tue, 13 Oct 2020 03:21:37 GMT  
		Size: 1.8 MB (1839142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f23ff5b2f49dbf01bbcabfe3c39e09035f01987cdb3987c44dd29b8e562c9c79`  
		Last Modified: Tue, 13 Oct 2020 03:21:38 GMT  
		Size: 5.5 MB (5479959 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6783146d326266ff3b29ec06b968d70f4c9d910ed3b3d4b90a52adce04f6a4f2`  
		Last Modified: Tue, 13 Oct 2020 03:21:36 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e71a40b93164b5b86c29eae7931a993d7a6b035139e1d330fcaa7bb9f1663d30`  
		Last Modified: Tue, 13 Oct 2020 03:21:37 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; arm variant v7

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

### `spiped:1.6` - linux; arm64 variant v8

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

### `spiped:1.6` - linux; 386

```console
$ docker pull spiped@sha256:020927c2bce85e0a6153b9e3fba53483f1ca59bec55e71c09bfb448087264273
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.5 MB (41517895 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:faa5ea3e409fa66afb6ac2267b51c0db7a950a67d5efd32aa7094a082bd8ac57`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 13 Oct 2020 01:41:03 GMT
ADD file:51108b89c70ce0773c897be520c84454660f38b84ba556da49c7fe77e5d52416 in / 
# Tue, 13 Oct 2020 01:41:03 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 07:08:37 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 13 Oct 2020 07:08:42 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 13 Oct 2020 07:08:43 GMT
ENV SPIPED_VERSION=1.6.1
# Tue, 13 Oct 2020 07:08:43 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Tue, 13 Oct 2020 07:08:43 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Tue, 13 Oct 2020 07:09:13 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 13 Oct 2020 07:09:14 GMT
VOLUME [/spiped]
# Tue, 13 Oct 2020 07:09:14 GMT
WORKDIR /spiped
# Tue, 13 Oct 2020 07:09:14 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 13 Oct 2020 07:09:14 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 13 Oct 2020 07:09:15 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:97e4efec21eea92209464547d0f52a0f773c505cf4ea9d8090cef667bde145b8`  
		Last Modified: Tue, 13 Oct 2020 01:48:54 GMT  
		Size: 27.8 MB (27750243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:745fb22bef9b177604b68c486de51931377440e01812132d536beb88d70a5d21`  
		Last Modified: Tue, 13 Oct 2020 07:09:32 GMT  
		Size: 1.7 KB (1730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82d19eade6c6a313dc1c60e86222d6bafb19b6a105b28092bbd0cc98b4c0070f`  
		Last Modified: Tue, 13 Oct 2020 07:09:33 GMT  
		Size: 2.1 MB (2132324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:532cde1db9018cf5bdfd3b40054c0ad417b669d165c66aca9a994bc452d3c4fa`  
		Last Modified: Tue, 13 Oct 2020 07:09:36 GMT  
		Size: 11.6 MB (11633161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1dca20ce2d893f37dacd76615c6eacb8d643d74c3989b598ab4e4158b6bfc4e`  
		Last Modified: Tue, 13 Oct 2020 07:09:32 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:216b5ffd9d325d221945ae36ab00beed34a9aaea74f6118052db2fcba2c563ea`  
		Last Modified: Tue, 13 Oct 2020 07:09:32 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; mips64le

```console
$ docker pull spiped@sha256:bfe5c974767b865a68adb72cce4848ecaa36cab8992abfaff529176fc18ed961
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.9 MB (33893051 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0f86dfdfdd1df8f189c47811b193797f1bd21f709ec9849d5b71fb83d64fc0f8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 13 Oct 2020 01:09:50 GMT
ADD file:c2ad270f70511601478158cfe3854499c0b4887f049b78b66903412a811a428a in / 
# Tue, 13 Oct 2020 01:09:50 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 02:30:03 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 13 Oct 2020 02:30:16 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 13 Oct 2020 02:30:16 GMT
ENV SPIPED_VERSION=1.6.1
# Tue, 13 Oct 2020 02:30:16 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Tue, 13 Oct 2020 02:30:17 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Tue, 13 Oct 2020 02:31:24 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 13 Oct 2020 02:31:24 GMT
VOLUME [/spiped]
# Tue, 13 Oct 2020 02:31:24 GMT
WORKDIR /spiped
# Tue, 13 Oct 2020 02:31:25 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 13 Oct 2020 02:31:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 13 Oct 2020 02:31:26 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:9bc77d453b2242ec513032b61e23061712b79c3ba0c60114232d743e5ab4e4fa`  
		Last Modified: Tue, 13 Oct 2020 01:16:41 GMT  
		Size: 25.8 MB (25762577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5be50d34e573637b833f398c4bb03213fdc0e39948eb67673d4e6090fd69a86b`  
		Last Modified: Tue, 13 Oct 2020 02:31:50 GMT  
		Size: 1.7 KB (1740 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56986f62a854f267f51d23dcdfce8ed543e5c3f7ecaa67057a60aeba849366ae`  
		Last Modified: Tue, 13 Oct 2020 02:31:51 GMT  
		Size: 1.7 MB (1712061 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8827c190f0eb33937717d762d6cd11a35e2a49ba62d7af225998650be849266d`  
		Last Modified: Tue, 13 Oct 2020 02:31:56 GMT  
		Size: 6.4 MB (6416237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a38c49421fb63af5186fbe4e32552de9ad359f4d9611ca42956e2bce8ce49a98`  
		Last Modified: Tue, 13 Oct 2020 02:31:50 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74f89d8674f8700037b86df03ef1fd4e5e40b04138c1deb95601e7e1723050bb`  
		Last Modified: Tue, 13 Oct 2020 02:31:50 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; ppc64le

```console
$ docker pull spiped@sha256:11f9c1dbc68d2bcdd7a7f524027219a963ce523b201e71ae83c7052e635b27c1
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.5 MB (39488625 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cc337b8be5274e46ce4e2892582058be9fe426dc646660aa407e845573321c32`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 13 Oct 2020 01:38:54 GMT
ADD file:9992867f855c9bed54df6d26f3d8076689aff8a51e808fefba7d3b66dab250e5 in / 
# Tue, 13 Oct 2020 01:38:59 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 08:32:35 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 13 Oct 2020 08:33:10 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 13 Oct 2020 08:33:18 GMT
ENV SPIPED_VERSION=1.6.1
# Tue, 13 Oct 2020 08:33:25 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Tue, 13 Oct 2020 08:33:33 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Tue, 13 Oct 2020 08:40:10 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 13 Oct 2020 08:40:16 GMT
VOLUME [/spiped]
# Tue, 13 Oct 2020 08:40:29 GMT
WORKDIR /spiped
# Tue, 13 Oct 2020 08:40:33 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 13 Oct 2020 08:40:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 13 Oct 2020 08:40:44 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:523555c6877c72cfcdec912b4d0053c298b1c97835efc7c6b0211585a06bd563`  
		Last Modified: Tue, 13 Oct 2020 01:50:10 GMT  
		Size: 30.5 MB (30517878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e1d07b98a86b2674f96635104e41916c1e547434cb7d561cd85492408607281`  
		Last Modified: Tue, 13 Oct 2020 08:41:22 GMT  
		Size: 1.7 KB (1745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d2c21d3c72f09a47ee5eaa7be57ecda6468c5095c72c0ae090abfab50a53f17`  
		Last Modified: Tue, 13 Oct 2020 08:41:22 GMT  
		Size: 2.2 MB (2225018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b4a219f1f2d5be3ad0b26293fc2b817c1bb804bb21197d100b7dd072101f007`  
		Last Modified: Tue, 13 Oct 2020 08:41:22 GMT  
		Size: 6.7 MB (6743513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a3cacc68fbff4f9b9f07d0bb78c5b34216d92ff73ee186cbac165f8ee0cc552`  
		Last Modified: Tue, 13 Oct 2020 08:41:18 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:809a6e602fa91081254fd3482a446e8d14916d389cda086023515709324d584b`  
		Last Modified: Tue, 13 Oct 2020 08:41:18 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; s390x

```console
$ docker pull spiped@sha256:3feac6ba4263f960d8481dee734f70e1f4b0daea3436dcc444e6d37616e90f81
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.5 MB (33475004 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:239e569a133e1fb83824c9c12873d8c897d84bc87265b777b3b39e179c31d516`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 13 Oct 2020 01:42:26 GMT
ADD file:f932c1176fdc9bf45ced816290f83e6231df3dffa3b7f8de1a3bb0adcff1588b in / 
# Tue, 13 Oct 2020 01:42:27 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 06:29:14 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 13 Oct 2020 06:29:19 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 13 Oct 2020 06:29:20 GMT
ENV SPIPED_VERSION=1.6.1
# Tue, 13 Oct 2020 06:29:20 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Tue, 13 Oct 2020 06:29:20 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Tue, 13 Oct 2020 06:29:47 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 13 Oct 2020 06:29:48 GMT
VOLUME [/spiped]
# Tue, 13 Oct 2020 06:29:49 GMT
WORKDIR /spiped
# Tue, 13 Oct 2020 06:29:49 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 13 Oct 2020 06:29:49 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 13 Oct 2020 06:29:50 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:2a4f9dc00d797c86c4ffce3b50bea9037c2eb4637f045ad3fd68cf151577b639`  
		Last Modified: Tue, 13 Oct 2020 01:45:45 GMT  
		Size: 25.7 MB (25707519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8de0e34331f0b780854c48224e0de248e8951e70d8846ff0fe303e83d4425c38`  
		Last Modified: Tue, 13 Oct 2020 06:30:07 GMT  
		Size: 1.7 KB (1739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e4244b6ed8088d52ab38a21af88c52cfb32af480c91f3ebb8b84cdb807fe209`  
		Last Modified: Tue, 13 Oct 2020 06:30:07 GMT  
		Size: 1.8 MB (1821803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edbf619e3fe12a6407295c6f4a1cd8379ef1e9b588b41999d1fd99578395bf09`  
		Last Modified: Tue, 13 Oct 2020 06:30:08 GMT  
		Size: 5.9 MB (5943472 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4daaafe9626c1495df1df7db30d89e5f7a3e3e451f17cfe519a205fcd9e900c9`  
		Last Modified: Tue, 13 Oct 2020 06:30:07 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d3ebfbb7e7b045ea63889ea6b91bf081c0ba9ac7d0e7b7ca274a841059f6b31`  
		Last Modified: Tue, 13 Oct 2020 06:30:06 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:1.6.1`

```console
$ docker pull spiped@sha256:79df51f975875356a7b20bd3eeab8678f6d57e36bfd0f02566fd46e7c03e7b8b
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
$ docker pull spiped@sha256:cbcdcae2145e7f1c5b4c4e2ec9926e8f7cf2741c2edd41e74eb1a5ca85431c6a
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.3 MB (36260010 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ff3a3a8321db5126e2cfa970d9cabeafcbc493ae611c56ac1b7f3bc9c1877287`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 13 Oct 2020 01:39:05 GMT
ADD file:0dc53e7886c35bc21ae6c4f6cedda54d56ae9c9e9cd367678f1a72e68b3c43d4 in / 
# Tue, 13 Oct 2020 01:39:05 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 02:36:30 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 13 Oct 2020 02:36:35 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 13 Oct 2020 02:36:35 GMT
ENV SPIPED_VERSION=1.6.1
# Tue, 13 Oct 2020 02:36:36 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Tue, 13 Oct 2020 02:36:36 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Tue, 13 Oct 2020 02:37:05 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 13 Oct 2020 02:37:06 GMT
VOLUME [/spiped]
# Tue, 13 Oct 2020 02:37:06 GMT
WORKDIR /spiped
# Tue, 13 Oct 2020 02:37:06 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 13 Oct 2020 02:37:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 13 Oct 2020 02:37:07 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:bb79b6b2107fea8e8a47133a660b78e3a546998fcf0427be39ac9a0af4a97e90`  
		Last Modified: Tue, 13 Oct 2020 01:48:17 GMT  
		Size: 27.1 MB (27092228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e7e552308a9a7e56787eb8f2ee2cd0e5ae1bcd3e6e70767a3f1f63d04df1043`  
		Last Modified: Tue, 13 Oct 2020 02:37:24 GMT  
		Size: 1.7 KB (1738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fae3cfef5f840d90ca6a31c452db1ff437bc80f30c34bfe95e60a73d26faa39a`  
		Last Modified: Tue, 13 Oct 2020 02:37:25 GMT  
		Size: 2.1 MB (2128094 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3b92b058cf5a162f3e9e9c1b57e6ea521b98cfbdfe95c64e96543614c0aa889`  
		Last Modified: Tue, 13 Oct 2020 02:37:26 GMT  
		Size: 7.0 MB (7037515 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43e07e79b0faf86dec01bde507101fa39b284b027b0a16dcc2e0385b2711b7d7`  
		Last Modified: Tue, 13 Oct 2020 02:37:25 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2774b42f92e50846c6909f7c57a4559f4e39365596961f3cc60c181fd5ff02f7`  
		Last Modified: Tue, 13 Oct 2020 02:37:24 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1` - linux; arm variant v5

```console
$ docker pull spiped@sha256:672edee7237da76ba6de9367e734a27d7f8f8562c11afcb03f3b145d6d260015
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.2 MB (32157300 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:17e88bd24524f59d6103fec000e35dde5b823055a634e55e935d247d8ac5444a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 13 Oct 2020 01:52:17 GMT
ADD file:b71c0fa4957d6b65af37231a105f3d17cdbafe5c7d6c37b5843ebf619c608aaa in / 
# Tue, 13 Oct 2020 01:52:27 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 03:19:47 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 13 Oct 2020 03:20:02 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 13 Oct 2020 03:20:03 GMT
ENV SPIPED_VERSION=1.6.1
# Tue, 13 Oct 2020 03:20:04 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Tue, 13 Oct 2020 03:20:05 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Tue, 13 Oct 2020 03:21:05 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 13 Oct 2020 03:21:10 GMT
VOLUME [/spiped]
# Tue, 13 Oct 2020 03:21:11 GMT
WORKDIR /spiped
# Tue, 13 Oct 2020 03:21:12 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 13 Oct 2020 03:21:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 13 Oct 2020 03:21:14 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:f991c1e1ee2c48f16625b6b61310bf3c0616c0dbda4762019117e86fd29cf9ce`  
		Last Modified: Tue, 13 Oct 2020 02:01:27 GMT  
		Size: 24.8 MB (24835992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bfc2a4609d9b5232a9e51a28b5db91ffc8c66f8660df9bcf2f5d1e3bceccec0`  
		Last Modified: Tue, 13 Oct 2020 03:21:36 GMT  
		Size: 1.7 KB (1737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:098bc9c2699c25d745dbdf0cb778c6194789b2d87ee75581c62527cc53f62a01`  
		Last Modified: Tue, 13 Oct 2020 03:21:37 GMT  
		Size: 1.8 MB (1839142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f23ff5b2f49dbf01bbcabfe3c39e09035f01987cdb3987c44dd29b8e562c9c79`  
		Last Modified: Tue, 13 Oct 2020 03:21:38 GMT  
		Size: 5.5 MB (5479959 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6783146d326266ff3b29ec06b968d70f4c9d910ed3b3d4b90a52adce04f6a4f2`  
		Last Modified: Tue, 13 Oct 2020 03:21:36 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e71a40b93164b5b86c29eae7931a993d7a6b035139e1d330fcaa7bb9f1663d30`  
		Last Modified: Tue, 13 Oct 2020 03:21:37 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1` - linux; arm variant v7

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

### `spiped:1.6.1` - linux; arm64 variant v8

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

### `spiped:1.6.1` - linux; 386

```console
$ docker pull spiped@sha256:020927c2bce85e0a6153b9e3fba53483f1ca59bec55e71c09bfb448087264273
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.5 MB (41517895 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:faa5ea3e409fa66afb6ac2267b51c0db7a950a67d5efd32aa7094a082bd8ac57`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 13 Oct 2020 01:41:03 GMT
ADD file:51108b89c70ce0773c897be520c84454660f38b84ba556da49c7fe77e5d52416 in / 
# Tue, 13 Oct 2020 01:41:03 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 07:08:37 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 13 Oct 2020 07:08:42 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 13 Oct 2020 07:08:43 GMT
ENV SPIPED_VERSION=1.6.1
# Tue, 13 Oct 2020 07:08:43 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Tue, 13 Oct 2020 07:08:43 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Tue, 13 Oct 2020 07:09:13 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 13 Oct 2020 07:09:14 GMT
VOLUME [/spiped]
# Tue, 13 Oct 2020 07:09:14 GMT
WORKDIR /spiped
# Tue, 13 Oct 2020 07:09:14 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 13 Oct 2020 07:09:14 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 13 Oct 2020 07:09:15 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:97e4efec21eea92209464547d0f52a0f773c505cf4ea9d8090cef667bde145b8`  
		Last Modified: Tue, 13 Oct 2020 01:48:54 GMT  
		Size: 27.8 MB (27750243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:745fb22bef9b177604b68c486de51931377440e01812132d536beb88d70a5d21`  
		Last Modified: Tue, 13 Oct 2020 07:09:32 GMT  
		Size: 1.7 KB (1730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82d19eade6c6a313dc1c60e86222d6bafb19b6a105b28092bbd0cc98b4c0070f`  
		Last Modified: Tue, 13 Oct 2020 07:09:33 GMT  
		Size: 2.1 MB (2132324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:532cde1db9018cf5bdfd3b40054c0ad417b669d165c66aca9a994bc452d3c4fa`  
		Last Modified: Tue, 13 Oct 2020 07:09:36 GMT  
		Size: 11.6 MB (11633161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1dca20ce2d893f37dacd76615c6eacb8d643d74c3989b598ab4e4158b6bfc4e`  
		Last Modified: Tue, 13 Oct 2020 07:09:32 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:216b5ffd9d325d221945ae36ab00beed34a9aaea74f6118052db2fcba2c563ea`  
		Last Modified: Tue, 13 Oct 2020 07:09:32 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1` - linux; mips64le

```console
$ docker pull spiped@sha256:bfe5c974767b865a68adb72cce4848ecaa36cab8992abfaff529176fc18ed961
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.9 MB (33893051 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0f86dfdfdd1df8f189c47811b193797f1bd21f709ec9849d5b71fb83d64fc0f8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 13 Oct 2020 01:09:50 GMT
ADD file:c2ad270f70511601478158cfe3854499c0b4887f049b78b66903412a811a428a in / 
# Tue, 13 Oct 2020 01:09:50 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 02:30:03 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 13 Oct 2020 02:30:16 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 13 Oct 2020 02:30:16 GMT
ENV SPIPED_VERSION=1.6.1
# Tue, 13 Oct 2020 02:30:16 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Tue, 13 Oct 2020 02:30:17 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Tue, 13 Oct 2020 02:31:24 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 13 Oct 2020 02:31:24 GMT
VOLUME [/spiped]
# Tue, 13 Oct 2020 02:31:24 GMT
WORKDIR /spiped
# Tue, 13 Oct 2020 02:31:25 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 13 Oct 2020 02:31:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 13 Oct 2020 02:31:26 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:9bc77d453b2242ec513032b61e23061712b79c3ba0c60114232d743e5ab4e4fa`  
		Last Modified: Tue, 13 Oct 2020 01:16:41 GMT  
		Size: 25.8 MB (25762577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5be50d34e573637b833f398c4bb03213fdc0e39948eb67673d4e6090fd69a86b`  
		Last Modified: Tue, 13 Oct 2020 02:31:50 GMT  
		Size: 1.7 KB (1740 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56986f62a854f267f51d23dcdfce8ed543e5c3f7ecaa67057a60aeba849366ae`  
		Last Modified: Tue, 13 Oct 2020 02:31:51 GMT  
		Size: 1.7 MB (1712061 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8827c190f0eb33937717d762d6cd11a35e2a49ba62d7af225998650be849266d`  
		Last Modified: Tue, 13 Oct 2020 02:31:56 GMT  
		Size: 6.4 MB (6416237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a38c49421fb63af5186fbe4e32552de9ad359f4d9611ca42956e2bce8ce49a98`  
		Last Modified: Tue, 13 Oct 2020 02:31:50 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74f89d8674f8700037b86df03ef1fd4e5e40b04138c1deb95601e7e1723050bb`  
		Last Modified: Tue, 13 Oct 2020 02:31:50 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1` - linux; ppc64le

```console
$ docker pull spiped@sha256:11f9c1dbc68d2bcdd7a7f524027219a963ce523b201e71ae83c7052e635b27c1
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.5 MB (39488625 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cc337b8be5274e46ce4e2892582058be9fe426dc646660aa407e845573321c32`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 13 Oct 2020 01:38:54 GMT
ADD file:9992867f855c9bed54df6d26f3d8076689aff8a51e808fefba7d3b66dab250e5 in / 
# Tue, 13 Oct 2020 01:38:59 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 08:32:35 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 13 Oct 2020 08:33:10 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 13 Oct 2020 08:33:18 GMT
ENV SPIPED_VERSION=1.6.1
# Tue, 13 Oct 2020 08:33:25 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Tue, 13 Oct 2020 08:33:33 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Tue, 13 Oct 2020 08:40:10 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 13 Oct 2020 08:40:16 GMT
VOLUME [/spiped]
# Tue, 13 Oct 2020 08:40:29 GMT
WORKDIR /spiped
# Tue, 13 Oct 2020 08:40:33 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 13 Oct 2020 08:40:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 13 Oct 2020 08:40:44 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:523555c6877c72cfcdec912b4d0053c298b1c97835efc7c6b0211585a06bd563`  
		Last Modified: Tue, 13 Oct 2020 01:50:10 GMT  
		Size: 30.5 MB (30517878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e1d07b98a86b2674f96635104e41916c1e547434cb7d561cd85492408607281`  
		Last Modified: Tue, 13 Oct 2020 08:41:22 GMT  
		Size: 1.7 KB (1745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d2c21d3c72f09a47ee5eaa7be57ecda6468c5095c72c0ae090abfab50a53f17`  
		Last Modified: Tue, 13 Oct 2020 08:41:22 GMT  
		Size: 2.2 MB (2225018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b4a219f1f2d5be3ad0b26293fc2b817c1bb804bb21197d100b7dd072101f007`  
		Last Modified: Tue, 13 Oct 2020 08:41:22 GMT  
		Size: 6.7 MB (6743513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a3cacc68fbff4f9b9f07d0bb78c5b34216d92ff73ee186cbac165f8ee0cc552`  
		Last Modified: Tue, 13 Oct 2020 08:41:18 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:809a6e602fa91081254fd3482a446e8d14916d389cda086023515709324d584b`  
		Last Modified: Tue, 13 Oct 2020 08:41:18 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1` - linux; s390x

```console
$ docker pull spiped@sha256:3feac6ba4263f960d8481dee734f70e1f4b0daea3436dcc444e6d37616e90f81
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.5 MB (33475004 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:239e569a133e1fb83824c9c12873d8c897d84bc87265b777b3b39e179c31d516`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 13 Oct 2020 01:42:26 GMT
ADD file:f932c1176fdc9bf45ced816290f83e6231df3dffa3b7f8de1a3bb0adcff1588b in / 
# Tue, 13 Oct 2020 01:42:27 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 06:29:14 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 13 Oct 2020 06:29:19 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 13 Oct 2020 06:29:20 GMT
ENV SPIPED_VERSION=1.6.1
# Tue, 13 Oct 2020 06:29:20 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Tue, 13 Oct 2020 06:29:20 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Tue, 13 Oct 2020 06:29:47 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 13 Oct 2020 06:29:48 GMT
VOLUME [/spiped]
# Tue, 13 Oct 2020 06:29:49 GMT
WORKDIR /spiped
# Tue, 13 Oct 2020 06:29:49 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 13 Oct 2020 06:29:49 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 13 Oct 2020 06:29:50 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:2a4f9dc00d797c86c4ffce3b50bea9037c2eb4637f045ad3fd68cf151577b639`  
		Last Modified: Tue, 13 Oct 2020 01:45:45 GMT  
		Size: 25.7 MB (25707519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8de0e34331f0b780854c48224e0de248e8951e70d8846ff0fe303e83d4425c38`  
		Last Modified: Tue, 13 Oct 2020 06:30:07 GMT  
		Size: 1.7 KB (1739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e4244b6ed8088d52ab38a21af88c52cfb32af480c91f3ebb8b84cdb807fe209`  
		Last Modified: Tue, 13 Oct 2020 06:30:07 GMT  
		Size: 1.8 MB (1821803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edbf619e3fe12a6407295c6f4a1cd8379ef1e9b588b41999d1fd99578395bf09`  
		Last Modified: Tue, 13 Oct 2020 06:30:08 GMT  
		Size: 5.9 MB (5943472 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4daaafe9626c1495df1df7db30d89e5f7a3e3e451f17cfe519a205fcd9e900c9`  
		Last Modified: Tue, 13 Oct 2020 06:30:07 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d3ebfbb7e7b045ea63889ea6b91bf081c0ba9ac7d0e7b7ca274a841059f6b31`  
		Last Modified: Tue, 13 Oct 2020 06:30:06 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:1.6.1-alpine`

```console
$ docker pull spiped@sha256:1350110cc97a6b014a1bfb13ac574c0355b4b0adbd61223b04829a44448978a7
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
$ docker pull spiped@sha256:02675c9b94b81c42442961e3c3f8cee19e108ddd3a6b33f343adc2fe53b993c1
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.4 MB (3400367 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0a93ba8410da7de424982d8512bc0a2923d231ff8ada1683833045890d98b667`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 29 May 2020 21:19:46 GMT
ADD file:c92c248239f8c7b9b3c067650954815f391b7bcb09023f984972c082ace2a8d0 in / 
# Fri, 29 May 2020 21:19:46 GMT
CMD ["/bin/sh"]
# Mon, 03 Aug 2020 20:20:08 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Mon, 03 Aug 2020 20:20:09 GMT
RUN apk add --no-cache libssl1.1
# Mon, 03 Aug 2020 20:20:09 GMT
ENV SPIPED_VERSION=1.6.1
# Mon, 03 Aug 2020 20:20:09 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Mon, 03 Aug 2020 20:20:09 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Mon, 03 Aug 2020 20:20:25 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Mon, 03 Aug 2020 20:20:25 GMT
VOLUME [/spiped]
# Mon, 03 Aug 2020 20:20:26 GMT
WORKDIR /spiped
# Mon, 03 Aug 2020 20:20:26 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 03 Aug 2020 20:20:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 03 Aug 2020 20:20:26 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:df20fa9351a15782c64e6dddb2d4a6f50bf6d3688060a34c4014b0d9a752eb4c`  
		Last Modified: Fri, 29 May 2020 21:20:06 GMT  
		Size: 2.8 MB (2797541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0709a2fdbdb1ec0f8c6e66765ab3a151e1d5b34b886c8297a7031b92de0235b7`  
		Last Modified: Mon, 03 Aug 2020 20:20:37 GMT  
		Size: 1.2 KB (1233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c20256050734396b04f9988dad1e6df07d480c31a61ad023b92256947332287`  
		Last Modified: Mon, 03 Aug 2020 20:20:37 GMT  
		Size: 6.8 KB (6760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:226fbd39a157f769835312ebfabbc4eee4ddc298a97c5789859347ed820e67f0`  
		Last Modified: Mon, 03 Aug 2020 20:20:38 GMT  
		Size: 594.4 KB (594397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5dcd6aead3059d050069913b63bbad929137abd13d8c2187dd26f50cced1886`  
		Last Modified: Mon, 03 Aug 2020 20:20:37 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a24d7067723c20b97da438841dffd17f42f7b15b7376dd65e28358e8559f94f9`  
		Last Modified: Mon, 03 Aug 2020 20:20:37 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1-alpine` - linux; arm variant v6

```console
$ docker pull spiped@sha256:428f8af5290533d8d0486408946485d1ef27812cbd41efb050c7f4387e1a32e4
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.2 MB (3188866 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e66a19f7f66accfb73e0368a006b4e1f163d52335d6bdac248f0a4b90d3e5141`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 29 May 2020 21:50:55 GMT
ADD file:f46e997a56849423db17e5fc9f0249ab6c73b155245927dba5fcb9dfd65f622f in / 
# Fri, 29 May 2020 21:50:56 GMT
CMD ["/bin/sh"]
# Mon, 03 Aug 2020 19:50:37 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Mon, 03 Aug 2020 19:50:41 GMT
RUN apk add --no-cache libssl1.1
# Mon, 03 Aug 2020 19:50:42 GMT
ENV SPIPED_VERSION=1.6.1
# Mon, 03 Aug 2020 19:50:44 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Mon, 03 Aug 2020 19:50:44 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Mon, 03 Aug 2020 19:51:10 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Mon, 03 Aug 2020 19:51:11 GMT
VOLUME [/spiped]
# Mon, 03 Aug 2020 19:51:12 GMT
WORKDIR /spiped
# Mon, 03 Aug 2020 19:51:13 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 03 Aug 2020 19:51:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 03 Aug 2020 19:51:14 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:b4b72e716706d29f5d2351709c20bf737b94f876a5472a43ff1b6e203c65d27f`  
		Last Modified: Fri, 29 May 2020 21:51:30 GMT  
		Size: 2.6 MB (2603286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f06706dce439c2a25997202cc417d1774627055310639653a471802e1e18cedc`  
		Last Modified: Mon, 03 Aug 2020 19:51:29 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c306dde84d54b7dbf70384058b5aea64c8283806bfd63228147b3a9d61b68fe`  
		Last Modified: Mon, 03 Aug 2020 19:51:29 GMT  
		Size: 6.8 KB (6755 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9694005abebc012da97c33a53b778afbf6f7987c6ea39c984048b0c0f72c157f`  
		Last Modified: Mon, 03 Aug 2020 19:51:28 GMT  
		Size: 577.1 KB (577097 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d8220d0ea62d45c8735ee24114bfa496d9ae7da9d8e31e9f78f8bbfd9b4ad5a`  
		Last Modified: Mon, 03 Aug 2020 19:51:28 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85e1b721b9ec152691dfa04ad579c6d80c38e91ff54334dd14a53e8b97ee4f61`  
		Last Modified: Mon, 03 Aug 2020 19:51:28 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1-alpine` - linux; arm variant v7

```console
$ docker pull spiped@sha256:62721b07a25c4f0d9dd82e0b6bfb23adf8b83ea23013c65fd8dc878f8104824a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (2961408 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3aa8e983c241c8e1c7a70f352fd06b840613d94d7cbe725b3a3991691c76292c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 29 May 2020 21:02:07 GMT
ADD file:e97bf0d217846312b19a9f7264604851aedd125c23b4d291eed4c69b880dce26 in / 
# Fri, 29 May 2020 21:02:08 GMT
CMD ["/bin/sh"]
# Mon, 03 Aug 2020 19:58:42 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Mon, 03 Aug 2020 19:58:44 GMT
RUN apk add --no-cache libssl1.1
# Mon, 03 Aug 2020 19:58:45 GMT
ENV SPIPED_VERSION=1.6.1
# Mon, 03 Aug 2020 19:58:45 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Mon, 03 Aug 2020 19:58:46 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Mon, 03 Aug 2020 19:59:09 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Mon, 03 Aug 2020 19:59:10 GMT
VOLUME [/spiped]
# Mon, 03 Aug 2020 19:59:10 GMT
WORKDIR /spiped
# Mon, 03 Aug 2020 19:59:11 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 03 Aug 2020 19:59:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 03 Aug 2020 19:59:13 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:52278dd8e57993669c5b72a9620e89bebdc098f2af2379caaa8945f7403f77a2`  
		Last Modified: Fri, 29 May 2020 21:02:38 GMT  
		Size: 2.4 MB (2406763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96ebb7787066e1f6748cb01370284e61abdf9f769a185bb233de5269e70f4ff5`  
		Last Modified: Mon, 03 Aug 2020 19:59:28 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73e53e87064e4c4c848c3c5e5ccf508a596b96b15bd684fbace51390fba324c6`  
		Last Modified: Mon, 03 Aug 2020 19:59:28 GMT  
		Size: 6.8 KB (6751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c345b088bae12bc87048d3b0b67e872001d831aab0ff4feef6f43c775332188`  
		Last Modified: Mon, 03 Aug 2020 19:59:28 GMT  
		Size: 546.2 KB (546164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15b6a6679ac3b840cca72aee3291b5dea7e1a393a068c5df441f0f3c5954af4c`  
		Last Modified: Mon, 03 Aug 2020 19:59:28 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2b424a6439e7ac0d0af0e96b84399b46f36ec3ad2f19fc15fc0451a533fcc03`  
		Last Modified: Mon, 03 Aug 2020 19:59:28 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1-alpine` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:fecf4c0f91fd8da339bbf9a4a7a3f88705a826975ad0e7ea14ad7c08d7f744cd
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.3 MB (3310217 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:34101ceae6105bc2769fc3d77836cf2115c37767429dfebdcd8eec09a11284f9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 29 May 2020 21:43:19 GMT
ADD file:7574aee4e37a85460ab889212d52912723a9b30dda1c060548f0deb4a05fc398 in / 
# Fri, 29 May 2020 21:43:20 GMT
CMD ["/bin/sh"]
# Mon, 03 Aug 2020 19:40:20 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Mon, 03 Aug 2020 19:40:22 GMT
RUN apk add --no-cache libssl1.1
# Mon, 03 Aug 2020 19:40:22 GMT
ENV SPIPED_VERSION=1.6.1
# Mon, 03 Aug 2020 19:40:23 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Mon, 03 Aug 2020 19:40:23 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Mon, 03 Aug 2020 19:40:49 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Mon, 03 Aug 2020 19:40:49 GMT
VOLUME [/spiped]
# Mon, 03 Aug 2020 19:40:50 GMT
WORKDIR /spiped
# Mon, 03 Aug 2020 19:40:51 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 03 Aug 2020 19:40:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 03 Aug 2020 19:40:52 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:b538f80385f9b48122e3da068c932a96ea5018afa3c7be79da00437414bd18cd`  
		Last Modified: Fri, 29 May 2020 21:43:57 GMT  
		Size: 2.7 MB (2707964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:437a35bec8be5212ec28a179a42c49c1015ddd0ffa62c31242e962e4a2162b0a`  
		Last Modified: Mon, 03 Aug 2020 19:41:07 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c1314d231b23210ba600bd2763961e0bdd7aeb7b030c4522450b2a6a9e98c3a`  
		Last Modified: Mon, 03 Aug 2020 19:41:07 GMT  
		Size: 6.8 KB (6759 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bccf45ccb49331db2588902e283a2d1db4e7af8abd9e8487fa8cf0d4d25cffd8`  
		Last Modified: Mon, 03 Aug 2020 19:41:07 GMT  
		Size: 593.8 KB (593769 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75a74cfd6d8862147b08adcee3a5752adfc40b51af87a6a48ece418cc0ac6108`  
		Last Modified: Mon, 03 Aug 2020 19:41:06 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eff509bd366a6122dff1c828625fbe8ac8016c935041a30cf5a64d37c8fc434a`  
		Last Modified: Mon, 03 Aug 2020 19:41:07 GMT  
		Size: 338.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1-alpine` - linux; 386

```console
$ docker pull spiped@sha256:884fc0db36ace906a31efb70cf9740fda3e48e2e90a3b5f9453fc87d0f5291ad
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.4 MB (3394923 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0fbf9ab5830b6d380ce28dd35250ccef8e852b83e6c2debba73e82a6c1597b32`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 29 May 2020 21:38:33 GMT
ADD file:5624441d97aca5eeb82a582941efc3586397098b8391227a9040ebe434cc1d6b in / 
# Fri, 29 May 2020 21:38:33 GMT
CMD ["/bin/sh"]
# Mon, 03 Aug 2020 19:38:55 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Mon, 03 Aug 2020 19:38:56 GMT
RUN apk add --no-cache libssl1.1
# Mon, 03 Aug 2020 19:38:56 GMT
ENV SPIPED_VERSION=1.6.1
# Mon, 03 Aug 2020 19:38:56 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Mon, 03 Aug 2020 19:38:56 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Mon, 03 Aug 2020 19:39:14 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Mon, 03 Aug 2020 19:39:14 GMT
VOLUME [/spiped]
# Mon, 03 Aug 2020 19:39:14 GMT
WORKDIR /spiped
# Mon, 03 Aug 2020 19:39:15 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 03 Aug 2020 19:39:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 03 Aug 2020 19:39:15 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:0625b4155e2a59f647ece47c0cd77ed3196b1f84454fa64ce80cad90e2b9b79e`  
		Last Modified: Fri, 29 May 2020 21:38:53 GMT  
		Size: 2.8 MB (2792298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95b5d8b6933a806504d2858b32e5af5678af48f5b6e8d1449f6fb4dca90be1e9`  
		Last Modified: Mon, 03 Aug 2020 19:39:25 GMT  
		Size: 1.2 KB (1234 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08fa65eed96f55551abfa382372879649328469cc56d14a3bc9354094de4e6c6`  
		Last Modified: Mon, 03 Aug 2020 19:39:24 GMT  
		Size: 6.8 KB (6759 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0f2ab34b6a857c23f06895f0982c1aa304833b4350c483874340ac52ecae085`  
		Last Modified: Mon, 03 Aug 2020 19:39:24 GMT  
		Size: 594.2 KB (594197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca95090aba0b0eb00cdf63a03fda87aab71f510516e4619686900b1e94d0f2d1`  
		Last Modified: Mon, 03 Aug 2020 19:39:25 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a719dbef3762817781395041d1ed9371606bf1ca853ca83a51b8527f6f88a9e`  
		Last Modified: Mon, 03 Aug 2020 19:39:24 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1-alpine` - linux; ppc64le

```console
$ docker pull spiped@sha256:be28a8b592ef19aba9d3d720f74cc34cd2b890ce513a9681b84cedb81aa81d3c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.4 MB (3420796 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:326f45418e4eec122cd9ce53ec66be01c39b21ffb7550260808143f05db37ee9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 29 May 2020 21:23:03 GMT
ADD file:8194808a812370fd2202d80d1667f851bd9eac4c560d69d347fe1964f54343de in / 
# Fri, 29 May 2020 21:23:06 GMT
CMD ["/bin/sh"]
# Mon, 03 Aug 2020 20:17:58 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Mon, 03 Aug 2020 20:18:07 GMT
RUN apk add --no-cache libssl1.1
# Mon, 03 Aug 2020 20:18:14 GMT
ENV SPIPED_VERSION=1.6.1
# Mon, 03 Aug 2020 20:18:17 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Mon, 03 Aug 2020 20:18:21 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Mon, 03 Aug 2020 20:18:54 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Mon, 03 Aug 2020 20:18:59 GMT
VOLUME [/spiped]
# Mon, 03 Aug 2020 20:19:05 GMT
WORKDIR /spiped
# Mon, 03 Aug 2020 20:19:08 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 03 Aug 2020 20:19:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 03 Aug 2020 20:19:19 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:5077f8601dceb5744d875d7740ebc203f674b108a0188f3a31e292b21a4bee64`  
		Last Modified: Fri, 29 May 2020 21:23:37 GMT  
		Size: 2.8 MB (2805199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab223d5e8b6fad2e0a685c6d01913edb1021ad4f98cf6f280c84a587585b4be3`  
		Last Modified: Mon, 03 Aug 2020 20:19:40 GMT  
		Size: 1.3 KB (1262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c5463b129a00b3d487dc47b34bd226c4fcd815b44b9d4ec783ebbae814db9be`  
		Last Modified: Mon, 03 Aug 2020 20:19:40 GMT  
		Size: 6.8 KB (6760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb8a2aaec72079901e78cdcda1d214a6408e04fd111b01bbf4865e4731befef6`  
		Last Modified: Mon, 03 Aug 2020 20:19:41 GMT  
		Size: 607.1 KB (607103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5128ec33b43788f96f1f9d53e9b0e3a9b073f51bb7ef4bec5639b8367d9f0d5f`  
		Last Modified: Mon, 03 Aug 2020 20:19:40 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21cc02ad1ba276590592ea772c67711daefffc109f32e4a9114e67cd81c8f39d`  
		Last Modified: Mon, 03 Aug 2020 20:19:40 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1-alpine` - linux; s390x

```console
$ docker pull spiped@sha256:b73ea63f68d61aabf2d30f81eb4cf11388380f6b7779980550e039b24e8daf02
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.2 MB (3169341 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dedd11800ad772a1acff1311f9f24324d234762e6ba34aa4dc6f62bde7b8c720`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 29 May 2020 21:41:39 GMT
ADD file:9799ce3b2f782a28e10b1846cd9b3db827fa99c9bc601feb268456195856814e in / 
# Fri, 29 May 2020 21:41:39 GMT
CMD ["/bin/sh"]
# Mon, 03 Aug 2020 19:41:51 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Mon, 03 Aug 2020 19:41:52 GMT
RUN apk add --no-cache libssl1.1
# Mon, 03 Aug 2020 19:41:53 GMT
ENV SPIPED_VERSION=1.6.1
# Mon, 03 Aug 2020 19:41:53 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Mon, 03 Aug 2020 19:41:54 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Mon, 03 Aug 2020 19:42:04 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Mon, 03 Aug 2020 19:42:04 GMT
VOLUME [/spiped]
# Mon, 03 Aug 2020 19:42:04 GMT
WORKDIR /spiped
# Mon, 03 Aug 2020 19:42:05 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 03 Aug 2020 19:42:05 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 03 Aug 2020 19:42:05 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:8fb3d41b2e9a59630b51745f257cd2561f96bcd15cf309fcc20120d5fcee8c5b`  
		Last Modified: Fri, 29 May 2020 21:42:03 GMT  
		Size: 2.6 MB (2566189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88144f4b1d0ccb9e43e39ac154de5f74f7ad616622b69c604d959bbff10c05ae`  
		Last Modified: Mon, 03 Aug 2020 19:42:18 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4673652cef72557f23239dfa02e8752d0cb5336ab795da58e3f9e76156f6ea1c`  
		Last Modified: Mon, 03 Aug 2020 19:42:18 GMT  
		Size: 6.8 KB (6761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:104d19d98d1e4b1e750f13f131573f9a9757b8848b5f563485da6a594c80218f`  
		Last Modified: Mon, 03 Aug 2020 19:42:18 GMT  
		Size: 594.7 KB (594659 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b42dd365d6b02d300d2aec26f7518bcf990fa814282da55eafce7068a4b363b0`  
		Last Modified: Mon, 03 Aug 2020 19:42:18 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f59fcf025999094f1e53abf0e4be8d7087db6c325c10b049ea824f776365a917`  
		Last Modified: Mon, 03 Aug 2020 19:42:18 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:1.6-alpine`

```console
$ docker pull spiped@sha256:1350110cc97a6b014a1bfb13ac574c0355b4b0adbd61223b04829a44448978a7
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
$ docker pull spiped@sha256:02675c9b94b81c42442961e3c3f8cee19e108ddd3a6b33f343adc2fe53b993c1
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.4 MB (3400367 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0a93ba8410da7de424982d8512bc0a2923d231ff8ada1683833045890d98b667`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 29 May 2020 21:19:46 GMT
ADD file:c92c248239f8c7b9b3c067650954815f391b7bcb09023f984972c082ace2a8d0 in / 
# Fri, 29 May 2020 21:19:46 GMT
CMD ["/bin/sh"]
# Mon, 03 Aug 2020 20:20:08 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Mon, 03 Aug 2020 20:20:09 GMT
RUN apk add --no-cache libssl1.1
# Mon, 03 Aug 2020 20:20:09 GMT
ENV SPIPED_VERSION=1.6.1
# Mon, 03 Aug 2020 20:20:09 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Mon, 03 Aug 2020 20:20:09 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Mon, 03 Aug 2020 20:20:25 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Mon, 03 Aug 2020 20:20:25 GMT
VOLUME [/spiped]
# Mon, 03 Aug 2020 20:20:26 GMT
WORKDIR /spiped
# Mon, 03 Aug 2020 20:20:26 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 03 Aug 2020 20:20:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 03 Aug 2020 20:20:26 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:df20fa9351a15782c64e6dddb2d4a6f50bf6d3688060a34c4014b0d9a752eb4c`  
		Last Modified: Fri, 29 May 2020 21:20:06 GMT  
		Size: 2.8 MB (2797541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0709a2fdbdb1ec0f8c6e66765ab3a151e1d5b34b886c8297a7031b92de0235b7`  
		Last Modified: Mon, 03 Aug 2020 20:20:37 GMT  
		Size: 1.2 KB (1233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c20256050734396b04f9988dad1e6df07d480c31a61ad023b92256947332287`  
		Last Modified: Mon, 03 Aug 2020 20:20:37 GMT  
		Size: 6.8 KB (6760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:226fbd39a157f769835312ebfabbc4eee4ddc298a97c5789859347ed820e67f0`  
		Last Modified: Mon, 03 Aug 2020 20:20:38 GMT  
		Size: 594.4 KB (594397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5dcd6aead3059d050069913b63bbad929137abd13d8c2187dd26f50cced1886`  
		Last Modified: Mon, 03 Aug 2020 20:20:37 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a24d7067723c20b97da438841dffd17f42f7b15b7376dd65e28358e8559f94f9`  
		Last Modified: Mon, 03 Aug 2020 20:20:37 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; arm variant v6

```console
$ docker pull spiped@sha256:428f8af5290533d8d0486408946485d1ef27812cbd41efb050c7f4387e1a32e4
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.2 MB (3188866 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e66a19f7f66accfb73e0368a006b4e1f163d52335d6bdac248f0a4b90d3e5141`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 29 May 2020 21:50:55 GMT
ADD file:f46e997a56849423db17e5fc9f0249ab6c73b155245927dba5fcb9dfd65f622f in / 
# Fri, 29 May 2020 21:50:56 GMT
CMD ["/bin/sh"]
# Mon, 03 Aug 2020 19:50:37 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Mon, 03 Aug 2020 19:50:41 GMT
RUN apk add --no-cache libssl1.1
# Mon, 03 Aug 2020 19:50:42 GMT
ENV SPIPED_VERSION=1.6.1
# Mon, 03 Aug 2020 19:50:44 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Mon, 03 Aug 2020 19:50:44 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Mon, 03 Aug 2020 19:51:10 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Mon, 03 Aug 2020 19:51:11 GMT
VOLUME [/spiped]
# Mon, 03 Aug 2020 19:51:12 GMT
WORKDIR /spiped
# Mon, 03 Aug 2020 19:51:13 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 03 Aug 2020 19:51:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 03 Aug 2020 19:51:14 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:b4b72e716706d29f5d2351709c20bf737b94f876a5472a43ff1b6e203c65d27f`  
		Last Modified: Fri, 29 May 2020 21:51:30 GMT  
		Size: 2.6 MB (2603286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f06706dce439c2a25997202cc417d1774627055310639653a471802e1e18cedc`  
		Last Modified: Mon, 03 Aug 2020 19:51:29 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c306dde84d54b7dbf70384058b5aea64c8283806bfd63228147b3a9d61b68fe`  
		Last Modified: Mon, 03 Aug 2020 19:51:29 GMT  
		Size: 6.8 KB (6755 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9694005abebc012da97c33a53b778afbf6f7987c6ea39c984048b0c0f72c157f`  
		Last Modified: Mon, 03 Aug 2020 19:51:28 GMT  
		Size: 577.1 KB (577097 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d8220d0ea62d45c8735ee24114bfa496d9ae7da9d8e31e9f78f8bbfd9b4ad5a`  
		Last Modified: Mon, 03 Aug 2020 19:51:28 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85e1b721b9ec152691dfa04ad579c6d80c38e91ff54334dd14a53e8b97ee4f61`  
		Last Modified: Mon, 03 Aug 2020 19:51:28 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; arm variant v7

```console
$ docker pull spiped@sha256:62721b07a25c4f0d9dd82e0b6bfb23adf8b83ea23013c65fd8dc878f8104824a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (2961408 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3aa8e983c241c8e1c7a70f352fd06b840613d94d7cbe725b3a3991691c76292c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 29 May 2020 21:02:07 GMT
ADD file:e97bf0d217846312b19a9f7264604851aedd125c23b4d291eed4c69b880dce26 in / 
# Fri, 29 May 2020 21:02:08 GMT
CMD ["/bin/sh"]
# Mon, 03 Aug 2020 19:58:42 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Mon, 03 Aug 2020 19:58:44 GMT
RUN apk add --no-cache libssl1.1
# Mon, 03 Aug 2020 19:58:45 GMT
ENV SPIPED_VERSION=1.6.1
# Mon, 03 Aug 2020 19:58:45 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Mon, 03 Aug 2020 19:58:46 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Mon, 03 Aug 2020 19:59:09 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Mon, 03 Aug 2020 19:59:10 GMT
VOLUME [/spiped]
# Mon, 03 Aug 2020 19:59:10 GMT
WORKDIR /spiped
# Mon, 03 Aug 2020 19:59:11 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 03 Aug 2020 19:59:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 03 Aug 2020 19:59:13 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:52278dd8e57993669c5b72a9620e89bebdc098f2af2379caaa8945f7403f77a2`  
		Last Modified: Fri, 29 May 2020 21:02:38 GMT  
		Size: 2.4 MB (2406763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96ebb7787066e1f6748cb01370284e61abdf9f769a185bb233de5269e70f4ff5`  
		Last Modified: Mon, 03 Aug 2020 19:59:28 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73e53e87064e4c4c848c3c5e5ccf508a596b96b15bd684fbace51390fba324c6`  
		Last Modified: Mon, 03 Aug 2020 19:59:28 GMT  
		Size: 6.8 KB (6751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c345b088bae12bc87048d3b0b67e872001d831aab0ff4feef6f43c775332188`  
		Last Modified: Mon, 03 Aug 2020 19:59:28 GMT  
		Size: 546.2 KB (546164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15b6a6679ac3b840cca72aee3291b5dea7e1a393a068c5df441f0f3c5954af4c`  
		Last Modified: Mon, 03 Aug 2020 19:59:28 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2b424a6439e7ac0d0af0e96b84399b46f36ec3ad2f19fc15fc0451a533fcc03`  
		Last Modified: Mon, 03 Aug 2020 19:59:28 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:fecf4c0f91fd8da339bbf9a4a7a3f88705a826975ad0e7ea14ad7c08d7f744cd
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.3 MB (3310217 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:34101ceae6105bc2769fc3d77836cf2115c37767429dfebdcd8eec09a11284f9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 29 May 2020 21:43:19 GMT
ADD file:7574aee4e37a85460ab889212d52912723a9b30dda1c060548f0deb4a05fc398 in / 
# Fri, 29 May 2020 21:43:20 GMT
CMD ["/bin/sh"]
# Mon, 03 Aug 2020 19:40:20 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Mon, 03 Aug 2020 19:40:22 GMT
RUN apk add --no-cache libssl1.1
# Mon, 03 Aug 2020 19:40:22 GMT
ENV SPIPED_VERSION=1.6.1
# Mon, 03 Aug 2020 19:40:23 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Mon, 03 Aug 2020 19:40:23 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Mon, 03 Aug 2020 19:40:49 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Mon, 03 Aug 2020 19:40:49 GMT
VOLUME [/spiped]
# Mon, 03 Aug 2020 19:40:50 GMT
WORKDIR /spiped
# Mon, 03 Aug 2020 19:40:51 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 03 Aug 2020 19:40:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 03 Aug 2020 19:40:52 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:b538f80385f9b48122e3da068c932a96ea5018afa3c7be79da00437414bd18cd`  
		Last Modified: Fri, 29 May 2020 21:43:57 GMT  
		Size: 2.7 MB (2707964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:437a35bec8be5212ec28a179a42c49c1015ddd0ffa62c31242e962e4a2162b0a`  
		Last Modified: Mon, 03 Aug 2020 19:41:07 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c1314d231b23210ba600bd2763961e0bdd7aeb7b030c4522450b2a6a9e98c3a`  
		Last Modified: Mon, 03 Aug 2020 19:41:07 GMT  
		Size: 6.8 KB (6759 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bccf45ccb49331db2588902e283a2d1db4e7af8abd9e8487fa8cf0d4d25cffd8`  
		Last Modified: Mon, 03 Aug 2020 19:41:07 GMT  
		Size: 593.8 KB (593769 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75a74cfd6d8862147b08adcee3a5752adfc40b51af87a6a48ece418cc0ac6108`  
		Last Modified: Mon, 03 Aug 2020 19:41:06 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eff509bd366a6122dff1c828625fbe8ac8016c935041a30cf5a64d37c8fc434a`  
		Last Modified: Mon, 03 Aug 2020 19:41:07 GMT  
		Size: 338.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; 386

```console
$ docker pull spiped@sha256:884fc0db36ace906a31efb70cf9740fda3e48e2e90a3b5f9453fc87d0f5291ad
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.4 MB (3394923 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0fbf9ab5830b6d380ce28dd35250ccef8e852b83e6c2debba73e82a6c1597b32`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 29 May 2020 21:38:33 GMT
ADD file:5624441d97aca5eeb82a582941efc3586397098b8391227a9040ebe434cc1d6b in / 
# Fri, 29 May 2020 21:38:33 GMT
CMD ["/bin/sh"]
# Mon, 03 Aug 2020 19:38:55 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Mon, 03 Aug 2020 19:38:56 GMT
RUN apk add --no-cache libssl1.1
# Mon, 03 Aug 2020 19:38:56 GMT
ENV SPIPED_VERSION=1.6.1
# Mon, 03 Aug 2020 19:38:56 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Mon, 03 Aug 2020 19:38:56 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Mon, 03 Aug 2020 19:39:14 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Mon, 03 Aug 2020 19:39:14 GMT
VOLUME [/spiped]
# Mon, 03 Aug 2020 19:39:14 GMT
WORKDIR /spiped
# Mon, 03 Aug 2020 19:39:15 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 03 Aug 2020 19:39:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 03 Aug 2020 19:39:15 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:0625b4155e2a59f647ece47c0cd77ed3196b1f84454fa64ce80cad90e2b9b79e`  
		Last Modified: Fri, 29 May 2020 21:38:53 GMT  
		Size: 2.8 MB (2792298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95b5d8b6933a806504d2858b32e5af5678af48f5b6e8d1449f6fb4dca90be1e9`  
		Last Modified: Mon, 03 Aug 2020 19:39:25 GMT  
		Size: 1.2 KB (1234 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08fa65eed96f55551abfa382372879649328469cc56d14a3bc9354094de4e6c6`  
		Last Modified: Mon, 03 Aug 2020 19:39:24 GMT  
		Size: 6.8 KB (6759 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0f2ab34b6a857c23f06895f0982c1aa304833b4350c483874340ac52ecae085`  
		Last Modified: Mon, 03 Aug 2020 19:39:24 GMT  
		Size: 594.2 KB (594197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca95090aba0b0eb00cdf63a03fda87aab71f510516e4619686900b1e94d0f2d1`  
		Last Modified: Mon, 03 Aug 2020 19:39:25 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a719dbef3762817781395041d1ed9371606bf1ca853ca83a51b8527f6f88a9e`  
		Last Modified: Mon, 03 Aug 2020 19:39:24 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; ppc64le

```console
$ docker pull spiped@sha256:be28a8b592ef19aba9d3d720f74cc34cd2b890ce513a9681b84cedb81aa81d3c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.4 MB (3420796 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:326f45418e4eec122cd9ce53ec66be01c39b21ffb7550260808143f05db37ee9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 29 May 2020 21:23:03 GMT
ADD file:8194808a812370fd2202d80d1667f851bd9eac4c560d69d347fe1964f54343de in / 
# Fri, 29 May 2020 21:23:06 GMT
CMD ["/bin/sh"]
# Mon, 03 Aug 2020 20:17:58 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Mon, 03 Aug 2020 20:18:07 GMT
RUN apk add --no-cache libssl1.1
# Mon, 03 Aug 2020 20:18:14 GMT
ENV SPIPED_VERSION=1.6.1
# Mon, 03 Aug 2020 20:18:17 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Mon, 03 Aug 2020 20:18:21 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Mon, 03 Aug 2020 20:18:54 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Mon, 03 Aug 2020 20:18:59 GMT
VOLUME [/spiped]
# Mon, 03 Aug 2020 20:19:05 GMT
WORKDIR /spiped
# Mon, 03 Aug 2020 20:19:08 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 03 Aug 2020 20:19:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 03 Aug 2020 20:19:19 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:5077f8601dceb5744d875d7740ebc203f674b108a0188f3a31e292b21a4bee64`  
		Last Modified: Fri, 29 May 2020 21:23:37 GMT  
		Size: 2.8 MB (2805199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab223d5e8b6fad2e0a685c6d01913edb1021ad4f98cf6f280c84a587585b4be3`  
		Last Modified: Mon, 03 Aug 2020 20:19:40 GMT  
		Size: 1.3 KB (1262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c5463b129a00b3d487dc47b34bd226c4fcd815b44b9d4ec783ebbae814db9be`  
		Last Modified: Mon, 03 Aug 2020 20:19:40 GMT  
		Size: 6.8 KB (6760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb8a2aaec72079901e78cdcda1d214a6408e04fd111b01bbf4865e4731befef6`  
		Last Modified: Mon, 03 Aug 2020 20:19:41 GMT  
		Size: 607.1 KB (607103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5128ec33b43788f96f1f9d53e9b0e3a9b073f51bb7ef4bec5639b8367d9f0d5f`  
		Last Modified: Mon, 03 Aug 2020 20:19:40 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21cc02ad1ba276590592ea772c67711daefffc109f32e4a9114e67cd81c8f39d`  
		Last Modified: Mon, 03 Aug 2020 20:19:40 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; s390x

```console
$ docker pull spiped@sha256:b73ea63f68d61aabf2d30f81eb4cf11388380f6b7779980550e039b24e8daf02
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.2 MB (3169341 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dedd11800ad772a1acff1311f9f24324d234762e6ba34aa4dc6f62bde7b8c720`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 29 May 2020 21:41:39 GMT
ADD file:9799ce3b2f782a28e10b1846cd9b3db827fa99c9bc601feb268456195856814e in / 
# Fri, 29 May 2020 21:41:39 GMT
CMD ["/bin/sh"]
# Mon, 03 Aug 2020 19:41:51 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Mon, 03 Aug 2020 19:41:52 GMT
RUN apk add --no-cache libssl1.1
# Mon, 03 Aug 2020 19:41:53 GMT
ENV SPIPED_VERSION=1.6.1
# Mon, 03 Aug 2020 19:41:53 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Mon, 03 Aug 2020 19:41:54 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Mon, 03 Aug 2020 19:42:04 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Mon, 03 Aug 2020 19:42:04 GMT
VOLUME [/spiped]
# Mon, 03 Aug 2020 19:42:04 GMT
WORKDIR /spiped
# Mon, 03 Aug 2020 19:42:05 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 03 Aug 2020 19:42:05 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 03 Aug 2020 19:42:05 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:8fb3d41b2e9a59630b51745f257cd2561f96bcd15cf309fcc20120d5fcee8c5b`  
		Last Modified: Fri, 29 May 2020 21:42:03 GMT  
		Size: 2.6 MB (2566189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88144f4b1d0ccb9e43e39ac154de5f74f7ad616622b69c604d959bbff10c05ae`  
		Last Modified: Mon, 03 Aug 2020 19:42:18 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4673652cef72557f23239dfa02e8752d0cb5336ab795da58e3f9e76156f6ea1c`  
		Last Modified: Mon, 03 Aug 2020 19:42:18 GMT  
		Size: 6.8 KB (6761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:104d19d98d1e4b1e750f13f131573f9a9757b8848b5f563485da6a594c80218f`  
		Last Modified: Mon, 03 Aug 2020 19:42:18 GMT  
		Size: 594.7 KB (594659 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b42dd365d6b02d300d2aec26f7518bcf990fa814282da55eafce7068a4b363b0`  
		Last Modified: Mon, 03 Aug 2020 19:42:18 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f59fcf025999094f1e53abf0e4be8d7087db6c325c10b049ea824f776365a917`  
		Last Modified: Mon, 03 Aug 2020 19:42:18 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:1-alpine`

```console
$ docker pull spiped@sha256:1350110cc97a6b014a1bfb13ac574c0355b4b0adbd61223b04829a44448978a7
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
$ docker pull spiped@sha256:02675c9b94b81c42442961e3c3f8cee19e108ddd3a6b33f343adc2fe53b993c1
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.4 MB (3400367 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0a93ba8410da7de424982d8512bc0a2923d231ff8ada1683833045890d98b667`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 29 May 2020 21:19:46 GMT
ADD file:c92c248239f8c7b9b3c067650954815f391b7bcb09023f984972c082ace2a8d0 in / 
# Fri, 29 May 2020 21:19:46 GMT
CMD ["/bin/sh"]
# Mon, 03 Aug 2020 20:20:08 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Mon, 03 Aug 2020 20:20:09 GMT
RUN apk add --no-cache libssl1.1
# Mon, 03 Aug 2020 20:20:09 GMT
ENV SPIPED_VERSION=1.6.1
# Mon, 03 Aug 2020 20:20:09 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Mon, 03 Aug 2020 20:20:09 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Mon, 03 Aug 2020 20:20:25 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Mon, 03 Aug 2020 20:20:25 GMT
VOLUME [/spiped]
# Mon, 03 Aug 2020 20:20:26 GMT
WORKDIR /spiped
# Mon, 03 Aug 2020 20:20:26 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 03 Aug 2020 20:20:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 03 Aug 2020 20:20:26 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:df20fa9351a15782c64e6dddb2d4a6f50bf6d3688060a34c4014b0d9a752eb4c`  
		Last Modified: Fri, 29 May 2020 21:20:06 GMT  
		Size: 2.8 MB (2797541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0709a2fdbdb1ec0f8c6e66765ab3a151e1d5b34b886c8297a7031b92de0235b7`  
		Last Modified: Mon, 03 Aug 2020 20:20:37 GMT  
		Size: 1.2 KB (1233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c20256050734396b04f9988dad1e6df07d480c31a61ad023b92256947332287`  
		Last Modified: Mon, 03 Aug 2020 20:20:37 GMT  
		Size: 6.8 KB (6760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:226fbd39a157f769835312ebfabbc4eee4ddc298a97c5789859347ed820e67f0`  
		Last Modified: Mon, 03 Aug 2020 20:20:38 GMT  
		Size: 594.4 KB (594397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5dcd6aead3059d050069913b63bbad929137abd13d8c2187dd26f50cced1886`  
		Last Modified: Mon, 03 Aug 2020 20:20:37 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a24d7067723c20b97da438841dffd17f42f7b15b7376dd65e28358e8559f94f9`  
		Last Modified: Mon, 03 Aug 2020 20:20:37 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; arm variant v6

```console
$ docker pull spiped@sha256:428f8af5290533d8d0486408946485d1ef27812cbd41efb050c7f4387e1a32e4
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.2 MB (3188866 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e66a19f7f66accfb73e0368a006b4e1f163d52335d6bdac248f0a4b90d3e5141`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 29 May 2020 21:50:55 GMT
ADD file:f46e997a56849423db17e5fc9f0249ab6c73b155245927dba5fcb9dfd65f622f in / 
# Fri, 29 May 2020 21:50:56 GMT
CMD ["/bin/sh"]
# Mon, 03 Aug 2020 19:50:37 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Mon, 03 Aug 2020 19:50:41 GMT
RUN apk add --no-cache libssl1.1
# Mon, 03 Aug 2020 19:50:42 GMT
ENV SPIPED_VERSION=1.6.1
# Mon, 03 Aug 2020 19:50:44 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Mon, 03 Aug 2020 19:50:44 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Mon, 03 Aug 2020 19:51:10 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Mon, 03 Aug 2020 19:51:11 GMT
VOLUME [/spiped]
# Mon, 03 Aug 2020 19:51:12 GMT
WORKDIR /spiped
# Mon, 03 Aug 2020 19:51:13 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 03 Aug 2020 19:51:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 03 Aug 2020 19:51:14 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:b4b72e716706d29f5d2351709c20bf737b94f876a5472a43ff1b6e203c65d27f`  
		Last Modified: Fri, 29 May 2020 21:51:30 GMT  
		Size: 2.6 MB (2603286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f06706dce439c2a25997202cc417d1774627055310639653a471802e1e18cedc`  
		Last Modified: Mon, 03 Aug 2020 19:51:29 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c306dde84d54b7dbf70384058b5aea64c8283806bfd63228147b3a9d61b68fe`  
		Last Modified: Mon, 03 Aug 2020 19:51:29 GMT  
		Size: 6.8 KB (6755 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9694005abebc012da97c33a53b778afbf6f7987c6ea39c984048b0c0f72c157f`  
		Last Modified: Mon, 03 Aug 2020 19:51:28 GMT  
		Size: 577.1 KB (577097 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d8220d0ea62d45c8735ee24114bfa496d9ae7da9d8e31e9f78f8bbfd9b4ad5a`  
		Last Modified: Mon, 03 Aug 2020 19:51:28 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85e1b721b9ec152691dfa04ad579c6d80c38e91ff54334dd14a53e8b97ee4f61`  
		Last Modified: Mon, 03 Aug 2020 19:51:28 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; arm variant v7

```console
$ docker pull spiped@sha256:62721b07a25c4f0d9dd82e0b6bfb23adf8b83ea23013c65fd8dc878f8104824a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (2961408 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3aa8e983c241c8e1c7a70f352fd06b840613d94d7cbe725b3a3991691c76292c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 29 May 2020 21:02:07 GMT
ADD file:e97bf0d217846312b19a9f7264604851aedd125c23b4d291eed4c69b880dce26 in / 
# Fri, 29 May 2020 21:02:08 GMT
CMD ["/bin/sh"]
# Mon, 03 Aug 2020 19:58:42 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Mon, 03 Aug 2020 19:58:44 GMT
RUN apk add --no-cache libssl1.1
# Mon, 03 Aug 2020 19:58:45 GMT
ENV SPIPED_VERSION=1.6.1
# Mon, 03 Aug 2020 19:58:45 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Mon, 03 Aug 2020 19:58:46 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Mon, 03 Aug 2020 19:59:09 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Mon, 03 Aug 2020 19:59:10 GMT
VOLUME [/spiped]
# Mon, 03 Aug 2020 19:59:10 GMT
WORKDIR /spiped
# Mon, 03 Aug 2020 19:59:11 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 03 Aug 2020 19:59:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 03 Aug 2020 19:59:13 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:52278dd8e57993669c5b72a9620e89bebdc098f2af2379caaa8945f7403f77a2`  
		Last Modified: Fri, 29 May 2020 21:02:38 GMT  
		Size: 2.4 MB (2406763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96ebb7787066e1f6748cb01370284e61abdf9f769a185bb233de5269e70f4ff5`  
		Last Modified: Mon, 03 Aug 2020 19:59:28 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73e53e87064e4c4c848c3c5e5ccf508a596b96b15bd684fbace51390fba324c6`  
		Last Modified: Mon, 03 Aug 2020 19:59:28 GMT  
		Size: 6.8 KB (6751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c345b088bae12bc87048d3b0b67e872001d831aab0ff4feef6f43c775332188`  
		Last Modified: Mon, 03 Aug 2020 19:59:28 GMT  
		Size: 546.2 KB (546164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15b6a6679ac3b840cca72aee3291b5dea7e1a393a068c5df441f0f3c5954af4c`  
		Last Modified: Mon, 03 Aug 2020 19:59:28 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2b424a6439e7ac0d0af0e96b84399b46f36ec3ad2f19fc15fc0451a533fcc03`  
		Last Modified: Mon, 03 Aug 2020 19:59:28 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:fecf4c0f91fd8da339bbf9a4a7a3f88705a826975ad0e7ea14ad7c08d7f744cd
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.3 MB (3310217 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:34101ceae6105bc2769fc3d77836cf2115c37767429dfebdcd8eec09a11284f9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 29 May 2020 21:43:19 GMT
ADD file:7574aee4e37a85460ab889212d52912723a9b30dda1c060548f0deb4a05fc398 in / 
# Fri, 29 May 2020 21:43:20 GMT
CMD ["/bin/sh"]
# Mon, 03 Aug 2020 19:40:20 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Mon, 03 Aug 2020 19:40:22 GMT
RUN apk add --no-cache libssl1.1
# Mon, 03 Aug 2020 19:40:22 GMT
ENV SPIPED_VERSION=1.6.1
# Mon, 03 Aug 2020 19:40:23 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Mon, 03 Aug 2020 19:40:23 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Mon, 03 Aug 2020 19:40:49 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Mon, 03 Aug 2020 19:40:49 GMT
VOLUME [/spiped]
# Mon, 03 Aug 2020 19:40:50 GMT
WORKDIR /spiped
# Mon, 03 Aug 2020 19:40:51 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 03 Aug 2020 19:40:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 03 Aug 2020 19:40:52 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:b538f80385f9b48122e3da068c932a96ea5018afa3c7be79da00437414bd18cd`  
		Last Modified: Fri, 29 May 2020 21:43:57 GMT  
		Size: 2.7 MB (2707964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:437a35bec8be5212ec28a179a42c49c1015ddd0ffa62c31242e962e4a2162b0a`  
		Last Modified: Mon, 03 Aug 2020 19:41:07 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c1314d231b23210ba600bd2763961e0bdd7aeb7b030c4522450b2a6a9e98c3a`  
		Last Modified: Mon, 03 Aug 2020 19:41:07 GMT  
		Size: 6.8 KB (6759 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bccf45ccb49331db2588902e283a2d1db4e7af8abd9e8487fa8cf0d4d25cffd8`  
		Last Modified: Mon, 03 Aug 2020 19:41:07 GMT  
		Size: 593.8 KB (593769 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75a74cfd6d8862147b08adcee3a5752adfc40b51af87a6a48ece418cc0ac6108`  
		Last Modified: Mon, 03 Aug 2020 19:41:06 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eff509bd366a6122dff1c828625fbe8ac8016c935041a30cf5a64d37c8fc434a`  
		Last Modified: Mon, 03 Aug 2020 19:41:07 GMT  
		Size: 338.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; 386

```console
$ docker pull spiped@sha256:884fc0db36ace906a31efb70cf9740fda3e48e2e90a3b5f9453fc87d0f5291ad
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.4 MB (3394923 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0fbf9ab5830b6d380ce28dd35250ccef8e852b83e6c2debba73e82a6c1597b32`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 29 May 2020 21:38:33 GMT
ADD file:5624441d97aca5eeb82a582941efc3586397098b8391227a9040ebe434cc1d6b in / 
# Fri, 29 May 2020 21:38:33 GMT
CMD ["/bin/sh"]
# Mon, 03 Aug 2020 19:38:55 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Mon, 03 Aug 2020 19:38:56 GMT
RUN apk add --no-cache libssl1.1
# Mon, 03 Aug 2020 19:38:56 GMT
ENV SPIPED_VERSION=1.6.1
# Mon, 03 Aug 2020 19:38:56 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Mon, 03 Aug 2020 19:38:56 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Mon, 03 Aug 2020 19:39:14 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Mon, 03 Aug 2020 19:39:14 GMT
VOLUME [/spiped]
# Mon, 03 Aug 2020 19:39:14 GMT
WORKDIR /spiped
# Mon, 03 Aug 2020 19:39:15 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 03 Aug 2020 19:39:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 03 Aug 2020 19:39:15 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:0625b4155e2a59f647ece47c0cd77ed3196b1f84454fa64ce80cad90e2b9b79e`  
		Last Modified: Fri, 29 May 2020 21:38:53 GMT  
		Size: 2.8 MB (2792298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95b5d8b6933a806504d2858b32e5af5678af48f5b6e8d1449f6fb4dca90be1e9`  
		Last Modified: Mon, 03 Aug 2020 19:39:25 GMT  
		Size: 1.2 KB (1234 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08fa65eed96f55551abfa382372879649328469cc56d14a3bc9354094de4e6c6`  
		Last Modified: Mon, 03 Aug 2020 19:39:24 GMT  
		Size: 6.8 KB (6759 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0f2ab34b6a857c23f06895f0982c1aa304833b4350c483874340ac52ecae085`  
		Last Modified: Mon, 03 Aug 2020 19:39:24 GMT  
		Size: 594.2 KB (594197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca95090aba0b0eb00cdf63a03fda87aab71f510516e4619686900b1e94d0f2d1`  
		Last Modified: Mon, 03 Aug 2020 19:39:25 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a719dbef3762817781395041d1ed9371606bf1ca853ca83a51b8527f6f88a9e`  
		Last Modified: Mon, 03 Aug 2020 19:39:24 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; ppc64le

```console
$ docker pull spiped@sha256:be28a8b592ef19aba9d3d720f74cc34cd2b890ce513a9681b84cedb81aa81d3c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.4 MB (3420796 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:326f45418e4eec122cd9ce53ec66be01c39b21ffb7550260808143f05db37ee9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 29 May 2020 21:23:03 GMT
ADD file:8194808a812370fd2202d80d1667f851bd9eac4c560d69d347fe1964f54343de in / 
# Fri, 29 May 2020 21:23:06 GMT
CMD ["/bin/sh"]
# Mon, 03 Aug 2020 20:17:58 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Mon, 03 Aug 2020 20:18:07 GMT
RUN apk add --no-cache libssl1.1
# Mon, 03 Aug 2020 20:18:14 GMT
ENV SPIPED_VERSION=1.6.1
# Mon, 03 Aug 2020 20:18:17 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Mon, 03 Aug 2020 20:18:21 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Mon, 03 Aug 2020 20:18:54 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Mon, 03 Aug 2020 20:18:59 GMT
VOLUME [/spiped]
# Mon, 03 Aug 2020 20:19:05 GMT
WORKDIR /spiped
# Mon, 03 Aug 2020 20:19:08 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 03 Aug 2020 20:19:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 03 Aug 2020 20:19:19 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:5077f8601dceb5744d875d7740ebc203f674b108a0188f3a31e292b21a4bee64`  
		Last Modified: Fri, 29 May 2020 21:23:37 GMT  
		Size: 2.8 MB (2805199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab223d5e8b6fad2e0a685c6d01913edb1021ad4f98cf6f280c84a587585b4be3`  
		Last Modified: Mon, 03 Aug 2020 20:19:40 GMT  
		Size: 1.3 KB (1262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c5463b129a00b3d487dc47b34bd226c4fcd815b44b9d4ec783ebbae814db9be`  
		Last Modified: Mon, 03 Aug 2020 20:19:40 GMT  
		Size: 6.8 KB (6760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb8a2aaec72079901e78cdcda1d214a6408e04fd111b01bbf4865e4731befef6`  
		Last Modified: Mon, 03 Aug 2020 20:19:41 GMT  
		Size: 607.1 KB (607103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5128ec33b43788f96f1f9d53e9b0e3a9b073f51bb7ef4bec5639b8367d9f0d5f`  
		Last Modified: Mon, 03 Aug 2020 20:19:40 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21cc02ad1ba276590592ea772c67711daefffc109f32e4a9114e67cd81c8f39d`  
		Last Modified: Mon, 03 Aug 2020 20:19:40 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; s390x

```console
$ docker pull spiped@sha256:b73ea63f68d61aabf2d30f81eb4cf11388380f6b7779980550e039b24e8daf02
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.2 MB (3169341 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dedd11800ad772a1acff1311f9f24324d234762e6ba34aa4dc6f62bde7b8c720`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 29 May 2020 21:41:39 GMT
ADD file:9799ce3b2f782a28e10b1846cd9b3db827fa99c9bc601feb268456195856814e in / 
# Fri, 29 May 2020 21:41:39 GMT
CMD ["/bin/sh"]
# Mon, 03 Aug 2020 19:41:51 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Mon, 03 Aug 2020 19:41:52 GMT
RUN apk add --no-cache libssl1.1
# Mon, 03 Aug 2020 19:41:53 GMT
ENV SPIPED_VERSION=1.6.1
# Mon, 03 Aug 2020 19:41:53 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Mon, 03 Aug 2020 19:41:54 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Mon, 03 Aug 2020 19:42:04 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Mon, 03 Aug 2020 19:42:04 GMT
VOLUME [/spiped]
# Mon, 03 Aug 2020 19:42:04 GMT
WORKDIR /spiped
# Mon, 03 Aug 2020 19:42:05 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 03 Aug 2020 19:42:05 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 03 Aug 2020 19:42:05 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:8fb3d41b2e9a59630b51745f257cd2561f96bcd15cf309fcc20120d5fcee8c5b`  
		Last Modified: Fri, 29 May 2020 21:42:03 GMT  
		Size: 2.6 MB (2566189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88144f4b1d0ccb9e43e39ac154de5f74f7ad616622b69c604d959bbff10c05ae`  
		Last Modified: Mon, 03 Aug 2020 19:42:18 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4673652cef72557f23239dfa02e8752d0cb5336ab795da58e3f9e76156f6ea1c`  
		Last Modified: Mon, 03 Aug 2020 19:42:18 GMT  
		Size: 6.8 KB (6761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:104d19d98d1e4b1e750f13f131573f9a9757b8848b5f563485da6a594c80218f`  
		Last Modified: Mon, 03 Aug 2020 19:42:18 GMT  
		Size: 594.7 KB (594659 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b42dd365d6b02d300d2aec26f7518bcf990fa814282da55eafce7068a4b363b0`  
		Last Modified: Mon, 03 Aug 2020 19:42:18 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f59fcf025999094f1e53abf0e4be8d7087db6c325c10b049ea824f776365a917`  
		Last Modified: Mon, 03 Aug 2020 19:42:18 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:alpine`

```console
$ docker pull spiped@sha256:1350110cc97a6b014a1bfb13ac574c0355b4b0adbd61223b04829a44448978a7
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
$ docker pull spiped@sha256:02675c9b94b81c42442961e3c3f8cee19e108ddd3a6b33f343adc2fe53b993c1
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.4 MB (3400367 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0a93ba8410da7de424982d8512bc0a2923d231ff8ada1683833045890d98b667`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 29 May 2020 21:19:46 GMT
ADD file:c92c248239f8c7b9b3c067650954815f391b7bcb09023f984972c082ace2a8d0 in / 
# Fri, 29 May 2020 21:19:46 GMT
CMD ["/bin/sh"]
# Mon, 03 Aug 2020 20:20:08 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Mon, 03 Aug 2020 20:20:09 GMT
RUN apk add --no-cache libssl1.1
# Mon, 03 Aug 2020 20:20:09 GMT
ENV SPIPED_VERSION=1.6.1
# Mon, 03 Aug 2020 20:20:09 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Mon, 03 Aug 2020 20:20:09 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Mon, 03 Aug 2020 20:20:25 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Mon, 03 Aug 2020 20:20:25 GMT
VOLUME [/spiped]
# Mon, 03 Aug 2020 20:20:26 GMT
WORKDIR /spiped
# Mon, 03 Aug 2020 20:20:26 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 03 Aug 2020 20:20:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 03 Aug 2020 20:20:26 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:df20fa9351a15782c64e6dddb2d4a6f50bf6d3688060a34c4014b0d9a752eb4c`  
		Last Modified: Fri, 29 May 2020 21:20:06 GMT  
		Size: 2.8 MB (2797541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0709a2fdbdb1ec0f8c6e66765ab3a151e1d5b34b886c8297a7031b92de0235b7`  
		Last Modified: Mon, 03 Aug 2020 20:20:37 GMT  
		Size: 1.2 KB (1233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c20256050734396b04f9988dad1e6df07d480c31a61ad023b92256947332287`  
		Last Modified: Mon, 03 Aug 2020 20:20:37 GMT  
		Size: 6.8 KB (6760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:226fbd39a157f769835312ebfabbc4eee4ddc298a97c5789859347ed820e67f0`  
		Last Modified: Mon, 03 Aug 2020 20:20:38 GMT  
		Size: 594.4 KB (594397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5dcd6aead3059d050069913b63bbad929137abd13d8c2187dd26f50cced1886`  
		Last Modified: Mon, 03 Aug 2020 20:20:37 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a24d7067723c20b97da438841dffd17f42f7b15b7376dd65e28358e8559f94f9`  
		Last Modified: Mon, 03 Aug 2020 20:20:37 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; arm variant v6

```console
$ docker pull spiped@sha256:428f8af5290533d8d0486408946485d1ef27812cbd41efb050c7f4387e1a32e4
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.2 MB (3188866 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e66a19f7f66accfb73e0368a006b4e1f163d52335d6bdac248f0a4b90d3e5141`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 29 May 2020 21:50:55 GMT
ADD file:f46e997a56849423db17e5fc9f0249ab6c73b155245927dba5fcb9dfd65f622f in / 
# Fri, 29 May 2020 21:50:56 GMT
CMD ["/bin/sh"]
# Mon, 03 Aug 2020 19:50:37 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Mon, 03 Aug 2020 19:50:41 GMT
RUN apk add --no-cache libssl1.1
# Mon, 03 Aug 2020 19:50:42 GMT
ENV SPIPED_VERSION=1.6.1
# Mon, 03 Aug 2020 19:50:44 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Mon, 03 Aug 2020 19:50:44 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Mon, 03 Aug 2020 19:51:10 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Mon, 03 Aug 2020 19:51:11 GMT
VOLUME [/spiped]
# Mon, 03 Aug 2020 19:51:12 GMT
WORKDIR /spiped
# Mon, 03 Aug 2020 19:51:13 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 03 Aug 2020 19:51:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 03 Aug 2020 19:51:14 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:b4b72e716706d29f5d2351709c20bf737b94f876a5472a43ff1b6e203c65d27f`  
		Last Modified: Fri, 29 May 2020 21:51:30 GMT  
		Size: 2.6 MB (2603286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f06706dce439c2a25997202cc417d1774627055310639653a471802e1e18cedc`  
		Last Modified: Mon, 03 Aug 2020 19:51:29 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c306dde84d54b7dbf70384058b5aea64c8283806bfd63228147b3a9d61b68fe`  
		Last Modified: Mon, 03 Aug 2020 19:51:29 GMT  
		Size: 6.8 KB (6755 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9694005abebc012da97c33a53b778afbf6f7987c6ea39c984048b0c0f72c157f`  
		Last Modified: Mon, 03 Aug 2020 19:51:28 GMT  
		Size: 577.1 KB (577097 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d8220d0ea62d45c8735ee24114bfa496d9ae7da9d8e31e9f78f8bbfd9b4ad5a`  
		Last Modified: Mon, 03 Aug 2020 19:51:28 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85e1b721b9ec152691dfa04ad579c6d80c38e91ff54334dd14a53e8b97ee4f61`  
		Last Modified: Mon, 03 Aug 2020 19:51:28 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; arm variant v7

```console
$ docker pull spiped@sha256:62721b07a25c4f0d9dd82e0b6bfb23adf8b83ea23013c65fd8dc878f8104824a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (2961408 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3aa8e983c241c8e1c7a70f352fd06b840613d94d7cbe725b3a3991691c76292c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 29 May 2020 21:02:07 GMT
ADD file:e97bf0d217846312b19a9f7264604851aedd125c23b4d291eed4c69b880dce26 in / 
# Fri, 29 May 2020 21:02:08 GMT
CMD ["/bin/sh"]
# Mon, 03 Aug 2020 19:58:42 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Mon, 03 Aug 2020 19:58:44 GMT
RUN apk add --no-cache libssl1.1
# Mon, 03 Aug 2020 19:58:45 GMT
ENV SPIPED_VERSION=1.6.1
# Mon, 03 Aug 2020 19:58:45 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Mon, 03 Aug 2020 19:58:46 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Mon, 03 Aug 2020 19:59:09 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Mon, 03 Aug 2020 19:59:10 GMT
VOLUME [/spiped]
# Mon, 03 Aug 2020 19:59:10 GMT
WORKDIR /spiped
# Mon, 03 Aug 2020 19:59:11 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 03 Aug 2020 19:59:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 03 Aug 2020 19:59:13 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:52278dd8e57993669c5b72a9620e89bebdc098f2af2379caaa8945f7403f77a2`  
		Last Modified: Fri, 29 May 2020 21:02:38 GMT  
		Size: 2.4 MB (2406763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96ebb7787066e1f6748cb01370284e61abdf9f769a185bb233de5269e70f4ff5`  
		Last Modified: Mon, 03 Aug 2020 19:59:28 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73e53e87064e4c4c848c3c5e5ccf508a596b96b15bd684fbace51390fba324c6`  
		Last Modified: Mon, 03 Aug 2020 19:59:28 GMT  
		Size: 6.8 KB (6751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c345b088bae12bc87048d3b0b67e872001d831aab0ff4feef6f43c775332188`  
		Last Modified: Mon, 03 Aug 2020 19:59:28 GMT  
		Size: 546.2 KB (546164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15b6a6679ac3b840cca72aee3291b5dea7e1a393a068c5df441f0f3c5954af4c`  
		Last Modified: Mon, 03 Aug 2020 19:59:28 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2b424a6439e7ac0d0af0e96b84399b46f36ec3ad2f19fc15fc0451a533fcc03`  
		Last Modified: Mon, 03 Aug 2020 19:59:28 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:fecf4c0f91fd8da339bbf9a4a7a3f88705a826975ad0e7ea14ad7c08d7f744cd
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.3 MB (3310217 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:34101ceae6105bc2769fc3d77836cf2115c37767429dfebdcd8eec09a11284f9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 29 May 2020 21:43:19 GMT
ADD file:7574aee4e37a85460ab889212d52912723a9b30dda1c060548f0deb4a05fc398 in / 
# Fri, 29 May 2020 21:43:20 GMT
CMD ["/bin/sh"]
# Mon, 03 Aug 2020 19:40:20 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Mon, 03 Aug 2020 19:40:22 GMT
RUN apk add --no-cache libssl1.1
# Mon, 03 Aug 2020 19:40:22 GMT
ENV SPIPED_VERSION=1.6.1
# Mon, 03 Aug 2020 19:40:23 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Mon, 03 Aug 2020 19:40:23 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Mon, 03 Aug 2020 19:40:49 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Mon, 03 Aug 2020 19:40:49 GMT
VOLUME [/spiped]
# Mon, 03 Aug 2020 19:40:50 GMT
WORKDIR /spiped
# Mon, 03 Aug 2020 19:40:51 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 03 Aug 2020 19:40:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 03 Aug 2020 19:40:52 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:b538f80385f9b48122e3da068c932a96ea5018afa3c7be79da00437414bd18cd`  
		Last Modified: Fri, 29 May 2020 21:43:57 GMT  
		Size: 2.7 MB (2707964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:437a35bec8be5212ec28a179a42c49c1015ddd0ffa62c31242e962e4a2162b0a`  
		Last Modified: Mon, 03 Aug 2020 19:41:07 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c1314d231b23210ba600bd2763961e0bdd7aeb7b030c4522450b2a6a9e98c3a`  
		Last Modified: Mon, 03 Aug 2020 19:41:07 GMT  
		Size: 6.8 KB (6759 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bccf45ccb49331db2588902e283a2d1db4e7af8abd9e8487fa8cf0d4d25cffd8`  
		Last Modified: Mon, 03 Aug 2020 19:41:07 GMT  
		Size: 593.8 KB (593769 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75a74cfd6d8862147b08adcee3a5752adfc40b51af87a6a48ece418cc0ac6108`  
		Last Modified: Mon, 03 Aug 2020 19:41:06 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eff509bd366a6122dff1c828625fbe8ac8016c935041a30cf5a64d37c8fc434a`  
		Last Modified: Mon, 03 Aug 2020 19:41:07 GMT  
		Size: 338.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; 386

```console
$ docker pull spiped@sha256:884fc0db36ace906a31efb70cf9740fda3e48e2e90a3b5f9453fc87d0f5291ad
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.4 MB (3394923 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0fbf9ab5830b6d380ce28dd35250ccef8e852b83e6c2debba73e82a6c1597b32`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 29 May 2020 21:38:33 GMT
ADD file:5624441d97aca5eeb82a582941efc3586397098b8391227a9040ebe434cc1d6b in / 
# Fri, 29 May 2020 21:38:33 GMT
CMD ["/bin/sh"]
# Mon, 03 Aug 2020 19:38:55 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Mon, 03 Aug 2020 19:38:56 GMT
RUN apk add --no-cache libssl1.1
# Mon, 03 Aug 2020 19:38:56 GMT
ENV SPIPED_VERSION=1.6.1
# Mon, 03 Aug 2020 19:38:56 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Mon, 03 Aug 2020 19:38:56 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Mon, 03 Aug 2020 19:39:14 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Mon, 03 Aug 2020 19:39:14 GMT
VOLUME [/spiped]
# Mon, 03 Aug 2020 19:39:14 GMT
WORKDIR /spiped
# Mon, 03 Aug 2020 19:39:15 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 03 Aug 2020 19:39:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 03 Aug 2020 19:39:15 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:0625b4155e2a59f647ece47c0cd77ed3196b1f84454fa64ce80cad90e2b9b79e`  
		Last Modified: Fri, 29 May 2020 21:38:53 GMT  
		Size: 2.8 MB (2792298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95b5d8b6933a806504d2858b32e5af5678af48f5b6e8d1449f6fb4dca90be1e9`  
		Last Modified: Mon, 03 Aug 2020 19:39:25 GMT  
		Size: 1.2 KB (1234 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08fa65eed96f55551abfa382372879649328469cc56d14a3bc9354094de4e6c6`  
		Last Modified: Mon, 03 Aug 2020 19:39:24 GMT  
		Size: 6.8 KB (6759 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0f2ab34b6a857c23f06895f0982c1aa304833b4350c483874340ac52ecae085`  
		Last Modified: Mon, 03 Aug 2020 19:39:24 GMT  
		Size: 594.2 KB (594197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca95090aba0b0eb00cdf63a03fda87aab71f510516e4619686900b1e94d0f2d1`  
		Last Modified: Mon, 03 Aug 2020 19:39:25 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a719dbef3762817781395041d1ed9371606bf1ca853ca83a51b8527f6f88a9e`  
		Last Modified: Mon, 03 Aug 2020 19:39:24 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; ppc64le

```console
$ docker pull spiped@sha256:be28a8b592ef19aba9d3d720f74cc34cd2b890ce513a9681b84cedb81aa81d3c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.4 MB (3420796 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:326f45418e4eec122cd9ce53ec66be01c39b21ffb7550260808143f05db37ee9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 29 May 2020 21:23:03 GMT
ADD file:8194808a812370fd2202d80d1667f851bd9eac4c560d69d347fe1964f54343de in / 
# Fri, 29 May 2020 21:23:06 GMT
CMD ["/bin/sh"]
# Mon, 03 Aug 2020 20:17:58 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Mon, 03 Aug 2020 20:18:07 GMT
RUN apk add --no-cache libssl1.1
# Mon, 03 Aug 2020 20:18:14 GMT
ENV SPIPED_VERSION=1.6.1
# Mon, 03 Aug 2020 20:18:17 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Mon, 03 Aug 2020 20:18:21 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Mon, 03 Aug 2020 20:18:54 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Mon, 03 Aug 2020 20:18:59 GMT
VOLUME [/spiped]
# Mon, 03 Aug 2020 20:19:05 GMT
WORKDIR /spiped
# Mon, 03 Aug 2020 20:19:08 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 03 Aug 2020 20:19:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 03 Aug 2020 20:19:19 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:5077f8601dceb5744d875d7740ebc203f674b108a0188f3a31e292b21a4bee64`  
		Last Modified: Fri, 29 May 2020 21:23:37 GMT  
		Size: 2.8 MB (2805199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab223d5e8b6fad2e0a685c6d01913edb1021ad4f98cf6f280c84a587585b4be3`  
		Last Modified: Mon, 03 Aug 2020 20:19:40 GMT  
		Size: 1.3 KB (1262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c5463b129a00b3d487dc47b34bd226c4fcd815b44b9d4ec783ebbae814db9be`  
		Last Modified: Mon, 03 Aug 2020 20:19:40 GMT  
		Size: 6.8 KB (6760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb8a2aaec72079901e78cdcda1d214a6408e04fd111b01bbf4865e4731befef6`  
		Last Modified: Mon, 03 Aug 2020 20:19:41 GMT  
		Size: 607.1 KB (607103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5128ec33b43788f96f1f9d53e9b0e3a9b073f51bb7ef4bec5639b8367d9f0d5f`  
		Last Modified: Mon, 03 Aug 2020 20:19:40 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21cc02ad1ba276590592ea772c67711daefffc109f32e4a9114e67cd81c8f39d`  
		Last Modified: Mon, 03 Aug 2020 20:19:40 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; s390x

```console
$ docker pull spiped@sha256:b73ea63f68d61aabf2d30f81eb4cf11388380f6b7779980550e039b24e8daf02
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.2 MB (3169341 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dedd11800ad772a1acff1311f9f24324d234762e6ba34aa4dc6f62bde7b8c720`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 29 May 2020 21:41:39 GMT
ADD file:9799ce3b2f782a28e10b1846cd9b3db827fa99c9bc601feb268456195856814e in / 
# Fri, 29 May 2020 21:41:39 GMT
CMD ["/bin/sh"]
# Mon, 03 Aug 2020 19:41:51 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Mon, 03 Aug 2020 19:41:52 GMT
RUN apk add --no-cache libssl1.1
# Mon, 03 Aug 2020 19:41:53 GMT
ENV SPIPED_VERSION=1.6.1
# Mon, 03 Aug 2020 19:41:53 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Mon, 03 Aug 2020 19:41:54 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Mon, 03 Aug 2020 19:42:04 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Mon, 03 Aug 2020 19:42:04 GMT
VOLUME [/spiped]
# Mon, 03 Aug 2020 19:42:04 GMT
WORKDIR /spiped
# Mon, 03 Aug 2020 19:42:05 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 03 Aug 2020 19:42:05 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 03 Aug 2020 19:42:05 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:8fb3d41b2e9a59630b51745f257cd2561f96bcd15cf309fcc20120d5fcee8c5b`  
		Last Modified: Fri, 29 May 2020 21:42:03 GMT  
		Size: 2.6 MB (2566189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88144f4b1d0ccb9e43e39ac154de5f74f7ad616622b69c604d959bbff10c05ae`  
		Last Modified: Mon, 03 Aug 2020 19:42:18 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4673652cef72557f23239dfa02e8752d0cb5336ab795da58e3f9e76156f6ea1c`  
		Last Modified: Mon, 03 Aug 2020 19:42:18 GMT  
		Size: 6.8 KB (6761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:104d19d98d1e4b1e750f13f131573f9a9757b8848b5f563485da6a594c80218f`  
		Last Modified: Mon, 03 Aug 2020 19:42:18 GMT  
		Size: 594.7 KB (594659 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b42dd365d6b02d300d2aec26f7518bcf990fa814282da55eafce7068a4b363b0`  
		Last Modified: Mon, 03 Aug 2020 19:42:18 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f59fcf025999094f1e53abf0e4be8d7087db6c325c10b049ea824f776365a917`  
		Last Modified: Mon, 03 Aug 2020 19:42:18 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:latest`

```console
$ docker pull spiped@sha256:79df51f975875356a7b20bd3eeab8678f6d57e36bfd0f02566fd46e7c03e7b8b
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
$ docker pull spiped@sha256:cbcdcae2145e7f1c5b4c4e2ec9926e8f7cf2741c2edd41e74eb1a5ca85431c6a
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.3 MB (36260010 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ff3a3a8321db5126e2cfa970d9cabeafcbc493ae611c56ac1b7f3bc9c1877287`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 13 Oct 2020 01:39:05 GMT
ADD file:0dc53e7886c35bc21ae6c4f6cedda54d56ae9c9e9cd367678f1a72e68b3c43d4 in / 
# Tue, 13 Oct 2020 01:39:05 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 02:36:30 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 13 Oct 2020 02:36:35 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 13 Oct 2020 02:36:35 GMT
ENV SPIPED_VERSION=1.6.1
# Tue, 13 Oct 2020 02:36:36 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Tue, 13 Oct 2020 02:36:36 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Tue, 13 Oct 2020 02:37:05 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 13 Oct 2020 02:37:06 GMT
VOLUME [/spiped]
# Tue, 13 Oct 2020 02:37:06 GMT
WORKDIR /spiped
# Tue, 13 Oct 2020 02:37:06 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 13 Oct 2020 02:37:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 13 Oct 2020 02:37:07 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:bb79b6b2107fea8e8a47133a660b78e3a546998fcf0427be39ac9a0af4a97e90`  
		Last Modified: Tue, 13 Oct 2020 01:48:17 GMT  
		Size: 27.1 MB (27092228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e7e552308a9a7e56787eb8f2ee2cd0e5ae1bcd3e6e70767a3f1f63d04df1043`  
		Last Modified: Tue, 13 Oct 2020 02:37:24 GMT  
		Size: 1.7 KB (1738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fae3cfef5f840d90ca6a31c452db1ff437bc80f30c34bfe95e60a73d26faa39a`  
		Last Modified: Tue, 13 Oct 2020 02:37:25 GMT  
		Size: 2.1 MB (2128094 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3b92b058cf5a162f3e9e9c1b57e6ea521b98cfbdfe95c64e96543614c0aa889`  
		Last Modified: Tue, 13 Oct 2020 02:37:26 GMT  
		Size: 7.0 MB (7037515 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43e07e79b0faf86dec01bde507101fa39b284b027b0a16dcc2e0385b2711b7d7`  
		Last Modified: Tue, 13 Oct 2020 02:37:25 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2774b42f92e50846c6909f7c57a4559f4e39365596961f3cc60c181fd5ff02f7`  
		Last Modified: Tue, 13 Oct 2020 02:37:24 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; arm variant v5

```console
$ docker pull spiped@sha256:672edee7237da76ba6de9367e734a27d7f8f8562c11afcb03f3b145d6d260015
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.2 MB (32157300 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:17e88bd24524f59d6103fec000e35dde5b823055a634e55e935d247d8ac5444a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 13 Oct 2020 01:52:17 GMT
ADD file:b71c0fa4957d6b65af37231a105f3d17cdbafe5c7d6c37b5843ebf619c608aaa in / 
# Tue, 13 Oct 2020 01:52:27 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 03:19:47 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 13 Oct 2020 03:20:02 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 13 Oct 2020 03:20:03 GMT
ENV SPIPED_VERSION=1.6.1
# Tue, 13 Oct 2020 03:20:04 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Tue, 13 Oct 2020 03:20:05 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Tue, 13 Oct 2020 03:21:05 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 13 Oct 2020 03:21:10 GMT
VOLUME [/spiped]
# Tue, 13 Oct 2020 03:21:11 GMT
WORKDIR /spiped
# Tue, 13 Oct 2020 03:21:12 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 13 Oct 2020 03:21:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 13 Oct 2020 03:21:14 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:f991c1e1ee2c48f16625b6b61310bf3c0616c0dbda4762019117e86fd29cf9ce`  
		Last Modified: Tue, 13 Oct 2020 02:01:27 GMT  
		Size: 24.8 MB (24835992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bfc2a4609d9b5232a9e51a28b5db91ffc8c66f8660df9bcf2f5d1e3bceccec0`  
		Last Modified: Tue, 13 Oct 2020 03:21:36 GMT  
		Size: 1.7 KB (1737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:098bc9c2699c25d745dbdf0cb778c6194789b2d87ee75581c62527cc53f62a01`  
		Last Modified: Tue, 13 Oct 2020 03:21:37 GMT  
		Size: 1.8 MB (1839142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f23ff5b2f49dbf01bbcabfe3c39e09035f01987cdb3987c44dd29b8e562c9c79`  
		Last Modified: Tue, 13 Oct 2020 03:21:38 GMT  
		Size: 5.5 MB (5479959 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6783146d326266ff3b29ec06b968d70f4c9d910ed3b3d4b90a52adce04f6a4f2`  
		Last Modified: Tue, 13 Oct 2020 03:21:36 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e71a40b93164b5b86c29eae7931a993d7a6b035139e1d330fcaa7bb9f1663d30`  
		Last Modified: Tue, 13 Oct 2020 03:21:37 GMT  
		Size: 341.0 B  
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
$ docker pull spiped@sha256:020927c2bce85e0a6153b9e3fba53483f1ca59bec55e71c09bfb448087264273
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.5 MB (41517895 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:faa5ea3e409fa66afb6ac2267b51c0db7a950a67d5efd32aa7094a082bd8ac57`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 13 Oct 2020 01:41:03 GMT
ADD file:51108b89c70ce0773c897be520c84454660f38b84ba556da49c7fe77e5d52416 in / 
# Tue, 13 Oct 2020 01:41:03 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 07:08:37 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 13 Oct 2020 07:08:42 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 13 Oct 2020 07:08:43 GMT
ENV SPIPED_VERSION=1.6.1
# Tue, 13 Oct 2020 07:08:43 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Tue, 13 Oct 2020 07:08:43 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Tue, 13 Oct 2020 07:09:13 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 13 Oct 2020 07:09:14 GMT
VOLUME [/spiped]
# Tue, 13 Oct 2020 07:09:14 GMT
WORKDIR /spiped
# Tue, 13 Oct 2020 07:09:14 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 13 Oct 2020 07:09:14 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 13 Oct 2020 07:09:15 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:97e4efec21eea92209464547d0f52a0f773c505cf4ea9d8090cef667bde145b8`  
		Last Modified: Tue, 13 Oct 2020 01:48:54 GMT  
		Size: 27.8 MB (27750243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:745fb22bef9b177604b68c486de51931377440e01812132d536beb88d70a5d21`  
		Last Modified: Tue, 13 Oct 2020 07:09:32 GMT  
		Size: 1.7 KB (1730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82d19eade6c6a313dc1c60e86222d6bafb19b6a105b28092bbd0cc98b4c0070f`  
		Last Modified: Tue, 13 Oct 2020 07:09:33 GMT  
		Size: 2.1 MB (2132324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:532cde1db9018cf5bdfd3b40054c0ad417b669d165c66aca9a994bc452d3c4fa`  
		Last Modified: Tue, 13 Oct 2020 07:09:36 GMT  
		Size: 11.6 MB (11633161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1dca20ce2d893f37dacd76615c6eacb8d643d74c3989b598ab4e4158b6bfc4e`  
		Last Modified: Tue, 13 Oct 2020 07:09:32 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:216b5ffd9d325d221945ae36ab00beed34a9aaea74f6118052db2fcba2c563ea`  
		Last Modified: Tue, 13 Oct 2020 07:09:32 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; mips64le

```console
$ docker pull spiped@sha256:bfe5c974767b865a68adb72cce4848ecaa36cab8992abfaff529176fc18ed961
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.9 MB (33893051 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0f86dfdfdd1df8f189c47811b193797f1bd21f709ec9849d5b71fb83d64fc0f8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 13 Oct 2020 01:09:50 GMT
ADD file:c2ad270f70511601478158cfe3854499c0b4887f049b78b66903412a811a428a in / 
# Tue, 13 Oct 2020 01:09:50 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 02:30:03 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 13 Oct 2020 02:30:16 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 13 Oct 2020 02:30:16 GMT
ENV SPIPED_VERSION=1.6.1
# Tue, 13 Oct 2020 02:30:16 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Tue, 13 Oct 2020 02:30:17 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Tue, 13 Oct 2020 02:31:24 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 13 Oct 2020 02:31:24 GMT
VOLUME [/spiped]
# Tue, 13 Oct 2020 02:31:24 GMT
WORKDIR /spiped
# Tue, 13 Oct 2020 02:31:25 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 13 Oct 2020 02:31:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 13 Oct 2020 02:31:26 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:9bc77d453b2242ec513032b61e23061712b79c3ba0c60114232d743e5ab4e4fa`  
		Last Modified: Tue, 13 Oct 2020 01:16:41 GMT  
		Size: 25.8 MB (25762577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5be50d34e573637b833f398c4bb03213fdc0e39948eb67673d4e6090fd69a86b`  
		Last Modified: Tue, 13 Oct 2020 02:31:50 GMT  
		Size: 1.7 KB (1740 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56986f62a854f267f51d23dcdfce8ed543e5c3f7ecaa67057a60aeba849366ae`  
		Last Modified: Tue, 13 Oct 2020 02:31:51 GMT  
		Size: 1.7 MB (1712061 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8827c190f0eb33937717d762d6cd11a35e2a49ba62d7af225998650be849266d`  
		Last Modified: Tue, 13 Oct 2020 02:31:56 GMT  
		Size: 6.4 MB (6416237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a38c49421fb63af5186fbe4e32552de9ad359f4d9611ca42956e2bce8ce49a98`  
		Last Modified: Tue, 13 Oct 2020 02:31:50 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74f89d8674f8700037b86df03ef1fd4e5e40b04138c1deb95601e7e1723050bb`  
		Last Modified: Tue, 13 Oct 2020 02:31:50 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; ppc64le

```console
$ docker pull spiped@sha256:11f9c1dbc68d2bcdd7a7f524027219a963ce523b201e71ae83c7052e635b27c1
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.5 MB (39488625 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cc337b8be5274e46ce4e2892582058be9fe426dc646660aa407e845573321c32`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 13 Oct 2020 01:38:54 GMT
ADD file:9992867f855c9bed54df6d26f3d8076689aff8a51e808fefba7d3b66dab250e5 in / 
# Tue, 13 Oct 2020 01:38:59 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 08:32:35 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 13 Oct 2020 08:33:10 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 13 Oct 2020 08:33:18 GMT
ENV SPIPED_VERSION=1.6.1
# Tue, 13 Oct 2020 08:33:25 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Tue, 13 Oct 2020 08:33:33 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Tue, 13 Oct 2020 08:40:10 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 13 Oct 2020 08:40:16 GMT
VOLUME [/spiped]
# Tue, 13 Oct 2020 08:40:29 GMT
WORKDIR /spiped
# Tue, 13 Oct 2020 08:40:33 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 13 Oct 2020 08:40:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 13 Oct 2020 08:40:44 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:523555c6877c72cfcdec912b4d0053c298b1c97835efc7c6b0211585a06bd563`  
		Last Modified: Tue, 13 Oct 2020 01:50:10 GMT  
		Size: 30.5 MB (30517878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e1d07b98a86b2674f96635104e41916c1e547434cb7d561cd85492408607281`  
		Last Modified: Tue, 13 Oct 2020 08:41:22 GMT  
		Size: 1.7 KB (1745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d2c21d3c72f09a47ee5eaa7be57ecda6468c5095c72c0ae090abfab50a53f17`  
		Last Modified: Tue, 13 Oct 2020 08:41:22 GMT  
		Size: 2.2 MB (2225018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b4a219f1f2d5be3ad0b26293fc2b817c1bb804bb21197d100b7dd072101f007`  
		Last Modified: Tue, 13 Oct 2020 08:41:22 GMT  
		Size: 6.7 MB (6743513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a3cacc68fbff4f9b9f07d0bb78c5b34216d92ff73ee186cbac165f8ee0cc552`  
		Last Modified: Tue, 13 Oct 2020 08:41:18 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:809a6e602fa91081254fd3482a446e8d14916d389cda086023515709324d584b`  
		Last Modified: Tue, 13 Oct 2020 08:41:18 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; s390x

```console
$ docker pull spiped@sha256:3feac6ba4263f960d8481dee734f70e1f4b0daea3436dcc444e6d37616e90f81
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.5 MB (33475004 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:239e569a133e1fb83824c9c12873d8c897d84bc87265b777b3b39e179c31d516`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 13 Oct 2020 01:42:26 GMT
ADD file:f932c1176fdc9bf45ced816290f83e6231df3dffa3b7f8de1a3bb0adcff1588b in / 
# Tue, 13 Oct 2020 01:42:27 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 06:29:14 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 13 Oct 2020 06:29:19 GMT
RUN DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 13 Oct 2020 06:29:20 GMT
ENV SPIPED_VERSION=1.6.1
# Tue, 13 Oct 2020 06:29:20 GMT
ENV SPIPED_DOWNLOAD_URL=https://www.tarsnap.com/spiped/spiped-1.6.1.tgz
# Tue, 13 Oct 2020 06:29:20 GMT
ENV SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Tue, 13 Oct 2020 06:29:47 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update && apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "$SPIPED_DOWNLOAD_URL" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 13 Oct 2020 06:29:48 GMT
VOLUME [/spiped]
# Tue, 13 Oct 2020 06:29:49 GMT
WORKDIR /spiped
# Tue, 13 Oct 2020 06:29:49 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 13 Oct 2020 06:29:49 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 13 Oct 2020 06:29:50 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:2a4f9dc00d797c86c4ffce3b50bea9037c2eb4637f045ad3fd68cf151577b639`  
		Last Modified: Tue, 13 Oct 2020 01:45:45 GMT  
		Size: 25.7 MB (25707519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8de0e34331f0b780854c48224e0de248e8951e70d8846ff0fe303e83d4425c38`  
		Last Modified: Tue, 13 Oct 2020 06:30:07 GMT  
		Size: 1.7 KB (1739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e4244b6ed8088d52ab38a21af88c52cfb32af480c91f3ebb8b84cdb807fe209`  
		Last Modified: Tue, 13 Oct 2020 06:30:07 GMT  
		Size: 1.8 MB (1821803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edbf619e3fe12a6407295c6f4a1cd8379ef1e9b588b41999d1fd99578395bf09`  
		Last Modified: Tue, 13 Oct 2020 06:30:08 GMT  
		Size: 5.9 MB (5943472 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4daaafe9626c1495df1df7db30d89e5f7a3e3e451f17cfe519a205fcd9e900c9`  
		Last Modified: Tue, 13 Oct 2020 06:30:07 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d3ebfbb7e7b045ea63889ea6b91bf081c0ba9ac7d0e7b7ca274a841059f6b31`  
		Last Modified: Tue, 13 Oct 2020 06:30:06 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
