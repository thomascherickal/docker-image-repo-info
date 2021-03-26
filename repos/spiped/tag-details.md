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
$ docker pull spiped@sha256:7059805cf01965859918fa9d47d36661a2527a3cafd2dc66d92d2c54b7f5c7a4
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
$ docker pull spiped@sha256:48c027238fbc19554916ff378bed97ea4f5fd5c603e280747d70562648af3472
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (3032749 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:337c259d969e84592201606f94892febf289ce47a0d407e08a069666c2d69a77`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 17 Feb 2021 21:19:54 GMT
ADD file:80bf8bd014071345b1c0364eeb0a5e48f3fb0d87f9c31cb990e57caa652b59b8 in / 
# Wed, 17 Feb 2021 21:19:54 GMT
CMD ["/bin/sh"]
# Fri, 12 Mar 2021 13:35:19 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 12 Mar 2021 13:35:20 GMT
RUN apk add --no-cache libssl1.1
# Fri, 12 Mar 2021 13:35:20 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 12 Mar 2021 13:35:38 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 12 Mar 2021 13:35:38 GMT
VOLUME [/spiped]
# Fri, 12 Mar 2021 13:35:39 GMT
WORKDIR /spiped
# Fri, 12 Mar 2021 13:35:39 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 12 Mar 2021 13:35:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 12 Mar 2021 13:35:39 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:ba3557a56b150f9b813f9d02274d62914fd8fce120dd374d9ee17b87cf1d277d`  
		Last Modified: Wed, 17 Feb 2021 21:20:25 GMT  
		Size: 2.8 MB (2811657 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08ee8075a0364f96f14fb19f0cf1699bba69bbbd6ecb1346e65bf6f53789ec3f`  
		Last Modified: Fri, 12 Mar 2021 13:36:15 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3eb81ccfc669ba7ed08bc8dfbf286026d62b567a4ee7575ba3468e0f71dcadf8`  
		Last Modified: Fri, 12 Mar 2021 13:36:15 GMT  
		Size: 7.0 KB (7046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49bca945030c802bb92b127f52e8e01ed86d8e3575ed3856ce8f6a95a3e75353`  
		Last Modified: Fri, 12 Mar 2021 13:36:16 GMT  
		Size: 212.3 KB (212315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b234f0abff6e36d72f674d4781560a96fa1c771db2a9333fb53181e5673666c`  
		Last Modified: Fri, 12 Mar 2021 13:36:15 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2209594492d63e6e3a196fbeab335f9be161f51a495d896b89f0597e7386441e`  
		Last Modified: Fri, 12 Mar 2021 13:36:15 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; arm variant v6

```console
$ docker pull spiped@sha256:a4eae04b6b59fa1465464612d582ab381eae7d0fd508089e99a2d9642d83d589
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 MB (2833085 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:efa0d64ae65bd0aed1fae629f2219ead07f2df4d55520aa67fa73701725be6a4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 17 Feb 2021 20:49:32 GMT
ADD file:c04fbd3b039001c592cfa14f8388f8934ed4223ccf274dbb926e75039e172af4 in / 
# Wed, 17 Feb 2021 20:49:33 GMT
CMD ["/bin/sh"]
# Thu, 18 Feb 2021 01:08:57 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 18 Feb 2021 01:09:00 GMT
RUN apk add --no-cache libssl1.1
# Thu, 18 Feb 2021 01:09:00 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 18 Feb 2021 01:09:29 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Thu, 18 Feb 2021 01:09:29 GMT
VOLUME [/spiped]
# Thu, 18 Feb 2021 01:09:30 GMT
WORKDIR /spiped
# Thu, 18 Feb 2021 01:09:31 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 18 Feb 2021 01:09:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 18 Feb 2021 01:09:34 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:1353527ebe111f9bb1e271264a3c182e909e4b36463f80d7dbde1be0713eb892`  
		Last Modified: Wed, 17 Feb 2021 20:50:06 GMT  
		Size: 2.6 MB (2622039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56478beef0e3bf335b5084e01725a07c247a0df1c2ae4d79a9b37d8d7c1d8c6b`  
		Last Modified: Thu, 18 Feb 2021 01:09:52 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09965b504ec1fcd372f0f74e2de05a28c8cfc7546e5f9abac13b9969308fffc7`  
		Last Modified: Thu, 18 Feb 2021 01:09:52 GMT  
		Size: 7.1 KB (7053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ca4d95213096352ef307626e2b9b743cd56d9e041d9bad475b082bdda7cd8fb`  
		Last Modified: Thu, 18 Feb 2021 01:09:52 GMT  
		Size: 202.3 KB (202264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:448a184417c9c40109716c2bf6eb26c63873720e7d14b4e852ffe5da738e4871`  
		Last Modified: Thu, 18 Feb 2021 01:09:52 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fb506bcaf6432a313382d4600f3ae27df33c73cfc17f1d9615fee63b17b95c3`  
		Last Modified: Thu, 18 Feb 2021 01:09:51 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; arm variant v7

```console
$ docker pull spiped@sha256:e91e8dfd1379e2029d929ab8d21b5b7cacda7a1ac496cecd8c37417d9d48e708
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 MB (2628211 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2b8d028bc188683c4af6ec6c0afa9cf33c5e88a0569d98c54eebd1e02b4b78b2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 17 Feb 2021 20:57:36 GMT
ADD file:efdd39e5243eaf378f12ad5a85d2222b44930850a90263e5f17e8a6b5e9bc9b8 in / 
# Wed, 17 Feb 2021 20:57:37 GMT
CMD ["/bin/sh"]
# Thu, 18 Feb 2021 01:11:51 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 18 Feb 2021 01:11:53 GMT
RUN apk add --no-cache libssl1.1
# Thu, 18 Feb 2021 01:11:55 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 18 Feb 2021 01:12:23 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Thu, 18 Feb 2021 01:12:24 GMT
VOLUME [/spiped]
# Thu, 18 Feb 2021 01:12:25 GMT
WORKDIR /spiped
# Thu, 18 Feb 2021 01:12:26 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 18 Feb 2021 01:12:27 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 18 Feb 2021 01:12:27 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:f55b840e27d3dbe27e44497103a4397f043749f933eb0433d29e2f104b3435ef`  
		Last Modified: Wed, 17 Feb 2021 20:58:14 GMT  
		Size: 2.4 MB (2423892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfdfb8a36c4de90dba3240099eb1d0348f8627ed1bc968f7e4271d75b265ccf2`  
		Last Modified: Thu, 18 Feb 2021 01:12:49 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35ab61a202577acd7159b1a345fcb97d20c63e42a6a170dfe22345caa4af688f`  
		Last Modified: Thu, 18 Feb 2021 01:12:49 GMT  
		Size: 7.1 KB (7051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:374409fe6217df96932998b712912ebad072a21d4d4e7817b70b6dbb23d0f0a3`  
		Last Modified: Thu, 18 Feb 2021 01:12:49 GMT  
		Size: 195.5 KB (195539 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:592de5c2b9cc50ddf43d871cb052d160ae2dc235c136a1731e45e1cf529b7b80`  
		Last Modified: Thu, 18 Feb 2021 01:12:49 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:562929d72557b487b48b0dcc0ca66188d993a95431efb6ba6e82ecece7035616`  
		Last Modified: Thu, 18 Feb 2021 01:12:49 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:b0ca7cbad488b0fcb44506f1c6c65ae77f5573dc072c30c390b75e29a9d2c64c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 MB (2924800 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bffde3212b34beb453841e58f5ca6bcdbd5dee1c658ff1861926718f1f9c5499`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 17 Feb 2021 20:39:29 GMT
ADD file:3bf1497bd250cf7c73c12231dc4ebe3a3a67f2cd99e35bce47ef6674683aeb1d in / 
# Wed, 17 Feb 2021 20:39:30 GMT
CMD ["/bin/sh"]
# Thu, 18 Feb 2021 01:23:27 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 18 Feb 2021 01:23:30 GMT
RUN apk add --no-cache libssl1.1
# Thu, 18 Feb 2021 01:23:31 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 18 Feb 2021 01:24:04 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Thu, 18 Feb 2021 01:24:05 GMT
VOLUME [/spiped]
# Thu, 18 Feb 2021 01:24:06 GMT
WORKDIR /spiped
# Thu, 18 Feb 2021 01:24:07 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 18 Feb 2021 01:24:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 18 Feb 2021 01:24:10 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:069a56d6d07f6b186fbb82e4486616b9be9a37ce32a63013af6cddcb65898182`  
		Last Modified: Wed, 17 Feb 2021 20:40:04 GMT  
		Size: 2.7 MB (2711572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:991947bc8299281c0212c4f9312423d52074ad210f1eab639db0f6df247937b2`  
		Last Modified: Thu, 18 Feb 2021 01:24:34 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83a8e0ee83f949ca3f11000f9df3c4b551cff205fc9d645ed6aa3c13d4b41a14`  
		Last Modified: Thu, 18 Feb 2021 01:24:34 GMT  
		Size: 7.1 KB (7059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6da8757762737713d5ff919736307c7a18ea61e4e68e7a6f051974461de14f8a`  
		Last Modified: Thu, 18 Feb 2021 01:24:34 GMT  
		Size: 204.4 KB (204440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13a12b508a6a8ce19fd3eee0367c035a60aebd09e422b169e7e3acb5ec2cc376`  
		Last Modified: Thu, 18 Feb 2021 01:24:34 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd46a081f7acce468799a1512f765f8f304e396d48824de8d10a33c1e6416619`  
		Last Modified: Thu, 18 Feb 2021 01:24:34 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; 386

```console
$ docker pull spiped@sha256:a5232683a5bf13534483003265ab6cb9e3e55aee61cd5b4d2a191f17e03df617
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.1 MB (3050234 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f1a6d99184d1632163ebb9749eb334c1c33400fb870ffb934ad3a1ebba0996a9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 17 Feb 2021 21:38:34 GMT
ADD file:eaee53da3c87749799de55809e4a5b526c56855332b961a85b1184c660f1d65b in / 
# Wed, 17 Feb 2021 21:38:35 GMT
CMD ["/bin/sh"]
# Fri, 12 Mar 2021 08:02:19 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 12 Mar 2021 08:02:22 GMT
RUN apk add --no-cache libssl1.1
# Fri, 12 Mar 2021 08:02:22 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 12 Mar 2021 08:02:55 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 12 Mar 2021 08:02:55 GMT
VOLUME [/spiped]
# Fri, 12 Mar 2021 08:02:55 GMT
WORKDIR /spiped
# Fri, 12 Mar 2021 08:02:56 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 12 Mar 2021 08:02:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 12 Mar 2021 08:02:57 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:86205afa28f6bc624469015a543d16608258d2828411a92c662f4fdc6d276e18`  
		Last Modified: Wed, 17 Feb 2021 21:39:07 GMT  
		Size: 2.8 MB (2818177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01151086349ecbe9bf1a11e45d99c1cc13e5c802c8b30c0d4b9f1c812e6aea9a`  
		Last Modified: Fri, 12 Mar 2021 08:04:11 GMT  
		Size: 1.3 KB (1257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fefdaca39f4f34ba4bebf1b3db3bf1b02ce180e641aebe39f727fdd5c93728d`  
		Last Modified: Fri, 12 Mar 2021 08:04:11 GMT  
		Size: 7.0 KB (7041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97c9ba64f9b93ee3b970ffa96d2893600f07fc944fb30646a6511871b10f34b5`  
		Last Modified: Fri, 12 Mar 2021 08:04:11 GMT  
		Size: 223.3 KB (223292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5b3ca1f69125fe405d74ac176bb7c66b78a39aa626a7e5cb5fe3bdaa43b9fc5`  
		Last Modified: Fri, 12 Mar 2021 08:04:11 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5dcd5852a27cc455abd1b6ae425ba7ae69a62b0ae42dd0fc45c1f9993fc79d7`  
		Last Modified: Fri, 12 Mar 2021 08:04:11 GMT  
		Size: 338.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; ppc64le

```console
$ docker pull spiped@sha256:c289f487ff74d19e50727c07507d1609f142b15a496f3e829a8232e797f8fa86
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (3042847 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5452ec7d0568f7fa053d286ed0069f9ddd4be9dde9b516049498ade4047aa340`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 17 Feb 2021 21:17:29 GMT
ADD file:28f4377c61c0f8eb43a6b36e6a24ef5893f51d405d25b62e364988223537ae0b in / 
# Wed, 17 Feb 2021 21:17:37 GMT
CMD ["/bin/sh"]
# Thu, 18 Feb 2021 03:26:01 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 18 Feb 2021 03:26:27 GMT
RUN apk add --no-cache libssl1.1
# Thu, 18 Feb 2021 03:26:34 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 18 Feb 2021 03:27:18 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Thu, 18 Feb 2021 03:27:34 GMT
VOLUME [/spiped]
# Thu, 18 Feb 2021 03:27:46 GMT
WORKDIR /spiped
# Thu, 18 Feb 2021 03:27:51 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 18 Feb 2021 03:28:03 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 18 Feb 2021 03:28:09 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:cb672e0375a8f9bb3d33049ceb372ffa49b959bfc84fe6f72bfb97b682a608c8`  
		Last Modified: Wed, 17 Feb 2021 21:18:10 GMT  
		Size: 2.8 MB (2813081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60920645f2e5501fee7aa26e0c7d56e1e6b86944323cc7d2bc446665f8f00296`  
		Last Modified: Thu, 18 Feb 2021 03:28:43 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99be5791d197e7173e97bcde4c0cb34e0b0b041b0cfd0dd2e52ee1aeac336327`  
		Last Modified: Thu, 18 Feb 2021 03:28:43 GMT  
		Size: 7.1 KB (7058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b707542d6d894ec7ee45192bff36b0d35538f59e7f201a07e84ba7b2b3d9a216`  
		Last Modified: Thu, 18 Feb 2021 03:28:43 GMT  
		Size: 221.0 KB (220976 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:646679d9c65db513723f9e3d9b1e14a6ff198910adb40d95218a19fd2075e12c`  
		Last Modified: Thu, 18 Feb 2021 03:28:43 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d625be0be9dedbd5e83f126a8a7cce9eb5ca9932ee03459ebb286fbaca7fa39f`  
		Last Modified: Thu, 18 Feb 2021 03:28:43 GMT  
		Size: 343.0 B  
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
$ docker pull spiped@sha256:7059805cf01965859918fa9d47d36661a2527a3cafd2dc66d92d2c54b7f5c7a4
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
$ docker pull spiped@sha256:48c027238fbc19554916ff378bed97ea4f5fd5c603e280747d70562648af3472
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (3032749 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:337c259d969e84592201606f94892febf289ce47a0d407e08a069666c2d69a77`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 17 Feb 2021 21:19:54 GMT
ADD file:80bf8bd014071345b1c0364eeb0a5e48f3fb0d87f9c31cb990e57caa652b59b8 in / 
# Wed, 17 Feb 2021 21:19:54 GMT
CMD ["/bin/sh"]
# Fri, 12 Mar 2021 13:35:19 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 12 Mar 2021 13:35:20 GMT
RUN apk add --no-cache libssl1.1
# Fri, 12 Mar 2021 13:35:20 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 12 Mar 2021 13:35:38 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 12 Mar 2021 13:35:38 GMT
VOLUME [/spiped]
# Fri, 12 Mar 2021 13:35:39 GMT
WORKDIR /spiped
# Fri, 12 Mar 2021 13:35:39 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 12 Mar 2021 13:35:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 12 Mar 2021 13:35:39 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:ba3557a56b150f9b813f9d02274d62914fd8fce120dd374d9ee17b87cf1d277d`  
		Last Modified: Wed, 17 Feb 2021 21:20:25 GMT  
		Size: 2.8 MB (2811657 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08ee8075a0364f96f14fb19f0cf1699bba69bbbd6ecb1346e65bf6f53789ec3f`  
		Last Modified: Fri, 12 Mar 2021 13:36:15 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3eb81ccfc669ba7ed08bc8dfbf286026d62b567a4ee7575ba3468e0f71dcadf8`  
		Last Modified: Fri, 12 Mar 2021 13:36:15 GMT  
		Size: 7.0 KB (7046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49bca945030c802bb92b127f52e8e01ed86d8e3575ed3856ce8f6a95a3e75353`  
		Last Modified: Fri, 12 Mar 2021 13:36:16 GMT  
		Size: 212.3 KB (212315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b234f0abff6e36d72f674d4781560a96fa1c771db2a9333fb53181e5673666c`  
		Last Modified: Fri, 12 Mar 2021 13:36:15 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2209594492d63e6e3a196fbeab335f9be161f51a495d896b89f0597e7386441e`  
		Last Modified: Fri, 12 Mar 2021 13:36:15 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; arm variant v6

```console
$ docker pull spiped@sha256:a4eae04b6b59fa1465464612d582ab381eae7d0fd508089e99a2d9642d83d589
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 MB (2833085 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:efa0d64ae65bd0aed1fae629f2219ead07f2df4d55520aa67fa73701725be6a4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 17 Feb 2021 20:49:32 GMT
ADD file:c04fbd3b039001c592cfa14f8388f8934ed4223ccf274dbb926e75039e172af4 in / 
# Wed, 17 Feb 2021 20:49:33 GMT
CMD ["/bin/sh"]
# Thu, 18 Feb 2021 01:08:57 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 18 Feb 2021 01:09:00 GMT
RUN apk add --no-cache libssl1.1
# Thu, 18 Feb 2021 01:09:00 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 18 Feb 2021 01:09:29 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Thu, 18 Feb 2021 01:09:29 GMT
VOLUME [/spiped]
# Thu, 18 Feb 2021 01:09:30 GMT
WORKDIR /spiped
# Thu, 18 Feb 2021 01:09:31 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 18 Feb 2021 01:09:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 18 Feb 2021 01:09:34 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:1353527ebe111f9bb1e271264a3c182e909e4b36463f80d7dbde1be0713eb892`  
		Last Modified: Wed, 17 Feb 2021 20:50:06 GMT  
		Size: 2.6 MB (2622039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56478beef0e3bf335b5084e01725a07c247a0df1c2ae4d79a9b37d8d7c1d8c6b`  
		Last Modified: Thu, 18 Feb 2021 01:09:52 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09965b504ec1fcd372f0f74e2de05a28c8cfc7546e5f9abac13b9969308fffc7`  
		Last Modified: Thu, 18 Feb 2021 01:09:52 GMT  
		Size: 7.1 KB (7053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ca4d95213096352ef307626e2b9b743cd56d9e041d9bad475b082bdda7cd8fb`  
		Last Modified: Thu, 18 Feb 2021 01:09:52 GMT  
		Size: 202.3 KB (202264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:448a184417c9c40109716c2bf6eb26c63873720e7d14b4e852ffe5da738e4871`  
		Last Modified: Thu, 18 Feb 2021 01:09:52 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fb506bcaf6432a313382d4600f3ae27df33c73cfc17f1d9615fee63b17b95c3`  
		Last Modified: Thu, 18 Feb 2021 01:09:51 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; arm variant v7

```console
$ docker pull spiped@sha256:e91e8dfd1379e2029d929ab8d21b5b7cacda7a1ac496cecd8c37417d9d48e708
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 MB (2628211 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2b8d028bc188683c4af6ec6c0afa9cf33c5e88a0569d98c54eebd1e02b4b78b2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 17 Feb 2021 20:57:36 GMT
ADD file:efdd39e5243eaf378f12ad5a85d2222b44930850a90263e5f17e8a6b5e9bc9b8 in / 
# Wed, 17 Feb 2021 20:57:37 GMT
CMD ["/bin/sh"]
# Thu, 18 Feb 2021 01:11:51 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 18 Feb 2021 01:11:53 GMT
RUN apk add --no-cache libssl1.1
# Thu, 18 Feb 2021 01:11:55 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 18 Feb 2021 01:12:23 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Thu, 18 Feb 2021 01:12:24 GMT
VOLUME [/spiped]
# Thu, 18 Feb 2021 01:12:25 GMT
WORKDIR /spiped
# Thu, 18 Feb 2021 01:12:26 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 18 Feb 2021 01:12:27 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 18 Feb 2021 01:12:27 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:f55b840e27d3dbe27e44497103a4397f043749f933eb0433d29e2f104b3435ef`  
		Last Modified: Wed, 17 Feb 2021 20:58:14 GMT  
		Size: 2.4 MB (2423892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfdfb8a36c4de90dba3240099eb1d0348f8627ed1bc968f7e4271d75b265ccf2`  
		Last Modified: Thu, 18 Feb 2021 01:12:49 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35ab61a202577acd7159b1a345fcb97d20c63e42a6a170dfe22345caa4af688f`  
		Last Modified: Thu, 18 Feb 2021 01:12:49 GMT  
		Size: 7.1 KB (7051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:374409fe6217df96932998b712912ebad072a21d4d4e7817b70b6dbb23d0f0a3`  
		Last Modified: Thu, 18 Feb 2021 01:12:49 GMT  
		Size: 195.5 KB (195539 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:592de5c2b9cc50ddf43d871cb052d160ae2dc235c136a1731e45e1cf529b7b80`  
		Last Modified: Thu, 18 Feb 2021 01:12:49 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:562929d72557b487b48b0dcc0ca66188d993a95431efb6ba6e82ecece7035616`  
		Last Modified: Thu, 18 Feb 2021 01:12:49 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:b0ca7cbad488b0fcb44506f1c6c65ae77f5573dc072c30c390b75e29a9d2c64c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 MB (2924800 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bffde3212b34beb453841e58f5ca6bcdbd5dee1c658ff1861926718f1f9c5499`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 17 Feb 2021 20:39:29 GMT
ADD file:3bf1497bd250cf7c73c12231dc4ebe3a3a67f2cd99e35bce47ef6674683aeb1d in / 
# Wed, 17 Feb 2021 20:39:30 GMT
CMD ["/bin/sh"]
# Thu, 18 Feb 2021 01:23:27 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 18 Feb 2021 01:23:30 GMT
RUN apk add --no-cache libssl1.1
# Thu, 18 Feb 2021 01:23:31 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 18 Feb 2021 01:24:04 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Thu, 18 Feb 2021 01:24:05 GMT
VOLUME [/spiped]
# Thu, 18 Feb 2021 01:24:06 GMT
WORKDIR /spiped
# Thu, 18 Feb 2021 01:24:07 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 18 Feb 2021 01:24:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 18 Feb 2021 01:24:10 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:069a56d6d07f6b186fbb82e4486616b9be9a37ce32a63013af6cddcb65898182`  
		Last Modified: Wed, 17 Feb 2021 20:40:04 GMT  
		Size: 2.7 MB (2711572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:991947bc8299281c0212c4f9312423d52074ad210f1eab639db0f6df247937b2`  
		Last Modified: Thu, 18 Feb 2021 01:24:34 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83a8e0ee83f949ca3f11000f9df3c4b551cff205fc9d645ed6aa3c13d4b41a14`  
		Last Modified: Thu, 18 Feb 2021 01:24:34 GMT  
		Size: 7.1 KB (7059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6da8757762737713d5ff919736307c7a18ea61e4e68e7a6f051974461de14f8a`  
		Last Modified: Thu, 18 Feb 2021 01:24:34 GMT  
		Size: 204.4 KB (204440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13a12b508a6a8ce19fd3eee0367c035a60aebd09e422b169e7e3acb5ec2cc376`  
		Last Modified: Thu, 18 Feb 2021 01:24:34 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd46a081f7acce468799a1512f765f8f304e396d48824de8d10a33c1e6416619`  
		Last Modified: Thu, 18 Feb 2021 01:24:34 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; 386

```console
$ docker pull spiped@sha256:a5232683a5bf13534483003265ab6cb9e3e55aee61cd5b4d2a191f17e03df617
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.1 MB (3050234 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f1a6d99184d1632163ebb9749eb334c1c33400fb870ffb934ad3a1ebba0996a9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 17 Feb 2021 21:38:34 GMT
ADD file:eaee53da3c87749799de55809e4a5b526c56855332b961a85b1184c660f1d65b in / 
# Wed, 17 Feb 2021 21:38:35 GMT
CMD ["/bin/sh"]
# Fri, 12 Mar 2021 08:02:19 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 12 Mar 2021 08:02:22 GMT
RUN apk add --no-cache libssl1.1
# Fri, 12 Mar 2021 08:02:22 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 12 Mar 2021 08:02:55 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 12 Mar 2021 08:02:55 GMT
VOLUME [/spiped]
# Fri, 12 Mar 2021 08:02:55 GMT
WORKDIR /spiped
# Fri, 12 Mar 2021 08:02:56 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 12 Mar 2021 08:02:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 12 Mar 2021 08:02:57 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:86205afa28f6bc624469015a543d16608258d2828411a92c662f4fdc6d276e18`  
		Last Modified: Wed, 17 Feb 2021 21:39:07 GMT  
		Size: 2.8 MB (2818177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01151086349ecbe9bf1a11e45d99c1cc13e5c802c8b30c0d4b9f1c812e6aea9a`  
		Last Modified: Fri, 12 Mar 2021 08:04:11 GMT  
		Size: 1.3 KB (1257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fefdaca39f4f34ba4bebf1b3db3bf1b02ce180e641aebe39f727fdd5c93728d`  
		Last Modified: Fri, 12 Mar 2021 08:04:11 GMT  
		Size: 7.0 KB (7041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97c9ba64f9b93ee3b970ffa96d2893600f07fc944fb30646a6511871b10f34b5`  
		Last Modified: Fri, 12 Mar 2021 08:04:11 GMT  
		Size: 223.3 KB (223292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5b3ca1f69125fe405d74ac176bb7c66b78a39aa626a7e5cb5fe3bdaa43b9fc5`  
		Last Modified: Fri, 12 Mar 2021 08:04:11 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5dcd5852a27cc455abd1b6ae425ba7ae69a62b0ae42dd0fc45c1f9993fc79d7`  
		Last Modified: Fri, 12 Mar 2021 08:04:11 GMT  
		Size: 338.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; ppc64le

```console
$ docker pull spiped@sha256:c289f487ff74d19e50727c07507d1609f142b15a496f3e829a8232e797f8fa86
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (3042847 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5452ec7d0568f7fa053d286ed0069f9ddd4be9dde9b516049498ade4047aa340`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 17 Feb 2021 21:17:29 GMT
ADD file:28f4377c61c0f8eb43a6b36e6a24ef5893f51d405d25b62e364988223537ae0b in / 
# Wed, 17 Feb 2021 21:17:37 GMT
CMD ["/bin/sh"]
# Thu, 18 Feb 2021 03:26:01 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 18 Feb 2021 03:26:27 GMT
RUN apk add --no-cache libssl1.1
# Thu, 18 Feb 2021 03:26:34 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 18 Feb 2021 03:27:18 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Thu, 18 Feb 2021 03:27:34 GMT
VOLUME [/spiped]
# Thu, 18 Feb 2021 03:27:46 GMT
WORKDIR /spiped
# Thu, 18 Feb 2021 03:27:51 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 18 Feb 2021 03:28:03 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 18 Feb 2021 03:28:09 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:cb672e0375a8f9bb3d33049ceb372ffa49b959bfc84fe6f72bfb97b682a608c8`  
		Last Modified: Wed, 17 Feb 2021 21:18:10 GMT  
		Size: 2.8 MB (2813081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60920645f2e5501fee7aa26e0c7d56e1e6b86944323cc7d2bc446665f8f00296`  
		Last Modified: Thu, 18 Feb 2021 03:28:43 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99be5791d197e7173e97bcde4c0cb34e0b0b041b0cfd0dd2e52ee1aeac336327`  
		Last Modified: Thu, 18 Feb 2021 03:28:43 GMT  
		Size: 7.1 KB (7058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b707542d6d894ec7ee45192bff36b0d35538f59e7f201a07e84ba7b2b3d9a216`  
		Last Modified: Thu, 18 Feb 2021 03:28:43 GMT  
		Size: 221.0 KB (220976 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:646679d9c65db513723f9e3d9b1e14a6ff198910adb40d95218a19fd2075e12c`  
		Last Modified: Thu, 18 Feb 2021 03:28:43 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d625be0be9dedbd5e83f126a8a7cce9eb5ca9932ee03459ebb286fbaca7fa39f`  
		Last Modified: Thu, 18 Feb 2021 03:28:43 GMT  
		Size: 343.0 B  
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
$ docker pull spiped@sha256:7059805cf01965859918fa9d47d36661a2527a3cafd2dc66d92d2c54b7f5c7a4
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
$ docker pull spiped@sha256:48c027238fbc19554916ff378bed97ea4f5fd5c603e280747d70562648af3472
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (3032749 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:337c259d969e84592201606f94892febf289ce47a0d407e08a069666c2d69a77`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 17 Feb 2021 21:19:54 GMT
ADD file:80bf8bd014071345b1c0364eeb0a5e48f3fb0d87f9c31cb990e57caa652b59b8 in / 
# Wed, 17 Feb 2021 21:19:54 GMT
CMD ["/bin/sh"]
# Fri, 12 Mar 2021 13:35:19 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 12 Mar 2021 13:35:20 GMT
RUN apk add --no-cache libssl1.1
# Fri, 12 Mar 2021 13:35:20 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 12 Mar 2021 13:35:38 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 12 Mar 2021 13:35:38 GMT
VOLUME [/spiped]
# Fri, 12 Mar 2021 13:35:39 GMT
WORKDIR /spiped
# Fri, 12 Mar 2021 13:35:39 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 12 Mar 2021 13:35:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 12 Mar 2021 13:35:39 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:ba3557a56b150f9b813f9d02274d62914fd8fce120dd374d9ee17b87cf1d277d`  
		Last Modified: Wed, 17 Feb 2021 21:20:25 GMT  
		Size: 2.8 MB (2811657 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08ee8075a0364f96f14fb19f0cf1699bba69bbbd6ecb1346e65bf6f53789ec3f`  
		Last Modified: Fri, 12 Mar 2021 13:36:15 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3eb81ccfc669ba7ed08bc8dfbf286026d62b567a4ee7575ba3468e0f71dcadf8`  
		Last Modified: Fri, 12 Mar 2021 13:36:15 GMT  
		Size: 7.0 KB (7046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49bca945030c802bb92b127f52e8e01ed86d8e3575ed3856ce8f6a95a3e75353`  
		Last Modified: Fri, 12 Mar 2021 13:36:16 GMT  
		Size: 212.3 KB (212315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b234f0abff6e36d72f674d4781560a96fa1c771db2a9333fb53181e5673666c`  
		Last Modified: Fri, 12 Mar 2021 13:36:15 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2209594492d63e6e3a196fbeab335f9be161f51a495d896b89f0597e7386441e`  
		Last Modified: Fri, 12 Mar 2021 13:36:15 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1-alpine` - linux; arm variant v6

```console
$ docker pull spiped@sha256:a4eae04b6b59fa1465464612d582ab381eae7d0fd508089e99a2d9642d83d589
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 MB (2833085 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:efa0d64ae65bd0aed1fae629f2219ead07f2df4d55520aa67fa73701725be6a4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 17 Feb 2021 20:49:32 GMT
ADD file:c04fbd3b039001c592cfa14f8388f8934ed4223ccf274dbb926e75039e172af4 in / 
# Wed, 17 Feb 2021 20:49:33 GMT
CMD ["/bin/sh"]
# Thu, 18 Feb 2021 01:08:57 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 18 Feb 2021 01:09:00 GMT
RUN apk add --no-cache libssl1.1
# Thu, 18 Feb 2021 01:09:00 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 18 Feb 2021 01:09:29 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Thu, 18 Feb 2021 01:09:29 GMT
VOLUME [/spiped]
# Thu, 18 Feb 2021 01:09:30 GMT
WORKDIR /spiped
# Thu, 18 Feb 2021 01:09:31 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 18 Feb 2021 01:09:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 18 Feb 2021 01:09:34 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:1353527ebe111f9bb1e271264a3c182e909e4b36463f80d7dbde1be0713eb892`  
		Last Modified: Wed, 17 Feb 2021 20:50:06 GMT  
		Size: 2.6 MB (2622039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56478beef0e3bf335b5084e01725a07c247a0df1c2ae4d79a9b37d8d7c1d8c6b`  
		Last Modified: Thu, 18 Feb 2021 01:09:52 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09965b504ec1fcd372f0f74e2de05a28c8cfc7546e5f9abac13b9969308fffc7`  
		Last Modified: Thu, 18 Feb 2021 01:09:52 GMT  
		Size: 7.1 KB (7053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ca4d95213096352ef307626e2b9b743cd56d9e041d9bad475b082bdda7cd8fb`  
		Last Modified: Thu, 18 Feb 2021 01:09:52 GMT  
		Size: 202.3 KB (202264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:448a184417c9c40109716c2bf6eb26c63873720e7d14b4e852ffe5da738e4871`  
		Last Modified: Thu, 18 Feb 2021 01:09:52 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fb506bcaf6432a313382d4600f3ae27df33c73cfc17f1d9615fee63b17b95c3`  
		Last Modified: Thu, 18 Feb 2021 01:09:51 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1-alpine` - linux; arm variant v7

```console
$ docker pull spiped@sha256:e91e8dfd1379e2029d929ab8d21b5b7cacda7a1ac496cecd8c37417d9d48e708
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 MB (2628211 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2b8d028bc188683c4af6ec6c0afa9cf33c5e88a0569d98c54eebd1e02b4b78b2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 17 Feb 2021 20:57:36 GMT
ADD file:efdd39e5243eaf378f12ad5a85d2222b44930850a90263e5f17e8a6b5e9bc9b8 in / 
# Wed, 17 Feb 2021 20:57:37 GMT
CMD ["/bin/sh"]
# Thu, 18 Feb 2021 01:11:51 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 18 Feb 2021 01:11:53 GMT
RUN apk add --no-cache libssl1.1
# Thu, 18 Feb 2021 01:11:55 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 18 Feb 2021 01:12:23 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Thu, 18 Feb 2021 01:12:24 GMT
VOLUME [/spiped]
# Thu, 18 Feb 2021 01:12:25 GMT
WORKDIR /spiped
# Thu, 18 Feb 2021 01:12:26 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 18 Feb 2021 01:12:27 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 18 Feb 2021 01:12:27 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:f55b840e27d3dbe27e44497103a4397f043749f933eb0433d29e2f104b3435ef`  
		Last Modified: Wed, 17 Feb 2021 20:58:14 GMT  
		Size: 2.4 MB (2423892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfdfb8a36c4de90dba3240099eb1d0348f8627ed1bc968f7e4271d75b265ccf2`  
		Last Modified: Thu, 18 Feb 2021 01:12:49 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35ab61a202577acd7159b1a345fcb97d20c63e42a6a170dfe22345caa4af688f`  
		Last Modified: Thu, 18 Feb 2021 01:12:49 GMT  
		Size: 7.1 KB (7051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:374409fe6217df96932998b712912ebad072a21d4d4e7817b70b6dbb23d0f0a3`  
		Last Modified: Thu, 18 Feb 2021 01:12:49 GMT  
		Size: 195.5 KB (195539 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:592de5c2b9cc50ddf43d871cb052d160ae2dc235c136a1731e45e1cf529b7b80`  
		Last Modified: Thu, 18 Feb 2021 01:12:49 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:562929d72557b487b48b0dcc0ca66188d993a95431efb6ba6e82ecece7035616`  
		Last Modified: Thu, 18 Feb 2021 01:12:49 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1-alpine` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:b0ca7cbad488b0fcb44506f1c6c65ae77f5573dc072c30c390b75e29a9d2c64c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 MB (2924800 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bffde3212b34beb453841e58f5ca6bcdbd5dee1c658ff1861926718f1f9c5499`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 17 Feb 2021 20:39:29 GMT
ADD file:3bf1497bd250cf7c73c12231dc4ebe3a3a67f2cd99e35bce47ef6674683aeb1d in / 
# Wed, 17 Feb 2021 20:39:30 GMT
CMD ["/bin/sh"]
# Thu, 18 Feb 2021 01:23:27 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 18 Feb 2021 01:23:30 GMT
RUN apk add --no-cache libssl1.1
# Thu, 18 Feb 2021 01:23:31 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 18 Feb 2021 01:24:04 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Thu, 18 Feb 2021 01:24:05 GMT
VOLUME [/spiped]
# Thu, 18 Feb 2021 01:24:06 GMT
WORKDIR /spiped
# Thu, 18 Feb 2021 01:24:07 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 18 Feb 2021 01:24:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 18 Feb 2021 01:24:10 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:069a56d6d07f6b186fbb82e4486616b9be9a37ce32a63013af6cddcb65898182`  
		Last Modified: Wed, 17 Feb 2021 20:40:04 GMT  
		Size: 2.7 MB (2711572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:991947bc8299281c0212c4f9312423d52074ad210f1eab639db0f6df247937b2`  
		Last Modified: Thu, 18 Feb 2021 01:24:34 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83a8e0ee83f949ca3f11000f9df3c4b551cff205fc9d645ed6aa3c13d4b41a14`  
		Last Modified: Thu, 18 Feb 2021 01:24:34 GMT  
		Size: 7.1 KB (7059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6da8757762737713d5ff919736307c7a18ea61e4e68e7a6f051974461de14f8a`  
		Last Modified: Thu, 18 Feb 2021 01:24:34 GMT  
		Size: 204.4 KB (204440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13a12b508a6a8ce19fd3eee0367c035a60aebd09e422b169e7e3acb5ec2cc376`  
		Last Modified: Thu, 18 Feb 2021 01:24:34 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd46a081f7acce468799a1512f765f8f304e396d48824de8d10a33c1e6416619`  
		Last Modified: Thu, 18 Feb 2021 01:24:34 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1-alpine` - linux; 386

```console
$ docker pull spiped@sha256:a5232683a5bf13534483003265ab6cb9e3e55aee61cd5b4d2a191f17e03df617
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.1 MB (3050234 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f1a6d99184d1632163ebb9749eb334c1c33400fb870ffb934ad3a1ebba0996a9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 17 Feb 2021 21:38:34 GMT
ADD file:eaee53da3c87749799de55809e4a5b526c56855332b961a85b1184c660f1d65b in / 
# Wed, 17 Feb 2021 21:38:35 GMT
CMD ["/bin/sh"]
# Fri, 12 Mar 2021 08:02:19 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 12 Mar 2021 08:02:22 GMT
RUN apk add --no-cache libssl1.1
# Fri, 12 Mar 2021 08:02:22 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 12 Mar 2021 08:02:55 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 12 Mar 2021 08:02:55 GMT
VOLUME [/spiped]
# Fri, 12 Mar 2021 08:02:55 GMT
WORKDIR /spiped
# Fri, 12 Mar 2021 08:02:56 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 12 Mar 2021 08:02:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 12 Mar 2021 08:02:57 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:86205afa28f6bc624469015a543d16608258d2828411a92c662f4fdc6d276e18`  
		Last Modified: Wed, 17 Feb 2021 21:39:07 GMT  
		Size: 2.8 MB (2818177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01151086349ecbe9bf1a11e45d99c1cc13e5c802c8b30c0d4b9f1c812e6aea9a`  
		Last Modified: Fri, 12 Mar 2021 08:04:11 GMT  
		Size: 1.3 KB (1257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fefdaca39f4f34ba4bebf1b3db3bf1b02ce180e641aebe39f727fdd5c93728d`  
		Last Modified: Fri, 12 Mar 2021 08:04:11 GMT  
		Size: 7.0 KB (7041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97c9ba64f9b93ee3b970ffa96d2893600f07fc944fb30646a6511871b10f34b5`  
		Last Modified: Fri, 12 Mar 2021 08:04:11 GMT  
		Size: 223.3 KB (223292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5b3ca1f69125fe405d74ac176bb7c66b78a39aa626a7e5cb5fe3bdaa43b9fc5`  
		Last Modified: Fri, 12 Mar 2021 08:04:11 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5dcd5852a27cc455abd1b6ae425ba7ae69a62b0ae42dd0fc45c1f9993fc79d7`  
		Last Modified: Fri, 12 Mar 2021 08:04:11 GMT  
		Size: 338.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.1-alpine` - linux; ppc64le

```console
$ docker pull spiped@sha256:c289f487ff74d19e50727c07507d1609f142b15a496f3e829a8232e797f8fa86
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (3042847 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5452ec7d0568f7fa053d286ed0069f9ddd4be9dde9b516049498ade4047aa340`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 17 Feb 2021 21:17:29 GMT
ADD file:28f4377c61c0f8eb43a6b36e6a24ef5893f51d405d25b62e364988223537ae0b in / 
# Wed, 17 Feb 2021 21:17:37 GMT
CMD ["/bin/sh"]
# Thu, 18 Feb 2021 03:26:01 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 18 Feb 2021 03:26:27 GMT
RUN apk add --no-cache libssl1.1
# Thu, 18 Feb 2021 03:26:34 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 18 Feb 2021 03:27:18 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Thu, 18 Feb 2021 03:27:34 GMT
VOLUME [/spiped]
# Thu, 18 Feb 2021 03:27:46 GMT
WORKDIR /spiped
# Thu, 18 Feb 2021 03:27:51 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 18 Feb 2021 03:28:03 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 18 Feb 2021 03:28:09 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:cb672e0375a8f9bb3d33049ceb372ffa49b959bfc84fe6f72bfb97b682a608c8`  
		Last Modified: Wed, 17 Feb 2021 21:18:10 GMT  
		Size: 2.8 MB (2813081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60920645f2e5501fee7aa26e0c7d56e1e6b86944323cc7d2bc446665f8f00296`  
		Last Modified: Thu, 18 Feb 2021 03:28:43 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99be5791d197e7173e97bcde4c0cb34e0b0b041b0cfd0dd2e52ee1aeac336327`  
		Last Modified: Thu, 18 Feb 2021 03:28:43 GMT  
		Size: 7.1 KB (7058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b707542d6d894ec7ee45192bff36b0d35538f59e7f201a07e84ba7b2b3d9a216`  
		Last Modified: Thu, 18 Feb 2021 03:28:43 GMT  
		Size: 221.0 KB (220976 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:646679d9c65db513723f9e3d9b1e14a6ff198910adb40d95218a19fd2075e12c`  
		Last Modified: Thu, 18 Feb 2021 03:28:43 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d625be0be9dedbd5e83f126a8a7cce9eb5ca9932ee03459ebb286fbaca7fa39f`  
		Last Modified: Thu, 18 Feb 2021 03:28:43 GMT  
		Size: 343.0 B  
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
$ docker pull spiped@sha256:7059805cf01965859918fa9d47d36661a2527a3cafd2dc66d92d2c54b7f5c7a4
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
$ docker pull spiped@sha256:48c027238fbc19554916ff378bed97ea4f5fd5c603e280747d70562648af3472
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (3032749 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:337c259d969e84592201606f94892febf289ce47a0d407e08a069666c2d69a77`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 17 Feb 2021 21:19:54 GMT
ADD file:80bf8bd014071345b1c0364eeb0a5e48f3fb0d87f9c31cb990e57caa652b59b8 in / 
# Wed, 17 Feb 2021 21:19:54 GMT
CMD ["/bin/sh"]
# Fri, 12 Mar 2021 13:35:19 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 12 Mar 2021 13:35:20 GMT
RUN apk add --no-cache libssl1.1
# Fri, 12 Mar 2021 13:35:20 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 12 Mar 2021 13:35:38 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 12 Mar 2021 13:35:38 GMT
VOLUME [/spiped]
# Fri, 12 Mar 2021 13:35:39 GMT
WORKDIR /spiped
# Fri, 12 Mar 2021 13:35:39 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 12 Mar 2021 13:35:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 12 Mar 2021 13:35:39 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:ba3557a56b150f9b813f9d02274d62914fd8fce120dd374d9ee17b87cf1d277d`  
		Last Modified: Wed, 17 Feb 2021 21:20:25 GMT  
		Size: 2.8 MB (2811657 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08ee8075a0364f96f14fb19f0cf1699bba69bbbd6ecb1346e65bf6f53789ec3f`  
		Last Modified: Fri, 12 Mar 2021 13:36:15 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3eb81ccfc669ba7ed08bc8dfbf286026d62b567a4ee7575ba3468e0f71dcadf8`  
		Last Modified: Fri, 12 Mar 2021 13:36:15 GMT  
		Size: 7.0 KB (7046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49bca945030c802bb92b127f52e8e01ed86d8e3575ed3856ce8f6a95a3e75353`  
		Last Modified: Fri, 12 Mar 2021 13:36:16 GMT  
		Size: 212.3 KB (212315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b234f0abff6e36d72f674d4781560a96fa1c771db2a9333fb53181e5673666c`  
		Last Modified: Fri, 12 Mar 2021 13:36:15 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2209594492d63e6e3a196fbeab335f9be161f51a495d896b89f0597e7386441e`  
		Last Modified: Fri, 12 Mar 2021 13:36:15 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; arm variant v6

```console
$ docker pull spiped@sha256:a4eae04b6b59fa1465464612d582ab381eae7d0fd508089e99a2d9642d83d589
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 MB (2833085 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:efa0d64ae65bd0aed1fae629f2219ead07f2df4d55520aa67fa73701725be6a4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 17 Feb 2021 20:49:32 GMT
ADD file:c04fbd3b039001c592cfa14f8388f8934ed4223ccf274dbb926e75039e172af4 in / 
# Wed, 17 Feb 2021 20:49:33 GMT
CMD ["/bin/sh"]
# Thu, 18 Feb 2021 01:08:57 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 18 Feb 2021 01:09:00 GMT
RUN apk add --no-cache libssl1.1
# Thu, 18 Feb 2021 01:09:00 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 18 Feb 2021 01:09:29 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Thu, 18 Feb 2021 01:09:29 GMT
VOLUME [/spiped]
# Thu, 18 Feb 2021 01:09:30 GMT
WORKDIR /spiped
# Thu, 18 Feb 2021 01:09:31 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 18 Feb 2021 01:09:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 18 Feb 2021 01:09:34 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:1353527ebe111f9bb1e271264a3c182e909e4b36463f80d7dbde1be0713eb892`  
		Last Modified: Wed, 17 Feb 2021 20:50:06 GMT  
		Size: 2.6 MB (2622039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56478beef0e3bf335b5084e01725a07c247a0df1c2ae4d79a9b37d8d7c1d8c6b`  
		Last Modified: Thu, 18 Feb 2021 01:09:52 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09965b504ec1fcd372f0f74e2de05a28c8cfc7546e5f9abac13b9969308fffc7`  
		Last Modified: Thu, 18 Feb 2021 01:09:52 GMT  
		Size: 7.1 KB (7053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ca4d95213096352ef307626e2b9b743cd56d9e041d9bad475b082bdda7cd8fb`  
		Last Modified: Thu, 18 Feb 2021 01:09:52 GMT  
		Size: 202.3 KB (202264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:448a184417c9c40109716c2bf6eb26c63873720e7d14b4e852ffe5da738e4871`  
		Last Modified: Thu, 18 Feb 2021 01:09:52 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fb506bcaf6432a313382d4600f3ae27df33c73cfc17f1d9615fee63b17b95c3`  
		Last Modified: Thu, 18 Feb 2021 01:09:51 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; arm variant v7

```console
$ docker pull spiped@sha256:e91e8dfd1379e2029d929ab8d21b5b7cacda7a1ac496cecd8c37417d9d48e708
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 MB (2628211 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2b8d028bc188683c4af6ec6c0afa9cf33c5e88a0569d98c54eebd1e02b4b78b2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 17 Feb 2021 20:57:36 GMT
ADD file:efdd39e5243eaf378f12ad5a85d2222b44930850a90263e5f17e8a6b5e9bc9b8 in / 
# Wed, 17 Feb 2021 20:57:37 GMT
CMD ["/bin/sh"]
# Thu, 18 Feb 2021 01:11:51 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 18 Feb 2021 01:11:53 GMT
RUN apk add --no-cache libssl1.1
# Thu, 18 Feb 2021 01:11:55 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 18 Feb 2021 01:12:23 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Thu, 18 Feb 2021 01:12:24 GMT
VOLUME [/spiped]
# Thu, 18 Feb 2021 01:12:25 GMT
WORKDIR /spiped
# Thu, 18 Feb 2021 01:12:26 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 18 Feb 2021 01:12:27 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 18 Feb 2021 01:12:27 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:f55b840e27d3dbe27e44497103a4397f043749f933eb0433d29e2f104b3435ef`  
		Last Modified: Wed, 17 Feb 2021 20:58:14 GMT  
		Size: 2.4 MB (2423892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfdfb8a36c4de90dba3240099eb1d0348f8627ed1bc968f7e4271d75b265ccf2`  
		Last Modified: Thu, 18 Feb 2021 01:12:49 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35ab61a202577acd7159b1a345fcb97d20c63e42a6a170dfe22345caa4af688f`  
		Last Modified: Thu, 18 Feb 2021 01:12:49 GMT  
		Size: 7.1 KB (7051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:374409fe6217df96932998b712912ebad072a21d4d4e7817b70b6dbb23d0f0a3`  
		Last Modified: Thu, 18 Feb 2021 01:12:49 GMT  
		Size: 195.5 KB (195539 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:592de5c2b9cc50ddf43d871cb052d160ae2dc235c136a1731e45e1cf529b7b80`  
		Last Modified: Thu, 18 Feb 2021 01:12:49 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:562929d72557b487b48b0dcc0ca66188d993a95431efb6ba6e82ecece7035616`  
		Last Modified: Thu, 18 Feb 2021 01:12:49 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:b0ca7cbad488b0fcb44506f1c6c65ae77f5573dc072c30c390b75e29a9d2c64c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 MB (2924800 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bffde3212b34beb453841e58f5ca6bcdbd5dee1c658ff1861926718f1f9c5499`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 17 Feb 2021 20:39:29 GMT
ADD file:3bf1497bd250cf7c73c12231dc4ebe3a3a67f2cd99e35bce47ef6674683aeb1d in / 
# Wed, 17 Feb 2021 20:39:30 GMT
CMD ["/bin/sh"]
# Thu, 18 Feb 2021 01:23:27 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 18 Feb 2021 01:23:30 GMT
RUN apk add --no-cache libssl1.1
# Thu, 18 Feb 2021 01:23:31 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 18 Feb 2021 01:24:04 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Thu, 18 Feb 2021 01:24:05 GMT
VOLUME [/spiped]
# Thu, 18 Feb 2021 01:24:06 GMT
WORKDIR /spiped
# Thu, 18 Feb 2021 01:24:07 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 18 Feb 2021 01:24:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 18 Feb 2021 01:24:10 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:069a56d6d07f6b186fbb82e4486616b9be9a37ce32a63013af6cddcb65898182`  
		Last Modified: Wed, 17 Feb 2021 20:40:04 GMT  
		Size: 2.7 MB (2711572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:991947bc8299281c0212c4f9312423d52074ad210f1eab639db0f6df247937b2`  
		Last Modified: Thu, 18 Feb 2021 01:24:34 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83a8e0ee83f949ca3f11000f9df3c4b551cff205fc9d645ed6aa3c13d4b41a14`  
		Last Modified: Thu, 18 Feb 2021 01:24:34 GMT  
		Size: 7.1 KB (7059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6da8757762737713d5ff919736307c7a18ea61e4e68e7a6f051974461de14f8a`  
		Last Modified: Thu, 18 Feb 2021 01:24:34 GMT  
		Size: 204.4 KB (204440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13a12b508a6a8ce19fd3eee0367c035a60aebd09e422b169e7e3acb5ec2cc376`  
		Last Modified: Thu, 18 Feb 2021 01:24:34 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd46a081f7acce468799a1512f765f8f304e396d48824de8d10a33c1e6416619`  
		Last Modified: Thu, 18 Feb 2021 01:24:34 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; 386

```console
$ docker pull spiped@sha256:a5232683a5bf13534483003265ab6cb9e3e55aee61cd5b4d2a191f17e03df617
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.1 MB (3050234 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f1a6d99184d1632163ebb9749eb334c1c33400fb870ffb934ad3a1ebba0996a9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 17 Feb 2021 21:38:34 GMT
ADD file:eaee53da3c87749799de55809e4a5b526c56855332b961a85b1184c660f1d65b in / 
# Wed, 17 Feb 2021 21:38:35 GMT
CMD ["/bin/sh"]
# Fri, 12 Mar 2021 08:02:19 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 12 Mar 2021 08:02:22 GMT
RUN apk add --no-cache libssl1.1
# Fri, 12 Mar 2021 08:02:22 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 12 Mar 2021 08:02:55 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 12 Mar 2021 08:02:55 GMT
VOLUME [/spiped]
# Fri, 12 Mar 2021 08:02:55 GMT
WORKDIR /spiped
# Fri, 12 Mar 2021 08:02:56 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 12 Mar 2021 08:02:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 12 Mar 2021 08:02:57 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:86205afa28f6bc624469015a543d16608258d2828411a92c662f4fdc6d276e18`  
		Last Modified: Wed, 17 Feb 2021 21:39:07 GMT  
		Size: 2.8 MB (2818177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01151086349ecbe9bf1a11e45d99c1cc13e5c802c8b30c0d4b9f1c812e6aea9a`  
		Last Modified: Fri, 12 Mar 2021 08:04:11 GMT  
		Size: 1.3 KB (1257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fefdaca39f4f34ba4bebf1b3db3bf1b02ce180e641aebe39f727fdd5c93728d`  
		Last Modified: Fri, 12 Mar 2021 08:04:11 GMT  
		Size: 7.0 KB (7041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97c9ba64f9b93ee3b970ffa96d2893600f07fc944fb30646a6511871b10f34b5`  
		Last Modified: Fri, 12 Mar 2021 08:04:11 GMT  
		Size: 223.3 KB (223292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5b3ca1f69125fe405d74ac176bb7c66b78a39aa626a7e5cb5fe3bdaa43b9fc5`  
		Last Modified: Fri, 12 Mar 2021 08:04:11 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5dcd5852a27cc455abd1b6ae425ba7ae69a62b0ae42dd0fc45c1f9993fc79d7`  
		Last Modified: Fri, 12 Mar 2021 08:04:11 GMT  
		Size: 338.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; ppc64le

```console
$ docker pull spiped@sha256:c289f487ff74d19e50727c07507d1609f142b15a496f3e829a8232e797f8fa86
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (3042847 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5452ec7d0568f7fa053d286ed0069f9ddd4be9dde9b516049498ade4047aa340`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 17 Feb 2021 21:17:29 GMT
ADD file:28f4377c61c0f8eb43a6b36e6a24ef5893f51d405d25b62e364988223537ae0b in / 
# Wed, 17 Feb 2021 21:17:37 GMT
CMD ["/bin/sh"]
# Thu, 18 Feb 2021 03:26:01 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 18 Feb 2021 03:26:27 GMT
RUN apk add --no-cache libssl1.1
# Thu, 18 Feb 2021 03:26:34 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Thu, 18 Feb 2021 03:27:18 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Thu, 18 Feb 2021 03:27:34 GMT
VOLUME [/spiped]
# Thu, 18 Feb 2021 03:27:46 GMT
WORKDIR /spiped
# Thu, 18 Feb 2021 03:27:51 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 18 Feb 2021 03:28:03 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 18 Feb 2021 03:28:09 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:cb672e0375a8f9bb3d33049ceb372ffa49b959bfc84fe6f72bfb97b682a608c8`  
		Last Modified: Wed, 17 Feb 2021 21:18:10 GMT  
		Size: 2.8 MB (2813081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60920645f2e5501fee7aa26e0c7d56e1e6b86944323cc7d2bc446665f8f00296`  
		Last Modified: Thu, 18 Feb 2021 03:28:43 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99be5791d197e7173e97bcde4c0cb34e0b0b041b0cfd0dd2e52ee1aeac336327`  
		Last Modified: Thu, 18 Feb 2021 03:28:43 GMT  
		Size: 7.1 KB (7058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b707542d6d894ec7ee45192bff36b0d35538f59e7f201a07e84ba7b2b3d9a216`  
		Last Modified: Thu, 18 Feb 2021 03:28:43 GMT  
		Size: 221.0 KB (220976 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:646679d9c65db513723f9e3d9b1e14a6ff198910adb40d95218a19fd2075e12c`  
		Last Modified: Thu, 18 Feb 2021 03:28:43 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d625be0be9dedbd5e83f126a8a7cce9eb5ca9932ee03459ebb286fbaca7fa39f`  
		Last Modified: Thu, 18 Feb 2021 03:28:43 GMT  
		Size: 343.0 B  
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
