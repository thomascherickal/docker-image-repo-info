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
$ docker pull spiped@sha256:f00a200fc1b19303be35892bcaaf6f82dffb6d5afe90d49d3bbfa350c1ae2161
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
$ docker pull spiped@sha256:7be4a2a8c7741dcedad533f936408fce6017373a865914793bbeceb65ac7317c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.2 MB (32167233 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2d2d9655883de89f3593e8c0503223ad9d77ec8ef3b444604cbdbe0bef719dc5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 12 Mar 2021 01:52:27 GMT
ADD file:8e357182800adfe658856515726f1e012cc120349f0f305692cf50282f6d8b7b in / 
# Fri, 12 Mar 2021 01:52:29 GMT
CMD ["bash"]
# Fri, 12 Mar 2021 06:51:44 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Fri, 12 Mar 2021 06:51:54 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Fri, 12 Mar 2021 06:51:55 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 12 Mar 2021 06:52:51 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Fri, 12 Mar 2021 06:52:53 GMT
VOLUME [/spiped]
# Fri, 12 Mar 2021 06:52:54 GMT
WORKDIR /spiped
# Fri, 12 Mar 2021 06:52:55 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 12 Mar 2021 06:52:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 12 Mar 2021 06:52:57 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:9babb1be2e38b3bddad5a4e05bb34173369ae3472c0c0d8668853011cd65969f`  
		Last Modified: Fri, 12 Mar 2021 02:02:01 GMT  
		Size: 24.8 MB (24845925 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45a5a61bab7c668da4dca4f04035d1591f3f881de089cf7d5d0eb5c61047b24e`  
		Last Modified: Fri, 12 Mar 2021 06:53:21 GMT  
		Size: 1.7 KB (1726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95f2a4734ac3b65e38716098f68a245ec070b19c13e25c973384974080985a39`  
		Last Modified: Fri, 12 Mar 2021 06:53:21 GMT  
		Size: 1.8 MB (1839165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df35f9246e6d14f7ad431c61302e7bad1e572f12961d03cfbae8002566cf015e`  
		Last Modified: Fri, 12 Mar 2021 06:53:23 GMT  
		Size: 5.5 MB (5479946 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df39c466be406089e873a655fc3d9585e6728944c50a09f712c9288e4821840a`  
		Last Modified: Fri, 12 Mar 2021 06:53:21 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61632ee9ac22afc34d099b3aa93bd9266d46353b31d941b698472895798f76d5`  
		Last Modified: Fri, 12 Mar 2021 06:53:20 GMT  
		Size: 342.0 B  
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
$ docker pull spiped@sha256:983466fa8b75cc318fce3c1038b7f9b2e24be7bf710f1234918a2364434d33cd
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.5 MB (41528897 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:17d7f4efc36fd2e78999383994c2a57513df86a50c9b4b8a2a70745c0ef01c3f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 12 Mar 2021 01:44:27 GMT
ADD file:90c103e04bd6fe0f39733cbf8eb2d8845aed3e4fc3fd1e5c3354df69e40aa615 in / 
# Fri, 12 Mar 2021 01:44:28 GMT
CMD ["bash"]
# Fri, 12 Mar 2021 08:01:04 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Fri, 12 Mar 2021 08:01:13 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Fri, 12 Mar 2021 08:01:13 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 12 Mar 2021 08:02:03 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Fri, 12 Mar 2021 08:02:03 GMT
VOLUME [/spiped]
# Fri, 12 Mar 2021 08:02:04 GMT
WORKDIR /spiped
# Fri, 12 Mar 2021 08:02:04 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 12 Mar 2021 08:02:05 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 12 Mar 2021 08:02:05 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:0898aa7472f57f223652846337cf862f142e109d0c039b41886e7f20c345f85e`  
		Last Modified: Fri, 12 Mar 2021 01:52:08 GMT  
		Size: 27.8 MB (27760948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2eeafcbbeef1137b3b2433a649677cdfd7113607c5b693cb276cd3810d6383bb`  
		Last Modified: Fri, 12 Mar 2021 08:03:39 GMT  
		Size: 1.7 KB (1727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f067ef9a68fd173c54513f6d3c9ba77456cecbb432abe4a3c8c42a9bc99dc3c3`  
		Last Modified: Fri, 12 Mar 2021 08:03:40 GMT  
		Size: 2.1 MB (2132517 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b0901526cede0fd9a9131582f346bfc4dda397797919300292b605ab8d95446`  
		Last Modified: Fri, 12 Mar 2021 08:03:45 GMT  
		Size: 11.6 MB (11633235 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b70641cb409fc1dfa619f62e8e07e4b213dfdb2606f52ad06a19f4bd0a400ac7`  
		Last Modified: Fri, 12 Mar 2021 08:03:39 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d91d719b7b0195babc02c423652700f85d1ea7e72f9624383e05cf0ce9d5ee80`  
		Last Modified: Fri, 12 Mar 2021 08:03:39 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; mips64le

```console
$ docker pull spiped@sha256:032d1b7cf8b68483133baf48781840d8146637e72564e09a1d82e376ff9eb33b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.9 MB (33903158 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0c74c8ea83b0be3818801b895be0ff244b7eedbdd6f3e1ae04db57d6099310bc`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 12 Mar 2021 02:10:02 GMT
ADD file:491c5ca15fe098b83de42861289c216c693d788a1f9e739a78acefb0cad453c8 in / 
# Fri, 12 Mar 2021 02:10:03 GMT
CMD ["bash"]
# Fri, 12 Mar 2021 02:38:08 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Fri, 12 Mar 2021 02:38:21 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Fri, 12 Mar 2021 02:38:21 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 12 Mar 2021 02:39:31 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Fri, 12 Mar 2021 02:39:32 GMT
VOLUME [/spiped]
# Fri, 12 Mar 2021 02:39:32 GMT
WORKDIR /spiped
# Fri, 12 Mar 2021 02:39:33 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 12 Mar 2021 02:39:33 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 12 Mar 2021 02:39:33 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:d0b6b2cc51bdde474395b8c32ff8012e471727bba69f221cfb79b46e8283f047`  
		Last Modified: Fri, 12 Mar 2021 02:17:07 GMT  
		Size: 25.8 MB (25772338 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dff97d649bac8fe9b39d04479cb1b7c29bc5ffa49396a377ac8cccad33c57f80`  
		Last Modified: Fri, 12 Mar 2021 02:39:57 GMT  
		Size: 1.7 KB (1736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f20c729eedeccd3e485c767cb313809c2f0f0b1c4f0260e61c3d17de850fe27`  
		Last Modified: Fri, 12 Mar 2021 02:39:58 GMT  
		Size: 1.7 MB (1712217 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47bec35739b82d57c3b55153ffc2209c8eb0648ce203f093da154ba888b51465`  
		Last Modified: Fri, 12 Mar 2021 02:40:02 GMT  
		Size: 6.4 MB (6416430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26904b89eba14cd7eb16008f7281ab8ef034dd86d850f5caedd21241ec49fb9a`  
		Last Modified: Fri, 12 Mar 2021 02:39:56 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bdf822474fdfb17ae182dd3e7a3bb12ec21e278a2420b250366826eded9cc09`  
		Last Modified: Fri, 12 Mar 2021 02:39:56 GMT  
		Size: 342.0 B  
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
$ docker pull spiped@sha256:d82c38d06159e7db0753db1e0f845dc0f1eb3961674c5bc22cd41e9621dbc76a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.5 MB (33483809 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:645016ed58a1c6ce99c54f4cc811986d2a5e214cea1b492cfa0899a2438f4a88`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 12 Mar 2021 01:46:04 GMT
ADD file:afec039adf230a9186a38b57eed85262696f8d178ac649a445657066f16fe806 in / 
# Fri, 12 Mar 2021 01:46:07 GMT
CMD ["bash"]
# Fri, 12 Mar 2021 08:07:34 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Fri, 12 Mar 2021 08:07:38 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Fri, 12 Mar 2021 08:07:38 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 12 Mar 2021 08:08:04 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Fri, 12 Mar 2021 08:08:05 GMT
VOLUME [/spiped]
# Fri, 12 Mar 2021 08:08:06 GMT
WORKDIR /spiped
# Fri, 12 Mar 2021 08:08:06 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 12 Mar 2021 08:08:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 12 Mar 2021 08:08:06 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:d41215965c091534e809ab2e8f4a2c1cebee3de536c2c74a7bc8302bbc8af7e1`  
		Last Modified: Fri, 12 Mar 2021 01:50:30 GMT  
		Size: 25.7 MB (25716294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b579a281fa0ba65a910c9115d88b9822da2db452b18a36a96eca5dcd343cedab`  
		Last Modified: Fri, 12 Mar 2021 08:08:27 GMT  
		Size: 1.7 KB (1737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57ee5dd0e1e787ff01f176042d7d39f1a9edc84e1ee227e05c4d4051ffba9407`  
		Last Modified: Fri, 12 Mar 2021 08:08:28 GMT  
		Size: 1.8 MB (1821831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab7081653748b145146444bd9b5eb8a31bd7c3c19208f896624e14cee98fed28`  
		Last Modified: Fri, 12 Mar 2021 08:08:28 GMT  
		Size: 5.9 MB (5943478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc6da0d690b9f949713ec9144564f002a3deb708a362c8c03b8a44ad7ef98e08`  
		Last Modified: Fri, 12 Mar 2021 08:08:27 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63c6089d8250b376ca27d8144b7724c128400730110c27b351c0cb952cbf5694`  
		Last Modified: Fri, 12 Mar 2021 08:08:28 GMT  
		Size: 340.0 B  
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
$ docker pull spiped@sha256:f00a200fc1b19303be35892bcaaf6f82dffb6d5afe90d49d3bbfa350c1ae2161
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
$ docker pull spiped@sha256:7be4a2a8c7741dcedad533f936408fce6017373a865914793bbeceb65ac7317c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.2 MB (32167233 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2d2d9655883de89f3593e8c0503223ad9d77ec8ef3b444604cbdbe0bef719dc5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 12 Mar 2021 01:52:27 GMT
ADD file:8e357182800adfe658856515726f1e012cc120349f0f305692cf50282f6d8b7b in / 
# Fri, 12 Mar 2021 01:52:29 GMT
CMD ["bash"]
# Fri, 12 Mar 2021 06:51:44 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Fri, 12 Mar 2021 06:51:54 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Fri, 12 Mar 2021 06:51:55 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 12 Mar 2021 06:52:51 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Fri, 12 Mar 2021 06:52:53 GMT
VOLUME [/spiped]
# Fri, 12 Mar 2021 06:52:54 GMT
WORKDIR /spiped
# Fri, 12 Mar 2021 06:52:55 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 12 Mar 2021 06:52:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 12 Mar 2021 06:52:57 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:9babb1be2e38b3bddad5a4e05bb34173369ae3472c0c0d8668853011cd65969f`  
		Last Modified: Fri, 12 Mar 2021 02:02:01 GMT  
		Size: 24.8 MB (24845925 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45a5a61bab7c668da4dca4f04035d1591f3f881de089cf7d5d0eb5c61047b24e`  
		Last Modified: Fri, 12 Mar 2021 06:53:21 GMT  
		Size: 1.7 KB (1726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95f2a4734ac3b65e38716098f68a245ec070b19c13e25c973384974080985a39`  
		Last Modified: Fri, 12 Mar 2021 06:53:21 GMT  
		Size: 1.8 MB (1839165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df35f9246e6d14f7ad431c61302e7bad1e572f12961d03cfbae8002566cf015e`  
		Last Modified: Fri, 12 Mar 2021 06:53:23 GMT  
		Size: 5.5 MB (5479946 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df39c466be406089e873a655fc3d9585e6728944c50a09f712c9288e4821840a`  
		Last Modified: Fri, 12 Mar 2021 06:53:21 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61632ee9ac22afc34d099b3aa93bd9266d46353b31d941b698472895798f76d5`  
		Last Modified: Fri, 12 Mar 2021 06:53:20 GMT  
		Size: 342.0 B  
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
$ docker pull spiped@sha256:983466fa8b75cc318fce3c1038b7f9b2e24be7bf710f1234918a2364434d33cd
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.5 MB (41528897 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:17d7f4efc36fd2e78999383994c2a57513df86a50c9b4b8a2a70745c0ef01c3f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 12 Mar 2021 01:44:27 GMT
ADD file:90c103e04bd6fe0f39733cbf8eb2d8845aed3e4fc3fd1e5c3354df69e40aa615 in / 
# Fri, 12 Mar 2021 01:44:28 GMT
CMD ["bash"]
# Fri, 12 Mar 2021 08:01:04 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Fri, 12 Mar 2021 08:01:13 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Fri, 12 Mar 2021 08:01:13 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 12 Mar 2021 08:02:03 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Fri, 12 Mar 2021 08:02:03 GMT
VOLUME [/spiped]
# Fri, 12 Mar 2021 08:02:04 GMT
WORKDIR /spiped
# Fri, 12 Mar 2021 08:02:04 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 12 Mar 2021 08:02:05 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 12 Mar 2021 08:02:05 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:0898aa7472f57f223652846337cf862f142e109d0c039b41886e7f20c345f85e`  
		Last Modified: Fri, 12 Mar 2021 01:52:08 GMT  
		Size: 27.8 MB (27760948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2eeafcbbeef1137b3b2433a649677cdfd7113607c5b693cb276cd3810d6383bb`  
		Last Modified: Fri, 12 Mar 2021 08:03:39 GMT  
		Size: 1.7 KB (1727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f067ef9a68fd173c54513f6d3c9ba77456cecbb432abe4a3c8c42a9bc99dc3c3`  
		Last Modified: Fri, 12 Mar 2021 08:03:40 GMT  
		Size: 2.1 MB (2132517 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b0901526cede0fd9a9131582f346bfc4dda397797919300292b605ab8d95446`  
		Last Modified: Fri, 12 Mar 2021 08:03:45 GMT  
		Size: 11.6 MB (11633235 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b70641cb409fc1dfa619f62e8e07e4b213dfdb2606f52ad06a19f4bd0a400ac7`  
		Last Modified: Fri, 12 Mar 2021 08:03:39 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d91d719b7b0195babc02c423652700f85d1ea7e72f9624383e05cf0ce9d5ee80`  
		Last Modified: Fri, 12 Mar 2021 08:03:39 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; mips64le

```console
$ docker pull spiped@sha256:032d1b7cf8b68483133baf48781840d8146637e72564e09a1d82e376ff9eb33b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.9 MB (33903158 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0c74c8ea83b0be3818801b895be0ff244b7eedbdd6f3e1ae04db57d6099310bc`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 12 Mar 2021 02:10:02 GMT
ADD file:491c5ca15fe098b83de42861289c216c693d788a1f9e739a78acefb0cad453c8 in / 
# Fri, 12 Mar 2021 02:10:03 GMT
CMD ["bash"]
# Fri, 12 Mar 2021 02:38:08 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Fri, 12 Mar 2021 02:38:21 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Fri, 12 Mar 2021 02:38:21 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 12 Mar 2021 02:39:31 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Fri, 12 Mar 2021 02:39:32 GMT
VOLUME [/spiped]
# Fri, 12 Mar 2021 02:39:32 GMT
WORKDIR /spiped
# Fri, 12 Mar 2021 02:39:33 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 12 Mar 2021 02:39:33 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 12 Mar 2021 02:39:33 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:d0b6b2cc51bdde474395b8c32ff8012e471727bba69f221cfb79b46e8283f047`  
		Last Modified: Fri, 12 Mar 2021 02:17:07 GMT  
		Size: 25.8 MB (25772338 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dff97d649bac8fe9b39d04479cb1b7c29bc5ffa49396a377ac8cccad33c57f80`  
		Last Modified: Fri, 12 Mar 2021 02:39:57 GMT  
		Size: 1.7 KB (1736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f20c729eedeccd3e485c767cb313809c2f0f0b1c4f0260e61c3d17de850fe27`  
		Last Modified: Fri, 12 Mar 2021 02:39:58 GMT  
		Size: 1.7 MB (1712217 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47bec35739b82d57c3b55153ffc2209c8eb0648ce203f093da154ba888b51465`  
		Last Modified: Fri, 12 Mar 2021 02:40:02 GMT  
		Size: 6.4 MB (6416430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26904b89eba14cd7eb16008f7281ab8ef034dd86d850f5caedd21241ec49fb9a`  
		Last Modified: Fri, 12 Mar 2021 02:39:56 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bdf822474fdfb17ae182dd3e7a3bb12ec21e278a2420b250366826eded9cc09`  
		Last Modified: Fri, 12 Mar 2021 02:39:56 GMT  
		Size: 342.0 B  
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
$ docker pull spiped@sha256:d82c38d06159e7db0753db1e0f845dc0f1eb3961674c5bc22cd41e9621dbc76a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.5 MB (33483809 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:645016ed58a1c6ce99c54f4cc811986d2a5e214cea1b492cfa0899a2438f4a88`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 12 Mar 2021 01:46:04 GMT
ADD file:afec039adf230a9186a38b57eed85262696f8d178ac649a445657066f16fe806 in / 
# Fri, 12 Mar 2021 01:46:07 GMT
CMD ["bash"]
# Fri, 12 Mar 2021 08:07:34 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Fri, 12 Mar 2021 08:07:38 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Fri, 12 Mar 2021 08:07:38 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 12 Mar 2021 08:08:04 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Fri, 12 Mar 2021 08:08:05 GMT
VOLUME [/spiped]
# Fri, 12 Mar 2021 08:08:06 GMT
WORKDIR /spiped
# Fri, 12 Mar 2021 08:08:06 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 12 Mar 2021 08:08:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 12 Mar 2021 08:08:06 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:d41215965c091534e809ab2e8f4a2c1cebee3de536c2c74a7bc8302bbc8af7e1`  
		Last Modified: Fri, 12 Mar 2021 01:50:30 GMT  
		Size: 25.7 MB (25716294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b579a281fa0ba65a910c9115d88b9822da2db452b18a36a96eca5dcd343cedab`  
		Last Modified: Fri, 12 Mar 2021 08:08:27 GMT  
		Size: 1.7 KB (1737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57ee5dd0e1e787ff01f176042d7d39f1a9edc84e1ee227e05c4d4051ffba9407`  
		Last Modified: Fri, 12 Mar 2021 08:08:28 GMT  
		Size: 1.8 MB (1821831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab7081653748b145146444bd9b5eb8a31bd7c3c19208f896624e14cee98fed28`  
		Last Modified: Fri, 12 Mar 2021 08:08:28 GMT  
		Size: 5.9 MB (5943478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc6da0d690b9f949713ec9144564f002a3deb708a362c8c03b8a44ad7ef98e08`  
		Last Modified: Fri, 12 Mar 2021 08:08:27 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63c6089d8250b376ca27d8144b7724c128400730110c27b351c0cb952cbf5694`  
		Last Modified: Fri, 12 Mar 2021 08:08:28 GMT  
		Size: 340.0 B  
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
$ docker pull spiped@sha256:f00a200fc1b19303be35892bcaaf6f82dffb6d5afe90d49d3bbfa350c1ae2161
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
$ docker pull spiped@sha256:7be4a2a8c7741dcedad533f936408fce6017373a865914793bbeceb65ac7317c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.2 MB (32167233 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2d2d9655883de89f3593e8c0503223ad9d77ec8ef3b444604cbdbe0bef719dc5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 12 Mar 2021 01:52:27 GMT
ADD file:8e357182800adfe658856515726f1e012cc120349f0f305692cf50282f6d8b7b in / 
# Fri, 12 Mar 2021 01:52:29 GMT
CMD ["bash"]
# Fri, 12 Mar 2021 06:51:44 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Fri, 12 Mar 2021 06:51:54 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Fri, 12 Mar 2021 06:51:55 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 12 Mar 2021 06:52:51 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Fri, 12 Mar 2021 06:52:53 GMT
VOLUME [/spiped]
# Fri, 12 Mar 2021 06:52:54 GMT
WORKDIR /spiped
# Fri, 12 Mar 2021 06:52:55 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 12 Mar 2021 06:52:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 12 Mar 2021 06:52:57 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:9babb1be2e38b3bddad5a4e05bb34173369ae3472c0c0d8668853011cd65969f`  
		Last Modified: Fri, 12 Mar 2021 02:02:01 GMT  
		Size: 24.8 MB (24845925 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45a5a61bab7c668da4dca4f04035d1591f3f881de089cf7d5d0eb5c61047b24e`  
		Last Modified: Fri, 12 Mar 2021 06:53:21 GMT  
		Size: 1.7 KB (1726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95f2a4734ac3b65e38716098f68a245ec070b19c13e25c973384974080985a39`  
		Last Modified: Fri, 12 Mar 2021 06:53:21 GMT  
		Size: 1.8 MB (1839165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df35f9246e6d14f7ad431c61302e7bad1e572f12961d03cfbae8002566cf015e`  
		Last Modified: Fri, 12 Mar 2021 06:53:23 GMT  
		Size: 5.5 MB (5479946 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df39c466be406089e873a655fc3d9585e6728944c50a09f712c9288e4821840a`  
		Last Modified: Fri, 12 Mar 2021 06:53:21 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61632ee9ac22afc34d099b3aa93bd9266d46353b31d941b698472895798f76d5`  
		Last Modified: Fri, 12 Mar 2021 06:53:20 GMT  
		Size: 342.0 B  
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
$ docker pull spiped@sha256:983466fa8b75cc318fce3c1038b7f9b2e24be7bf710f1234918a2364434d33cd
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.5 MB (41528897 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:17d7f4efc36fd2e78999383994c2a57513df86a50c9b4b8a2a70745c0ef01c3f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 12 Mar 2021 01:44:27 GMT
ADD file:90c103e04bd6fe0f39733cbf8eb2d8845aed3e4fc3fd1e5c3354df69e40aa615 in / 
# Fri, 12 Mar 2021 01:44:28 GMT
CMD ["bash"]
# Fri, 12 Mar 2021 08:01:04 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Fri, 12 Mar 2021 08:01:13 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Fri, 12 Mar 2021 08:01:13 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 12 Mar 2021 08:02:03 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Fri, 12 Mar 2021 08:02:03 GMT
VOLUME [/spiped]
# Fri, 12 Mar 2021 08:02:04 GMT
WORKDIR /spiped
# Fri, 12 Mar 2021 08:02:04 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 12 Mar 2021 08:02:05 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 12 Mar 2021 08:02:05 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:0898aa7472f57f223652846337cf862f142e109d0c039b41886e7f20c345f85e`  
		Last Modified: Fri, 12 Mar 2021 01:52:08 GMT  
		Size: 27.8 MB (27760948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2eeafcbbeef1137b3b2433a649677cdfd7113607c5b693cb276cd3810d6383bb`  
		Last Modified: Fri, 12 Mar 2021 08:03:39 GMT  
		Size: 1.7 KB (1727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f067ef9a68fd173c54513f6d3c9ba77456cecbb432abe4a3c8c42a9bc99dc3c3`  
		Last Modified: Fri, 12 Mar 2021 08:03:40 GMT  
		Size: 2.1 MB (2132517 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b0901526cede0fd9a9131582f346bfc4dda397797919300292b605ab8d95446`  
		Last Modified: Fri, 12 Mar 2021 08:03:45 GMT  
		Size: 11.6 MB (11633235 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b70641cb409fc1dfa619f62e8e07e4b213dfdb2606f52ad06a19f4bd0a400ac7`  
		Last Modified: Fri, 12 Mar 2021 08:03:39 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d91d719b7b0195babc02c423652700f85d1ea7e72f9624383e05cf0ce9d5ee80`  
		Last Modified: Fri, 12 Mar 2021 08:03:39 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1` - linux; mips64le

```console
$ docker pull spiped@sha256:032d1b7cf8b68483133baf48781840d8146637e72564e09a1d82e376ff9eb33b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.9 MB (33903158 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0c74c8ea83b0be3818801b895be0ff244b7eedbdd6f3e1ae04db57d6099310bc`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 12 Mar 2021 02:10:02 GMT
ADD file:491c5ca15fe098b83de42861289c216c693d788a1f9e739a78acefb0cad453c8 in / 
# Fri, 12 Mar 2021 02:10:03 GMT
CMD ["bash"]
# Fri, 12 Mar 2021 02:38:08 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Fri, 12 Mar 2021 02:38:21 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Fri, 12 Mar 2021 02:38:21 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 12 Mar 2021 02:39:31 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Fri, 12 Mar 2021 02:39:32 GMT
VOLUME [/spiped]
# Fri, 12 Mar 2021 02:39:32 GMT
WORKDIR /spiped
# Fri, 12 Mar 2021 02:39:33 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 12 Mar 2021 02:39:33 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 12 Mar 2021 02:39:33 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:d0b6b2cc51bdde474395b8c32ff8012e471727bba69f221cfb79b46e8283f047`  
		Last Modified: Fri, 12 Mar 2021 02:17:07 GMT  
		Size: 25.8 MB (25772338 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dff97d649bac8fe9b39d04479cb1b7c29bc5ffa49396a377ac8cccad33c57f80`  
		Last Modified: Fri, 12 Mar 2021 02:39:57 GMT  
		Size: 1.7 KB (1736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f20c729eedeccd3e485c767cb313809c2f0f0b1c4f0260e61c3d17de850fe27`  
		Last Modified: Fri, 12 Mar 2021 02:39:58 GMT  
		Size: 1.7 MB (1712217 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47bec35739b82d57c3b55153ffc2209c8eb0648ce203f093da154ba888b51465`  
		Last Modified: Fri, 12 Mar 2021 02:40:02 GMT  
		Size: 6.4 MB (6416430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26904b89eba14cd7eb16008f7281ab8ef034dd86d850f5caedd21241ec49fb9a`  
		Last Modified: Fri, 12 Mar 2021 02:39:56 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bdf822474fdfb17ae182dd3e7a3bb12ec21e278a2420b250366826eded9cc09`  
		Last Modified: Fri, 12 Mar 2021 02:39:56 GMT  
		Size: 342.0 B  
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
$ docker pull spiped@sha256:d82c38d06159e7db0753db1e0f845dc0f1eb3961674c5bc22cd41e9621dbc76a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.5 MB (33483809 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:645016ed58a1c6ce99c54f4cc811986d2a5e214cea1b492cfa0899a2438f4a88`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 12 Mar 2021 01:46:04 GMT
ADD file:afec039adf230a9186a38b57eed85262696f8d178ac649a445657066f16fe806 in / 
# Fri, 12 Mar 2021 01:46:07 GMT
CMD ["bash"]
# Fri, 12 Mar 2021 08:07:34 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Fri, 12 Mar 2021 08:07:38 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Fri, 12 Mar 2021 08:07:38 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 12 Mar 2021 08:08:04 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Fri, 12 Mar 2021 08:08:05 GMT
VOLUME [/spiped]
# Fri, 12 Mar 2021 08:08:06 GMT
WORKDIR /spiped
# Fri, 12 Mar 2021 08:08:06 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 12 Mar 2021 08:08:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 12 Mar 2021 08:08:06 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:d41215965c091534e809ab2e8f4a2c1cebee3de536c2c74a7bc8302bbc8af7e1`  
		Last Modified: Fri, 12 Mar 2021 01:50:30 GMT  
		Size: 25.7 MB (25716294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b579a281fa0ba65a910c9115d88b9822da2db452b18a36a96eca5dcd343cedab`  
		Last Modified: Fri, 12 Mar 2021 08:08:27 GMT  
		Size: 1.7 KB (1737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57ee5dd0e1e787ff01f176042d7d39f1a9edc84e1ee227e05c4d4051ffba9407`  
		Last Modified: Fri, 12 Mar 2021 08:08:28 GMT  
		Size: 1.8 MB (1821831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab7081653748b145146444bd9b5eb8a31bd7c3c19208f896624e14cee98fed28`  
		Last Modified: Fri, 12 Mar 2021 08:08:28 GMT  
		Size: 5.9 MB (5943478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc6da0d690b9f949713ec9144564f002a3deb708a362c8c03b8a44ad7ef98e08`  
		Last Modified: Fri, 12 Mar 2021 08:08:27 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63c6089d8250b376ca27d8144b7724c128400730110c27b351c0cb952cbf5694`  
		Last Modified: Fri, 12 Mar 2021 08:08:28 GMT  
		Size: 340.0 B  
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
$ docker pull spiped@sha256:f00a200fc1b19303be35892bcaaf6f82dffb6d5afe90d49d3bbfa350c1ae2161
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
$ docker pull spiped@sha256:7be4a2a8c7741dcedad533f936408fce6017373a865914793bbeceb65ac7317c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.2 MB (32167233 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2d2d9655883de89f3593e8c0503223ad9d77ec8ef3b444604cbdbe0bef719dc5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 12 Mar 2021 01:52:27 GMT
ADD file:8e357182800adfe658856515726f1e012cc120349f0f305692cf50282f6d8b7b in / 
# Fri, 12 Mar 2021 01:52:29 GMT
CMD ["bash"]
# Fri, 12 Mar 2021 06:51:44 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Fri, 12 Mar 2021 06:51:54 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Fri, 12 Mar 2021 06:51:55 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 12 Mar 2021 06:52:51 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Fri, 12 Mar 2021 06:52:53 GMT
VOLUME [/spiped]
# Fri, 12 Mar 2021 06:52:54 GMT
WORKDIR /spiped
# Fri, 12 Mar 2021 06:52:55 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 12 Mar 2021 06:52:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 12 Mar 2021 06:52:57 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:9babb1be2e38b3bddad5a4e05bb34173369ae3472c0c0d8668853011cd65969f`  
		Last Modified: Fri, 12 Mar 2021 02:02:01 GMT  
		Size: 24.8 MB (24845925 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45a5a61bab7c668da4dca4f04035d1591f3f881de089cf7d5d0eb5c61047b24e`  
		Last Modified: Fri, 12 Mar 2021 06:53:21 GMT  
		Size: 1.7 KB (1726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95f2a4734ac3b65e38716098f68a245ec070b19c13e25c973384974080985a39`  
		Last Modified: Fri, 12 Mar 2021 06:53:21 GMT  
		Size: 1.8 MB (1839165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df35f9246e6d14f7ad431c61302e7bad1e572f12961d03cfbae8002566cf015e`  
		Last Modified: Fri, 12 Mar 2021 06:53:23 GMT  
		Size: 5.5 MB (5479946 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df39c466be406089e873a655fc3d9585e6728944c50a09f712c9288e4821840a`  
		Last Modified: Fri, 12 Mar 2021 06:53:21 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61632ee9ac22afc34d099b3aa93bd9266d46353b31d941b698472895798f76d5`  
		Last Modified: Fri, 12 Mar 2021 06:53:20 GMT  
		Size: 342.0 B  
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
$ docker pull spiped@sha256:983466fa8b75cc318fce3c1038b7f9b2e24be7bf710f1234918a2364434d33cd
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.5 MB (41528897 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:17d7f4efc36fd2e78999383994c2a57513df86a50c9b4b8a2a70745c0ef01c3f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 12 Mar 2021 01:44:27 GMT
ADD file:90c103e04bd6fe0f39733cbf8eb2d8845aed3e4fc3fd1e5c3354df69e40aa615 in / 
# Fri, 12 Mar 2021 01:44:28 GMT
CMD ["bash"]
# Fri, 12 Mar 2021 08:01:04 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Fri, 12 Mar 2021 08:01:13 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Fri, 12 Mar 2021 08:01:13 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 12 Mar 2021 08:02:03 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Fri, 12 Mar 2021 08:02:03 GMT
VOLUME [/spiped]
# Fri, 12 Mar 2021 08:02:04 GMT
WORKDIR /spiped
# Fri, 12 Mar 2021 08:02:04 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 12 Mar 2021 08:02:05 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 12 Mar 2021 08:02:05 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:0898aa7472f57f223652846337cf862f142e109d0c039b41886e7f20c345f85e`  
		Last Modified: Fri, 12 Mar 2021 01:52:08 GMT  
		Size: 27.8 MB (27760948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2eeafcbbeef1137b3b2433a649677cdfd7113607c5b693cb276cd3810d6383bb`  
		Last Modified: Fri, 12 Mar 2021 08:03:39 GMT  
		Size: 1.7 KB (1727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f067ef9a68fd173c54513f6d3c9ba77456cecbb432abe4a3c8c42a9bc99dc3c3`  
		Last Modified: Fri, 12 Mar 2021 08:03:40 GMT  
		Size: 2.1 MB (2132517 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b0901526cede0fd9a9131582f346bfc4dda397797919300292b605ab8d95446`  
		Last Modified: Fri, 12 Mar 2021 08:03:45 GMT  
		Size: 11.6 MB (11633235 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b70641cb409fc1dfa619f62e8e07e4b213dfdb2606f52ad06a19f4bd0a400ac7`  
		Last Modified: Fri, 12 Mar 2021 08:03:39 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d91d719b7b0195babc02c423652700f85d1ea7e72f9624383e05cf0ce9d5ee80`  
		Last Modified: Fri, 12 Mar 2021 08:03:39 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; mips64le

```console
$ docker pull spiped@sha256:032d1b7cf8b68483133baf48781840d8146637e72564e09a1d82e376ff9eb33b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.9 MB (33903158 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0c74c8ea83b0be3818801b895be0ff244b7eedbdd6f3e1ae04db57d6099310bc`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 12 Mar 2021 02:10:02 GMT
ADD file:491c5ca15fe098b83de42861289c216c693d788a1f9e739a78acefb0cad453c8 in / 
# Fri, 12 Mar 2021 02:10:03 GMT
CMD ["bash"]
# Fri, 12 Mar 2021 02:38:08 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Fri, 12 Mar 2021 02:38:21 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Fri, 12 Mar 2021 02:38:21 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 12 Mar 2021 02:39:31 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Fri, 12 Mar 2021 02:39:32 GMT
VOLUME [/spiped]
# Fri, 12 Mar 2021 02:39:32 GMT
WORKDIR /spiped
# Fri, 12 Mar 2021 02:39:33 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 12 Mar 2021 02:39:33 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 12 Mar 2021 02:39:33 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:d0b6b2cc51bdde474395b8c32ff8012e471727bba69f221cfb79b46e8283f047`  
		Last Modified: Fri, 12 Mar 2021 02:17:07 GMT  
		Size: 25.8 MB (25772338 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dff97d649bac8fe9b39d04479cb1b7c29bc5ffa49396a377ac8cccad33c57f80`  
		Last Modified: Fri, 12 Mar 2021 02:39:57 GMT  
		Size: 1.7 KB (1736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f20c729eedeccd3e485c767cb313809c2f0f0b1c4f0260e61c3d17de850fe27`  
		Last Modified: Fri, 12 Mar 2021 02:39:58 GMT  
		Size: 1.7 MB (1712217 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47bec35739b82d57c3b55153ffc2209c8eb0648ce203f093da154ba888b51465`  
		Last Modified: Fri, 12 Mar 2021 02:40:02 GMT  
		Size: 6.4 MB (6416430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26904b89eba14cd7eb16008f7281ab8ef034dd86d850f5caedd21241ec49fb9a`  
		Last Modified: Fri, 12 Mar 2021 02:39:56 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bdf822474fdfb17ae182dd3e7a3bb12ec21e278a2420b250366826eded9cc09`  
		Last Modified: Fri, 12 Mar 2021 02:39:56 GMT  
		Size: 342.0 B  
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
$ docker pull spiped@sha256:d82c38d06159e7db0753db1e0f845dc0f1eb3961674c5bc22cd41e9621dbc76a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.5 MB (33483809 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:645016ed58a1c6ce99c54f4cc811986d2a5e214cea1b492cfa0899a2438f4a88`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 12 Mar 2021 01:46:04 GMT
ADD file:afec039adf230a9186a38b57eed85262696f8d178ac649a445657066f16fe806 in / 
# Fri, 12 Mar 2021 01:46:07 GMT
CMD ["bash"]
# Fri, 12 Mar 2021 08:07:34 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Fri, 12 Mar 2021 08:07:38 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Fri, 12 Mar 2021 08:07:38 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 12 Mar 2021 08:08:04 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Fri, 12 Mar 2021 08:08:05 GMT
VOLUME [/spiped]
# Fri, 12 Mar 2021 08:08:06 GMT
WORKDIR /spiped
# Fri, 12 Mar 2021 08:08:06 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 12 Mar 2021 08:08:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 12 Mar 2021 08:08:06 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:d41215965c091534e809ab2e8f4a2c1cebee3de536c2c74a7bc8302bbc8af7e1`  
		Last Modified: Fri, 12 Mar 2021 01:50:30 GMT  
		Size: 25.7 MB (25716294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b579a281fa0ba65a910c9115d88b9822da2db452b18a36a96eca5dcd343cedab`  
		Last Modified: Fri, 12 Mar 2021 08:08:27 GMT  
		Size: 1.7 KB (1737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57ee5dd0e1e787ff01f176042d7d39f1a9edc84e1ee227e05c4d4051ffba9407`  
		Last Modified: Fri, 12 Mar 2021 08:08:28 GMT  
		Size: 1.8 MB (1821831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab7081653748b145146444bd9b5eb8a31bd7c3c19208f896624e14cee98fed28`  
		Last Modified: Fri, 12 Mar 2021 08:08:28 GMT  
		Size: 5.9 MB (5943478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc6da0d690b9f949713ec9144564f002a3deb708a362c8c03b8a44ad7ef98e08`  
		Last Modified: Fri, 12 Mar 2021 08:08:27 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63c6089d8250b376ca27d8144b7724c128400730110c27b351c0cb952cbf5694`  
		Last Modified: Fri, 12 Mar 2021 08:08:28 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
