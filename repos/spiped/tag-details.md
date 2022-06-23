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
$ docker pull spiped@sha256:2a04458cf6cb5fa31173ddeeaec6840207e46a3186dbb1e1de6b3c83a009c5d0
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
$ docker pull spiped@sha256:b2ff44d1d923f53540c90249f0186c6bcc7dccb99603a5bcb501d4aa81fda546
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.3 MB (37349979 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5823c93a49f14efb19ac802a6042b74cb55529fbfcce6ab550db72f9b6a7dd30`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 23 Jun 2022 00:20:27 GMT
ADD file:8adbbab04d6f84cd83b5f4205b89b0acb7ecbf27a1bb2dc181d0a629479039fe in / 
# Thu, 23 Jun 2022 00:20:27 GMT
CMD ["bash"]
# Thu, 23 Jun 2022 14:24:59 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Thu, 23 Jun 2022 14:25:02 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Thu, 23 Jun 2022 14:25:02 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 23 Jun 2022 14:25:21 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 23 Jun 2022 14:25:21 GMT
VOLUME [/spiped]
# Thu, 23 Jun 2022 14:25:22 GMT
WORKDIR /spiped
# Thu, 23 Jun 2022 14:25:22 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 23 Jun 2022 14:25:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Jun 2022 14:25:22 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:b85a868b505ffd0342a37e6a3b1c49f7c71878afe569a807e6238ef08252fcb7`  
		Last Modified: Thu, 23 Jun 2022 00:25:18 GMT  
		Size: 31.4 MB (31379408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55454b6a8916eece033c9dfe8babcaa0cd04c0901055b9040e2eac12cbb05f97`  
		Last Modified: Thu, 23 Jun 2022 14:25:40 GMT  
		Size: 1.7 KB (1733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dad7666375bb50bbfccbc5bad922741a65570699f108894f77601d31d4b76fba`  
		Last Modified: Thu, 23 Jun 2022 14:25:40 GMT  
		Size: 1.1 KB (1052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43a0a6b62b5421f4c74facfba698b0434d6899e1c77c61fefc4f28e7a0ab10d1`  
		Last Modified: Thu, 23 Jun 2022 14:25:41 GMT  
		Size: 6.0 MB (5967315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:756782629170475511f5a3ee4cb4717e152d25e3993ecc99aa0772dd2a518179`  
		Last Modified: Thu, 23 Jun 2022 14:25:40 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:331a176397a9e42d10ecaaae616afffdfffaef1527eb16f81d10ae9141ba19cf`  
		Last Modified: Thu, 23 Jun 2022 14:25:40 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; arm variant v5

```console
$ docker pull spiped@sha256:feec4c6defea9575b6b723a20ac0d667a6a0b7c896a4553cd8950674899f1d6f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.0 MB (33952417 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:609536328e039bda4f2dd352cefca6776a998bd2debfa65c39928aa2052752d3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Sat, 28 May 2022 02:03:06 GMT
ADD file:d9560b279f64bc3973a6aaa0e0ab8f483d60a1c66647899850689eee01a729ec in / 
# Sat, 28 May 2022 02:03:07 GMT
CMD ["bash"]
# Sat, 28 May 2022 19:53:26 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Sat, 28 May 2022 19:53:35 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 19:53:35 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Sat, 28 May 2022 19:54:26 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Sat, 28 May 2022 19:54:27 GMT
VOLUME [/spiped]
# Sat, 28 May 2022 19:54:27 GMT
WORKDIR /spiped
# Sat, 28 May 2022 19:54:28 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 28 May 2022 19:54:28 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 28 May 2022 19:54:29 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:b24540c95c3d5b61dba94dfa3665e0cc1231b3602edfb61432041c1f108be50d`  
		Last Modified: Sat, 28 May 2022 02:18:37 GMT  
		Size: 28.9 MB (28921471 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aea4df7367cff72ae8d9118ef5266476e59c66462928466d605c1d9623180448`  
		Last Modified: Sat, 28 May 2022 19:55:02 GMT  
		Size: 1.7 KB (1727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:246aeb209300265ffd136d8ef9420bc206bd86aec58047847f3aa4e50cf3c3eb`  
		Last Modified: Sat, 28 May 2022 19:55:02 GMT  
		Size: 1.1 KB (1054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bf79bde433a8bd87a705f9a94a90ee36cc3fcc94f66f88444fe45670af95100`  
		Last Modified: Sat, 28 May 2022 19:55:07 GMT  
		Size: 5.0 MB (5027692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9733b89df15002a08795a040cdad7e97743b49f08303f89ae9d1a578f43d4782`  
		Last Modified: Sat, 28 May 2022 19:55:02 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dce9b97ee80126486958e7e92f4caa4888c8367d20d8d39bec8c62797aee6cfd`  
		Last Modified: Sat, 28 May 2022 19:55:02 GMT  
		Size: 344.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; arm variant v7

```console
$ docker pull spiped@sha256:27ceab9292afad9550739501c64b6f5cc11c3dbe3b65f93bcc390c4120433c51
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.3 MB (31327718 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:22929e8964c6549f3d8123da06f309aa6f679e4714692df4bfa197d0e2c8f399`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Sat, 28 May 2022 00:59:48 GMT
ADD file:975c801b5b50aa75e07d18e69af11f21e165561abc16246e2c413c2ef96ce4c6 in / 
# Sat, 28 May 2022 00:59:49 GMT
CMD ["bash"]
# Sun, 29 May 2022 06:25:09 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Sun, 29 May 2022 06:25:16 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Sun, 29 May 2022 06:25:16 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Sun, 29 May 2022 06:26:02 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Sun, 29 May 2022 06:26:03 GMT
VOLUME [/spiped]
# Sun, 29 May 2022 06:26:03 GMT
WORKDIR /spiped
# Sun, 29 May 2022 06:26:04 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sun, 29 May 2022 06:26:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sun, 29 May 2022 06:26:05 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:eeb117569618df53320eb28d32b7a1d87792bda3362017123fa1025b55db44c3`  
		Last Modified: Sat, 28 May 2022 01:15:35 GMT  
		Size: 26.6 MB (26576237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f673a628d46f411f6fa471dacc6a7f093320a9060f586c46fd61466e55c0e684`  
		Last Modified: Sun, 29 May 2022 06:27:04 GMT  
		Size: 1.7 KB (1726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b972855b62da685c2bb09ca3ed5808bfc51cd9b062ad73b9ba2a0ac8497e321`  
		Last Modified: Sun, 29 May 2022 06:27:04 GMT  
		Size: 1.1 KB (1054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abf09d9445796b62d51bb11fe3f1236c17a50784d5fb850e1b26d4bcc677b3b2`  
		Last Modified: Sun, 29 May 2022 06:27:08 GMT  
		Size: 4.7 MB (4748232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:988142d33ab11d2901370155c8b902ad639de76fd48866e961b307372b37cee8`  
		Last Modified: Sun, 29 May 2022 06:27:04 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b5ba53ff286b0137dddc9613a5e23aacaa1cf035b46b78799a9dcba485d0c63`  
		Last Modified: Sun, 29 May 2022 06:27:04 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:50b5813789a1de2455e1602e814b1ba46c2f92226a13ce8acb0a33e3bb237ef8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.3 MB (35339663 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:79448de18bfa13cb33bf4a88178cbea587a26f574f5db947d339d48f822e6be8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 23 Jun 2022 00:40:43 GMT
ADD file:134be48af13f80f3474bf1b080ca781feb7b972148d482849862e55eb2acd61c in / 
# Thu, 23 Jun 2022 00:40:44 GMT
CMD ["bash"]
# Thu, 23 Jun 2022 14:19:37 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Thu, 23 Jun 2022 14:19:40 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Thu, 23 Jun 2022 14:19:41 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 23 Jun 2022 14:19:59 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 23 Jun 2022 14:19:59 GMT
VOLUME [/spiped]
# Thu, 23 Jun 2022 14:20:00 GMT
WORKDIR /spiped
# Thu, 23 Jun 2022 14:20:02 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 23 Jun 2022 14:20:02 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Jun 2022 14:20:03 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:3b157c852f2736e12f09046f214fe5f6a0b1652bd860269b3988c92a197026e8`  
		Last Modified: Thu, 23 Jun 2022 00:47:22 GMT  
		Size: 30.1 MB (30065720 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d2b50ae5c80cf61302029794b9bb8788bc1c4340583fe19b3886a328bd2e59c`  
		Last Modified: Thu, 23 Jun 2022 14:20:30 GMT  
		Size: 1.6 KB (1618 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3f8033bf687e78771c0955fb5ad0dbd87fe3ecbadc7779f0fbff1ddaed4a38b`  
		Last Modified: Thu, 23 Jun 2022 14:20:30 GMT  
		Size: 925.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90442e6da9e0bf71d16d1004502b61ac0ee04335adeb4ea1c0f5322793923308`  
		Last Modified: Thu, 23 Jun 2022 14:20:31 GMT  
		Size: 5.3 MB (5270963 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c1a82ee02be4fd41ba26092fcccc4a7ef039055a227e0d7f92ad587546071ad`  
		Last Modified: Thu, 23 Jun 2022 14:20:30 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad041befbc894c998e7065d943ec5a35b70eaf5024d5e19fa6192a489202122a`  
		Last Modified: Thu, 23 Jun 2022 14:20:30 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; 386

```console
$ docker pull spiped@sha256:0418180e629bf6c4c671ceb932c0bb7d8cc2245cd53ad80a3f9ff42a289131bf
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.3 MB (40284635 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f33d96114c1233c804814373fd9cd85fb08296fa76ac20445c2fe9d2fa0ac225`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 23 Jun 2022 00:39:33 GMT
ADD file:9d46d3f8fb63833a6dbd8dd796ad541d556046a48342d22e1fd3bffa3fb8e504 in / 
# Thu, 23 Jun 2022 00:39:33 GMT
CMD ["bash"]
# Thu, 23 Jun 2022 15:04:24 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Thu, 23 Jun 2022 15:04:28 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Thu, 23 Jun 2022 15:04:29 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 23 Jun 2022 15:04:49 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 23 Jun 2022 15:04:50 GMT
VOLUME [/spiped]
# Thu, 23 Jun 2022 15:04:51 GMT
WORKDIR /spiped
# Thu, 23 Jun 2022 15:04:53 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 23 Jun 2022 15:04:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Jun 2022 15:04:54 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:4870b12e407743816673c11cfb39974d80c1569d876287bef61f8c585954822f`  
		Last Modified: Thu, 23 Jun 2022 00:46:40 GMT  
		Size: 32.4 MB (32390198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:886cea7325b13f7203d5e830883ba71c98d83a0686704a1b6982442fd97d827c`  
		Last Modified: Thu, 23 Jun 2022 15:05:25 GMT  
		Size: 1.6 KB (1610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6a0a4b187e0c9f93860637c1c720af4b8e8cf1d089783dfbf0a07ba662fac22`  
		Last Modified: Thu, 23 Jun 2022 15:05:25 GMT  
		Size: 925.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bb9eaa94baa3de99a61cef041ce22494d7ffdbbbdabc1ea1629f4bb0d977bdd`  
		Last Modified: Thu, 23 Jun 2022 15:05:27 GMT  
		Size: 7.9 MB (7891464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3560d550fd7c038f01cf33f88495c9761131e2304f6d1f17a85e272656dd82ff`  
		Last Modified: Thu, 23 Jun 2022 15:05:25 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:776c52a49bfdec3ad5665559540af9ec46f9eced7d9aa5d664aaa96582d28fb4`  
		Last Modified: Thu, 23 Jun 2022 15:05:25 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; mips64le

```console
$ docker pull spiped@sha256:327ab349035e42e2520c87903f12e1e4b8aa2b46f5af20028c6148d435015ac6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.3 MB (35349399 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:134640be221db73739d4c6d145ed454eb1f6b7c530d7b5a037f8566a5c50d315`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Sat, 28 May 2022 01:11:13 GMT
ADD file:f685a156b7ddafe7bafc6fad17cc36cc8a5d6d922fc1c425656ca92266d9a98e in / 
# Sat, 28 May 2022 01:11:18 GMT
CMD ["bash"]
# Sat, 28 May 2022 11:02:07 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Sat, 28 May 2022 11:02:24 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 11:02:26 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Sat, 28 May 2022 11:03:57 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Sat, 28 May 2022 11:04:00 GMT
VOLUME [/spiped]
# Sat, 28 May 2022 11:04:03 GMT
WORKDIR /spiped
# Sat, 28 May 2022 11:04:06 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 28 May 2022 11:04:08 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 28 May 2022 11:04:11 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:fdea7139ce36b557a23c4b9c4255387b175f851ed0c51e1e7d78dd301c0e4da8`  
		Last Modified: Sat, 28 May 2022 01:21:35 GMT  
		Size: 29.6 MB (29641237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:638fcc9a2aca909e0ddad028b40a02f45370c5c4864972531afa7a02e7d5f8b5`  
		Last Modified: Sat, 28 May 2022 11:04:37 GMT  
		Size: 1.6 KB (1620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62732d2f48eb3a503a80f0fcc97263b3feb49c39cfec9026b62d02698d569084`  
		Last Modified: Sat, 28 May 2022 11:04:37 GMT  
		Size: 925.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec6d02d49d5fc774a71ed9e0211b9250e5926d8a45f48011929bc45eea21a764`  
		Last Modified: Sat, 28 May 2022 11:04:43 GMT  
		Size: 5.7 MB (5705180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:551ee4c909a9bed061c23e73af4c6586e9b6144160f20081c7c31a2e78d21357`  
		Last Modified: Sat, 28 May 2022 11:04:37 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8231a7adeed86962f2691999debe4256643805fd3dd1b4deb1e8e6d30fbd2e2`  
		Last Modified: Sat, 28 May 2022 11:04:37 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; ppc64le

```console
$ docker pull spiped@sha256:b6377c503b8d6a42b6db7ff3590aca7406bbb9fb1550d8baaf89f61ee4e6f222
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.3 MB (41289157 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ed59345839d9409f475ce2fce73fb95e4ba9c41a970711589fb2014d87459aa9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Sat, 28 May 2022 01:22:54 GMT
ADD file:64e264b12eed99d87380e38f36bfecd62b9bb1e5460f0242cfbc5dc76c212ead in / 
# Sat, 28 May 2022 01:22:59 GMT
CMD ["bash"]
# Sat, 28 May 2022 20:47:31 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Sat, 28 May 2022 20:47:49 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 20:48:09 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Sat, 28 May 2022 20:50:59 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Sat, 28 May 2022 20:51:04 GMT
VOLUME [/spiped]
# Sat, 28 May 2022 20:51:09 GMT
WORKDIR /spiped
# Sat, 28 May 2022 20:51:31 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 28 May 2022 20:51:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 28 May 2022 20:52:04 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:893e245a8f6219935016f2dd4422ec4b7fdab43d98ba29c024ec0d9ce57794ba`  
		Last Modified: Sat, 28 May 2022 01:32:28 GMT  
		Size: 35.3 MB (35286698 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:922a5f50c37cc3b0d1fef17e00862a91bd28f367cd75a7ad0414852ec8d6809e`  
		Last Modified: Sat, 28 May 2022 20:52:46 GMT  
		Size: 1.7 KB (1737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59b8faf9aaa0e83c1e60be75a9512012bfbe307b7facc7fc65656db5f3f4c3ff`  
		Last Modified: Sat, 28 May 2022 20:52:46 GMT  
		Size: 1.1 KB (1056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7583ca3e72d7ba19d9282d7cceb754c6b78dcc5dafe87fb40ba11abcdfad841b`  
		Last Modified: Sat, 28 May 2022 20:52:47 GMT  
		Size: 6.0 MB (5999195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3c570e58336fa60b88539aef4e1ffa0289798f70a906a55c0b291cf386d76c2`  
		Last Modified: Sat, 28 May 2022 20:52:46 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9a0eb6589f42f53d4c16113fbeee7f38fff9157291e8c9b22be42ce45653820`  
		Last Modified: Sat, 28 May 2022 20:52:46 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; s390x

```console
$ docker pull spiped@sha256:a9442b276bfaee2a75715fe608363309aca4373dc2dc502604bb2bb0d5f4dea8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.8 MB (34845447 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2941968d748f4b2e9298f5f6ecd1c8ef8a6e9fc6074a6649a7b6ea6f03eff523`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 23 Jun 2022 00:43:10 GMT
ADD file:0b511e3efd87267fb27161eae56c4d08f0fed733697da6ffe6ea96a4cb68e938 in / 
# Thu, 23 Jun 2022 00:43:15 GMT
CMD ["bash"]
# Thu, 23 Jun 2022 13:40:29 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Thu, 23 Jun 2022 13:40:31 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Thu, 23 Jun 2022 13:40:32 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 23 Jun 2022 13:40:43 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 23 Jun 2022 13:40:44 GMT
VOLUME [/spiped]
# Thu, 23 Jun 2022 13:40:44 GMT
WORKDIR /spiped
# Thu, 23 Jun 2022 13:40:44 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 23 Jun 2022 13:40:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Jun 2022 13:40:44 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:c547f465e0c8708ad0c57cf09caa52f4c2b5b295bf10ab1ce71ca17ff81ea36a`  
		Last Modified: Thu, 23 Jun 2022 00:51:59 GMT  
		Size: 29.7 MB (29655262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f10418190b72e9fc95fa6f7bd6436f85792a11bac97bf409ebb489733c6cdeb`  
		Last Modified: Thu, 23 Jun 2022 13:41:20 GMT  
		Size: 1.7 KB (1736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d9de83495ba48b01499e858c82e09a1dbed7baa1add5136e5adce6e7d60d452`  
		Last Modified: Thu, 23 Jun 2022 13:41:19 GMT  
		Size: 1.1 KB (1052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1af8046b93a37ad2bb5d08d4a2b031d01e804f6215b67365ba7b72766510a52c`  
		Last Modified: Thu, 23 Jun 2022 13:41:20 GMT  
		Size: 5.2 MB (5186928 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d254cd7b5719c3b1ba5880a1daa9212d49f5999c4c6f371e32d84733730ddcfe`  
		Last Modified: Thu, 23 Jun 2022 13:41:19 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2556f06bac5f4c72f60c12325c5c156dd6d3cc548dbc2d60398e43f72584c19`  
		Last Modified: Thu, 23 Jun 2022 13:41:19 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:1-alpine`

```console
$ docker pull spiped@sha256:574b58f2dcd9c3904a6435230c713766d0690f6282db43000ca61e233d59d401
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
$ docker pull spiped@sha256:bdd3a85420e8c8d55b154c7d7f1a043ca1bbae32a53dceaca4838f70ff3376b9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (3022980 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6c7e9665581a5ef894060d275062ab85a542c8fa4a4aae78d4f2617be109e728`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Mon, 23 May 2022 19:19:30 GMT
ADD file:8e81116368669ed3dd361bc898d61bff249f524139a239fdaf3ec46869a39921 in / 
# Mon, 23 May 2022 19:19:31 GMT
CMD ["/bin/sh"]
# Tue, 24 May 2022 19:34:44 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Tue, 24 May 2022 19:34:45 GMT
RUN apk add --no-cache libssl1.1
# Tue, 24 May 2022 19:34:45 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 24 May 2022 19:34:55 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Tue, 24 May 2022 19:34:55 GMT
VOLUME [/spiped]
# Tue, 24 May 2022 19:34:55 GMT
WORKDIR /spiped
# Tue, 24 May 2022 19:34:56 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 24 May 2022 19:34:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 24 May 2022 19:34:56 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:2408cc74d12b6cd092bb8b516ba7d5e290f485d3eb9672efc00f0583730179e8`  
		Last Modified: Mon, 23 May 2022 19:09:38 GMT  
		Size: 2.8 MB (2798889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:becf26afb9051910736e73bcdbfc94bfb72d60a534521c9d4d8bd49f058953ca`  
		Last Modified: Tue, 24 May 2022 19:35:11 GMT  
		Size: 1.3 KB (1271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:744686996785b12019a749f4c09b2b5d59b293aca28e90b0a63b3b6683296350`  
		Last Modified: Tue, 24 May 2022 19:35:11 GMT  
		Size: 7.7 KB (7731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fdf476035643e2d6746fa2acf3e72b7d990dfbf92675e53c57fc5eff30f88ca`  
		Last Modified: Tue, 24 May 2022 19:35:11 GMT  
		Size: 214.6 KB (214618 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a5688549417be3b134e241c450a08175acf2c8cd842b2e30f3310f6a58314a6`  
		Last Modified: Tue, 24 May 2022 19:35:11 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0acff87013e49fae028cf81385e161bc4f11ec1173a9799808132863c6bfa34`  
		Last Modified: Tue, 24 May 2022 19:35:11 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; arm variant v6

```console
$ docker pull spiped@sha256:406809ea0a81e5db518b787d7612be34a70855479615ff4cace100dc08c1ce5d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 MB (2814958 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:765f7c1b3fd5477fdd79037421a66d16f15550314f4344b2e7f359d1ab9f5a6b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Mon, 23 May 2022 19:49:32 GMT
ADD file:f7cee617575b5e5a7672d298a519bb8d8b5098efb90aa2a5d7b0510003457d52 in / 
# Mon, 23 May 2022 19:49:33 GMT
CMD ["/bin/sh"]
# Tue, 24 May 2022 20:14:54 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Tue, 24 May 2022 20:14:56 GMT
RUN apk add --no-cache libssl1.1
# Tue, 24 May 2022 20:14:57 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 24 May 2022 20:15:17 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Tue, 24 May 2022 20:15:18 GMT
VOLUME [/spiped]
# Tue, 24 May 2022 20:15:18 GMT
WORKDIR /spiped
# Tue, 24 May 2022 20:15:19 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 24 May 2022 20:15:19 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 24 May 2022 20:15:20 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:79a25ccaf940855872635c06e7614d9b27dd38ffb5a8adfdb9274dfdc0ea0d87`  
		Last Modified: Mon, 23 May 2022 19:08:47 GMT  
		Size: 2.6 MB (2606142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0a7e07c35741a1549360e780bc005cf673a71e419a28d8a6b9c13991457fd00`  
		Last Modified: Tue, 24 May 2022 20:15:52 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cdf6aebe85933f39c72c58c99c4ec7d111a159f1235bfe85319b66d6203ef8a`  
		Last Modified: Tue, 24 May 2022 20:15:52 GMT  
		Size: 7.7 KB (7726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c66c128b4f04df47fadf6a72f2ba745ba461f8a90f759782eca976719289bfa`  
		Last Modified: Tue, 24 May 2022 20:15:52 GMT  
		Size: 199.3 KB (199349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cff01690378c3c28fddd84bf4b93277c045d39f051cf3b935d00174aa4f2eb45`  
		Last Modified: Tue, 24 May 2022 20:15:52 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fab83e2c93a7364c569439bdd1bcb23f85d4b7900ff40e1cb25bece561c431a`  
		Last Modified: Tue, 24 May 2022 20:15:52 GMT  
		Size: 344.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; arm variant v7

```console
$ docker pull spiped@sha256:acc8ca060038077aa20644d95dfd50f3a9faa59990d2318895033343f94456eb
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 MB (2614203 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:afa4570c887e85e41ae28860d1797be642647270341c2b31a2d07268170d3d18`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Mon, 23 May 2022 18:57:46 GMT
ADD file:72698cc08524b911ebaacf992490707e5a951ddd2fe6edb3fb598e9dc7155049 in / 
# Mon, 23 May 2022 18:57:47 GMT
CMD ["/bin/sh"]
# Tue, 24 May 2022 23:57:01 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Tue, 24 May 2022 23:57:03 GMT
RUN apk add --no-cache libssl1.1
# Tue, 24 May 2022 23:57:03 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 24 May 2022 23:57:23 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Tue, 24 May 2022 23:57:24 GMT
VOLUME [/spiped]
# Tue, 24 May 2022 23:57:24 GMT
WORKDIR /spiped
# Tue, 24 May 2022 23:57:25 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 24 May 2022 23:57:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 24 May 2022 23:57:26 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:6366ba92f08e2418e90171f1e34bd86ecd50fdc95953b3f33b8943c143518eca`  
		Last Modified: Mon, 23 May 2022 18:59:17 GMT  
		Size: 2.4 MB (2411648 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:744a106e187f9790be6dbdde860ada60aab7e95bae779540c813da16ce184ea7`  
		Last Modified: Tue, 24 May 2022 23:58:19 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e8f51295340b65e165fffa3de719118e625ca751a7c465a96dee14a0441de72`  
		Last Modified: Tue, 24 May 2022 23:58:19 GMT  
		Size: 7.7 KB (7717 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a1da9fdb3c39499af6413db4aeed00e8577a949c49968ffd86c20f438118a88`  
		Last Modified: Tue, 24 May 2022 23:58:19 GMT  
		Size: 193.1 KB (193098 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83b416966b1e14463ce73c56ecba5fd804f4c565b4d781199f3b02247ffdf8e7`  
		Last Modified: Tue, 24 May 2022 23:58:19 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f1016107cea29ba85ecc25a6bba5c5c3494ef9ed31194cc5e7b6ea8add7ef4a`  
		Last Modified: Tue, 24 May 2022 23:58:19 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:bdfcd3d661a8017ef3286486269e41c2ab4d2c4662672ea7e21ac01a7e8572c8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 MB (2911518 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:12a66ddef290c67283604068f9b4d679bc4dd400e2bdf0d2826b55e9bdf23aeb`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Mon, 23 May 2022 19:39:22 GMT
ADD file:3ae36c6c4a1fc43157692da97c6c4fa6c3d0189ba82e2bef7f5aaf4a5e083f18 in / 
# Mon, 23 May 2022 19:39:22 GMT
CMD ["/bin/sh"]
# Tue, 24 May 2022 20:25:00 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Tue, 24 May 2022 20:25:02 GMT
RUN apk add --no-cache libssl1.1
# Tue, 24 May 2022 20:25:03 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 24 May 2022 20:25:22 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Tue, 24 May 2022 20:25:23 GMT
VOLUME [/spiped]
# Tue, 24 May 2022 20:25:24 GMT
WORKDIR /spiped
# Tue, 24 May 2022 20:25:26 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 24 May 2022 20:25:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 24 May 2022 20:25:27 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:b3c136eddcbf2003d3180787cef00f39d46b9fd9e4623178282ad6a8d63ad3b0`  
		Last Modified: Mon, 23 May 2022 19:08:34 GMT  
		Size: 2.7 MB (2694464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20a86dbffa956db3e6a8cd773330f1ec06aa87e6987f0f5c9a031e2af7975a9a`  
		Last Modified: Tue, 24 May 2022 20:25:57 GMT  
		Size: 1.2 KB (1244 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:168f9b4c4b922cf44b915dedb800de4176f18b715d6a917a6576a2d24ba0b78a`  
		Last Modified: Tue, 24 May 2022 20:25:57 GMT  
		Size: 7.7 KB (7705 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba2ce83ec0aa17bde883cf7689464f8502798d298fd4296e17e51c9ab614ebd6`  
		Last Modified: Tue, 24 May 2022 20:25:57 GMT  
		Size: 207.7 KB (207671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7796ce5b43cb7f8557eb86d1bb3682848bca4769f1886634356d8952e37e262`  
		Last Modified: Tue, 24 May 2022 20:25:57 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c60cf321cf0b839869c31f5a9ac3374f3c43dba87ab4d0794c93d1436b27e37d`  
		Last Modified: Tue, 24 May 2022 20:25:56 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; 386

```console
$ docker pull spiped@sha256:6eb9e3e76d959724427cca66e52c7bdeebb58c9297c5fd7d60b50838669fe7ef
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (3036399 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b0215089b25dc2844d60ff524e3c7359fc6094c7376d2646e5482fa918c91bad`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Mon, 23 May 2022 19:38:20 GMT
ADD file:1750ccfabfe93636015070d51a6e824cbd738056223421c69d8aaabc38041b18 in / 
# Mon, 23 May 2022 19:38:20 GMT
CMD ["/bin/sh"]
# Tue, 24 May 2022 20:13:25 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Tue, 24 May 2022 20:13:26 GMT
RUN apk add --no-cache libssl1.1
# Tue, 24 May 2022 20:13:27 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 24 May 2022 20:13:38 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Tue, 24 May 2022 20:13:39 GMT
VOLUME [/spiped]
# Tue, 24 May 2022 20:13:40 GMT
WORKDIR /spiped
# Tue, 24 May 2022 20:13:42 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 24 May 2022 20:13:42 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 24 May 2022 20:13:43 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:bb638a3869eed698f88775c7a48f36f8e22e7c6bbaa98fa1d5678966b619b859`  
		Last Modified: Mon, 23 May 2022 19:09:25 GMT  
		Size: 2.8 MB (2801887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:538c30644db57c76ff9a69c435c96a6d269cf8da91c4d632beffff39511588ca`  
		Last Modified: Tue, 24 May 2022 20:14:13 GMT  
		Size: 1.2 KB (1241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d193ad41299c95702ee3dcff9a3399e567cc04c5e640af6cc098795b475843fe`  
		Last Modified: Tue, 24 May 2022 20:14:12 GMT  
		Size: 7.7 KB (7697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec3ef77db5428642bb00b1436a0a844fca99ef4cc676e787f6307ac237f4f65d`  
		Last Modified: Tue, 24 May 2022 20:14:13 GMT  
		Size: 225.1 KB (225139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce435cec46d2206fbfa56e9dc4c9a2907fcd4bdba6acb8c4f332a2f1246e1a8c`  
		Last Modified: Tue, 24 May 2022 20:14:13 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ab3029834f1c60801bbb7cb77e5fec645e494281b466eaed4fb5c5ed38f4b26`  
		Last Modified: Tue, 24 May 2022 20:14:12 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; ppc64le

```console
$ docker pull spiped@sha256:394770c1c3e52c18b2e060896dc946a7de8c0581c1691fe3a2458c6442d51071
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (3012900 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:45dd65bd18433f8227345eb1bc628c92fb777cc4d5e9e790835ba272eaadec4e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Mon, 23 May 2022 19:16:51 GMT
ADD file:6a5450c8a7cee3ceda59e7cb350c54df4139b0f7b7cf49c8b31bb9c01646c3cd in / 
# Mon, 23 May 2022 19:16:53 GMT
CMD ["/bin/sh"]
# Tue, 24 May 2022 19:50:10 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Tue, 24 May 2022 19:50:18 GMT
RUN apk add --no-cache libssl1.1
# Tue, 24 May 2022 19:50:20 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 24 May 2022 19:50:38 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Tue, 24 May 2022 19:50:42 GMT
VOLUME [/spiped]
# Tue, 24 May 2022 19:50:47 GMT
WORKDIR /spiped
# Tue, 24 May 2022 19:50:48 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 24 May 2022 19:50:52 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 24 May 2022 19:50:56 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:d3deabf2a506ef6f5fa7c2a68bf27047574cef9908b30a97ff2d01ae539b089a`  
		Last Modified: Mon, 23 May 2022 19:09:13 GMT  
		Size: 2.8 MB (2789745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6d245add1998dabc480629fde1ae678cfbb96f740737e4acede363c37eda348`  
		Last Modified: Tue, 24 May 2022 19:51:36 GMT  
		Size: 1.3 KB (1272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bea94be815996b73043903da4f60b4ea3573e9689c5b3b1b0348ef5ef54fe25b`  
		Last Modified: Tue, 24 May 2022 19:51:36 GMT  
		Size: 7.7 KB (7727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b25cc9d25fe567c300c07c50cb1d341544a9751b92d44874cef5399d1beee0aa`  
		Last Modified: Tue, 24 May 2022 19:51:36 GMT  
		Size: 213.7 KB (213687 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2b003e2ac252266dcd49f568ddc62ed5a04668bc0655e7cd74521a21c0089eb`  
		Last Modified: Tue, 24 May 2022 19:51:36 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fed434cd18f8048c2624c1d26c27721d4ce3e46b39d5d9adcbeec4733e3954ff`  
		Last Modified: Tue, 24 May 2022 19:51:36 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; s390x

```console
$ docker pull spiped@sha256:4c56dd9796353102785f0a5f8f38e81e0638a1ca2b745795770b8e137ebc657d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 MB (2791966 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a3497d9a69b26f419f935637e370f6a57f1d4e5ad7000970a7ecdcbf0333263c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Mon, 23 May 2022 19:41:59 GMT
ADD file:e1852d8ef555a0d3ef6d0b74a898720c82bb9f491430b06a0dd0499497ce118e in / 
# Mon, 23 May 2022 19:42:10 GMT
CMD ["/bin/sh"]
# Tue, 24 May 2022 20:27:25 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Tue, 24 May 2022 20:27:27 GMT
RUN apk add --no-cache libssl1.1
# Tue, 24 May 2022 20:27:27 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 24 May 2022 20:27:35 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Tue, 24 May 2022 20:27:36 GMT
VOLUME [/spiped]
# Tue, 24 May 2022 20:27:36 GMT
WORKDIR /spiped
# Tue, 24 May 2022 20:27:37 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 24 May 2022 20:27:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 24 May 2022 20:27:38 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:af1ac1a73384e058591d04d19bc05a06781cc32d52d4593b468d6cb95eda9858`  
		Last Modified: Mon, 23 May 2022 19:43:36 GMT  
		Size: 2.6 MB (2580494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9623718447e29295a23001aae3dbed26ca7b41b14965f02c9ae5324963330ef0`  
		Last Modified: Tue, 24 May 2022 20:28:11 GMT  
		Size: 1.3 KB (1267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74a000d8db4a14acf7833a4d32f3d85f452d72236f3a96360d4518ee2abba268`  
		Last Modified: Tue, 24 May 2022 20:28:11 GMT  
		Size: 7.7 KB (7722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4024830388cfd5531b6e2ca6468204a9d4fb81958bad00a9f8694fcea02a1d0`  
		Last Modified: Tue, 24 May 2022 20:28:11 GMT  
		Size: 202.0 KB (202015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f77170c060013a5bc5e10927cde6e8c315bd601aab054eb5717725f98bb2b0c`  
		Last Modified: Tue, 24 May 2022 20:28:11 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6dcb80a5752c8255af9b16d7c0d66266c0e5ecfec63891ebdb6c7a2d47ff7c71`  
		Last Modified: Tue, 24 May 2022 20:28:11 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:1.6`

```console
$ docker pull spiped@sha256:2a04458cf6cb5fa31173ddeeaec6840207e46a3186dbb1e1de6b3c83a009c5d0
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
$ docker pull spiped@sha256:b2ff44d1d923f53540c90249f0186c6bcc7dccb99603a5bcb501d4aa81fda546
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.3 MB (37349979 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5823c93a49f14efb19ac802a6042b74cb55529fbfcce6ab550db72f9b6a7dd30`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 23 Jun 2022 00:20:27 GMT
ADD file:8adbbab04d6f84cd83b5f4205b89b0acb7ecbf27a1bb2dc181d0a629479039fe in / 
# Thu, 23 Jun 2022 00:20:27 GMT
CMD ["bash"]
# Thu, 23 Jun 2022 14:24:59 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Thu, 23 Jun 2022 14:25:02 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Thu, 23 Jun 2022 14:25:02 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 23 Jun 2022 14:25:21 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 23 Jun 2022 14:25:21 GMT
VOLUME [/spiped]
# Thu, 23 Jun 2022 14:25:22 GMT
WORKDIR /spiped
# Thu, 23 Jun 2022 14:25:22 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 23 Jun 2022 14:25:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Jun 2022 14:25:22 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:b85a868b505ffd0342a37e6a3b1c49f7c71878afe569a807e6238ef08252fcb7`  
		Last Modified: Thu, 23 Jun 2022 00:25:18 GMT  
		Size: 31.4 MB (31379408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55454b6a8916eece033c9dfe8babcaa0cd04c0901055b9040e2eac12cbb05f97`  
		Last Modified: Thu, 23 Jun 2022 14:25:40 GMT  
		Size: 1.7 KB (1733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dad7666375bb50bbfccbc5bad922741a65570699f108894f77601d31d4b76fba`  
		Last Modified: Thu, 23 Jun 2022 14:25:40 GMT  
		Size: 1.1 KB (1052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43a0a6b62b5421f4c74facfba698b0434d6899e1c77c61fefc4f28e7a0ab10d1`  
		Last Modified: Thu, 23 Jun 2022 14:25:41 GMT  
		Size: 6.0 MB (5967315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:756782629170475511f5a3ee4cb4717e152d25e3993ecc99aa0772dd2a518179`  
		Last Modified: Thu, 23 Jun 2022 14:25:40 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:331a176397a9e42d10ecaaae616afffdfffaef1527eb16f81d10ae9141ba19cf`  
		Last Modified: Thu, 23 Jun 2022 14:25:40 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; arm variant v5

```console
$ docker pull spiped@sha256:feec4c6defea9575b6b723a20ac0d667a6a0b7c896a4553cd8950674899f1d6f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.0 MB (33952417 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:609536328e039bda4f2dd352cefca6776a998bd2debfa65c39928aa2052752d3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Sat, 28 May 2022 02:03:06 GMT
ADD file:d9560b279f64bc3973a6aaa0e0ab8f483d60a1c66647899850689eee01a729ec in / 
# Sat, 28 May 2022 02:03:07 GMT
CMD ["bash"]
# Sat, 28 May 2022 19:53:26 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Sat, 28 May 2022 19:53:35 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 19:53:35 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Sat, 28 May 2022 19:54:26 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Sat, 28 May 2022 19:54:27 GMT
VOLUME [/spiped]
# Sat, 28 May 2022 19:54:27 GMT
WORKDIR /spiped
# Sat, 28 May 2022 19:54:28 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 28 May 2022 19:54:28 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 28 May 2022 19:54:29 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:b24540c95c3d5b61dba94dfa3665e0cc1231b3602edfb61432041c1f108be50d`  
		Last Modified: Sat, 28 May 2022 02:18:37 GMT  
		Size: 28.9 MB (28921471 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aea4df7367cff72ae8d9118ef5266476e59c66462928466d605c1d9623180448`  
		Last Modified: Sat, 28 May 2022 19:55:02 GMT  
		Size: 1.7 KB (1727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:246aeb209300265ffd136d8ef9420bc206bd86aec58047847f3aa4e50cf3c3eb`  
		Last Modified: Sat, 28 May 2022 19:55:02 GMT  
		Size: 1.1 KB (1054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bf79bde433a8bd87a705f9a94a90ee36cc3fcc94f66f88444fe45670af95100`  
		Last Modified: Sat, 28 May 2022 19:55:07 GMT  
		Size: 5.0 MB (5027692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9733b89df15002a08795a040cdad7e97743b49f08303f89ae9d1a578f43d4782`  
		Last Modified: Sat, 28 May 2022 19:55:02 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dce9b97ee80126486958e7e92f4caa4888c8367d20d8d39bec8c62797aee6cfd`  
		Last Modified: Sat, 28 May 2022 19:55:02 GMT  
		Size: 344.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; arm variant v7

```console
$ docker pull spiped@sha256:27ceab9292afad9550739501c64b6f5cc11c3dbe3b65f93bcc390c4120433c51
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.3 MB (31327718 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:22929e8964c6549f3d8123da06f309aa6f679e4714692df4bfa197d0e2c8f399`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Sat, 28 May 2022 00:59:48 GMT
ADD file:975c801b5b50aa75e07d18e69af11f21e165561abc16246e2c413c2ef96ce4c6 in / 
# Sat, 28 May 2022 00:59:49 GMT
CMD ["bash"]
# Sun, 29 May 2022 06:25:09 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Sun, 29 May 2022 06:25:16 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Sun, 29 May 2022 06:25:16 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Sun, 29 May 2022 06:26:02 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Sun, 29 May 2022 06:26:03 GMT
VOLUME [/spiped]
# Sun, 29 May 2022 06:26:03 GMT
WORKDIR /spiped
# Sun, 29 May 2022 06:26:04 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sun, 29 May 2022 06:26:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sun, 29 May 2022 06:26:05 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:eeb117569618df53320eb28d32b7a1d87792bda3362017123fa1025b55db44c3`  
		Last Modified: Sat, 28 May 2022 01:15:35 GMT  
		Size: 26.6 MB (26576237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f673a628d46f411f6fa471dacc6a7f093320a9060f586c46fd61466e55c0e684`  
		Last Modified: Sun, 29 May 2022 06:27:04 GMT  
		Size: 1.7 KB (1726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b972855b62da685c2bb09ca3ed5808bfc51cd9b062ad73b9ba2a0ac8497e321`  
		Last Modified: Sun, 29 May 2022 06:27:04 GMT  
		Size: 1.1 KB (1054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abf09d9445796b62d51bb11fe3f1236c17a50784d5fb850e1b26d4bcc677b3b2`  
		Last Modified: Sun, 29 May 2022 06:27:08 GMT  
		Size: 4.7 MB (4748232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:988142d33ab11d2901370155c8b902ad639de76fd48866e961b307372b37cee8`  
		Last Modified: Sun, 29 May 2022 06:27:04 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b5ba53ff286b0137dddc9613a5e23aacaa1cf035b46b78799a9dcba485d0c63`  
		Last Modified: Sun, 29 May 2022 06:27:04 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:50b5813789a1de2455e1602e814b1ba46c2f92226a13ce8acb0a33e3bb237ef8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.3 MB (35339663 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:79448de18bfa13cb33bf4a88178cbea587a26f574f5db947d339d48f822e6be8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 23 Jun 2022 00:40:43 GMT
ADD file:134be48af13f80f3474bf1b080ca781feb7b972148d482849862e55eb2acd61c in / 
# Thu, 23 Jun 2022 00:40:44 GMT
CMD ["bash"]
# Thu, 23 Jun 2022 14:19:37 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Thu, 23 Jun 2022 14:19:40 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Thu, 23 Jun 2022 14:19:41 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 23 Jun 2022 14:19:59 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 23 Jun 2022 14:19:59 GMT
VOLUME [/spiped]
# Thu, 23 Jun 2022 14:20:00 GMT
WORKDIR /spiped
# Thu, 23 Jun 2022 14:20:02 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 23 Jun 2022 14:20:02 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Jun 2022 14:20:03 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:3b157c852f2736e12f09046f214fe5f6a0b1652bd860269b3988c92a197026e8`  
		Last Modified: Thu, 23 Jun 2022 00:47:22 GMT  
		Size: 30.1 MB (30065720 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d2b50ae5c80cf61302029794b9bb8788bc1c4340583fe19b3886a328bd2e59c`  
		Last Modified: Thu, 23 Jun 2022 14:20:30 GMT  
		Size: 1.6 KB (1618 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3f8033bf687e78771c0955fb5ad0dbd87fe3ecbadc7779f0fbff1ddaed4a38b`  
		Last Modified: Thu, 23 Jun 2022 14:20:30 GMT  
		Size: 925.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90442e6da9e0bf71d16d1004502b61ac0ee04335adeb4ea1c0f5322793923308`  
		Last Modified: Thu, 23 Jun 2022 14:20:31 GMT  
		Size: 5.3 MB (5270963 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c1a82ee02be4fd41ba26092fcccc4a7ef039055a227e0d7f92ad587546071ad`  
		Last Modified: Thu, 23 Jun 2022 14:20:30 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad041befbc894c998e7065d943ec5a35b70eaf5024d5e19fa6192a489202122a`  
		Last Modified: Thu, 23 Jun 2022 14:20:30 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; 386

```console
$ docker pull spiped@sha256:0418180e629bf6c4c671ceb932c0bb7d8cc2245cd53ad80a3f9ff42a289131bf
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.3 MB (40284635 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f33d96114c1233c804814373fd9cd85fb08296fa76ac20445c2fe9d2fa0ac225`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 23 Jun 2022 00:39:33 GMT
ADD file:9d46d3f8fb63833a6dbd8dd796ad541d556046a48342d22e1fd3bffa3fb8e504 in / 
# Thu, 23 Jun 2022 00:39:33 GMT
CMD ["bash"]
# Thu, 23 Jun 2022 15:04:24 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Thu, 23 Jun 2022 15:04:28 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Thu, 23 Jun 2022 15:04:29 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 23 Jun 2022 15:04:49 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 23 Jun 2022 15:04:50 GMT
VOLUME [/spiped]
# Thu, 23 Jun 2022 15:04:51 GMT
WORKDIR /spiped
# Thu, 23 Jun 2022 15:04:53 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 23 Jun 2022 15:04:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Jun 2022 15:04:54 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:4870b12e407743816673c11cfb39974d80c1569d876287bef61f8c585954822f`  
		Last Modified: Thu, 23 Jun 2022 00:46:40 GMT  
		Size: 32.4 MB (32390198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:886cea7325b13f7203d5e830883ba71c98d83a0686704a1b6982442fd97d827c`  
		Last Modified: Thu, 23 Jun 2022 15:05:25 GMT  
		Size: 1.6 KB (1610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6a0a4b187e0c9f93860637c1c720af4b8e8cf1d089783dfbf0a07ba662fac22`  
		Last Modified: Thu, 23 Jun 2022 15:05:25 GMT  
		Size: 925.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bb9eaa94baa3de99a61cef041ce22494d7ffdbbbdabc1ea1629f4bb0d977bdd`  
		Last Modified: Thu, 23 Jun 2022 15:05:27 GMT  
		Size: 7.9 MB (7891464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3560d550fd7c038f01cf33f88495c9761131e2304f6d1f17a85e272656dd82ff`  
		Last Modified: Thu, 23 Jun 2022 15:05:25 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:776c52a49bfdec3ad5665559540af9ec46f9eced7d9aa5d664aaa96582d28fb4`  
		Last Modified: Thu, 23 Jun 2022 15:05:25 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; mips64le

```console
$ docker pull spiped@sha256:327ab349035e42e2520c87903f12e1e4b8aa2b46f5af20028c6148d435015ac6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.3 MB (35349399 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:134640be221db73739d4c6d145ed454eb1f6b7c530d7b5a037f8566a5c50d315`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Sat, 28 May 2022 01:11:13 GMT
ADD file:f685a156b7ddafe7bafc6fad17cc36cc8a5d6d922fc1c425656ca92266d9a98e in / 
# Sat, 28 May 2022 01:11:18 GMT
CMD ["bash"]
# Sat, 28 May 2022 11:02:07 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Sat, 28 May 2022 11:02:24 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 11:02:26 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Sat, 28 May 2022 11:03:57 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Sat, 28 May 2022 11:04:00 GMT
VOLUME [/spiped]
# Sat, 28 May 2022 11:04:03 GMT
WORKDIR /spiped
# Sat, 28 May 2022 11:04:06 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 28 May 2022 11:04:08 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 28 May 2022 11:04:11 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:fdea7139ce36b557a23c4b9c4255387b175f851ed0c51e1e7d78dd301c0e4da8`  
		Last Modified: Sat, 28 May 2022 01:21:35 GMT  
		Size: 29.6 MB (29641237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:638fcc9a2aca909e0ddad028b40a02f45370c5c4864972531afa7a02e7d5f8b5`  
		Last Modified: Sat, 28 May 2022 11:04:37 GMT  
		Size: 1.6 KB (1620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62732d2f48eb3a503a80f0fcc97263b3feb49c39cfec9026b62d02698d569084`  
		Last Modified: Sat, 28 May 2022 11:04:37 GMT  
		Size: 925.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec6d02d49d5fc774a71ed9e0211b9250e5926d8a45f48011929bc45eea21a764`  
		Last Modified: Sat, 28 May 2022 11:04:43 GMT  
		Size: 5.7 MB (5705180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:551ee4c909a9bed061c23e73af4c6586e9b6144160f20081c7c31a2e78d21357`  
		Last Modified: Sat, 28 May 2022 11:04:37 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8231a7adeed86962f2691999debe4256643805fd3dd1b4deb1e8e6d30fbd2e2`  
		Last Modified: Sat, 28 May 2022 11:04:37 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; ppc64le

```console
$ docker pull spiped@sha256:b6377c503b8d6a42b6db7ff3590aca7406bbb9fb1550d8baaf89f61ee4e6f222
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.3 MB (41289157 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ed59345839d9409f475ce2fce73fb95e4ba9c41a970711589fb2014d87459aa9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Sat, 28 May 2022 01:22:54 GMT
ADD file:64e264b12eed99d87380e38f36bfecd62b9bb1e5460f0242cfbc5dc76c212ead in / 
# Sat, 28 May 2022 01:22:59 GMT
CMD ["bash"]
# Sat, 28 May 2022 20:47:31 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Sat, 28 May 2022 20:47:49 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 20:48:09 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Sat, 28 May 2022 20:50:59 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Sat, 28 May 2022 20:51:04 GMT
VOLUME [/spiped]
# Sat, 28 May 2022 20:51:09 GMT
WORKDIR /spiped
# Sat, 28 May 2022 20:51:31 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 28 May 2022 20:51:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 28 May 2022 20:52:04 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:893e245a8f6219935016f2dd4422ec4b7fdab43d98ba29c024ec0d9ce57794ba`  
		Last Modified: Sat, 28 May 2022 01:32:28 GMT  
		Size: 35.3 MB (35286698 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:922a5f50c37cc3b0d1fef17e00862a91bd28f367cd75a7ad0414852ec8d6809e`  
		Last Modified: Sat, 28 May 2022 20:52:46 GMT  
		Size: 1.7 KB (1737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59b8faf9aaa0e83c1e60be75a9512012bfbe307b7facc7fc65656db5f3f4c3ff`  
		Last Modified: Sat, 28 May 2022 20:52:46 GMT  
		Size: 1.1 KB (1056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7583ca3e72d7ba19d9282d7cceb754c6b78dcc5dafe87fb40ba11abcdfad841b`  
		Last Modified: Sat, 28 May 2022 20:52:47 GMT  
		Size: 6.0 MB (5999195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3c570e58336fa60b88539aef4e1ffa0289798f70a906a55c0b291cf386d76c2`  
		Last Modified: Sat, 28 May 2022 20:52:46 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9a0eb6589f42f53d4c16113fbeee7f38fff9157291e8c9b22be42ce45653820`  
		Last Modified: Sat, 28 May 2022 20:52:46 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; s390x

```console
$ docker pull spiped@sha256:a9442b276bfaee2a75715fe608363309aca4373dc2dc502604bb2bb0d5f4dea8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.8 MB (34845447 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2941968d748f4b2e9298f5f6ecd1c8ef8a6e9fc6074a6649a7b6ea6f03eff523`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 23 Jun 2022 00:43:10 GMT
ADD file:0b511e3efd87267fb27161eae56c4d08f0fed733697da6ffe6ea96a4cb68e938 in / 
# Thu, 23 Jun 2022 00:43:15 GMT
CMD ["bash"]
# Thu, 23 Jun 2022 13:40:29 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Thu, 23 Jun 2022 13:40:31 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Thu, 23 Jun 2022 13:40:32 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 23 Jun 2022 13:40:43 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 23 Jun 2022 13:40:44 GMT
VOLUME [/spiped]
# Thu, 23 Jun 2022 13:40:44 GMT
WORKDIR /spiped
# Thu, 23 Jun 2022 13:40:44 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 23 Jun 2022 13:40:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Jun 2022 13:40:44 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:c547f465e0c8708ad0c57cf09caa52f4c2b5b295bf10ab1ce71ca17ff81ea36a`  
		Last Modified: Thu, 23 Jun 2022 00:51:59 GMT  
		Size: 29.7 MB (29655262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f10418190b72e9fc95fa6f7bd6436f85792a11bac97bf409ebb489733c6cdeb`  
		Last Modified: Thu, 23 Jun 2022 13:41:20 GMT  
		Size: 1.7 KB (1736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d9de83495ba48b01499e858c82e09a1dbed7baa1add5136e5adce6e7d60d452`  
		Last Modified: Thu, 23 Jun 2022 13:41:19 GMT  
		Size: 1.1 KB (1052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1af8046b93a37ad2bb5d08d4a2b031d01e804f6215b67365ba7b72766510a52c`  
		Last Modified: Thu, 23 Jun 2022 13:41:20 GMT  
		Size: 5.2 MB (5186928 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d254cd7b5719c3b1ba5880a1daa9212d49f5999c4c6f371e32d84733730ddcfe`  
		Last Modified: Thu, 23 Jun 2022 13:41:19 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2556f06bac5f4c72f60c12325c5c156dd6d3cc548dbc2d60398e43f72584c19`  
		Last Modified: Thu, 23 Jun 2022 13:41:19 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:1.6-alpine`

```console
$ docker pull spiped@sha256:574b58f2dcd9c3904a6435230c713766d0690f6282db43000ca61e233d59d401
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
$ docker pull spiped@sha256:bdd3a85420e8c8d55b154c7d7f1a043ca1bbae32a53dceaca4838f70ff3376b9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (3022980 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6c7e9665581a5ef894060d275062ab85a542c8fa4a4aae78d4f2617be109e728`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Mon, 23 May 2022 19:19:30 GMT
ADD file:8e81116368669ed3dd361bc898d61bff249f524139a239fdaf3ec46869a39921 in / 
# Mon, 23 May 2022 19:19:31 GMT
CMD ["/bin/sh"]
# Tue, 24 May 2022 19:34:44 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Tue, 24 May 2022 19:34:45 GMT
RUN apk add --no-cache libssl1.1
# Tue, 24 May 2022 19:34:45 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 24 May 2022 19:34:55 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Tue, 24 May 2022 19:34:55 GMT
VOLUME [/spiped]
# Tue, 24 May 2022 19:34:55 GMT
WORKDIR /spiped
# Tue, 24 May 2022 19:34:56 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 24 May 2022 19:34:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 24 May 2022 19:34:56 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:2408cc74d12b6cd092bb8b516ba7d5e290f485d3eb9672efc00f0583730179e8`  
		Last Modified: Mon, 23 May 2022 19:09:38 GMT  
		Size: 2.8 MB (2798889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:becf26afb9051910736e73bcdbfc94bfb72d60a534521c9d4d8bd49f058953ca`  
		Last Modified: Tue, 24 May 2022 19:35:11 GMT  
		Size: 1.3 KB (1271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:744686996785b12019a749f4c09b2b5d59b293aca28e90b0a63b3b6683296350`  
		Last Modified: Tue, 24 May 2022 19:35:11 GMT  
		Size: 7.7 KB (7731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fdf476035643e2d6746fa2acf3e72b7d990dfbf92675e53c57fc5eff30f88ca`  
		Last Modified: Tue, 24 May 2022 19:35:11 GMT  
		Size: 214.6 KB (214618 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a5688549417be3b134e241c450a08175acf2c8cd842b2e30f3310f6a58314a6`  
		Last Modified: Tue, 24 May 2022 19:35:11 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0acff87013e49fae028cf81385e161bc4f11ec1173a9799808132863c6bfa34`  
		Last Modified: Tue, 24 May 2022 19:35:11 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; arm variant v6

```console
$ docker pull spiped@sha256:406809ea0a81e5db518b787d7612be34a70855479615ff4cace100dc08c1ce5d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 MB (2814958 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:765f7c1b3fd5477fdd79037421a66d16f15550314f4344b2e7f359d1ab9f5a6b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Mon, 23 May 2022 19:49:32 GMT
ADD file:f7cee617575b5e5a7672d298a519bb8d8b5098efb90aa2a5d7b0510003457d52 in / 
# Mon, 23 May 2022 19:49:33 GMT
CMD ["/bin/sh"]
# Tue, 24 May 2022 20:14:54 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Tue, 24 May 2022 20:14:56 GMT
RUN apk add --no-cache libssl1.1
# Tue, 24 May 2022 20:14:57 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 24 May 2022 20:15:17 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Tue, 24 May 2022 20:15:18 GMT
VOLUME [/spiped]
# Tue, 24 May 2022 20:15:18 GMT
WORKDIR /spiped
# Tue, 24 May 2022 20:15:19 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 24 May 2022 20:15:19 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 24 May 2022 20:15:20 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:79a25ccaf940855872635c06e7614d9b27dd38ffb5a8adfdb9274dfdc0ea0d87`  
		Last Modified: Mon, 23 May 2022 19:08:47 GMT  
		Size: 2.6 MB (2606142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0a7e07c35741a1549360e780bc005cf673a71e419a28d8a6b9c13991457fd00`  
		Last Modified: Tue, 24 May 2022 20:15:52 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cdf6aebe85933f39c72c58c99c4ec7d111a159f1235bfe85319b66d6203ef8a`  
		Last Modified: Tue, 24 May 2022 20:15:52 GMT  
		Size: 7.7 KB (7726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c66c128b4f04df47fadf6a72f2ba745ba461f8a90f759782eca976719289bfa`  
		Last Modified: Tue, 24 May 2022 20:15:52 GMT  
		Size: 199.3 KB (199349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cff01690378c3c28fddd84bf4b93277c045d39f051cf3b935d00174aa4f2eb45`  
		Last Modified: Tue, 24 May 2022 20:15:52 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fab83e2c93a7364c569439bdd1bcb23f85d4b7900ff40e1cb25bece561c431a`  
		Last Modified: Tue, 24 May 2022 20:15:52 GMT  
		Size: 344.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; arm variant v7

```console
$ docker pull spiped@sha256:acc8ca060038077aa20644d95dfd50f3a9faa59990d2318895033343f94456eb
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 MB (2614203 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:afa4570c887e85e41ae28860d1797be642647270341c2b31a2d07268170d3d18`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Mon, 23 May 2022 18:57:46 GMT
ADD file:72698cc08524b911ebaacf992490707e5a951ddd2fe6edb3fb598e9dc7155049 in / 
# Mon, 23 May 2022 18:57:47 GMT
CMD ["/bin/sh"]
# Tue, 24 May 2022 23:57:01 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Tue, 24 May 2022 23:57:03 GMT
RUN apk add --no-cache libssl1.1
# Tue, 24 May 2022 23:57:03 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 24 May 2022 23:57:23 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Tue, 24 May 2022 23:57:24 GMT
VOLUME [/spiped]
# Tue, 24 May 2022 23:57:24 GMT
WORKDIR /spiped
# Tue, 24 May 2022 23:57:25 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 24 May 2022 23:57:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 24 May 2022 23:57:26 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:6366ba92f08e2418e90171f1e34bd86ecd50fdc95953b3f33b8943c143518eca`  
		Last Modified: Mon, 23 May 2022 18:59:17 GMT  
		Size: 2.4 MB (2411648 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:744a106e187f9790be6dbdde860ada60aab7e95bae779540c813da16ce184ea7`  
		Last Modified: Tue, 24 May 2022 23:58:19 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e8f51295340b65e165fffa3de719118e625ca751a7c465a96dee14a0441de72`  
		Last Modified: Tue, 24 May 2022 23:58:19 GMT  
		Size: 7.7 KB (7717 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a1da9fdb3c39499af6413db4aeed00e8577a949c49968ffd86c20f438118a88`  
		Last Modified: Tue, 24 May 2022 23:58:19 GMT  
		Size: 193.1 KB (193098 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83b416966b1e14463ce73c56ecba5fd804f4c565b4d781199f3b02247ffdf8e7`  
		Last Modified: Tue, 24 May 2022 23:58:19 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f1016107cea29ba85ecc25a6bba5c5c3494ef9ed31194cc5e7b6ea8add7ef4a`  
		Last Modified: Tue, 24 May 2022 23:58:19 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:bdfcd3d661a8017ef3286486269e41c2ab4d2c4662672ea7e21ac01a7e8572c8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 MB (2911518 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:12a66ddef290c67283604068f9b4d679bc4dd400e2bdf0d2826b55e9bdf23aeb`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Mon, 23 May 2022 19:39:22 GMT
ADD file:3ae36c6c4a1fc43157692da97c6c4fa6c3d0189ba82e2bef7f5aaf4a5e083f18 in / 
# Mon, 23 May 2022 19:39:22 GMT
CMD ["/bin/sh"]
# Tue, 24 May 2022 20:25:00 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Tue, 24 May 2022 20:25:02 GMT
RUN apk add --no-cache libssl1.1
# Tue, 24 May 2022 20:25:03 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 24 May 2022 20:25:22 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Tue, 24 May 2022 20:25:23 GMT
VOLUME [/spiped]
# Tue, 24 May 2022 20:25:24 GMT
WORKDIR /spiped
# Tue, 24 May 2022 20:25:26 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 24 May 2022 20:25:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 24 May 2022 20:25:27 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:b3c136eddcbf2003d3180787cef00f39d46b9fd9e4623178282ad6a8d63ad3b0`  
		Last Modified: Mon, 23 May 2022 19:08:34 GMT  
		Size: 2.7 MB (2694464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20a86dbffa956db3e6a8cd773330f1ec06aa87e6987f0f5c9a031e2af7975a9a`  
		Last Modified: Tue, 24 May 2022 20:25:57 GMT  
		Size: 1.2 KB (1244 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:168f9b4c4b922cf44b915dedb800de4176f18b715d6a917a6576a2d24ba0b78a`  
		Last Modified: Tue, 24 May 2022 20:25:57 GMT  
		Size: 7.7 KB (7705 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba2ce83ec0aa17bde883cf7689464f8502798d298fd4296e17e51c9ab614ebd6`  
		Last Modified: Tue, 24 May 2022 20:25:57 GMT  
		Size: 207.7 KB (207671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7796ce5b43cb7f8557eb86d1bb3682848bca4769f1886634356d8952e37e262`  
		Last Modified: Tue, 24 May 2022 20:25:57 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c60cf321cf0b839869c31f5a9ac3374f3c43dba87ab4d0794c93d1436b27e37d`  
		Last Modified: Tue, 24 May 2022 20:25:56 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; 386

```console
$ docker pull spiped@sha256:6eb9e3e76d959724427cca66e52c7bdeebb58c9297c5fd7d60b50838669fe7ef
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (3036399 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b0215089b25dc2844d60ff524e3c7359fc6094c7376d2646e5482fa918c91bad`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Mon, 23 May 2022 19:38:20 GMT
ADD file:1750ccfabfe93636015070d51a6e824cbd738056223421c69d8aaabc38041b18 in / 
# Mon, 23 May 2022 19:38:20 GMT
CMD ["/bin/sh"]
# Tue, 24 May 2022 20:13:25 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Tue, 24 May 2022 20:13:26 GMT
RUN apk add --no-cache libssl1.1
# Tue, 24 May 2022 20:13:27 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 24 May 2022 20:13:38 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Tue, 24 May 2022 20:13:39 GMT
VOLUME [/spiped]
# Tue, 24 May 2022 20:13:40 GMT
WORKDIR /spiped
# Tue, 24 May 2022 20:13:42 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 24 May 2022 20:13:42 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 24 May 2022 20:13:43 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:bb638a3869eed698f88775c7a48f36f8e22e7c6bbaa98fa1d5678966b619b859`  
		Last Modified: Mon, 23 May 2022 19:09:25 GMT  
		Size: 2.8 MB (2801887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:538c30644db57c76ff9a69c435c96a6d269cf8da91c4d632beffff39511588ca`  
		Last Modified: Tue, 24 May 2022 20:14:13 GMT  
		Size: 1.2 KB (1241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d193ad41299c95702ee3dcff9a3399e567cc04c5e640af6cc098795b475843fe`  
		Last Modified: Tue, 24 May 2022 20:14:12 GMT  
		Size: 7.7 KB (7697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec3ef77db5428642bb00b1436a0a844fca99ef4cc676e787f6307ac237f4f65d`  
		Last Modified: Tue, 24 May 2022 20:14:13 GMT  
		Size: 225.1 KB (225139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce435cec46d2206fbfa56e9dc4c9a2907fcd4bdba6acb8c4f332a2f1246e1a8c`  
		Last Modified: Tue, 24 May 2022 20:14:13 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ab3029834f1c60801bbb7cb77e5fec645e494281b466eaed4fb5c5ed38f4b26`  
		Last Modified: Tue, 24 May 2022 20:14:12 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; ppc64le

```console
$ docker pull spiped@sha256:394770c1c3e52c18b2e060896dc946a7de8c0581c1691fe3a2458c6442d51071
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (3012900 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:45dd65bd18433f8227345eb1bc628c92fb777cc4d5e9e790835ba272eaadec4e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Mon, 23 May 2022 19:16:51 GMT
ADD file:6a5450c8a7cee3ceda59e7cb350c54df4139b0f7b7cf49c8b31bb9c01646c3cd in / 
# Mon, 23 May 2022 19:16:53 GMT
CMD ["/bin/sh"]
# Tue, 24 May 2022 19:50:10 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Tue, 24 May 2022 19:50:18 GMT
RUN apk add --no-cache libssl1.1
# Tue, 24 May 2022 19:50:20 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 24 May 2022 19:50:38 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Tue, 24 May 2022 19:50:42 GMT
VOLUME [/spiped]
# Tue, 24 May 2022 19:50:47 GMT
WORKDIR /spiped
# Tue, 24 May 2022 19:50:48 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 24 May 2022 19:50:52 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 24 May 2022 19:50:56 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:d3deabf2a506ef6f5fa7c2a68bf27047574cef9908b30a97ff2d01ae539b089a`  
		Last Modified: Mon, 23 May 2022 19:09:13 GMT  
		Size: 2.8 MB (2789745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6d245add1998dabc480629fde1ae678cfbb96f740737e4acede363c37eda348`  
		Last Modified: Tue, 24 May 2022 19:51:36 GMT  
		Size: 1.3 KB (1272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bea94be815996b73043903da4f60b4ea3573e9689c5b3b1b0348ef5ef54fe25b`  
		Last Modified: Tue, 24 May 2022 19:51:36 GMT  
		Size: 7.7 KB (7727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b25cc9d25fe567c300c07c50cb1d341544a9751b92d44874cef5399d1beee0aa`  
		Last Modified: Tue, 24 May 2022 19:51:36 GMT  
		Size: 213.7 KB (213687 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2b003e2ac252266dcd49f568ddc62ed5a04668bc0655e7cd74521a21c0089eb`  
		Last Modified: Tue, 24 May 2022 19:51:36 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fed434cd18f8048c2624c1d26c27721d4ce3e46b39d5d9adcbeec4733e3954ff`  
		Last Modified: Tue, 24 May 2022 19:51:36 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; s390x

```console
$ docker pull spiped@sha256:4c56dd9796353102785f0a5f8f38e81e0638a1ca2b745795770b8e137ebc657d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 MB (2791966 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a3497d9a69b26f419f935637e370f6a57f1d4e5ad7000970a7ecdcbf0333263c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Mon, 23 May 2022 19:41:59 GMT
ADD file:e1852d8ef555a0d3ef6d0b74a898720c82bb9f491430b06a0dd0499497ce118e in / 
# Mon, 23 May 2022 19:42:10 GMT
CMD ["/bin/sh"]
# Tue, 24 May 2022 20:27:25 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Tue, 24 May 2022 20:27:27 GMT
RUN apk add --no-cache libssl1.1
# Tue, 24 May 2022 20:27:27 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 24 May 2022 20:27:35 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Tue, 24 May 2022 20:27:36 GMT
VOLUME [/spiped]
# Tue, 24 May 2022 20:27:36 GMT
WORKDIR /spiped
# Tue, 24 May 2022 20:27:37 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 24 May 2022 20:27:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 24 May 2022 20:27:38 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:af1ac1a73384e058591d04d19bc05a06781cc32d52d4593b468d6cb95eda9858`  
		Last Modified: Mon, 23 May 2022 19:43:36 GMT  
		Size: 2.6 MB (2580494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9623718447e29295a23001aae3dbed26ca7b41b14965f02c9ae5324963330ef0`  
		Last Modified: Tue, 24 May 2022 20:28:11 GMT  
		Size: 1.3 KB (1267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74a000d8db4a14acf7833a4d32f3d85f452d72236f3a96360d4518ee2abba268`  
		Last Modified: Tue, 24 May 2022 20:28:11 GMT  
		Size: 7.7 KB (7722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4024830388cfd5531b6e2ca6468204a9d4fb81958bad00a9f8694fcea02a1d0`  
		Last Modified: Tue, 24 May 2022 20:28:11 GMT  
		Size: 202.0 KB (202015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f77170c060013a5bc5e10927cde6e8c315bd601aab054eb5717725f98bb2b0c`  
		Last Modified: Tue, 24 May 2022 20:28:11 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6dcb80a5752c8255af9b16d7c0d66266c0e5ecfec63891ebdb6c7a2d47ff7c71`  
		Last Modified: Tue, 24 May 2022 20:28:11 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:1.6.2`

```console
$ docker pull spiped@sha256:2a04458cf6cb5fa31173ddeeaec6840207e46a3186dbb1e1de6b3c83a009c5d0
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
$ docker pull spiped@sha256:b2ff44d1d923f53540c90249f0186c6bcc7dccb99603a5bcb501d4aa81fda546
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.3 MB (37349979 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5823c93a49f14efb19ac802a6042b74cb55529fbfcce6ab550db72f9b6a7dd30`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 23 Jun 2022 00:20:27 GMT
ADD file:8adbbab04d6f84cd83b5f4205b89b0acb7ecbf27a1bb2dc181d0a629479039fe in / 
# Thu, 23 Jun 2022 00:20:27 GMT
CMD ["bash"]
# Thu, 23 Jun 2022 14:24:59 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Thu, 23 Jun 2022 14:25:02 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Thu, 23 Jun 2022 14:25:02 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 23 Jun 2022 14:25:21 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 23 Jun 2022 14:25:21 GMT
VOLUME [/spiped]
# Thu, 23 Jun 2022 14:25:22 GMT
WORKDIR /spiped
# Thu, 23 Jun 2022 14:25:22 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 23 Jun 2022 14:25:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Jun 2022 14:25:22 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:b85a868b505ffd0342a37e6a3b1c49f7c71878afe569a807e6238ef08252fcb7`  
		Last Modified: Thu, 23 Jun 2022 00:25:18 GMT  
		Size: 31.4 MB (31379408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55454b6a8916eece033c9dfe8babcaa0cd04c0901055b9040e2eac12cbb05f97`  
		Last Modified: Thu, 23 Jun 2022 14:25:40 GMT  
		Size: 1.7 KB (1733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dad7666375bb50bbfccbc5bad922741a65570699f108894f77601d31d4b76fba`  
		Last Modified: Thu, 23 Jun 2022 14:25:40 GMT  
		Size: 1.1 KB (1052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43a0a6b62b5421f4c74facfba698b0434d6899e1c77c61fefc4f28e7a0ab10d1`  
		Last Modified: Thu, 23 Jun 2022 14:25:41 GMT  
		Size: 6.0 MB (5967315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:756782629170475511f5a3ee4cb4717e152d25e3993ecc99aa0772dd2a518179`  
		Last Modified: Thu, 23 Jun 2022 14:25:40 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:331a176397a9e42d10ecaaae616afffdfffaef1527eb16f81d10ae9141ba19cf`  
		Last Modified: Thu, 23 Jun 2022 14:25:40 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.2` - linux; arm variant v5

```console
$ docker pull spiped@sha256:feec4c6defea9575b6b723a20ac0d667a6a0b7c896a4553cd8950674899f1d6f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.0 MB (33952417 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:609536328e039bda4f2dd352cefca6776a998bd2debfa65c39928aa2052752d3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Sat, 28 May 2022 02:03:06 GMT
ADD file:d9560b279f64bc3973a6aaa0e0ab8f483d60a1c66647899850689eee01a729ec in / 
# Sat, 28 May 2022 02:03:07 GMT
CMD ["bash"]
# Sat, 28 May 2022 19:53:26 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Sat, 28 May 2022 19:53:35 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 19:53:35 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Sat, 28 May 2022 19:54:26 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Sat, 28 May 2022 19:54:27 GMT
VOLUME [/spiped]
# Sat, 28 May 2022 19:54:27 GMT
WORKDIR /spiped
# Sat, 28 May 2022 19:54:28 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 28 May 2022 19:54:28 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 28 May 2022 19:54:29 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:b24540c95c3d5b61dba94dfa3665e0cc1231b3602edfb61432041c1f108be50d`  
		Last Modified: Sat, 28 May 2022 02:18:37 GMT  
		Size: 28.9 MB (28921471 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aea4df7367cff72ae8d9118ef5266476e59c66462928466d605c1d9623180448`  
		Last Modified: Sat, 28 May 2022 19:55:02 GMT  
		Size: 1.7 KB (1727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:246aeb209300265ffd136d8ef9420bc206bd86aec58047847f3aa4e50cf3c3eb`  
		Last Modified: Sat, 28 May 2022 19:55:02 GMT  
		Size: 1.1 KB (1054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bf79bde433a8bd87a705f9a94a90ee36cc3fcc94f66f88444fe45670af95100`  
		Last Modified: Sat, 28 May 2022 19:55:07 GMT  
		Size: 5.0 MB (5027692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9733b89df15002a08795a040cdad7e97743b49f08303f89ae9d1a578f43d4782`  
		Last Modified: Sat, 28 May 2022 19:55:02 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dce9b97ee80126486958e7e92f4caa4888c8367d20d8d39bec8c62797aee6cfd`  
		Last Modified: Sat, 28 May 2022 19:55:02 GMT  
		Size: 344.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.2` - linux; arm variant v7

```console
$ docker pull spiped@sha256:27ceab9292afad9550739501c64b6f5cc11c3dbe3b65f93bcc390c4120433c51
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.3 MB (31327718 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:22929e8964c6549f3d8123da06f309aa6f679e4714692df4bfa197d0e2c8f399`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Sat, 28 May 2022 00:59:48 GMT
ADD file:975c801b5b50aa75e07d18e69af11f21e165561abc16246e2c413c2ef96ce4c6 in / 
# Sat, 28 May 2022 00:59:49 GMT
CMD ["bash"]
# Sun, 29 May 2022 06:25:09 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Sun, 29 May 2022 06:25:16 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Sun, 29 May 2022 06:25:16 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Sun, 29 May 2022 06:26:02 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Sun, 29 May 2022 06:26:03 GMT
VOLUME [/spiped]
# Sun, 29 May 2022 06:26:03 GMT
WORKDIR /spiped
# Sun, 29 May 2022 06:26:04 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sun, 29 May 2022 06:26:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sun, 29 May 2022 06:26:05 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:eeb117569618df53320eb28d32b7a1d87792bda3362017123fa1025b55db44c3`  
		Last Modified: Sat, 28 May 2022 01:15:35 GMT  
		Size: 26.6 MB (26576237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f673a628d46f411f6fa471dacc6a7f093320a9060f586c46fd61466e55c0e684`  
		Last Modified: Sun, 29 May 2022 06:27:04 GMT  
		Size: 1.7 KB (1726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b972855b62da685c2bb09ca3ed5808bfc51cd9b062ad73b9ba2a0ac8497e321`  
		Last Modified: Sun, 29 May 2022 06:27:04 GMT  
		Size: 1.1 KB (1054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abf09d9445796b62d51bb11fe3f1236c17a50784d5fb850e1b26d4bcc677b3b2`  
		Last Modified: Sun, 29 May 2022 06:27:08 GMT  
		Size: 4.7 MB (4748232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:988142d33ab11d2901370155c8b902ad639de76fd48866e961b307372b37cee8`  
		Last Modified: Sun, 29 May 2022 06:27:04 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b5ba53ff286b0137dddc9613a5e23aacaa1cf035b46b78799a9dcba485d0c63`  
		Last Modified: Sun, 29 May 2022 06:27:04 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.2` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:50b5813789a1de2455e1602e814b1ba46c2f92226a13ce8acb0a33e3bb237ef8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.3 MB (35339663 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:79448de18bfa13cb33bf4a88178cbea587a26f574f5db947d339d48f822e6be8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 23 Jun 2022 00:40:43 GMT
ADD file:134be48af13f80f3474bf1b080ca781feb7b972148d482849862e55eb2acd61c in / 
# Thu, 23 Jun 2022 00:40:44 GMT
CMD ["bash"]
# Thu, 23 Jun 2022 14:19:37 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Thu, 23 Jun 2022 14:19:40 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Thu, 23 Jun 2022 14:19:41 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 23 Jun 2022 14:19:59 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 23 Jun 2022 14:19:59 GMT
VOLUME [/spiped]
# Thu, 23 Jun 2022 14:20:00 GMT
WORKDIR /spiped
# Thu, 23 Jun 2022 14:20:02 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 23 Jun 2022 14:20:02 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Jun 2022 14:20:03 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:3b157c852f2736e12f09046f214fe5f6a0b1652bd860269b3988c92a197026e8`  
		Last Modified: Thu, 23 Jun 2022 00:47:22 GMT  
		Size: 30.1 MB (30065720 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d2b50ae5c80cf61302029794b9bb8788bc1c4340583fe19b3886a328bd2e59c`  
		Last Modified: Thu, 23 Jun 2022 14:20:30 GMT  
		Size: 1.6 KB (1618 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3f8033bf687e78771c0955fb5ad0dbd87fe3ecbadc7779f0fbff1ddaed4a38b`  
		Last Modified: Thu, 23 Jun 2022 14:20:30 GMT  
		Size: 925.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90442e6da9e0bf71d16d1004502b61ac0ee04335adeb4ea1c0f5322793923308`  
		Last Modified: Thu, 23 Jun 2022 14:20:31 GMT  
		Size: 5.3 MB (5270963 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c1a82ee02be4fd41ba26092fcccc4a7ef039055a227e0d7f92ad587546071ad`  
		Last Modified: Thu, 23 Jun 2022 14:20:30 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad041befbc894c998e7065d943ec5a35b70eaf5024d5e19fa6192a489202122a`  
		Last Modified: Thu, 23 Jun 2022 14:20:30 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.2` - linux; 386

```console
$ docker pull spiped@sha256:0418180e629bf6c4c671ceb932c0bb7d8cc2245cd53ad80a3f9ff42a289131bf
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.3 MB (40284635 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f33d96114c1233c804814373fd9cd85fb08296fa76ac20445c2fe9d2fa0ac225`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 23 Jun 2022 00:39:33 GMT
ADD file:9d46d3f8fb63833a6dbd8dd796ad541d556046a48342d22e1fd3bffa3fb8e504 in / 
# Thu, 23 Jun 2022 00:39:33 GMT
CMD ["bash"]
# Thu, 23 Jun 2022 15:04:24 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Thu, 23 Jun 2022 15:04:28 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Thu, 23 Jun 2022 15:04:29 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 23 Jun 2022 15:04:49 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 23 Jun 2022 15:04:50 GMT
VOLUME [/spiped]
# Thu, 23 Jun 2022 15:04:51 GMT
WORKDIR /spiped
# Thu, 23 Jun 2022 15:04:53 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 23 Jun 2022 15:04:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Jun 2022 15:04:54 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:4870b12e407743816673c11cfb39974d80c1569d876287bef61f8c585954822f`  
		Last Modified: Thu, 23 Jun 2022 00:46:40 GMT  
		Size: 32.4 MB (32390198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:886cea7325b13f7203d5e830883ba71c98d83a0686704a1b6982442fd97d827c`  
		Last Modified: Thu, 23 Jun 2022 15:05:25 GMT  
		Size: 1.6 KB (1610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6a0a4b187e0c9f93860637c1c720af4b8e8cf1d089783dfbf0a07ba662fac22`  
		Last Modified: Thu, 23 Jun 2022 15:05:25 GMT  
		Size: 925.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bb9eaa94baa3de99a61cef041ce22494d7ffdbbbdabc1ea1629f4bb0d977bdd`  
		Last Modified: Thu, 23 Jun 2022 15:05:27 GMT  
		Size: 7.9 MB (7891464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3560d550fd7c038f01cf33f88495c9761131e2304f6d1f17a85e272656dd82ff`  
		Last Modified: Thu, 23 Jun 2022 15:05:25 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:776c52a49bfdec3ad5665559540af9ec46f9eced7d9aa5d664aaa96582d28fb4`  
		Last Modified: Thu, 23 Jun 2022 15:05:25 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.2` - linux; mips64le

```console
$ docker pull spiped@sha256:327ab349035e42e2520c87903f12e1e4b8aa2b46f5af20028c6148d435015ac6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.3 MB (35349399 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:134640be221db73739d4c6d145ed454eb1f6b7c530d7b5a037f8566a5c50d315`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Sat, 28 May 2022 01:11:13 GMT
ADD file:f685a156b7ddafe7bafc6fad17cc36cc8a5d6d922fc1c425656ca92266d9a98e in / 
# Sat, 28 May 2022 01:11:18 GMT
CMD ["bash"]
# Sat, 28 May 2022 11:02:07 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Sat, 28 May 2022 11:02:24 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 11:02:26 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Sat, 28 May 2022 11:03:57 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Sat, 28 May 2022 11:04:00 GMT
VOLUME [/spiped]
# Sat, 28 May 2022 11:04:03 GMT
WORKDIR /spiped
# Sat, 28 May 2022 11:04:06 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 28 May 2022 11:04:08 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 28 May 2022 11:04:11 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:fdea7139ce36b557a23c4b9c4255387b175f851ed0c51e1e7d78dd301c0e4da8`  
		Last Modified: Sat, 28 May 2022 01:21:35 GMT  
		Size: 29.6 MB (29641237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:638fcc9a2aca909e0ddad028b40a02f45370c5c4864972531afa7a02e7d5f8b5`  
		Last Modified: Sat, 28 May 2022 11:04:37 GMT  
		Size: 1.6 KB (1620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62732d2f48eb3a503a80f0fcc97263b3feb49c39cfec9026b62d02698d569084`  
		Last Modified: Sat, 28 May 2022 11:04:37 GMT  
		Size: 925.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec6d02d49d5fc774a71ed9e0211b9250e5926d8a45f48011929bc45eea21a764`  
		Last Modified: Sat, 28 May 2022 11:04:43 GMT  
		Size: 5.7 MB (5705180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:551ee4c909a9bed061c23e73af4c6586e9b6144160f20081c7c31a2e78d21357`  
		Last Modified: Sat, 28 May 2022 11:04:37 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8231a7adeed86962f2691999debe4256643805fd3dd1b4deb1e8e6d30fbd2e2`  
		Last Modified: Sat, 28 May 2022 11:04:37 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.2` - linux; ppc64le

```console
$ docker pull spiped@sha256:b6377c503b8d6a42b6db7ff3590aca7406bbb9fb1550d8baaf89f61ee4e6f222
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.3 MB (41289157 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ed59345839d9409f475ce2fce73fb95e4ba9c41a970711589fb2014d87459aa9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Sat, 28 May 2022 01:22:54 GMT
ADD file:64e264b12eed99d87380e38f36bfecd62b9bb1e5460f0242cfbc5dc76c212ead in / 
# Sat, 28 May 2022 01:22:59 GMT
CMD ["bash"]
# Sat, 28 May 2022 20:47:31 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Sat, 28 May 2022 20:47:49 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 20:48:09 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Sat, 28 May 2022 20:50:59 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Sat, 28 May 2022 20:51:04 GMT
VOLUME [/spiped]
# Sat, 28 May 2022 20:51:09 GMT
WORKDIR /spiped
# Sat, 28 May 2022 20:51:31 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 28 May 2022 20:51:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 28 May 2022 20:52:04 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:893e245a8f6219935016f2dd4422ec4b7fdab43d98ba29c024ec0d9ce57794ba`  
		Last Modified: Sat, 28 May 2022 01:32:28 GMT  
		Size: 35.3 MB (35286698 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:922a5f50c37cc3b0d1fef17e00862a91bd28f367cd75a7ad0414852ec8d6809e`  
		Last Modified: Sat, 28 May 2022 20:52:46 GMT  
		Size: 1.7 KB (1737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59b8faf9aaa0e83c1e60be75a9512012bfbe307b7facc7fc65656db5f3f4c3ff`  
		Last Modified: Sat, 28 May 2022 20:52:46 GMT  
		Size: 1.1 KB (1056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7583ca3e72d7ba19d9282d7cceb754c6b78dcc5dafe87fb40ba11abcdfad841b`  
		Last Modified: Sat, 28 May 2022 20:52:47 GMT  
		Size: 6.0 MB (5999195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3c570e58336fa60b88539aef4e1ffa0289798f70a906a55c0b291cf386d76c2`  
		Last Modified: Sat, 28 May 2022 20:52:46 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9a0eb6589f42f53d4c16113fbeee7f38fff9157291e8c9b22be42ce45653820`  
		Last Modified: Sat, 28 May 2022 20:52:46 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.2` - linux; s390x

```console
$ docker pull spiped@sha256:a9442b276bfaee2a75715fe608363309aca4373dc2dc502604bb2bb0d5f4dea8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.8 MB (34845447 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2941968d748f4b2e9298f5f6ecd1c8ef8a6e9fc6074a6649a7b6ea6f03eff523`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 23 Jun 2022 00:43:10 GMT
ADD file:0b511e3efd87267fb27161eae56c4d08f0fed733697da6ffe6ea96a4cb68e938 in / 
# Thu, 23 Jun 2022 00:43:15 GMT
CMD ["bash"]
# Thu, 23 Jun 2022 13:40:29 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Thu, 23 Jun 2022 13:40:31 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Thu, 23 Jun 2022 13:40:32 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 23 Jun 2022 13:40:43 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 23 Jun 2022 13:40:44 GMT
VOLUME [/spiped]
# Thu, 23 Jun 2022 13:40:44 GMT
WORKDIR /spiped
# Thu, 23 Jun 2022 13:40:44 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 23 Jun 2022 13:40:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Jun 2022 13:40:44 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:c547f465e0c8708ad0c57cf09caa52f4c2b5b295bf10ab1ce71ca17ff81ea36a`  
		Last Modified: Thu, 23 Jun 2022 00:51:59 GMT  
		Size: 29.7 MB (29655262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f10418190b72e9fc95fa6f7bd6436f85792a11bac97bf409ebb489733c6cdeb`  
		Last Modified: Thu, 23 Jun 2022 13:41:20 GMT  
		Size: 1.7 KB (1736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d9de83495ba48b01499e858c82e09a1dbed7baa1add5136e5adce6e7d60d452`  
		Last Modified: Thu, 23 Jun 2022 13:41:19 GMT  
		Size: 1.1 KB (1052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1af8046b93a37ad2bb5d08d4a2b031d01e804f6215b67365ba7b72766510a52c`  
		Last Modified: Thu, 23 Jun 2022 13:41:20 GMT  
		Size: 5.2 MB (5186928 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d254cd7b5719c3b1ba5880a1daa9212d49f5999c4c6f371e32d84733730ddcfe`  
		Last Modified: Thu, 23 Jun 2022 13:41:19 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2556f06bac5f4c72f60c12325c5c156dd6d3cc548dbc2d60398e43f72584c19`  
		Last Modified: Thu, 23 Jun 2022 13:41:19 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:1.6.2-alpine`

```console
$ docker pull spiped@sha256:574b58f2dcd9c3904a6435230c713766d0690f6282db43000ca61e233d59d401
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
$ docker pull spiped@sha256:bdd3a85420e8c8d55b154c7d7f1a043ca1bbae32a53dceaca4838f70ff3376b9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (3022980 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6c7e9665581a5ef894060d275062ab85a542c8fa4a4aae78d4f2617be109e728`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Mon, 23 May 2022 19:19:30 GMT
ADD file:8e81116368669ed3dd361bc898d61bff249f524139a239fdaf3ec46869a39921 in / 
# Mon, 23 May 2022 19:19:31 GMT
CMD ["/bin/sh"]
# Tue, 24 May 2022 19:34:44 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Tue, 24 May 2022 19:34:45 GMT
RUN apk add --no-cache libssl1.1
# Tue, 24 May 2022 19:34:45 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 24 May 2022 19:34:55 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Tue, 24 May 2022 19:34:55 GMT
VOLUME [/spiped]
# Tue, 24 May 2022 19:34:55 GMT
WORKDIR /spiped
# Tue, 24 May 2022 19:34:56 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 24 May 2022 19:34:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 24 May 2022 19:34:56 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:2408cc74d12b6cd092bb8b516ba7d5e290f485d3eb9672efc00f0583730179e8`  
		Last Modified: Mon, 23 May 2022 19:09:38 GMT  
		Size: 2.8 MB (2798889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:becf26afb9051910736e73bcdbfc94bfb72d60a534521c9d4d8bd49f058953ca`  
		Last Modified: Tue, 24 May 2022 19:35:11 GMT  
		Size: 1.3 KB (1271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:744686996785b12019a749f4c09b2b5d59b293aca28e90b0a63b3b6683296350`  
		Last Modified: Tue, 24 May 2022 19:35:11 GMT  
		Size: 7.7 KB (7731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fdf476035643e2d6746fa2acf3e72b7d990dfbf92675e53c57fc5eff30f88ca`  
		Last Modified: Tue, 24 May 2022 19:35:11 GMT  
		Size: 214.6 KB (214618 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a5688549417be3b134e241c450a08175acf2c8cd842b2e30f3310f6a58314a6`  
		Last Modified: Tue, 24 May 2022 19:35:11 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0acff87013e49fae028cf81385e161bc4f11ec1173a9799808132863c6bfa34`  
		Last Modified: Tue, 24 May 2022 19:35:11 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.2-alpine` - linux; arm variant v6

```console
$ docker pull spiped@sha256:406809ea0a81e5db518b787d7612be34a70855479615ff4cace100dc08c1ce5d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 MB (2814958 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:765f7c1b3fd5477fdd79037421a66d16f15550314f4344b2e7f359d1ab9f5a6b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Mon, 23 May 2022 19:49:32 GMT
ADD file:f7cee617575b5e5a7672d298a519bb8d8b5098efb90aa2a5d7b0510003457d52 in / 
# Mon, 23 May 2022 19:49:33 GMT
CMD ["/bin/sh"]
# Tue, 24 May 2022 20:14:54 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Tue, 24 May 2022 20:14:56 GMT
RUN apk add --no-cache libssl1.1
# Tue, 24 May 2022 20:14:57 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 24 May 2022 20:15:17 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Tue, 24 May 2022 20:15:18 GMT
VOLUME [/spiped]
# Tue, 24 May 2022 20:15:18 GMT
WORKDIR /spiped
# Tue, 24 May 2022 20:15:19 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 24 May 2022 20:15:19 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 24 May 2022 20:15:20 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:79a25ccaf940855872635c06e7614d9b27dd38ffb5a8adfdb9274dfdc0ea0d87`  
		Last Modified: Mon, 23 May 2022 19:08:47 GMT  
		Size: 2.6 MB (2606142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0a7e07c35741a1549360e780bc005cf673a71e419a28d8a6b9c13991457fd00`  
		Last Modified: Tue, 24 May 2022 20:15:52 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cdf6aebe85933f39c72c58c99c4ec7d111a159f1235bfe85319b66d6203ef8a`  
		Last Modified: Tue, 24 May 2022 20:15:52 GMT  
		Size: 7.7 KB (7726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c66c128b4f04df47fadf6a72f2ba745ba461f8a90f759782eca976719289bfa`  
		Last Modified: Tue, 24 May 2022 20:15:52 GMT  
		Size: 199.3 KB (199349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cff01690378c3c28fddd84bf4b93277c045d39f051cf3b935d00174aa4f2eb45`  
		Last Modified: Tue, 24 May 2022 20:15:52 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fab83e2c93a7364c569439bdd1bcb23f85d4b7900ff40e1cb25bece561c431a`  
		Last Modified: Tue, 24 May 2022 20:15:52 GMT  
		Size: 344.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.2-alpine` - linux; arm variant v7

```console
$ docker pull spiped@sha256:acc8ca060038077aa20644d95dfd50f3a9faa59990d2318895033343f94456eb
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 MB (2614203 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:afa4570c887e85e41ae28860d1797be642647270341c2b31a2d07268170d3d18`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Mon, 23 May 2022 18:57:46 GMT
ADD file:72698cc08524b911ebaacf992490707e5a951ddd2fe6edb3fb598e9dc7155049 in / 
# Mon, 23 May 2022 18:57:47 GMT
CMD ["/bin/sh"]
# Tue, 24 May 2022 23:57:01 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Tue, 24 May 2022 23:57:03 GMT
RUN apk add --no-cache libssl1.1
# Tue, 24 May 2022 23:57:03 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 24 May 2022 23:57:23 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Tue, 24 May 2022 23:57:24 GMT
VOLUME [/spiped]
# Tue, 24 May 2022 23:57:24 GMT
WORKDIR /spiped
# Tue, 24 May 2022 23:57:25 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 24 May 2022 23:57:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 24 May 2022 23:57:26 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:6366ba92f08e2418e90171f1e34bd86ecd50fdc95953b3f33b8943c143518eca`  
		Last Modified: Mon, 23 May 2022 18:59:17 GMT  
		Size: 2.4 MB (2411648 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:744a106e187f9790be6dbdde860ada60aab7e95bae779540c813da16ce184ea7`  
		Last Modified: Tue, 24 May 2022 23:58:19 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e8f51295340b65e165fffa3de719118e625ca751a7c465a96dee14a0441de72`  
		Last Modified: Tue, 24 May 2022 23:58:19 GMT  
		Size: 7.7 KB (7717 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a1da9fdb3c39499af6413db4aeed00e8577a949c49968ffd86c20f438118a88`  
		Last Modified: Tue, 24 May 2022 23:58:19 GMT  
		Size: 193.1 KB (193098 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83b416966b1e14463ce73c56ecba5fd804f4c565b4d781199f3b02247ffdf8e7`  
		Last Modified: Tue, 24 May 2022 23:58:19 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f1016107cea29ba85ecc25a6bba5c5c3494ef9ed31194cc5e7b6ea8add7ef4a`  
		Last Modified: Tue, 24 May 2022 23:58:19 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.2-alpine` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:bdfcd3d661a8017ef3286486269e41c2ab4d2c4662672ea7e21ac01a7e8572c8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 MB (2911518 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:12a66ddef290c67283604068f9b4d679bc4dd400e2bdf0d2826b55e9bdf23aeb`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Mon, 23 May 2022 19:39:22 GMT
ADD file:3ae36c6c4a1fc43157692da97c6c4fa6c3d0189ba82e2bef7f5aaf4a5e083f18 in / 
# Mon, 23 May 2022 19:39:22 GMT
CMD ["/bin/sh"]
# Tue, 24 May 2022 20:25:00 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Tue, 24 May 2022 20:25:02 GMT
RUN apk add --no-cache libssl1.1
# Tue, 24 May 2022 20:25:03 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 24 May 2022 20:25:22 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Tue, 24 May 2022 20:25:23 GMT
VOLUME [/spiped]
# Tue, 24 May 2022 20:25:24 GMT
WORKDIR /spiped
# Tue, 24 May 2022 20:25:26 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 24 May 2022 20:25:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 24 May 2022 20:25:27 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:b3c136eddcbf2003d3180787cef00f39d46b9fd9e4623178282ad6a8d63ad3b0`  
		Last Modified: Mon, 23 May 2022 19:08:34 GMT  
		Size: 2.7 MB (2694464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20a86dbffa956db3e6a8cd773330f1ec06aa87e6987f0f5c9a031e2af7975a9a`  
		Last Modified: Tue, 24 May 2022 20:25:57 GMT  
		Size: 1.2 KB (1244 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:168f9b4c4b922cf44b915dedb800de4176f18b715d6a917a6576a2d24ba0b78a`  
		Last Modified: Tue, 24 May 2022 20:25:57 GMT  
		Size: 7.7 KB (7705 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba2ce83ec0aa17bde883cf7689464f8502798d298fd4296e17e51c9ab614ebd6`  
		Last Modified: Tue, 24 May 2022 20:25:57 GMT  
		Size: 207.7 KB (207671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7796ce5b43cb7f8557eb86d1bb3682848bca4769f1886634356d8952e37e262`  
		Last Modified: Tue, 24 May 2022 20:25:57 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c60cf321cf0b839869c31f5a9ac3374f3c43dba87ab4d0794c93d1436b27e37d`  
		Last Modified: Tue, 24 May 2022 20:25:56 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.2-alpine` - linux; 386

```console
$ docker pull spiped@sha256:6eb9e3e76d959724427cca66e52c7bdeebb58c9297c5fd7d60b50838669fe7ef
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (3036399 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b0215089b25dc2844d60ff524e3c7359fc6094c7376d2646e5482fa918c91bad`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Mon, 23 May 2022 19:38:20 GMT
ADD file:1750ccfabfe93636015070d51a6e824cbd738056223421c69d8aaabc38041b18 in / 
# Mon, 23 May 2022 19:38:20 GMT
CMD ["/bin/sh"]
# Tue, 24 May 2022 20:13:25 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Tue, 24 May 2022 20:13:26 GMT
RUN apk add --no-cache libssl1.1
# Tue, 24 May 2022 20:13:27 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 24 May 2022 20:13:38 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Tue, 24 May 2022 20:13:39 GMT
VOLUME [/spiped]
# Tue, 24 May 2022 20:13:40 GMT
WORKDIR /spiped
# Tue, 24 May 2022 20:13:42 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 24 May 2022 20:13:42 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 24 May 2022 20:13:43 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:bb638a3869eed698f88775c7a48f36f8e22e7c6bbaa98fa1d5678966b619b859`  
		Last Modified: Mon, 23 May 2022 19:09:25 GMT  
		Size: 2.8 MB (2801887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:538c30644db57c76ff9a69c435c96a6d269cf8da91c4d632beffff39511588ca`  
		Last Modified: Tue, 24 May 2022 20:14:13 GMT  
		Size: 1.2 KB (1241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d193ad41299c95702ee3dcff9a3399e567cc04c5e640af6cc098795b475843fe`  
		Last Modified: Tue, 24 May 2022 20:14:12 GMT  
		Size: 7.7 KB (7697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec3ef77db5428642bb00b1436a0a844fca99ef4cc676e787f6307ac237f4f65d`  
		Last Modified: Tue, 24 May 2022 20:14:13 GMT  
		Size: 225.1 KB (225139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce435cec46d2206fbfa56e9dc4c9a2907fcd4bdba6acb8c4f332a2f1246e1a8c`  
		Last Modified: Tue, 24 May 2022 20:14:13 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ab3029834f1c60801bbb7cb77e5fec645e494281b466eaed4fb5c5ed38f4b26`  
		Last Modified: Tue, 24 May 2022 20:14:12 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.2-alpine` - linux; ppc64le

```console
$ docker pull spiped@sha256:394770c1c3e52c18b2e060896dc946a7de8c0581c1691fe3a2458c6442d51071
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (3012900 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:45dd65bd18433f8227345eb1bc628c92fb777cc4d5e9e790835ba272eaadec4e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Mon, 23 May 2022 19:16:51 GMT
ADD file:6a5450c8a7cee3ceda59e7cb350c54df4139b0f7b7cf49c8b31bb9c01646c3cd in / 
# Mon, 23 May 2022 19:16:53 GMT
CMD ["/bin/sh"]
# Tue, 24 May 2022 19:50:10 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Tue, 24 May 2022 19:50:18 GMT
RUN apk add --no-cache libssl1.1
# Tue, 24 May 2022 19:50:20 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 24 May 2022 19:50:38 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Tue, 24 May 2022 19:50:42 GMT
VOLUME [/spiped]
# Tue, 24 May 2022 19:50:47 GMT
WORKDIR /spiped
# Tue, 24 May 2022 19:50:48 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 24 May 2022 19:50:52 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 24 May 2022 19:50:56 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:d3deabf2a506ef6f5fa7c2a68bf27047574cef9908b30a97ff2d01ae539b089a`  
		Last Modified: Mon, 23 May 2022 19:09:13 GMT  
		Size: 2.8 MB (2789745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6d245add1998dabc480629fde1ae678cfbb96f740737e4acede363c37eda348`  
		Last Modified: Tue, 24 May 2022 19:51:36 GMT  
		Size: 1.3 KB (1272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bea94be815996b73043903da4f60b4ea3573e9689c5b3b1b0348ef5ef54fe25b`  
		Last Modified: Tue, 24 May 2022 19:51:36 GMT  
		Size: 7.7 KB (7727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b25cc9d25fe567c300c07c50cb1d341544a9751b92d44874cef5399d1beee0aa`  
		Last Modified: Tue, 24 May 2022 19:51:36 GMT  
		Size: 213.7 KB (213687 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2b003e2ac252266dcd49f568ddc62ed5a04668bc0655e7cd74521a21c0089eb`  
		Last Modified: Tue, 24 May 2022 19:51:36 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fed434cd18f8048c2624c1d26c27721d4ce3e46b39d5d9adcbeec4733e3954ff`  
		Last Modified: Tue, 24 May 2022 19:51:36 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.2-alpine` - linux; s390x

```console
$ docker pull spiped@sha256:4c56dd9796353102785f0a5f8f38e81e0638a1ca2b745795770b8e137ebc657d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 MB (2791966 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a3497d9a69b26f419f935637e370f6a57f1d4e5ad7000970a7ecdcbf0333263c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Mon, 23 May 2022 19:41:59 GMT
ADD file:e1852d8ef555a0d3ef6d0b74a898720c82bb9f491430b06a0dd0499497ce118e in / 
# Mon, 23 May 2022 19:42:10 GMT
CMD ["/bin/sh"]
# Tue, 24 May 2022 20:27:25 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Tue, 24 May 2022 20:27:27 GMT
RUN apk add --no-cache libssl1.1
# Tue, 24 May 2022 20:27:27 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 24 May 2022 20:27:35 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Tue, 24 May 2022 20:27:36 GMT
VOLUME [/spiped]
# Tue, 24 May 2022 20:27:36 GMT
WORKDIR /spiped
# Tue, 24 May 2022 20:27:37 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 24 May 2022 20:27:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 24 May 2022 20:27:38 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:af1ac1a73384e058591d04d19bc05a06781cc32d52d4593b468d6cb95eda9858`  
		Last Modified: Mon, 23 May 2022 19:43:36 GMT  
		Size: 2.6 MB (2580494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9623718447e29295a23001aae3dbed26ca7b41b14965f02c9ae5324963330ef0`  
		Last Modified: Tue, 24 May 2022 20:28:11 GMT  
		Size: 1.3 KB (1267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74a000d8db4a14acf7833a4d32f3d85f452d72236f3a96360d4518ee2abba268`  
		Last Modified: Tue, 24 May 2022 20:28:11 GMT  
		Size: 7.7 KB (7722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4024830388cfd5531b6e2ca6468204a9d4fb81958bad00a9f8694fcea02a1d0`  
		Last Modified: Tue, 24 May 2022 20:28:11 GMT  
		Size: 202.0 KB (202015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f77170c060013a5bc5e10927cde6e8c315bd601aab054eb5717725f98bb2b0c`  
		Last Modified: Tue, 24 May 2022 20:28:11 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6dcb80a5752c8255af9b16d7c0d66266c0e5ecfec63891ebdb6c7a2d47ff7c71`  
		Last Modified: Tue, 24 May 2022 20:28:11 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:alpine`

```console
$ docker pull spiped@sha256:574b58f2dcd9c3904a6435230c713766d0690f6282db43000ca61e233d59d401
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
$ docker pull spiped@sha256:bdd3a85420e8c8d55b154c7d7f1a043ca1bbae32a53dceaca4838f70ff3376b9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (3022980 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6c7e9665581a5ef894060d275062ab85a542c8fa4a4aae78d4f2617be109e728`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Mon, 23 May 2022 19:19:30 GMT
ADD file:8e81116368669ed3dd361bc898d61bff249f524139a239fdaf3ec46869a39921 in / 
# Mon, 23 May 2022 19:19:31 GMT
CMD ["/bin/sh"]
# Tue, 24 May 2022 19:34:44 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Tue, 24 May 2022 19:34:45 GMT
RUN apk add --no-cache libssl1.1
# Tue, 24 May 2022 19:34:45 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 24 May 2022 19:34:55 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Tue, 24 May 2022 19:34:55 GMT
VOLUME [/spiped]
# Tue, 24 May 2022 19:34:55 GMT
WORKDIR /spiped
# Tue, 24 May 2022 19:34:56 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 24 May 2022 19:34:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 24 May 2022 19:34:56 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:2408cc74d12b6cd092bb8b516ba7d5e290f485d3eb9672efc00f0583730179e8`  
		Last Modified: Mon, 23 May 2022 19:09:38 GMT  
		Size: 2.8 MB (2798889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:becf26afb9051910736e73bcdbfc94bfb72d60a534521c9d4d8bd49f058953ca`  
		Last Modified: Tue, 24 May 2022 19:35:11 GMT  
		Size: 1.3 KB (1271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:744686996785b12019a749f4c09b2b5d59b293aca28e90b0a63b3b6683296350`  
		Last Modified: Tue, 24 May 2022 19:35:11 GMT  
		Size: 7.7 KB (7731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fdf476035643e2d6746fa2acf3e72b7d990dfbf92675e53c57fc5eff30f88ca`  
		Last Modified: Tue, 24 May 2022 19:35:11 GMT  
		Size: 214.6 KB (214618 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a5688549417be3b134e241c450a08175acf2c8cd842b2e30f3310f6a58314a6`  
		Last Modified: Tue, 24 May 2022 19:35:11 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0acff87013e49fae028cf81385e161bc4f11ec1173a9799808132863c6bfa34`  
		Last Modified: Tue, 24 May 2022 19:35:11 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; arm variant v6

```console
$ docker pull spiped@sha256:406809ea0a81e5db518b787d7612be34a70855479615ff4cace100dc08c1ce5d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 MB (2814958 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:765f7c1b3fd5477fdd79037421a66d16f15550314f4344b2e7f359d1ab9f5a6b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Mon, 23 May 2022 19:49:32 GMT
ADD file:f7cee617575b5e5a7672d298a519bb8d8b5098efb90aa2a5d7b0510003457d52 in / 
# Mon, 23 May 2022 19:49:33 GMT
CMD ["/bin/sh"]
# Tue, 24 May 2022 20:14:54 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Tue, 24 May 2022 20:14:56 GMT
RUN apk add --no-cache libssl1.1
# Tue, 24 May 2022 20:14:57 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 24 May 2022 20:15:17 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Tue, 24 May 2022 20:15:18 GMT
VOLUME [/spiped]
# Tue, 24 May 2022 20:15:18 GMT
WORKDIR /spiped
# Tue, 24 May 2022 20:15:19 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 24 May 2022 20:15:19 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 24 May 2022 20:15:20 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:79a25ccaf940855872635c06e7614d9b27dd38ffb5a8adfdb9274dfdc0ea0d87`  
		Last Modified: Mon, 23 May 2022 19:08:47 GMT  
		Size: 2.6 MB (2606142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0a7e07c35741a1549360e780bc005cf673a71e419a28d8a6b9c13991457fd00`  
		Last Modified: Tue, 24 May 2022 20:15:52 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cdf6aebe85933f39c72c58c99c4ec7d111a159f1235bfe85319b66d6203ef8a`  
		Last Modified: Tue, 24 May 2022 20:15:52 GMT  
		Size: 7.7 KB (7726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c66c128b4f04df47fadf6a72f2ba745ba461f8a90f759782eca976719289bfa`  
		Last Modified: Tue, 24 May 2022 20:15:52 GMT  
		Size: 199.3 KB (199349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cff01690378c3c28fddd84bf4b93277c045d39f051cf3b935d00174aa4f2eb45`  
		Last Modified: Tue, 24 May 2022 20:15:52 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fab83e2c93a7364c569439bdd1bcb23f85d4b7900ff40e1cb25bece561c431a`  
		Last Modified: Tue, 24 May 2022 20:15:52 GMT  
		Size: 344.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; arm variant v7

```console
$ docker pull spiped@sha256:acc8ca060038077aa20644d95dfd50f3a9faa59990d2318895033343f94456eb
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 MB (2614203 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:afa4570c887e85e41ae28860d1797be642647270341c2b31a2d07268170d3d18`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Mon, 23 May 2022 18:57:46 GMT
ADD file:72698cc08524b911ebaacf992490707e5a951ddd2fe6edb3fb598e9dc7155049 in / 
# Mon, 23 May 2022 18:57:47 GMT
CMD ["/bin/sh"]
# Tue, 24 May 2022 23:57:01 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Tue, 24 May 2022 23:57:03 GMT
RUN apk add --no-cache libssl1.1
# Tue, 24 May 2022 23:57:03 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 24 May 2022 23:57:23 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Tue, 24 May 2022 23:57:24 GMT
VOLUME [/spiped]
# Tue, 24 May 2022 23:57:24 GMT
WORKDIR /spiped
# Tue, 24 May 2022 23:57:25 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 24 May 2022 23:57:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 24 May 2022 23:57:26 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:6366ba92f08e2418e90171f1e34bd86ecd50fdc95953b3f33b8943c143518eca`  
		Last Modified: Mon, 23 May 2022 18:59:17 GMT  
		Size: 2.4 MB (2411648 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:744a106e187f9790be6dbdde860ada60aab7e95bae779540c813da16ce184ea7`  
		Last Modified: Tue, 24 May 2022 23:58:19 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e8f51295340b65e165fffa3de719118e625ca751a7c465a96dee14a0441de72`  
		Last Modified: Tue, 24 May 2022 23:58:19 GMT  
		Size: 7.7 KB (7717 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a1da9fdb3c39499af6413db4aeed00e8577a949c49968ffd86c20f438118a88`  
		Last Modified: Tue, 24 May 2022 23:58:19 GMT  
		Size: 193.1 KB (193098 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83b416966b1e14463ce73c56ecba5fd804f4c565b4d781199f3b02247ffdf8e7`  
		Last Modified: Tue, 24 May 2022 23:58:19 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f1016107cea29ba85ecc25a6bba5c5c3494ef9ed31194cc5e7b6ea8add7ef4a`  
		Last Modified: Tue, 24 May 2022 23:58:19 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:bdfcd3d661a8017ef3286486269e41c2ab4d2c4662672ea7e21ac01a7e8572c8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 MB (2911518 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:12a66ddef290c67283604068f9b4d679bc4dd400e2bdf0d2826b55e9bdf23aeb`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Mon, 23 May 2022 19:39:22 GMT
ADD file:3ae36c6c4a1fc43157692da97c6c4fa6c3d0189ba82e2bef7f5aaf4a5e083f18 in / 
# Mon, 23 May 2022 19:39:22 GMT
CMD ["/bin/sh"]
# Tue, 24 May 2022 20:25:00 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Tue, 24 May 2022 20:25:02 GMT
RUN apk add --no-cache libssl1.1
# Tue, 24 May 2022 20:25:03 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 24 May 2022 20:25:22 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Tue, 24 May 2022 20:25:23 GMT
VOLUME [/spiped]
# Tue, 24 May 2022 20:25:24 GMT
WORKDIR /spiped
# Tue, 24 May 2022 20:25:26 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 24 May 2022 20:25:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 24 May 2022 20:25:27 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:b3c136eddcbf2003d3180787cef00f39d46b9fd9e4623178282ad6a8d63ad3b0`  
		Last Modified: Mon, 23 May 2022 19:08:34 GMT  
		Size: 2.7 MB (2694464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20a86dbffa956db3e6a8cd773330f1ec06aa87e6987f0f5c9a031e2af7975a9a`  
		Last Modified: Tue, 24 May 2022 20:25:57 GMT  
		Size: 1.2 KB (1244 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:168f9b4c4b922cf44b915dedb800de4176f18b715d6a917a6576a2d24ba0b78a`  
		Last Modified: Tue, 24 May 2022 20:25:57 GMT  
		Size: 7.7 KB (7705 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba2ce83ec0aa17bde883cf7689464f8502798d298fd4296e17e51c9ab614ebd6`  
		Last Modified: Tue, 24 May 2022 20:25:57 GMT  
		Size: 207.7 KB (207671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7796ce5b43cb7f8557eb86d1bb3682848bca4769f1886634356d8952e37e262`  
		Last Modified: Tue, 24 May 2022 20:25:57 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c60cf321cf0b839869c31f5a9ac3374f3c43dba87ab4d0794c93d1436b27e37d`  
		Last Modified: Tue, 24 May 2022 20:25:56 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; 386

```console
$ docker pull spiped@sha256:6eb9e3e76d959724427cca66e52c7bdeebb58c9297c5fd7d60b50838669fe7ef
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (3036399 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b0215089b25dc2844d60ff524e3c7359fc6094c7376d2646e5482fa918c91bad`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Mon, 23 May 2022 19:38:20 GMT
ADD file:1750ccfabfe93636015070d51a6e824cbd738056223421c69d8aaabc38041b18 in / 
# Mon, 23 May 2022 19:38:20 GMT
CMD ["/bin/sh"]
# Tue, 24 May 2022 20:13:25 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Tue, 24 May 2022 20:13:26 GMT
RUN apk add --no-cache libssl1.1
# Tue, 24 May 2022 20:13:27 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 24 May 2022 20:13:38 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Tue, 24 May 2022 20:13:39 GMT
VOLUME [/spiped]
# Tue, 24 May 2022 20:13:40 GMT
WORKDIR /spiped
# Tue, 24 May 2022 20:13:42 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 24 May 2022 20:13:42 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 24 May 2022 20:13:43 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:bb638a3869eed698f88775c7a48f36f8e22e7c6bbaa98fa1d5678966b619b859`  
		Last Modified: Mon, 23 May 2022 19:09:25 GMT  
		Size: 2.8 MB (2801887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:538c30644db57c76ff9a69c435c96a6d269cf8da91c4d632beffff39511588ca`  
		Last Modified: Tue, 24 May 2022 20:14:13 GMT  
		Size: 1.2 KB (1241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d193ad41299c95702ee3dcff9a3399e567cc04c5e640af6cc098795b475843fe`  
		Last Modified: Tue, 24 May 2022 20:14:12 GMT  
		Size: 7.7 KB (7697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec3ef77db5428642bb00b1436a0a844fca99ef4cc676e787f6307ac237f4f65d`  
		Last Modified: Tue, 24 May 2022 20:14:13 GMT  
		Size: 225.1 KB (225139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce435cec46d2206fbfa56e9dc4c9a2907fcd4bdba6acb8c4f332a2f1246e1a8c`  
		Last Modified: Tue, 24 May 2022 20:14:13 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ab3029834f1c60801bbb7cb77e5fec645e494281b466eaed4fb5c5ed38f4b26`  
		Last Modified: Tue, 24 May 2022 20:14:12 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; ppc64le

```console
$ docker pull spiped@sha256:394770c1c3e52c18b2e060896dc946a7de8c0581c1691fe3a2458c6442d51071
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (3012900 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:45dd65bd18433f8227345eb1bc628c92fb777cc4d5e9e790835ba272eaadec4e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Mon, 23 May 2022 19:16:51 GMT
ADD file:6a5450c8a7cee3ceda59e7cb350c54df4139b0f7b7cf49c8b31bb9c01646c3cd in / 
# Mon, 23 May 2022 19:16:53 GMT
CMD ["/bin/sh"]
# Tue, 24 May 2022 19:50:10 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Tue, 24 May 2022 19:50:18 GMT
RUN apk add --no-cache libssl1.1
# Tue, 24 May 2022 19:50:20 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 24 May 2022 19:50:38 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Tue, 24 May 2022 19:50:42 GMT
VOLUME [/spiped]
# Tue, 24 May 2022 19:50:47 GMT
WORKDIR /spiped
# Tue, 24 May 2022 19:50:48 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 24 May 2022 19:50:52 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 24 May 2022 19:50:56 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:d3deabf2a506ef6f5fa7c2a68bf27047574cef9908b30a97ff2d01ae539b089a`  
		Last Modified: Mon, 23 May 2022 19:09:13 GMT  
		Size: 2.8 MB (2789745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6d245add1998dabc480629fde1ae678cfbb96f740737e4acede363c37eda348`  
		Last Modified: Tue, 24 May 2022 19:51:36 GMT  
		Size: 1.3 KB (1272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bea94be815996b73043903da4f60b4ea3573e9689c5b3b1b0348ef5ef54fe25b`  
		Last Modified: Tue, 24 May 2022 19:51:36 GMT  
		Size: 7.7 KB (7727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b25cc9d25fe567c300c07c50cb1d341544a9751b92d44874cef5399d1beee0aa`  
		Last Modified: Tue, 24 May 2022 19:51:36 GMT  
		Size: 213.7 KB (213687 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2b003e2ac252266dcd49f568ddc62ed5a04668bc0655e7cd74521a21c0089eb`  
		Last Modified: Tue, 24 May 2022 19:51:36 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fed434cd18f8048c2624c1d26c27721d4ce3e46b39d5d9adcbeec4733e3954ff`  
		Last Modified: Tue, 24 May 2022 19:51:36 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; s390x

```console
$ docker pull spiped@sha256:4c56dd9796353102785f0a5f8f38e81e0638a1ca2b745795770b8e137ebc657d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 MB (2791966 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a3497d9a69b26f419f935637e370f6a57f1d4e5ad7000970a7ecdcbf0333263c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Mon, 23 May 2022 19:41:59 GMT
ADD file:e1852d8ef555a0d3ef6d0b74a898720c82bb9f491430b06a0dd0499497ce118e in / 
# Mon, 23 May 2022 19:42:10 GMT
CMD ["/bin/sh"]
# Tue, 24 May 2022 20:27:25 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Tue, 24 May 2022 20:27:27 GMT
RUN apk add --no-cache libssl1.1
# Tue, 24 May 2022 20:27:27 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 24 May 2022 20:27:35 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Tue, 24 May 2022 20:27:36 GMT
VOLUME [/spiped]
# Tue, 24 May 2022 20:27:36 GMT
WORKDIR /spiped
# Tue, 24 May 2022 20:27:37 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 24 May 2022 20:27:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 24 May 2022 20:27:38 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:af1ac1a73384e058591d04d19bc05a06781cc32d52d4593b468d6cb95eda9858`  
		Last Modified: Mon, 23 May 2022 19:43:36 GMT  
		Size: 2.6 MB (2580494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9623718447e29295a23001aae3dbed26ca7b41b14965f02c9ae5324963330ef0`  
		Last Modified: Tue, 24 May 2022 20:28:11 GMT  
		Size: 1.3 KB (1267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74a000d8db4a14acf7833a4d32f3d85f452d72236f3a96360d4518ee2abba268`  
		Last Modified: Tue, 24 May 2022 20:28:11 GMT  
		Size: 7.7 KB (7722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4024830388cfd5531b6e2ca6468204a9d4fb81958bad00a9f8694fcea02a1d0`  
		Last Modified: Tue, 24 May 2022 20:28:11 GMT  
		Size: 202.0 KB (202015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f77170c060013a5bc5e10927cde6e8c315bd601aab054eb5717725f98bb2b0c`  
		Last Modified: Tue, 24 May 2022 20:28:11 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6dcb80a5752c8255af9b16d7c0d66266c0e5ecfec63891ebdb6c7a2d47ff7c71`  
		Last Modified: Tue, 24 May 2022 20:28:11 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:latest`

```console
$ docker pull spiped@sha256:2a04458cf6cb5fa31173ddeeaec6840207e46a3186dbb1e1de6b3c83a009c5d0
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
$ docker pull spiped@sha256:b2ff44d1d923f53540c90249f0186c6bcc7dccb99603a5bcb501d4aa81fda546
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.3 MB (37349979 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5823c93a49f14efb19ac802a6042b74cb55529fbfcce6ab550db72f9b6a7dd30`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 23 Jun 2022 00:20:27 GMT
ADD file:8adbbab04d6f84cd83b5f4205b89b0acb7ecbf27a1bb2dc181d0a629479039fe in / 
# Thu, 23 Jun 2022 00:20:27 GMT
CMD ["bash"]
# Thu, 23 Jun 2022 14:24:59 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Thu, 23 Jun 2022 14:25:02 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Thu, 23 Jun 2022 14:25:02 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 23 Jun 2022 14:25:21 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 23 Jun 2022 14:25:21 GMT
VOLUME [/spiped]
# Thu, 23 Jun 2022 14:25:22 GMT
WORKDIR /spiped
# Thu, 23 Jun 2022 14:25:22 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 23 Jun 2022 14:25:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Jun 2022 14:25:22 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:b85a868b505ffd0342a37e6a3b1c49f7c71878afe569a807e6238ef08252fcb7`  
		Last Modified: Thu, 23 Jun 2022 00:25:18 GMT  
		Size: 31.4 MB (31379408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55454b6a8916eece033c9dfe8babcaa0cd04c0901055b9040e2eac12cbb05f97`  
		Last Modified: Thu, 23 Jun 2022 14:25:40 GMT  
		Size: 1.7 KB (1733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dad7666375bb50bbfccbc5bad922741a65570699f108894f77601d31d4b76fba`  
		Last Modified: Thu, 23 Jun 2022 14:25:40 GMT  
		Size: 1.1 KB (1052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43a0a6b62b5421f4c74facfba698b0434d6899e1c77c61fefc4f28e7a0ab10d1`  
		Last Modified: Thu, 23 Jun 2022 14:25:41 GMT  
		Size: 6.0 MB (5967315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:756782629170475511f5a3ee4cb4717e152d25e3993ecc99aa0772dd2a518179`  
		Last Modified: Thu, 23 Jun 2022 14:25:40 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:331a176397a9e42d10ecaaae616afffdfffaef1527eb16f81d10ae9141ba19cf`  
		Last Modified: Thu, 23 Jun 2022 14:25:40 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; arm variant v5

```console
$ docker pull spiped@sha256:feec4c6defea9575b6b723a20ac0d667a6a0b7c896a4553cd8950674899f1d6f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.0 MB (33952417 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:609536328e039bda4f2dd352cefca6776a998bd2debfa65c39928aa2052752d3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Sat, 28 May 2022 02:03:06 GMT
ADD file:d9560b279f64bc3973a6aaa0e0ab8f483d60a1c66647899850689eee01a729ec in / 
# Sat, 28 May 2022 02:03:07 GMT
CMD ["bash"]
# Sat, 28 May 2022 19:53:26 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Sat, 28 May 2022 19:53:35 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 19:53:35 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Sat, 28 May 2022 19:54:26 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Sat, 28 May 2022 19:54:27 GMT
VOLUME [/spiped]
# Sat, 28 May 2022 19:54:27 GMT
WORKDIR /spiped
# Sat, 28 May 2022 19:54:28 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 28 May 2022 19:54:28 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 28 May 2022 19:54:29 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:b24540c95c3d5b61dba94dfa3665e0cc1231b3602edfb61432041c1f108be50d`  
		Last Modified: Sat, 28 May 2022 02:18:37 GMT  
		Size: 28.9 MB (28921471 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aea4df7367cff72ae8d9118ef5266476e59c66462928466d605c1d9623180448`  
		Last Modified: Sat, 28 May 2022 19:55:02 GMT  
		Size: 1.7 KB (1727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:246aeb209300265ffd136d8ef9420bc206bd86aec58047847f3aa4e50cf3c3eb`  
		Last Modified: Sat, 28 May 2022 19:55:02 GMT  
		Size: 1.1 KB (1054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bf79bde433a8bd87a705f9a94a90ee36cc3fcc94f66f88444fe45670af95100`  
		Last Modified: Sat, 28 May 2022 19:55:07 GMT  
		Size: 5.0 MB (5027692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9733b89df15002a08795a040cdad7e97743b49f08303f89ae9d1a578f43d4782`  
		Last Modified: Sat, 28 May 2022 19:55:02 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dce9b97ee80126486958e7e92f4caa4888c8367d20d8d39bec8c62797aee6cfd`  
		Last Modified: Sat, 28 May 2022 19:55:02 GMT  
		Size: 344.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; arm variant v7

```console
$ docker pull spiped@sha256:27ceab9292afad9550739501c64b6f5cc11c3dbe3b65f93bcc390c4120433c51
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.3 MB (31327718 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:22929e8964c6549f3d8123da06f309aa6f679e4714692df4bfa197d0e2c8f399`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Sat, 28 May 2022 00:59:48 GMT
ADD file:975c801b5b50aa75e07d18e69af11f21e165561abc16246e2c413c2ef96ce4c6 in / 
# Sat, 28 May 2022 00:59:49 GMT
CMD ["bash"]
# Sun, 29 May 2022 06:25:09 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Sun, 29 May 2022 06:25:16 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Sun, 29 May 2022 06:25:16 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Sun, 29 May 2022 06:26:02 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Sun, 29 May 2022 06:26:03 GMT
VOLUME [/spiped]
# Sun, 29 May 2022 06:26:03 GMT
WORKDIR /spiped
# Sun, 29 May 2022 06:26:04 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sun, 29 May 2022 06:26:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sun, 29 May 2022 06:26:05 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:eeb117569618df53320eb28d32b7a1d87792bda3362017123fa1025b55db44c3`  
		Last Modified: Sat, 28 May 2022 01:15:35 GMT  
		Size: 26.6 MB (26576237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f673a628d46f411f6fa471dacc6a7f093320a9060f586c46fd61466e55c0e684`  
		Last Modified: Sun, 29 May 2022 06:27:04 GMT  
		Size: 1.7 KB (1726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b972855b62da685c2bb09ca3ed5808bfc51cd9b062ad73b9ba2a0ac8497e321`  
		Last Modified: Sun, 29 May 2022 06:27:04 GMT  
		Size: 1.1 KB (1054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abf09d9445796b62d51bb11fe3f1236c17a50784d5fb850e1b26d4bcc677b3b2`  
		Last Modified: Sun, 29 May 2022 06:27:08 GMT  
		Size: 4.7 MB (4748232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:988142d33ab11d2901370155c8b902ad639de76fd48866e961b307372b37cee8`  
		Last Modified: Sun, 29 May 2022 06:27:04 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b5ba53ff286b0137dddc9613a5e23aacaa1cf035b46b78799a9dcba485d0c63`  
		Last Modified: Sun, 29 May 2022 06:27:04 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:50b5813789a1de2455e1602e814b1ba46c2f92226a13ce8acb0a33e3bb237ef8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.3 MB (35339663 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:79448de18bfa13cb33bf4a88178cbea587a26f574f5db947d339d48f822e6be8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 23 Jun 2022 00:40:43 GMT
ADD file:134be48af13f80f3474bf1b080ca781feb7b972148d482849862e55eb2acd61c in / 
# Thu, 23 Jun 2022 00:40:44 GMT
CMD ["bash"]
# Thu, 23 Jun 2022 14:19:37 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Thu, 23 Jun 2022 14:19:40 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Thu, 23 Jun 2022 14:19:41 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 23 Jun 2022 14:19:59 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 23 Jun 2022 14:19:59 GMT
VOLUME [/spiped]
# Thu, 23 Jun 2022 14:20:00 GMT
WORKDIR /spiped
# Thu, 23 Jun 2022 14:20:02 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 23 Jun 2022 14:20:02 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Jun 2022 14:20:03 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:3b157c852f2736e12f09046f214fe5f6a0b1652bd860269b3988c92a197026e8`  
		Last Modified: Thu, 23 Jun 2022 00:47:22 GMT  
		Size: 30.1 MB (30065720 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d2b50ae5c80cf61302029794b9bb8788bc1c4340583fe19b3886a328bd2e59c`  
		Last Modified: Thu, 23 Jun 2022 14:20:30 GMT  
		Size: 1.6 KB (1618 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3f8033bf687e78771c0955fb5ad0dbd87fe3ecbadc7779f0fbff1ddaed4a38b`  
		Last Modified: Thu, 23 Jun 2022 14:20:30 GMT  
		Size: 925.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90442e6da9e0bf71d16d1004502b61ac0ee04335adeb4ea1c0f5322793923308`  
		Last Modified: Thu, 23 Jun 2022 14:20:31 GMT  
		Size: 5.3 MB (5270963 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c1a82ee02be4fd41ba26092fcccc4a7ef039055a227e0d7f92ad587546071ad`  
		Last Modified: Thu, 23 Jun 2022 14:20:30 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad041befbc894c998e7065d943ec5a35b70eaf5024d5e19fa6192a489202122a`  
		Last Modified: Thu, 23 Jun 2022 14:20:30 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; 386

```console
$ docker pull spiped@sha256:0418180e629bf6c4c671ceb932c0bb7d8cc2245cd53ad80a3f9ff42a289131bf
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.3 MB (40284635 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f33d96114c1233c804814373fd9cd85fb08296fa76ac20445c2fe9d2fa0ac225`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 23 Jun 2022 00:39:33 GMT
ADD file:9d46d3f8fb63833a6dbd8dd796ad541d556046a48342d22e1fd3bffa3fb8e504 in / 
# Thu, 23 Jun 2022 00:39:33 GMT
CMD ["bash"]
# Thu, 23 Jun 2022 15:04:24 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Thu, 23 Jun 2022 15:04:28 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Thu, 23 Jun 2022 15:04:29 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 23 Jun 2022 15:04:49 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 23 Jun 2022 15:04:50 GMT
VOLUME [/spiped]
# Thu, 23 Jun 2022 15:04:51 GMT
WORKDIR /spiped
# Thu, 23 Jun 2022 15:04:53 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 23 Jun 2022 15:04:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Jun 2022 15:04:54 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:4870b12e407743816673c11cfb39974d80c1569d876287bef61f8c585954822f`  
		Last Modified: Thu, 23 Jun 2022 00:46:40 GMT  
		Size: 32.4 MB (32390198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:886cea7325b13f7203d5e830883ba71c98d83a0686704a1b6982442fd97d827c`  
		Last Modified: Thu, 23 Jun 2022 15:05:25 GMT  
		Size: 1.6 KB (1610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6a0a4b187e0c9f93860637c1c720af4b8e8cf1d089783dfbf0a07ba662fac22`  
		Last Modified: Thu, 23 Jun 2022 15:05:25 GMT  
		Size: 925.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bb9eaa94baa3de99a61cef041ce22494d7ffdbbbdabc1ea1629f4bb0d977bdd`  
		Last Modified: Thu, 23 Jun 2022 15:05:27 GMT  
		Size: 7.9 MB (7891464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3560d550fd7c038f01cf33f88495c9761131e2304f6d1f17a85e272656dd82ff`  
		Last Modified: Thu, 23 Jun 2022 15:05:25 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:776c52a49bfdec3ad5665559540af9ec46f9eced7d9aa5d664aaa96582d28fb4`  
		Last Modified: Thu, 23 Jun 2022 15:05:25 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; mips64le

```console
$ docker pull spiped@sha256:327ab349035e42e2520c87903f12e1e4b8aa2b46f5af20028c6148d435015ac6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.3 MB (35349399 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:134640be221db73739d4c6d145ed454eb1f6b7c530d7b5a037f8566a5c50d315`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Sat, 28 May 2022 01:11:13 GMT
ADD file:f685a156b7ddafe7bafc6fad17cc36cc8a5d6d922fc1c425656ca92266d9a98e in / 
# Sat, 28 May 2022 01:11:18 GMT
CMD ["bash"]
# Sat, 28 May 2022 11:02:07 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Sat, 28 May 2022 11:02:24 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 11:02:26 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Sat, 28 May 2022 11:03:57 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Sat, 28 May 2022 11:04:00 GMT
VOLUME [/spiped]
# Sat, 28 May 2022 11:04:03 GMT
WORKDIR /spiped
# Sat, 28 May 2022 11:04:06 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 28 May 2022 11:04:08 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 28 May 2022 11:04:11 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:fdea7139ce36b557a23c4b9c4255387b175f851ed0c51e1e7d78dd301c0e4da8`  
		Last Modified: Sat, 28 May 2022 01:21:35 GMT  
		Size: 29.6 MB (29641237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:638fcc9a2aca909e0ddad028b40a02f45370c5c4864972531afa7a02e7d5f8b5`  
		Last Modified: Sat, 28 May 2022 11:04:37 GMT  
		Size: 1.6 KB (1620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62732d2f48eb3a503a80f0fcc97263b3feb49c39cfec9026b62d02698d569084`  
		Last Modified: Sat, 28 May 2022 11:04:37 GMT  
		Size: 925.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec6d02d49d5fc774a71ed9e0211b9250e5926d8a45f48011929bc45eea21a764`  
		Last Modified: Sat, 28 May 2022 11:04:43 GMT  
		Size: 5.7 MB (5705180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:551ee4c909a9bed061c23e73af4c6586e9b6144160f20081c7c31a2e78d21357`  
		Last Modified: Sat, 28 May 2022 11:04:37 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8231a7adeed86962f2691999debe4256643805fd3dd1b4deb1e8e6d30fbd2e2`  
		Last Modified: Sat, 28 May 2022 11:04:37 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; ppc64le

```console
$ docker pull spiped@sha256:b6377c503b8d6a42b6db7ff3590aca7406bbb9fb1550d8baaf89f61ee4e6f222
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.3 MB (41289157 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ed59345839d9409f475ce2fce73fb95e4ba9c41a970711589fb2014d87459aa9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Sat, 28 May 2022 01:22:54 GMT
ADD file:64e264b12eed99d87380e38f36bfecd62b9bb1e5460f0242cfbc5dc76c212ead in / 
# Sat, 28 May 2022 01:22:59 GMT
CMD ["bash"]
# Sat, 28 May 2022 20:47:31 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Sat, 28 May 2022 20:47:49 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 20:48:09 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Sat, 28 May 2022 20:50:59 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Sat, 28 May 2022 20:51:04 GMT
VOLUME [/spiped]
# Sat, 28 May 2022 20:51:09 GMT
WORKDIR /spiped
# Sat, 28 May 2022 20:51:31 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 28 May 2022 20:51:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 28 May 2022 20:52:04 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:893e245a8f6219935016f2dd4422ec4b7fdab43d98ba29c024ec0d9ce57794ba`  
		Last Modified: Sat, 28 May 2022 01:32:28 GMT  
		Size: 35.3 MB (35286698 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:922a5f50c37cc3b0d1fef17e00862a91bd28f367cd75a7ad0414852ec8d6809e`  
		Last Modified: Sat, 28 May 2022 20:52:46 GMT  
		Size: 1.7 KB (1737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59b8faf9aaa0e83c1e60be75a9512012bfbe307b7facc7fc65656db5f3f4c3ff`  
		Last Modified: Sat, 28 May 2022 20:52:46 GMT  
		Size: 1.1 KB (1056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7583ca3e72d7ba19d9282d7cceb754c6b78dcc5dafe87fb40ba11abcdfad841b`  
		Last Modified: Sat, 28 May 2022 20:52:47 GMT  
		Size: 6.0 MB (5999195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3c570e58336fa60b88539aef4e1ffa0289798f70a906a55c0b291cf386d76c2`  
		Last Modified: Sat, 28 May 2022 20:52:46 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9a0eb6589f42f53d4c16113fbeee7f38fff9157291e8c9b22be42ce45653820`  
		Last Modified: Sat, 28 May 2022 20:52:46 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; s390x

```console
$ docker pull spiped@sha256:a9442b276bfaee2a75715fe608363309aca4373dc2dc502604bb2bb0d5f4dea8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.8 MB (34845447 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2941968d748f4b2e9298f5f6ecd1c8ef8a6e9fc6074a6649a7b6ea6f03eff523`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 23 Jun 2022 00:43:10 GMT
ADD file:0b511e3efd87267fb27161eae56c4d08f0fed733697da6ffe6ea96a4cb68e938 in / 
# Thu, 23 Jun 2022 00:43:15 GMT
CMD ["bash"]
# Thu, 23 Jun 2022 13:40:29 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Thu, 23 Jun 2022 13:40:31 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Thu, 23 Jun 2022 13:40:32 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 23 Jun 2022 13:40:43 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 23 Jun 2022 13:40:44 GMT
VOLUME [/spiped]
# Thu, 23 Jun 2022 13:40:44 GMT
WORKDIR /spiped
# Thu, 23 Jun 2022 13:40:44 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 23 Jun 2022 13:40:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Jun 2022 13:40:44 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:c547f465e0c8708ad0c57cf09caa52f4c2b5b295bf10ab1ce71ca17ff81ea36a`  
		Last Modified: Thu, 23 Jun 2022 00:51:59 GMT  
		Size: 29.7 MB (29655262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f10418190b72e9fc95fa6f7bd6436f85792a11bac97bf409ebb489733c6cdeb`  
		Last Modified: Thu, 23 Jun 2022 13:41:20 GMT  
		Size: 1.7 KB (1736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d9de83495ba48b01499e858c82e09a1dbed7baa1add5136e5adce6e7d60d452`  
		Last Modified: Thu, 23 Jun 2022 13:41:19 GMT  
		Size: 1.1 KB (1052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1af8046b93a37ad2bb5d08d4a2b031d01e804f6215b67365ba7b72766510a52c`  
		Last Modified: Thu, 23 Jun 2022 13:41:20 GMT  
		Size: 5.2 MB (5186928 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d254cd7b5719c3b1ba5880a1daa9212d49f5999c4c6f371e32d84733730ddcfe`  
		Last Modified: Thu, 23 Jun 2022 13:41:19 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2556f06bac5f4c72f60c12325c5c156dd6d3cc548dbc2d60398e43f72584c19`  
		Last Modified: Thu, 23 Jun 2022 13:41:19 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
