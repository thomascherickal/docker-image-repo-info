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
$ docker pull spiped@sha256:2df475af81759906c3da1ca65516f492123ebdb8bd14ab5dbd99082d8e21e38f
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
$ docker pull spiped@sha256:baa7adbbf67c6427f370b092b71b3e084e6b6f2b1b69d7830826bad32dc6474a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.3 MB (37337248 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ec58bdda4c26deb18400f539b267f1b2d59944078a579281e32030d0fac85c72`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 12 Jul 2022 01:20:10 GMT
ADD file:d978f6d3025a06f5142a0c13c98bf12fbd47cdf9162ed31fbc05c86983b0a679 in / 
# Tue, 12 Jul 2022 01:20:10 GMT
CMD ["bash"]
# Tue, 12 Jul 2022 14:24:08 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 12 Jul 2022 14:24:12 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jul 2022 14:24:12 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 12 Jul 2022 14:24:32 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 12 Jul 2022 14:24:32 GMT
VOLUME [/spiped]
# Tue, 12 Jul 2022 14:24:32 GMT
WORKDIR /spiped
# Tue, 12 Jul 2022 14:24:33 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 12 Jul 2022 14:24:33 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 12 Jul 2022 14:24:33 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:461246efe0a75316d99afdbf348f7063b57b0caeee8daab775f1f08152ea36f4`  
		Last Modified: Tue, 12 Jul 2022 01:24:34 GMT  
		Size: 31.4 MB (31366610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73ffd90cb7ba935b5f839a884b1ed9a58536b59f2da2d55ddbc19013590ac2bb`  
		Last Modified: Tue, 12 Jul 2022 14:24:50 GMT  
		Size: 1.7 KB (1731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:996ee512378210a090efc903c1338cd3ee02e97cd22d95ab5f8ee2418e65ffc4`  
		Last Modified: Tue, 12 Jul 2022 14:24:51 GMT  
		Size: 1.1 KB (1051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28eae5d1f26957502a0e384167f16a5ff3c906bf4c45cb3be57cbe2dde4e6c0f`  
		Last Modified: Tue, 12 Jul 2022 14:24:52 GMT  
		Size: 6.0 MB (5967386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcb594120cd340a1d759860341474d83f98217ae59b8e456504e58405a5c6168`  
		Last Modified: Tue, 12 Jul 2022 14:24:50 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b01900430d194aeac11a8520319b898c4bfb10e0ec043fa2a18ccca55ed39d8b`  
		Last Modified: Tue, 12 Jul 2022 14:24:51 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; arm variant v5

```console
$ docker pull spiped@sha256:da5c36b11149105885a68f9d371f023a53ddb8f039bf4128454a2e40eb570d0c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.9 MB (33936339 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3e4724dc7ea3fa813169dd39cb5ad7f614e01b9f08009359909a91a99521245d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 12 Jul 2022 00:50:38 GMT
ADD file:c11ce95201c98565eb5f40f837837d88c7b16d81d608b6dce953f51c90167b03 in / 
# Tue, 12 Jul 2022 00:50:39 GMT
CMD ["bash"]
# Wed, 13 Jul 2022 03:55:57 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 13 Jul 2022 03:56:07 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 13 Jul 2022 03:56:07 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 13 Jul 2022 03:56:58 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 13 Jul 2022 03:56:58 GMT
VOLUME [/spiped]
# Wed, 13 Jul 2022 03:56:59 GMT
WORKDIR /spiped
# Wed, 13 Jul 2022 03:57:00 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 13 Jul 2022 03:57:00 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 13 Jul 2022 03:57:00 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:f9371f3d7174b9da7d72bb3a49a5a3c5e96d5b106ef3113b25c27d30bb020de9`  
		Last Modified: Tue, 12 Jul 2022 01:03:01 GMT  
		Size: 28.9 MB (28905415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f17733f89592728022be14b12aa535e575d50c3af74c6b4b62ffeeddc543a9b`  
		Last Modified: Wed, 13 Jul 2022 03:57:34 GMT  
		Size: 1.7 KB (1726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c097088c4865734e08ad4830fec93508c0904f69a50143f46f5279682cb86d75`  
		Last Modified: Wed, 13 Jul 2022 03:57:34 GMT  
		Size: 1.0 KB (1049 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f772f929026de6cad41e4a47b51a6637f4d5eabed19b86d781c4c53cc1b251b`  
		Last Modified: Wed, 13 Jul 2022 03:57:39 GMT  
		Size: 5.0 MB (5027678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91ad846449f44ff79e0a2ae39faf88bdd83c752f9f30771988f0d0f56ffaf72a`  
		Last Modified: Wed, 13 Jul 2022 03:57:34 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15d89609ea2873d6e123e1f3296a9699103b5b3cf1e6362b1435ca04c1b04c9e`  
		Last Modified: Wed, 13 Jul 2022 03:57:34 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; arm variant v7

```console
$ docker pull spiped@sha256:8606eb476cb64fde0e9aa39f886d9bd31597a0197cdf07a090bc7881a0bdd8c1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.3 MB (31327684 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6aabe5099ff3912ff7cd11a03c60ba8aa2b298483f82513f7d086cd55a442181`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 23 Jun 2022 00:59:45 GMT
ADD file:925abfb9fc0e4a7cc0c979b12c9bd2607f5c493d37b05535ca010f81beb060a9 in / 
# Thu, 23 Jun 2022 00:59:46 GMT
CMD ["bash"]
# Thu, 23 Jun 2022 21:30:10 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Thu, 23 Jun 2022 21:30:18 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Thu, 23 Jun 2022 21:30:18 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 23 Jun 2022 21:31:06 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 23 Jun 2022 21:31:07 GMT
VOLUME [/spiped]
# Thu, 23 Jun 2022 21:31:08 GMT
WORKDIR /spiped
# Thu, 23 Jun 2022 21:31:08 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 23 Jun 2022 21:31:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Jun 2022 21:31:09 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:d2fd562560d8062a78064adfbfa204521167c301f00f5ab3c65b9c2a54083dba`  
		Last Modified: Thu, 23 Jun 2022 01:15:22 GMT  
		Size: 26.6 MB (26576105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99432086fbbe1dcdd9be0ab7f0395f40cfb463377a77ce42991d7938e5f97f4c`  
		Last Modified: Thu, 23 Jun 2022 21:32:07 GMT  
		Size: 1.7 KB (1728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f42f8e77af251ad3785548e41f782a72d1741d7a2a81d5ac4211cedfc6fd1322`  
		Last Modified: Thu, 23 Jun 2022 21:32:08 GMT  
		Size: 1.0 KB (1048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bdfcd7452d405dbbd5f03f66e9575a068f1e051c476a4d6ca7a9de6e3488a7b`  
		Last Modified: Thu, 23 Jun 2022 21:32:12 GMT  
		Size: 4.7 MB (4748331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91a24918704d53ee97e582f9cda126c8ae9faee7fea7f9a641174a290aa77352`  
		Last Modified: Thu, 23 Jun 2022 21:32:07 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0907fd39763b46ef91c12e8200fc7e8f4058a375ff39d8038aeffd79a4658d9f`  
		Last Modified: Thu, 23 Jun 2022 21:32:07 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:d7fc07e0161591d29e9c32ac511cad353265235e4e7c6e934471100bb8550cae
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.3 MB (35328185 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1cb54f7071b7db52f99ebd71b070c0129825389d5aab5ccb3d0cc2aefead6566`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 12 Jul 2022 00:40:34 GMT
ADD file:f3a33075f4c3324c6a634ef37a1965ddd5606b4449c0f5909ce18eeb8268b612 in / 
# Tue, 12 Jul 2022 00:40:35 GMT
CMD ["bash"]
# Tue, 12 Jul 2022 13:19:40 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 12 Jul 2022 13:19:43 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jul 2022 13:19:44 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 12 Jul 2022 13:20:02 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 12 Jul 2022 13:20:03 GMT
VOLUME [/spiped]
# Tue, 12 Jul 2022 13:20:04 GMT
WORKDIR /spiped
# Tue, 12 Jul 2022 13:20:06 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 12 Jul 2022 13:20:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 12 Jul 2022 13:20:07 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:60197a4c18d4b386d371cf39d01c48e98c357bba06da0b070a3c1f75006fd838`  
		Last Modified: Tue, 12 Jul 2022 00:46:13 GMT  
		Size: 30.1 MB (30054226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a089893717292b09eece50f192b80ac5ff6ff00637913777ba5c2df7ea8313a`  
		Last Modified: Tue, 12 Jul 2022 13:20:38 GMT  
		Size: 1.6 KB (1614 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f83311e0bf4416e1545ca652c599935e87c6b49e2b56f4bf7fa507de53cd0f17`  
		Last Modified: Tue, 12 Jul 2022 13:20:38 GMT  
		Size: 921.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efed5fb9a9bdee51f1f2c28ed64516d3ec10c256aa210403727ae6ff9d84a4ee`  
		Last Modified: Tue, 12 Jul 2022 13:20:39 GMT  
		Size: 5.3 MB (5270986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b74d6a8a5fa581a44b7d8e4e36dacdda29cee05dd3c17b98e55ff5ae56148c3a`  
		Last Modified: Tue, 12 Jul 2022 13:20:38 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a598427601e24498db86a01b1652d4cc3bb8862e1ebbdd06f38bf30347cd172a`  
		Last Modified: Tue, 12 Jul 2022 13:20:38 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; 386

```console
$ docker pull spiped@sha256:1fd21a5b9b47d2e84a4f398b21be00c2357ac211b9a7435ea05ce93ae14683c5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.3 MB (40268498 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1b4bdb79b659b9bd62a3954d3fcf8119356992184a3b5310ab501f92b829a8a3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 12 Jul 2022 00:39:27 GMT
ADD file:7f2bf44013d7848f051407d854b68c0d415a5328a3f5d241fca3150ce23bde65 in / 
# Tue, 12 Jul 2022 00:39:27 GMT
CMD ["bash"]
# Tue, 12 Jul 2022 10:11:10 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 12 Jul 2022 10:11:14 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jul 2022 10:11:15 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 12 Jul 2022 10:11:36 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 12 Jul 2022 10:11:36 GMT
VOLUME [/spiped]
# Tue, 12 Jul 2022 10:11:37 GMT
WORKDIR /spiped
# Tue, 12 Jul 2022 10:11:39 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 12 Jul 2022 10:11:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 12 Jul 2022 10:11:40 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:1c0050b86a85a326857dbfa0456b3321f92df7e98ca468c048ee3e60dd14c923`  
		Last Modified: Tue, 12 Jul 2022 00:45:18 GMT  
		Size: 32.4 MB (32373949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8e6e812ac96abfcdb717a800cd828d568e7def1b3d35917aa8d4bca8dad5652`  
		Last Modified: Tue, 12 Jul 2022 10:12:09 GMT  
		Size: 1.6 KB (1608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00784f965ad2178a9dd189e47fa9d1dead759f8c77c4e1f9dc67f275a10e9ae9`  
		Last Modified: Tue, 12 Jul 2022 10:12:10 GMT  
		Size: 922.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f126b63a54a392ada3fd3a6b53de7045492f7f22ba2be170869580fd28547e01`  
		Last Modified: Tue, 12 Jul 2022 10:12:11 GMT  
		Size: 7.9 MB (7891582 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe752dbaa4e447a373aa54669e500c4e32f6f9b284533e19369ebc7438872f7c`  
		Last Modified: Tue, 12 Jul 2022 10:12:10 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f569d4d60dc0a559ed6ae4016595063cc8e4295684748541fc7fa85fe5d9547`  
		Last Modified: Tue, 12 Jul 2022 10:12:09 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; mips64le

```console
$ docker pull spiped@sha256:e162af37a4e20d682207ae49cd093bf7b0044cfc99ce551f5b10332794c5da65
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.3 MB (35349361 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6156c0cf6d90b9a331f11ae7e24f56d0305f54663334a41f53fa135306d66d45`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 23 Jun 2022 01:10:25 GMT
ADD file:fd1174cc47ac636f0cab382578a899d69ed489e4dee53ec838955e36066f526a in / 
# Thu, 23 Jun 2022 01:10:29 GMT
CMD ["bash"]
# Fri, 24 Jun 2022 18:58:18 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Fri, 24 Jun 2022 18:58:34 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Fri, 24 Jun 2022 18:58:37 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Fri, 24 Jun 2022 19:00:20 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Fri, 24 Jun 2022 19:00:23 GMT
VOLUME [/spiped]
# Fri, 24 Jun 2022 19:00:26 GMT
WORKDIR /spiped
# Fri, 24 Jun 2022 19:00:28 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 24 Jun 2022 19:00:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Jun 2022 19:00:34 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:9d199cb5e183b38c9edcc527cbaaa79bb56da73bd09ed449223842775ef4a244`  
		Last Modified: Thu, 23 Jun 2022 01:20:19 GMT  
		Size: 29.6 MB (29641027 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8b35ee3e9eb3ab4bd957c8fea2c070a89f00c8f52ca8de3288710051a9d1cd7`  
		Last Modified: Fri, 24 Jun 2022 19:00:48 GMT  
		Size: 1.6 KB (1629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b32716be1c1f2a4ddb4e5d54c3dcb56d3896e6824a35de4f561fee6dcc0e5992`  
		Last Modified: Fri, 24 Jun 2022 19:00:47 GMT  
		Size: 924.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cfae5b6fc11567c80ba42c9a1bd9de3715ef02276eed98c5b1ffb39d3fc758f`  
		Last Modified: Fri, 24 Jun 2022 19:00:52 GMT  
		Size: 5.7 MB (5705345 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56f38b405f221bf7479d8aa86b51068189793ddf16ac8d31e4cf4d5edfd75852`  
		Last Modified: Fri, 24 Jun 2022 19:00:47 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6df85a395a7ffbf2a27733183a022f3ffcf7f349ac191fb29be597a6f1826f0`  
		Last Modified: Fri, 24 Jun 2022 19:00:47 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; ppc64le

```console
$ docker pull spiped@sha256:d89bb7855b25826b0a725d13d5a13450999577803276bf8332af654bd87f70a0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.3 MB (41289345 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9b13180f5cd20f6db660992739b76dd4de2df48ec900ac0993ce5d41a7de4935`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 23 Jun 2022 02:02:32 GMT
ADD file:e18c13649ea1f145047652c8e171c4824f9b6b0dbc92127a914c7fca910acf96 in / 
# Thu, 23 Jun 2022 02:02:34 GMT
CMD ["bash"]
# Fri, 24 Jun 2022 03:18:35 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Fri, 24 Jun 2022 03:18:53 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Fri, 24 Jun 2022 03:18:57 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Fri, 24 Jun 2022 03:22:06 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Fri, 24 Jun 2022 03:22:12 GMT
VOLUME [/spiped]
# Fri, 24 Jun 2022 03:22:16 GMT
WORKDIR /spiped
# Fri, 24 Jun 2022 03:22:19 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 24 Jun 2022 03:22:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Jun 2022 03:22:27 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:7716f0df7ba06b6f1937cd664805984e25e386a4165f2c6acc65356686e35221`  
		Last Modified: Thu, 23 Jun 2022 02:15:20 GMT  
		Size: 35.3 MB (35286823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7ec9e1d5d07930dad33455ce5b658cb281b8b4ca54222eb1f60024ac816fbc7`  
		Last Modified: Fri, 24 Jun 2022 03:23:14 GMT  
		Size: 1.7 KB (1733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3db828a2d417c8a194dd6302acc44d0b0dd40d9b3fae07aadb0d20cc2a41e8b8`  
		Last Modified: Fri, 24 Jun 2022 03:23:13 GMT  
		Size: 1.1 KB (1054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03b13ec4baae0d6a140fe33601b6558b6b701e8d05eda8694d6e8b3a7598b74c`  
		Last Modified: Fri, 24 Jun 2022 03:23:15 GMT  
		Size: 6.0 MB (5999265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cac7d6f2fa097fe319d066933e0935b2de3401e1d842b9f32b2c94c6bfbc67c3`  
		Last Modified: Fri, 24 Jun 2022 03:23:13 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12b073d940ae730da8aa3f7369e0330f23a60789b3b477fca16b9af9beee52f7`  
		Last Modified: Fri, 24 Jun 2022 03:23:13 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; s390x

```console
$ docker pull spiped@sha256:8bd972f0849565f3731043355685c384106f649c1f341696e27b1b7d14bf8be3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.8 MB (34830502 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:18eac88cea751312874733838faf543f49c72e22acbc9731c2b8b41a687a5dd1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 12 Jul 2022 00:43:45 GMT
ADD file:70135711d42f7b2b32586e31afb57a0590019326efa82abf1402dc7a8f02a3f2 in / 
# Tue, 12 Jul 2022 00:43:49 GMT
CMD ["bash"]
# Tue, 12 Jul 2022 19:04:26 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 12 Jul 2022 19:04:31 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jul 2022 19:04:31 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 12 Jul 2022 19:05:04 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 12 Jul 2022 19:05:05 GMT
VOLUME [/spiped]
# Tue, 12 Jul 2022 19:05:06 GMT
WORKDIR /spiped
# Tue, 12 Jul 2022 19:05:06 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 12 Jul 2022 19:05:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 12 Jul 2022 19:05:07 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:447abc12b0c6da6e339b4fa17a2a7dd672d6f0631d30ee44c28b8b06e78884bd`  
		Last Modified: Tue, 12 Jul 2022 00:53:41 GMT  
		Size: 29.6 MB (29640209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5e8516db4eb8498fa25399fcdd57535b384acd4cfafd600572406c2aaf2ff06`  
		Last Modified: Tue, 12 Jul 2022 19:05:43 GMT  
		Size: 1.7 KB (1737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6724c44933ba59db5206197c52fc793f22f6666770d763bdefd2d83dc5280280`  
		Last Modified: Tue, 12 Jul 2022 19:05:43 GMT  
		Size: 1.1 KB (1052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3c0d2a85bf2d33562af565ac7d71584f04dcc861ffa720e2b756f47f32c4e4a`  
		Last Modified: Tue, 12 Jul 2022 19:05:44 GMT  
		Size: 5.2 MB (5187033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98ac9eaef5a9f646ed4fb767554c1aea10cdf9728990d98f03202ca185835a7d`  
		Last Modified: Tue, 12 Jul 2022 19:05:43 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdd350cfb7df80ef53f9da517d83a19efdfe980ef285d99a4d249093b4f8a52d`  
		Last Modified: Tue, 12 Jul 2022 19:05:43 GMT  
		Size: 342.0 B  
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
$ docker pull spiped@sha256:2df475af81759906c3da1ca65516f492123ebdb8bd14ab5dbd99082d8e21e38f
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
$ docker pull spiped@sha256:baa7adbbf67c6427f370b092b71b3e084e6b6f2b1b69d7830826bad32dc6474a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.3 MB (37337248 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ec58bdda4c26deb18400f539b267f1b2d59944078a579281e32030d0fac85c72`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 12 Jul 2022 01:20:10 GMT
ADD file:d978f6d3025a06f5142a0c13c98bf12fbd47cdf9162ed31fbc05c86983b0a679 in / 
# Tue, 12 Jul 2022 01:20:10 GMT
CMD ["bash"]
# Tue, 12 Jul 2022 14:24:08 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 12 Jul 2022 14:24:12 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jul 2022 14:24:12 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 12 Jul 2022 14:24:32 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 12 Jul 2022 14:24:32 GMT
VOLUME [/spiped]
# Tue, 12 Jul 2022 14:24:32 GMT
WORKDIR /spiped
# Tue, 12 Jul 2022 14:24:33 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 12 Jul 2022 14:24:33 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 12 Jul 2022 14:24:33 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:461246efe0a75316d99afdbf348f7063b57b0caeee8daab775f1f08152ea36f4`  
		Last Modified: Tue, 12 Jul 2022 01:24:34 GMT  
		Size: 31.4 MB (31366610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73ffd90cb7ba935b5f839a884b1ed9a58536b59f2da2d55ddbc19013590ac2bb`  
		Last Modified: Tue, 12 Jul 2022 14:24:50 GMT  
		Size: 1.7 KB (1731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:996ee512378210a090efc903c1338cd3ee02e97cd22d95ab5f8ee2418e65ffc4`  
		Last Modified: Tue, 12 Jul 2022 14:24:51 GMT  
		Size: 1.1 KB (1051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28eae5d1f26957502a0e384167f16a5ff3c906bf4c45cb3be57cbe2dde4e6c0f`  
		Last Modified: Tue, 12 Jul 2022 14:24:52 GMT  
		Size: 6.0 MB (5967386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcb594120cd340a1d759860341474d83f98217ae59b8e456504e58405a5c6168`  
		Last Modified: Tue, 12 Jul 2022 14:24:50 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b01900430d194aeac11a8520319b898c4bfb10e0ec043fa2a18ccca55ed39d8b`  
		Last Modified: Tue, 12 Jul 2022 14:24:51 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; arm variant v5

```console
$ docker pull spiped@sha256:da5c36b11149105885a68f9d371f023a53ddb8f039bf4128454a2e40eb570d0c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.9 MB (33936339 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3e4724dc7ea3fa813169dd39cb5ad7f614e01b9f08009359909a91a99521245d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 12 Jul 2022 00:50:38 GMT
ADD file:c11ce95201c98565eb5f40f837837d88c7b16d81d608b6dce953f51c90167b03 in / 
# Tue, 12 Jul 2022 00:50:39 GMT
CMD ["bash"]
# Wed, 13 Jul 2022 03:55:57 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 13 Jul 2022 03:56:07 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 13 Jul 2022 03:56:07 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 13 Jul 2022 03:56:58 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 13 Jul 2022 03:56:58 GMT
VOLUME [/spiped]
# Wed, 13 Jul 2022 03:56:59 GMT
WORKDIR /spiped
# Wed, 13 Jul 2022 03:57:00 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 13 Jul 2022 03:57:00 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 13 Jul 2022 03:57:00 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:f9371f3d7174b9da7d72bb3a49a5a3c5e96d5b106ef3113b25c27d30bb020de9`  
		Last Modified: Tue, 12 Jul 2022 01:03:01 GMT  
		Size: 28.9 MB (28905415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f17733f89592728022be14b12aa535e575d50c3af74c6b4b62ffeeddc543a9b`  
		Last Modified: Wed, 13 Jul 2022 03:57:34 GMT  
		Size: 1.7 KB (1726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c097088c4865734e08ad4830fec93508c0904f69a50143f46f5279682cb86d75`  
		Last Modified: Wed, 13 Jul 2022 03:57:34 GMT  
		Size: 1.0 KB (1049 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f772f929026de6cad41e4a47b51a6637f4d5eabed19b86d781c4c53cc1b251b`  
		Last Modified: Wed, 13 Jul 2022 03:57:39 GMT  
		Size: 5.0 MB (5027678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91ad846449f44ff79e0a2ae39faf88bdd83c752f9f30771988f0d0f56ffaf72a`  
		Last Modified: Wed, 13 Jul 2022 03:57:34 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15d89609ea2873d6e123e1f3296a9699103b5b3cf1e6362b1435ca04c1b04c9e`  
		Last Modified: Wed, 13 Jul 2022 03:57:34 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; arm variant v7

```console
$ docker pull spiped@sha256:8606eb476cb64fde0e9aa39f886d9bd31597a0197cdf07a090bc7881a0bdd8c1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.3 MB (31327684 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6aabe5099ff3912ff7cd11a03c60ba8aa2b298483f82513f7d086cd55a442181`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 23 Jun 2022 00:59:45 GMT
ADD file:925abfb9fc0e4a7cc0c979b12c9bd2607f5c493d37b05535ca010f81beb060a9 in / 
# Thu, 23 Jun 2022 00:59:46 GMT
CMD ["bash"]
# Thu, 23 Jun 2022 21:30:10 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Thu, 23 Jun 2022 21:30:18 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Thu, 23 Jun 2022 21:30:18 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 23 Jun 2022 21:31:06 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 23 Jun 2022 21:31:07 GMT
VOLUME [/spiped]
# Thu, 23 Jun 2022 21:31:08 GMT
WORKDIR /spiped
# Thu, 23 Jun 2022 21:31:08 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 23 Jun 2022 21:31:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Jun 2022 21:31:09 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:d2fd562560d8062a78064adfbfa204521167c301f00f5ab3c65b9c2a54083dba`  
		Last Modified: Thu, 23 Jun 2022 01:15:22 GMT  
		Size: 26.6 MB (26576105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99432086fbbe1dcdd9be0ab7f0395f40cfb463377a77ce42991d7938e5f97f4c`  
		Last Modified: Thu, 23 Jun 2022 21:32:07 GMT  
		Size: 1.7 KB (1728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f42f8e77af251ad3785548e41f782a72d1741d7a2a81d5ac4211cedfc6fd1322`  
		Last Modified: Thu, 23 Jun 2022 21:32:08 GMT  
		Size: 1.0 KB (1048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bdfcd7452d405dbbd5f03f66e9575a068f1e051c476a4d6ca7a9de6e3488a7b`  
		Last Modified: Thu, 23 Jun 2022 21:32:12 GMT  
		Size: 4.7 MB (4748331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91a24918704d53ee97e582f9cda126c8ae9faee7fea7f9a641174a290aa77352`  
		Last Modified: Thu, 23 Jun 2022 21:32:07 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0907fd39763b46ef91c12e8200fc7e8f4058a375ff39d8038aeffd79a4658d9f`  
		Last Modified: Thu, 23 Jun 2022 21:32:07 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:d7fc07e0161591d29e9c32ac511cad353265235e4e7c6e934471100bb8550cae
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.3 MB (35328185 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1cb54f7071b7db52f99ebd71b070c0129825389d5aab5ccb3d0cc2aefead6566`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 12 Jul 2022 00:40:34 GMT
ADD file:f3a33075f4c3324c6a634ef37a1965ddd5606b4449c0f5909ce18eeb8268b612 in / 
# Tue, 12 Jul 2022 00:40:35 GMT
CMD ["bash"]
# Tue, 12 Jul 2022 13:19:40 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 12 Jul 2022 13:19:43 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jul 2022 13:19:44 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 12 Jul 2022 13:20:02 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 12 Jul 2022 13:20:03 GMT
VOLUME [/spiped]
# Tue, 12 Jul 2022 13:20:04 GMT
WORKDIR /spiped
# Tue, 12 Jul 2022 13:20:06 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 12 Jul 2022 13:20:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 12 Jul 2022 13:20:07 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:60197a4c18d4b386d371cf39d01c48e98c357bba06da0b070a3c1f75006fd838`  
		Last Modified: Tue, 12 Jul 2022 00:46:13 GMT  
		Size: 30.1 MB (30054226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a089893717292b09eece50f192b80ac5ff6ff00637913777ba5c2df7ea8313a`  
		Last Modified: Tue, 12 Jul 2022 13:20:38 GMT  
		Size: 1.6 KB (1614 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f83311e0bf4416e1545ca652c599935e87c6b49e2b56f4bf7fa507de53cd0f17`  
		Last Modified: Tue, 12 Jul 2022 13:20:38 GMT  
		Size: 921.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efed5fb9a9bdee51f1f2c28ed64516d3ec10c256aa210403727ae6ff9d84a4ee`  
		Last Modified: Tue, 12 Jul 2022 13:20:39 GMT  
		Size: 5.3 MB (5270986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b74d6a8a5fa581a44b7d8e4e36dacdda29cee05dd3c17b98e55ff5ae56148c3a`  
		Last Modified: Tue, 12 Jul 2022 13:20:38 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a598427601e24498db86a01b1652d4cc3bb8862e1ebbdd06f38bf30347cd172a`  
		Last Modified: Tue, 12 Jul 2022 13:20:38 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; 386

```console
$ docker pull spiped@sha256:1fd21a5b9b47d2e84a4f398b21be00c2357ac211b9a7435ea05ce93ae14683c5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.3 MB (40268498 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1b4bdb79b659b9bd62a3954d3fcf8119356992184a3b5310ab501f92b829a8a3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 12 Jul 2022 00:39:27 GMT
ADD file:7f2bf44013d7848f051407d854b68c0d415a5328a3f5d241fca3150ce23bde65 in / 
# Tue, 12 Jul 2022 00:39:27 GMT
CMD ["bash"]
# Tue, 12 Jul 2022 10:11:10 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 12 Jul 2022 10:11:14 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jul 2022 10:11:15 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 12 Jul 2022 10:11:36 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 12 Jul 2022 10:11:36 GMT
VOLUME [/spiped]
# Tue, 12 Jul 2022 10:11:37 GMT
WORKDIR /spiped
# Tue, 12 Jul 2022 10:11:39 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 12 Jul 2022 10:11:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 12 Jul 2022 10:11:40 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:1c0050b86a85a326857dbfa0456b3321f92df7e98ca468c048ee3e60dd14c923`  
		Last Modified: Tue, 12 Jul 2022 00:45:18 GMT  
		Size: 32.4 MB (32373949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8e6e812ac96abfcdb717a800cd828d568e7def1b3d35917aa8d4bca8dad5652`  
		Last Modified: Tue, 12 Jul 2022 10:12:09 GMT  
		Size: 1.6 KB (1608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00784f965ad2178a9dd189e47fa9d1dead759f8c77c4e1f9dc67f275a10e9ae9`  
		Last Modified: Tue, 12 Jul 2022 10:12:10 GMT  
		Size: 922.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f126b63a54a392ada3fd3a6b53de7045492f7f22ba2be170869580fd28547e01`  
		Last Modified: Tue, 12 Jul 2022 10:12:11 GMT  
		Size: 7.9 MB (7891582 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe752dbaa4e447a373aa54669e500c4e32f6f9b284533e19369ebc7438872f7c`  
		Last Modified: Tue, 12 Jul 2022 10:12:10 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f569d4d60dc0a559ed6ae4016595063cc8e4295684748541fc7fa85fe5d9547`  
		Last Modified: Tue, 12 Jul 2022 10:12:09 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; mips64le

```console
$ docker pull spiped@sha256:e162af37a4e20d682207ae49cd093bf7b0044cfc99ce551f5b10332794c5da65
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.3 MB (35349361 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6156c0cf6d90b9a331f11ae7e24f56d0305f54663334a41f53fa135306d66d45`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 23 Jun 2022 01:10:25 GMT
ADD file:fd1174cc47ac636f0cab382578a899d69ed489e4dee53ec838955e36066f526a in / 
# Thu, 23 Jun 2022 01:10:29 GMT
CMD ["bash"]
# Fri, 24 Jun 2022 18:58:18 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Fri, 24 Jun 2022 18:58:34 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Fri, 24 Jun 2022 18:58:37 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Fri, 24 Jun 2022 19:00:20 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Fri, 24 Jun 2022 19:00:23 GMT
VOLUME [/spiped]
# Fri, 24 Jun 2022 19:00:26 GMT
WORKDIR /spiped
# Fri, 24 Jun 2022 19:00:28 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 24 Jun 2022 19:00:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Jun 2022 19:00:34 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:9d199cb5e183b38c9edcc527cbaaa79bb56da73bd09ed449223842775ef4a244`  
		Last Modified: Thu, 23 Jun 2022 01:20:19 GMT  
		Size: 29.6 MB (29641027 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8b35ee3e9eb3ab4bd957c8fea2c070a89f00c8f52ca8de3288710051a9d1cd7`  
		Last Modified: Fri, 24 Jun 2022 19:00:48 GMT  
		Size: 1.6 KB (1629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b32716be1c1f2a4ddb4e5d54c3dcb56d3896e6824a35de4f561fee6dcc0e5992`  
		Last Modified: Fri, 24 Jun 2022 19:00:47 GMT  
		Size: 924.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cfae5b6fc11567c80ba42c9a1bd9de3715ef02276eed98c5b1ffb39d3fc758f`  
		Last Modified: Fri, 24 Jun 2022 19:00:52 GMT  
		Size: 5.7 MB (5705345 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56f38b405f221bf7479d8aa86b51068189793ddf16ac8d31e4cf4d5edfd75852`  
		Last Modified: Fri, 24 Jun 2022 19:00:47 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6df85a395a7ffbf2a27733183a022f3ffcf7f349ac191fb29be597a6f1826f0`  
		Last Modified: Fri, 24 Jun 2022 19:00:47 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; ppc64le

```console
$ docker pull spiped@sha256:d89bb7855b25826b0a725d13d5a13450999577803276bf8332af654bd87f70a0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.3 MB (41289345 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9b13180f5cd20f6db660992739b76dd4de2df48ec900ac0993ce5d41a7de4935`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 23 Jun 2022 02:02:32 GMT
ADD file:e18c13649ea1f145047652c8e171c4824f9b6b0dbc92127a914c7fca910acf96 in / 
# Thu, 23 Jun 2022 02:02:34 GMT
CMD ["bash"]
# Fri, 24 Jun 2022 03:18:35 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Fri, 24 Jun 2022 03:18:53 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Fri, 24 Jun 2022 03:18:57 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Fri, 24 Jun 2022 03:22:06 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Fri, 24 Jun 2022 03:22:12 GMT
VOLUME [/spiped]
# Fri, 24 Jun 2022 03:22:16 GMT
WORKDIR /spiped
# Fri, 24 Jun 2022 03:22:19 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 24 Jun 2022 03:22:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Jun 2022 03:22:27 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:7716f0df7ba06b6f1937cd664805984e25e386a4165f2c6acc65356686e35221`  
		Last Modified: Thu, 23 Jun 2022 02:15:20 GMT  
		Size: 35.3 MB (35286823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7ec9e1d5d07930dad33455ce5b658cb281b8b4ca54222eb1f60024ac816fbc7`  
		Last Modified: Fri, 24 Jun 2022 03:23:14 GMT  
		Size: 1.7 KB (1733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3db828a2d417c8a194dd6302acc44d0b0dd40d9b3fae07aadb0d20cc2a41e8b8`  
		Last Modified: Fri, 24 Jun 2022 03:23:13 GMT  
		Size: 1.1 KB (1054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03b13ec4baae0d6a140fe33601b6558b6b701e8d05eda8694d6e8b3a7598b74c`  
		Last Modified: Fri, 24 Jun 2022 03:23:15 GMT  
		Size: 6.0 MB (5999265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cac7d6f2fa097fe319d066933e0935b2de3401e1d842b9f32b2c94c6bfbc67c3`  
		Last Modified: Fri, 24 Jun 2022 03:23:13 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12b073d940ae730da8aa3f7369e0330f23a60789b3b477fca16b9af9beee52f7`  
		Last Modified: Fri, 24 Jun 2022 03:23:13 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; s390x

```console
$ docker pull spiped@sha256:8bd972f0849565f3731043355685c384106f649c1f341696e27b1b7d14bf8be3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.8 MB (34830502 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:18eac88cea751312874733838faf543f49c72e22acbc9731c2b8b41a687a5dd1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 12 Jul 2022 00:43:45 GMT
ADD file:70135711d42f7b2b32586e31afb57a0590019326efa82abf1402dc7a8f02a3f2 in / 
# Tue, 12 Jul 2022 00:43:49 GMT
CMD ["bash"]
# Tue, 12 Jul 2022 19:04:26 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 12 Jul 2022 19:04:31 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jul 2022 19:04:31 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 12 Jul 2022 19:05:04 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 12 Jul 2022 19:05:05 GMT
VOLUME [/spiped]
# Tue, 12 Jul 2022 19:05:06 GMT
WORKDIR /spiped
# Tue, 12 Jul 2022 19:05:06 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 12 Jul 2022 19:05:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 12 Jul 2022 19:05:07 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:447abc12b0c6da6e339b4fa17a2a7dd672d6f0631d30ee44c28b8b06e78884bd`  
		Last Modified: Tue, 12 Jul 2022 00:53:41 GMT  
		Size: 29.6 MB (29640209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5e8516db4eb8498fa25399fcdd57535b384acd4cfafd600572406c2aaf2ff06`  
		Last Modified: Tue, 12 Jul 2022 19:05:43 GMT  
		Size: 1.7 KB (1737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6724c44933ba59db5206197c52fc793f22f6666770d763bdefd2d83dc5280280`  
		Last Modified: Tue, 12 Jul 2022 19:05:43 GMT  
		Size: 1.1 KB (1052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3c0d2a85bf2d33562af565ac7d71584f04dcc861ffa720e2b756f47f32c4e4a`  
		Last Modified: Tue, 12 Jul 2022 19:05:44 GMT  
		Size: 5.2 MB (5187033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98ac9eaef5a9f646ed4fb767554c1aea10cdf9728990d98f03202ca185835a7d`  
		Last Modified: Tue, 12 Jul 2022 19:05:43 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdd350cfb7df80ef53f9da517d83a19efdfe980ef285d99a4d249093b4f8a52d`  
		Last Modified: Tue, 12 Jul 2022 19:05:43 GMT  
		Size: 342.0 B  
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
$ docker pull spiped@sha256:2df475af81759906c3da1ca65516f492123ebdb8bd14ab5dbd99082d8e21e38f
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
$ docker pull spiped@sha256:baa7adbbf67c6427f370b092b71b3e084e6b6f2b1b69d7830826bad32dc6474a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.3 MB (37337248 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ec58bdda4c26deb18400f539b267f1b2d59944078a579281e32030d0fac85c72`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 12 Jul 2022 01:20:10 GMT
ADD file:d978f6d3025a06f5142a0c13c98bf12fbd47cdf9162ed31fbc05c86983b0a679 in / 
# Tue, 12 Jul 2022 01:20:10 GMT
CMD ["bash"]
# Tue, 12 Jul 2022 14:24:08 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 12 Jul 2022 14:24:12 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jul 2022 14:24:12 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 12 Jul 2022 14:24:32 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 12 Jul 2022 14:24:32 GMT
VOLUME [/spiped]
# Tue, 12 Jul 2022 14:24:32 GMT
WORKDIR /spiped
# Tue, 12 Jul 2022 14:24:33 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 12 Jul 2022 14:24:33 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 12 Jul 2022 14:24:33 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:461246efe0a75316d99afdbf348f7063b57b0caeee8daab775f1f08152ea36f4`  
		Last Modified: Tue, 12 Jul 2022 01:24:34 GMT  
		Size: 31.4 MB (31366610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73ffd90cb7ba935b5f839a884b1ed9a58536b59f2da2d55ddbc19013590ac2bb`  
		Last Modified: Tue, 12 Jul 2022 14:24:50 GMT  
		Size: 1.7 KB (1731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:996ee512378210a090efc903c1338cd3ee02e97cd22d95ab5f8ee2418e65ffc4`  
		Last Modified: Tue, 12 Jul 2022 14:24:51 GMT  
		Size: 1.1 KB (1051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28eae5d1f26957502a0e384167f16a5ff3c906bf4c45cb3be57cbe2dde4e6c0f`  
		Last Modified: Tue, 12 Jul 2022 14:24:52 GMT  
		Size: 6.0 MB (5967386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcb594120cd340a1d759860341474d83f98217ae59b8e456504e58405a5c6168`  
		Last Modified: Tue, 12 Jul 2022 14:24:50 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b01900430d194aeac11a8520319b898c4bfb10e0ec043fa2a18ccca55ed39d8b`  
		Last Modified: Tue, 12 Jul 2022 14:24:51 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.2` - linux; arm variant v5

```console
$ docker pull spiped@sha256:da5c36b11149105885a68f9d371f023a53ddb8f039bf4128454a2e40eb570d0c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.9 MB (33936339 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3e4724dc7ea3fa813169dd39cb5ad7f614e01b9f08009359909a91a99521245d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 12 Jul 2022 00:50:38 GMT
ADD file:c11ce95201c98565eb5f40f837837d88c7b16d81d608b6dce953f51c90167b03 in / 
# Tue, 12 Jul 2022 00:50:39 GMT
CMD ["bash"]
# Wed, 13 Jul 2022 03:55:57 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 13 Jul 2022 03:56:07 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 13 Jul 2022 03:56:07 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 13 Jul 2022 03:56:58 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 13 Jul 2022 03:56:58 GMT
VOLUME [/spiped]
# Wed, 13 Jul 2022 03:56:59 GMT
WORKDIR /spiped
# Wed, 13 Jul 2022 03:57:00 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 13 Jul 2022 03:57:00 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 13 Jul 2022 03:57:00 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:f9371f3d7174b9da7d72bb3a49a5a3c5e96d5b106ef3113b25c27d30bb020de9`  
		Last Modified: Tue, 12 Jul 2022 01:03:01 GMT  
		Size: 28.9 MB (28905415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f17733f89592728022be14b12aa535e575d50c3af74c6b4b62ffeeddc543a9b`  
		Last Modified: Wed, 13 Jul 2022 03:57:34 GMT  
		Size: 1.7 KB (1726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c097088c4865734e08ad4830fec93508c0904f69a50143f46f5279682cb86d75`  
		Last Modified: Wed, 13 Jul 2022 03:57:34 GMT  
		Size: 1.0 KB (1049 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f772f929026de6cad41e4a47b51a6637f4d5eabed19b86d781c4c53cc1b251b`  
		Last Modified: Wed, 13 Jul 2022 03:57:39 GMT  
		Size: 5.0 MB (5027678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91ad846449f44ff79e0a2ae39faf88bdd83c752f9f30771988f0d0f56ffaf72a`  
		Last Modified: Wed, 13 Jul 2022 03:57:34 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15d89609ea2873d6e123e1f3296a9699103b5b3cf1e6362b1435ca04c1b04c9e`  
		Last Modified: Wed, 13 Jul 2022 03:57:34 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.2` - linux; arm variant v7

```console
$ docker pull spiped@sha256:8606eb476cb64fde0e9aa39f886d9bd31597a0197cdf07a090bc7881a0bdd8c1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.3 MB (31327684 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6aabe5099ff3912ff7cd11a03c60ba8aa2b298483f82513f7d086cd55a442181`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 23 Jun 2022 00:59:45 GMT
ADD file:925abfb9fc0e4a7cc0c979b12c9bd2607f5c493d37b05535ca010f81beb060a9 in / 
# Thu, 23 Jun 2022 00:59:46 GMT
CMD ["bash"]
# Thu, 23 Jun 2022 21:30:10 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Thu, 23 Jun 2022 21:30:18 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Thu, 23 Jun 2022 21:30:18 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 23 Jun 2022 21:31:06 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 23 Jun 2022 21:31:07 GMT
VOLUME [/spiped]
# Thu, 23 Jun 2022 21:31:08 GMT
WORKDIR /spiped
# Thu, 23 Jun 2022 21:31:08 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 23 Jun 2022 21:31:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Jun 2022 21:31:09 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:d2fd562560d8062a78064adfbfa204521167c301f00f5ab3c65b9c2a54083dba`  
		Last Modified: Thu, 23 Jun 2022 01:15:22 GMT  
		Size: 26.6 MB (26576105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99432086fbbe1dcdd9be0ab7f0395f40cfb463377a77ce42991d7938e5f97f4c`  
		Last Modified: Thu, 23 Jun 2022 21:32:07 GMT  
		Size: 1.7 KB (1728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f42f8e77af251ad3785548e41f782a72d1741d7a2a81d5ac4211cedfc6fd1322`  
		Last Modified: Thu, 23 Jun 2022 21:32:08 GMT  
		Size: 1.0 KB (1048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bdfcd7452d405dbbd5f03f66e9575a068f1e051c476a4d6ca7a9de6e3488a7b`  
		Last Modified: Thu, 23 Jun 2022 21:32:12 GMT  
		Size: 4.7 MB (4748331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91a24918704d53ee97e582f9cda126c8ae9faee7fea7f9a641174a290aa77352`  
		Last Modified: Thu, 23 Jun 2022 21:32:07 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0907fd39763b46ef91c12e8200fc7e8f4058a375ff39d8038aeffd79a4658d9f`  
		Last Modified: Thu, 23 Jun 2022 21:32:07 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.2` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:d7fc07e0161591d29e9c32ac511cad353265235e4e7c6e934471100bb8550cae
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.3 MB (35328185 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1cb54f7071b7db52f99ebd71b070c0129825389d5aab5ccb3d0cc2aefead6566`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 12 Jul 2022 00:40:34 GMT
ADD file:f3a33075f4c3324c6a634ef37a1965ddd5606b4449c0f5909ce18eeb8268b612 in / 
# Tue, 12 Jul 2022 00:40:35 GMT
CMD ["bash"]
# Tue, 12 Jul 2022 13:19:40 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 12 Jul 2022 13:19:43 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jul 2022 13:19:44 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 12 Jul 2022 13:20:02 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 12 Jul 2022 13:20:03 GMT
VOLUME [/spiped]
# Tue, 12 Jul 2022 13:20:04 GMT
WORKDIR /spiped
# Tue, 12 Jul 2022 13:20:06 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 12 Jul 2022 13:20:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 12 Jul 2022 13:20:07 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:60197a4c18d4b386d371cf39d01c48e98c357bba06da0b070a3c1f75006fd838`  
		Last Modified: Tue, 12 Jul 2022 00:46:13 GMT  
		Size: 30.1 MB (30054226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a089893717292b09eece50f192b80ac5ff6ff00637913777ba5c2df7ea8313a`  
		Last Modified: Tue, 12 Jul 2022 13:20:38 GMT  
		Size: 1.6 KB (1614 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f83311e0bf4416e1545ca652c599935e87c6b49e2b56f4bf7fa507de53cd0f17`  
		Last Modified: Tue, 12 Jul 2022 13:20:38 GMT  
		Size: 921.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efed5fb9a9bdee51f1f2c28ed64516d3ec10c256aa210403727ae6ff9d84a4ee`  
		Last Modified: Tue, 12 Jul 2022 13:20:39 GMT  
		Size: 5.3 MB (5270986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b74d6a8a5fa581a44b7d8e4e36dacdda29cee05dd3c17b98e55ff5ae56148c3a`  
		Last Modified: Tue, 12 Jul 2022 13:20:38 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a598427601e24498db86a01b1652d4cc3bb8862e1ebbdd06f38bf30347cd172a`  
		Last Modified: Tue, 12 Jul 2022 13:20:38 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.2` - linux; 386

```console
$ docker pull spiped@sha256:1fd21a5b9b47d2e84a4f398b21be00c2357ac211b9a7435ea05ce93ae14683c5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.3 MB (40268498 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1b4bdb79b659b9bd62a3954d3fcf8119356992184a3b5310ab501f92b829a8a3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 12 Jul 2022 00:39:27 GMT
ADD file:7f2bf44013d7848f051407d854b68c0d415a5328a3f5d241fca3150ce23bde65 in / 
# Tue, 12 Jul 2022 00:39:27 GMT
CMD ["bash"]
# Tue, 12 Jul 2022 10:11:10 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 12 Jul 2022 10:11:14 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jul 2022 10:11:15 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 12 Jul 2022 10:11:36 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 12 Jul 2022 10:11:36 GMT
VOLUME [/spiped]
# Tue, 12 Jul 2022 10:11:37 GMT
WORKDIR /spiped
# Tue, 12 Jul 2022 10:11:39 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 12 Jul 2022 10:11:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 12 Jul 2022 10:11:40 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:1c0050b86a85a326857dbfa0456b3321f92df7e98ca468c048ee3e60dd14c923`  
		Last Modified: Tue, 12 Jul 2022 00:45:18 GMT  
		Size: 32.4 MB (32373949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8e6e812ac96abfcdb717a800cd828d568e7def1b3d35917aa8d4bca8dad5652`  
		Last Modified: Tue, 12 Jul 2022 10:12:09 GMT  
		Size: 1.6 KB (1608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00784f965ad2178a9dd189e47fa9d1dead759f8c77c4e1f9dc67f275a10e9ae9`  
		Last Modified: Tue, 12 Jul 2022 10:12:10 GMT  
		Size: 922.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f126b63a54a392ada3fd3a6b53de7045492f7f22ba2be170869580fd28547e01`  
		Last Modified: Tue, 12 Jul 2022 10:12:11 GMT  
		Size: 7.9 MB (7891582 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe752dbaa4e447a373aa54669e500c4e32f6f9b284533e19369ebc7438872f7c`  
		Last Modified: Tue, 12 Jul 2022 10:12:10 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f569d4d60dc0a559ed6ae4016595063cc8e4295684748541fc7fa85fe5d9547`  
		Last Modified: Tue, 12 Jul 2022 10:12:09 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.2` - linux; mips64le

```console
$ docker pull spiped@sha256:e162af37a4e20d682207ae49cd093bf7b0044cfc99ce551f5b10332794c5da65
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.3 MB (35349361 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6156c0cf6d90b9a331f11ae7e24f56d0305f54663334a41f53fa135306d66d45`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 23 Jun 2022 01:10:25 GMT
ADD file:fd1174cc47ac636f0cab382578a899d69ed489e4dee53ec838955e36066f526a in / 
# Thu, 23 Jun 2022 01:10:29 GMT
CMD ["bash"]
# Fri, 24 Jun 2022 18:58:18 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Fri, 24 Jun 2022 18:58:34 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Fri, 24 Jun 2022 18:58:37 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Fri, 24 Jun 2022 19:00:20 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Fri, 24 Jun 2022 19:00:23 GMT
VOLUME [/spiped]
# Fri, 24 Jun 2022 19:00:26 GMT
WORKDIR /spiped
# Fri, 24 Jun 2022 19:00:28 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 24 Jun 2022 19:00:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Jun 2022 19:00:34 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:9d199cb5e183b38c9edcc527cbaaa79bb56da73bd09ed449223842775ef4a244`  
		Last Modified: Thu, 23 Jun 2022 01:20:19 GMT  
		Size: 29.6 MB (29641027 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8b35ee3e9eb3ab4bd957c8fea2c070a89f00c8f52ca8de3288710051a9d1cd7`  
		Last Modified: Fri, 24 Jun 2022 19:00:48 GMT  
		Size: 1.6 KB (1629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b32716be1c1f2a4ddb4e5d54c3dcb56d3896e6824a35de4f561fee6dcc0e5992`  
		Last Modified: Fri, 24 Jun 2022 19:00:47 GMT  
		Size: 924.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cfae5b6fc11567c80ba42c9a1bd9de3715ef02276eed98c5b1ffb39d3fc758f`  
		Last Modified: Fri, 24 Jun 2022 19:00:52 GMT  
		Size: 5.7 MB (5705345 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56f38b405f221bf7479d8aa86b51068189793ddf16ac8d31e4cf4d5edfd75852`  
		Last Modified: Fri, 24 Jun 2022 19:00:47 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6df85a395a7ffbf2a27733183a022f3ffcf7f349ac191fb29be597a6f1826f0`  
		Last Modified: Fri, 24 Jun 2022 19:00:47 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.2` - linux; ppc64le

```console
$ docker pull spiped@sha256:d89bb7855b25826b0a725d13d5a13450999577803276bf8332af654bd87f70a0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.3 MB (41289345 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9b13180f5cd20f6db660992739b76dd4de2df48ec900ac0993ce5d41a7de4935`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 23 Jun 2022 02:02:32 GMT
ADD file:e18c13649ea1f145047652c8e171c4824f9b6b0dbc92127a914c7fca910acf96 in / 
# Thu, 23 Jun 2022 02:02:34 GMT
CMD ["bash"]
# Fri, 24 Jun 2022 03:18:35 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Fri, 24 Jun 2022 03:18:53 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Fri, 24 Jun 2022 03:18:57 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Fri, 24 Jun 2022 03:22:06 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Fri, 24 Jun 2022 03:22:12 GMT
VOLUME [/spiped]
# Fri, 24 Jun 2022 03:22:16 GMT
WORKDIR /spiped
# Fri, 24 Jun 2022 03:22:19 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 24 Jun 2022 03:22:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Jun 2022 03:22:27 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:7716f0df7ba06b6f1937cd664805984e25e386a4165f2c6acc65356686e35221`  
		Last Modified: Thu, 23 Jun 2022 02:15:20 GMT  
		Size: 35.3 MB (35286823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7ec9e1d5d07930dad33455ce5b658cb281b8b4ca54222eb1f60024ac816fbc7`  
		Last Modified: Fri, 24 Jun 2022 03:23:14 GMT  
		Size: 1.7 KB (1733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3db828a2d417c8a194dd6302acc44d0b0dd40d9b3fae07aadb0d20cc2a41e8b8`  
		Last Modified: Fri, 24 Jun 2022 03:23:13 GMT  
		Size: 1.1 KB (1054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03b13ec4baae0d6a140fe33601b6558b6b701e8d05eda8694d6e8b3a7598b74c`  
		Last Modified: Fri, 24 Jun 2022 03:23:15 GMT  
		Size: 6.0 MB (5999265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cac7d6f2fa097fe319d066933e0935b2de3401e1d842b9f32b2c94c6bfbc67c3`  
		Last Modified: Fri, 24 Jun 2022 03:23:13 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12b073d940ae730da8aa3f7369e0330f23a60789b3b477fca16b9af9beee52f7`  
		Last Modified: Fri, 24 Jun 2022 03:23:13 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.2` - linux; s390x

```console
$ docker pull spiped@sha256:8bd972f0849565f3731043355685c384106f649c1f341696e27b1b7d14bf8be3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.8 MB (34830502 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:18eac88cea751312874733838faf543f49c72e22acbc9731c2b8b41a687a5dd1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 12 Jul 2022 00:43:45 GMT
ADD file:70135711d42f7b2b32586e31afb57a0590019326efa82abf1402dc7a8f02a3f2 in / 
# Tue, 12 Jul 2022 00:43:49 GMT
CMD ["bash"]
# Tue, 12 Jul 2022 19:04:26 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 12 Jul 2022 19:04:31 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jul 2022 19:04:31 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 12 Jul 2022 19:05:04 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 12 Jul 2022 19:05:05 GMT
VOLUME [/spiped]
# Tue, 12 Jul 2022 19:05:06 GMT
WORKDIR /spiped
# Tue, 12 Jul 2022 19:05:06 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 12 Jul 2022 19:05:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 12 Jul 2022 19:05:07 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:447abc12b0c6da6e339b4fa17a2a7dd672d6f0631d30ee44c28b8b06e78884bd`  
		Last Modified: Tue, 12 Jul 2022 00:53:41 GMT  
		Size: 29.6 MB (29640209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5e8516db4eb8498fa25399fcdd57535b384acd4cfafd600572406c2aaf2ff06`  
		Last Modified: Tue, 12 Jul 2022 19:05:43 GMT  
		Size: 1.7 KB (1737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6724c44933ba59db5206197c52fc793f22f6666770d763bdefd2d83dc5280280`  
		Last Modified: Tue, 12 Jul 2022 19:05:43 GMT  
		Size: 1.1 KB (1052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3c0d2a85bf2d33562af565ac7d71584f04dcc861ffa720e2b756f47f32c4e4a`  
		Last Modified: Tue, 12 Jul 2022 19:05:44 GMT  
		Size: 5.2 MB (5187033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98ac9eaef5a9f646ed4fb767554c1aea10cdf9728990d98f03202ca185835a7d`  
		Last Modified: Tue, 12 Jul 2022 19:05:43 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdd350cfb7df80ef53f9da517d83a19efdfe980ef285d99a4d249093b4f8a52d`  
		Last Modified: Tue, 12 Jul 2022 19:05:43 GMT  
		Size: 342.0 B  
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
$ docker pull spiped@sha256:2df475af81759906c3da1ca65516f492123ebdb8bd14ab5dbd99082d8e21e38f
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
$ docker pull spiped@sha256:baa7adbbf67c6427f370b092b71b3e084e6b6f2b1b69d7830826bad32dc6474a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.3 MB (37337248 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ec58bdda4c26deb18400f539b267f1b2d59944078a579281e32030d0fac85c72`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 12 Jul 2022 01:20:10 GMT
ADD file:d978f6d3025a06f5142a0c13c98bf12fbd47cdf9162ed31fbc05c86983b0a679 in / 
# Tue, 12 Jul 2022 01:20:10 GMT
CMD ["bash"]
# Tue, 12 Jul 2022 14:24:08 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 12 Jul 2022 14:24:12 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jul 2022 14:24:12 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 12 Jul 2022 14:24:32 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 12 Jul 2022 14:24:32 GMT
VOLUME [/spiped]
# Tue, 12 Jul 2022 14:24:32 GMT
WORKDIR /spiped
# Tue, 12 Jul 2022 14:24:33 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 12 Jul 2022 14:24:33 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 12 Jul 2022 14:24:33 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:461246efe0a75316d99afdbf348f7063b57b0caeee8daab775f1f08152ea36f4`  
		Last Modified: Tue, 12 Jul 2022 01:24:34 GMT  
		Size: 31.4 MB (31366610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73ffd90cb7ba935b5f839a884b1ed9a58536b59f2da2d55ddbc19013590ac2bb`  
		Last Modified: Tue, 12 Jul 2022 14:24:50 GMT  
		Size: 1.7 KB (1731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:996ee512378210a090efc903c1338cd3ee02e97cd22d95ab5f8ee2418e65ffc4`  
		Last Modified: Tue, 12 Jul 2022 14:24:51 GMT  
		Size: 1.1 KB (1051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28eae5d1f26957502a0e384167f16a5ff3c906bf4c45cb3be57cbe2dde4e6c0f`  
		Last Modified: Tue, 12 Jul 2022 14:24:52 GMT  
		Size: 6.0 MB (5967386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcb594120cd340a1d759860341474d83f98217ae59b8e456504e58405a5c6168`  
		Last Modified: Tue, 12 Jul 2022 14:24:50 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b01900430d194aeac11a8520319b898c4bfb10e0ec043fa2a18ccca55ed39d8b`  
		Last Modified: Tue, 12 Jul 2022 14:24:51 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; arm variant v5

```console
$ docker pull spiped@sha256:da5c36b11149105885a68f9d371f023a53ddb8f039bf4128454a2e40eb570d0c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.9 MB (33936339 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3e4724dc7ea3fa813169dd39cb5ad7f614e01b9f08009359909a91a99521245d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 12 Jul 2022 00:50:38 GMT
ADD file:c11ce95201c98565eb5f40f837837d88c7b16d81d608b6dce953f51c90167b03 in / 
# Tue, 12 Jul 2022 00:50:39 GMT
CMD ["bash"]
# Wed, 13 Jul 2022 03:55:57 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 13 Jul 2022 03:56:07 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 13 Jul 2022 03:56:07 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 13 Jul 2022 03:56:58 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 13 Jul 2022 03:56:58 GMT
VOLUME [/spiped]
# Wed, 13 Jul 2022 03:56:59 GMT
WORKDIR /spiped
# Wed, 13 Jul 2022 03:57:00 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 13 Jul 2022 03:57:00 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 13 Jul 2022 03:57:00 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:f9371f3d7174b9da7d72bb3a49a5a3c5e96d5b106ef3113b25c27d30bb020de9`  
		Last Modified: Tue, 12 Jul 2022 01:03:01 GMT  
		Size: 28.9 MB (28905415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f17733f89592728022be14b12aa535e575d50c3af74c6b4b62ffeeddc543a9b`  
		Last Modified: Wed, 13 Jul 2022 03:57:34 GMT  
		Size: 1.7 KB (1726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c097088c4865734e08ad4830fec93508c0904f69a50143f46f5279682cb86d75`  
		Last Modified: Wed, 13 Jul 2022 03:57:34 GMT  
		Size: 1.0 KB (1049 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f772f929026de6cad41e4a47b51a6637f4d5eabed19b86d781c4c53cc1b251b`  
		Last Modified: Wed, 13 Jul 2022 03:57:39 GMT  
		Size: 5.0 MB (5027678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91ad846449f44ff79e0a2ae39faf88bdd83c752f9f30771988f0d0f56ffaf72a`  
		Last Modified: Wed, 13 Jul 2022 03:57:34 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15d89609ea2873d6e123e1f3296a9699103b5b3cf1e6362b1435ca04c1b04c9e`  
		Last Modified: Wed, 13 Jul 2022 03:57:34 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; arm variant v7

```console
$ docker pull spiped@sha256:8606eb476cb64fde0e9aa39f886d9bd31597a0197cdf07a090bc7881a0bdd8c1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.3 MB (31327684 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6aabe5099ff3912ff7cd11a03c60ba8aa2b298483f82513f7d086cd55a442181`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 23 Jun 2022 00:59:45 GMT
ADD file:925abfb9fc0e4a7cc0c979b12c9bd2607f5c493d37b05535ca010f81beb060a9 in / 
# Thu, 23 Jun 2022 00:59:46 GMT
CMD ["bash"]
# Thu, 23 Jun 2022 21:30:10 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Thu, 23 Jun 2022 21:30:18 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Thu, 23 Jun 2022 21:30:18 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 23 Jun 2022 21:31:06 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 23 Jun 2022 21:31:07 GMT
VOLUME [/spiped]
# Thu, 23 Jun 2022 21:31:08 GMT
WORKDIR /spiped
# Thu, 23 Jun 2022 21:31:08 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 23 Jun 2022 21:31:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Jun 2022 21:31:09 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:d2fd562560d8062a78064adfbfa204521167c301f00f5ab3c65b9c2a54083dba`  
		Last Modified: Thu, 23 Jun 2022 01:15:22 GMT  
		Size: 26.6 MB (26576105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99432086fbbe1dcdd9be0ab7f0395f40cfb463377a77ce42991d7938e5f97f4c`  
		Last Modified: Thu, 23 Jun 2022 21:32:07 GMT  
		Size: 1.7 KB (1728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f42f8e77af251ad3785548e41f782a72d1741d7a2a81d5ac4211cedfc6fd1322`  
		Last Modified: Thu, 23 Jun 2022 21:32:08 GMT  
		Size: 1.0 KB (1048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bdfcd7452d405dbbd5f03f66e9575a068f1e051c476a4d6ca7a9de6e3488a7b`  
		Last Modified: Thu, 23 Jun 2022 21:32:12 GMT  
		Size: 4.7 MB (4748331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91a24918704d53ee97e582f9cda126c8ae9faee7fea7f9a641174a290aa77352`  
		Last Modified: Thu, 23 Jun 2022 21:32:07 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0907fd39763b46ef91c12e8200fc7e8f4058a375ff39d8038aeffd79a4658d9f`  
		Last Modified: Thu, 23 Jun 2022 21:32:07 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:d7fc07e0161591d29e9c32ac511cad353265235e4e7c6e934471100bb8550cae
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.3 MB (35328185 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1cb54f7071b7db52f99ebd71b070c0129825389d5aab5ccb3d0cc2aefead6566`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 12 Jul 2022 00:40:34 GMT
ADD file:f3a33075f4c3324c6a634ef37a1965ddd5606b4449c0f5909ce18eeb8268b612 in / 
# Tue, 12 Jul 2022 00:40:35 GMT
CMD ["bash"]
# Tue, 12 Jul 2022 13:19:40 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 12 Jul 2022 13:19:43 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jul 2022 13:19:44 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 12 Jul 2022 13:20:02 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 12 Jul 2022 13:20:03 GMT
VOLUME [/spiped]
# Tue, 12 Jul 2022 13:20:04 GMT
WORKDIR /spiped
# Tue, 12 Jul 2022 13:20:06 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 12 Jul 2022 13:20:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 12 Jul 2022 13:20:07 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:60197a4c18d4b386d371cf39d01c48e98c357bba06da0b070a3c1f75006fd838`  
		Last Modified: Tue, 12 Jul 2022 00:46:13 GMT  
		Size: 30.1 MB (30054226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a089893717292b09eece50f192b80ac5ff6ff00637913777ba5c2df7ea8313a`  
		Last Modified: Tue, 12 Jul 2022 13:20:38 GMT  
		Size: 1.6 KB (1614 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f83311e0bf4416e1545ca652c599935e87c6b49e2b56f4bf7fa507de53cd0f17`  
		Last Modified: Tue, 12 Jul 2022 13:20:38 GMT  
		Size: 921.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efed5fb9a9bdee51f1f2c28ed64516d3ec10c256aa210403727ae6ff9d84a4ee`  
		Last Modified: Tue, 12 Jul 2022 13:20:39 GMT  
		Size: 5.3 MB (5270986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b74d6a8a5fa581a44b7d8e4e36dacdda29cee05dd3c17b98e55ff5ae56148c3a`  
		Last Modified: Tue, 12 Jul 2022 13:20:38 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a598427601e24498db86a01b1652d4cc3bb8862e1ebbdd06f38bf30347cd172a`  
		Last Modified: Tue, 12 Jul 2022 13:20:38 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; 386

```console
$ docker pull spiped@sha256:1fd21a5b9b47d2e84a4f398b21be00c2357ac211b9a7435ea05ce93ae14683c5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.3 MB (40268498 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1b4bdb79b659b9bd62a3954d3fcf8119356992184a3b5310ab501f92b829a8a3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 12 Jul 2022 00:39:27 GMT
ADD file:7f2bf44013d7848f051407d854b68c0d415a5328a3f5d241fca3150ce23bde65 in / 
# Tue, 12 Jul 2022 00:39:27 GMT
CMD ["bash"]
# Tue, 12 Jul 2022 10:11:10 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 12 Jul 2022 10:11:14 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jul 2022 10:11:15 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 12 Jul 2022 10:11:36 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 12 Jul 2022 10:11:36 GMT
VOLUME [/spiped]
# Tue, 12 Jul 2022 10:11:37 GMT
WORKDIR /spiped
# Tue, 12 Jul 2022 10:11:39 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 12 Jul 2022 10:11:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 12 Jul 2022 10:11:40 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:1c0050b86a85a326857dbfa0456b3321f92df7e98ca468c048ee3e60dd14c923`  
		Last Modified: Tue, 12 Jul 2022 00:45:18 GMT  
		Size: 32.4 MB (32373949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8e6e812ac96abfcdb717a800cd828d568e7def1b3d35917aa8d4bca8dad5652`  
		Last Modified: Tue, 12 Jul 2022 10:12:09 GMT  
		Size: 1.6 KB (1608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00784f965ad2178a9dd189e47fa9d1dead759f8c77c4e1f9dc67f275a10e9ae9`  
		Last Modified: Tue, 12 Jul 2022 10:12:10 GMT  
		Size: 922.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f126b63a54a392ada3fd3a6b53de7045492f7f22ba2be170869580fd28547e01`  
		Last Modified: Tue, 12 Jul 2022 10:12:11 GMT  
		Size: 7.9 MB (7891582 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe752dbaa4e447a373aa54669e500c4e32f6f9b284533e19369ebc7438872f7c`  
		Last Modified: Tue, 12 Jul 2022 10:12:10 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f569d4d60dc0a559ed6ae4016595063cc8e4295684748541fc7fa85fe5d9547`  
		Last Modified: Tue, 12 Jul 2022 10:12:09 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; mips64le

```console
$ docker pull spiped@sha256:e162af37a4e20d682207ae49cd093bf7b0044cfc99ce551f5b10332794c5da65
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.3 MB (35349361 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6156c0cf6d90b9a331f11ae7e24f56d0305f54663334a41f53fa135306d66d45`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 23 Jun 2022 01:10:25 GMT
ADD file:fd1174cc47ac636f0cab382578a899d69ed489e4dee53ec838955e36066f526a in / 
# Thu, 23 Jun 2022 01:10:29 GMT
CMD ["bash"]
# Fri, 24 Jun 2022 18:58:18 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Fri, 24 Jun 2022 18:58:34 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Fri, 24 Jun 2022 18:58:37 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Fri, 24 Jun 2022 19:00:20 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Fri, 24 Jun 2022 19:00:23 GMT
VOLUME [/spiped]
# Fri, 24 Jun 2022 19:00:26 GMT
WORKDIR /spiped
# Fri, 24 Jun 2022 19:00:28 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 24 Jun 2022 19:00:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Jun 2022 19:00:34 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:9d199cb5e183b38c9edcc527cbaaa79bb56da73bd09ed449223842775ef4a244`  
		Last Modified: Thu, 23 Jun 2022 01:20:19 GMT  
		Size: 29.6 MB (29641027 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8b35ee3e9eb3ab4bd957c8fea2c070a89f00c8f52ca8de3288710051a9d1cd7`  
		Last Modified: Fri, 24 Jun 2022 19:00:48 GMT  
		Size: 1.6 KB (1629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b32716be1c1f2a4ddb4e5d54c3dcb56d3896e6824a35de4f561fee6dcc0e5992`  
		Last Modified: Fri, 24 Jun 2022 19:00:47 GMT  
		Size: 924.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cfae5b6fc11567c80ba42c9a1bd9de3715ef02276eed98c5b1ffb39d3fc758f`  
		Last Modified: Fri, 24 Jun 2022 19:00:52 GMT  
		Size: 5.7 MB (5705345 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56f38b405f221bf7479d8aa86b51068189793ddf16ac8d31e4cf4d5edfd75852`  
		Last Modified: Fri, 24 Jun 2022 19:00:47 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6df85a395a7ffbf2a27733183a022f3ffcf7f349ac191fb29be597a6f1826f0`  
		Last Modified: Fri, 24 Jun 2022 19:00:47 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; ppc64le

```console
$ docker pull spiped@sha256:d89bb7855b25826b0a725d13d5a13450999577803276bf8332af654bd87f70a0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.3 MB (41289345 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9b13180f5cd20f6db660992739b76dd4de2df48ec900ac0993ce5d41a7de4935`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 23 Jun 2022 02:02:32 GMT
ADD file:e18c13649ea1f145047652c8e171c4824f9b6b0dbc92127a914c7fca910acf96 in / 
# Thu, 23 Jun 2022 02:02:34 GMT
CMD ["bash"]
# Fri, 24 Jun 2022 03:18:35 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Fri, 24 Jun 2022 03:18:53 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Fri, 24 Jun 2022 03:18:57 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Fri, 24 Jun 2022 03:22:06 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Fri, 24 Jun 2022 03:22:12 GMT
VOLUME [/spiped]
# Fri, 24 Jun 2022 03:22:16 GMT
WORKDIR /spiped
# Fri, 24 Jun 2022 03:22:19 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 24 Jun 2022 03:22:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Jun 2022 03:22:27 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:7716f0df7ba06b6f1937cd664805984e25e386a4165f2c6acc65356686e35221`  
		Last Modified: Thu, 23 Jun 2022 02:15:20 GMT  
		Size: 35.3 MB (35286823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7ec9e1d5d07930dad33455ce5b658cb281b8b4ca54222eb1f60024ac816fbc7`  
		Last Modified: Fri, 24 Jun 2022 03:23:14 GMT  
		Size: 1.7 KB (1733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3db828a2d417c8a194dd6302acc44d0b0dd40d9b3fae07aadb0d20cc2a41e8b8`  
		Last Modified: Fri, 24 Jun 2022 03:23:13 GMT  
		Size: 1.1 KB (1054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03b13ec4baae0d6a140fe33601b6558b6b701e8d05eda8694d6e8b3a7598b74c`  
		Last Modified: Fri, 24 Jun 2022 03:23:15 GMT  
		Size: 6.0 MB (5999265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cac7d6f2fa097fe319d066933e0935b2de3401e1d842b9f32b2c94c6bfbc67c3`  
		Last Modified: Fri, 24 Jun 2022 03:23:13 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12b073d940ae730da8aa3f7369e0330f23a60789b3b477fca16b9af9beee52f7`  
		Last Modified: Fri, 24 Jun 2022 03:23:13 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; s390x

```console
$ docker pull spiped@sha256:8bd972f0849565f3731043355685c384106f649c1f341696e27b1b7d14bf8be3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.8 MB (34830502 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:18eac88cea751312874733838faf543f49c72e22acbc9731c2b8b41a687a5dd1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 12 Jul 2022 00:43:45 GMT
ADD file:70135711d42f7b2b32586e31afb57a0590019326efa82abf1402dc7a8f02a3f2 in / 
# Tue, 12 Jul 2022 00:43:49 GMT
CMD ["bash"]
# Tue, 12 Jul 2022 19:04:26 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 12 Jul 2022 19:04:31 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jul 2022 19:04:31 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 12 Jul 2022 19:05:04 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 12 Jul 2022 19:05:05 GMT
VOLUME [/spiped]
# Tue, 12 Jul 2022 19:05:06 GMT
WORKDIR /spiped
# Tue, 12 Jul 2022 19:05:06 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 12 Jul 2022 19:05:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 12 Jul 2022 19:05:07 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:447abc12b0c6da6e339b4fa17a2a7dd672d6f0631d30ee44c28b8b06e78884bd`  
		Last Modified: Tue, 12 Jul 2022 00:53:41 GMT  
		Size: 29.6 MB (29640209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5e8516db4eb8498fa25399fcdd57535b384acd4cfafd600572406c2aaf2ff06`  
		Last Modified: Tue, 12 Jul 2022 19:05:43 GMT  
		Size: 1.7 KB (1737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6724c44933ba59db5206197c52fc793f22f6666770d763bdefd2d83dc5280280`  
		Last Modified: Tue, 12 Jul 2022 19:05:43 GMT  
		Size: 1.1 KB (1052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3c0d2a85bf2d33562af565ac7d71584f04dcc861ffa720e2b756f47f32c4e4a`  
		Last Modified: Tue, 12 Jul 2022 19:05:44 GMT  
		Size: 5.2 MB (5187033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98ac9eaef5a9f646ed4fb767554c1aea10cdf9728990d98f03202ca185835a7d`  
		Last Modified: Tue, 12 Jul 2022 19:05:43 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdd350cfb7df80ef53f9da517d83a19efdfe980ef285d99a4d249093b4f8a52d`  
		Last Modified: Tue, 12 Jul 2022 19:05:43 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
