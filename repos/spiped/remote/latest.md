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
