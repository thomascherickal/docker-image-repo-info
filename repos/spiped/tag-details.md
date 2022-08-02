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
$ docker pull spiped@sha256:893b1d34151bff6fc3b147f4492989c25976f4c5bd2b714b7872c22ddcf32453
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
$ docker pull spiped@sha256:f83b419d27348b2bdbf4d6e78da6d2e62f75d514a1ed39855e1899dc9b59fe73
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.3 MB (31312141 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:524e3e7d21e31be2a48e1548d86d5ced3a2ee4185440b47edacceca48ca97031`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 12 Jul 2022 00:59:54 GMT
ADD file:ae890621b36ff6e27364bb7316b5bd4319a820ddf7e65565c6201eb11d70fde9 in / 
# Tue, 12 Jul 2022 00:59:55 GMT
CMD ["bash"]
# Wed, 13 Jul 2022 07:57:44 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 13 Jul 2022 07:57:51 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 13 Jul 2022 07:57:52 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 13 Jul 2022 07:58:36 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 13 Jul 2022 07:58:37 GMT
VOLUME [/spiped]
# Wed, 13 Jul 2022 07:58:37 GMT
WORKDIR /spiped
# Wed, 13 Jul 2022 07:58:38 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 13 Jul 2022 07:58:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 13 Jul 2022 07:58:39 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:314cda9d0ef2282082d2bd0efd7659e0d9edb3ceae8e7919d990bcf95cbb3d2b`  
		Last Modified: Tue, 12 Jul 2022 01:12:37 GMT  
		Size: 26.6 MB (26560559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:090471f791b0f328f3661d50b9ff593c83c6e102cdb08df2fd72cecb662ff0be`  
		Last Modified: Wed, 13 Jul 2022 07:59:38 GMT  
		Size: 1.7 KB (1727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c4dfc160206772b3b1e6340d5d682c20ec1e14e0871426b46711d58b7d6833c`  
		Last Modified: Wed, 13 Jul 2022 07:59:38 GMT  
		Size: 1.1 KB (1053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89bb0f704911b77275d75f7bc8b4cf0b5162ade51f380f463c6cc820cac6968d`  
		Last Modified: Wed, 13 Jul 2022 07:59:42 GMT  
		Size: 4.7 MB (4748333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5b67ae8b1bcc4511eeadde14a66ebab56c086d30f91559679a64b68b73fc76a`  
		Last Modified: Wed, 13 Jul 2022 07:59:38 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:630225b9ddc0c86154ca5f1fa26d05def1293638c2be832017738f83eadd93a3`  
		Last Modified: Wed, 13 Jul 2022 07:59:38 GMT  
		Size: 342.0 B  
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
$ docker pull spiped@sha256:0912dd64711f962ed20b280e96cc372e615b95b97ee1aa6a9056ba1f36a9f4cc
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.3 MB (35337184 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:40302e59e0dfc3ac7483cdda59a1917781d6bf1697c399cd8718d32fc20b3ab8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 12 Jul 2022 04:40:59 GMT
ADD file:e0c3a3f07bbd2b798f2f620e295566d0b49142660f897083f73164c0356f37a2 in / 
# Tue, 12 Jul 2022 04:41:04 GMT
CMD ["bash"]
# Wed, 13 Jul 2022 10:54:04 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 13 Jul 2022 10:54:19 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 13 Jul 2022 10:54:21 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 13 Jul 2022 10:55:53 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 13 Jul 2022 10:55:55 GMT
VOLUME [/spiped]
# Wed, 13 Jul 2022 10:55:58 GMT
WORKDIR /spiped
# Wed, 13 Jul 2022 10:56:00 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 13 Jul 2022 10:56:03 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 13 Jul 2022 10:56:06 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:88869778ecefe05f3e79ed90f3c06c22dfef4c56919a454f67eba47fb8072189`  
		Last Modified: Tue, 12 Jul 2022 04:51:44 GMT  
		Size: 29.6 MB (29628932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8dce35712b9df24fe23728e831a2d450572f507f476fca4f37b578b13c0f258f`  
		Last Modified: Wed, 13 Jul 2022 10:56:20 GMT  
		Size: 1.6 KB (1619 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78bf32252f913a3a579a40ec4538d9f0a46238b5bf83d6660c4967cca14df32a`  
		Last Modified: Wed, 13 Jul 2022 10:56:20 GMT  
		Size: 922.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:895648de55366c4420ab371cebceab082edcb43321c746dc76fb385c47594187`  
		Last Modified: Wed, 13 Jul 2022 10:56:26 GMT  
		Size: 5.7 MB (5705273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:918d7dc0f0ce53174644562b626a49d277285fa8c4ea2bcc0acc8efc1e63f7f6`  
		Last Modified: Wed, 13 Jul 2022 10:56:20 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1777ed1e7ecf5154695c61e242216358df92c1b5d2cef0c91e5b19b3b500b7c9`  
		Last Modified: Wed, 13 Jul 2022 10:56:20 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; ppc64le

```console
$ docker pull spiped@sha256:81003cf3de708c1d144d9355412aec5bdf2094c49b740cb388711db570b4356f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.3 MB (41275059 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4406e24e415436179ca82b111445f95864a4f68270845d8f13f8f6738e6dd613`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 12 Jul 2022 01:25:28 GMT
ADD file:9e1afe48f40d94f879aefb12a7e68da2f0772d701e95b8219bd1f79a83e1933a in / 
# Tue, 12 Jul 2022 01:25:32 GMT
CMD ["bash"]
# Wed, 13 Jul 2022 06:43:01 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 13 Jul 2022 06:43:12 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 13 Jul 2022 06:43:14 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 13 Jul 2022 06:45:53 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 13 Jul 2022 06:45:55 GMT
VOLUME [/spiped]
# Wed, 13 Jul 2022 06:45:59 GMT
WORKDIR /spiped
# Wed, 13 Jul 2022 06:46:01 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 13 Jul 2022 06:46:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 13 Jul 2022 06:46:06 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:bd3d68d1ce583727f6378a16916795b955cc0ad39e0ebe754a26007ef54744fa`  
		Last Modified: Tue, 12 Jul 2022 01:36:03 GMT  
		Size: 35.3 MB (35272500 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9118819a47938b959974a2c187124c206d412a4381b1fa00b07702644095ac5d`  
		Last Modified: Wed, 13 Jul 2022 06:46:45 GMT  
		Size: 1.7 KB (1730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:387914e121edf896abe5847d4c111ed304f65ba32e283e8c551636e0603f325c`  
		Last Modified: Wed, 13 Jul 2022 06:46:45 GMT  
		Size: 1.1 KB (1053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bbc4a7edac4c6f551075397bc114c02da11b03ddf357cadb338265a627754b4`  
		Last Modified: Wed, 13 Jul 2022 06:46:46 GMT  
		Size: 6.0 MB (5999305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:773d9584db6f6fede768ee1493062d61d3061585c34a2d6716802a94dcf16103`  
		Last Modified: Wed, 13 Jul 2022 06:46:45 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e83ac10baec3d66ad682bc3eefbc4b8d96730fafcf154ef2da09edeb47bb1f7b`  
		Last Modified: Wed, 13 Jul 2022 06:46:45 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; s390x

```console
$ docker pull spiped@sha256:7bf397f297d1ea78dd655acc6c96775a5343e89423693de15ff17f08a7e69fda
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.8 MB (34830403 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3d0f9f2ec0119a2ccfd6b0ef28575b5bc407594263c24f89aa33495fe897631e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 02 Aug 2022 00:42:27 GMT
ADD file:c2afc8990930846fbe7c99bfdfe9ea562c75feb6e3c9122431f7c9f8b5e51a7f in / 
# Tue, 02 Aug 2022 00:42:29 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 11:36:27 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 02 Aug 2022 11:36:30 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 11:36:30 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 02 Aug 2022 11:36:42 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 02 Aug 2022 11:36:43 GMT
VOLUME [/spiped]
# Tue, 02 Aug 2022 11:36:43 GMT
WORKDIR /spiped
# Tue, 02 Aug 2022 11:36:43 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 02 Aug 2022 11:36:43 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 02 Aug 2022 11:36:43 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:026d311d0716db60eba0572ea784c21031f420960510cebcc383dc53949b4db8`  
		Last Modified: Tue, 02 Aug 2022 00:48:01 GMT  
		Size: 29.6 MB (29640259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7541e31145bcc880fcc60aff1fd1a6d96cc9bfff5e16ef0d5d327dd9497e2c1e`  
		Last Modified: Tue, 02 Aug 2022 11:37:16 GMT  
		Size: 1.7 KB (1736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd776eddcc8f7519e60d13e33bc0d710d15961af956903b4361c059231a13fb4`  
		Last Modified: Tue, 02 Aug 2022 11:37:16 GMT  
		Size: 1.1 KB (1051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bc0a264606dbae8f6555594bd36ddec88a7aa137902dd45515476c03ba153af`  
		Last Modified: Tue, 02 Aug 2022 11:37:16 GMT  
		Size: 5.2 MB (5186886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b5adf2a4c0e90db6b594339181e513b60ec0843bce0a63c90ac2330aa21bb51`  
		Last Modified: Tue, 02 Aug 2022 11:37:16 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfd03b0951b798cc22685c0158dc76558cc97d72e2f54238e5a9af5be042cbef`  
		Last Modified: Tue, 02 Aug 2022 11:37:16 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:1-alpine`

```console
$ docker pull spiped@sha256:e5d676b01e625c44b03a97f212d2e01b80e93817b2879a812d27930808ce1710
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
$ docker pull spiped@sha256:960558dde1fffd85012e80768bb5fb6b5ce16f56a6d8ba36c4eb4871b3d7ad20
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (3022913 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a4f255584cbbb67f7dca6e7842e9ba534deb82bcc7d271ddb94d37ca749d4143`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Mon, 18 Jul 2022 21:00:15 GMT
ADD file:a2648378045615c3785c752423b1afc8dc1c2b213393344f4d0ca17e7255c1cb in / 
# Mon, 18 Jul 2022 21:00:15 GMT
CMD ["/bin/sh"]
# Tue, 19 Jul 2022 02:58:44 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Tue, 19 Jul 2022 02:58:45 GMT
RUN apk add --no-cache libssl1.1
# Tue, 19 Jul 2022 02:58:45 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 19 Jul 2022 02:58:56 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Tue, 19 Jul 2022 02:58:56 GMT
VOLUME [/spiped]
# Tue, 19 Jul 2022 02:58:56 GMT
WORKDIR /spiped
# Tue, 19 Jul 2022 02:58:56 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 19 Jul 2022 02:58:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 19 Jul 2022 02:58:56 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:530afca65e2ea04227630ae746e0c85b2bd1a179379cbf2b6501b49c4cab2ccc`  
		Last Modified: Mon, 18 Jul 2022 19:09:35 GMT  
		Size: 2.8 MB (2798806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53ccfd605bd789873358dddbc12507c07697196241ef12b229daede89fede305`  
		Last Modified: Tue, 19 Jul 2022 02:59:13 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91eb30e4056e3cf1d260026125f2c0969702f9eda398caa33c77fcc1efb6da0f`  
		Last Modified: Tue, 19 Jul 2022 02:59:13 GMT  
		Size: 7.7 KB (7739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eeedfc703c38a2268ccf7afedcb792b89f9b7d7ff21f541ba671f04052a7f654`  
		Last Modified: Tue, 19 Jul 2022 02:59:13 GMT  
		Size: 214.6 KB (214629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e96340c6dfa203988333004e74c69a13274414e98de4322ea0c789ad7df42c9`  
		Last Modified: Tue, 19 Jul 2022 02:59:13 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:383211380910b0d4fcc33212392f07b13de80297232cd9da3c25f3a80b67dd34`  
		Last Modified: Tue, 19 Jul 2022 02:59:13 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; arm variant v6

```console
$ docker pull spiped@sha256:78d7c6b26405f2ccec387dbd5f5f8380bfac8922c0cde017bf83199a7c93de3f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 MB (2815244 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0975d891cb5d986fa371064357d538cff8e162c0dbcbeb412b87e765eea2bee6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Mon, 18 Jul 2022 19:49:37 GMT
ADD file:7a20333469e71664904a0cb8f61613250f2bd092b4a27bfa7bbae1dc7e21b7ed in / 
# Mon, 18 Jul 2022 19:49:37 GMT
CMD ["/bin/sh"]
# Tue, 19 Jul 2022 04:28:52 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Tue, 19 Jul 2022 04:28:54 GMT
RUN apk add --no-cache libssl1.1
# Tue, 19 Jul 2022 04:28:55 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 19 Jul 2022 04:29:15 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Tue, 19 Jul 2022 04:29:16 GMT
VOLUME [/spiped]
# Tue, 19 Jul 2022 04:29:16 GMT
WORKDIR /spiped
# Tue, 19 Jul 2022 04:29:17 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 19 Jul 2022 04:29:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 19 Jul 2022 04:29:18 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:b7885075fcd06a866d12dfd56eb704045eaadbd22dc03a224cd98715be566677`  
		Last Modified: Mon, 18 Jul 2022 19:08:42 GMT  
		Size: 2.6 MB (2606431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7794ac6005a3d1042ca428fddd078ac26956535628f13a1901b8aaf3986288d`  
		Last Modified: Tue, 19 Jul 2022 04:29:51 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0a8bbac389bb4b97ec5a6d16185ce572d9e89d45f67d819d9eee81fee855e51`  
		Last Modified: Tue, 19 Jul 2022 04:29:51 GMT  
		Size: 7.7 KB (7735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:382b8ab18f4e21efbd2668e38088fe5d0a5e016a65d8f3845cfa386c1d974999`  
		Last Modified: Tue, 19 Jul 2022 04:29:51 GMT  
		Size: 199.3 KB (199338 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:940073d33e787162c6aa336ae5ef93efdd6641a3dc59e5d4a0eb01f0c24aeecf`  
		Last Modified: Tue, 19 Jul 2022 04:29:51 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cf4811d369ed3ed91ee23a134ab53b91888e93efc80c38c6c15d44a1ec8e9de`  
		Last Modified: Tue, 19 Jul 2022 04:29:51 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; arm variant v7

```console
$ docker pull spiped@sha256:406d539553f81f86ec46ac0c9d08717c75356e6a706276e25986ea7ec4bb70df
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 MB (2614862 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ea10f25c876d7c1e28ac07d56cfd6dd1840cab98ca857fc651e9f8a5ba29e9a6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Mon, 18 Jul 2022 21:24:47 GMT
ADD file:68590e866bc6db27ad54d23de7dd275d0389cb86e4e6291a1243fcc234f2f7a1 in / 
# Mon, 18 Jul 2022 21:24:47 GMT
CMD ["/bin/sh"]
# Tue, 19 Jul 2022 09:42:16 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Tue, 19 Jul 2022 09:42:18 GMT
RUN apk add --no-cache libssl1.1
# Tue, 19 Jul 2022 09:42:19 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 19 Jul 2022 09:42:38 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Tue, 19 Jul 2022 09:42:38 GMT
VOLUME [/spiped]
# Tue, 19 Jul 2022 09:42:39 GMT
WORKDIR /spiped
# Tue, 19 Jul 2022 09:42:39 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 19 Jul 2022 09:42:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 19 Jul 2022 09:42:40 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:a6b45ace95f42a930d15c33679ab9c85d46019b7e73954cadc73bb9ba176509b`  
		Last Modified: Mon, 18 Jul 2022 19:08:56 GMT  
		Size: 2.4 MB (2412307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c22ed0b9f7779fd593471ef1630a429072a4f3bcd202ea38f6cb1627bead8e4`  
		Last Modified: Tue, 19 Jul 2022 09:43:34 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38d4163652a3ead1410becbb61a24e8f06d77f6d284534294a0bccb49bac57b8`  
		Last Modified: Tue, 19 Jul 2022 09:43:34 GMT  
		Size: 7.7 KB (7727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53df3c1757f5b854f0a5eefe967294a0d6ec49e4a5049dc712fafa9800599afc`  
		Last Modified: Tue, 19 Jul 2022 09:43:34 GMT  
		Size: 193.1 KB (193092 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1a490c5af6b8a6ec597efac4811e4ee5c156fabde11c8438da0344a492454f7`  
		Last Modified: Tue, 19 Jul 2022 09:43:34 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:191417a31477ff188751e4c9bb0754f52a807992a390563f7d84ed86683eaa30`  
		Last Modified: Tue, 19 Jul 2022 09:43:34 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:b4e4831c1382ba6191159248fbf92a052b843dd76ffb3e5ab9590a9b50033a72
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 MB (2911791 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:48fa91c14a7ba129a596b0eaffb3c321c3d4c509db24ecf103535d7fb2bd6598`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Mon, 18 Jul 2022 21:57:05 GMT
ADD file:9ccb70abba88b6de789b29f17770246f765ffbb072fe598580bfc29ce3213f1c in / 
# Mon, 18 Jul 2022 21:57:05 GMT
CMD ["/bin/sh"]
# Tue, 19 Jul 2022 03:11:40 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Tue, 19 Jul 2022 03:11:41 GMT
RUN apk add --no-cache libssl1.1
# Tue, 19 Jul 2022 03:11:42 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 19 Jul 2022 03:11:53 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Tue, 19 Jul 2022 03:11:54 GMT
VOLUME [/spiped]
# Tue, 19 Jul 2022 03:11:55 GMT
WORKDIR /spiped
# Tue, 19 Jul 2022 03:11:57 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 19 Jul 2022 03:11:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 19 Jul 2022 03:11:58 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:f97344484467e4c4ebb85aae724170073799295a3442c50ab532e249bd27b412`  
		Last Modified: Mon, 18 Jul 2022 19:08:29 GMT  
		Size: 2.7 MB (2694720 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51a8e96b71a119a7753279fa24fc1b097b559f365c0d74c928ec0827108be3ac`  
		Last Modified: Tue, 19 Jul 2022 03:12:25 GMT  
		Size: 1.2 KB (1243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef5b7ffd6e7e16898220160e758a91b7ae6e5fa7763e22b1f929570b0e877432`  
		Last Modified: Tue, 19 Jul 2022 03:12:25 GMT  
		Size: 7.7 KB (7708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54764cd29a52b45365923ab1e756750d07330c69ea57b318f8f4b2660940a1fa`  
		Last Modified: Tue, 19 Jul 2022 03:12:25 GMT  
		Size: 207.7 KB (207685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a2841c7d2c1268e60c21c01e69c10868bef688cc32f57dbe883e975040d003f`  
		Last Modified: Tue, 19 Jul 2022 03:12:25 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b456f54f4f08db25a2b70f3ecd5b9a2273937e824ae2e3d919c7f3d8b31102a2`  
		Last Modified: Tue, 19 Jul 2022 03:12:25 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; 386

```console
$ docker pull spiped@sha256:bd3d4904f8e1d52ce4a28eb847bc57f54248490fc15e9ac6e88cca4566f2bbec
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (3036863 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:abc7cf0e554fe461e7d95534758c990b4c5f507ac6912d08de0ab5c7192d5a4b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Mon, 18 Jul 2022 20:38:19 GMT
ADD file:be69b7550bf861d8fb12bdbe1edf3a0d2519a6a4da61bd04858b6258ffbf48a7 in / 
# Mon, 18 Jul 2022 20:38:19 GMT
CMD ["/bin/sh"]
# Tue, 19 Jul 2022 00:52:10 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Tue, 19 Jul 2022 00:52:11 GMT
RUN apk add --no-cache libssl1.1
# Tue, 19 Jul 2022 00:52:12 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 19 Jul 2022 00:52:24 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Tue, 19 Jul 2022 00:52:25 GMT
VOLUME [/spiped]
# Tue, 19 Jul 2022 00:52:26 GMT
WORKDIR /spiped
# Tue, 19 Jul 2022 00:52:28 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 19 Jul 2022 00:52:28 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 19 Jul 2022 00:52:29 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:5d7f927419794ebb7496ac38b0659686317b2d2fac7252a4a0d40d43d5fdd662`  
		Last Modified: Mon, 18 Jul 2022 19:09:22 GMT  
		Size: 2.8 MB (2802334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8be475f4c97c2b6a50a82b2cda5d04dcf3be627667431e283146f5ef2467cf2`  
		Last Modified: Tue, 19 Jul 2022 00:52:57 GMT  
		Size: 1.2 KB (1243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ccf382b13c23a3fe33bbd2b36efca3ac3493d37bbda16a50f5df1a18b997e00`  
		Last Modified: Tue, 19 Jul 2022 00:52:57 GMT  
		Size: 7.7 KB (7711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb7cd3baa7c17abca3fa3c456474f8fe1b0aa45d19cba81de21b85554722608e`  
		Last Modified: Tue, 19 Jul 2022 00:52:58 GMT  
		Size: 225.1 KB (225138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a1a6c9df0a41f62802eec16036b66a1513b5b158004c13839da1b3ba266ac38`  
		Last Modified: Tue, 19 Jul 2022 00:52:57 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16f06336cb65e863eccc316001a0037fbb6fc5dd05ff03301c9a513d42af9128`  
		Last Modified: Tue, 19 Jul 2022 00:52:58 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; ppc64le

```console
$ docker pull spiped@sha256:f9db2c66d081de674f9c2b6be02eded176cb2fdbe2ed251d040663111d8d765f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (3013087 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:64a91098c0d88cb338eb43ccb20d859d67efe05df38a850d2b645a1f3aa26c5c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Mon, 18 Jul 2022 21:29:30 GMT
ADD file:69e4080f15f54e2d8f8aa25fdcba9c01dde149d43592edd5023106675e54a769 in / 
# Mon, 18 Jul 2022 21:29:31 GMT
CMD ["/bin/sh"]
# Tue, 19 Jul 2022 07:44:52 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Tue, 19 Jul 2022 07:45:01 GMT
RUN apk add --no-cache libssl1.1
# Tue, 19 Jul 2022 07:45:03 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 19 Jul 2022 07:45:21 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Tue, 19 Jul 2022 07:45:23 GMT
VOLUME [/spiped]
# Tue, 19 Jul 2022 07:45:25 GMT
WORKDIR /spiped
# Tue, 19 Jul 2022 07:45:28 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 19 Jul 2022 07:45:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 19 Jul 2022 07:45:36 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:602896d442490cd3fbb6599f0f862d3673b7cd58eca3ac842b8e09bf8d012443`  
		Last Modified: Mon, 18 Jul 2022 19:09:09 GMT  
		Size: 2.8 MB (2789923 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:625e385ac9fcd0da39e5754ecac93c3230b8a4b0b5f6f466f5df607a9f76dd58`  
		Last Modified: Tue, 19 Jul 2022 07:46:14 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae1de895bed2f7ec17e8fccb9e6d944457809f1e9fc22e7c1a8b52a630caf1c3`  
		Last Modified: Tue, 19 Jul 2022 07:46:14 GMT  
		Size: 7.7 KB (7734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5828466d70a99b3e62cd1f6cbbe9ce7bf47fecfefbc3a91eecdb80647c749856`  
		Last Modified: Tue, 19 Jul 2022 07:46:14 GMT  
		Size: 213.7 KB (213691 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee54a465cd2b488f11e4e693d68d679ec15b3c5b1c88679f87a485b200f94160`  
		Last Modified: Tue, 19 Jul 2022 07:46:14 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3c9a834c167df5b7cf9265a0390b7e6c81bf076f8b0b9d3b848ddb02c9cf8ff`  
		Last Modified: Tue, 19 Jul 2022 07:46:14 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; s390x

```console
$ docker pull spiped@sha256:5abc9d546636b6670ca2c300303d57c59e066f9b42af71ffc12fce775274b2b8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 MB (2792283 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dc9891884c555841cd06fd9c1a3608fcb75e6ab6cdb389c07e53fed03b6bb500`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Mon, 18 Jul 2022 20:41:35 GMT
ADD file:deaa573cd61e07709846a5300fb627a8610e9754129c085ed483ff8897d0c002 in / 
# Mon, 18 Jul 2022 20:41:36 GMT
CMD ["/bin/sh"]
# Tue, 19 Jul 2022 05:40:59 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Tue, 19 Jul 2022 05:41:01 GMT
RUN apk add --no-cache libssl1.1
# Tue, 19 Jul 2022 05:41:02 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 19 Jul 2022 05:41:11 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Tue, 19 Jul 2022 05:41:11 GMT
VOLUME [/spiped]
# Tue, 19 Jul 2022 05:41:12 GMT
WORKDIR /spiped
# Tue, 19 Jul 2022 05:41:13 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 19 Jul 2022 05:41:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 19 Jul 2022 05:41:13 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:5f1840d5bacf4162a87f497e22d94bce946e660bdfce8eeefcbf7bd0beb193f3`  
		Last Modified: Mon, 18 Jul 2022 20:42:36 GMT  
		Size: 2.6 MB (2580798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd6993821da2e7957193713709542cca3a229ed17d3d859ca823a7ef4e38b011`  
		Last Modified: Tue, 19 Jul 2022 05:41:47 GMT  
		Size: 1.3 KB (1266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09df37c5f8ac9a24ba5f55d4d545b4835141a55e5f9ecd71f8b936809f8fddd3`  
		Last Modified: Tue, 19 Jul 2022 05:41:47 GMT  
		Size: 7.7 KB (7742 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9c64cd2f7e97c8f03ec8ef34a7ba77e455842217cfcc3e9c6816f56ea8108b6`  
		Last Modified: Tue, 19 Jul 2022 05:41:47 GMT  
		Size: 202.0 KB (202009 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3ec9f775174ce04ae9cf626a975e42a1f50926f1d9f9cdecf513cdb1514809b`  
		Last Modified: Tue, 19 Jul 2022 05:41:47 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41b76904392c2be02eeefc2c55db23094f8f3578806838b317aec9d39ec86abd`  
		Last Modified: Tue, 19 Jul 2022 05:41:47 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:1.6`

```console
$ docker pull spiped@sha256:893b1d34151bff6fc3b147f4492989c25976f4c5bd2b714b7872c22ddcf32453
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
$ docker pull spiped@sha256:f83b419d27348b2bdbf4d6e78da6d2e62f75d514a1ed39855e1899dc9b59fe73
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.3 MB (31312141 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:524e3e7d21e31be2a48e1548d86d5ced3a2ee4185440b47edacceca48ca97031`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 12 Jul 2022 00:59:54 GMT
ADD file:ae890621b36ff6e27364bb7316b5bd4319a820ddf7e65565c6201eb11d70fde9 in / 
# Tue, 12 Jul 2022 00:59:55 GMT
CMD ["bash"]
# Wed, 13 Jul 2022 07:57:44 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 13 Jul 2022 07:57:51 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 13 Jul 2022 07:57:52 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 13 Jul 2022 07:58:36 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 13 Jul 2022 07:58:37 GMT
VOLUME [/spiped]
# Wed, 13 Jul 2022 07:58:37 GMT
WORKDIR /spiped
# Wed, 13 Jul 2022 07:58:38 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 13 Jul 2022 07:58:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 13 Jul 2022 07:58:39 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:314cda9d0ef2282082d2bd0efd7659e0d9edb3ceae8e7919d990bcf95cbb3d2b`  
		Last Modified: Tue, 12 Jul 2022 01:12:37 GMT  
		Size: 26.6 MB (26560559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:090471f791b0f328f3661d50b9ff593c83c6e102cdb08df2fd72cecb662ff0be`  
		Last Modified: Wed, 13 Jul 2022 07:59:38 GMT  
		Size: 1.7 KB (1727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c4dfc160206772b3b1e6340d5d682c20ec1e14e0871426b46711d58b7d6833c`  
		Last Modified: Wed, 13 Jul 2022 07:59:38 GMT  
		Size: 1.1 KB (1053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89bb0f704911b77275d75f7bc8b4cf0b5162ade51f380f463c6cc820cac6968d`  
		Last Modified: Wed, 13 Jul 2022 07:59:42 GMT  
		Size: 4.7 MB (4748333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5b67ae8b1bcc4511eeadde14a66ebab56c086d30f91559679a64b68b73fc76a`  
		Last Modified: Wed, 13 Jul 2022 07:59:38 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:630225b9ddc0c86154ca5f1fa26d05def1293638c2be832017738f83eadd93a3`  
		Last Modified: Wed, 13 Jul 2022 07:59:38 GMT  
		Size: 342.0 B  
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
$ docker pull spiped@sha256:0912dd64711f962ed20b280e96cc372e615b95b97ee1aa6a9056ba1f36a9f4cc
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.3 MB (35337184 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:40302e59e0dfc3ac7483cdda59a1917781d6bf1697c399cd8718d32fc20b3ab8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 12 Jul 2022 04:40:59 GMT
ADD file:e0c3a3f07bbd2b798f2f620e295566d0b49142660f897083f73164c0356f37a2 in / 
# Tue, 12 Jul 2022 04:41:04 GMT
CMD ["bash"]
# Wed, 13 Jul 2022 10:54:04 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 13 Jul 2022 10:54:19 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 13 Jul 2022 10:54:21 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 13 Jul 2022 10:55:53 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 13 Jul 2022 10:55:55 GMT
VOLUME [/spiped]
# Wed, 13 Jul 2022 10:55:58 GMT
WORKDIR /spiped
# Wed, 13 Jul 2022 10:56:00 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 13 Jul 2022 10:56:03 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 13 Jul 2022 10:56:06 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:88869778ecefe05f3e79ed90f3c06c22dfef4c56919a454f67eba47fb8072189`  
		Last Modified: Tue, 12 Jul 2022 04:51:44 GMT  
		Size: 29.6 MB (29628932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8dce35712b9df24fe23728e831a2d450572f507f476fca4f37b578b13c0f258f`  
		Last Modified: Wed, 13 Jul 2022 10:56:20 GMT  
		Size: 1.6 KB (1619 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78bf32252f913a3a579a40ec4538d9f0a46238b5bf83d6660c4967cca14df32a`  
		Last Modified: Wed, 13 Jul 2022 10:56:20 GMT  
		Size: 922.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:895648de55366c4420ab371cebceab082edcb43321c746dc76fb385c47594187`  
		Last Modified: Wed, 13 Jul 2022 10:56:26 GMT  
		Size: 5.7 MB (5705273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:918d7dc0f0ce53174644562b626a49d277285fa8c4ea2bcc0acc8efc1e63f7f6`  
		Last Modified: Wed, 13 Jul 2022 10:56:20 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1777ed1e7ecf5154695c61e242216358df92c1b5d2cef0c91e5b19b3b500b7c9`  
		Last Modified: Wed, 13 Jul 2022 10:56:20 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; ppc64le

```console
$ docker pull spiped@sha256:81003cf3de708c1d144d9355412aec5bdf2094c49b740cb388711db570b4356f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.3 MB (41275059 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4406e24e415436179ca82b111445f95864a4f68270845d8f13f8f6738e6dd613`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 12 Jul 2022 01:25:28 GMT
ADD file:9e1afe48f40d94f879aefb12a7e68da2f0772d701e95b8219bd1f79a83e1933a in / 
# Tue, 12 Jul 2022 01:25:32 GMT
CMD ["bash"]
# Wed, 13 Jul 2022 06:43:01 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 13 Jul 2022 06:43:12 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 13 Jul 2022 06:43:14 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 13 Jul 2022 06:45:53 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 13 Jul 2022 06:45:55 GMT
VOLUME [/spiped]
# Wed, 13 Jul 2022 06:45:59 GMT
WORKDIR /spiped
# Wed, 13 Jul 2022 06:46:01 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 13 Jul 2022 06:46:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 13 Jul 2022 06:46:06 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:bd3d68d1ce583727f6378a16916795b955cc0ad39e0ebe754a26007ef54744fa`  
		Last Modified: Tue, 12 Jul 2022 01:36:03 GMT  
		Size: 35.3 MB (35272500 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9118819a47938b959974a2c187124c206d412a4381b1fa00b07702644095ac5d`  
		Last Modified: Wed, 13 Jul 2022 06:46:45 GMT  
		Size: 1.7 KB (1730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:387914e121edf896abe5847d4c111ed304f65ba32e283e8c551636e0603f325c`  
		Last Modified: Wed, 13 Jul 2022 06:46:45 GMT  
		Size: 1.1 KB (1053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bbc4a7edac4c6f551075397bc114c02da11b03ddf357cadb338265a627754b4`  
		Last Modified: Wed, 13 Jul 2022 06:46:46 GMT  
		Size: 6.0 MB (5999305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:773d9584db6f6fede768ee1493062d61d3061585c34a2d6716802a94dcf16103`  
		Last Modified: Wed, 13 Jul 2022 06:46:45 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e83ac10baec3d66ad682bc3eefbc4b8d96730fafcf154ef2da09edeb47bb1f7b`  
		Last Modified: Wed, 13 Jul 2022 06:46:45 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; s390x

```console
$ docker pull spiped@sha256:7bf397f297d1ea78dd655acc6c96775a5343e89423693de15ff17f08a7e69fda
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.8 MB (34830403 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3d0f9f2ec0119a2ccfd6b0ef28575b5bc407594263c24f89aa33495fe897631e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 02 Aug 2022 00:42:27 GMT
ADD file:c2afc8990930846fbe7c99bfdfe9ea562c75feb6e3c9122431f7c9f8b5e51a7f in / 
# Tue, 02 Aug 2022 00:42:29 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 11:36:27 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 02 Aug 2022 11:36:30 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 11:36:30 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 02 Aug 2022 11:36:42 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 02 Aug 2022 11:36:43 GMT
VOLUME [/spiped]
# Tue, 02 Aug 2022 11:36:43 GMT
WORKDIR /spiped
# Tue, 02 Aug 2022 11:36:43 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 02 Aug 2022 11:36:43 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 02 Aug 2022 11:36:43 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:026d311d0716db60eba0572ea784c21031f420960510cebcc383dc53949b4db8`  
		Last Modified: Tue, 02 Aug 2022 00:48:01 GMT  
		Size: 29.6 MB (29640259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7541e31145bcc880fcc60aff1fd1a6d96cc9bfff5e16ef0d5d327dd9497e2c1e`  
		Last Modified: Tue, 02 Aug 2022 11:37:16 GMT  
		Size: 1.7 KB (1736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd776eddcc8f7519e60d13e33bc0d710d15961af956903b4361c059231a13fb4`  
		Last Modified: Tue, 02 Aug 2022 11:37:16 GMT  
		Size: 1.1 KB (1051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bc0a264606dbae8f6555594bd36ddec88a7aa137902dd45515476c03ba153af`  
		Last Modified: Tue, 02 Aug 2022 11:37:16 GMT  
		Size: 5.2 MB (5186886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b5adf2a4c0e90db6b594339181e513b60ec0843bce0a63c90ac2330aa21bb51`  
		Last Modified: Tue, 02 Aug 2022 11:37:16 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfd03b0951b798cc22685c0158dc76558cc97d72e2f54238e5a9af5be042cbef`  
		Last Modified: Tue, 02 Aug 2022 11:37:16 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:1.6-alpine`

```console
$ docker pull spiped@sha256:e5d676b01e625c44b03a97f212d2e01b80e93817b2879a812d27930808ce1710
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
$ docker pull spiped@sha256:960558dde1fffd85012e80768bb5fb6b5ce16f56a6d8ba36c4eb4871b3d7ad20
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (3022913 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a4f255584cbbb67f7dca6e7842e9ba534deb82bcc7d271ddb94d37ca749d4143`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Mon, 18 Jul 2022 21:00:15 GMT
ADD file:a2648378045615c3785c752423b1afc8dc1c2b213393344f4d0ca17e7255c1cb in / 
# Mon, 18 Jul 2022 21:00:15 GMT
CMD ["/bin/sh"]
# Tue, 19 Jul 2022 02:58:44 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Tue, 19 Jul 2022 02:58:45 GMT
RUN apk add --no-cache libssl1.1
# Tue, 19 Jul 2022 02:58:45 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 19 Jul 2022 02:58:56 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Tue, 19 Jul 2022 02:58:56 GMT
VOLUME [/spiped]
# Tue, 19 Jul 2022 02:58:56 GMT
WORKDIR /spiped
# Tue, 19 Jul 2022 02:58:56 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 19 Jul 2022 02:58:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 19 Jul 2022 02:58:56 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:530afca65e2ea04227630ae746e0c85b2bd1a179379cbf2b6501b49c4cab2ccc`  
		Last Modified: Mon, 18 Jul 2022 19:09:35 GMT  
		Size: 2.8 MB (2798806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53ccfd605bd789873358dddbc12507c07697196241ef12b229daede89fede305`  
		Last Modified: Tue, 19 Jul 2022 02:59:13 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91eb30e4056e3cf1d260026125f2c0969702f9eda398caa33c77fcc1efb6da0f`  
		Last Modified: Tue, 19 Jul 2022 02:59:13 GMT  
		Size: 7.7 KB (7739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eeedfc703c38a2268ccf7afedcb792b89f9b7d7ff21f541ba671f04052a7f654`  
		Last Modified: Tue, 19 Jul 2022 02:59:13 GMT  
		Size: 214.6 KB (214629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e96340c6dfa203988333004e74c69a13274414e98de4322ea0c789ad7df42c9`  
		Last Modified: Tue, 19 Jul 2022 02:59:13 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:383211380910b0d4fcc33212392f07b13de80297232cd9da3c25f3a80b67dd34`  
		Last Modified: Tue, 19 Jul 2022 02:59:13 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; arm variant v6

```console
$ docker pull spiped@sha256:78d7c6b26405f2ccec387dbd5f5f8380bfac8922c0cde017bf83199a7c93de3f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 MB (2815244 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0975d891cb5d986fa371064357d538cff8e162c0dbcbeb412b87e765eea2bee6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Mon, 18 Jul 2022 19:49:37 GMT
ADD file:7a20333469e71664904a0cb8f61613250f2bd092b4a27bfa7bbae1dc7e21b7ed in / 
# Mon, 18 Jul 2022 19:49:37 GMT
CMD ["/bin/sh"]
# Tue, 19 Jul 2022 04:28:52 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Tue, 19 Jul 2022 04:28:54 GMT
RUN apk add --no-cache libssl1.1
# Tue, 19 Jul 2022 04:28:55 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 19 Jul 2022 04:29:15 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Tue, 19 Jul 2022 04:29:16 GMT
VOLUME [/spiped]
# Tue, 19 Jul 2022 04:29:16 GMT
WORKDIR /spiped
# Tue, 19 Jul 2022 04:29:17 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 19 Jul 2022 04:29:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 19 Jul 2022 04:29:18 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:b7885075fcd06a866d12dfd56eb704045eaadbd22dc03a224cd98715be566677`  
		Last Modified: Mon, 18 Jul 2022 19:08:42 GMT  
		Size: 2.6 MB (2606431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7794ac6005a3d1042ca428fddd078ac26956535628f13a1901b8aaf3986288d`  
		Last Modified: Tue, 19 Jul 2022 04:29:51 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0a8bbac389bb4b97ec5a6d16185ce572d9e89d45f67d819d9eee81fee855e51`  
		Last Modified: Tue, 19 Jul 2022 04:29:51 GMT  
		Size: 7.7 KB (7735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:382b8ab18f4e21efbd2668e38088fe5d0a5e016a65d8f3845cfa386c1d974999`  
		Last Modified: Tue, 19 Jul 2022 04:29:51 GMT  
		Size: 199.3 KB (199338 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:940073d33e787162c6aa336ae5ef93efdd6641a3dc59e5d4a0eb01f0c24aeecf`  
		Last Modified: Tue, 19 Jul 2022 04:29:51 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cf4811d369ed3ed91ee23a134ab53b91888e93efc80c38c6c15d44a1ec8e9de`  
		Last Modified: Tue, 19 Jul 2022 04:29:51 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; arm variant v7

```console
$ docker pull spiped@sha256:406d539553f81f86ec46ac0c9d08717c75356e6a706276e25986ea7ec4bb70df
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 MB (2614862 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ea10f25c876d7c1e28ac07d56cfd6dd1840cab98ca857fc651e9f8a5ba29e9a6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Mon, 18 Jul 2022 21:24:47 GMT
ADD file:68590e866bc6db27ad54d23de7dd275d0389cb86e4e6291a1243fcc234f2f7a1 in / 
# Mon, 18 Jul 2022 21:24:47 GMT
CMD ["/bin/sh"]
# Tue, 19 Jul 2022 09:42:16 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Tue, 19 Jul 2022 09:42:18 GMT
RUN apk add --no-cache libssl1.1
# Tue, 19 Jul 2022 09:42:19 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 19 Jul 2022 09:42:38 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Tue, 19 Jul 2022 09:42:38 GMT
VOLUME [/spiped]
# Tue, 19 Jul 2022 09:42:39 GMT
WORKDIR /spiped
# Tue, 19 Jul 2022 09:42:39 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 19 Jul 2022 09:42:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 19 Jul 2022 09:42:40 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:a6b45ace95f42a930d15c33679ab9c85d46019b7e73954cadc73bb9ba176509b`  
		Last Modified: Mon, 18 Jul 2022 19:08:56 GMT  
		Size: 2.4 MB (2412307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c22ed0b9f7779fd593471ef1630a429072a4f3bcd202ea38f6cb1627bead8e4`  
		Last Modified: Tue, 19 Jul 2022 09:43:34 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38d4163652a3ead1410becbb61a24e8f06d77f6d284534294a0bccb49bac57b8`  
		Last Modified: Tue, 19 Jul 2022 09:43:34 GMT  
		Size: 7.7 KB (7727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53df3c1757f5b854f0a5eefe967294a0d6ec49e4a5049dc712fafa9800599afc`  
		Last Modified: Tue, 19 Jul 2022 09:43:34 GMT  
		Size: 193.1 KB (193092 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1a490c5af6b8a6ec597efac4811e4ee5c156fabde11c8438da0344a492454f7`  
		Last Modified: Tue, 19 Jul 2022 09:43:34 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:191417a31477ff188751e4c9bb0754f52a807992a390563f7d84ed86683eaa30`  
		Last Modified: Tue, 19 Jul 2022 09:43:34 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:b4e4831c1382ba6191159248fbf92a052b843dd76ffb3e5ab9590a9b50033a72
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 MB (2911791 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:48fa91c14a7ba129a596b0eaffb3c321c3d4c509db24ecf103535d7fb2bd6598`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Mon, 18 Jul 2022 21:57:05 GMT
ADD file:9ccb70abba88b6de789b29f17770246f765ffbb072fe598580bfc29ce3213f1c in / 
# Mon, 18 Jul 2022 21:57:05 GMT
CMD ["/bin/sh"]
# Tue, 19 Jul 2022 03:11:40 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Tue, 19 Jul 2022 03:11:41 GMT
RUN apk add --no-cache libssl1.1
# Tue, 19 Jul 2022 03:11:42 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 19 Jul 2022 03:11:53 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Tue, 19 Jul 2022 03:11:54 GMT
VOLUME [/spiped]
# Tue, 19 Jul 2022 03:11:55 GMT
WORKDIR /spiped
# Tue, 19 Jul 2022 03:11:57 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 19 Jul 2022 03:11:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 19 Jul 2022 03:11:58 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:f97344484467e4c4ebb85aae724170073799295a3442c50ab532e249bd27b412`  
		Last Modified: Mon, 18 Jul 2022 19:08:29 GMT  
		Size: 2.7 MB (2694720 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51a8e96b71a119a7753279fa24fc1b097b559f365c0d74c928ec0827108be3ac`  
		Last Modified: Tue, 19 Jul 2022 03:12:25 GMT  
		Size: 1.2 KB (1243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef5b7ffd6e7e16898220160e758a91b7ae6e5fa7763e22b1f929570b0e877432`  
		Last Modified: Tue, 19 Jul 2022 03:12:25 GMT  
		Size: 7.7 KB (7708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54764cd29a52b45365923ab1e756750d07330c69ea57b318f8f4b2660940a1fa`  
		Last Modified: Tue, 19 Jul 2022 03:12:25 GMT  
		Size: 207.7 KB (207685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a2841c7d2c1268e60c21c01e69c10868bef688cc32f57dbe883e975040d003f`  
		Last Modified: Tue, 19 Jul 2022 03:12:25 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b456f54f4f08db25a2b70f3ecd5b9a2273937e824ae2e3d919c7f3d8b31102a2`  
		Last Modified: Tue, 19 Jul 2022 03:12:25 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; 386

```console
$ docker pull spiped@sha256:bd3d4904f8e1d52ce4a28eb847bc57f54248490fc15e9ac6e88cca4566f2bbec
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (3036863 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:abc7cf0e554fe461e7d95534758c990b4c5f507ac6912d08de0ab5c7192d5a4b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Mon, 18 Jul 2022 20:38:19 GMT
ADD file:be69b7550bf861d8fb12bdbe1edf3a0d2519a6a4da61bd04858b6258ffbf48a7 in / 
# Mon, 18 Jul 2022 20:38:19 GMT
CMD ["/bin/sh"]
# Tue, 19 Jul 2022 00:52:10 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Tue, 19 Jul 2022 00:52:11 GMT
RUN apk add --no-cache libssl1.1
# Tue, 19 Jul 2022 00:52:12 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 19 Jul 2022 00:52:24 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Tue, 19 Jul 2022 00:52:25 GMT
VOLUME [/spiped]
# Tue, 19 Jul 2022 00:52:26 GMT
WORKDIR /spiped
# Tue, 19 Jul 2022 00:52:28 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 19 Jul 2022 00:52:28 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 19 Jul 2022 00:52:29 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:5d7f927419794ebb7496ac38b0659686317b2d2fac7252a4a0d40d43d5fdd662`  
		Last Modified: Mon, 18 Jul 2022 19:09:22 GMT  
		Size: 2.8 MB (2802334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8be475f4c97c2b6a50a82b2cda5d04dcf3be627667431e283146f5ef2467cf2`  
		Last Modified: Tue, 19 Jul 2022 00:52:57 GMT  
		Size: 1.2 KB (1243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ccf382b13c23a3fe33bbd2b36efca3ac3493d37bbda16a50f5df1a18b997e00`  
		Last Modified: Tue, 19 Jul 2022 00:52:57 GMT  
		Size: 7.7 KB (7711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb7cd3baa7c17abca3fa3c456474f8fe1b0aa45d19cba81de21b85554722608e`  
		Last Modified: Tue, 19 Jul 2022 00:52:58 GMT  
		Size: 225.1 KB (225138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a1a6c9df0a41f62802eec16036b66a1513b5b158004c13839da1b3ba266ac38`  
		Last Modified: Tue, 19 Jul 2022 00:52:57 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16f06336cb65e863eccc316001a0037fbb6fc5dd05ff03301c9a513d42af9128`  
		Last Modified: Tue, 19 Jul 2022 00:52:58 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; ppc64le

```console
$ docker pull spiped@sha256:f9db2c66d081de674f9c2b6be02eded176cb2fdbe2ed251d040663111d8d765f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (3013087 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:64a91098c0d88cb338eb43ccb20d859d67efe05df38a850d2b645a1f3aa26c5c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Mon, 18 Jul 2022 21:29:30 GMT
ADD file:69e4080f15f54e2d8f8aa25fdcba9c01dde149d43592edd5023106675e54a769 in / 
# Mon, 18 Jul 2022 21:29:31 GMT
CMD ["/bin/sh"]
# Tue, 19 Jul 2022 07:44:52 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Tue, 19 Jul 2022 07:45:01 GMT
RUN apk add --no-cache libssl1.1
# Tue, 19 Jul 2022 07:45:03 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 19 Jul 2022 07:45:21 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Tue, 19 Jul 2022 07:45:23 GMT
VOLUME [/spiped]
# Tue, 19 Jul 2022 07:45:25 GMT
WORKDIR /spiped
# Tue, 19 Jul 2022 07:45:28 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 19 Jul 2022 07:45:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 19 Jul 2022 07:45:36 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:602896d442490cd3fbb6599f0f862d3673b7cd58eca3ac842b8e09bf8d012443`  
		Last Modified: Mon, 18 Jul 2022 19:09:09 GMT  
		Size: 2.8 MB (2789923 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:625e385ac9fcd0da39e5754ecac93c3230b8a4b0b5f6f466f5df607a9f76dd58`  
		Last Modified: Tue, 19 Jul 2022 07:46:14 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae1de895bed2f7ec17e8fccb9e6d944457809f1e9fc22e7c1a8b52a630caf1c3`  
		Last Modified: Tue, 19 Jul 2022 07:46:14 GMT  
		Size: 7.7 KB (7734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5828466d70a99b3e62cd1f6cbbe9ce7bf47fecfefbc3a91eecdb80647c749856`  
		Last Modified: Tue, 19 Jul 2022 07:46:14 GMT  
		Size: 213.7 KB (213691 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee54a465cd2b488f11e4e693d68d679ec15b3c5b1c88679f87a485b200f94160`  
		Last Modified: Tue, 19 Jul 2022 07:46:14 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3c9a834c167df5b7cf9265a0390b7e6c81bf076f8b0b9d3b848ddb02c9cf8ff`  
		Last Modified: Tue, 19 Jul 2022 07:46:14 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; s390x

```console
$ docker pull spiped@sha256:5abc9d546636b6670ca2c300303d57c59e066f9b42af71ffc12fce775274b2b8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 MB (2792283 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dc9891884c555841cd06fd9c1a3608fcb75e6ab6cdb389c07e53fed03b6bb500`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Mon, 18 Jul 2022 20:41:35 GMT
ADD file:deaa573cd61e07709846a5300fb627a8610e9754129c085ed483ff8897d0c002 in / 
# Mon, 18 Jul 2022 20:41:36 GMT
CMD ["/bin/sh"]
# Tue, 19 Jul 2022 05:40:59 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Tue, 19 Jul 2022 05:41:01 GMT
RUN apk add --no-cache libssl1.1
# Tue, 19 Jul 2022 05:41:02 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 19 Jul 2022 05:41:11 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Tue, 19 Jul 2022 05:41:11 GMT
VOLUME [/spiped]
# Tue, 19 Jul 2022 05:41:12 GMT
WORKDIR /spiped
# Tue, 19 Jul 2022 05:41:13 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 19 Jul 2022 05:41:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 19 Jul 2022 05:41:13 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:5f1840d5bacf4162a87f497e22d94bce946e660bdfce8eeefcbf7bd0beb193f3`  
		Last Modified: Mon, 18 Jul 2022 20:42:36 GMT  
		Size: 2.6 MB (2580798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd6993821da2e7957193713709542cca3a229ed17d3d859ca823a7ef4e38b011`  
		Last Modified: Tue, 19 Jul 2022 05:41:47 GMT  
		Size: 1.3 KB (1266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09df37c5f8ac9a24ba5f55d4d545b4835141a55e5f9ecd71f8b936809f8fddd3`  
		Last Modified: Tue, 19 Jul 2022 05:41:47 GMT  
		Size: 7.7 KB (7742 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9c64cd2f7e97c8f03ec8ef34a7ba77e455842217cfcc3e9c6816f56ea8108b6`  
		Last Modified: Tue, 19 Jul 2022 05:41:47 GMT  
		Size: 202.0 KB (202009 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3ec9f775174ce04ae9cf626a975e42a1f50926f1d9f9cdecf513cdb1514809b`  
		Last Modified: Tue, 19 Jul 2022 05:41:47 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41b76904392c2be02eeefc2c55db23094f8f3578806838b317aec9d39ec86abd`  
		Last Modified: Tue, 19 Jul 2022 05:41:47 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:1.6.2`

```console
$ docker pull spiped@sha256:893b1d34151bff6fc3b147f4492989c25976f4c5bd2b714b7872c22ddcf32453
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
$ docker pull spiped@sha256:f83b419d27348b2bdbf4d6e78da6d2e62f75d514a1ed39855e1899dc9b59fe73
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.3 MB (31312141 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:524e3e7d21e31be2a48e1548d86d5ced3a2ee4185440b47edacceca48ca97031`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 12 Jul 2022 00:59:54 GMT
ADD file:ae890621b36ff6e27364bb7316b5bd4319a820ddf7e65565c6201eb11d70fde9 in / 
# Tue, 12 Jul 2022 00:59:55 GMT
CMD ["bash"]
# Wed, 13 Jul 2022 07:57:44 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 13 Jul 2022 07:57:51 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 13 Jul 2022 07:57:52 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 13 Jul 2022 07:58:36 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 13 Jul 2022 07:58:37 GMT
VOLUME [/spiped]
# Wed, 13 Jul 2022 07:58:37 GMT
WORKDIR /spiped
# Wed, 13 Jul 2022 07:58:38 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 13 Jul 2022 07:58:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 13 Jul 2022 07:58:39 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:314cda9d0ef2282082d2bd0efd7659e0d9edb3ceae8e7919d990bcf95cbb3d2b`  
		Last Modified: Tue, 12 Jul 2022 01:12:37 GMT  
		Size: 26.6 MB (26560559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:090471f791b0f328f3661d50b9ff593c83c6e102cdb08df2fd72cecb662ff0be`  
		Last Modified: Wed, 13 Jul 2022 07:59:38 GMT  
		Size: 1.7 KB (1727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c4dfc160206772b3b1e6340d5d682c20ec1e14e0871426b46711d58b7d6833c`  
		Last Modified: Wed, 13 Jul 2022 07:59:38 GMT  
		Size: 1.1 KB (1053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89bb0f704911b77275d75f7bc8b4cf0b5162ade51f380f463c6cc820cac6968d`  
		Last Modified: Wed, 13 Jul 2022 07:59:42 GMT  
		Size: 4.7 MB (4748333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5b67ae8b1bcc4511eeadde14a66ebab56c086d30f91559679a64b68b73fc76a`  
		Last Modified: Wed, 13 Jul 2022 07:59:38 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:630225b9ddc0c86154ca5f1fa26d05def1293638c2be832017738f83eadd93a3`  
		Last Modified: Wed, 13 Jul 2022 07:59:38 GMT  
		Size: 342.0 B  
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
$ docker pull spiped@sha256:0912dd64711f962ed20b280e96cc372e615b95b97ee1aa6a9056ba1f36a9f4cc
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.3 MB (35337184 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:40302e59e0dfc3ac7483cdda59a1917781d6bf1697c399cd8718d32fc20b3ab8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 12 Jul 2022 04:40:59 GMT
ADD file:e0c3a3f07bbd2b798f2f620e295566d0b49142660f897083f73164c0356f37a2 in / 
# Tue, 12 Jul 2022 04:41:04 GMT
CMD ["bash"]
# Wed, 13 Jul 2022 10:54:04 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 13 Jul 2022 10:54:19 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 13 Jul 2022 10:54:21 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 13 Jul 2022 10:55:53 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 13 Jul 2022 10:55:55 GMT
VOLUME [/spiped]
# Wed, 13 Jul 2022 10:55:58 GMT
WORKDIR /spiped
# Wed, 13 Jul 2022 10:56:00 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 13 Jul 2022 10:56:03 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 13 Jul 2022 10:56:06 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:88869778ecefe05f3e79ed90f3c06c22dfef4c56919a454f67eba47fb8072189`  
		Last Modified: Tue, 12 Jul 2022 04:51:44 GMT  
		Size: 29.6 MB (29628932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8dce35712b9df24fe23728e831a2d450572f507f476fca4f37b578b13c0f258f`  
		Last Modified: Wed, 13 Jul 2022 10:56:20 GMT  
		Size: 1.6 KB (1619 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78bf32252f913a3a579a40ec4538d9f0a46238b5bf83d6660c4967cca14df32a`  
		Last Modified: Wed, 13 Jul 2022 10:56:20 GMT  
		Size: 922.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:895648de55366c4420ab371cebceab082edcb43321c746dc76fb385c47594187`  
		Last Modified: Wed, 13 Jul 2022 10:56:26 GMT  
		Size: 5.7 MB (5705273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:918d7dc0f0ce53174644562b626a49d277285fa8c4ea2bcc0acc8efc1e63f7f6`  
		Last Modified: Wed, 13 Jul 2022 10:56:20 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1777ed1e7ecf5154695c61e242216358df92c1b5d2cef0c91e5b19b3b500b7c9`  
		Last Modified: Wed, 13 Jul 2022 10:56:20 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.2` - linux; ppc64le

```console
$ docker pull spiped@sha256:81003cf3de708c1d144d9355412aec5bdf2094c49b740cb388711db570b4356f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.3 MB (41275059 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4406e24e415436179ca82b111445f95864a4f68270845d8f13f8f6738e6dd613`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 12 Jul 2022 01:25:28 GMT
ADD file:9e1afe48f40d94f879aefb12a7e68da2f0772d701e95b8219bd1f79a83e1933a in / 
# Tue, 12 Jul 2022 01:25:32 GMT
CMD ["bash"]
# Wed, 13 Jul 2022 06:43:01 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 13 Jul 2022 06:43:12 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 13 Jul 2022 06:43:14 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 13 Jul 2022 06:45:53 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 13 Jul 2022 06:45:55 GMT
VOLUME [/spiped]
# Wed, 13 Jul 2022 06:45:59 GMT
WORKDIR /spiped
# Wed, 13 Jul 2022 06:46:01 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 13 Jul 2022 06:46:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 13 Jul 2022 06:46:06 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:bd3d68d1ce583727f6378a16916795b955cc0ad39e0ebe754a26007ef54744fa`  
		Last Modified: Tue, 12 Jul 2022 01:36:03 GMT  
		Size: 35.3 MB (35272500 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9118819a47938b959974a2c187124c206d412a4381b1fa00b07702644095ac5d`  
		Last Modified: Wed, 13 Jul 2022 06:46:45 GMT  
		Size: 1.7 KB (1730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:387914e121edf896abe5847d4c111ed304f65ba32e283e8c551636e0603f325c`  
		Last Modified: Wed, 13 Jul 2022 06:46:45 GMT  
		Size: 1.1 KB (1053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bbc4a7edac4c6f551075397bc114c02da11b03ddf357cadb338265a627754b4`  
		Last Modified: Wed, 13 Jul 2022 06:46:46 GMT  
		Size: 6.0 MB (5999305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:773d9584db6f6fede768ee1493062d61d3061585c34a2d6716802a94dcf16103`  
		Last Modified: Wed, 13 Jul 2022 06:46:45 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e83ac10baec3d66ad682bc3eefbc4b8d96730fafcf154ef2da09edeb47bb1f7b`  
		Last Modified: Wed, 13 Jul 2022 06:46:45 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.2` - linux; s390x

```console
$ docker pull spiped@sha256:7bf397f297d1ea78dd655acc6c96775a5343e89423693de15ff17f08a7e69fda
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.8 MB (34830403 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3d0f9f2ec0119a2ccfd6b0ef28575b5bc407594263c24f89aa33495fe897631e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 02 Aug 2022 00:42:27 GMT
ADD file:c2afc8990930846fbe7c99bfdfe9ea562c75feb6e3c9122431f7c9f8b5e51a7f in / 
# Tue, 02 Aug 2022 00:42:29 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 11:36:27 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 02 Aug 2022 11:36:30 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 11:36:30 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 02 Aug 2022 11:36:42 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 02 Aug 2022 11:36:43 GMT
VOLUME [/spiped]
# Tue, 02 Aug 2022 11:36:43 GMT
WORKDIR /spiped
# Tue, 02 Aug 2022 11:36:43 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 02 Aug 2022 11:36:43 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 02 Aug 2022 11:36:43 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:026d311d0716db60eba0572ea784c21031f420960510cebcc383dc53949b4db8`  
		Last Modified: Tue, 02 Aug 2022 00:48:01 GMT  
		Size: 29.6 MB (29640259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7541e31145bcc880fcc60aff1fd1a6d96cc9bfff5e16ef0d5d327dd9497e2c1e`  
		Last Modified: Tue, 02 Aug 2022 11:37:16 GMT  
		Size: 1.7 KB (1736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd776eddcc8f7519e60d13e33bc0d710d15961af956903b4361c059231a13fb4`  
		Last Modified: Tue, 02 Aug 2022 11:37:16 GMT  
		Size: 1.1 KB (1051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bc0a264606dbae8f6555594bd36ddec88a7aa137902dd45515476c03ba153af`  
		Last Modified: Tue, 02 Aug 2022 11:37:16 GMT  
		Size: 5.2 MB (5186886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b5adf2a4c0e90db6b594339181e513b60ec0843bce0a63c90ac2330aa21bb51`  
		Last Modified: Tue, 02 Aug 2022 11:37:16 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfd03b0951b798cc22685c0158dc76558cc97d72e2f54238e5a9af5be042cbef`  
		Last Modified: Tue, 02 Aug 2022 11:37:16 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:1.6.2-alpine`

```console
$ docker pull spiped@sha256:e5d676b01e625c44b03a97f212d2e01b80e93817b2879a812d27930808ce1710
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
$ docker pull spiped@sha256:960558dde1fffd85012e80768bb5fb6b5ce16f56a6d8ba36c4eb4871b3d7ad20
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (3022913 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a4f255584cbbb67f7dca6e7842e9ba534deb82bcc7d271ddb94d37ca749d4143`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Mon, 18 Jul 2022 21:00:15 GMT
ADD file:a2648378045615c3785c752423b1afc8dc1c2b213393344f4d0ca17e7255c1cb in / 
# Mon, 18 Jul 2022 21:00:15 GMT
CMD ["/bin/sh"]
# Tue, 19 Jul 2022 02:58:44 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Tue, 19 Jul 2022 02:58:45 GMT
RUN apk add --no-cache libssl1.1
# Tue, 19 Jul 2022 02:58:45 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 19 Jul 2022 02:58:56 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Tue, 19 Jul 2022 02:58:56 GMT
VOLUME [/spiped]
# Tue, 19 Jul 2022 02:58:56 GMT
WORKDIR /spiped
# Tue, 19 Jul 2022 02:58:56 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 19 Jul 2022 02:58:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 19 Jul 2022 02:58:56 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:530afca65e2ea04227630ae746e0c85b2bd1a179379cbf2b6501b49c4cab2ccc`  
		Last Modified: Mon, 18 Jul 2022 19:09:35 GMT  
		Size: 2.8 MB (2798806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53ccfd605bd789873358dddbc12507c07697196241ef12b229daede89fede305`  
		Last Modified: Tue, 19 Jul 2022 02:59:13 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91eb30e4056e3cf1d260026125f2c0969702f9eda398caa33c77fcc1efb6da0f`  
		Last Modified: Tue, 19 Jul 2022 02:59:13 GMT  
		Size: 7.7 KB (7739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eeedfc703c38a2268ccf7afedcb792b89f9b7d7ff21f541ba671f04052a7f654`  
		Last Modified: Tue, 19 Jul 2022 02:59:13 GMT  
		Size: 214.6 KB (214629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e96340c6dfa203988333004e74c69a13274414e98de4322ea0c789ad7df42c9`  
		Last Modified: Tue, 19 Jul 2022 02:59:13 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:383211380910b0d4fcc33212392f07b13de80297232cd9da3c25f3a80b67dd34`  
		Last Modified: Tue, 19 Jul 2022 02:59:13 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.2-alpine` - linux; arm variant v6

```console
$ docker pull spiped@sha256:78d7c6b26405f2ccec387dbd5f5f8380bfac8922c0cde017bf83199a7c93de3f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 MB (2815244 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0975d891cb5d986fa371064357d538cff8e162c0dbcbeb412b87e765eea2bee6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Mon, 18 Jul 2022 19:49:37 GMT
ADD file:7a20333469e71664904a0cb8f61613250f2bd092b4a27bfa7bbae1dc7e21b7ed in / 
# Mon, 18 Jul 2022 19:49:37 GMT
CMD ["/bin/sh"]
# Tue, 19 Jul 2022 04:28:52 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Tue, 19 Jul 2022 04:28:54 GMT
RUN apk add --no-cache libssl1.1
# Tue, 19 Jul 2022 04:28:55 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 19 Jul 2022 04:29:15 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Tue, 19 Jul 2022 04:29:16 GMT
VOLUME [/spiped]
# Tue, 19 Jul 2022 04:29:16 GMT
WORKDIR /spiped
# Tue, 19 Jul 2022 04:29:17 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 19 Jul 2022 04:29:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 19 Jul 2022 04:29:18 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:b7885075fcd06a866d12dfd56eb704045eaadbd22dc03a224cd98715be566677`  
		Last Modified: Mon, 18 Jul 2022 19:08:42 GMT  
		Size: 2.6 MB (2606431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7794ac6005a3d1042ca428fddd078ac26956535628f13a1901b8aaf3986288d`  
		Last Modified: Tue, 19 Jul 2022 04:29:51 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0a8bbac389bb4b97ec5a6d16185ce572d9e89d45f67d819d9eee81fee855e51`  
		Last Modified: Tue, 19 Jul 2022 04:29:51 GMT  
		Size: 7.7 KB (7735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:382b8ab18f4e21efbd2668e38088fe5d0a5e016a65d8f3845cfa386c1d974999`  
		Last Modified: Tue, 19 Jul 2022 04:29:51 GMT  
		Size: 199.3 KB (199338 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:940073d33e787162c6aa336ae5ef93efdd6641a3dc59e5d4a0eb01f0c24aeecf`  
		Last Modified: Tue, 19 Jul 2022 04:29:51 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cf4811d369ed3ed91ee23a134ab53b91888e93efc80c38c6c15d44a1ec8e9de`  
		Last Modified: Tue, 19 Jul 2022 04:29:51 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.2-alpine` - linux; arm variant v7

```console
$ docker pull spiped@sha256:406d539553f81f86ec46ac0c9d08717c75356e6a706276e25986ea7ec4bb70df
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 MB (2614862 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ea10f25c876d7c1e28ac07d56cfd6dd1840cab98ca857fc651e9f8a5ba29e9a6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Mon, 18 Jul 2022 21:24:47 GMT
ADD file:68590e866bc6db27ad54d23de7dd275d0389cb86e4e6291a1243fcc234f2f7a1 in / 
# Mon, 18 Jul 2022 21:24:47 GMT
CMD ["/bin/sh"]
# Tue, 19 Jul 2022 09:42:16 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Tue, 19 Jul 2022 09:42:18 GMT
RUN apk add --no-cache libssl1.1
# Tue, 19 Jul 2022 09:42:19 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 19 Jul 2022 09:42:38 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Tue, 19 Jul 2022 09:42:38 GMT
VOLUME [/spiped]
# Tue, 19 Jul 2022 09:42:39 GMT
WORKDIR /spiped
# Tue, 19 Jul 2022 09:42:39 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 19 Jul 2022 09:42:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 19 Jul 2022 09:42:40 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:a6b45ace95f42a930d15c33679ab9c85d46019b7e73954cadc73bb9ba176509b`  
		Last Modified: Mon, 18 Jul 2022 19:08:56 GMT  
		Size: 2.4 MB (2412307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c22ed0b9f7779fd593471ef1630a429072a4f3bcd202ea38f6cb1627bead8e4`  
		Last Modified: Tue, 19 Jul 2022 09:43:34 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38d4163652a3ead1410becbb61a24e8f06d77f6d284534294a0bccb49bac57b8`  
		Last Modified: Tue, 19 Jul 2022 09:43:34 GMT  
		Size: 7.7 KB (7727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53df3c1757f5b854f0a5eefe967294a0d6ec49e4a5049dc712fafa9800599afc`  
		Last Modified: Tue, 19 Jul 2022 09:43:34 GMT  
		Size: 193.1 KB (193092 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1a490c5af6b8a6ec597efac4811e4ee5c156fabde11c8438da0344a492454f7`  
		Last Modified: Tue, 19 Jul 2022 09:43:34 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:191417a31477ff188751e4c9bb0754f52a807992a390563f7d84ed86683eaa30`  
		Last Modified: Tue, 19 Jul 2022 09:43:34 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.2-alpine` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:b4e4831c1382ba6191159248fbf92a052b843dd76ffb3e5ab9590a9b50033a72
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 MB (2911791 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:48fa91c14a7ba129a596b0eaffb3c321c3d4c509db24ecf103535d7fb2bd6598`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Mon, 18 Jul 2022 21:57:05 GMT
ADD file:9ccb70abba88b6de789b29f17770246f765ffbb072fe598580bfc29ce3213f1c in / 
# Mon, 18 Jul 2022 21:57:05 GMT
CMD ["/bin/sh"]
# Tue, 19 Jul 2022 03:11:40 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Tue, 19 Jul 2022 03:11:41 GMT
RUN apk add --no-cache libssl1.1
# Tue, 19 Jul 2022 03:11:42 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 19 Jul 2022 03:11:53 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Tue, 19 Jul 2022 03:11:54 GMT
VOLUME [/spiped]
# Tue, 19 Jul 2022 03:11:55 GMT
WORKDIR /spiped
# Tue, 19 Jul 2022 03:11:57 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 19 Jul 2022 03:11:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 19 Jul 2022 03:11:58 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:f97344484467e4c4ebb85aae724170073799295a3442c50ab532e249bd27b412`  
		Last Modified: Mon, 18 Jul 2022 19:08:29 GMT  
		Size: 2.7 MB (2694720 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51a8e96b71a119a7753279fa24fc1b097b559f365c0d74c928ec0827108be3ac`  
		Last Modified: Tue, 19 Jul 2022 03:12:25 GMT  
		Size: 1.2 KB (1243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef5b7ffd6e7e16898220160e758a91b7ae6e5fa7763e22b1f929570b0e877432`  
		Last Modified: Tue, 19 Jul 2022 03:12:25 GMT  
		Size: 7.7 KB (7708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54764cd29a52b45365923ab1e756750d07330c69ea57b318f8f4b2660940a1fa`  
		Last Modified: Tue, 19 Jul 2022 03:12:25 GMT  
		Size: 207.7 KB (207685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a2841c7d2c1268e60c21c01e69c10868bef688cc32f57dbe883e975040d003f`  
		Last Modified: Tue, 19 Jul 2022 03:12:25 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b456f54f4f08db25a2b70f3ecd5b9a2273937e824ae2e3d919c7f3d8b31102a2`  
		Last Modified: Tue, 19 Jul 2022 03:12:25 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.2-alpine` - linux; 386

```console
$ docker pull spiped@sha256:bd3d4904f8e1d52ce4a28eb847bc57f54248490fc15e9ac6e88cca4566f2bbec
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (3036863 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:abc7cf0e554fe461e7d95534758c990b4c5f507ac6912d08de0ab5c7192d5a4b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Mon, 18 Jul 2022 20:38:19 GMT
ADD file:be69b7550bf861d8fb12bdbe1edf3a0d2519a6a4da61bd04858b6258ffbf48a7 in / 
# Mon, 18 Jul 2022 20:38:19 GMT
CMD ["/bin/sh"]
# Tue, 19 Jul 2022 00:52:10 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Tue, 19 Jul 2022 00:52:11 GMT
RUN apk add --no-cache libssl1.1
# Tue, 19 Jul 2022 00:52:12 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 19 Jul 2022 00:52:24 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Tue, 19 Jul 2022 00:52:25 GMT
VOLUME [/spiped]
# Tue, 19 Jul 2022 00:52:26 GMT
WORKDIR /spiped
# Tue, 19 Jul 2022 00:52:28 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 19 Jul 2022 00:52:28 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 19 Jul 2022 00:52:29 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:5d7f927419794ebb7496ac38b0659686317b2d2fac7252a4a0d40d43d5fdd662`  
		Last Modified: Mon, 18 Jul 2022 19:09:22 GMT  
		Size: 2.8 MB (2802334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8be475f4c97c2b6a50a82b2cda5d04dcf3be627667431e283146f5ef2467cf2`  
		Last Modified: Tue, 19 Jul 2022 00:52:57 GMT  
		Size: 1.2 KB (1243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ccf382b13c23a3fe33bbd2b36efca3ac3493d37bbda16a50f5df1a18b997e00`  
		Last Modified: Tue, 19 Jul 2022 00:52:57 GMT  
		Size: 7.7 KB (7711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb7cd3baa7c17abca3fa3c456474f8fe1b0aa45d19cba81de21b85554722608e`  
		Last Modified: Tue, 19 Jul 2022 00:52:58 GMT  
		Size: 225.1 KB (225138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a1a6c9df0a41f62802eec16036b66a1513b5b158004c13839da1b3ba266ac38`  
		Last Modified: Tue, 19 Jul 2022 00:52:57 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16f06336cb65e863eccc316001a0037fbb6fc5dd05ff03301c9a513d42af9128`  
		Last Modified: Tue, 19 Jul 2022 00:52:58 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.2-alpine` - linux; ppc64le

```console
$ docker pull spiped@sha256:f9db2c66d081de674f9c2b6be02eded176cb2fdbe2ed251d040663111d8d765f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (3013087 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:64a91098c0d88cb338eb43ccb20d859d67efe05df38a850d2b645a1f3aa26c5c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Mon, 18 Jul 2022 21:29:30 GMT
ADD file:69e4080f15f54e2d8f8aa25fdcba9c01dde149d43592edd5023106675e54a769 in / 
# Mon, 18 Jul 2022 21:29:31 GMT
CMD ["/bin/sh"]
# Tue, 19 Jul 2022 07:44:52 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Tue, 19 Jul 2022 07:45:01 GMT
RUN apk add --no-cache libssl1.1
# Tue, 19 Jul 2022 07:45:03 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 19 Jul 2022 07:45:21 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Tue, 19 Jul 2022 07:45:23 GMT
VOLUME [/spiped]
# Tue, 19 Jul 2022 07:45:25 GMT
WORKDIR /spiped
# Tue, 19 Jul 2022 07:45:28 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 19 Jul 2022 07:45:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 19 Jul 2022 07:45:36 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:602896d442490cd3fbb6599f0f862d3673b7cd58eca3ac842b8e09bf8d012443`  
		Last Modified: Mon, 18 Jul 2022 19:09:09 GMT  
		Size: 2.8 MB (2789923 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:625e385ac9fcd0da39e5754ecac93c3230b8a4b0b5f6f466f5df607a9f76dd58`  
		Last Modified: Tue, 19 Jul 2022 07:46:14 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae1de895bed2f7ec17e8fccb9e6d944457809f1e9fc22e7c1a8b52a630caf1c3`  
		Last Modified: Tue, 19 Jul 2022 07:46:14 GMT  
		Size: 7.7 KB (7734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5828466d70a99b3e62cd1f6cbbe9ce7bf47fecfefbc3a91eecdb80647c749856`  
		Last Modified: Tue, 19 Jul 2022 07:46:14 GMT  
		Size: 213.7 KB (213691 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee54a465cd2b488f11e4e693d68d679ec15b3c5b1c88679f87a485b200f94160`  
		Last Modified: Tue, 19 Jul 2022 07:46:14 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3c9a834c167df5b7cf9265a0390b7e6c81bf076f8b0b9d3b848ddb02c9cf8ff`  
		Last Modified: Tue, 19 Jul 2022 07:46:14 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.2-alpine` - linux; s390x

```console
$ docker pull spiped@sha256:5abc9d546636b6670ca2c300303d57c59e066f9b42af71ffc12fce775274b2b8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 MB (2792283 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dc9891884c555841cd06fd9c1a3608fcb75e6ab6cdb389c07e53fed03b6bb500`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Mon, 18 Jul 2022 20:41:35 GMT
ADD file:deaa573cd61e07709846a5300fb627a8610e9754129c085ed483ff8897d0c002 in / 
# Mon, 18 Jul 2022 20:41:36 GMT
CMD ["/bin/sh"]
# Tue, 19 Jul 2022 05:40:59 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Tue, 19 Jul 2022 05:41:01 GMT
RUN apk add --no-cache libssl1.1
# Tue, 19 Jul 2022 05:41:02 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 19 Jul 2022 05:41:11 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Tue, 19 Jul 2022 05:41:11 GMT
VOLUME [/spiped]
# Tue, 19 Jul 2022 05:41:12 GMT
WORKDIR /spiped
# Tue, 19 Jul 2022 05:41:13 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 19 Jul 2022 05:41:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 19 Jul 2022 05:41:13 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:5f1840d5bacf4162a87f497e22d94bce946e660bdfce8eeefcbf7bd0beb193f3`  
		Last Modified: Mon, 18 Jul 2022 20:42:36 GMT  
		Size: 2.6 MB (2580798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd6993821da2e7957193713709542cca3a229ed17d3d859ca823a7ef4e38b011`  
		Last Modified: Tue, 19 Jul 2022 05:41:47 GMT  
		Size: 1.3 KB (1266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09df37c5f8ac9a24ba5f55d4d545b4835141a55e5f9ecd71f8b936809f8fddd3`  
		Last Modified: Tue, 19 Jul 2022 05:41:47 GMT  
		Size: 7.7 KB (7742 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9c64cd2f7e97c8f03ec8ef34a7ba77e455842217cfcc3e9c6816f56ea8108b6`  
		Last Modified: Tue, 19 Jul 2022 05:41:47 GMT  
		Size: 202.0 KB (202009 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3ec9f775174ce04ae9cf626a975e42a1f50926f1d9f9cdecf513cdb1514809b`  
		Last Modified: Tue, 19 Jul 2022 05:41:47 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41b76904392c2be02eeefc2c55db23094f8f3578806838b317aec9d39ec86abd`  
		Last Modified: Tue, 19 Jul 2022 05:41:47 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:alpine`

```console
$ docker pull spiped@sha256:e5d676b01e625c44b03a97f212d2e01b80e93817b2879a812d27930808ce1710
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
$ docker pull spiped@sha256:960558dde1fffd85012e80768bb5fb6b5ce16f56a6d8ba36c4eb4871b3d7ad20
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (3022913 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a4f255584cbbb67f7dca6e7842e9ba534deb82bcc7d271ddb94d37ca749d4143`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Mon, 18 Jul 2022 21:00:15 GMT
ADD file:a2648378045615c3785c752423b1afc8dc1c2b213393344f4d0ca17e7255c1cb in / 
# Mon, 18 Jul 2022 21:00:15 GMT
CMD ["/bin/sh"]
# Tue, 19 Jul 2022 02:58:44 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Tue, 19 Jul 2022 02:58:45 GMT
RUN apk add --no-cache libssl1.1
# Tue, 19 Jul 2022 02:58:45 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 19 Jul 2022 02:58:56 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Tue, 19 Jul 2022 02:58:56 GMT
VOLUME [/spiped]
# Tue, 19 Jul 2022 02:58:56 GMT
WORKDIR /spiped
# Tue, 19 Jul 2022 02:58:56 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 19 Jul 2022 02:58:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 19 Jul 2022 02:58:56 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:530afca65e2ea04227630ae746e0c85b2bd1a179379cbf2b6501b49c4cab2ccc`  
		Last Modified: Mon, 18 Jul 2022 19:09:35 GMT  
		Size: 2.8 MB (2798806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53ccfd605bd789873358dddbc12507c07697196241ef12b229daede89fede305`  
		Last Modified: Tue, 19 Jul 2022 02:59:13 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91eb30e4056e3cf1d260026125f2c0969702f9eda398caa33c77fcc1efb6da0f`  
		Last Modified: Tue, 19 Jul 2022 02:59:13 GMT  
		Size: 7.7 KB (7739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eeedfc703c38a2268ccf7afedcb792b89f9b7d7ff21f541ba671f04052a7f654`  
		Last Modified: Tue, 19 Jul 2022 02:59:13 GMT  
		Size: 214.6 KB (214629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e96340c6dfa203988333004e74c69a13274414e98de4322ea0c789ad7df42c9`  
		Last Modified: Tue, 19 Jul 2022 02:59:13 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:383211380910b0d4fcc33212392f07b13de80297232cd9da3c25f3a80b67dd34`  
		Last Modified: Tue, 19 Jul 2022 02:59:13 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; arm variant v6

```console
$ docker pull spiped@sha256:78d7c6b26405f2ccec387dbd5f5f8380bfac8922c0cde017bf83199a7c93de3f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 MB (2815244 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0975d891cb5d986fa371064357d538cff8e162c0dbcbeb412b87e765eea2bee6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Mon, 18 Jul 2022 19:49:37 GMT
ADD file:7a20333469e71664904a0cb8f61613250f2bd092b4a27bfa7bbae1dc7e21b7ed in / 
# Mon, 18 Jul 2022 19:49:37 GMT
CMD ["/bin/sh"]
# Tue, 19 Jul 2022 04:28:52 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Tue, 19 Jul 2022 04:28:54 GMT
RUN apk add --no-cache libssl1.1
# Tue, 19 Jul 2022 04:28:55 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 19 Jul 2022 04:29:15 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Tue, 19 Jul 2022 04:29:16 GMT
VOLUME [/spiped]
# Tue, 19 Jul 2022 04:29:16 GMT
WORKDIR /spiped
# Tue, 19 Jul 2022 04:29:17 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 19 Jul 2022 04:29:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 19 Jul 2022 04:29:18 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:b7885075fcd06a866d12dfd56eb704045eaadbd22dc03a224cd98715be566677`  
		Last Modified: Mon, 18 Jul 2022 19:08:42 GMT  
		Size: 2.6 MB (2606431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7794ac6005a3d1042ca428fddd078ac26956535628f13a1901b8aaf3986288d`  
		Last Modified: Tue, 19 Jul 2022 04:29:51 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0a8bbac389bb4b97ec5a6d16185ce572d9e89d45f67d819d9eee81fee855e51`  
		Last Modified: Tue, 19 Jul 2022 04:29:51 GMT  
		Size: 7.7 KB (7735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:382b8ab18f4e21efbd2668e38088fe5d0a5e016a65d8f3845cfa386c1d974999`  
		Last Modified: Tue, 19 Jul 2022 04:29:51 GMT  
		Size: 199.3 KB (199338 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:940073d33e787162c6aa336ae5ef93efdd6641a3dc59e5d4a0eb01f0c24aeecf`  
		Last Modified: Tue, 19 Jul 2022 04:29:51 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cf4811d369ed3ed91ee23a134ab53b91888e93efc80c38c6c15d44a1ec8e9de`  
		Last Modified: Tue, 19 Jul 2022 04:29:51 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; arm variant v7

```console
$ docker pull spiped@sha256:406d539553f81f86ec46ac0c9d08717c75356e6a706276e25986ea7ec4bb70df
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 MB (2614862 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ea10f25c876d7c1e28ac07d56cfd6dd1840cab98ca857fc651e9f8a5ba29e9a6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Mon, 18 Jul 2022 21:24:47 GMT
ADD file:68590e866bc6db27ad54d23de7dd275d0389cb86e4e6291a1243fcc234f2f7a1 in / 
# Mon, 18 Jul 2022 21:24:47 GMT
CMD ["/bin/sh"]
# Tue, 19 Jul 2022 09:42:16 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Tue, 19 Jul 2022 09:42:18 GMT
RUN apk add --no-cache libssl1.1
# Tue, 19 Jul 2022 09:42:19 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 19 Jul 2022 09:42:38 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Tue, 19 Jul 2022 09:42:38 GMT
VOLUME [/spiped]
# Tue, 19 Jul 2022 09:42:39 GMT
WORKDIR /spiped
# Tue, 19 Jul 2022 09:42:39 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 19 Jul 2022 09:42:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 19 Jul 2022 09:42:40 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:a6b45ace95f42a930d15c33679ab9c85d46019b7e73954cadc73bb9ba176509b`  
		Last Modified: Mon, 18 Jul 2022 19:08:56 GMT  
		Size: 2.4 MB (2412307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c22ed0b9f7779fd593471ef1630a429072a4f3bcd202ea38f6cb1627bead8e4`  
		Last Modified: Tue, 19 Jul 2022 09:43:34 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38d4163652a3ead1410becbb61a24e8f06d77f6d284534294a0bccb49bac57b8`  
		Last Modified: Tue, 19 Jul 2022 09:43:34 GMT  
		Size: 7.7 KB (7727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53df3c1757f5b854f0a5eefe967294a0d6ec49e4a5049dc712fafa9800599afc`  
		Last Modified: Tue, 19 Jul 2022 09:43:34 GMT  
		Size: 193.1 KB (193092 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1a490c5af6b8a6ec597efac4811e4ee5c156fabde11c8438da0344a492454f7`  
		Last Modified: Tue, 19 Jul 2022 09:43:34 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:191417a31477ff188751e4c9bb0754f52a807992a390563f7d84ed86683eaa30`  
		Last Modified: Tue, 19 Jul 2022 09:43:34 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:b4e4831c1382ba6191159248fbf92a052b843dd76ffb3e5ab9590a9b50033a72
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 MB (2911791 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:48fa91c14a7ba129a596b0eaffb3c321c3d4c509db24ecf103535d7fb2bd6598`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Mon, 18 Jul 2022 21:57:05 GMT
ADD file:9ccb70abba88b6de789b29f17770246f765ffbb072fe598580bfc29ce3213f1c in / 
# Mon, 18 Jul 2022 21:57:05 GMT
CMD ["/bin/sh"]
# Tue, 19 Jul 2022 03:11:40 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Tue, 19 Jul 2022 03:11:41 GMT
RUN apk add --no-cache libssl1.1
# Tue, 19 Jul 2022 03:11:42 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 19 Jul 2022 03:11:53 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Tue, 19 Jul 2022 03:11:54 GMT
VOLUME [/spiped]
# Tue, 19 Jul 2022 03:11:55 GMT
WORKDIR /spiped
# Tue, 19 Jul 2022 03:11:57 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 19 Jul 2022 03:11:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 19 Jul 2022 03:11:58 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:f97344484467e4c4ebb85aae724170073799295a3442c50ab532e249bd27b412`  
		Last Modified: Mon, 18 Jul 2022 19:08:29 GMT  
		Size: 2.7 MB (2694720 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51a8e96b71a119a7753279fa24fc1b097b559f365c0d74c928ec0827108be3ac`  
		Last Modified: Tue, 19 Jul 2022 03:12:25 GMT  
		Size: 1.2 KB (1243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef5b7ffd6e7e16898220160e758a91b7ae6e5fa7763e22b1f929570b0e877432`  
		Last Modified: Tue, 19 Jul 2022 03:12:25 GMT  
		Size: 7.7 KB (7708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54764cd29a52b45365923ab1e756750d07330c69ea57b318f8f4b2660940a1fa`  
		Last Modified: Tue, 19 Jul 2022 03:12:25 GMT  
		Size: 207.7 KB (207685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a2841c7d2c1268e60c21c01e69c10868bef688cc32f57dbe883e975040d003f`  
		Last Modified: Tue, 19 Jul 2022 03:12:25 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b456f54f4f08db25a2b70f3ecd5b9a2273937e824ae2e3d919c7f3d8b31102a2`  
		Last Modified: Tue, 19 Jul 2022 03:12:25 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; 386

```console
$ docker pull spiped@sha256:bd3d4904f8e1d52ce4a28eb847bc57f54248490fc15e9ac6e88cca4566f2bbec
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (3036863 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:abc7cf0e554fe461e7d95534758c990b4c5f507ac6912d08de0ab5c7192d5a4b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Mon, 18 Jul 2022 20:38:19 GMT
ADD file:be69b7550bf861d8fb12bdbe1edf3a0d2519a6a4da61bd04858b6258ffbf48a7 in / 
# Mon, 18 Jul 2022 20:38:19 GMT
CMD ["/bin/sh"]
# Tue, 19 Jul 2022 00:52:10 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Tue, 19 Jul 2022 00:52:11 GMT
RUN apk add --no-cache libssl1.1
# Tue, 19 Jul 2022 00:52:12 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 19 Jul 2022 00:52:24 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Tue, 19 Jul 2022 00:52:25 GMT
VOLUME [/spiped]
# Tue, 19 Jul 2022 00:52:26 GMT
WORKDIR /spiped
# Tue, 19 Jul 2022 00:52:28 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 19 Jul 2022 00:52:28 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 19 Jul 2022 00:52:29 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:5d7f927419794ebb7496ac38b0659686317b2d2fac7252a4a0d40d43d5fdd662`  
		Last Modified: Mon, 18 Jul 2022 19:09:22 GMT  
		Size: 2.8 MB (2802334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8be475f4c97c2b6a50a82b2cda5d04dcf3be627667431e283146f5ef2467cf2`  
		Last Modified: Tue, 19 Jul 2022 00:52:57 GMT  
		Size: 1.2 KB (1243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ccf382b13c23a3fe33bbd2b36efca3ac3493d37bbda16a50f5df1a18b997e00`  
		Last Modified: Tue, 19 Jul 2022 00:52:57 GMT  
		Size: 7.7 KB (7711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb7cd3baa7c17abca3fa3c456474f8fe1b0aa45d19cba81de21b85554722608e`  
		Last Modified: Tue, 19 Jul 2022 00:52:58 GMT  
		Size: 225.1 KB (225138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a1a6c9df0a41f62802eec16036b66a1513b5b158004c13839da1b3ba266ac38`  
		Last Modified: Tue, 19 Jul 2022 00:52:57 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16f06336cb65e863eccc316001a0037fbb6fc5dd05ff03301c9a513d42af9128`  
		Last Modified: Tue, 19 Jul 2022 00:52:58 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; ppc64le

```console
$ docker pull spiped@sha256:f9db2c66d081de674f9c2b6be02eded176cb2fdbe2ed251d040663111d8d765f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (3013087 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:64a91098c0d88cb338eb43ccb20d859d67efe05df38a850d2b645a1f3aa26c5c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Mon, 18 Jul 2022 21:29:30 GMT
ADD file:69e4080f15f54e2d8f8aa25fdcba9c01dde149d43592edd5023106675e54a769 in / 
# Mon, 18 Jul 2022 21:29:31 GMT
CMD ["/bin/sh"]
# Tue, 19 Jul 2022 07:44:52 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Tue, 19 Jul 2022 07:45:01 GMT
RUN apk add --no-cache libssl1.1
# Tue, 19 Jul 2022 07:45:03 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 19 Jul 2022 07:45:21 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Tue, 19 Jul 2022 07:45:23 GMT
VOLUME [/spiped]
# Tue, 19 Jul 2022 07:45:25 GMT
WORKDIR /spiped
# Tue, 19 Jul 2022 07:45:28 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 19 Jul 2022 07:45:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 19 Jul 2022 07:45:36 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:602896d442490cd3fbb6599f0f862d3673b7cd58eca3ac842b8e09bf8d012443`  
		Last Modified: Mon, 18 Jul 2022 19:09:09 GMT  
		Size: 2.8 MB (2789923 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:625e385ac9fcd0da39e5754ecac93c3230b8a4b0b5f6f466f5df607a9f76dd58`  
		Last Modified: Tue, 19 Jul 2022 07:46:14 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae1de895bed2f7ec17e8fccb9e6d944457809f1e9fc22e7c1a8b52a630caf1c3`  
		Last Modified: Tue, 19 Jul 2022 07:46:14 GMT  
		Size: 7.7 KB (7734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5828466d70a99b3e62cd1f6cbbe9ce7bf47fecfefbc3a91eecdb80647c749856`  
		Last Modified: Tue, 19 Jul 2022 07:46:14 GMT  
		Size: 213.7 KB (213691 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee54a465cd2b488f11e4e693d68d679ec15b3c5b1c88679f87a485b200f94160`  
		Last Modified: Tue, 19 Jul 2022 07:46:14 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3c9a834c167df5b7cf9265a0390b7e6c81bf076f8b0b9d3b848ddb02c9cf8ff`  
		Last Modified: Tue, 19 Jul 2022 07:46:14 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; s390x

```console
$ docker pull spiped@sha256:5abc9d546636b6670ca2c300303d57c59e066f9b42af71ffc12fce775274b2b8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 MB (2792283 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dc9891884c555841cd06fd9c1a3608fcb75e6ab6cdb389c07e53fed03b6bb500`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Mon, 18 Jul 2022 20:41:35 GMT
ADD file:deaa573cd61e07709846a5300fb627a8610e9754129c085ed483ff8897d0c002 in / 
# Mon, 18 Jul 2022 20:41:36 GMT
CMD ["/bin/sh"]
# Tue, 19 Jul 2022 05:40:59 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Tue, 19 Jul 2022 05:41:01 GMT
RUN apk add --no-cache libssl1.1
# Tue, 19 Jul 2022 05:41:02 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 19 Jul 2022 05:41:11 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Tue, 19 Jul 2022 05:41:11 GMT
VOLUME [/spiped]
# Tue, 19 Jul 2022 05:41:12 GMT
WORKDIR /spiped
# Tue, 19 Jul 2022 05:41:13 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 19 Jul 2022 05:41:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 19 Jul 2022 05:41:13 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:5f1840d5bacf4162a87f497e22d94bce946e660bdfce8eeefcbf7bd0beb193f3`  
		Last Modified: Mon, 18 Jul 2022 20:42:36 GMT  
		Size: 2.6 MB (2580798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd6993821da2e7957193713709542cca3a229ed17d3d859ca823a7ef4e38b011`  
		Last Modified: Tue, 19 Jul 2022 05:41:47 GMT  
		Size: 1.3 KB (1266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09df37c5f8ac9a24ba5f55d4d545b4835141a55e5f9ecd71f8b936809f8fddd3`  
		Last Modified: Tue, 19 Jul 2022 05:41:47 GMT  
		Size: 7.7 KB (7742 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9c64cd2f7e97c8f03ec8ef34a7ba77e455842217cfcc3e9c6816f56ea8108b6`  
		Last Modified: Tue, 19 Jul 2022 05:41:47 GMT  
		Size: 202.0 KB (202009 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3ec9f775174ce04ae9cf626a975e42a1f50926f1d9f9cdecf513cdb1514809b`  
		Last Modified: Tue, 19 Jul 2022 05:41:47 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41b76904392c2be02eeefc2c55db23094f8f3578806838b317aec9d39ec86abd`  
		Last Modified: Tue, 19 Jul 2022 05:41:47 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:latest`

```console
$ docker pull spiped@sha256:893b1d34151bff6fc3b147f4492989c25976f4c5bd2b714b7872c22ddcf32453
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
$ docker pull spiped@sha256:f83b419d27348b2bdbf4d6e78da6d2e62f75d514a1ed39855e1899dc9b59fe73
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.3 MB (31312141 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:524e3e7d21e31be2a48e1548d86d5ced3a2ee4185440b47edacceca48ca97031`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 12 Jul 2022 00:59:54 GMT
ADD file:ae890621b36ff6e27364bb7316b5bd4319a820ddf7e65565c6201eb11d70fde9 in / 
# Tue, 12 Jul 2022 00:59:55 GMT
CMD ["bash"]
# Wed, 13 Jul 2022 07:57:44 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 13 Jul 2022 07:57:51 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 13 Jul 2022 07:57:52 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 13 Jul 2022 07:58:36 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 13 Jul 2022 07:58:37 GMT
VOLUME [/spiped]
# Wed, 13 Jul 2022 07:58:37 GMT
WORKDIR /spiped
# Wed, 13 Jul 2022 07:58:38 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 13 Jul 2022 07:58:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 13 Jul 2022 07:58:39 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:314cda9d0ef2282082d2bd0efd7659e0d9edb3ceae8e7919d990bcf95cbb3d2b`  
		Last Modified: Tue, 12 Jul 2022 01:12:37 GMT  
		Size: 26.6 MB (26560559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:090471f791b0f328f3661d50b9ff593c83c6e102cdb08df2fd72cecb662ff0be`  
		Last Modified: Wed, 13 Jul 2022 07:59:38 GMT  
		Size: 1.7 KB (1727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c4dfc160206772b3b1e6340d5d682c20ec1e14e0871426b46711d58b7d6833c`  
		Last Modified: Wed, 13 Jul 2022 07:59:38 GMT  
		Size: 1.1 KB (1053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89bb0f704911b77275d75f7bc8b4cf0b5162ade51f380f463c6cc820cac6968d`  
		Last Modified: Wed, 13 Jul 2022 07:59:42 GMT  
		Size: 4.7 MB (4748333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5b67ae8b1bcc4511eeadde14a66ebab56c086d30f91559679a64b68b73fc76a`  
		Last Modified: Wed, 13 Jul 2022 07:59:38 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:630225b9ddc0c86154ca5f1fa26d05def1293638c2be832017738f83eadd93a3`  
		Last Modified: Wed, 13 Jul 2022 07:59:38 GMT  
		Size: 342.0 B  
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
$ docker pull spiped@sha256:0912dd64711f962ed20b280e96cc372e615b95b97ee1aa6a9056ba1f36a9f4cc
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.3 MB (35337184 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:40302e59e0dfc3ac7483cdda59a1917781d6bf1697c399cd8718d32fc20b3ab8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 12 Jul 2022 04:40:59 GMT
ADD file:e0c3a3f07bbd2b798f2f620e295566d0b49142660f897083f73164c0356f37a2 in / 
# Tue, 12 Jul 2022 04:41:04 GMT
CMD ["bash"]
# Wed, 13 Jul 2022 10:54:04 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 13 Jul 2022 10:54:19 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 13 Jul 2022 10:54:21 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 13 Jul 2022 10:55:53 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 13 Jul 2022 10:55:55 GMT
VOLUME [/spiped]
# Wed, 13 Jul 2022 10:55:58 GMT
WORKDIR /spiped
# Wed, 13 Jul 2022 10:56:00 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 13 Jul 2022 10:56:03 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 13 Jul 2022 10:56:06 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:88869778ecefe05f3e79ed90f3c06c22dfef4c56919a454f67eba47fb8072189`  
		Last Modified: Tue, 12 Jul 2022 04:51:44 GMT  
		Size: 29.6 MB (29628932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8dce35712b9df24fe23728e831a2d450572f507f476fca4f37b578b13c0f258f`  
		Last Modified: Wed, 13 Jul 2022 10:56:20 GMT  
		Size: 1.6 KB (1619 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78bf32252f913a3a579a40ec4538d9f0a46238b5bf83d6660c4967cca14df32a`  
		Last Modified: Wed, 13 Jul 2022 10:56:20 GMT  
		Size: 922.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:895648de55366c4420ab371cebceab082edcb43321c746dc76fb385c47594187`  
		Last Modified: Wed, 13 Jul 2022 10:56:26 GMT  
		Size: 5.7 MB (5705273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:918d7dc0f0ce53174644562b626a49d277285fa8c4ea2bcc0acc8efc1e63f7f6`  
		Last Modified: Wed, 13 Jul 2022 10:56:20 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1777ed1e7ecf5154695c61e242216358df92c1b5d2cef0c91e5b19b3b500b7c9`  
		Last Modified: Wed, 13 Jul 2022 10:56:20 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; ppc64le

```console
$ docker pull spiped@sha256:81003cf3de708c1d144d9355412aec5bdf2094c49b740cb388711db570b4356f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.3 MB (41275059 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4406e24e415436179ca82b111445f95864a4f68270845d8f13f8f6738e6dd613`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 12 Jul 2022 01:25:28 GMT
ADD file:9e1afe48f40d94f879aefb12a7e68da2f0772d701e95b8219bd1f79a83e1933a in / 
# Tue, 12 Jul 2022 01:25:32 GMT
CMD ["bash"]
# Wed, 13 Jul 2022 06:43:01 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 13 Jul 2022 06:43:12 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 13 Jul 2022 06:43:14 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 13 Jul 2022 06:45:53 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 13 Jul 2022 06:45:55 GMT
VOLUME [/spiped]
# Wed, 13 Jul 2022 06:45:59 GMT
WORKDIR /spiped
# Wed, 13 Jul 2022 06:46:01 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 13 Jul 2022 06:46:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 13 Jul 2022 06:46:06 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:bd3d68d1ce583727f6378a16916795b955cc0ad39e0ebe754a26007ef54744fa`  
		Last Modified: Tue, 12 Jul 2022 01:36:03 GMT  
		Size: 35.3 MB (35272500 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9118819a47938b959974a2c187124c206d412a4381b1fa00b07702644095ac5d`  
		Last Modified: Wed, 13 Jul 2022 06:46:45 GMT  
		Size: 1.7 KB (1730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:387914e121edf896abe5847d4c111ed304f65ba32e283e8c551636e0603f325c`  
		Last Modified: Wed, 13 Jul 2022 06:46:45 GMT  
		Size: 1.1 KB (1053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bbc4a7edac4c6f551075397bc114c02da11b03ddf357cadb338265a627754b4`  
		Last Modified: Wed, 13 Jul 2022 06:46:46 GMT  
		Size: 6.0 MB (5999305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:773d9584db6f6fede768ee1493062d61d3061585c34a2d6716802a94dcf16103`  
		Last Modified: Wed, 13 Jul 2022 06:46:45 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e83ac10baec3d66ad682bc3eefbc4b8d96730fafcf154ef2da09edeb47bb1f7b`  
		Last Modified: Wed, 13 Jul 2022 06:46:45 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; s390x

```console
$ docker pull spiped@sha256:7bf397f297d1ea78dd655acc6c96775a5343e89423693de15ff17f08a7e69fda
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.8 MB (34830403 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3d0f9f2ec0119a2ccfd6b0ef28575b5bc407594263c24f89aa33495fe897631e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 02 Aug 2022 00:42:27 GMT
ADD file:c2afc8990930846fbe7c99bfdfe9ea562c75feb6e3c9122431f7c9f8b5e51a7f in / 
# Tue, 02 Aug 2022 00:42:29 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 11:36:27 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 02 Aug 2022 11:36:30 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 11:36:30 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 02 Aug 2022 11:36:42 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 02 Aug 2022 11:36:43 GMT
VOLUME [/spiped]
# Tue, 02 Aug 2022 11:36:43 GMT
WORKDIR /spiped
# Tue, 02 Aug 2022 11:36:43 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 02 Aug 2022 11:36:43 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 02 Aug 2022 11:36:43 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:026d311d0716db60eba0572ea784c21031f420960510cebcc383dc53949b4db8`  
		Last Modified: Tue, 02 Aug 2022 00:48:01 GMT  
		Size: 29.6 MB (29640259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7541e31145bcc880fcc60aff1fd1a6d96cc9bfff5e16ef0d5d327dd9497e2c1e`  
		Last Modified: Tue, 02 Aug 2022 11:37:16 GMT  
		Size: 1.7 KB (1736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd776eddcc8f7519e60d13e33bc0d710d15961af956903b4361c059231a13fb4`  
		Last Modified: Tue, 02 Aug 2022 11:37:16 GMT  
		Size: 1.1 KB (1051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bc0a264606dbae8f6555594bd36ddec88a7aa137902dd45515476c03ba153af`  
		Last Modified: Tue, 02 Aug 2022 11:37:16 GMT  
		Size: 5.2 MB (5186886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b5adf2a4c0e90db6b594339181e513b60ec0843bce0a63c90ac2330aa21bb51`  
		Last Modified: Tue, 02 Aug 2022 11:37:16 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfd03b0951b798cc22685c0158dc76558cc97d72e2f54238e5a9af5be042cbef`  
		Last Modified: Tue, 02 Aug 2022 11:37:16 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
