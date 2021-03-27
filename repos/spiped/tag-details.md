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
$ docker pull spiped@sha256:de60f1e86120845dfc5fc566e992ac2528bab5092551860ff597aaa498ba6d12
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
$ docker pull spiped@sha256:cf4b9920b3942ecc606b6251cd4eb1bd48f98354d8e022b3f6307e507a32a3eb
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.3 MB (36268832 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:57285b121dc86ae46a0c0ce8c6f60015ae52e9e52103a25f3f7e0bee876c9013`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 12 Mar 2021 02:20:40 GMT
ADD file:3c32f1cd03198e141dd233a7ffd13444157d4150ad917d548f3ee9bf5953ce22 in / 
# Fri, 12 Mar 2021 02:20:41 GMT
CMD ["bash"]
# Fri, 12 Mar 2021 13:34:43 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Fri, 12 Mar 2021 13:34:48 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Fri, 12 Mar 2021 13:34:48 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 12 Mar 2021 13:35:13 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Fri, 12 Mar 2021 13:35:13 GMT
VOLUME [/spiped]
# Fri, 12 Mar 2021 13:35:14 GMT
WORKDIR /spiped
# Fri, 12 Mar 2021 13:35:14 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 12 Mar 2021 13:35:14 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 12 Mar 2021 13:35:14 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:6f28985ad1843afd6fd4fe0b42a30bfab63c27d302362e7341e3316e8ba25ced`  
		Last Modified: Fri, 12 Mar 2021 02:26:11 GMT  
		Size: 27.1 MB (27101001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f47a7b37f3c4e528ff97e5decf3ec7f0f82137d90195c99d3fe65b624ca58fd`  
		Last Modified: Fri, 12 Mar 2021 13:35:54 GMT  
		Size: 1.7 KB (1732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e4ec8344be05d9a5973c107aaf4e4cf134ba0065ba7d21299b2a6e1bb25c514`  
		Last Modified: Fri, 12 Mar 2021 13:35:54 GMT  
		Size: 2.1 MB (2128360 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2b9fc3b146c01478f36950913fdf41df19eea49b156804c28887e9f174b295c`  
		Last Modified: Fri, 12 Mar 2021 13:35:56 GMT  
		Size: 7.0 MB (7037267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bb08069f68a0c759772577589709386d06dea228eaec0950fe149dd7650cc0d`  
		Last Modified: Fri, 12 Mar 2021 13:35:54 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6172a7d7369794ee94aa0835f18b712095f912fa4d72e79d8194dbc44ec7eb9d`  
		Last Modified: Fri, 12 Mar 2021 13:35:54 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; arm variant v5

```console
$ docker pull spiped@sha256:a1859deb50255891bcc3c7a0d51355f4f70c6edfe53681e7ef9b5f7c5176e954
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.2 MB (32167605 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2d0a64bf564abffe8a63869d6aa971922106895f4b214fc7169fa59e36c3ee08`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 26 Mar 2021 07:51:46 GMT
ADD file:3dd25698bf1578e8580b2f437a2199bfc3b1818480b874d73622357e955a091f in / 
# Fri, 26 Mar 2021 07:51:48 GMT
CMD ["bash"]
# Fri, 26 Mar 2021 18:25:23 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Fri, 26 Mar 2021 18:25:35 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Fri, 26 Mar 2021 18:25:36 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 26 Mar 2021 18:26:34 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Fri, 26 Mar 2021 18:26:35 GMT
VOLUME [/spiped]
# Fri, 26 Mar 2021 18:26:36 GMT
WORKDIR /spiped
# Fri, 26 Mar 2021 18:26:37 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 26 Mar 2021 18:26:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 26 Mar 2021 18:26:39 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:997e59852ec0e1a23e4a179db14793947d60390c392ce15abc0f811e797c49ca`  
		Last Modified: Fri, 26 Mar 2021 08:00:22 GMT  
		Size: 24.8 MB (24846159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d845bf35fa4e16c567b254de98a71d1e4e1f5abfecc37f18041fc0ad9ac367d0`  
		Last Modified: Fri, 26 Mar 2021 18:26:57 GMT  
		Size: 1.7 KB (1728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99392226a8fd34bae433f750e9ddade149245f97aed7ab145c5a2d5027ca7b04`  
		Last Modified: Fri, 26 Mar 2021 18:26:57 GMT  
		Size: 1.8 MB (1839291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1365ecba2ae17a6ae4b2804ea9b0487564b2a3ca585c2dc067d772334005706c`  
		Last Modified: Fri, 26 Mar 2021 18:26:59 GMT  
		Size: 5.5 MB (5479955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23e98946787ec7084b445443fa69efa539d294f50a40e4451f6f309e8654b6de`  
		Last Modified: Fri, 26 Mar 2021 18:26:57 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9323331d38da7c134c92cc01ac4d70bd80866d063ce6c830123cd5642c48a5c1`  
		Last Modified: Fri, 26 Mar 2021 18:26:57 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; arm variant v7

```console
$ docker pull spiped@sha256:44b3d70bc67d9e79a0419fc5a58d5f75c2346b6b91c850eb8022d695c86d6dc0
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.8 MB (29756566 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c089b8e65d7c3f6294c9228488e4f6a557c3953b0c0bf77c853af5a8bbe4c8dc`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 12 Mar 2021 02:00:12 GMT
ADD file:123da9848f87c8ed4c5122a104b8650564c09767725916f822def7b645a019f1 in / 
# Fri, 12 Mar 2021 02:00:14 GMT
CMD ["bash"]
# Fri, 12 Mar 2021 18:06:58 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Fri, 12 Mar 2021 18:07:07 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Fri, 12 Mar 2021 18:07:08 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 12 Mar 2021 18:07:54 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Fri, 12 Mar 2021 18:07:56 GMT
VOLUME [/spiped]
# Fri, 12 Mar 2021 18:07:57 GMT
WORKDIR /spiped
# Fri, 12 Mar 2021 18:07:59 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 12 Mar 2021 18:08:00 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 12 Mar 2021 18:08:01 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:e12d26f75fe8b7fd14712965ff5178762227d07d2151bb35fa21105ddfc4a14a`  
		Last Modified: Fri, 12 Mar 2021 02:10:28 GMT  
		Size: 22.7 MB (22709467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a72435c8477703e20922f5027fd6568243135941b80e77d47c7dbd306deb7db`  
		Last Modified: Fri, 12 Mar 2021 18:08:30 GMT  
		Size: 1.7 KB (1737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24a18dda64e40f4f3e5a9f9ca31fb7c16865b51ae45cfe5ac2e617eae69cc491`  
		Last Modified: Fri, 12 Mar 2021 18:08:30 GMT  
		Size: 1.8 MB (1759316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53f4ee5438547836415ee455059b8e85b95417a1756c8b483e918d759f168738`  
		Last Modified: Fri, 12 Mar 2021 18:08:32 GMT  
		Size: 5.3 MB (5285580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c3c8111fcdf41439b1a236c436224ce598dded7c6865d854ec18b4f9a55066a`  
		Last Modified: Fri, 12 Mar 2021 18:08:33 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42912a86aee0cc95765faede7cbe55af4057798a132a2122904ff3032149f477`  
		Last Modified: Fri, 12 Mar 2021 18:08:30 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:996a11488350dceb8604e33f1f98f228dfcb4695ca0d70bf95143b1f96dca774
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.8 MB (33771660 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:877033d2e28e782f80c0ce3818b074e662a0b919a33677f21291883e5623c318`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 12 Mar 2021 01:53:53 GMT
ADD file:6130ddc0a939dd72c0614de4aa77de47aa16fe211274bacb31995aa1a0526164 in / 
# Fri, 12 Mar 2021 01:53:56 GMT
CMD ["bash"]
# Fri, 12 Mar 2021 17:40:51 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Fri, 12 Mar 2021 17:40:59 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Fri, 12 Mar 2021 17:41:00 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 12 Mar 2021 17:41:49 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Fri, 12 Mar 2021 17:41:51 GMT
VOLUME [/spiped]
# Fri, 12 Mar 2021 17:41:52 GMT
WORKDIR /spiped
# Fri, 12 Mar 2021 17:41:53 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 12 Mar 2021 17:41:54 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 12 Mar 2021 17:41:55 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:706ee5d0a6b53d9257cbea22d8409fb22c867ab3a001c65f6b8bfd37dace0e58`  
		Last Modified: Fri, 12 Mar 2021 02:01:39 GMT  
		Size: 25.9 MB (25856512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca354c521ef166c95eb0651133c5463b60c4eac376b689c5bcb60986e9646614`  
		Last Modified: Fri, 12 Mar 2021 17:42:23 GMT  
		Size: 1.7 KB (1742 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9ae9f3f5cb127a6f21b277922c584457d48075bfab82aa39f465f1eab493e83`  
		Last Modified: Fri, 12 Mar 2021 17:42:23 GMT  
		Size: 2.0 MB (2007619 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d8e463abc2137a48bc46b91b4d802e93372aac904b001fb2afc6f8499bde098`  
		Last Modified: Fri, 12 Mar 2021 17:42:25 GMT  
		Size: 5.9 MB (5905317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:911bcabad5c4b743e2880b1bef893d4af3f85656bd20931a8067b35b3f7242ec`  
		Last Modified: Fri, 12 Mar 2021 17:42:23 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2994d1820f2d23b01afa44ab9c272d84d2c302cf2b48a6486c4123af5b63403`  
		Last Modified: Fri, 12 Mar 2021 17:42:23 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; 386

```console
$ docker pull spiped@sha256:4dc923ad898759bc3d6fab0372921a04485aeaabdc63decde7af4063d743e298
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.5 MB (41529023 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c50ce465ce8c1a90ec0ce4d52c4e9da147bfaa6b030d3b167bfd7978a376bdf9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 26 Mar 2021 13:53:11 GMT
ADD file:6c7524352aadfb597840d7c62001b10cf663f17dc2752a1bc5ad40b538138432 in / 
# Fri, 26 Mar 2021 13:53:12 GMT
CMD ["bash"]
# Sat, 27 Mar 2021 02:37:06 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Sat, 27 Mar 2021 02:37:11 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Sat, 27 Mar 2021 02:37:11 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Sat, 27 Mar 2021 02:37:38 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Sat, 27 Mar 2021 02:37:39 GMT
VOLUME [/spiped]
# Sat, 27 Mar 2021 02:37:39 GMT
WORKDIR /spiped
# Sat, 27 Mar 2021 02:37:39 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 27 Mar 2021 02:37:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 27 Mar 2021 02:37:40 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:8cd20c3ac698e839ccd9bbdb86bc90efa00779d975e4064809852f86f56d8f3e`  
		Last Modified: Fri, 26 Mar 2021 14:01:40 GMT  
		Size: 27.8 MB (27760999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10a64bde3f02634d1619c75e254b9961b99e6a7efc85fc274622e191406d2fc9`  
		Last Modified: Sat, 27 Mar 2021 02:38:14 GMT  
		Size: 1.7 KB (1732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:897b2ee4d4d2d7adcf310cc6e555b8e238213756205c7063ff7edaae68dcf3aa`  
		Last Modified: Sat, 27 Mar 2021 02:38:15 GMT  
		Size: 2.1 MB (2132610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8871f8a1e0b60f5223ffb9eed20ea1b49d52cd3c8e946accfb3c40ddf83dbbc`  
		Last Modified: Sat, 27 Mar 2021 02:38:17 GMT  
		Size: 11.6 MB (11633213 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afe7c2c6f83bc692c92f33ea153c717a6b73fb3b20e06a52a92c94008f72572a`  
		Last Modified: Sat, 27 Mar 2021 02:38:14 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42bf3b4efa0c3e5627678a36308847efdaec6f832d4d3b410e85288f491da1a2`  
		Last Modified: Sat, 27 Mar 2021 02:38:14 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; mips64le

```console
$ docker pull spiped@sha256:7c7c058360198a6cdf1c0c5de4c7536b662d0aadb492a39eb71da1745ec6ead9
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.9 MB (33903367 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4c2e30091907d1d9785d74152c96711b6ea697670f5b2e51c2fef7e50032815e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 26 Mar 2021 08:09:56 GMT
ADD file:74d504a9a34f47729165ef4ceedc9f0eaa2e91bfb6a24ebfc3ceed0248267a27 in / 
# Fri, 26 Mar 2021 08:09:57 GMT
CMD ["bash"]
# Fri, 26 Mar 2021 18:56:33 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Fri, 26 Mar 2021 18:56:45 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Fri, 26 Mar 2021 18:56:45 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 26 Mar 2021 18:57:53 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Fri, 26 Mar 2021 18:57:54 GMT
VOLUME [/spiped]
# Fri, 26 Mar 2021 18:57:54 GMT
WORKDIR /spiped
# Fri, 26 Mar 2021 18:57:55 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 26 Mar 2021 18:57:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 26 Mar 2021 18:57:55 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:5f863e006c40853ec8c23aa5b7a0e95918001f96878fb45770410ac4df51cf88`  
		Last Modified: Fri, 26 Mar 2021 08:16:29 GMT  
		Size: 25.8 MB (25772487 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:920815f459af869c2bafde850a4833f2c0af39a10540924371f7c810a2740698`  
		Last Modified: Fri, 26 Mar 2021 18:58:20 GMT  
		Size: 1.7 KB (1733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0ecefc467b0208174c90913c171e0635fc983fe0271e56d94814d9365402d9a`  
		Last Modified: Fri, 26 Mar 2021 18:58:21 GMT  
		Size: 1.7 MB (1712436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b946d42bf9e7b59ba6752c87e806b5dfbcaab31bb0b4c62ad64e1106e2806bb5`  
		Last Modified: Fri, 26 Mar 2021 18:58:26 GMT  
		Size: 6.4 MB (6416271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19bca10ef1481bbdde6f3709e04eb5245089e289de05b36095d3c0b7cd7d5a32`  
		Last Modified: Fri, 26 Mar 2021 18:58:20 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fbf9a1588f37aee944ed6e518b80a6c1c787fe4b75da67bfd3b3f191544931e`  
		Last Modified: Fri, 26 Mar 2021 18:58:23 GMT  
		Size: 345.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; ppc64le

```console
$ docker pull spiped@sha256:e122036d98543d87b9208165ec52dbb80182b3995a8fe6f959e114bfceedab05
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.5 MB (39496384 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:16d2afbae5f13389e96b5a75c34b3f3d8779d7bdfdb5b632016a0a7dc8a6bba4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 12 Mar 2021 02:32:43 GMT
ADD file:6a0c0cfa71979cf6fdd859dce1e32582f0e55ed382b9e17b77a2001defc2c9db in / 
# Fri, 12 Mar 2021 02:32:50 GMT
CMD ["bash"]
# Fri, 12 Mar 2021 17:29:17 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Fri, 12 Mar 2021 17:29:37 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Fri, 12 Mar 2021 17:29:40 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 12 Mar 2021 17:33:02 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Fri, 12 Mar 2021 17:33:05 GMT
VOLUME [/spiped]
# Fri, 12 Mar 2021 17:33:15 GMT
WORKDIR /spiped
# Fri, 12 Mar 2021 17:33:17 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 12 Mar 2021 17:33:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 12 Mar 2021 17:33:29 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:1d686056fdac1848f4fd78ba2b335502055ffe98c79619e21d0c2fb7db95257e`  
		Last Modified: Fri, 12 Mar 2021 02:45:35 GMT  
		Size: 30.5 MB (30525728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e82731719cf164c1334090880e51dcdc657bcf76a28356d37ab5d3b29dddb03c`  
		Last Modified: Fri, 12 Mar 2021 17:33:48 GMT  
		Size: 1.7 KB (1737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:078b30e1777b326949f45e26c2edccb9206038fc736257bd267b5de2b0bd2e4c`  
		Last Modified: Fri, 12 Mar 2021 17:33:48 GMT  
		Size: 2.2 MB (2224920 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b723c17a647249606d310a15aed3e35bf407aa07bc6a804c155f9ccb16dd32a`  
		Last Modified: Fri, 12 Mar 2021 17:33:49 GMT  
		Size: 6.7 MB (6743532 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98d16a0a03be990173113dcd300a3a1d3a78851790b9ad337a52548d0b831471`  
		Last Modified: Fri, 12 Mar 2021 17:33:48 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e13c1f1fd23a837927b6a7954e91788f660a1abbbcfad8c58a0ad6829a0efcc7`  
		Last Modified: Fri, 12 Mar 2021 17:33:48 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; s390x

```console
$ docker pull spiped@sha256:12f759b16118c1f0d7e9e94a6b9fb43b6f2eef818e37aa4a77f30b5f3d42d1e3
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.5 MB (33483871 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f9093d4f6f1989a735c83e462a300ec7787a5fc1bfd5733a853b8e7a6c6178f0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 26 Mar 2021 10:53:48 GMT
ADD file:3a3cf2e796c665cae881fb0b8a23a071206531af98c03548ab5a8721b3c67353 in / 
# Fri, 26 Mar 2021 10:53:49 GMT
CMD ["bash"]
# Fri, 26 Mar 2021 16:47:47 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Fri, 26 Mar 2021 16:47:51 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Fri, 26 Mar 2021 16:47:52 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 26 Mar 2021 16:48:21 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Fri, 26 Mar 2021 16:48:22 GMT
VOLUME [/spiped]
# Fri, 26 Mar 2021 16:48:23 GMT
WORKDIR /spiped
# Fri, 26 Mar 2021 16:48:23 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 26 Mar 2021 16:48:23 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 26 Mar 2021 16:48:24 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:a37ca8d63090f0f22441ceecc0af7881a2668336202cf586e841e3d9e06f2f4b`  
		Last Modified: Fri, 26 Mar 2021 10:57:46 GMT  
		Size: 25.7 MB (25716264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9218249b019c346421bbd61020211795c99650c27d1d482109567f5c54d83852`  
		Last Modified: Fri, 26 Mar 2021 16:48:43 GMT  
		Size: 1.7 KB (1738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:960815f9e510f19f5c7d87ed71ad7ee4a2a617b01fa3126deaf13d93c68e6abc`  
		Last Modified: Fri, 26 Mar 2021 16:48:43 GMT  
		Size: 1.8 MB (1821963 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38910ce19f0387b2df268b10b4691bdc33d47d3b4148957276b91ed47e9c6143`  
		Last Modified: Fri, 26 Mar 2021 16:48:44 GMT  
		Size: 5.9 MB (5943433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fc6af6e6cc8e3705de996630edc8234b408062e105fc7913be86eccec68e28e`  
		Last Modified: Fri, 26 Mar 2021 16:48:43 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9279df31dc6bb719879202509a10292d1046cf406b6032ec3bcd331c1782ec52`  
		Last Modified: Fri, 26 Mar 2021 16:48:43 GMT  
		Size: 344.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:1-alpine`

```console
$ docker pull spiped@sha256:19684fbf0023be921667a91a92d2cf6e979393817c9e69f7062aa2bb5bd5d5e1
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
$ docker pull spiped@sha256:7c4d89762c482bcf41a44c8e1f6b3739708632622256e86d68f55f45b0c2745b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (3032740 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2deb36ffdd5ae6e40f8fda35467c81fadf16c835baefec4bf31877250d5f323c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 25 Mar 2021 22:19:32 GMT
ADD file:6b081cabb4b256ee07587d249c4989b5b679375529542b81550a65b6f19f274e in / 
# Thu, 25 Mar 2021 22:19:32 GMT
CMD ["/bin/sh"]
# Fri, 26 Mar 2021 07:47:14 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 26 Mar 2021 07:47:15 GMT
RUN apk add --no-cache libssl1.1
# Fri, 26 Mar 2021 07:47:16 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 26 Mar 2021 07:47:32 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 26 Mar 2021 07:47:32 GMT
VOLUME [/spiped]
# Fri, 26 Mar 2021 07:47:32 GMT
WORKDIR /spiped
# Fri, 26 Mar 2021 07:47:32 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 26 Mar 2021 07:47:33 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 26 Mar 2021 07:47:33 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:9aae54b2144e5b2b00c610f8805128f4f86822e1e52d3714c463744a431f0f4a`  
		Last Modified: Thu, 25 Mar 2021 22:20:18 GMT  
		Size: 2.8 MB (2811681 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d45422fa5d9e33ce619592de1fe51e4e5755f7b1ec8cdcbe3583b8d3c134f359`  
		Last Modified: Fri, 26 Mar 2021 07:47:52 GMT  
		Size: 1.3 KB (1255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6268afa2960420a8e8af65442a79bf113b0c2e517876f7d3eafb9bf6a80ec7b0`  
		Last Modified: Fri, 26 Mar 2021 07:47:52 GMT  
		Size: 7.0 KB (7040 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c07e7b337f3a675b6ff2edcb1e924b887d6a2ada39fface3d935a676df512cd9`  
		Last Modified: Fri, 26 Mar 2021 07:47:52 GMT  
		Size: 212.3 KB (212294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:995e64d8a9fa092d9aa88315bf05bee732152be501021335f35c9fb78e83826c`  
		Last Modified: Fri, 26 Mar 2021 07:47:52 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8d62f73aa1818308c4b15eda57f7955be9df97218b51b60c86cd68454fd9dcf`  
		Last Modified: Fri, 26 Mar 2021 07:47:52 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; arm variant v6

```console
$ docker pull spiped@sha256:da8bf89069f02c44e64a52cd3c311da57833ba52c0dfd401bf5b400bcba42fab
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 MB (2833098 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a6928a48d8b494975b09a73ff31d4ec85bbf1a70eb5240a267316a1495d85c91`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 25 Mar 2021 22:50:09 GMT
ADD file:ca4136238cb9a01d079efd129bccd1470945d7d4320da61373af90645a4b1146 in / 
# Thu, 25 Mar 2021 22:50:28 GMT
CMD ["/bin/sh"]
# Fri, 26 Mar 2021 10:26:08 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 26 Mar 2021 10:26:10 GMT
RUN apk add --no-cache libssl1.1
# Fri, 26 Mar 2021 10:26:11 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 26 Mar 2021 10:26:43 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 26 Mar 2021 10:26:43 GMT
VOLUME [/spiped]
# Fri, 26 Mar 2021 10:26:44 GMT
WORKDIR /spiped
# Fri, 26 Mar 2021 10:26:45 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 26 Mar 2021 10:26:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 26 Mar 2021 10:26:47 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:bca6a70a54896d072b6919d2ae18d3ef685bc7aed783731f68a4adac0fb93d52`  
		Last Modified: Thu, 25 Mar 2021 22:54:24 GMT  
		Size: 2.6 MB (2622062 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05731027fa533b4ddfd5253b33af7f2e6329040d608478a1cf595d3594e504fd`  
		Last Modified: Fri, 26 Mar 2021 10:27:01 GMT  
		Size: 1.3 KB (1256 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71c330cdff7f6294e87be781c7a86aac39a7e7d2431c24def9e8af9476e2c7da`  
		Last Modified: Fri, 26 Mar 2021 10:27:01 GMT  
		Size: 7.0 KB (7045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7422b39d0efd63a811763e22eb91fcaa0ea348b8a13c6a2afd70562f5cb9bb89`  
		Last Modified: Fri, 26 Mar 2021 10:27:01 GMT  
		Size: 202.3 KB (202264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:641ca636eaa042a42ed82a4494fe4030af9725300ffdc103faa9e12ce1a3816a`  
		Last Modified: Fri, 26 Mar 2021 10:27:01 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a6f1740d604bc2886348af7061a47d9a4343057827419e05f23191d5b911a3a`  
		Last Modified: Fri, 26 Mar 2021 10:27:01 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; arm variant v7

```console
$ docker pull spiped@sha256:14941d01ae5098a1d858bf7e121da3658551e205d024fa897fa7546a9fbd4abc
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 MB (2628316 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4e65ce0598e497561ad9fb8ec4017431a413266afd6380648d27bc30d43d7724`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 25 Mar 2021 22:05:53 GMT
ADD file:44ef6cff6e7d37a67c5846eb792fec65025702c00c56ff96801ac79bf81b0cc3 in / 
# Thu, 25 Mar 2021 22:05:55 GMT
CMD ["/bin/sh"]
# Fri, 26 Mar 2021 04:44:58 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 26 Mar 2021 04:45:04 GMT
RUN apk add --no-cache libssl1.1
# Fri, 26 Mar 2021 04:45:07 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 26 Mar 2021 04:45:42 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 26 Mar 2021 04:45:44 GMT
VOLUME [/spiped]
# Fri, 26 Mar 2021 04:45:46 GMT
WORKDIR /spiped
# Fri, 26 Mar 2021 04:45:47 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 26 Mar 2021 04:45:49 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 26 Mar 2021 04:45:51 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:6c1162af251f0d5ab4945f8506f3265b86d0a03cda37f703c2446a71a233bc20`  
		Last Modified: Thu, 25 Mar 2021 22:07:21 GMT  
		Size: 2.4 MB (2423999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:667f803c1b4052f1f926ae983925d213e0f3558398d4ee3c98e4454d329242cf`  
		Last Modified: Fri, 26 Mar 2021 04:46:12 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7743a5f52834665622361e9a9e693e527cf4038145e1a90cd0a1dfaf2079ac2`  
		Last Modified: Fri, 26 Mar 2021 04:46:12 GMT  
		Size: 7.0 KB (7047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f12109ee1cfc25e39ff0122e6f7b4675b1a18881b88bc8bd654e817b168367c`  
		Last Modified: Fri, 26 Mar 2021 04:46:12 GMT  
		Size: 195.5 KB (195542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e222321da5649854e89f7f9bce7e2b10e9a007e928f0d2bb8d638b29c06d77a6`  
		Last Modified: Fri, 26 Mar 2021 04:46:12 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c42d1c3a4a5b0fd44807df70c5e43af939f6cbe058af4a40acf38192c579c27`  
		Last Modified: Fri, 26 Mar 2021 04:46:12 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:61bd801aefe1449a09ff4878790de0abc5e7c14eb03e7f5c02942a1d5012e7f4
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 MB (2925134 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f9480900df457045488fe844eae0ef1a1c77f40752471d5a8045b4e8c997ae0f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 25 Mar 2021 22:40:10 GMT
ADD file:8d7431f7e3e42b162a1626e7abf4ef7605146671dccc753d490de6b7fe429261 in / 
# Thu, 25 Mar 2021 22:40:23 GMT
CMD ["/bin/sh"]
# Fri, 26 Mar 2021 12:42:20 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 26 Mar 2021 12:42:23 GMT
RUN apk add --no-cache libssl1.1
# Fri, 26 Mar 2021 12:42:24 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 26 Mar 2021 12:42:55 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 26 Mar 2021 12:42:56 GMT
VOLUME [/spiped]
# Fri, 26 Mar 2021 12:42:57 GMT
WORKDIR /spiped
# Fri, 26 Mar 2021 12:42:58 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 26 Mar 2021 12:43:00 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 26 Mar 2021 12:43:00 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:5ceb5101e3b0d54efb5f18318982508a04b181b4d5ae52b096dd35dea3a006cc`  
		Last Modified: Thu, 25 Mar 2021 22:44:41 GMT  
		Size: 2.7 MB (2711898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afb0697971531870407244187323611295c2a45bc7f9f6d5612a003ed0ff0f94`  
		Last Modified: Fri, 26 Mar 2021 12:43:17 GMT  
		Size: 1.3 KB (1256 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1b8c73fede3ea6cbea819460ad1d16f216421e4fc4ed242874949533b74bca9`  
		Last Modified: Fri, 26 Mar 2021 12:43:17 GMT  
		Size: 7.1 KB (7057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a99d1206487fd426b988ae95bd7fb2335d44e6d2b92c2406aae0a3c0e4d71510`  
		Last Modified: Fri, 26 Mar 2021 12:43:17 GMT  
		Size: 204.4 KB (204450 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d88d549d372a38efe8470d52960f2d06e5561634bbecdbca74659a499d423012`  
		Last Modified: Fri, 26 Mar 2021 12:43:17 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54484df3d81811a2e6bfd6d8714590479e14e5643127c5ad98a5821b1637035b`  
		Last Modified: Fri, 26 Mar 2021 12:43:17 GMT  
		Size: 344.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; 386

```console
$ docker pull spiped@sha256:6d4e4fe6948e5a7992c124e61fa437b6e0413a5bb3401654fb248eb3cb12d114
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.1 MB (3050179 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ed9c19db803961bd8dcd8229779fef2771123c1e74079d8339d813fcec140a2c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 25 Mar 2021 22:38:25 GMT
ADD file:8953415d4b98f486af17a39ba53b38f7262aa590734c18ff9318927e5a705baf in / 
# Thu, 25 Mar 2021 22:38:26 GMT
CMD ["/bin/sh"]
# Fri, 26 Mar 2021 11:35:29 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 26 Mar 2021 11:35:31 GMT
RUN apk add --no-cache libssl1.1
# Fri, 26 Mar 2021 11:35:32 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 26 Mar 2021 11:35:52 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 26 Mar 2021 11:35:53 GMT
VOLUME [/spiped]
# Fri, 26 Mar 2021 11:35:53 GMT
WORKDIR /spiped
# Fri, 26 Mar 2021 11:35:53 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 26 Mar 2021 11:35:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 26 Mar 2021 11:35:54 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:1fbd1c9912b638ce64a4740e3af7a3a03452f8705b8103950d677f1d79ae8164`  
		Last Modified: Thu, 25 Mar 2021 22:39:34 GMT  
		Size: 2.8 MB (2818129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc70e02a3b4bec768000b32f6cd554e24e6c8494cbd013299b945dfba9976453`  
		Last Modified: Fri, 26 Mar 2021 11:36:25 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40be889af3bc0980bb5b61ae0b456dbd90907f154b74b796a26046e96f70c4f6`  
		Last Modified: Fri, 26 Mar 2021 11:36:25 GMT  
		Size: 7.0 KB (7042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16a408cdd7892cb9e528cde840b9bf4c2457e6b9540f7b3eeba4b75bb22d5729`  
		Last Modified: Fri, 26 Mar 2021 11:36:26 GMT  
		Size: 223.3 KB (223278 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02bb962d5a258d79b6a952f2eb3e3c6f8e4497529c9b722d855f051a120a68c0`  
		Last Modified: Fri, 26 Mar 2021 11:36:25 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a76c91539d601c2ba091818f38b8b0b17362626aca4e30ca053825d5b4920cbe`  
		Last Modified: Fri, 26 Mar 2021 11:36:25 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; ppc64le

```console
$ docker pull spiped@sha256:90360f53f918820e5f6a844dee0754fa75b275607dbe5c71293fd0e7af7797c7
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (3042891 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:62f4df11bdbbf450f4e6fbf2b9bd4b57d9432205d415896d1ec7179a79658764`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 25 Mar 2021 22:22:28 GMT
ADD file:f91f8e0aa646cb847f6e210056280f9332382ad2f8d6a8839fd9aa69b81c4a2a in / 
# Thu, 25 Mar 2021 22:22:30 GMT
CMD ["/bin/sh"]
# Fri, 26 Mar 2021 05:46:59 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 26 Mar 2021 05:47:14 GMT
RUN apk add --no-cache libssl1.1
# Fri, 26 Mar 2021 05:47:18 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 26 Mar 2021 05:47:54 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 26 Mar 2021 05:47:57 GMT
VOLUME [/spiped]
# Fri, 26 Mar 2021 05:48:02 GMT
WORKDIR /spiped
# Fri, 26 Mar 2021 05:48:06 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 26 Mar 2021 05:48:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 26 Mar 2021 05:48:15 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:f3b2866c25f0a9167af050d646a7a740ccc88d46e068c90ff28a5c2ec2ee0030`  
		Last Modified: Thu, 25 Mar 2021 22:24:08 GMT  
		Size: 2.8 MB (2813115 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5ade0bad869d6db8a4e76203a6dfe3818480c33c407956be758da40b7da8e87`  
		Last Modified: Fri, 26 Mar 2021 05:48:36 GMT  
		Size: 1.3 KB (1262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6878fc6b1c7c9ff2cb9cd6603daa1608abf9847d920dbc2a975313b81d54d09`  
		Last Modified: Fri, 26 Mar 2021 05:48:36 GMT  
		Size: 7.1 KB (7056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a3e8e86fc5762fedfcc865b9618a77f7c27214bf2068e2bdb0f7151d8964030`  
		Last Modified: Fri, 26 Mar 2021 05:48:36 GMT  
		Size: 221.0 KB (220985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1956adc5bd10550d52ee7f60d1d249008d2ca8b414e697b229923777c89fffae`  
		Last Modified: Fri, 26 Mar 2021 05:48:36 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73dac4482b42db1364dec4448343ae95036dd4f7b02440507ae3e40da8dc0d43`  
		Last Modified: Fri, 26 Mar 2021 05:48:36 GMT  
		Size: 344.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; s390x

```console
$ docker pull spiped@sha256:c1f0c63244642a743f32f026370285292f3dae250a308e6364fc3de8ab05effa
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 MB (2816202 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:40d526ff26ded3a191cd728d6ee4458ac19061aadfef60a349e786aab31ba72c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 25 Mar 2021 22:41:34 GMT
ADD file:44e2c7cd992fc98df702bef7022e0f8c4ee86312c311ab5ae185fd5fc878edf9 in / 
# Thu, 25 Mar 2021 22:41:34 GMT
CMD ["/bin/sh"]
# Thu, 25 Mar 2021 23:56:53 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 25 Mar 2021 23:56:54 GMT
RUN apk add --no-cache libssl1.1
# Thu, 25 Mar 2021 23:56:54 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 25 Mar 2021 23:57:05 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Thu, 25 Mar 2021 23:57:06 GMT
VOLUME [/spiped]
# Thu, 25 Mar 2021 23:57:06 GMT
WORKDIR /spiped
# Thu, 25 Mar 2021 23:57:06 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 25 Mar 2021 23:57:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 25 Mar 2021 23:57:07 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:a266c0a9554add02ea09a46b8584cb36b7f606b7b4398b9ad7369f899f8360df`  
		Last Modified: Thu, 25 Mar 2021 22:42:07 GMT  
		Size: 2.6 MB (2602387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d211148772ab04d0ac7d6a254412fe1f42c1e2e7015b60b873a95da6f14a452`  
		Last Modified: Thu, 25 Mar 2021 23:57:22 GMT  
		Size: 1.3 KB (1254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9963e2f655c56703f1a6c0ddfe5ddd34f7f2725e4b4dadfe50a44dccb3fabbef`  
		Last Modified: Thu, 25 Mar 2021 23:57:22 GMT  
		Size: 7.1 KB (7052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bd16cb6da0cae4c5ecfe500cf635456f5c13193987be355c858e78a57bf1150`  
		Last Modified: Thu, 25 Mar 2021 23:57:22 GMT  
		Size: 205.0 KB (205040 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:463e1d0912abda7c19a7c110819c8a1b49e67d57f21ab80715f4a0ee1664927a`  
		Last Modified: Thu, 25 Mar 2021 23:57:22 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48866150c20dea94d44784f072b65bdf6f2292cc61d11de364bbe2d47f21ecce`  
		Last Modified: Thu, 25 Mar 2021 23:57:22 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:1.6`

```console
$ docker pull spiped@sha256:de60f1e86120845dfc5fc566e992ac2528bab5092551860ff597aaa498ba6d12
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
$ docker pull spiped@sha256:cf4b9920b3942ecc606b6251cd4eb1bd48f98354d8e022b3f6307e507a32a3eb
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.3 MB (36268832 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:57285b121dc86ae46a0c0ce8c6f60015ae52e9e52103a25f3f7e0bee876c9013`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 12 Mar 2021 02:20:40 GMT
ADD file:3c32f1cd03198e141dd233a7ffd13444157d4150ad917d548f3ee9bf5953ce22 in / 
# Fri, 12 Mar 2021 02:20:41 GMT
CMD ["bash"]
# Fri, 12 Mar 2021 13:34:43 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Fri, 12 Mar 2021 13:34:48 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Fri, 12 Mar 2021 13:34:48 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 12 Mar 2021 13:35:13 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Fri, 12 Mar 2021 13:35:13 GMT
VOLUME [/spiped]
# Fri, 12 Mar 2021 13:35:14 GMT
WORKDIR /spiped
# Fri, 12 Mar 2021 13:35:14 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 12 Mar 2021 13:35:14 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 12 Mar 2021 13:35:14 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:6f28985ad1843afd6fd4fe0b42a30bfab63c27d302362e7341e3316e8ba25ced`  
		Last Modified: Fri, 12 Mar 2021 02:26:11 GMT  
		Size: 27.1 MB (27101001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f47a7b37f3c4e528ff97e5decf3ec7f0f82137d90195c99d3fe65b624ca58fd`  
		Last Modified: Fri, 12 Mar 2021 13:35:54 GMT  
		Size: 1.7 KB (1732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e4ec8344be05d9a5973c107aaf4e4cf134ba0065ba7d21299b2a6e1bb25c514`  
		Last Modified: Fri, 12 Mar 2021 13:35:54 GMT  
		Size: 2.1 MB (2128360 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2b9fc3b146c01478f36950913fdf41df19eea49b156804c28887e9f174b295c`  
		Last Modified: Fri, 12 Mar 2021 13:35:56 GMT  
		Size: 7.0 MB (7037267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bb08069f68a0c759772577589709386d06dea228eaec0950fe149dd7650cc0d`  
		Last Modified: Fri, 12 Mar 2021 13:35:54 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6172a7d7369794ee94aa0835f18b712095f912fa4d72e79d8194dbc44ec7eb9d`  
		Last Modified: Fri, 12 Mar 2021 13:35:54 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; arm variant v5

```console
$ docker pull spiped@sha256:a1859deb50255891bcc3c7a0d51355f4f70c6edfe53681e7ef9b5f7c5176e954
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.2 MB (32167605 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2d0a64bf564abffe8a63869d6aa971922106895f4b214fc7169fa59e36c3ee08`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 26 Mar 2021 07:51:46 GMT
ADD file:3dd25698bf1578e8580b2f437a2199bfc3b1818480b874d73622357e955a091f in / 
# Fri, 26 Mar 2021 07:51:48 GMT
CMD ["bash"]
# Fri, 26 Mar 2021 18:25:23 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Fri, 26 Mar 2021 18:25:35 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Fri, 26 Mar 2021 18:25:36 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 26 Mar 2021 18:26:34 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Fri, 26 Mar 2021 18:26:35 GMT
VOLUME [/spiped]
# Fri, 26 Mar 2021 18:26:36 GMT
WORKDIR /spiped
# Fri, 26 Mar 2021 18:26:37 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 26 Mar 2021 18:26:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 26 Mar 2021 18:26:39 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:997e59852ec0e1a23e4a179db14793947d60390c392ce15abc0f811e797c49ca`  
		Last Modified: Fri, 26 Mar 2021 08:00:22 GMT  
		Size: 24.8 MB (24846159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d845bf35fa4e16c567b254de98a71d1e4e1f5abfecc37f18041fc0ad9ac367d0`  
		Last Modified: Fri, 26 Mar 2021 18:26:57 GMT  
		Size: 1.7 KB (1728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99392226a8fd34bae433f750e9ddade149245f97aed7ab145c5a2d5027ca7b04`  
		Last Modified: Fri, 26 Mar 2021 18:26:57 GMT  
		Size: 1.8 MB (1839291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1365ecba2ae17a6ae4b2804ea9b0487564b2a3ca585c2dc067d772334005706c`  
		Last Modified: Fri, 26 Mar 2021 18:26:59 GMT  
		Size: 5.5 MB (5479955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23e98946787ec7084b445443fa69efa539d294f50a40e4451f6f309e8654b6de`  
		Last Modified: Fri, 26 Mar 2021 18:26:57 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9323331d38da7c134c92cc01ac4d70bd80866d063ce6c830123cd5642c48a5c1`  
		Last Modified: Fri, 26 Mar 2021 18:26:57 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; arm variant v7

```console
$ docker pull spiped@sha256:44b3d70bc67d9e79a0419fc5a58d5f75c2346b6b91c850eb8022d695c86d6dc0
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.8 MB (29756566 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c089b8e65d7c3f6294c9228488e4f6a557c3953b0c0bf77c853af5a8bbe4c8dc`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 12 Mar 2021 02:00:12 GMT
ADD file:123da9848f87c8ed4c5122a104b8650564c09767725916f822def7b645a019f1 in / 
# Fri, 12 Mar 2021 02:00:14 GMT
CMD ["bash"]
# Fri, 12 Mar 2021 18:06:58 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Fri, 12 Mar 2021 18:07:07 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Fri, 12 Mar 2021 18:07:08 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 12 Mar 2021 18:07:54 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Fri, 12 Mar 2021 18:07:56 GMT
VOLUME [/spiped]
# Fri, 12 Mar 2021 18:07:57 GMT
WORKDIR /spiped
# Fri, 12 Mar 2021 18:07:59 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 12 Mar 2021 18:08:00 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 12 Mar 2021 18:08:01 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:e12d26f75fe8b7fd14712965ff5178762227d07d2151bb35fa21105ddfc4a14a`  
		Last Modified: Fri, 12 Mar 2021 02:10:28 GMT  
		Size: 22.7 MB (22709467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a72435c8477703e20922f5027fd6568243135941b80e77d47c7dbd306deb7db`  
		Last Modified: Fri, 12 Mar 2021 18:08:30 GMT  
		Size: 1.7 KB (1737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24a18dda64e40f4f3e5a9f9ca31fb7c16865b51ae45cfe5ac2e617eae69cc491`  
		Last Modified: Fri, 12 Mar 2021 18:08:30 GMT  
		Size: 1.8 MB (1759316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53f4ee5438547836415ee455059b8e85b95417a1756c8b483e918d759f168738`  
		Last Modified: Fri, 12 Mar 2021 18:08:32 GMT  
		Size: 5.3 MB (5285580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c3c8111fcdf41439b1a236c436224ce598dded7c6865d854ec18b4f9a55066a`  
		Last Modified: Fri, 12 Mar 2021 18:08:33 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42912a86aee0cc95765faede7cbe55af4057798a132a2122904ff3032149f477`  
		Last Modified: Fri, 12 Mar 2021 18:08:30 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:996a11488350dceb8604e33f1f98f228dfcb4695ca0d70bf95143b1f96dca774
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.8 MB (33771660 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:877033d2e28e782f80c0ce3818b074e662a0b919a33677f21291883e5623c318`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 12 Mar 2021 01:53:53 GMT
ADD file:6130ddc0a939dd72c0614de4aa77de47aa16fe211274bacb31995aa1a0526164 in / 
# Fri, 12 Mar 2021 01:53:56 GMT
CMD ["bash"]
# Fri, 12 Mar 2021 17:40:51 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Fri, 12 Mar 2021 17:40:59 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Fri, 12 Mar 2021 17:41:00 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 12 Mar 2021 17:41:49 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Fri, 12 Mar 2021 17:41:51 GMT
VOLUME [/spiped]
# Fri, 12 Mar 2021 17:41:52 GMT
WORKDIR /spiped
# Fri, 12 Mar 2021 17:41:53 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 12 Mar 2021 17:41:54 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 12 Mar 2021 17:41:55 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:706ee5d0a6b53d9257cbea22d8409fb22c867ab3a001c65f6b8bfd37dace0e58`  
		Last Modified: Fri, 12 Mar 2021 02:01:39 GMT  
		Size: 25.9 MB (25856512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca354c521ef166c95eb0651133c5463b60c4eac376b689c5bcb60986e9646614`  
		Last Modified: Fri, 12 Mar 2021 17:42:23 GMT  
		Size: 1.7 KB (1742 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9ae9f3f5cb127a6f21b277922c584457d48075bfab82aa39f465f1eab493e83`  
		Last Modified: Fri, 12 Mar 2021 17:42:23 GMT  
		Size: 2.0 MB (2007619 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d8e463abc2137a48bc46b91b4d802e93372aac904b001fb2afc6f8499bde098`  
		Last Modified: Fri, 12 Mar 2021 17:42:25 GMT  
		Size: 5.9 MB (5905317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:911bcabad5c4b743e2880b1bef893d4af3f85656bd20931a8067b35b3f7242ec`  
		Last Modified: Fri, 12 Mar 2021 17:42:23 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2994d1820f2d23b01afa44ab9c272d84d2c302cf2b48a6486c4123af5b63403`  
		Last Modified: Fri, 12 Mar 2021 17:42:23 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; 386

```console
$ docker pull spiped@sha256:4dc923ad898759bc3d6fab0372921a04485aeaabdc63decde7af4063d743e298
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.5 MB (41529023 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c50ce465ce8c1a90ec0ce4d52c4e9da147bfaa6b030d3b167bfd7978a376bdf9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 26 Mar 2021 13:53:11 GMT
ADD file:6c7524352aadfb597840d7c62001b10cf663f17dc2752a1bc5ad40b538138432 in / 
# Fri, 26 Mar 2021 13:53:12 GMT
CMD ["bash"]
# Sat, 27 Mar 2021 02:37:06 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Sat, 27 Mar 2021 02:37:11 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Sat, 27 Mar 2021 02:37:11 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Sat, 27 Mar 2021 02:37:38 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Sat, 27 Mar 2021 02:37:39 GMT
VOLUME [/spiped]
# Sat, 27 Mar 2021 02:37:39 GMT
WORKDIR /spiped
# Sat, 27 Mar 2021 02:37:39 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 27 Mar 2021 02:37:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 27 Mar 2021 02:37:40 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:8cd20c3ac698e839ccd9bbdb86bc90efa00779d975e4064809852f86f56d8f3e`  
		Last Modified: Fri, 26 Mar 2021 14:01:40 GMT  
		Size: 27.8 MB (27760999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10a64bde3f02634d1619c75e254b9961b99e6a7efc85fc274622e191406d2fc9`  
		Last Modified: Sat, 27 Mar 2021 02:38:14 GMT  
		Size: 1.7 KB (1732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:897b2ee4d4d2d7adcf310cc6e555b8e238213756205c7063ff7edaae68dcf3aa`  
		Last Modified: Sat, 27 Mar 2021 02:38:15 GMT  
		Size: 2.1 MB (2132610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8871f8a1e0b60f5223ffb9eed20ea1b49d52cd3c8e946accfb3c40ddf83dbbc`  
		Last Modified: Sat, 27 Mar 2021 02:38:17 GMT  
		Size: 11.6 MB (11633213 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afe7c2c6f83bc692c92f33ea153c717a6b73fb3b20e06a52a92c94008f72572a`  
		Last Modified: Sat, 27 Mar 2021 02:38:14 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42bf3b4efa0c3e5627678a36308847efdaec6f832d4d3b410e85288f491da1a2`  
		Last Modified: Sat, 27 Mar 2021 02:38:14 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; mips64le

```console
$ docker pull spiped@sha256:7c7c058360198a6cdf1c0c5de4c7536b662d0aadb492a39eb71da1745ec6ead9
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.9 MB (33903367 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4c2e30091907d1d9785d74152c96711b6ea697670f5b2e51c2fef7e50032815e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 26 Mar 2021 08:09:56 GMT
ADD file:74d504a9a34f47729165ef4ceedc9f0eaa2e91bfb6a24ebfc3ceed0248267a27 in / 
# Fri, 26 Mar 2021 08:09:57 GMT
CMD ["bash"]
# Fri, 26 Mar 2021 18:56:33 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Fri, 26 Mar 2021 18:56:45 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Fri, 26 Mar 2021 18:56:45 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 26 Mar 2021 18:57:53 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Fri, 26 Mar 2021 18:57:54 GMT
VOLUME [/spiped]
# Fri, 26 Mar 2021 18:57:54 GMT
WORKDIR /spiped
# Fri, 26 Mar 2021 18:57:55 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 26 Mar 2021 18:57:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 26 Mar 2021 18:57:55 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:5f863e006c40853ec8c23aa5b7a0e95918001f96878fb45770410ac4df51cf88`  
		Last Modified: Fri, 26 Mar 2021 08:16:29 GMT  
		Size: 25.8 MB (25772487 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:920815f459af869c2bafde850a4833f2c0af39a10540924371f7c810a2740698`  
		Last Modified: Fri, 26 Mar 2021 18:58:20 GMT  
		Size: 1.7 KB (1733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0ecefc467b0208174c90913c171e0635fc983fe0271e56d94814d9365402d9a`  
		Last Modified: Fri, 26 Mar 2021 18:58:21 GMT  
		Size: 1.7 MB (1712436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b946d42bf9e7b59ba6752c87e806b5dfbcaab31bb0b4c62ad64e1106e2806bb5`  
		Last Modified: Fri, 26 Mar 2021 18:58:26 GMT  
		Size: 6.4 MB (6416271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19bca10ef1481bbdde6f3709e04eb5245089e289de05b36095d3c0b7cd7d5a32`  
		Last Modified: Fri, 26 Mar 2021 18:58:20 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fbf9a1588f37aee944ed6e518b80a6c1c787fe4b75da67bfd3b3f191544931e`  
		Last Modified: Fri, 26 Mar 2021 18:58:23 GMT  
		Size: 345.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; ppc64le

```console
$ docker pull spiped@sha256:e122036d98543d87b9208165ec52dbb80182b3995a8fe6f959e114bfceedab05
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.5 MB (39496384 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:16d2afbae5f13389e96b5a75c34b3f3d8779d7bdfdb5b632016a0a7dc8a6bba4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 12 Mar 2021 02:32:43 GMT
ADD file:6a0c0cfa71979cf6fdd859dce1e32582f0e55ed382b9e17b77a2001defc2c9db in / 
# Fri, 12 Mar 2021 02:32:50 GMT
CMD ["bash"]
# Fri, 12 Mar 2021 17:29:17 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Fri, 12 Mar 2021 17:29:37 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Fri, 12 Mar 2021 17:29:40 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 12 Mar 2021 17:33:02 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Fri, 12 Mar 2021 17:33:05 GMT
VOLUME [/spiped]
# Fri, 12 Mar 2021 17:33:15 GMT
WORKDIR /spiped
# Fri, 12 Mar 2021 17:33:17 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 12 Mar 2021 17:33:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 12 Mar 2021 17:33:29 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:1d686056fdac1848f4fd78ba2b335502055ffe98c79619e21d0c2fb7db95257e`  
		Last Modified: Fri, 12 Mar 2021 02:45:35 GMT  
		Size: 30.5 MB (30525728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e82731719cf164c1334090880e51dcdc657bcf76a28356d37ab5d3b29dddb03c`  
		Last Modified: Fri, 12 Mar 2021 17:33:48 GMT  
		Size: 1.7 KB (1737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:078b30e1777b326949f45e26c2edccb9206038fc736257bd267b5de2b0bd2e4c`  
		Last Modified: Fri, 12 Mar 2021 17:33:48 GMT  
		Size: 2.2 MB (2224920 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b723c17a647249606d310a15aed3e35bf407aa07bc6a804c155f9ccb16dd32a`  
		Last Modified: Fri, 12 Mar 2021 17:33:49 GMT  
		Size: 6.7 MB (6743532 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98d16a0a03be990173113dcd300a3a1d3a78851790b9ad337a52548d0b831471`  
		Last Modified: Fri, 12 Mar 2021 17:33:48 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e13c1f1fd23a837927b6a7954e91788f660a1abbbcfad8c58a0ad6829a0efcc7`  
		Last Modified: Fri, 12 Mar 2021 17:33:48 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; s390x

```console
$ docker pull spiped@sha256:12f759b16118c1f0d7e9e94a6b9fb43b6f2eef818e37aa4a77f30b5f3d42d1e3
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.5 MB (33483871 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f9093d4f6f1989a735c83e462a300ec7787a5fc1bfd5733a853b8e7a6c6178f0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 26 Mar 2021 10:53:48 GMT
ADD file:3a3cf2e796c665cae881fb0b8a23a071206531af98c03548ab5a8721b3c67353 in / 
# Fri, 26 Mar 2021 10:53:49 GMT
CMD ["bash"]
# Fri, 26 Mar 2021 16:47:47 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Fri, 26 Mar 2021 16:47:51 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Fri, 26 Mar 2021 16:47:52 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 26 Mar 2021 16:48:21 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Fri, 26 Mar 2021 16:48:22 GMT
VOLUME [/spiped]
# Fri, 26 Mar 2021 16:48:23 GMT
WORKDIR /spiped
# Fri, 26 Mar 2021 16:48:23 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 26 Mar 2021 16:48:23 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 26 Mar 2021 16:48:24 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:a37ca8d63090f0f22441ceecc0af7881a2668336202cf586e841e3d9e06f2f4b`  
		Last Modified: Fri, 26 Mar 2021 10:57:46 GMT  
		Size: 25.7 MB (25716264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9218249b019c346421bbd61020211795c99650c27d1d482109567f5c54d83852`  
		Last Modified: Fri, 26 Mar 2021 16:48:43 GMT  
		Size: 1.7 KB (1738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:960815f9e510f19f5c7d87ed71ad7ee4a2a617b01fa3126deaf13d93c68e6abc`  
		Last Modified: Fri, 26 Mar 2021 16:48:43 GMT  
		Size: 1.8 MB (1821963 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38910ce19f0387b2df268b10b4691bdc33d47d3b4148957276b91ed47e9c6143`  
		Last Modified: Fri, 26 Mar 2021 16:48:44 GMT  
		Size: 5.9 MB (5943433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fc6af6e6cc8e3705de996630edc8234b408062e105fc7913be86eccec68e28e`  
		Last Modified: Fri, 26 Mar 2021 16:48:43 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9279df31dc6bb719879202509a10292d1046cf406b6032ec3bcd331c1782ec52`  
		Last Modified: Fri, 26 Mar 2021 16:48:43 GMT  
		Size: 344.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:1.6-alpine`

```console
$ docker pull spiped@sha256:19684fbf0023be921667a91a92d2cf6e979393817c9e69f7062aa2bb5bd5d5e1
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
$ docker pull spiped@sha256:7c4d89762c482bcf41a44c8e1f6b3739708632622256e86d68f55f45b0c2745b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (3032740 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2deb36ffdd5ae6e40f8fda35467c81fadf16c835baefec4bf31877250d5f323c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 25 Mar 2021 22:19:32 GMT
ADD file:6b081cabb4b256ee07587d249c4989b5b679375529542b81550a65b6f19f274e in / 
# Thu, 25 Mar 2021 22:19:32 GMT
CMD ["/bin/sh"]
# Fri, 26 Mar 2021 07:47:14 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 26 Mar 2021 07:47:15 GMT
RUN apk add --no-cache libssl1.1
# Fri, 26 Mar 2021 07:47:16 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 26 Mar 2021 07:47:32 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 26 Mar 2021 07:47:32 GMT
VOLUME [/spiped]
# Fri, 26 Mar 2021 07:47:32 GMT
WORKDIR /spiped
# Fri, 26 Mar 2021 07:47:32 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 26 Mar 2021 07:47:33 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 26 Mar 2021 07:47:33 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:9aae54b2144e5b2b00c610f8805128f4f86822e1e52d3714c463744a431f0f4a`  
		Last Modified: Thu, 25 Mar 2021 22:20:18 GMT  
		Size: 2.8 MB (2811681 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d45422fa5d9e33ce619592de1fe51e4e5755f7b1ec8cdcbe3583b8d3c134f359`  
		Last Modified: Fri, 26 Mar 2021 07:47:52 GMT  
		Size: 1.3 KB (1255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6268afa2960420a8e8af65442a79bf113b0c2e517876f7d3eafb9bf6a80ec7b0`  
		Last Modified: Fri, 26 Mar 2021 07:47:52 GMT  
		Size: 7.0 KB (7040 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c07e7b337f3a675b6ff2edcb1e924b887d6a2ada39fface3d935a676df512cd9`  
		Last Modified: Fri, 26 Mar 2021 07:47:52 GMT  
		Size: 212.3 KB (212294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:995e64d8a9fa092d9aa88315bf05bee732152be501021335f35c9fb78e83826c`  
		Last Modified: Fri, 26 Mar 2021 07:47:52 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8d62f73aa1818308c4b15eda57f7955be9df97218b51b60c86cd68454fd9dcf`  
		Last Modified: Fri, 26 Mar 2021 07:47:52 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; arm variant v6

```console
$ docker pull spiped@sha256:da8bf89069f02c44e64a52cd3c311da57833ba52c0dfd401bf5b400bcba42fab
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 MB (2833098 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a6928a48d8b494975b09a73ff31d4ec85bbf1a70eb5240a267316a1495d85c91`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 25 Mar 2021 22:50:09 GMT
ADD file:ca4136238cb9a01d079efd129bccd1470945d7d4320da61373af90645a4b1146 in / 
# Thu, 25 Mar 2021 22:50:28 GMT
CMD ["/bin/sh"]
# Fri, 26 Mar 2021 10:26:08 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 26 Mar 2021 10:26:10 GMT
RUN apk add --no-cache libssl1.1
# Fri, 26 Mar 2021 10:26:11 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 26 Mar 2021 10:26:43 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 26 Mar 2021 10:26:43 GMT
VOLUME [/spiped]
# Fri, 26 Mar 2021 10:26:44 GMT
WORKDIR /spiped
# Fri, 26 Mar 2021 10:26:45 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 26 Mar 2021 10:26:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 26 Mar 2021 10:26:47 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:bca6a70a54896d072b6919d2ae18d3ef685bc7aed783731f68a4adac0fb93d52`  
		Last Modified: Thu, 25 Mar 2021 22:54:24 GMT  
		Size: 2.6 MB (2622062 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05731027fa533b4ddfd5253b33af7f2e6329040d608478a1cf595d3594e504fd`  
		Last Modified: Fri, 26 Mar 2021 10:27:01 GMT  
		Size: 1.3 KB (1256 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71c330cdff7f6294e87be781c7a86aac39a7e7d2431c24def9e8af9476e2c7da`  
		Last Modified: Fri, 26 Mar 2021 10:27:01 GMT  
		Size: 7.0 KB (7045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7422b39d0efd63a811763e22eb91fcaa0ea348b8a13c6a2afd70562f5cb9bb89`  
		Last Modified: Fri, 26 Mar 2021 10:27:01 GMT  
		Size: 202.3 KB (202264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:641ca636eaa042a42ed82a4494fe4030af9725300ffdc103faa9e12ce1a3816a`  
		Last Modified: Fri, 26 Mar 2021 10:27:01 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a6f1740d604bc2886348af7061a47d9a4343057827419e05f23191d5b911a3a`  
		Last Modified: Fri, 26 Mar 2021 10:27:01 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; arm variant v7

```console
$ docker pull spiped@sha256:14941d01ae5098a1d858bf7e121da3658551e205d024fa897fa7546a9fbd4abc
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 MB (2628316 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4e65ce0598e497561ad9fb8ec4017431a413266afd6380648d27bc30d43d7724`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 25 Mar 2021 22:05:53 GMT
ADD file:44ef6cff6e7d37a67c5846eb792fec65025702c00c56ff96801ac79bf81b0cc3 in / 
# Thu, 25 Mar 2021 22:05:55 GMT
CMD ["/bin/sh"]
# Fri, 26 Mar 2021 04:44:58 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 26 Mar 2021 04:45:04 GMT
RUN apk add --no-cache libssl1.1
# Fri, 26 Mar 2021 04:45:07 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 26 Mar 2021 04:45:42 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 26 Mar 2021 04:45:44 GMT
VOLUME [/spiped]
# Fri, 26 Mar 2021 04:45:46 GMT
WORKDIR /spiped
# Fri, 26 Mar 2021 04:45:47 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 26 Mar 2021 04:45:49 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 26 Mar 2021 04:45:51 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:6c1162af251f0d5ab4945f8506f3265b86d0a03cda37f703c2446a71a233bc20`  
		Last Modified: Thu, 25 Mar 2021 22:07:21 GMT  
		Size: 2.4 MB (2423999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:667f803c1b4052f1f926ae983925d213e0f3558398d4ee3c98e4454d329242cf`  
		Last Modified: Fri, 26 Mar 2021 04:46:12 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7743a5f52834665622361e9a9e693e527cf4038145e1a90cd0a1dfaf2079ac2`  
		Last Modified: Fri, 26 Mar 2021 04:46:12 GMT  
		Size: 7.0 KB (7047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f12109ee1cfc25e39ff0122e6f7b4675b1a18881b88bc8bd654e817b168367c`  
		Last Modified: Fri, 26 Mar 2021 04:46:12 GMT  
		Size: 195.5 KB (195542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e222321da5649854e89f7f9bce7e2b10e9a007e928f0d2bb8d638b29c06d77a6`  
		Last Modified: Fri, 26 Mar 2021 04:46:12 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c42d1c3a4a5b0fd44807df70c5e43af939f6cbe058af4a40acf38192c579c27`  
		Last Modified: Fri, 26 Mar 2021 04:46:12 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:61bd801aefe1449a09ff4878790de0abc5e7c14eb03e7f5c02942a1d5012e7f4
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 MB (2925134 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f9480900df457045488fe844eae0ef1a1c77f40752471d5a8045b4e8c997ae0f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 25 Mar 2021 22:40:10 GMT
ADD file:8d7431f7e3e42b162a1626e7abf4ef7605146671dccc753d490de6b7fe429261 in / 
# Thu, 25 Mar 2021 22:40:23 GMT
CMD ["/bin/sh"]
# Fri, 26 Mar 2021 12:42:20 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 26 Mar 2021 12:42:23 GMT
RUN apk add --no-cache libssl1.1
# Fri, 26 Mar 2021 12:42:24 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 26 Mar 2021 12:42:55 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 26 Mar 2021 12:42:56 GMT
VOLUME [/spiped]
# Fri, 26 Mar 2021 12:42:57 GMT
WORKDIR /spiped
# Fri, 26 Mar 2021 12:42:58 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 26 Mar 2021 12:43:00 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 26 Mar 2021 12:43:00 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:5ceb5101e3b0d54efb5f18318982508a04b181b4d5ae52b096dd35dea3a006cc`  
		Last Modified: Thu, 25 Mar 2021 22:44:41 GMT  
		Size: 2.7 MB (2711898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afb0697971531870407244187323611295c2a45bc7f9f6d5612a003ed0ff0f94`  
		Last Modified: Fri, 26 Mar 2021 12:43:17 GMT  
		Size: 1.3 KB (1256 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1b8c73fede3ea6cbea819460ad1d16f216421e4fc4ed242874949533b74bca9`  
		Last Modified: Fri, 26 Mar 2021 12:43:17 GMT  
		Size: 7.1 KB (7057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a99d1206487fd426b988ae95bd7fb2335d44e6d2b92c2406aae0a3c0e4d71510`  
		Last Modified: Fri, 26 Mar 2021 12:43:17 GMT  
		Size: 204.4 KB (204450 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d88d549d372a38efe8470d52960f2d06e5561634bbecdbca74659a499d423012`  
		Last Modified: Fri, 26 Mar 2021 12:43:17 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54484df3d81811a2e6bfd6d8714590479e14e5643127c5ad98a5821b1637035b`  
		Last Modified: Fri, 26 Mar 2021 12:43:17 GMT  
		Size: 344.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; 386

```console
$ docker pull spiped@sha256:6d4e4fe6948e5a7992c124e61fa437b6e0413a5bb3401654fb248eb3cb12d114
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.1 MB (3050179 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ed9c19db803961bd8dcd8229779fef2771123c1e74079d8339d813fcec140a2c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 25 Mar 2021 22:38:25 GMT
ADD file:8953415d4b98f486af17a39ba53b38f7262aa590734c18ff9318927e5a705baf in / 
# Thu, 25 Mar 2021 22:38:26 GMT
CMD ["/bin/sh"]
# Fri, 26 Mar 2021 11:35:29 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 26 Mar 2021 11:35:31 GMT
RUN apk add --no-cache libssl1.1
# Fri, 26 Mar 2021 11:35:32 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 26 Mar 2021 11:35:52 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 26 Mar 2021 11:35:53 GMT
VOLUME [/spiped]
# Fri, 26 Mar 2021 11:35:53 GMT
WORKDIR /spiped
# Fri, 26 Mar 2021 11:35:53 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 26 Mar 2021 11:35:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 26 Mar 2021 11:35:54 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:1fbd1c9912b638ce64a4740e3af7a3a03452f8705b8103950d677f1d79ae8164`  
		Last Modified: Thu, 25 Mar 2021 22:39:34 GMT  
		Size: 2.8 MB (2818129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc70e02a3b4bec768000b32f6cd554e24e6c8494cbd013299b945dfba9976453`  
		Last Modified: Fri, 26 Mar 2021 11:36:25 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40be889af3bc0980bb5b61ae0b456dbd90907f154b74b796a26046e96f70c4f6`  
		Last Modified: Fri, 26 Mar 2021 11:36:25 GMT  
		Size: 7.0 KB (7042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16a408cdd7892cb9e528cde840b9bf4c2457e6b9540f7b3eeba4b75bb22d5729`  
		Last Modified: Fri, 26 Mar 2021 11:36:26 GMT  
		Size: 223.3 KB (223278 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02bb962d5a258d79b6a952f2eb3e3c6f8e4497529c9b722d855f051a120a68c0`  
		Last Modified: Fri, 26 Mar 2021 11:36:25 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a76c91539d601c2ba091818f38b8b0b17362626aca4e30ca053825d5b4920cbe`  
		Last Modified: Fri, 26 Mar 2021 11:36:25 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; ppc64le

```console
$ docker pull spiped@sha256:90360f53f918820e5f6a844dee0754fa75b275607dbe5c71293fd0e7af7797c7
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (3042891 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:62f4df11bdbbf450f4e6fbf2b9bd4b57d9432205d415896d1ec7179a79658764`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 25 Mar 2021 22:22:28 GMT
ADD file:f91f8e0aa646cb847f6e210056280f9332382ad2f8d6a8839fd9aa69b81c4a2a in / 
# Thu, 25 Mar 2021 22:22:30 GMT
CMD ["/bin/sh"]
# Fri, 26 Mar 2021 05:46:59 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 26 Mar 2021 05:47:14 GMT
RUN apk add --no-cache libssl1.1
# Fri, 26 Mar 2021 05:47:18 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 26 Mar 2021 05:47:54 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 26 Mar 2021 05:47:57 GMT
VOLUME [/spiped]
# Fri, 26 Mar 2021 05:48:02 GMT
WORKDIR /spiped
# Fri, 26 Mar 2021 05:48:06 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 26 Mar 2021 05:48:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 26 Mar 2021 05:48:15 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:f3b2866c25f0a9167af050d646a7a740ccc88d46e068c90ff28a5c2ec2ee0030`  
		Last Modified: Thu, 25 Mar 2021 22:24:08 GMT  
		Size: 2.8 MB (2813115 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5ade0bad869d6db8a4e76203a6dfe3818480c33c407956be758da40b7da8e87`  
		Last Modified: Fri, 26 Mar 2021 05:48:36 GMT  
		Size: 1.3 KB (1262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6878fc6b1c7c9ff2cb9cd6603daa1608abf9847d920dbc2a975313b81d54d09`  
		Last Modified: Fri, 26 Mar 2021 05:48:36 GMT  
		Size: 7.1 KB (7056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a3e8e86fc5762fedfcc865b9618a77f7c27214bf2068e2bdb0f7151d8964030`  
		Last Modified: Fri, 26 Mar 2021 05:48:36 GMT  
		Size: 221.0 KB (220985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1956adc5bd10550d52ee7f60d1d249008d2ca8b414e697b229923777c89fffae`  
		Last Modified: Fri, 26 Mar 2021 05:48:36 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73dac4482b42db1364dec4448343ae95036dd4f7b02440507ae3e40da8dc0d43`  
		Last Modified: Fri, 26 Mar 2021 05:48:36 GMT  
		Size: 344.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; s390x

```console
$ docker pull spiped@sha256:c1f0c63244642a743f32f026370285292f3dae250a308e6364fc3de8ab05effa
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 MB (2816202 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:40d526ff26ded3a191cd728d6ee4458ac19061aadfef60a349e786aab31ba72c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 25 Mar 2021 22:41:34 GMT
ADD file:44e2c7cd992fc98df702bef7022e0f8c4ee86312c311ab5ae185fd5fc878edf9 in / 
# Thu, 25 Mar 2021 22:41:34 GMT
CMD ["/bin/sh"]
# Thu, 25 Mar 2021 23:56:53 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 25 Mar 2021 23:56:54 GMT
RUN apk add --no-cache libssl1.1
# Thu, 25 Mar 2021 23:56:54 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 25 Mar 2021 23:57:05 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Thu, 25 Mar 2021 23:57:06 GMT
VOLUME [/spiped]
# Thu, 25 Mar 2021 23:57:06 GMT
WORKDIR /spiped
# Thu, 25 Mar 2021 23:57:06 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 25 Mar 2021 23:57:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 25 Mar 2021 23:57:07 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:a266c0a9554add02ea09a46b8584cb36b7f606b7b4398b9ad7369f899f8360df`  
		Last Modified: Thu, 25 Mar 2021 22:42:07 GMT  
		Size: 2.6 MB (2602387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d211148772ab04d0ac7d6a254412fe1f42c1e2e7015b60b873a95da6f14a452`  
		Last Modified: Thu, 25 Mar 2021 23:57:22 GMT  
		Size: 1.3 KB (1254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9963e2f655c56703f1a6c0ddfe5ddd34f7f2725e4b4dadfe50a44dccb3fabbef`  
		Last Modified: Thu, 25 Mar 2021 23:57:22 GMT  
		Size: 7.1 KB (7052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bd16cb6da0cae4c5ecfe500cf635456f5c13193987be355c858e78a57bf1150`  
		Last Modified: Thu, 25 Mar 2021 23:57:22 GMT  
		Size: 205.0 KB (205040 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:463e1d0912abda7c19a7c110819c8a1b49e67d57f21ab80715f4a0ee1664927a`  
		Last Modified: Thu, 25 Mar 2021 23:57:22 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48866150c20dea94d44784f072b65bdf6f2292cc61d11de364bbe2d47f21ecce`  
		Last Modified: Thu, 25 Mar 2021 23:57:22 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:1.6.1`

```console
$ docker pull spiped@sha256:de60f1e86120845dfc5fc566e992ac2528bab5092551860ff597aaa498ba6d12
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
$ docker pull spiped@sha256:cf4b9920b3942ecc606b6251cd4eb1bd48f98354d8e022b3f6307e507a32a3eb
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.3 MB (36268832 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:57285b121dc86ae46a0c0ce8c6f60015ae52e9e52103a25f3f7e0bee876c9013`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 12 Mar 2021 02:20:40 GMT
ADD file:3c32f1cd03198e141dd233a7ffd13444157d4150ad917d548f3ee9bf5953ce22 in / 
# Fri, 12 Mar 2021 02:20:41 GMT
CMD ["bash"]
# Fri, 12 Mar 2021 13:34:43 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Fri, 12 Mar 2021 13:34:48 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Fri, 12 Mar 2021 13:34:48 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 12 Mar 2021 13:35:13 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Fri, 12 Mar 2021 13:35:13 GMT
VOLUME [/spiped]
# Fri, 12 Mar 2021 13:35:14 GMT
WORKDIR /spiped
# Fri, 12 Mar 2021 13:35:14 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 12 Mar 2021 13:35:14 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 12 Mar 2021 13:35:14 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:6f28985ad1843afd6fd4fe0b42a30bfab63c27d302362e7341e3316e8ba25ced`  
		Last Modified: Fri, 12 Mar 2021 02:26:11 GMT  
		Size: 27.1 MB (27101001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f47a7b37f3c4e528ff97e5decf3ec7f0f82137d90195c99d3fe65b624ca58fd`  
		Last Modified: Fri, 12 Mar 2021 13:35:54 GMT  
		Size: 1.7 KB (1732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e4ec8344be05d9a5973c107aaf4e4cf134ba0065ba7d21299b2a6e1bb25c514`  
		Last Modified: Fri, 12 Mar 2021 13:35:54 GMT  
		Size: 2.1 MB (2128360 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2b9fc3b146c01478f36950913fdf41df19eea49b156804c28887e9f174b295c`  
		Last Modified: Fri, 12 Mar 2021 13:35:56 GMT  
		Size: 7.0 MB (7037267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bb08069f68a0c759772577589709386d06dea228eaec0950fe149dd7650cc0d`  
		Last Modified: Fri, 12 Mar 2021 13:35:54 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6172a7d7369794ee94aa0835f18b712095f912fa4d72e79d8194dbc44ec7eb9d`  
		Last Modified: Fri, 12 Mar 2021 13:35:54 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1` - linux; arm variant v5

```console
$ docker pull spiped@sha256:a1859deb50255891bcc3c7a0d51355f4f70c6edfe53681e7ef9b5f7c5176e954
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.2 MB (32167605 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2d0a64bf564abffe8a63869d6aa971922106895f4b214fc7169fa59e36c3ee08`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 26 Mar 2021 07:51:46 GMT
ADD file:3dd25698bf1578e8580b2f437a2199bfc3b1818480b874d73622357e955a091f in / 
# Fri, 26 Mar 2021 07:51:48 GMT
CMD ["bash"]
# Fri, 26 Mar 2021 18:25:23 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Fri, 26 Mar 2021 18:25:35 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Fri, 26 Mar 2021 18:25:36 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 26 Mar 2021 18:26:34 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Fri, 26 Mar 2021 18:26:35 GMT
VOLUME [/spiped]
# Fri, 26 Mar 2021 18:26:36 GMT
WORKDIR /spiped
# Fri, 26 Mar 2021 18:26:37 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 26 Mar 2021 18:26:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 26 Mar 2021 18:26:39 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:997e59852ec0e1a23e4a179db14793947d60390c392ce15abc0f811e797c49ca`  
		Last Modified: Fri, 26 Mar 2021 08:00:22 GMT  
		Size: 24.8 MB (24846159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d845bf35fa4e16c567b254de98a71d1e4e1f5abfecc37f18041fc0ad9ac367d0`  
		Last Modified: Fri, 26 Mar 2021 18:26:57 GMT  
		Size: 1.7 KB (1728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99392226a8fd34bae433f750e9ddade149245f97aed7ab145c5a2d5027ca7b04`  
		Last Modified: Fri, 26 Mar 2021 18:26:57 GMT  
		Size: 1.8 MB (1839291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1365ecba2ae17a6ae4b2804ea9b0487564b2a3ca585c2dc067d772334005706c`  
		Last Modified: Fri, 26 Mar 2021 18:26:59 GMT  
		Size: 5.5 MB (5479955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23e98946787ec7084b445443fa69efa539d294f50a40e4451f6f309e8654b6de`  
		Last Modified: Fri, 26 Mar 2021 18:26:57 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9323331d38da7c134c92cc01ac4d70bd80866d063ce6c830123cd5642c48a5c1`  
		Last Modified: Fri, 26 Mar 2021 18:26:57 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1` - linux; arm variant v7

```console
$ docker pull spiped@sha256:44b3d70bc67d9e79a0419fc5a58d5f75c2346b6b91c850eb8022d695c86d6dc0
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.8 MB (29756566 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c089b8e65d7c3f6294c9228488e4f6a557c3953b0c0bf77c853af5a8bbe4c8dc`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 12 Mar 2021 02:00:12 GMT
ADD file:123da9848f87c8ed4c5122a104b8650564c09767725916f822def7b645a019f1 in / 
# Fri, 12 Mar 2021 02:00:14 GMT
CMD ["bash"]
# Fri, 12 Mar 2021 18:06:58 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Fri, 12 Mar 2021 18:07:07 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Fri, 12 Mar 2021 18:07:08 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 12 Mar 2021 18:07:54 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Fri, 12 Mar 2021 18:07:56 GMT
VOLUME [/spiped]
# Fri, 12 Mar 2021 18:07:57 GMT
WORKDIR /spiped
# Fri, 12 Mar 2021 18:07:59 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 12 Mar 2021 18:08:00 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 12 Mar 2021 18:08:01 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:e12d26f75fe8b7fd14712965ff5178762227d07d2151bb35fa21105ddfc4a14a`  
		Last Modified: Fri, 12 Mar 2021 02:10:28 GMT  
		Size: 22.7 MB (22709467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a72435c8477703e20922f5027fd6568243135941b80e77d47c7dbd306deb7db`  
		Last Modified: Fri, 12 Mar 2021 18:08:30 GMT  
		Size: 1.7 KB (1737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24a18dda64e40f4f3e5a9f9ca31fb7c16865b51ae45cfe5ac2e617eae69cc491`  
		Last Modified: Fri, 12 Mar 2021 18:08:30 GMT  
		Size: 1.8 MB (1759316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53f4ee5438547836415ee455059b8e85b95417a1756c8b483e918d759f168738`  
		Last Modified: Fri, 12 Mar 2021 18:08:32 GMT  
		Size: 5.3 MB (5285580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c3c8111fcdf41439b1a236c436224ce598dded7c6865d854ec18b4f9a55066a`  
		Last Modified: Fri, 12 Mar 2021 18:08:33 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42912a86aee0cc95765faede7cbe55af4057798a132a2122904ff3032149f477`  
		Last Modified: Fri, 12 Mar 2021 18:08:30 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:996a11488350dceb8604e33f1f98f228dfcb4695ca0d70bf95143b1f96dca774
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.8 MB (33771660 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:877033d2e28e782f80c0ce3818b074e662a0b919a33677f21291883e5623c318`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 12 Mar 2021 01:53:53 GMT
ADD file:6130ddc0a939dd72c0614de4aa77de47aa16fe211274bacb31995aa1a0526164 in / 
# Fri, 12 Mar 2021 01:53:56 GMT
CMD ["bash"]
# Fri, 12 Mar 2021 17:40:51 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Fri, 12 Mar 2021 17:40:59 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Fri, 12 Mar 2021 17:41:00 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 12 Mar 2021 17:41:49 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Fri, 12 Mar 2021 17:41:51 GMT
VOLUME [/spiped]
# Fri, 12 Mar 2021 17:41:52 GMT
WORKDIR /spiped
# Fri, 12 Mar 2021 17:41:53 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 12 Mar 2021 17:41:54 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 12 Mar 2021 17:41:55 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:706ee5d0a6b53d9257cbea22d8409fb22c867ab3a001c65f6b8bfd37dace0e58`  
		Last Modified: Fri, 12 Mar 2021 02:01:39 GMT  
		Size: 25.9 MB (25856512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca354c521ef166c95eb0651133c5463b60c4eac376b689c5bcb60986e9646614`  
		Last Modified: Fri, 12 Mar 2021 17:42:23 GMT  
		Size: 1.7 KB (1742 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9ae9f3f5cb127a6f21b277922c584457d48075bfab82aa39f465f1eab493e83`  
		Last Modified: Fri, 12 Mar 2021 17:42:23 GMT  
		Size: 2.0 MB (2007619 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d8e463abc2137a48bc46b91b4d802e93372aac904b001fb2afc6f8499bde098`  
		Last Modified: Fri, 12 Mar 2021 17:42:25 GMT  
		Size: 5.9 MB (5905317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:911bcabad5c4b743e2880b1bef893d4af3f85656bd20931a8067b35b3f7242ec`  
		Last Modified: Fri, 12 Mar 2021 17:42:23 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2994d1820f2d23b01afa44ab9c272d84d2c302cf2b48a6486c4123af5b63403`  
		Last Modified: Fri, 12 Mar 2021 17:42:23 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1` - linux; 386

```console
$ docker pull spiped@sha256:4dc923ad898759bc3d6fab0372921a04485aeaabdc63decde7af4063d743e298
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.5 MB (41529023 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c50ce465ce8c1a90ec0ce4d52c4e9da147bfaa6b030d3b167bfd7978a376bdf9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 26 Mar 2021 13:53:11 GMT
ADD file:6c7524352aadfb597840d7c62001b10cf663f17dc2752a1bc5ad40b538138432 in / 
# Fri, 26 Mar 2021 13:53:12 GMT
CMD ["bash"]
# Sat, 27 Mar 2021 02:37:06 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Sat, 27 Mar 2021 02:37:11 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Sat, 27 Mar 2021 02:37:11 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Sat, 27 Mar 2021 02:37:38 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Sat, 27 Mar 2021 02:37:39 GMT
VOLUME [/spiped]
# Sat, 27 Mar 2021 02:37:39 GMT
WORKDIR /spiped
# Sat, 27 Mar 2021 02:37:39 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 27 Mar 2021 02:37:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 27 Mar 2021 02:37:40 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:8cd20c3ac698e839ccd9bbdb86bc90efa00779d975e4064809852f86f56d8f3e`  
		Last Modified: Fri, 26 Mar 2021 14:01:40 GMT  
		Size: 27.8 MB (27760999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10a64bde3f02634d1619c75e254b9961b99e6a7efc85fc274622e191406d2fc9`  
		Last Modified: Sat, 27 Mar 2021 02:38:14 GMT  
		Size: 1.7 KB (1732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:897b2ee4d4d2d7adcf310cc6e555b8e238213756205c7063ff7edaae68dcf3aa`  
		Last Modified: Sat, 27 Mar 2021 02:38:15 GMT  
		Size: 2.1 MB (2132610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8871f8a1e0b60f5223ffb9eed20ea1b49d52cd3c8e946accfb3c40ddf83dbbc`  
		Last Modified: Sat, 27 Mar 2021 02:38:17 GMT  
		Size: 11.6 MB (11633213 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afe7c2c6f83bc692c92f33ea153c717a6b73fb3b20e06a52a92c94008f72572a`  
		Last Modified: Sat, 27 Mar 2021 02:38:14 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42bf3b4efa0c3e5627678a36308847efdaec6f832d4d3b410e85288f491da1a2`  
		Last Modified: Sat, 27 Mar 2021 02:38:14 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1` - linux; mips64le

```console
$ docker pull spiped@sha256:7c7c058360198a6cdf1c0c5de4c7536b662d0aadb492a39eb71da1745ec6ead9
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.9 MB (33903367 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4c2e30091907d1d9785d74152c96711b6ea697670f5b2e51c2fef7e50032815e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 26 Mar 2021 08:09:56 GMT
ADD file:74d504a9a34f47729165ef4ceedc9f0eaa2e91bfb6a24ebfc3ceed0248267a27 in / 
# Fri, 26 Mar 2021 08:09:57 GMT
CMD ["bash"]
# Fri, 26 Mar 2021 18:56:33 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Fri, 26 Mar 2021 18:56:45 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Fri, 26 Mar 2021 18:56:45 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 26 Mar 2021 18:57:53 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Fri, 26 Mar 2021 18:57:54 GMT
VOLUME [/spiped]
# Fri, 26 Mar 2021 18:57:54 GMT
WORKDIR /spiped
# Fri, 26 Mar 2021 18:57:55 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 26 Mar 2021 18:57:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 26 Mar 2021 18:57:55 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:5f863e006c40853ec8c23aa5b7a0e95918001f96878fb45770410ac4df51cf88`  
		Last Modified: Fri, 26 Mar 2021 08:16:29 GMT  
		Size: 25.8 MB (25772487 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:920815f459af869c2bafde850a4833f2c0af39a10540924371f7c810a2740698`  
		Last Modified: Fri, 26 Mar 2021 18:58:20 GMT  
		Size: 1.7 KB (1733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0ecefc467b0208174c90913c171e0635fc983fe0271e56d94814d9365402d9a`  
		Last Modified: Fri, 26 Mar 2021 18:58:21 GMT  
		Size: 1.7 MB (1712436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b946d42bf9e7b59ba6752c87e806b5dfbcaab31bb0b4c62ad64e1106e2806bb5`  
		Last Modified: Fri, 26 Mar 2021 18:58:26 GMT  
		Size: 6.4 MB (6416271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19bca10ef1481bbdde6f3709e04eb5245089e289de05b36095d3c0b7cd7d5a32`  
		Last Modified: Fri, 26 Mar 2021 18:58:20 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fbf9a1588f37aee944ed6e518b80a6c1c787fe4b75da67bfd3b3f191544931e`  
		Last Modified: Fri, 26 Mar 2021 18:58:23 GMT  
		Size: 345.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1` - linux; ppc64le

```console
$ docker pull spiped@sha256:e122036d98543d87b9208165ec52dbb80182b3995a8fe6f959e114bfceedab05
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.5 MB (39496384 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:16d2afbae5f13389e96b5a75c34b3f3d8779d7bdfdb5b632016a0a7dc8a6bba4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 12 Mar 2021 02:32:43 GMT
ADD file:6a0c0cfa71979cf6fdd859dce1e32582f0e55ed382b9e17b77a2001defc2c9db in / 
# Fri, 12 Mar 2021 02:32:50 GMT
CMD ["bash"]
# Fri, 12 Mar 2021 17:29:17 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Fri, 12 Mar 2021 17:29:37 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Fri, 12 Mar 2021 17:29:40 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 12 Mar 2021 17:33:02 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Fri, 12 Mar 2021 17:33:05 GMT
VOLUME [/spiped]
# Fri, 12 Mar 2021 17:33:15 GMT
WORKDIR /spiped
# Fri, 12 Mar 2021 17:33:17 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 12 Mar 2021 17:33:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 12 Mar 2021 17:33:29 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:1d686056fdac1848f4fd78ba2b335502055ffe98c79619e21d0c2fb7db95257e`  
		Last Modified: Fri, 12 Mar 2021 02:45:35 GMT  
		Size: 30.5 MB (30525728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e82731719cf164c1334090880e51dcdc657bcf76a28356d37ab5d3b29dddb03c`  
		Last Modified: Fri, 12 Mar 2021 17:33:48 GMT  
		Size: 1.7 KB (1737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:078b30e1777b326949f45e26c2edccb9206038fc736257bd267b5de2b0bd2e4c`  
		Last Modified: Fri, 12 Mar 2021 17:33:48 GMT  
		Size: 2.2 MB (2224920 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b723c17a647249606d310a15aed3e35bf407aa07bc6a804c155f9ccb16dd32a`  
		Last Modified: Fri, 12 Mar 2021 17:33:49 GMT  
		Size: 6.7 MB (6743532 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98d16a0a03be990173113dcd300a3a1d3a78851790b9ad337a52548d0b831471`  
		Last Modified: Fri, 12 Mar 2021 17:33:48 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e13c1f1fd23a837927b6a7954e91788f660a1abbbcfad8c58a0ad6829a0efcc7`  
		Last Modified: Fri, 12 Mar 2021 17:33:48 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1` - linux; s390x

```console
$ docker pull spiped@sha256:12f759b16118c1f0d7e9e94a6b9fb43b6f2eef818e37aa4a77f30b5f3d42d1e3
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.5 MB (33483871 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f9093d4f6f1989a735c83e462a300ec7787a5fc1bfd5733a853b8e7a6c6178f0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 26 Mar 2021 10:53:48 GMT
ADD file:3a3cf2e796c665cae881fb0b8a23a071206531af98c03548ab5a8721b3c67353 in / 
# Fri, 26 Mar 2021 10:53:49 GMT
CMD ["bash"]
# Fri, 26 Mar 2021 16:47:47 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Fri, 26 Mar 2021 16:47:51 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Fri, 26 Mar 2021 16:47:52 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 26 Mar 2021 16:48:21 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Fri, 26 Mar 2021 16:48:22 GMT
VOLUME [/spiped]
# Fri, 26 Mar 2021 16:48:23 GMT
WORKDIR /spiped
# Fri, 26 Mar 2021 16:48:23 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 26 Mar 2021 16:48:23 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 26 Mar 2021 16:48:24 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:a37ca8d63090f0f22441ceecc0af7881a2668336202cf586e841e3d9e06f2f4b`  
		Last Modified: Fri, 26 Mar 2021 10:57:46 GMT  
		Size: 25.7 MB (25716264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9218249b019c346421bbd61020211795c99650c27d1d482109567f5c54d83852`  
		Last Modified: Fri, 26 Mar 2021 16:48:43 GMT  
		Size: 1.7 KB (1738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:960815f9e510f19f5c7d87ed71ad7ee4a2a617b01fa3126deaf13d93c68e6abc`  
		Last Modified: Fri, 26 Mar 2021 16:48:43 GMT  
		Size: 1.8 MB (1821963 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38910ce19f0387b2df268b10b4691bdc33d47d3b4148957276b91ed47e9c6143`  
		Last Modified: Fri, 26 Mar 2021 16:48:44 GMT  
		Size: 5.9 MB (5943433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fc6af6e6cc8e3705de996630edc8234b408062e105fc7913be86eccec68e28e`  
		Last Modified: Fri, 26 Mar 2021 16:48:43 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9279df31dc6bb719879202509a10292d1046cf406b6032ec3bcd331c1782ec52`  
		Last Modified: Fri, 26 Mar 2021 16:48:43 GMT  
		Size: 344.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:1.6.1-alpine`

```console
$ docker pull spiped@sha256:19684fbf0023be921667a91a92d2cf6e979393817c9e69f7062aa2bb5bd5d5e1
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
$ docker pull spiped@sha256:7c4d89762c482bcf41a44c8e1f6b3739708632622256e86d68f55f45b0c2745b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (3032740 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2deb36ffdd5ae6e40f8fda35467c81fadf16c835baefec4bf31877250d5f323c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 25 Mar 2021 22:19:32 GMT
ADD file:6b081cabb4b256ee07587d249c4989b5b679375529542b81550a65b6f19f274e in / 
# Thu, 25 Mar 2021 22:19:32 GMT
CMD ["/bin/sh"]
# Fri, 26 Mar 2021 07:47:14 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 26 Mar 2021 07:47:15 GMT
RUN apk add --no-cache libssl1.1
# Fri, 26 Mar 2021 07:47:16 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 26 Mar 2021 07:47:32 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 26 Mar 2021 07:47:32 GMT
VOLUME [/spiped]
# Fri, 26 Mar 2021 07:47:32 GMT
WORKDIR /spiped
# Fri, 26 Mar 2021 07:47:32 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 26 Mar 2021 07:47:33 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 26 Mar 2021 07:47:33 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:9aae54b2144e5b2b00c610f8805128f4f86822e1e52d3714c463744a431f0f4a`  
		Last Modified: Thu, 25 Mar 2021 22:20:18 GMT  
		Size: 2.8 MB (2811681 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d45422fa5d9e33ce619592de1fe51e4e5755f7b1ec8cdcbe3583b8d3c134f359`  
		Last Modified: Fri, 26 Mar 2021 07:47:52 GMT  
		Size: 1.3 KB (1255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6268afa2960420a8e8af65442a79bf113b0c2e517876f7d3eafb9bf6a80ec7b0`  
		Last Modified: Fri, 26 Mar 2021 07:47:52 GMT  
		Size: 7.0 KB (7040 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c07e7b337f3a675b6ff2edcb1e924b887d6a2ada39fface3d935a676df512cd9`  
		Last Modified: Fri, 26 Mar 2021 07:47:52 GMT  
		Size: 212.3 KB (212294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:995e64d8a9fa092d9aa88315bf05bee732152be501021335f35c9fb78e83826c`  
		Last Modified: Fri, 26 Mar 2021 07:47:52 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8d62f73aa1818308c4b15eda57f7955be9df97218b51b60c86cd68454fd9dcf`  
		Last Modified: Fri, 26 Mar 2021 07:47:52 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1-alpine` - linux; arm variant v6

```console
$ docker pull spiped@sha256:da8bf89069f02c44e64a52cd3c311da57833ba52c0dfd401bf5b400bcba42fab
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 MB (2833098 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a6928a48d8b494975b09a73ff31d4ec85bbf1a70eb5240a267316a1495d85c91`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 25 Mar 2021 22:50:09 GMT
ADD file:ca4136238cb9a01d079efd129bccd1470945d7d4320da61373af90645a4b1146 in / 
# Thu, 25 Mar 2021 22:50:28 GMT
CMD ["/bin/sh"]
# Fri, 26 Mar 2021 10:26:08 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 26 Mar 2021 10:26:10 GMT
RUN apk add --no-cache libssl1.1
# Fri, 26 Mar 2021 10:26:11 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 26 Mar 2021 10:26:43 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 26 Mar 2021 10:26:43 GMT
VOLUME [/spiped]
# Fri, 26 Mar 2021 10:26:44 GMT
WORKDIR /spiped
# Fri, 26 Mar 2021 10:26:45 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 26 Mar 2021 10:26:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 26 Mar 2021 10:26:47 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:bca6a70a54896d072b6919d2ae18d3ef685bc7aed783731f68a4adac0fb93d52`  
		Last Modified: Thu, 25 Mar 2021 22:54:24 GMT  
		Size: 2.6 MB (2622062 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05731027fa533b4ddfd5253b33af7f2e6329040d608478a1cf595d3594e504fd`  
		Last Modified: Fri, 26 Mar 2021 10:27:01 GMT  
		Size: 1.3 KB (1256 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71c330cdff7f6294e87be781c7a86aac39a7e7d2431c24def9e8af9476e2c7da`  
		Last Modified: Fri, 26 Mar 2021 10:27:01 GMT  
		Size: 7.0 KB (7045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7422b39d0efd63a811763e22eb91fcaa0ea348b8a13c6a2afd70562f5cb9bb89`  
		Last Modified: Fri, 26 Mar 2021 10:27:01 GMT  
		Size: 202.3 KB (202264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:641ca636eaa042a42ed82a4494fe4030af9725300ffdc103faa9e12ce1a3816a`  
		Last Modified: Fri, 26 Mar 2021 10:27:01 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a6f1740d604bc2886348af7061a47d9a4343057827419e05f23191d5b911a3a`  
		Last Modified: Fri, 26 Mar 2021 10:27:01 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1-alpine` - linux; arm variant v7

```console
$ docker pull spiped@sha256:14941d01ae5098a1d858bf7e121da3658551e205d024fa897fa7546a9fbd4abc
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 MB (2628316 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4e65ce0598e497561ad9fb8ec4017431a413266afd6380648d27bc30d43d7724`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 25 Mar 2021 22:05:53 GMT
ADD file:44ef6cff6e7d37a67c5846eb792fec65025702c00c56ff96801ac79bf81b0cc3 in / 
# Thu, 25 Mar 2021 22:05:55 GMT
CMD ["/bin/sh"]
# Fri, 26 Mar 2021 04:44:58 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 26 Mar 2021 04:45:04 GMT
RUN apk add --no-cache libssl1.1
# Fri, 26 Mar 2021 04:45:07 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 26 Mar 2021 04:45:42 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 26 Mar 2021 04:45:44 GMT
VOLUME [/spiped]
# Fri, 26 Mar 2021 04:45:46 GMT
WORKDIR /spiped
# Fri, 26 Mar 2021 04:45:47 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 26 Mar 2021 04:45:49 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 26 Mar 2021 04:45:51 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:6c1162af251f0d5ab4945f8506f3265b86d0a03cda37f703c2446a71a233bc20`  
		Last Modified: Thu, 25 Mar 2021 22:07:21 GMT  
		Size: 2.4 MB (2423999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:667f803c1b4052f1f926ae983925d213e0f3558398d4ee3c98e4454d329242cf`  
		Last Modified: Fri, 26 Mar 2021 04:46:12 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7743a5f52834665622361e9a9e693e527cf4038145e1a90cd0a1dfaf2079ac2`  
		Last Modified: Fri, 26 Mar 2021 04:46:12 GMT  
		Size: 7.0 KB (7047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f12109ee1cfc25e39ff0122e6f7b4675b1a18881b88bc8bd654e817b168367c`  
		Last Modified: Fri, 26 Mar 2021 04:46:12 GMT  
		Size: 195.5 KB (195542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e222321da5649854e89f7f9bce7e2b10e9a007e928f0d2bb8d638b29c06d77a6`  
		Last Modified: Fri, 26 Mar 2021 04:46:12 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c42d1c3a4a5b0fd44807df70c5e43af939f6cbe058af4a40acf38192c579c27`  
		Last Modified: Fri, 26 Mar 2021 04:46:12 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1-alpine` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:61bd801aefe1449a09ff4878790de0abc5e7c14eb03e7f5c02942a1d5012e7f4
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 MB (2925134 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f9480900df457045488fe844eae0ef1a1c77f40752471d5a8045b4e8c997ae0f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 25 Mar 2021 22:40:10 GMT
ADD file:8d7431f7e3e42b162a1626e7abf4ef7605146671dccc753d490de6b7fe429261 in / 
# Thu, 25 Mar 2021 22:40:23 GMT
CMD ["/bin/sh"]
# Fri, 26 Mar 2021 12:42:20 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 26 Mar 2021 12:42:23 GMT
RUN apk add --no-cache libssl1.1
# Fri, 26 Mar 2021 12:42:24 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 26 Mar 2021 12:42:55 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 26 Mar 2021 12:42:56 GMT
VOLUME [/spiped]
# Fri, 26 Mar 2021 12:42:57 GMT
WORKDIR /spiped
# Fri, 26 Mar 2021 12:42:58 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 26 Mar 2021 12:43:00 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 26 Mar 2021 12:43:00 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:5ceb5101e3b0d54efb5f18318982508a04b181b4d5ae52b096dd35dea3a006cc`  
		Last Modified: Thu, 25 Mar 2021 22:44:41 GMT  
		Size: 2.7 MB (2711898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afb0697971531870407244187323611295c2a45bc7f9f6d5612a003ed0ff0f94`  
		Last Modified: Fri, 26 Mar 2021 12:43:17 GMT  
		Size: 1.3 KB (1256 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1b8c73fede3ea6cbea819460ad1d16f216421e4fc4ed242874949533b74bca9`  
		Last Modified: Fri, 26 Mar 2021 12:43:17 GMT  
		Size: 7.1 KB (7057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a99d1206487fd426b988ae95bd7fb2335d44e6d2b92c2406aae0a3c0e4d71510`  
		Last Modified: Fri, 26 Mar 2021 12:43:17 GMT  
		Size: 204.4 KB (204450 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d88d549d372a38efe8470d52960f2d06e5561634bbecdbca74659a499d423012`  
		Last Modified: Fri, 26 Mar 2021 12:43:17 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54484df3d81811a2e6bfd6d8714590479e14e5643127c5ad98a5821b1637035b`  
		Last Modified: Fri, 26 Mar 2021 12:43:17 GMT  
		Size: 344.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1-alpine` - linux; 386

```console
$ docker pull spiped@sha256:6d4e4fe6948e5a7992c124e61fa437b6e0413a5bb3401654fb248eb3cb12d114
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.1 MB (3050179 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ed9c19db803961bd8dcd8229779fef2771123c1e74079d8339d813fcec140a2c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 25 Mar 2021 22:38:25 GMT
ADD file:8953415d4b98f486af17a39ba53b38f7262aa590734c18ff9318927e5a705baf in / 
# Thu, 25 Mar 2021 22:38:26 GMT
CMD ["/bin/sh"]
# Fri, 26 Mar 2021 11:35:29 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 26 Mar 2021 11:35:31 GMT
RUN apk add --no-cache libssl1.1
# Fri, 26 Mar 2021 11:35:32 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 26 Mar 2021 11:35:52 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 26 Mar 2021 11:35:53 GMT
VOLUME [/spiped]
# Fri, 26 Mar 2021 11:35:53 GMT
WORKDIR /spiped
# Fri, 26 Mar 2021 11:35:53 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 26 Mar 2021 11:35:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 26 Mar 2021 11:35:54 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:1fbd1c9912b638ce64a4740e3af7a3a03452f8705b8103950d677f1d79ae8164`  
		Last Modified: Thu, 25 Mar 2021 22:39:34 GMT  
		Size: 2.8 MB (2818129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc70e02a3b4bec768000b32f6cd554e24e6c8494cbd013299b945dfba9976453`  
		Last Modified: Fri, 26 Mar 2021 11:36:25 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40be889af3bc0980bb5b61ae0b456dbd90907f154b74b796a26046e96f70c4f6`  
		Last Modified: Fri, 26 Mar 2021 11:36:25 GMT  
		Size: 7.0 KB (7042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16a408cdd7892cb9e528cde840b9bf4c2457e6b9540f7b3eeba4b75bb22d5729`  
		Last Modified: Fri, 26 Mar 2021 11:36:26 GMT  
		Size: 223.3 KB (223278 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02bb962d5a258d79b6a952f2eb3e3c6f8e4497529c9b722d855f051a120a68c0`  
		Last Modified: Fri, 26 Mar 2021 11:36:25 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a76c91539d601c2ba091818f38b8b0b17362626aca4e30ca053825d5b4920cbe`  
		Last Modified: Fri, 26 Mar 2021 11:36:25 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1-alpine` - linux; ppc64le

```console
$ docker pull spiped@sha256:90360f53f918820e5f6a844dee0754fa75b275607dbe5c71293fd0e7af7797c7
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (3042891 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:62f4df11bdbbf450f4e6fbf2b9bd4b57d9432205d415896d1ec7179a79658764`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 25 Mar 2021 22:22:28 GMT
ADD file:f91f8e0aa646cb847f6e210056280f9332382ad2f8d6a8839fd9aa69b81c4a2a in / 
# Thu, 25 Mar 2021 22:22:30 GMT
CMD ["/bin/sh"]
# Fri, 26 Mar 2021 05:46:59 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 26 Mar 2021 05:47:14 GMT
RUN apk add --no-cache libssl1.1
# Fri, 26 Mar 2021 05:47:18 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 26 Mar 2021 05:47:54 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 26 Mar 2021 05:47:57 GMT
VOLUME [/spiped]
# Fri, 26 Mar 2021 05:48:02 GMT
WORKDIR /spiped
# Fri, 26 Mar 2021 05:48:06 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 26 Mar 2021 05:48:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 26 Mar 2021 05:48:15 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:f3b2866c25f0a9167af050d646a7a740ccc88d46e068c90ff28a5c2ec2ee0030`  
		Last Modified: Thu, 25 Mar 2021 22:24:08 GMT  
		Size: 2.8 MB (2813115 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5ade0bad869d6db8a4e76203a6dfe3818480c33c407956be758da40b7da8e87`  
		Last Modified: Fri, 26 Mar 2021 05:48:36 GMT  
		Size: 1.3 KB (1262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6878fc6b1c7c9ff2cb9cd6603daa1608abf9847d920dbc2a975313b81d54d09`  
		Last Modified: Fri, 26 Mar 2021 05:48:36 GMT  
		Size: 7.1 KB (7056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a3e8e86fc5762fedfcc865b9618a77f7c27214bf2068e2bdb0f7151d8964030`  
		Last Modified: Fri, 26 Mar 2021 05:48:36 GMT  
		Size: 221.0 KB (220985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1956adc5bd10550d52ee7f60d1d249008d2ca8b414e697b229923777c89fffae`  
		Last Modified: Fri, 26 Mar 2021 05:48:36 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73dac4482b42db1364dec4448343ae95036dd4f7b02440507ae3e40da8dc0d43`  
		Last Modified: Fri, 26 Mar 2021 05:48:36 GMT  
		Size: 344.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1-alpine` - linux; s390x

```console
$ docker pull spiped@sha256:c1f0c63244642a743f32f026370285292f3dae250a308e6364fc3de8ab05effa
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 MB (2816202 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:40d526ff26ded3a191cd728d6ee4458ac19061aadfef60a349e786aab31ba72c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 25 Mar 2021 22:41:34 GMT
ADD file:44e2c7cd992fc98df702bef7022e0f8c4ee86312c311ab5ae185fd5fc878edf9 in / 
# Thu, 25 Mar 2021 22:41:34 GMT
CMD ["/bin/sh"]
# Thu, 25 Mar 2021 23:56:53 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 25 Mar 2021 23:56:54 GMT
RUN apk add --no-cache libssl1.1
# Thu, 25 Mar 2021 23:56:54 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 25 Mar 2021 23:57:05 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Thu, 25 Mar 2021 23:57:06 GMT
VOLUME [/spiped]
# Thu, 25 Mar 2021 23:57:06 GMT
WORKDIR /spiped
# Thu, 25 Mar 2021 23:57:06 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 25 Mar 2021 23:57:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 25 Mar 2021 23:57:07 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:a266c0a9554add02ea09a46b8584cb36b7f606b7b4398b9ad7369f899f8360df`  
		Last Modified: Thu, 25 Mar 2021 22:42:07 GMT  
		Size: 2.6 MB (2602387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d211148772ab04d0ac7d6a254412fe1f42c1e2e7015b60b873a95da6f14a452`  
		Last Modified: Thu, 25 Mar 2021 23:57:22 GMT  
		Size: 1.3 KB (1254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9963e2f655c56703f1a6c0ddfe5ddd34f7f2725e4b4dadfe50a44dccb3fabbef`  
		Last Modified: Thu, 25 Mar 2021 23:57:22 GMT  
		Size: 7.1 KB (7052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bd16cb6da0cae4c5ecfe500cf635456f5c13193987be355c858e78a57bf1150`  
		Last Modified: Thu, 25 Mar 2021 23:57:22 GMT  
		Size: 205.0 KB (205040 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:463e1d0912abda7c19a7c110819c8a1b49e67d57f21ab80715f4a0ee1664927a`  
		Last Modified: Thu, 25 Mar 2021 23:57:22 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48866150c20dea94d44784f072b65bdf6f2292cc61d11de364bbe2d47f21ecce`  
		Last Modified: Thu, 25 Mar 2021 23:57:22 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:alpine`

```console
$ docker pull spiped@sha256:19684fbf0023be921667a91a92d2cf6e979393817c9e69f7062aa2bb5bd5d5e1
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
$ docker pull spiped@sha256:7c4d89762c482bcf41a44c8e1f6b3739708632622256e86d68f55f45b0c2745b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (3032740 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2deb36ffdd5ae6e40f8fda35467c81fadf16c835baefec4bf31877250d5f323c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 25 Mar 2021 22:19:32 GMT
ADD file:6b081cabb4b256ee07587d249c4989b5b679375529542b81550a65b6f19f274e in / 
# Thu, 25 Mar 2021 22:19:32 GMT
CMD ["/bin/sh"]
# Fri, 26 Mar 2021 07:47:14 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 26 Mar 2021 07:47:15 GMT
RUN apk add --no-cache libssl1.1
# Fri, 26 Mar 2021 07:47:16 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 26 Mar 2021 07:47:32 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 26 Mar 2021 07:47:32 GMT
VOLUME [/spiped]
# Fri, 26 Mar 2021 07:47:32 GMT
WORKDIR /spiped
# Fri, 26 Mar 2021 07:47:32 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 26 Mar 2021 07:47:33 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 26 Mar 2021 07:47:33 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:9aae54b2144e5b2b00c610f8805128f4f86822e1e52d3714c463744a431f0f4a`  
		Last Modified: Thu, 25 Mar 2021 22:20:18 GMT  
		Size: 2.8 MB (2811681 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d45422fa5d9e33ce619592de1fe51e4e5755f7b1ec8cdcbe3583b8d3c134f359`  
		Last Modified: Fri, 26 Mar 2021 07:47:52 GMT  
		Size: 1.3 KB (1255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6268afa2960420a8e8af65442a79bf113b0c2e517876f7d3eafb9bf6a80ec7b0`  
		Last Modified: Fri, 26 Mar 2021 07:47:52 GMT  
		Size: 7.0 KB (7040 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c07e7b337f3a675b6ff2edcb1e924b887d6a2ada39fface3d935a676df512cd9`  
		Last Modified: Fri, 26 Mar 2021 07:47:52 GMT  
		Size: 212.3 KB (212294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:995e64d8a9fa092d9aa88315bf05bee732152be501021335f35c9fb78e83826c`  
		Last Modified: Fri, 26 Mar 2021 07:47:52 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8d62f73aa1818308c4b15eda57f7955be9df97218b51b60c86cd68454fd9dcf`  
		Last Modified: Fri, 26 Mar 2021 07:47:52 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; arm variant v6

```console
$ docker pull spiped@sha256:da8bf89069f02c44e64a52cd3c311da57833ba52c0dfd401bf5b400bcba42fab
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 MB (2833098 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a6928a48d8b494975b09a73ff31d4ec85bbf1a70eb5240a267316a1495d85c91`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 25 Mar 2021 22:50:09 GMT
ADD file:ca4136238cb9a01d079efd129bccd1470945d7d4320da61373af90645a4b1146 in / 
# Thu, 25 Mar 2021 22:50:28 GMT
CMD ["/bin/sh"]
# Fri, 26 Mar 2021 10:26:08 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 26 Mar 2021 10:26:10 GMT
RUN apk add --no-cache libssl1.1
# Fri, 26 Mar 2021 10:26:11 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 26 Mar 2021 10:26:43 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 26 Mar 2021 10:26:43 GMT
VOLUME [/spiped]
# Fri, 26 Mar 2021 10:26:44 GMT
WORKDIR /spiped
# Fri, 26 Mar 2021 10:26:45 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 26 Mar 2021 10:26:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 26 Mar 2021 10:26:47 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:bca6a70a54896d072b6919d2ae18d3ef685bc7aed783731f68a4adac0fb93d52`  
		Last Modified: Thu, 25 Mar 2021 22:54:24 GMT  
		Size: 2.6 MB (2622062 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05731027fa533b4ddfd5253b33af7f2e6329040d608478a1cf595d3594e504fd`  
		Last Modified: Fri, 26 Mar 2021 10:27:01 GMT  
		Size: 1.3 KB (1256 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71c330cdff7f6294e87be781c7a86aac39a7e7d2431c24def9e8af9476e2c7da`  
		Last Modified: Fri, 26 Mar 2021 10:27:01 GMT  
		Size: 7.0 KB (7045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7422b39d0efd63a811763e22eb91fcaa0ea348b8a13c6a2afd70562f5cb9bb89`  
		Last Modified: Fri, 26 Mar 2021 10:27:01 GMT  
		Size: 202.3 KB (202264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:641ca636eaa042a42ed82a4494fe4030af9725300ffdc103faa9e12ce1a3816a`  
		Last Modified: Fri, 26 Mar 2021 10:27:01 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a6f1740d604bc2886348af7061a47d9a4343057827419e05f23191d5b911a3a`  
		Last Modified: Fri, 26 Mar 2021 10:27:01 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; arm variant v7

```console
$ docker pull spiped@sha256:14941d01ae5098a1d858bf7e121da3658551e205d024fa897fa7546a9fbd4abc
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 MB (2628316 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4e65ce0598e497561ad9fb8ec4017431a413266afd6380648d27bc30d43d7724`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 25 Mar 2021 22:05:53 GMT
ADD file:44ef6cff6e7d37a67c5846eb792fec65025702c00c56ff96801ac79bf81b0cc3 in / 
# Thu, 25 Mar 2021 22:05:55 GMT
CMD ["/bin/sh"]
# Fri, 26 Mar 2021 04:44:58 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 26 Mar 2021 04:45:04 GMT
RUN apk add --no-cache libssl1.1
# Fri, 26 Mar 2021 04:45:07 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 26 Mar 2021 04:45:42 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 26 Mar 2021 04:45:44 GMT
VOLUME [/spiped]
# Fri, 26 Mar 2021 04:45:46 GMT
WORKDIR /spiped
# Fri, 26 Mar 2021 04:45:47 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 26 Mar 2021 04:45:49 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 26 Mar 2021 04:45:51 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:6c1162af251f0d5ab4945f8506f3265b86d0a03cda37f703c2446a71a233bc20`  
		Last Modified: Thu, 25 Mar 2021 22:07:21 GMT  
		Size: 2.4 MB (2423999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:667f803c1b4052f1f926ae983925d213e0f3558398d4ee3c98e4454d329242cf`  
		Last Modified: Fri, 26 Mar 2021 04:46:12 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7743a5f52834665622361e9a9e693e527cf4038145e1a90cd0a1dfaf2079ac2`  
		Last Modified: Fri, 26 Mar 2021 04:46:12 GMT  
		Size: 7.0 KB (7047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f12109ee1cfc25e39ff0122e6f7b4675b1a18881b88bc8bd654e817b168367c`  
		Last Modified: Fri, 26 Mar 2021 04:46:12 GMT  
		Size: 195.5 KB (195542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e222321da5649854e89f7f9bce7e2b10e9a007e928f0d2bb8d638b29c06d77a6`  
		Last Modified: Fri, 26 Mar 2021 04:46:12 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c42d1c3a4a5b0fd44807df70c5e43af939f6cbe058af4a40acf38192c579c27`  
		Last Modified: Fri, 26 Mar 2021 04:46:12 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:61bd801aefe1449a09ff4878790de0abc5e7c14eb03e7f5c02942a1d5012e7f4
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 MB (2925134 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f9480900df457045488fe844eae0ef1a1c77f40752471d5a8045b4e8c997ae0f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 25 Mar 2021 22:40:10 GMT
ADD file:8d7431f7e3e42b162a1626e7abf4ef7605146671dccc753d490de6b7fe429261 in / 
# Thu, 25 Mar 2021 22:40:23 GMT
CMD ["/bin/sh"]
# Fri, 26 Mar 2021 12:42:20 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 26 Mar 2021 12:42:23 GMT
RUN apk add --no-cache libssl1.1
# Fri, 26 Mar 2021 12:42:24 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 26 Mar 2021 12:42:55 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 26 Mar 2021 12:42:56 GMT
VOLUME [/spiped]
# Fri, 26 Mar 2021 12:42:57 GMT
WORKDIR /spiped
# Fri, 26 Mar 2021 12:42:58 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 26 Mar 2021 12:43:00 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 26 Mar 2021 12:43:00 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:5ceb5101e3b0d54efb5f18318982508a04b181b4d5ae52b096dd35dea3a006cc`  
		Last Modified: Thu, 25 Mar 2021 22:44:41 GMT  
		Size: 2.7 MB (2711898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afb0697971531870407244187323611295c2a45bc7f9f6d5612a003ed0ff0f94`  
		Last Modified: Fri, 26 Mar 2021 12:43:17 GMT  
		Size: 1.3 KB (1256 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1b8c73fede3ea6cbea819460ad1d16f216421e4fc4ed242874949533b74bca9`  
		Last Modified: Fri, 26 Mar 2021 12:43:17 GMT  
		Size: 7.1 KB (7057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a99d1206487fd426b988ae95bd7fb2335d44e6d2b92c2406aae0a3c0e4d71510`  
		Last Modified: Fri, 26 Mar 2021 12:43:17 GMT  
		Size: 204.4 KB (204450 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d88d549d372a38efe8470d52960f2d06e5561634bbecdbca74659a499d423012`  
		Last Modified: Fri, 26 Mar 2021 12:43:17 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54484df3d81811a2e6bfd6d8714590479e14e5643127c5ad98a5821b1637035b`  
		Last Modified: Fri, 26 Mar 2021 12:43:17 GMT  
		Size: 344.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; 386

```console
$ docker pull spiped@sha256:6d4e4fe6948e5a7992c124e61fa437b6e0413a5bb3401654fb248eb3cb12d114
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.1 MB (3050179 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ed9c19db803961bd8dcd8229779fef2771123c1e74079d8339d813fcec140a2c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 25 Mar 2021 22:38:25 GMT
ADD file:8953415d4b98f486af17a39ba53b38f7262aa590734c18ff9318927e5a705baf in / 
# Thu, 25 Mar 2021 22:38:26 GMT
CMD ["/bin/sh"]
# Fri, 26 Mar 2021 11:35:29 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 26 Mar 2021 11:35:31 GMT
RUN apk add --no-cache libssl1.1
# Fri, 26 Mar 2021 11:35:32 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 26 Mar 2021 11:35:52 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 26 Mar 2021 11:35:53 GMT
VOLUME [/spiped]
# Fri, 26 Mar 2021 11:35:53 GMT
WORKDIR /spiped
# Fri, 26 Mar 2021 11:35:53 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 26 Mar 2021 11:35:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 26 Mar 2021 11:35:54 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:1fbd1c9912b638ce64a4740e3af7a3a03452f8705b8103950d677f1d79ae8164`  
		Last Modified: Thu, 25 Mar 2021 22:39:34 GMT  
		Size: 2.8 MB (2818129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc70e02a3b4bec768000b32f6cd554e24e6c8494cbd013299b945dfba9976453`  
		Last Modified: Fri, 26 Mar 2021 11:36:25 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40be889af3bc0980bb5b61ae0b456dbd90907f154b74b796a26046e96f70c4f6`  
		Last Modified: Fri, 26 Mar 2021 11:36:25 GMT  
		Size: 7.0 KB (7042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16a408cdd7892cb9e528cde840b9bf4c2457e6b9540f7b3eeba4b75bb22d5729`  
		Last Modified: Fri, 26 Mar 2021 11:36:26 GMT  
		Size: 223.3 KB (223278 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02bb962d5a258d79b6a952f2eb3e3c6f8e4497529c9b722d855f051a120a68c0`  
		Last Modified: Fri, 26 Mar 2021 11:36:25 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a76c91539d601c2ba091818f38b8b0b17362626aca4e30ca053825d5b4920cbe`  
		Last Modified: Fri, 26 Mar 2021 11:36:25 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; ppc64le

```console
$ docker pull spiped@sha256:90360f53f918820e5f6a844dee0754fa75b275607dbe5c71293fd0e7af7797c7
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (3042891 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:62f4df11bdbbf450f4e6fbf2b9bd4b57d9432205d415896d1ec7179a79658764`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 25 Mar 2021 22:22:28 GMT
ADD file:f91f8e0aa646cb847f6e210056280f9332382ad2f8d6a8839fd9aa69b81c4a2a in / 
# Thu, 25 Mar 2021 22:22:30 GMT
CMD ["/bin/sh"]
# Fri, 26 Mar 2021 05:46:59 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 26 Mar 2021 05:47:14 GMT
RUN apk add --no-cache libssl1.1
# Fri, 26 Mar 2021 05:47:18 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 26 Mar 2021 05:47:54 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 26 Mar 2021 05:47:57 GMT
VOLUME [/spiped]
# Fri, 26 Mar 2021 05:48:02 GMT
WORKDIR /spiped
# Fri, 26 Mar 2021 05:48:06 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 26 Mar 2021 05:48:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 26 Mar 2021 05:48:15 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:f3b2866c25f0a9167af050d646a7a740ccc88d46e068c90ff28a5c2ec2ee0030`  
		Last Modified: Thu, 25 Mar 2021 22:24:08 GMT  
		Size: 2.8 MB (2813115 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5ade0bad869d6db8a4e76203a6dfe3818480c33c407956be758da40b7da8e87`  
		Last Modified: Fri, 26 Mar 2021 05:48:36 GMT  
		Size: 1.3 KB (1262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6878fc6b1c7c9ff2cb9cd6603daa1608abf9847d920dbc2a975313b81d54d09`  
		Last Modified: Fri, 26 Mar 2021 05:48:36 GMT  
		Size: 7.1 KB (7056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a3e8e86fc5762fedfcc865b9618a77f7c27214bf2068e2bdb0f7151d8964030`  
		Last Modified: Fri, 26 Mar 2021 05:48:36 GMT  
		Size: 221.0 KB (220985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1956adc5bd10550d52ee7f60d1d249008d2ca8b414e697b229923777c89fffae`  
		Last Modified: Fri, 26 Mar 2021 05:48:36 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73dac4482b42db1364dec4448343ae95036dd4f7b02440507ae3e40da8dc0d43`  
		Last Modified: Fri, 26 Mar 2021 05:48:36 GMT  
		Size: 344.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; s390x

```console
$ docker pull spiped@sha256:c1f0c63244642a743f32f026370285292f3dae250a308e6364fc3de8ab05effa
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 MB (2816202 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:40d526ff26ded3a191cd728d6ee4458ac19061aadfef60a349e786aab31ba72c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 25 Mar 2021 22:41:34 GMT
ADD file:44e2c7cd992fc98df702bef7022e0f8c4ee86312c311ab5ae185fd5fc878edf9 in / 
# Thu, 25 Mar 2021 22:41:34 GMT
CMD ["/bin/sh"]
# Thu, 25 Mar 2021 23:56:53 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 25 Mar 2021 23:56:54 GMT
RUN apk add --no-cache libssl1.1
# Thu, 25 Mar 2021 23:56:54 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 25 Mar 2021 23:57:05 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Thu, 25 Mar 2021 23:57:06 GMT
VOLUME [/spiped]
# Thu, 25 Mar 2021 23:57:06 GMT
WORKDIR /spiped
# Thu, 25 Mar 2021 23:57:06 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 25 Mar 2021 23:57:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 25 Mar 2021 23:57:07 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:a266c0a9554add02ea09a46b8584cb36b7f606b7b4398b9ad7369f899f8360df`  
		Last Modified: Thu, 25 Mar 2021 22:42:07 GMT  
		Size: 2.6 MB (2602387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d211148772ab04d0ac7d6a254412fe1f42c1e2e7015b60b873a95da6f14a452`  
		Last Modified: Thu, 25 Mar 2021 23:57:22 GMT  
		Size: 1.3 KB (1254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9963e2f655c56703f1a6c0ddfe5ddd34f7f2725e4b4dadfe50a44dccb3fabbef`  
		Last Modified: Thu, 25 Mar 2021 23:57:22 GMT  
		Size: 7.1 KB (7052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bd16cb6da0cae4c5ecfe500cf635456f5c13193987be355c858e78a57bf1150`  
		Last Modified: Thu, 25 Mar 2021 23:57:22 GMT  
		Size: 205.0 KB (205040 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:463e1d0912abda7c19a7c110819c8a1b49e67d57f21ab80715f4a0ee1664927a`  
		Last Modified: Thu, 25 Mar 2021 23:57:22 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48866150c20dea94d44784f072b65bdf6f2292cc61d11de364bbe2d47f21ecce`  
		Last Modified: Thu, 25 Mar 2021 23:57:22 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:latest`

```console
$ docker pull spiped@sha256:de60f1e86120845dfc5fc566e992ac2528bab5092551860ff597aaa498ba6d12
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
$ docker pull spiped@sha256:cf4b9920b3942ecc606b6251cd4eb1bd48f98354d8e022b3f6307e507a32a3eb
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.3 MB (36268832 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:57285b121dc86ae46a0c0ce8c6f60015ae52e9e52103a25f3f7e0bee876c9013`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 12 Mar 2021 02:20:40 GMT
ADD file:3c32f1cd03198e141dd233a7ffd13444157d4150ad917d548f3ee9bf5953ce22 in / 
# Fri, 12 Mar 2021 02:20:41 GMT
CMD ["bash"]
# Fri, 12 Mar 2021 13:34:43 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Fri, 12 Mar 2021 13:34:48 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Fri, 12 Mar 2021 13:34:48 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 12 Mar 2021 13:35:13 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Fri, 12 Mar 2021 13:35:13 GMT
VOLUME [/spiped]
# Fri, 12 Mar 2021 13:35:14 GMT
WORKDIR /spiped
# Fri, 12 Mar 2021 13:35:14 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 12 Mar 2021 13:35:14 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 12 Mar 2021 13:35:14 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:6f28985ad1843afd6fd4fe0b42a30bfab63c27d302362e7341e3316e8ba25ced`  
		Last Modified: Fri, 12 Mar 2021 02:26:11 GMT  
		Size: 27.1 MB (27101001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f47a7b37f3c4e528ff97e5decf3ec7f0f82137d90195c99d3fe65b624ca58fd`  
		Last Modified: Fri, 12 Mar 2021 13:35:54 GMT  
		Size: 1.7 KB (1732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e4ec8344be05d9a5973c107aaf4e4cf134ba0065ba7d21299b2a6e1bb25c514`  
		Last Modified: Fri, 12 Mar 2021 13:35:54 GMT  
		Size: 2.1 MB (2128360 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2b9fc3b146c01478f36950913fdf41df19eea49b156804c28887e9f174b295c`  
		Last Modified: Fri, 12 Mar 2021 13:35:56 GMT  
		Size: 7.0 MB (7037267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bb08069f68a0c759772577589709386d06dea228eaec0950fe149dd7650cc0d`  
		Last Modified: Fri, 12 Mar 2021 13:35:54 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6172a7d7369794ee94aa0835f18b712095f912fa4d72e79d8194dbc44ec7eb9d`  
		Last Modified: Fri, 12 Mar 2021 13:35:54 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; arm variant v5

```console
$ docker pull spiped@sha256:a1859deb50255891bcc3c7a0d51355f4f70c6edfe53681e7ef9b5f7c5176e954
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.2 MB (32167605 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2d0a64bf564abffe8a63869d6aa971922106895f4b214fc7169fa59e36c3ee08`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 26 Mar 2021 07:51:46 GMT
ADD file:3dd25698bf1578e8580b2f437a2199bfc3b1818480b874d73622357e955a091f in / 
# Fri, 26 Mar 2021 07:51:48 GMT
CMD ["bash"]
# Fri, 26 Mar 2021 18:25:23 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Fri, 26 Mar 2021 18:25:35 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Fri, 26 Mar 2021 18:25:36 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 26 Mar 2021 18:26:34 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Fri, 26 Mar 2021 18:26:35 GMT
VOLUME [/spiped]
# Fri, 26 Mar 2021 18:26:36 GMT
WORKDIR /spiped
# Fri, 26 Mar 2021 18:26:37 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 26 Mar 2021 18:26:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 26 Mar 2021 18:26:39 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:997e59852ec0e1a23e4a179db14793947d60390c392ce15abc0f811e797c49ca`  
		Last Modified: Fri, 26 Mar 2021 08:00:22 GMT  
		Size: 24.8 MB (24846159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d845bf35fa4e16c567b254de98a71d1e4e1f5abfecc37f18041fc0ad9ac367d0`  
		Last Modified: Fri, 26 Mar 2021 18:26:57 GMT  
		Size: 1.7 KB (1728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99392226a8fd34bae433f750e9ddade149245f97aed7ab145c5a2d5027ca7b04`  
		Last Modified: Fri, 26 Mar 2021 18:26:57 GMT  
		Size: 1.8 MB (1839291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1365ecba2ae17a6ae4b2804ea9b0487564b2a3ca585c2dc067d772334005706c`  
		Last Modified: Fri, 26 Mar 2021 18:26:59 GMT  
		Size: 5.5 MB (5479955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23e98946787ec7084b445443fa69efa539d294f50a40e4451f6f309e8654b6de`  
		Last Modified: Fri, 26 Mar 2021 18:26:57 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9323331d38da7c134c92cc01ac4d70bd80866d063ce6c830123cd5642c48a5c1`  
		Last Modified: Fri, 26 Mar 2021 18:26:57 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; arm variant v7

```console
$ docker pull spiped@sha256:44b3d70bc67d9e79a0419fc5a58d5f75c2346b6b91c850eb8022d695c86d6dc0
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.8 MB (29756566 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c089b8e65d7c3f6294c9228488e4f6a557c3953b0c0bf77c853af5a8bbe4c8dc`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 12 Mar 2021 02:00:12 GMT
ADD file:123da9848f87c8ed4c5122a104b8650564c09767725916f822def7b645a019f1 in / 
# Fri, 12 Mar 2021 02:00:14 GMT
CMD ["bash"]
# Fri, 12 Mar 2021 18:06:58 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Fri, 12 Mar 2021 18:07:07 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Fri, 12 Mar 2021 18:07:08 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 12 Mar 2021 18:07:54 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Fri, 12 Mar 2021 18:07:56 GMT
VOLUME [/spiped]
# Fri, 12 Mar 2021 18:07:57 GMT
WORKDIR /spiped
# Fri, 12 Mar 2021 18:07:59 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 12 Mar 2021 18:08:00 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 12 Mar 2021 18:08:01 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:e12d26f75fe8b7fd14712965ff5178762227d07d2151bb35fa21105ddfc4a14a`  
		Last Modified: Fri, 12 Mar 2021 02:10:28 GMT  
		Size: 22.7 MB (22709467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a72435c8477703e20922f5027fd6568243135941b80e77d47c7dbd306deb7db`  
		Last Modified: Fri, 12 Mar 2021 18:08:30 GMT  
		Size: 1.7 KB (1737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24a18dda64e40f4f3e5a9f9ca31fb7c16865b51ae45cfe5ac2e617eae69cc491`  
		Last Modified: Fri, 12 Mar 2021 18:08:30 GMT  
		Size: 1.8 MB (1759316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53f4ee5438547836415ee455059b8e85b95417a1756c8b483e918d759f168738`  
		Last Modified: Fri, 12 Mar 2021 18:08:32 GMT  
		Size: 5.3 MB (5285580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c3c8111fcdf41439b1a236c436224ce598dded7c6865d854ec18b4f9a55066a`  
		Last Modified: Fri, 12 Mar 2021 18:08:33 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42912a86aee0cc95765faede7cbe55af4057798a132a2122904ff3032149f477`  
		Last Modified: Fri, 12 Mar 2021 18:08:30 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:996a11488350dceb8604e33f1f98f228dfcb4695ca0d70bf95143b1f96dca774
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.8 MB (33771660 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:877033d2e28e782f80c0ce3818b074e662a0b919a33677f21291883e5623c318`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 12 Mar 2021 01:53:53 GMT
ADD file:6130ddc0a939dd72c0614de4aa77de47aa16fe211274bacb31995aa1a0526164 in / 
# Fri, 12 Mar 2021 01:53:56 GMT
CMD ["bash"]
# Fri, 12 Mar 2021 17:40:51 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Fri, 12 Mar 2021 17:40:59 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Fri, 12 Mar 2021 17:41:00 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 12 Mar 2021 17:41:49 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Fri, 12 Mar 2021 17:41:51 GMT
VOLUME [/spiped]
# Fri, 12 Mar 2021 17:41:52 GMT
WORKDIR /spiped
# Fri, 12 Mar 2021 17:41:53 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 12 Mar 2021 17:41:54 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 12 Mar 2021 17:41:55 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:706ee5d0a6b53d9257cbea22d8409fb22c867ab3a001c65f6b8bfd37dace0e58`  
		Last Modified: Fri, 12 Mar 2021 02:01:39 GMT  
		Size: 25.9 MB (25856512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca354c521ef166c95eb0651133c5463b60c4eac376b689c5bcb60986e9646614`  
		Last Modified: Fri, 12 Mar 2021 17:42:23 GMT  
		Size: 1.7 KB (1742 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9ae9f3f5cb127a6f21b277922c584457d48075bfab82aa39f465f1eab493e83`  
		Last Modified: Fri, 12 Mar 2021 17:42:23 GMT  
		Size: 2.0 MB (2007619 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d8e463abc2137a48bc46b91b4d802e93372aac904b001fb2afc6f8499bde098`  
		Last Modified: Fri, 12 Mar 2021 17:42:25 GMT  
		Size: 5.9 MB (5905317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:911bcabad5c4b743e2880b1bef893d4af3f85656bd20931a8067b35b3f7242ec`  
		Last Modified: Fri, 12 Mar 2021 17:42:23 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2994d1820f2d23b01afa44ab9c272d84d2c302cf2b48a6486c4123af5b63403`  
		Last Modified: Fri, 12 Mar 2021 17:42:23 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; 386

```console
$ docker pull spiped@sha256:4dc923ad898759bc3d6fab0372921a04485aeaabdc63decde7af4063d743e298
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.5 MB (41529023 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c50ce465ce8c1a90ec0ce4d52c4e9da147bfaa6b030d3b167bfd7978a376bdf9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 26 Mar 2021 13:53:11 GMT
ADD file:6c7524352aadfb597840d7c62001b10cf663f17dc2752a1bc5ad40b538138432 in / 
# Fri, 26 Mar 2021 13:53:12 GMT
CMD ["bash"]
# Sat, 27 Mar 2021 02:37:06 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Sat, 27 Mar 2021 02:37:11 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Sat, 27 Mar 2021 02:37:11 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Sat, 27 Mar 2021 02:37:38 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Sat, 27 Mar 2021 02:37:39 GMT
VOLUME [/spiped]
# Sat, 27 Mar 2021 02:37:39 GMT
WORKDIR /spiped
# Sat, 27 Mar 2021 02:37:39 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 27 Mar 2021 02:37:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 27 Mar 2021 02:37:40 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:8cd20c3ac698e839ccd9bbdb86bc90efa00779d975e4064809852f86f56d8f3e`  
		Last Modified: Fri, 26 Mar 2021 14:01:40 GMT  
		Size: 27.8 MB (27760999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10a64bde3f02634d1619c75e254b9961b99e6a7efc85fc274622e191406d2fc9`  
		Last Modified: Sat, 27 Mar 2021 02:38:14 GMT  
		Size: 1.7 KB (1732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:897b2ee4d4d2d7adcf310cc6e555b8e238213756205c7063ff7edaae68dcf3aa`  
		Last Modified: Sat, 27 Mar 2021 02:38:15 GMT  
		Size: 2.1 MB (2132610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8871f8a1e0b60f5223ffb9eed20ea1b49d52cd3c8e946accfb3c40ddf83dbbc`  
		Last Modified: Sat, 27 Mar 2021 02:38:17 GMT  
		Size: 11.6 MB (11633213 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afe7c2c6f83bc692c92f33ea153c717a6b73fb3b20e06a52a92c94008f72572a`  
		Last Modified: Sat, 27 Mar 2021 02:38:14 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42bf3b4efa0c3e5627678a36308847efdaec6f832d4d3b410e85288f491da1a2`  
		Last Modified: Sat, 27 Mar 2021 02:38:14 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; mips64le

```console
$ docker pull spiped@sha256:7c7c058360198a6cdf1c0c5de4c7536b662d0aadb492a39eb71da1745ec6ead9
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.9 MB (33903367 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4c2e30091907d1d9785d74152c96711b6ea697670f5b2e51c2fef7e50032815e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 26 Mar 2021 08:09:56 GMT
ADD file:74d504a9a34f47729165ef4ceedc9f0eaa2e91bfb6a24ebfc3ceed0248267a27 in / 
# Fri, 26 Mar 2021 08:09:57 GMT
CMD ["bash"]
# Fri, 26 Mar 2021 18:56:33 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Fri, 26 Mar 2021 18:56:45 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Fri, 26 Mar 2021 18:56:45 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 26 Mar 2021 18:57:53 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Fri, 26 Mar 2021 18:57:54 GMT
VOLUME [/spiped]
# Fri, 26 Mar 2021 18:57:54 GMT
WORKDIR /spiped
# Fri, 26 Mar 2021 18:57:55 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 26 Mar 2021 18:57:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 26 Mar 2021 18:57:55 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:5f863e006c40853ec8c23aa5b7a0e95918001f96878fb45770410ac4df51cf88`  
		Last Modified: Fri, 26 Mar 2021 08:16:29 GMT  
		Size: 25.8 MB (25772487 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:920815f459af869c2bafde850a4833f2c0af39a10540924371f7c810a2740698`  
		Last Modified: Fri, 26 Mar 2021 18:58:20 GMT  
		Size: 1.7 KB (1733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0ecefc467b0208174c90913c171e0635fc983fe0271e56d94814d9365402d9a`  
		Last Modified: Fri, 26 Mar 2021 18:58:21 GMT  
		Size: 1.7 MB (1712436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b946d42bf9e7b59ba6752c87e806b5dfbcaab31bb0b4c62ad64e1106e2806bb5`  
		Last Modified: Fri, 26 Mar 2021 18:58:26 GMT  
		Size: 6.4 MB (6416271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19bca10ef1481bbdde6f3709e04eb5245089e289de05b36095d3c0b7cd7d5a32`  
		Last Modified: Fri, 26 Mar 2021 18:58:20 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fbf9a1588f37aee944ed6e518b80a6c1c787fe4b75da67bfd3b3f191544931e`  
		Last Modified: Fri, 26 Mar 2021 18:58:23 GMT  
		Size: 345.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; ppc64le

```console
$ docker pull spiped@sha256:e122036d98543d87b9208165ec52dbb80182b3995a8fe6f959e114bfceedab05
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.5 MB (39496384 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:16d2afbae5f13389e96b5a75c34b3f3d8779d7bdfdb5b632016a0a7dc8a6bba4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 12 Mar 2021 02:32:43 GMT
ADD file:6a0c0cfa71979cf6fdd859dce1e32582f0e55ed382b9e17b77a2001defc2c9db in / 
# Fri, 12 Mar 2021 02:32:50 GMT
CMD ["bash"]
# Fri, 12 Mar 2021 17:29:17 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Fri, 12 Mar 2021 17:29:37 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Fri, 12 Mar 2021 17:29:40 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 12 Mar 2021 17:33:02 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Fri, 12 Mar 2021 17:33:05 GMT
VOLUME [/spiped]
# Fri, 12 Mar 2021 17:33:15 GMT
WORKDIR /spiped
# Fri, 12 Mar 2021 17:33:17 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 12 Mar 2021 17:33:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 12 Mar 2021 17:33:29 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:1d686056fdac1848f4fd78ba2b335502055ffe98c79619e21d0c2fb7db95257e`  
		Last Modified: Fri, 12 Mar 2021 02:45:35 GMT  
		Size: 30.5 MB (30525728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e82731719cf164c1334090880e51dcdc657bcf76a28356d37ab5d3b29dddb03c`  
		Last Modified: Fri, 12 Mar 2021 17:33:48 GMT  
		Size: 1.7 KB (1737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:078b30e1777b326949f45e26c2edccb9206038fc736257bd267b5de2b0bd2e4c`  
		Last Modified: Fri, 12 Mar 2021 17:33:48 GMT  
		Size: 2.2 MB (2224920 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b723c17a647249606d310a15aed3e35bf407aa07bc6a804c155f9ccb16dd32a`  
		Last Modified: Fri, 12 Mar 2021 17:33:49 GMT  
		Size: 6.7 MB (6743532 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98d16a0a03be990173113dcd300a3a1d3a78851790b9ad337a52548d0b831471`  
		Last Modified: Fri, 12 Mar 2021 17:33:48 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e13c1f1fd23a837927b6a7954e91788f660a1abbbcfad8c58a0ad6829a0efcc7`  
		Last Modified: Fri, 12 Mar 2021 17:33:48 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; s390x

```console
$ docker pull spiped@sha256:12f759b16118c1f0d7e9e94a6b9fb43b6f2eef818e37aa4a77f30b5f3d42d1e3
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.5 MB (33483871 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f9093d4f6f1989a735c83e462a300ec7787a5fc1bfd5733a853b8e7a6c6178f0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 26 Mar 2021 10:53:48 GMT
ADD file:3a3cf2e796c665cae881fb0b8a23a071206531af98c03548ab5a8721b3c67353 in / 
# Fri, 26 Mar 2021 10:53:49 GMT
CMD ["bash"]
# Fri, 26 Mar 2021 16:47:47 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Fri, 26 Mar 2021 16:47:51 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Fri, 26 Mar 2021 16:47:52 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 26 Mar 2021 16:48:21 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Fri, 26 Mar 2021 16:48:22 GMT
VOLUME [/spiped]
# Fri, 26 Mar 2021 16:48:23 GMT
WORKDIR /spiped
# Fri, 26 Mar 2021 16:48:23 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 26 Mar 2021 16:48:23 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 26 Mar 2021 16:48:24 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:a37ca8d63090f0f22441ceecc0af7881a2668336202cf586e841e3d9e06f2f4b`  
		Last Modified: Fri, 26 Mar 2021 10:57:46 GMT  
		Size: 25.7 MB (25716264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9218249b019c346421bbd61020211795c99650c27d1d482109567f5c54d83852`  
		Last Modified: Fri, 26 Mar 2021 16:48:43 GMT  
		Size: 1.7 KB (1738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:960815f9e510f19f5c7d87ed71ad7ee4a2a617b01fa3126deaf13d93c68e6abc`  
		Last Modified: Fri, 26 Mar 2021 16:48:43 GMT  
		Size: 1.8 MB (1821963 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38910ce19f0387b2df268b10b4691bdc33d47d3b4148957276b91ed47e9c6143`  
		Last Modified: Fri, 26 Mar 2021 16:48:44 GMT  
		Size: 5.9 MB (5943433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fc6af6e6cc8e3705de996630edc8234b408062e105fc7913be86eccec68e28e`  
		Last Modified: Fri, 26 Mar 2021 16:48:43 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9279df31dc6bb719879202509a10292d1046cf406b6032ec3bcd331c1782ec52`  
		Last Modified: Fri, 26 Mar 2021 16:48:43 GMT  
		Size: 344.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
