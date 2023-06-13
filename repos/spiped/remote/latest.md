## `spiped:latest`

```console
$ docker pull spiped@sha256:45664117f82df90c734b80b011436bb995becb92aedda6105cb7a94ba503ca37
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
$ docker pull spiped@sha256:6e56f898cffedf314d7e78c36169a3c82a3cecb7b3eabcae761df786ffcfa776
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.4 MB (37404848 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c2a5c88f0c911b4337a918ef32508daa452d712618d486a0160cd5793cd361ce`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 23 May 2023 01:20:14 GMT
ADD file:88252a7f118b4d6f55dd5baf49dbcaa053c9d6172c652963c1151fa76f625e44 in / 
# Tue, 23 May 2023 01:20:14 GMT
CMD ["bash"]
# Tue, 23 May 2023 12:26:12 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 23 May 2023 12:26:15 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 12:26:15 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 23 May 2023 12:26:34 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 23 May 2023 12:26:34 GMT
VOLUME [/spiped]
# Tue, 23 May 2023 12:26:34 GMT
WORKDIR /spiped
# Tue, 23 May 2023 12:26:35 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 23 May 2023 12:26:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 23 May 2023 12:26:35 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:f03b40093957615593f2ed142961afb6b540507e0b47e3f7626ba5e02efbbbf1`  
		Last Modified: Tue, 23 May 2023 01:24:08 GMT  
		Size: 31.4 MB (31403586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03ec67773fceb5d595bfdd899df865f6dba186d457790bcbb5651bc6cc99d90d`  
		Last Modified: Tue, 23 May 2023 12:26:49 GMT  
		Size: 1.7 KB (1736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:843a0deb718885d4a7ec0829e15e29d5bf108522d62cb859c1ea655b40de7c37`  
		Last Modified: Tue, 23 May 2023 12:26:49 GMT  
		Size: 1.1 KB (1051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37406cfa1e5f43875100dd643b4ffe1d3d94166b88ca9c89e45c85f9836f4f3f`  
		Last Modified: Tue, 23 May 2023 12:26:50 GMT  
		Size: 6.0 MB (5998006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1da50da921d37b3dd928ff99cbe7041e472193b33f8e7a363565f0918192396`  
		Last Modified: Tue, 23 May 2023 12:26:49 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96e68bb6f8c79f1122c9447e56b77fc1f1f33701394359d7da671620d33ea690`  
		Last Modified: Tue, 23 May 2023 12:26:48 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; arm variant v5

```console
$ docker pull spiped@sha256:24b934455b3743e605c6bf598285166b2f98922c2e70540168f52e94e85d81b7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.0 MB (33950389 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3cbbbfc7c01ffb1a885d62d0f9d9bc3aa5dffa20a2e93693fe183213ac21491f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Mon, 12 Jun 2023 23:48:46 GMT
ADD file:b2773fa62bdb5672863ef317ee1b58de2a6074fe6aa0d8287a7cd0999028d7d2 in / 
# Mon, 12 Jun 2023 23:48:47 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 07:33:23 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 13 Jun 2023 07:33:28 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 07:33:28 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 13 Jun 2023 07:33:47 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 13 Jun 2023 07:33:47 GMT
VOLUME [/spiped]
# Tue, 13 Jun 2023 07:33:47 GMT
WORKDIR /spiped
# Tue, 13 Jun 2023 07:33:47 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 13 Jun 2023 07:33:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 13 Jun 2023 07:33:47 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:c04d7d6633d9b8cf1bfa9f6831ac7dd6f985411cb6307d91c6373085b09b8c19`  
		Last Modified: Mon, 12 Jun 2023 23:52:06 GMT  
		Size: 28.9 MB (28918779 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b671453761c75eb96860befad51cf5f56a865c865b1edac82a4e76091a901e52`  
		Last Modified: Tue, 13 Jun 2023 07:33:55 GMT  
		Size: 1.7 KB (1724 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b02935a3a3e5cd2836a50fe9b609623beb0b1449c4ea462eee32625d65812236`  
		Last Modified: Tue, 13 Jun 2023 07:33:55 GMT  
		Size: 1.1 KB (1050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38c69188f1110abb0c51052c228199a025151e8bbb22d3db5c176bceccf07807`  
		Last Modified: Tue, 13 Jun 2023 07:33:57 GMT  
		Size: 5.0 MB (5028369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31d5598cac813ac241adf1bb133102b83eb8fc297ec6f729d560966565cbba66`  
		Last Modified: Tue, 13 Jun 2023 07:33:56 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86371f5d879ce4f30d7f244fa8e619fd1b394eb0db43bcc1a2dd2f207e806208`  
		Last Modified: Tue, 13 Jun 2023 07:33:55 GMT  
		Size: 338.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; arm variant v7

```console
$ docker pull spiped@sha256:d31399b238dbdb230a9cfa846b14ef9412a90bb5ff332adb61ae284ce0851071
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.3 MB (31330050 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a486cf9f9f999073d91a737a152344b3c381b0b935067881a5467af6d20d8f33`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Mon, 12 Jun 2023 23:58:47 GMT
ADD file:319a24b7e30fc548f9dcf48ad6cee469e8bf7e89c67901cf3851e41e75693489 in / 
# Mon, 12 Jun 2023 23:58:47 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 05:06:39 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 13 Jun 2023 05:06:42 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 05:06:42 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 13 Jun 2023 05:06:59 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 13 Jun 2023 05:06:59 GMT
VOLUME [/spiped]
# Tue, 13 Jun 2023 05:06:59 GMT
WORKDIR /spiped
# Tue, 13 Jun 2023 05:06:59 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 13 Jun 2023 05:06:59 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 13 Jun 2023 05:06:59 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:b7c295cb849275e211d18b720d2349cc84c0038be1a362aca4765ceb3342043c`  
		Last Modified: Tue, 13 Jun 2023 00:04:24 GMT  
		Size: 26.6 MB (26578690 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0b04caa85914b99dff7f4b06947e3e1e8d96a6b2d37f04c5634659980cceb70`  
		Last Modified: Tue, 13 Jun 2023 05:07:09 GMT  
		Size: 1.7 KB (1723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb52c14c652c6a2863c614f6e972d12894ec89c5659c2d01a5ed29f674e236b8`  
		Last Modified: Tue, 13 Jun 2023 05:07:09 GMT  
		Size: 1.1 KB (1050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d51d9d2662c78c76acbbcfc4278436bfa8bb751811d0c0c56dcb6ee71f77be1d`  
		Last Modified: Tue, 13 Jun 2023 05:07:10 GMT  
		Size: 4.7 MB (4748120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5409490fd60a3b969f0918e8285e745a39e831a8902b4edb1cff3eee5e27f95`  
		Last Modified: Tue, 13 Jun 2023 05:07:09 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95d711dc379fb3ea577aadfbc60d33659ed29265ca904ef9ad1b2e7ae9697348`  
		Last Modified: Tue, 13 Jun 2023 05:07:09 GMT  
		Size: 338.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:8a5154f80fcd5049f56d81eaa5fa39c4fd82721f5cc583b6d14bdb7e1b23731f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.3 MB (35326914 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7da60844d4229ac6dffb12604f36f1438e8ff4ed0546651f6ba44ab83acc7c28`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 23 May 2023 00:43:15 GMT
ADD file:0fee550e337f1bd111a7ef785a9553674f25649f37deffa4aa8107ef6445d259 in / 
# Tue, 23 May 2023 00:43:15 GMT
CMD ["bash"]
# Tue, 23 May 2023 07:20:39 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 23 May 2023 07:20:42 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 07:20:42 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 23 May 2023 07:20:57 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 23 May 2023 07:20:57 GMT
VOLUME [/spiped]
# Tue, 23 May 2023 07:20:57 GMT
WORKDIR /spiped
# Tue, 23 May 2023 07:20:57 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 23 May 2023 07:20:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 23 May 2023 07:20:58 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:d981f2c20c93e1c57a46cd87bc5b9a554be5323072a0d0ab4b354aabd237bbcf`  
		Last Modified: Tue, 23 May 2023 00:46:07 GMT  
		Size: 30.1 MB (30052747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8aa8f6bfb1c027bb9f657161080f0ab93d19eebc194113b874d055fdcbfcb460`  
		Last Modified: Tue, 23 May 2023 07:21:10 GMT  
		Size: 1.7 KB (1736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d47a57eada7dc6536f84b1b4335e54a33593d6eb7ec21e4d1033d6ad1e0a86e7`  
		Last Modified: Tue, 23 May 2023 07:21:10 GMT  
		Size: 1.1 KB (1050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9e3fff08fa9daa5729dace8c989618277b41785008308f87afcc87e10c5bbb4`  
		Last Modified: Tue, 23 May 2023 07:21:11 GMT  
		Size: 5.3 MB (5270912 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c03b1322313f66b8edacbb1f3daf86f76fa0bcf2461f8e9b1c8b0182c569c41`  
		Last Modified: Tue, 23 May 2023 07:21:10 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bce57662b8b31a2ce6d26052524b37aa0e54ae5e585421cd7bd6202e7219607`  
		Last Modified: Tue, 23 May 2023 07:21:10 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; 386

```console
$ docker pull spiped@sha256:c86f183f59a1da0d47a0ef90433af289f2f2b7c2d833a89316c34d51afe2d0f1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.3 MB (40282845 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6185bc58ac223183e9461e6107bae7b0e9ca3bbb4338869c1f863ab9c624fa13`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 23 May 2023 00:39:30 GMT
ADD file:8319fc1c1a3c0f2a6bb03636fe1fd0eb7fa52c58505d279e4366627452ea2104 in / 
# Tue, 23 May 2023 00:39:30 GMT
CMD ["bash"]
# Tue, 23 May 2023 01:51:17 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 23 May 2023 01:51:20 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 01:51:20 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 23 May 2023 01:51:43 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 23 May 2023 01:51:43 GMT
VOLUME [/spiped]
# Tue, 23 May 2023 01:51:43 GMT
WORKDIR /spiped
# Tue, 23 May 2023 01:51:43 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 23 May 2023 01:51:43 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 23 May 2023 01:51:44 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:0f5d158483bd0ffef0c106b68514aece2ca0500d2990c830844277cbca7fe0bc`  
		Last Modified: Tue, 23 May 2023 00:44:28 GMT  
		Size: 32.4 MB (32388165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9100966936a8c84c9e0e8b57d0811fb36e0e2c2d3e1138a0d3a7a918fe6745c9`  
		Last Modified: Tue, 23 May 2023 01:51:59 GMT  
		Size: 1.7 KB (1730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57610b2efa5f7c48f7d1ab161334a38849ff14c70658cb48567036e35e685b91`  
		Last Modified: Tue, 23 May 2023 01:51:59 GMT  
		Size: 1.1 KB (1054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a1302ffc3a0d553d137a506717f8c2741436b82ff5b23b4353023fc9a35cd98`  
		Last Modified: Tue, 23 May 2023 01:52:01 GMT  
		Size: 7.9 MB (7891426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed28e099af4805a76b58eb4139bf498ac46acfb4d643ec70c9b840eb827750fb`  
		Last Modified: Tue, 23 May 2023 01:51:59 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ab03d42d20f08b827cfa1c2ef42e597ffbd8333e2237fa7167ad56119457fbb`  
		Last Modified: Tue, 23 May 2023 01:51:59 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; mips64le

```console
$ docker pull spiped@sha256:5048eca6297857f351909c330a9a32c045a8a5656f8a306773cd773ed026ca87
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.3 MB (35342488 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e69bb2dc15afa48fd2a905c1b95630d24cb02183dd2e42a0aea1139444f8b2e0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 13 Jun 2023 00:10:34 GMT
ADD file:4d5c7737e954f157e3d7ea47cc1814c46ec5c753a3d5d828ad9614969b572253 in / 
# Tue, 13 Jun 2023 00:10:38 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 01:43:24 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 13 Jun 2023 01:43:38 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 01:43:41 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 13 Jun 2023 01:45:11 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 13 Jun 2023 01:45:14 GMT
VOLUME [/spiped]
# Tue, 13 Jun 2023 01:45:17 GMT
WORKDIR /spiped
# Tue, 13 Jun 2023 01:45:19 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 13 Jun 2023 01:45:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 13 Jun 2023 01:45:25 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:61bd6562a93acd0a3b327321e5465408e1d921b3ce1fb4fe353633330c3ede91`  
		Last Modified: Tue, 13 Jun 2023 00:23:53 GMT  
		Size: 29.6 MB (29634422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4f0ef0a3861267b4ef08cf448b2f1fc3ade81711b0b5fbd9d6d1581d6d8444f`  
		Last Modified: Tue, 13 Jun 2023 01:45:38 GMT  
		Size: 1.6 KB (1607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a46baf526b17f9846cc40a9942d857383066be6d7b9a763ad5fffe1d117d59b3`  
		Last Modified: Tue, 13 Jun 2023 01:45:37 GMT  
		Size: 923.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b277e66890f62e701bf366cadb6b71924c5cb7a1a7286555f99f64fe3b06207`  
		Last Modified: Tue, 13 Jun 2023 01:45:42 GMT  
		Size: 5.7 MB (5705100 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4fd55e3c4b14927f26b90efaa6ce8242e295488d2b3bba74d8fb002479f80b0`  
		Last Modified: Tue, 13 Jun 2023 01:45:37 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b23161a5a3690af3fa56d7600a2430fad04ac37a3c42eebf022ebd04cc427fb5`  
		Last Modified: Tue, 13 Jun 2023 01:45:38 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; ppc64le

```console
$ docker pull spiped@sha256:e26c208c4a4342785c225a1004342e0114c3561ce9b1530544a567b47005086e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.3 MB (41284428 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c610878704350416c6e781ffc11dc286e43f4fd60173a4e237e7855a91d0ebb6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 23 May 2023 01:17:35 GMT
ADD file:719aea085739ec41c255f35070ca652d4e356c5ee62c8237f8ebc7389feb8e38 in / 
# Tue, 23 May 2023 01:17:37 GMT
CMD ["bash"]
# Tue, 23 May 2023 10:48:59 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 23 May 2023 10:49:05 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 10:49:06 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 23 May 2023 10:49:48 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 23 May 2023 10:49:49 GMT
VOLUME [/spiped]
# Tue, 23 May 2023 10:49:49 GMT
WORKDIR /spiped
# Tue, 23 May 2023 10:49:50 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 23 May 2023 10:49:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 23 May 2023 10:49:50 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:b6c83d2f160e7e38990586d26caa105ff577368a887fd754ae4634cdbfec83ff`  
		Last Modified: Tue, 23 May 2023 01:22:03 GMT  
		Size: 35.3 MB (35280911 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69f4a119486e3fcedd3af8f31d52c720861f5cacee89269ad7e0be2c0ab48eed`  
		Last Modified: Tue, 23 May 2023 10:50:08 GMT  
		Size: 1.7 KB (1736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78b52a815f8a92c8687a8959408e5922807bf95c0905f55a535f52551bf75e6a`  
		Last Modified: Tue, 23 May 2023 10:50:07 GMT  
		Size: 1.1 KB (1052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9b713f962480fbb84f8dd9a119a34339176e1e324df77251b08080ff5c51f96`  
		Last Modified: Tue, 23 May 2023 10:50:10 GMT  
		Size: 6.0 MB (6000259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d48bbdef4e3e839c97da555fe50a2684844e5f2050859146379821c9e9a67e8`  
		Last Modified: Tue, 23 May 2023 10:50:08 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0fd6c48b9797955661de6b1bbdb133281e646ce48bea218e29ecbaa8628958f`  
		Last Modified: Tue, 23 May 2023 10:50:08 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; s390x

```console
$ docker pull spiped@sha256:77c4a743329649cd8376baf45d3d6088c85b35a8ea5721c57edcb0d81618293f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.8 MB (34832955 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:100593e415fe1cca86ecefedad743a9d40d5d926f202e1640dce617d73db3e0a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 23 May 2023 00:42:52 GMT
ADD file:23b1e12559302529556a94a1d4098dbdb454e263265258b940c2b2d23a97c121 in / 
# Tue, 23 May 2023 00:42:54 GMT
CMD ["bash"]
# Tue, 23 May 2023 05:54:21 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 23 May 2023 05:54:24 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 05:54:24 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 23 May 2023 05:54:35 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 23 May 2023 05:54:36 GMT
VOLUME [/spiped]
# Tue, 23 May 2023 05:54:36 GMT
WORKDIR /spiped
# Tue, 23 May 2023 05:54:36 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 23 May 2023 05:54:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 23 May 2023 05:54:36 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:9c24ec455bdb6a9ad0d033c7cce8e71dd5bdbbe53a86d5feeb8d4cb7804fb8e5`  
		Last Modified: Tue, 23 May 2023 00:45:47 GMT  
		Size: 29.6 MB (29642170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b0b30fc529faa1ae767912072bbcccc2766cf1567a698bb67daa62fa10f3f50`  
		Last Modified: Tue, 23 May 2023 05:54:55 GMT  
		Size: 1.7 KB (1738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6dcb25beaa639b1e91802b771b089588a793ca63c16d6e04aa8ba4ca5a5a5e5`  
		Last Modified: Tue, 23 May 2023 05:54:55 GMT  
		Size: 1.1 KB (1055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7464ed886e0c0540af2e338ca3ee908bcc9304c2e6922e098a45971e97ca3d3c`  
		Last Modified: Tue, 23 May 2023 05:54:56 GMT  
		Size: 5.2 MB (5187522 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa28f63af2e817d0c24b1df2d0f6043a0a3d2dac2d8fb740d174f6edbfd68b30`  
		Last Modified: Tue, 23 May 2023 05:54:55 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6499d915f8b515d612f588a84d618d858617e13525e299f6856f58c80df8eaaf`  
		Last Modified: Tue, 23 May 2023 05:54:55 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
