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
$ docker pull spiped@sha256:fcecfb6a9c0c1da84943ba03f5f53edcf5508eadd518ba6f671ed2d1a34f3241
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
$ docker pull spiped@sha256:27655c03e38daa8aa4afed06a3d4c9f6127f971fe9ed16b98c8f48cc902ef314
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.3 MB (37327359 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:03b1412c46e8325a0589c93bac2d1990523e7e07b13698c2a9cb573fed4960bd`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 21 Dec 2021 01:22:43 GMT
ADD file:09675d11695f65c55efdc393ff0cd32f30194cd7d0fbef4631eebfed4414ac97 in / 
# Tue, 21 Dec 2021 01:22:43 GMT
CMD ["bash"]
# Mon, 27 Dec 2021 19:09:37 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Mon, 27 Dec 2021 19:09:40 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Mon, 27 Dec 2021 19:09:40 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Mon, 27 Dec 2021 19:10:01 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Mon, 27 Dec 2021 19:10:01 GMT
VOLUME [/spiped]
# Mon, 27 Dec 2021 19:10:01 GMT
WORKDIR /spiped
# Mon, 27 Dec 2021 19:10:02 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 27 Dec 2021 19:10:02 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 27 Dec 2021 19:10:02 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:a2abf6c4d29d43a4bf9fbb769f524d0fb36a2edab49819c1bf3e76f409f953ea`  
		Last Modified: Tue, 21 Dec 2021 01:27:48 GMT  
		Size: 31.4 MB (31357624 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d547106b69c042e6267b4030a20ff577bcfc9917ebf0a49d697c1d2819992416`  
		Last Modified: Mon, 27 Dec 2021 19:10:37 GMT  
		Size: 1.7 KB (1733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eda7224a790705cc7b53c6c57deb18f74ceeddf1a6a748cb1c59dd1d4f8b7c03`  
		Last Modified: Mon, 27 Dec 2021 19:10:37 GMT  
		Size: 1.1 KB (1055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7082f5785f33700aa63be5c0b314767d2b6039850a3dfcba2547dc823a464fff`  
		Last Modified: Mon, 27 Dec 2021 19:10:38 GMT  
		Size: 6.0 MB (5966475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8ceb17a2971caaf21db95998adb68b036ca18a5890dede0280840f93e2dabcb`  
		Last Modified: Mon, 27 Dec 2021 19:10:37 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7aed5299a2faa639446a4fc16f9364a4b444cae0a4c9855837063682ec7e4a88`  
		Last Modified: Mon, 27 Dec 2021 19:10:37 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; arm variant v5

```console
$ docker pull spiped@sha256:2bb8d6f9786620cb6d809309fe172b33c989c54afa2e70963dc028539cc711de
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.9 MB (33930835 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cb20a687f8f10c7552075675e860628f3cabd9d85426df4168e2085074497125`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 21 Dec 2021 01:50:31 GMT
ADD file:a3023f71bd93966e7db1419adda3ccde4fcc5e2e8cf58e7b13c51036ed5ff796 in / 
# Tue, 21 Dec 2021 01:50:32 GMT
CMD ["bash"]
# Mon, 27 Dec 2021 17:48:37 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Mon, 27 Dec 2021 17:48:47 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Mon, 27 Dec 2021 17:48:47 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Mon, 27 Dec 2021 17:49:39 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Mon, 27 Dec 2021 17:49:39 GMT
VOLUME [/spiped]
# Mon, 27 Dec 2021 17:49:40 GMT
WORKDIR /spiped
# Mon, 27 Dec 2021 17:49:40 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 27 Dec 2021 17:49:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 27 Dec 2021 17:49:41 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:054429d0cf4038fef39a3b5eb6ce52f600f9a2cbb71a4fb3e95ecf9b2da62581`  
		Last Modified: Tue, 21 Dec 2021 02:05:52 GMT  
		Size: 28.9 MB (28900253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:464a6f781a7abbf2236545af22e3b305148755b938eb4b3f80acfddda83fb330`  
		Last Modified: Mon, 27 Dec 2021 17:50:13 GMT  
		Size: 1.7 KB (1729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:901947b41fdff91f97c93d69ea6510e742f77e91ebe42dfb3151adcdaf03441a`  
		Last Modified: Mon, 27 Dec 2021 17:50:13 GMT  
		Size: 1.1 KB (1056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f468550fb64a624779d011e733e2288492ceeefbf1195d64f8bd54e57f57e4f`  
		Last Modified: Mon, 27 Dec 2021 17:50:18 GMT  
		Size: 5.0 MB (5027325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5aa37e6545912e2b7148568d33bbf517e5deadd118df40ce2ebe5f74710c2d66`  
		Last Modified: Mon, 27 Dec 2021 17:50:13 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18b0df784f0906422ce5e4c8eb5ee379506682e1ad31e783eeca4525c79ba55c`  
		Last Modified: Mon, 27 Dec 2021 17:50:13 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; arm variant v7

```console
$ docker pull spiped@sha256:5ff37adf5b2ffdb562129ff2c4c257c774150b80d954a9a0de388a5cd9c14ab4
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.3 MB (31311461 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:07fa1788ed3cfcc665390b07c5ea81b3818793dc7e8cd3cff01c89fc109cb0be`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 21 Dec 2021 01:59:48 GMT
ADD file:6a5555c3e40db91fae5bb112464a4c405a976de17ff64c98f25d3033a6a608d8 in / 
# Tue, 21 Dec 2021 01:59:48 GMT
CMD ["bash"]
# Mon, 27 Dec 2021 17:58:52 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Mon, 27 Dec 2021 17:58:59 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Mon, 27 Dec 2021 17:58:59 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Mon, 27 Dec 2021 17:59:46 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Mon, 27 Dec 2021 17:59:47 GMT
VOLUME [/spiped]
# Mon, 27 Dec 2021 17:59:47 GMT
WORKDIR /spiped
# Mon, 27 Dec 2021 17:59:48 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 27 Dec 2021 17:59:48 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 27 Dec 2021 17:59:49 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:d0061d6703dc4975804c3419e00c85efbe3f1b79c86d87e048fa14a683e88e31`  
		Last Modified: Tue, 21 Dec 2021 02:15:26 GMT  
		Size: 26.6 MB (26560815 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:379d1aaaf5cba2bb5aa182cc038a59938629d1ad6ec388340be3e8f34e5e65b0`  
		Last Modified: Mon, 27 Dec 2021 18:01:17 GMT  
		Size: 1.7 KB (1730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f6950d1ddd5e954a00fd9b56a607f737d4394ec2519f9c9d47ce2820e12bcfb`  
		Last Modified: Mon, 27 Dec 2021 18:01:17 GMT  
		Size: 1.1 KB (1054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6424dc46a62a8c5530fa74a2aaddc612ea6e099df67cfbe39b49dad4b2416fa4`  
		Last Modified: Mon, 27 Dec 2021 18:01:21 GMT  
		Size: 4.7 MB (4747390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b16a5e406437b655a5c55e8e9027607ad607deb3047cf60539ca94a8a6dd8be`  
		Last Modified: Mon, 27 Dec 2021 18:01:18 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c526844e52b7ac486211e17526f3bd96806de407bdad85bbace1e9268e01d2c`  
		Last Modified: Mon, 27 Dec 2021 18:01:17 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:076eed23d69622023465551277b292c4b20c7e53ff970f4ec2c0c88c721002a3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.3 MB (35310451 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:558381a048e4dd5c28f2a72bdfb28f021302afc0b9044d17373f8513e2c57b64`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 21 Dec 2021 01:42:23 GMT
ADD file:986f91febed4aa8e2072081ff8419d52ba2060510822e717086d3b3d9469e4d7 in / 
# Tue, 21 Dec 2021 01:42:24 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 13:37:31 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 21 Dec 2021 13:37:35 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 13:37:35 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Tue, 21 Dec 2021 13:37:56 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 21 Dec 2021 13:37:57 GMT
VOLUME [/spiped]
# Tue, 21 Dec 2021 13:37:58 GMT
WORKDIR /spiped
# Tue, 21 Dec 2021 13:38:00 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 21 Dec 2021 13:38:00 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 21 Dec 2021 13:38:01 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:927a35006d93ea08499b57046904046d7926cd76fb17be193e3e74f56d634a08`  
		Last Modified: Tue, 21 Dec 2021 01:48:54 GMT  
		Size: 30.0 MB (30043793 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11307cfb62981d1477c624d0946d440cae59b97d5241be5622b4a1a2170b7087`  
		Last Modified: Tue, 21 Dec 2021 13:38:28 GMT  
		Size: 1.6 KB (1618 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a0b4f4a9f9d7183fa8a6390427dd6151121434bd32d1539e46a81b5b7195e9e`  
		Last Modified: Tue, 21 Dec 2021 13:38:28 GMT  
		Size: 924.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:498cf759f2f5ad49bf12c6c9162ea1c630f9fba1005c0a5cd96d9d40f3c3bc9c`  
		Last Modified: Tue, 21 Dec 2021 13:38:30 GMT  
		Size: 5.3 MB (5263680 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7310cca9b3933670873fa963c55ba0370617e570124050a904a3eabfd50f0b8a`  
		Last Modified: Tue, 21 Dec 2021 13:38:29 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3ebb7feec0bee35aea3ecb3f98485656fa38f1ef9c1c9faccf4d07b68e3ebbe`  
		Last Modified: Tue, 21 Dec 2021 13:38:28 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; 386

```console
$ docker pull spiped@sha256:126609a7885028d241e5a5879a81db1e409324ad4299d35fa13d8cb81db7741b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.3 MB (40265566 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e63888bbd27971f057151d0bfa298298857717efa83c94412e8ccc0a77dd65d5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 21 Dec 2021 01:40:06 GMT
ADD file:6b67a0d4d176747cc8cefbd105facde82f1795467bf02eb45e8385c91cdc9c41 in / 
# Tue, 21 Dec 2021 01:40:09 GMT
CMD ["bash"]
# Mon, 27 Dec 2021 18:38:49 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Mon, 27 Dec 2021 18:38:53 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Mon, 27 Dec 2021 18:38:53 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Mon, 27 Dec 2021 18:39:18 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Mon, 27 Dec 2021 18:39:19 GMT
VOLUME [/spiped]
# Mon, 27 Dec 2021 18:39:19 GMT
WORKDIR /spiped
# Mon, 27 Dec 2021 18:39:19 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 27 Dec 2021 18:39:20 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 27 Dec 2021 18:39:20 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:9b9a100d632569e96aeb2d7b0bc45bc436609bb61335815f207994f3b557f0f7`  
		Last Modified: Tue, 21 Dec 2021 01:48:45 GMT  
		Size: 32.4 MB (32370850 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bacb6a90485f91c14c0461997a7afe3993a50f138c22f09ce39f21024c2062b8`  
		Last Modified: Mon, 27 Dec 2021 18:40:12 GMT  
		Size: 1.7 KB (1730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15dd5efb02f26ea602aaebe8f67a9f3a6947dad763a495fef3a9318f12fface9`  
		Last Modified: Mon, 27 Dec 2021 18:40:12 GMT  
		Size: 1.1 KB (1058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82f0e51dee85e4dcfc46978558a24091bc87a2559c3f2a36c3543893184a4c43`  
		Last Modified: Mon, 27 Dec 2021 18:40:14 GMT  
		Size: 7.9 MB (7891457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8925f3c59859f8e255f517eb2391360847148d17eb2715caa30753707600716`  
		Last Modified: Mon, 27 Dec 2021 18:40:12 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce7c6638e6c8f4a87a2847736b51b3093f589a601733574eb08c60e0c4707d43`  
		Last Modified: Mon, 27 Dec 2021 18:40:12 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; mips64le

```console
$ docker pull spiped@sha256:130c01d2a02859608af1ff69b512e606c6b0afab129f4f55f3b214e4439a961e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.3 MB (35327767 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8059d8a507f312d8d77dc186576b8b33cbc65306a9ff8fd918ca17b2b9163198`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 21 Dec 2021 02:09:07 GMT
ADD file:9e5931d5ed32a23b2e93bd8846258c647613637c581b6813bbc7d7e6b86bbdf5 in / 
# Tue, 21 Dec 2021 02:09:08 GMT
CMD ["bash"]
# Mon, 27 Dec 2021 18:07:30 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Mon, 27 Dec 2021 18:07:41 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Mon, 27 Dec 2021 18:07:41 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Mon, 27 Dec 2021 18:08:36 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Mon, 27 Dec 2021 18:08:36 GMT
VOLUME [/spiped]
# Mon, 27 Dec 2021 18:08:37 GMT
WORKDIR /spiped
# Mon, 27 Dec 2021 18:08:37 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 27 Dec 2021 18:08:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 27 Dec 2021 18:08:38 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:6a6edb95e2485a5b9b3c44b27b7ebad16384c0e08a3d61b7e48c65d7278763cf`  
		Last Modified: Tue, 21 Dec 2021 02:18:14 GMT  
		Size: 29.6 MB (29619177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffc41050c10fb28c363303084d216e4a84358c365e0c0c3ea780e76094ac5b62`  
		Last Modified: Mon, 27 Dec 2021 18:08:50 GMT  
		Size: 1.7 KB (1735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ccfed374e34e3e33bb1dac88ddd7d7bd1e7f5274368492e37c693a71768d15b`  
		Last Modified: Mon, 27 Dec 2021 18:08:50 GMT  
		Size: 1.0 KB (1028 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13d7546f5c1590f88787a1fc6a1c2e0d48c67af85dd4b7e8249ff573bee2daad`  
		Last Modified: Mon, 27 Dec 2021 18:08:55 GMT  
		Size: 5.7 MB (5705389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e85af9afd2d869bd928b4990f6fd908f635c5421d1dc8083fc5fd377b8bbd90`  
		Last Modified: Mon, 27 Dec 2021 18:08:50 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:870f16daf77f715fb9dc96eccb5b8d4af6d8b166fa70454d7fab605bd39d022b`  
		Last Modified: Mon, 27 Dec 2021 18:08:50 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; ppc64le

```console
$ docker pull spiped@sha256:60a73d5603e4031736039ecc463577365c1f717538d9abebaffc2f8772464669
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.3 MB (41260220 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:33b349656fc3b5caf98e066d0fdb6c40beca910e76b65314e5f1f5cfea9fc2c5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 21 Dec 2021 02:20:24 GMT
ADD file:078a17bf7e519cb7a60fbbf743ba7e5897554201cb44957154ab518d6991a033 in / 
# Tue, 21 Dec 2021 02:20:28 GMT
CMD ["bash"]
# Mon, 27 Dec 2021 18:16:48 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Mon, 27 Dec 2021 18:16:58 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Mon, 27 Dec 2021 18:17:00 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Mon, 27 Dec 2021 18:18:26 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Mon, 27 Dec 2021 18:18:28 GMT
VOLUME [/spiped]
# Mon, 27 Dec 2021 18:18:31 GMT
WORKDIR /spiped
# Mon, 27 Dec 2021 18:18:32 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 27 Dec 2021 18:18:34 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 27 Dec 2021 18:18:37 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:3345479fea0cdce1382b927b0908af4f239b288b30efa203c50edf7ac0cb055e`  
		Last Modified: Tue, 21 Dec 2021 02:29:20 GMT  
		Size: 35.3 MB (35258992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45821758d9ac9ef7ddf59278b25a098454da513ab2a4469079d31efd2872e496`  
		Last Modified: Mon, 27 Dec 2021 18:20:01 GMT  
		Size: 1.7 KB (1734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6621a4339ab8321307888b642f6c34ede9ba4af6ac0ed96e946ac50ec1227849`  
		Last Modified: Mon, 27 Dec 2021 18:20:01 GMT  
		Size: 1.1 KB (1057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2eb85ea75c9e8b313cfbfc6e4cfef155d0183d2f926c786afe58fc17f96afdae`  
		Last Modified: Mon, 27 Dec 2021 18:20:03 GMT  
		Size: 6.0 MB (5997966 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92b8831f840f6baaf8d56f6cae0b098c6a56d239108b4ae79ca3788881609e16`  
		Last Modified: Mon, 27 Dec 2021 18:20:01 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:918e7af5ea63b6fcb7ce923b4e73eaf873a1247710e432fc8214fd19aad04405`  
		Last Modified: Mon, 27 Dec 2021 18:20:01 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; s390x

```console
$ docker pull spiped@sha256:85d5e0719445d2cdab3cbf858a459655e3240a92ee8d2f2f802f6ac1b211f948
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.8 MB (34830564 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c2df5426aa3ed82a47988087e8347fbcad4453d2a97b19988ddb6026a0947c78`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 21 Dec 2021 01:42:27 GMT
ADD file:c8a482d41bf09dfb6484bf2a6e38535bf0594d26dd6eedd5abde4e3cc811fa6c in / 
# Tue, 21 Dec 2021 01:42:29 GMT
CMD ["bash"]
# Mon, 27 Dec 2021 18:41:39 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Mon, 27 Dec 2021 18:41:42 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Mon, 27 Dec 2021 18:41:42 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Mon, 27 Dec 2021 18:41:54 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Mon, 27 Dec 2021 18:41:55 GMT
VOLUME [/spiped]
# Mon, 27 Dec 2021 18:41:55 GMT
WORKDIR /spiped
# Mon, 27 Dec 2021 18:41:55 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 27 Dec 2021 18:41:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 27 Dec 2021 18:41:55 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:12562551722a758d23ceea9abcdc2bee737e38c8f62a0f3d3afb2cc2626c28b1`  
		Last Modified: Tue, 21 Dec 2021 01:48:15 GMT  
		Size: 29.6 MB (29641636 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e50be5fdb0a5e34432208396d23522b1701f3dff2f0ad3d78fbd79b6b41b6ce`  
		Last Modified: Mon, 27 Dec 2021 18:42:37 GMT  
		Size: 1.7 KB (1739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a42e79bc5e5489f7b5513adce4e87bffd082bb140296c35dd729fa90a5a4868`  
		Last Modified: Mon, 27 Dec 2021 18:42:37 GMT  
		Size: 1.1 KB (1052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e1da3833503470ef9b807b846f2ff4fbaaab0831b1447b2f18bba93952c3435`  
		Last Modified: Mon, 27 Dec 2021 18:42:38 GMT  
		Size: 5.2 MB (5185667 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4c82c9810dbf5e873e822ea28782e813bd5277a73013e0e015bf69827be95f1`  
		Last Modified: Mon, 27 Dec 2021 18:42:37 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51b12ef5c112d47a91c90766ac49e1b42fd0a2a3a6c3d6af4b2349c285ea742c`  
		Last Modified: Mon, 27 Dec 2021 18:42:37 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:1-alpine`

```console
$ docker pull spiped@sha256:35234b9a4b8b07015b0a9b6712fd3440cc9738a2ac14760483e070c75a602e70
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
$ docker pull spiped@sha256:f4aaae543ff5aba181d531aa5504251d883a40559812a85cff78c7526d3f713e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4523758 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d71e35e9a762b19f1a767061f3cf181454d7090d64dec7acef852f68d4c01262`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 24 Nov 2021 20:19:40 GMT
ADD file:9233f6f2237d79659a9521f7e390df217cec49f1a8aa3a12147bbca1956acdb9 in / 
# Wed, 24 Nov 2021 20:19:40 GMT
CMD ["/bin/sh"]
# Mon, 27 Dec 2021 19:10:10 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Mon, 27 Dec 2021 19:10:11 GMT
RUN apk add --no-cache libssl1.1
# Mon, 27 Dec 2021 19:10:11 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Mon, 27 Dec 2021 19:10:22 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Mon, 27 Dec 2021 19:10:22 GMT
VOLUME [/spiped]
# Mon, 27 Dec 2021 19:10:22 GMT
WORKDIR /spiped
# Mon, 27 Dec 2021 19:10:22 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 27 Dec 2021 19:10:23 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 27 Dec 2021 19:10:23 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:59bf1c3509f33515622619af21ed55bbe26d24913cedbca106468a5fb37a50c3`  
		Last Modified: Wed, 24 Nov 2021 20:20:05 GMT  
		Size: 2.8 MB (2818413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50c602680384586a0fe7febde9f529aea001928a6d26e84d9a3f7be94049ef27`  
		Last Modified: Mon, 27 Dec 2021 19:10:53 GMT  
		Size: 1.3 KB (1265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee913a58b01d029ed458f92226b5b52747e0877c39585d9f93ec5dd2ef0a8cf9`  
		Last Modified: Mon, 27 Dec 2021 19:10:53 GMT  
		Size: 7.7 KB (7749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd8bf950f1ef1b7c96ba1781b5a87d4044135ae197871b261e86d74bc35a8bf5`  
		Last Modified: Mon, 27 Dec 2021 19:10:54 GMT  
		Size: 1.7 MB (1695862 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56d41f282509324afd98cc83dab31aee8ba6459973698c8ccaf3978cddc4ede4`  
		Last Modified: Mon, 27 Dec 2021 19:10:53 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8ba766abbc809d26737c9cc94fbe15a6311c603bfd673bd6db553169dd0f141`  
		Last Modified: Mon, 27 Dec 2021 19:10:53 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; arm variant v6

```console
$ docker pull spiped@sha256:b6482b55d0b7700b0393783f0ea8e49e6a4329c07187fdf826b6902d0ccfa3e6
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.1 MB (4080480 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1df9593d1c7a93c5f606ef97c05cc8d86e1a5bce25cd9895c104e2e1a7edbe19`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 24 Nov 2021 21:08:16 GMT
ADD file:61137e0aa49ba06f57ac69466fe2fb116f580b5e6159d56f846b1d72c4a3c814 in / 
# Wed, 24 Nov 2021 21:08:16 GMT
CMD ["/bin/sh"]
# Mon, 27 Dec 2021 17:49:44 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Mon, 27 Dec 2021 17:49:46 GMT
RUN apk add --no-cache libssl1.1
# Mon, 27 Dec 2021 17:49:47 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Mon, 27 Dec 2021 17:50:06 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Mon, 27 Dec 2021 17:50:07 GMT
VOLUME [/spiped]
# Mon, 27 Dec 2021 17:50:07 GMT
WORKDIR /spiped
# Mon, 27 Dec 2021 17:50:08 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 27 Dec 2021 17:50:08 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 27 Dec 2021 17:50:09 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:e4a43de54da9e309482f6762f0c11f5f547cd8fd61a49c5f158453066162023e`  
		Last Modified: Wed, 24 Nov 2021 21:09:46 GMT  
		Size: 2.6 MB (2631421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c04f27a458746dfc1d07b0b03b9b8f205b08ebef9d6060ef92027b709fee313e`  
		Last Modified: Mon, 27 Dec 2021 17:50:41 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fffa3b0ec9bb32d2efab9fa903af078baf37201f4ec2026c0afce9c14156229`  
		Last Modified: Mon, 27 Dec 2021 17:50:41 GMT  
		Size: 7.7 KB (7743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e2344d51f830abe738f710343c04e056b2ec80e33a48522878caa568c9f553c`  
		Last Modified: Mon, 27 Dec 2021 17:50:42 GMT  
		Size: 1.4 MB (1439576 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd3eeeb2545dce6884a99d866ca20bd742d7e133aacf869b4cddbe974bfde627`  
		Last Modified: Mon, 27 Dec 2021 17:50:41 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2681e39729f29c202bc97138be5a28bb84d92220ffe45df47fb643301eef46aa`  
		Last Modified: Mon, 27 Dec 2021 17:50:41 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; arm variant v7

```console
$ docker pull spiped@sha256:277d22d33ab8cd23ff5bf04d4e60841c8a335de8fdb772173601e9a4d4cb00bf
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.8 MB (3802328 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2f94c64b2c706a58b82aa60bafca69c1fd15fb76714e5ca4aae0f1e4a47e3f1d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 24 Nov 2021 21:42:11 GMT
ADD file:ca436da5b0bfc9c0e2fc685533c6628918000c8fff109fe9a8da625b9a798002 in / 
# Wed, 24 Nov 2021 21:42:11 GMT
CMD ["/bin/sh"]
# Mon, 27 Dec 2021 18:00:04 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Mon, 27 Dec 2021 18:00:06 GMT
RUN apk add --no-cache libssl1.1
# Mon, 27 Dec 2021 18:00:06 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Mon, 27 Dec 2021 18:00:25 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Mon, 27 Dec 2021 18:00:26 GMT
VOLUME [/spiped]
# Mon, 27 Dec 2021 18:00:26 GMT
WORKDIR /spiped
# Mon, 27 Dec 2021 18:00:27 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 27 Dec 2021 18:00:27 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 27 Dec 2021 18:00:28 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:5480d2ca1740c20ce17652e01ed2265cdc914458acd41256a2b1ccff28f2762c`  
		Last Modified: Wed, 24 Nov 2021 21:43:40 GMT  
		Size: 2.4 MB (2434764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fca194041621ab40d8e7f24b7f7e82aa07760b2dafcd26472bd7fae96171989a`  
		Last Modified: Mon, 27 Dec 2021 18:01:41 GMT  
		Size: 1.3 KB (1267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7e934f04cb0ca6a107389bcb614eb02143fb079eef09a47a9248e3c4ff07864`  
		Last Modified: Mon, 27 Dec 2021 18:01:41 GMT  
		Size: 7.7 KB (7749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4111e5d44f2316d799c8b9144d8f35765b0bf330b8d596d99e504969cd48e07a`  
		Last Modified: Mon, 27 Dec 2021 18:01:42 GMT  
		Size: 1.4 MB (1358077 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f46d751b026ad913b2a48630c96460959a733e75728d55aafbd389197bf81857`  
		Last Modified: Mon, 27 Dec 2021 18:01:41 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5140561b01c4c6ae8b47c729fd289d7eef4a2b0e9c427a6bd35a86747e966206`  
		Last Modified: Mon, 27 Dec 2021 18:01:41 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:cbaa0533059fb17c768fe05790c3675b5b5cecf35f0b461e5347d763b1322af8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 MB (2932006 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a49787cc7861893f9d6020342db1639e60d7af6850ca4866d08840d8438a2b0c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 12 Nov 2021 16:39:58 GMT
ADD file:400c0466b29ccad54e0f6c0acef22542992828678c96693ef1f9f4d0551935d8 in / 
# Fri, 12 Nov 2021 16:39:58 GMT
CMD ["/bin/sh"]
# Fri, 12 Nov 2021 18:19:31 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 12 Nov 2021 18:19:33 GMT
RUN apk add --no-cache libssl1.1
# Fri, 12 Nov 2021 18:19:34 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 12 Nov 2021 18:19:54 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 12 Nov 2021 18:19:55 GMT
VOLUME [/spiped]
# Fri, 12 Nov 2021 18:19:56 GMT
WORKDIR /spiped
# Fri, 12 Nov 2021 18:19:58 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 12 Nov 2021 18:19:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 12 Nov 2021 18:19:59 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:be307f383ecc62b27a29b599c3fc9d3129693a798e7fcce614f09174cfe2d354`  
		Last Modified: Fri, 12 Nov 2021 16:40:59 GMT  
		Size: 2.7 MB (2717700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffbcce6bf922e4817964b0a9575d547fbb39004874a87c290658dcbb8939209e`  
		Last Modified: Fri, 12 Nov 2021 18:20:41 GMT  
		Size: 1.2 KB (1239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b342172a90f6f6a837eeb8f0025e02facad5a97fdd12c0aeac68c2411928d16f`  
		Last Modified: Fri, 12 Nov 2021 18:20:41 GMT  
		Size: 7.8 KB (7751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd8a670bc36ab2f74e650d7cb573c4c3542673b9488e2659efbc0d6b9db67529`  
		Last Modified: Fri, 12 Nov 2021 18:20:41 GMT  
		Size: 204.9 KB (204879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:698de19c09a4c9763fb04c4946f3bffafe6556fcfe73a3d55bbb4255f65bd458`  
		Last Modified: Fri, 12 Nov 2021 18:20:41 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1d1aa9a890181cdc95e60ea01849306cb72c967e13716722baa68c7bca76fdb`  
		Last Modified: Fri, 12 Nov 2021 18:20:42 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; 386

```console
$ docker pull spiped@sha256:fc962e82018b393667a7d2b43c9bee0b19c4650fadcc16335cf984b44d859d65
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4539662 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:64dc6529164f107ee83f0edafa6bcf506960ffc646e0e9e161cb2640feb90f96`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 24 Nov 2021 20:53:48 GMT
ADD file:b9a17131c440053f2f67e127b447645f25fd7de2d6caca42f569cafab6291855 in / 
# Wed, 24 Nov 2021 20:53:48 GMT
CMD ["/bin/sh"]
# Mon, 27 Dec 2021 18:39:31 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Mon, 27 Dec 2021 18:39:32 GMT
RUN apk add --no-cache libssl1.1
# Mon, 27 Dec 2021 18:39:33 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Mon, 27 Dec 2021 18:39:45 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Mon, 27 Dec 2021 18:39:45 GMT
VOLUME [/spiped]
# Mon, 27 Dec 2021 18:39:45 GMT
WORKDIR /spiped
# Mon, 27 Dec 2021 18:39:46 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 27 Dec 2021 18:39:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 27 Dec 2021 18:39:46 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:e6889e0d66307a4b916fc844f2dcbc03245c63bc4189dd3e88126d9dcf2f9231`  
		Last Modified: Wed, 24 Nov 2021 20:54:48 GMT  
		Size: 2.8 MB (2827117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc39bdf14cf5dcbf704b50f736d82a339b1879574765ef87fbbf5ecb8d7d574e`  
		Last Modified: Mon, 27 Dec 2021 18:40:32 GMT  
		Size: 1.3 KB (1266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7128f9e1b03ce01ba1b51bce7aa1bc585b6c3e6ce1650259721463f363e9aaab`  
		Last Modified: Mon, 27 Dec 2021 18:40:32 GMT  
		Size: 7.8 KB (7750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb2ebf4c9a2525659cebde6ee501a457c4a31d364f3f568be0f076191d96855d`  
		Last Modified: Mon, 27 Dec 2021 18:40:33 GMT  
		Size: 1.7 MB (1703060 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75adf8fe66ad441b9c8e209efcc7d5b68b61c6a33e05b3aed401756e55493d07`  
		Last Modified: Mon, 27 Dec 2021 18:40:32 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99b656b54398310f3a0f295c7737034732b9ee5c7e294ad5df27230309fff8ae`  
		Last Modified: Mon, 27 Dec 2021 18:40:32 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; ppc64le

```console
$ docker pull spiped@sha256:bdb5c0f748fb29dd4c96f71d1eec1c471f348b68e39063a5674e88c6655400ac
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.4 MB (4447359 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c2ab0ba82f0f9badd5246249195a67d4e12bc4f6cfb1822b3454aca1c3dae586`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 24 Nov 2021 20:20:16 GMT
ADD file:57115dca2eb707f46b6301e75174e6aa316fb02ac28643b91429b75be51bd8c8 in / 
# Wed, 24 Nov 2021 20:20:20 GMT
CMD ["/bin/sh"]
# Mon, 27 Dec 2021 18:18:59 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Mon, 27 Dec 2021 18:19:06 GMT
RUN apk add --no-cache libssl1.1
# Mon, 27 Dec 2021 18:19:08 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Mon, 27 Dec 2021 18:19:22 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Mon, 27 Dec 2021 18:19:25 GMT
VOLUME [/spiped]
# Mon, 27 Dec 2021 18:19:28 GMT
WORKDIR /spiped
# Mon, 27 Dec 2021 18:19:28 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 27 Dec 2021 18:19:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 27 Dec 2021 18:19:33 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:159b5dcb1717c815c76ff5ea1db730e18e8609c9090238e43282856db9e71f47`  
		Last Modified: Wed, 24 Nov 2021 20:21:14 GMT  
		Size: 2.8 MB (2814780 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5ef2b17ec4445a63d712289fc62b0e3e30ab15992e0a0d38ab25e290abcb38e`  
		Last Modified: Mon, 27 Dec 2021 18:20:21 GMT  
		Size: 1.3 KB (1274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:210460e69fcfc508eae94f5666c4fc57c0cdf6163c3a6e39710f5da7a2e5ceb6`  
		Last Modified: Mon, 27 Dec 2021 18:20:21 GMT  
		Size: 7.7 KB (7737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0860c3c69dcd2673558f15fc9c46c8447274ce23c207e936804fe5a268e5e7f`  
		Last Modified: Mon, 27 Dec 2021 18:20:22 GMT  
		Size: 1.6 MB (1623097 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13cd96844150db5d01e32349b5f650aafd01dd1789c2a11fee82b6f55bd43560`  
		Last Modified: Mon, 27 Dec 2021 18:20:21 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a52b1de785dfc0bc3d07ee3d3f619d0681bc34b7eeee205db16da01946663a91`  
		Last Modified: Mon, 27 Dec 2021 18:20:21 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; s390x

```console
$ docker pull spiped@sha256:e5972c57d035e42883aca7354deb92cd65a9bbbc8d5d6aaa8b364891cbdba20d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.0 MB (4034365 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6b297cc2c896c2d11d20abe50ce763f606504b9aad55d18a6c8bcf3407db63c8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 24 Nov 2021 20:41:23 GMT
ADD file:cd24c711a2ef431b3ff94f9a02bfc42f159bc60de1d0eceecafea4e8af02441d in / 
# Wed, 24 Nov 2021 20:41:23 GMT
CMD ["/bin/sh"]
# Mon, 27 Dec 2021 18:42:02 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Mon, 27 Dec 2021 18:42:04 GMT
RUN apk add --no-cache libssl1.1
# Mon, 27 Dec 2021 18:42:04 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Mon, 27 Dec 2021 18:42:09 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Mon, 27 Dec 2021 18:42:09 GMT
VOLUME [/spiped]
# Mon, 27 Dec 2021 18:42:09 GMT
WORKDIR /spiped
# Mon, 27 Dec 2021 18:42:10 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 27 Dec 2021 18:42:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 27 Dec 2021 18:42:10 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:d6baca485f3d0f7c77221be60fbef5db014a5ef9d8f53db4a310c947c690d189`  
		Last Modified: Wed, 24 Nov 2021 20:42:15 GMT  
		Size: 2.6 MB (2605944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:631b52683dec736314bc4a995e6d4aa8fe70ccec0ccb0b4f0349543c0b9d315d`  
		Last Modified: Mon, 27 Dec 2021 18:42:54 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8a99397842c922d6589a78e8df8f8b4feac626485047c36e902a2966e19dfe2`  
		Last Modified: Mon, 27 Dec 2021 18:42:54 GMT  
		Size: 7.7 KB (7743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:556dc6882e78ba3518dbab7eaae8412b06f9ad7e09122f6478d9d1cc80b978e4`  
		Last Modified: Mon, 27 Dec 2021 18:42:55 GMT  
		Size: 1.4 MB (1418939 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9680c33180071ffeb1ac5cfe629daff266a5cf86a4072e251e4b0bef70d20b3`  
		Last Modified: Mon, 27 Dec 2021 18:42:54 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2742416115dba0ead2f2dc1f9aa438a1ef9179b4e11cfd9d665c918f92b53c55`  
		Last Modified: Mon, 27 Dec 2021 18:42:54 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:1.6`

```console
$ docker pull spiped@sha256:fcecfb6a9c0c1da84943ba03f5f53edcf5508eadd518ba6f671ed2d1a34f3241
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
$ docker pull spiped@sha256:27655c03e38daa8aa4afed06a3d4c9f6127f971fe9ed16b98c8f48cc902ef314
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.3 MB (37327359 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:03b1412c46e8325a0589c93bac2d1990523e7e07b13698c2a9cb573fed4960bd`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 21 Dec 2021 01:22:43 GMT
ADD file:09675d11695f65c55efdc393ff0cd32f30194cd7d0fbef4631eebfed4414ac97 in / 
# Tue, 21 Dec 2021 01:22:43 GMT
CMD ["bash"]
# Mon, 27 Dec 2021 19:09:37 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Mon, 27 Dec 2021 19:09:40 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Mon, 27 Dec 2021 19:09:40 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Mon, 27 Dec 2021 19:10:01 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Mon, 27 Dec 2021 19:10:01 GMT
VOLUME [/spiped]
# Mon, 27 Dec 2021 19:10:01 GMT
WORKDIR /spiped
# Mon, 27 Dec 2021 19:10:02 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 27 Dec 2021 19:10:02 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 27 Dec 2021 19:10:02 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:a2abf6c4d29d43a4bf9fbb769f524d0fb36a2edab49819c1bf3e76f409f953ea`  
		Last Modified: Tue, 21 Dec 2021 01:27:48 GMT  
		Size: 31.4 MB (31357624 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d547106b69c042e6267b4030a20ff577bcfc9917ebf0a49d697c1d2819992416`  
		Last Modified: Mon, 27 Dec 2021 19:10:37 GMT  
		Size: 1.7 KB (1733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eda7224a790705cc7b53c6c57deb18f74ceeddf1a6a748cb1c59dd1d4f8b7c03`  
		Last Modified: Mon, 27 Dec 2021 19:10:37 GMT  
		Size: 1.1 KB (1055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7082f5785f33700aa63be5c0b314767d2b6039850a3dfcba2547dc823a464fff`  
		Last Modified: Mon, 27 Dec 2021 19:10:38 GMT  
		Size: 6.0 MB (5966475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8ceb17a2971caaf21db95998adb68b036ca18a5890dede0280840f93e2dabcb`  
		Last Modified: Mon, 27 Dec 2021 19:10:37 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7aed5299a2faa639446a4fc16f9364a4b444cae0a4c9855837063682ec7e4a88`  
		Last Modified: Mon, 27 Dec 2021 19:10:37 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; arm variant v5

```console
$ docker pull spiped@sha256:2bb8d6f9786620cb6d809309fe172b33c989c54afa2e70963dc028539cc711de
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.9 MB (33930835 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cb20a687f8f10c7552075675e860628f3cabd9d85426df4168e2085074497125`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 21 Dec 2021 01:50:31 GMT
ADD file:a3023f71bd93966e7db1419adda3ccde4fcc5e2e8cf58e7b13c51036ed5ff796 in / 
# Tue, 21 Dec 2021 01:50:32 GMT
CMD ["bash"]
# Mon, 27 Dec 2021 17:48:37 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Mon, 27 Dec 2021 17:48:47 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Mon, 27 Dec 2021 17:48:47 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Mon, 27 Dec 2021 17:49:39 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Mon, 27 Dec 2021 17:49:39 GMT
VOLUME [/spiped]
# Mon, 27 Dec 2021 17:49:40 GMT
WORKDIR /spiped
# Mon, 27 Dec 2021 17:49:40 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 27 Dec 2021 17:49:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 27 Dec 2021 17:49:41 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:054429d0cf4038fef39a3b5eb6ce52f600f9a2cbb71a4fb3e95ecf9b2da62581`  
		Last Modified: Tue, 21 Dec 2021 02:05:52 GMT  
		Size: 28.9 MB (28900253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:464a6f781a7abbf2236545af22e3b305148755b938eb4b3f80acfddda83fb330`  
		Last Modified: Mon, 27 Dec 2021 17:50:13 GMT  
		Size: 1.7 KB (1729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:901947b41fdff91f97c93d69ea6510e742f77e91ebe42dfb3151adcdaf03441a`  
		Last Modified: Mon, 27 Dec 2021 17:50:13 GMT  
		Size: 1.1 KB (1056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f468550fb64a624779d011e733e2288492ceeefbf1195d64f8bd54e57f57e4f`  
		Last Modified: Mon, 27 Dec 2021 17:50:18 GMT  
		Size: 5.0 MB (5027325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5aa37e6545912e2b7148568d33bbf517e5deadd118df40ce2ebe5f74710c2d66`  
		Last Modified: Mon, 27 Dec 2021 17:50:13 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18b0df784f0906422ce5e4c8eb5ee379506682e1ad31e783eeca4525c79ba55c`  
		Last Modified: Mon, 27 Dec 2021 17:50:13 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; arm variant v7

```console
$ docker pull spiped@sha256:5ff37adf5b2ffdb562129ff2c4c257c774150b80d954a9a0de388a5cd9c14ab4
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.3 MB (31311461 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:07fa1788ed3cfcc665390b07c5ea81b3818793dc7e8cd3cff01c89fc109cb0be`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 21 Dec 2021 01:59:48 GMT
ADD file:6a5555c3e40db91fae5bb112464a4c405a976de17ff64c98f25d3033a6a608d8 in / 
# Tue, 21 Dec 2021 01:59:48 GMT
CMD ["bash"]
# Mon, 27 Dec 2021 17:58:52 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Mon, 27 Dec 2021 17:58:59 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Mon, 27 Dec 2021 17:58:59 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Mon, 27 Dec 2021 17:59:46 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Mon, 27 Dec 2021 17:59:47 GMT
VOLUME [/spiped]
# Mon, 27 Dec 2021 17:59:47 GMT
WORKDIR /spiped
# Mon, 27 Dec 2021 17:59:48 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 27 Dec 2021 17:59:48 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 27 Dec 2021 17:59:49 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:d0061d6703dc4975804c3419e00c85efbe3f1b79c86d87e048fa14a683e88e31`  
		Last Modified: Tue, 21 Dec 2021 02:15:26 GMT  
		Size: 26.6 MB (26560815 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:379d1aaaf5cba2bb5aa182cc038a59938629d1ad6ec388340be3e8f34e5e65b0`  
		Last Modified: Mon, 27 Dec 2021 18:01:17 GMT  
		Size: 1.7 KB (1730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f6950d1ddd5e954a00fd9b56a607f737d4394ec2519f9c9d47ce2820e12bcfb`  
		Last Modified: Mon, 27 Dec 2021 18:01:17 GMT  
		Size: 1.1 KB (1054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6424dc46a62a8c5530fa74a2aaddc612ea6e099df67cfbe39b49dad4b2416fa4`  
		Last Modified: Mon, 27 Dec 2021 18:01:21 GMT  
		Size: 4.7 MB (4747390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b16a5e406437b655a5c55e8e9027607ad607deb3047cf60539ca94a8a6dd8be`  
		Last Modified: Mon, 27 Dec 2021 18:01:18 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c526844e52b7ac486211e17526f3bd96806de407bdad85bbace1e9268e01d2c`  
		Last Modified: Mon, 27 Dec 2021 18:01:17 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:076eed23d69622023465551277b292c4b20c7e53ff970f4ec2c0c88c721002a3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.3 MB (35310451 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:558381a048e4dd5c28f2a72bdfb28f021302afc0b9044d17373f8513e2c57b64`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 21 Dec 2021 01:42:23 GMT
ADD file:986f91febed4aa8e2072081ff8419d52ba2060510822e717086d3b3d9469e4d7 in / 
# Tue, 21 Dec 2021 01:42:24 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 13:37:31 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 21 Dec 2021 13:37:35 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 13:37:35 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Tue, 21 Dec 2021 13:37:56 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 21 Dec 2021 13:37:57 GMT
VOLUME [/spiped]
# Tue, 21 Dec 2021 13:37:58 GMT
WORKDIR /spiped
# Tue, 21 Dec 2021 13:38:00 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 21 Dec 2021 13:38:00 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 21 Dec 2021 13:38:01 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:927a35006d93ea08499b57046904046d7926cd76fb17be193e3e74f56d634a08`  
		Last Modified: Tue, 21 Dec 2021 01:48:54 GMT  
		Size: 30.0 MB (30043793 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11307cfb62981d1477c624d0946d440cae59b97d5241be5622b4a1a2170b7087`  
		Last Modified: Tue, 21 Dec 2021 13:38:28 GMT  
		Size: 1.6 KB (1618 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a0b4f4a9f9d7183fa8a6390427dd6151121434bd32d1539e46a81b5b7195e9e`  
		Last Modified: Tue, 21 Dec 2021 13:38:28 GMT  
		Size: 924.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:498cf759f2f5ad49bf12c6c9162ea1c630f9fba1005c0a5cd96d9d40f3c3bc9c`  
		Last Modified: Tue, 21 Dec 2021 13:38:30 GMT  
		Size: 5.3 MB (5263680 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7310cca9b3933670873fa963c55ba0370617e570124050a904a3eabfd50f0b8a`  
		Last Modified: Tue, 21 Dec 2021 13:38:29 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3ebb7feec0bee35aea3ecb3f98485656fa38f1ef9c1c9faccf4d07b68e3ebbe`  
		Last Modified: Tue, 21 Dec 2021 13:38:28 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; 386

```console
$ docker pull spiped@sha256:126609a7885028d241e5a5879a81db1e409324ad4299d35fa13d8cb81db7741b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.3 MB (40265566 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e63888bbd27971f057151d0bfa298298857717efa83c94412e8ccc0a77dd65d5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 21 Dec 2021 01:40:06 GMT
ADD file:6b67a0d4d176747cc8cefbd105facde82f1795467bf02eb45e8385c91cdc9c41 in / 
# Tue, 21 Dec 2021 01:40:09 GMT
CMD ["bash"]
# Mon, 27 Dec 2021 18:38:49 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Mon, 27 Dec 2021 18:38:53 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Mon, 27 Dec 2021 18:38:53 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Mon, 27 Dec 2021 18:39:18 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Mon, 27 Dec 2021 18:39:19 GMT
VOLUME [/spiped]
# Mon, 27 Dec 2021 18:39:19 GMT
WORKDIR /spiped
# Mon, 27 Dec 2021 18:39:19 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 27 Dec 2021 18:39:20 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 27 Dec 2021 18:39:20 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:9b9a100d632569e96aeb2d7b0bc45bc436609bb61335815f207994f3b557f0f7`  
		Last Modified: Tue, 21 Dec 2021 01:48:45 GMT  
		Size: 32.4 MB (32370850 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bacb6a90485f91c14c0461997a7afe3993a50f138c22f09ce39f21024c2062b8`  
		Last Modified: Mon, 27 Dec 2021 18:40:12 GMT  
		Size: 1.7 KB (1730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15dd5efb02f26ea602aaebe8f67a9f3a6947dad763a495fef3a9318f12fface9`  
		Last Modified: Mon, 27 Dec 2021 18:40:12 GMT  
		Size: 1.1 KB (1058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82f0e51dee85e4dcfc46978558a24091bc87a2559c3f2a36c3543893184a4c43`  
		Last Modified: Mon, 27 Dec 2021 18:40:14 GMT  
		Size: 7.9 MB (7891457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8925f3c59859f8e255f517eb2391360847148d17eb2715caa30753707600716`  
		Last Modified: Mon, 27 Dec 2021 18:40:12 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce7c6638e6c8f4a87a2847736b51b3093f589a601733574eb08c60e0c4707d43`  
		Last Modified: Mon, 27 Dec 2021 18:40:12 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; mips64le

```console
$ docker pull spiped@sha256:130c01d2a02859608af1ff69b512e606c6b0afab129f4f55f3b214e4439a961e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.3 MB (35327767 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8059d8a507f312d8d77dc186576b8b33cbc65306a9ff8fd918ca17b2b9163198`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 21 Dec 2021 02:09:07 GMT
ADD file:9e5931d5ed32a23b2e93bd8846258c647613637c581b6813bbc7d7e6b86bbdf5 in / 
# Tue, 21 Dec 2021 02:09:08 GMT
CMD ["bash"]
# Mon, 27 Dec 2021 18:07:30 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Mon, 27 Dec 2021 18:07:41 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Mon, 27 Dec 2021 18:07:41 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Mon, 27 Dec 2021 18:08:36 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Mon, 27 Dec 2021 18:08:36 GMT
VOLUME [/spiped]
# Mon, 27 Dec 2021 18:08:37 GMT
WORKDIR /spiped
# Mon, 27 Dec 2021 18:08:37 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 27 Dec 2021 18:08:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 27 Dec 2021 18:08:38 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:6a6edb95e2485a5b9b3c44b27b7ebad16384c0e08a3d61b7e48c65d7278763cf`  
		Last Modified: Tue, 21 Dec 2021 02:18:14 GMT  
		Size: 29.6 MB (29619177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffc41050c10fb28c363303084d216e4a84358c365e0c0c3ea780e76094ac5b62`  
		Last Modified: Mon, 27 Dec 2021 18:08:50 GMT  
		Size: 1.7 KB (1735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ccfed374e34e3e33bb1dac88ddd7d7bd1e7f5274368492e37c693a71768d15b`  
		Last Modified: Mon, 27 Dec 2021 18:08:50 GMT  
		Size: 1.0 KB (1028 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13d7546f5c1590f88787a1fc6a1c2e0d48c67af85dd4b7e8249ff573bee2daad`  
		Last Modified: Mon, 27 Dec 2021 18:08:55 GMT  
		Size: 5.7 MB (5705389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e85af9afd2d869bd928b4990f6fd908f635c5421d1dc8083fc5fd377b8bbd90`  
		Last Modified: Mon, 27 Dec 2021 18:08:50 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:870f16daf77f715fb9dc96eccb5b8d4af6d8b166fa70454d7fab605bd39d022b`  
		Last Modified: Mon, 27 Dec 2021 18:08:50 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; ppc64le

```console
$ docker pull spiped@sha256:60a73d5603e4031736039ecc463577365c1f717538d9abebaffc2f8772464669
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.3 MB (41260220 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:33b349656fc3b5caf98e066d0fdb6c40beca910e76b65314e5f1f5cfea9fc2c5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 21 Dec 2021 02:20:24 GMT
ADD file:078a17bf7e519cb7a60fbbf743ba7e5897554201cb44957154ab518d6991a033 in / 
# Tue, 21 Dec 2021 02:20:28 GMT
CMD ["bash"]
# Mon, 27 Dec 2021 18:16:48 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Mon, 27 Dec 2021 18:16:58 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Mon, 27 Dec 2021 18:17:00 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Mon, 27 Dec 2021 18:18:26 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Mon, 27 Dec 2021 18:18:28 GMT
VOLUME [/spiped]
# Mon, 27 Dec 2021 18:18:31 GMT
WORKDIR /spiped
# Mon, 27 Dec 2021 18:18:32 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 27 Dec 2021 18:18:34 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 27 Dec 2021 18:18:37 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:3345479fea0cdce1382b927b0908af4f239b288b30efa203c50edf7ac0cb055e`  
		Last Modified: Tue, 21 Dec 2021 02:29:20 GMT  
		Size: 35.3 MB (35258992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45821758d9ac9ef7ddf59278b25a098454da513ab2a4469079d31efd2872e496`  
		Last Modified: Mon, 27 Dec 2021 18:20:01 GMT  
		Size: 1.7 KB (1734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6621a4339ab8321307888b642f6c34ede9ba4af6ac0ed96e946ac50ec1227849`  
		Last Modified: Mon, 27 Dec 2021 18:20:01 GMT  
		Size: 1.1 KB (1057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2eb85ea75c9e8b313cfbfc6e4cfef155d0183d2f926c786afe58fc17f96afdae`  
		Last Modified: Mon, 27 Dec 2021 18:20:03 GMT  
		Size: 6.0 MB (5997966 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92b8831f840f6baaf8d56f6cae0b098c6a56d239108b4ae79ca3788881609e16`  
		Last Modified: Mon, 27 Dec 2021 18:20:01 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:918e7af5ea63b6fcb7ce923b4e73eaf873a1247710e432fc8214fd19aad04405`  
		Last Modified: Mon, 27 Dec 2021 18:20:01 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; s390x

```console
$ docker pull spiped@sha256:85d5e0719445d2cdab3cbf858a459655e3240a92ee8d2f2f802f6ac1b211f948
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.8 MB (34830564 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c2df5426aa3ed82a47988087e8347fbcad4453d2a97b19988ddb6026a0947c78`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 21 Dec 2021 01:42:27 GMT
ADD file:c8a482d41bf09dfb6484bf2a6e38535bf0594d26dd6eedd5abde4e3cc811fa6c in / 
# Tue, 21 Dec 2021 01:42:29 GMT
CMD ["bash"]
# Mon, 27 Dec 2021 18:41:39 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Mon, 27 Dec 2021 18:41:42 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Mon, 27 Dec 2021 18:41:42 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Mon, 27 Dec 2021 18:41:54 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Mon, 27 Dec 2021 18:41:55 GMT
VOLUME [/spiped]
# Mon, 27 Dec 2021 18:41:55 GMT
WORKDIR /spiped
# Mon, 27 Dec 2021 18:41:55 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 27 Dec 2021 18:41:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 27 Dec 2021 18:41:55 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:12562551722a758d23ceea9abcdc2bee737e38c8f62a0f3d3afb2cc2626c28b1`  
		Last Modified: Tue, 21 Dec 2021 01:48:15 GMT  
		Size: 29.6 MB (29641636 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e50be5fdb0a5e34432208396d23522b1701f3dff2f0ad3d78fbd79b6b41b6ce`  
		Last Modified: Mon, 27 Dec 2021 18:42:37 GMT  
		Size: 1.7 KB (1739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a42e79bc5e5489f7b5513adce4e87bffd082bb140296c35dd729fa90a5a4868`  
		Last Modified: Mon, 27 Dec 2021 18:42:37 GMT  
		Size: 1.1 KB (1052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e1da3833503470ef9b807b846f2ff4fbaaab0831b1447b2f18bba93952c3435`  
		Last Modified: Mon, 27 Dec 2021 18:42:38 GMT  
		Size: 5.2 MB (5185667 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4c82c9810dbf5e873e822ea28782e813bd5277a73013e0e015bf69827be95f1`  
		Last Modified: Mon, 27 Dec 2021 18:42:37 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51b12ef5c112d47a91c90766ac49e1b42fd0a2a3a6c3d6af4b2349c285ea742c`  
		Last Modified: Mon, 27 Dec 2021 18:42:37 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:1.6-alpine`

```console
$ docker pull spiped@sha256:35234b9a4b8b07015b0a9b6712fd3440cc9738a2ac14760483e070c75a602e70
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
$ docker pull spiped@sha256:f4aaae543ff5aba181d531aa5504251d883a40559812a85cff78c7526d3f713e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4523758 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d71e35e9a762b19f1a767061f3cf181454d7090d64dec7acef852f68d4c01262`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 24 Nov 2021 20:19:40 GMT
ADD file:9233f6f2237d79659a9521f7e390df217cec49f1a8aa3a12147bbca1956acdb9 in / 
# Wed, 24 Nov 2021 20:19:40 GMT
CMD ["/bin/sh"]
# Mon, 27 Dec 2021 19:10:10 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Mon, 27 Dec 2021 19:10:11 GMT
RUN apk add --no-cache libssl1.1
# Mon, 27 Dec 2021 19:10:11 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Mon, 27 Dec 2021 19:10:22 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Mon, 27 Dec 2021 19:10:22 GMT
VOLUME [/spiped]
# Mon, 27 Dec 2021 19:10:22 GMT
WORKDIR /spiped
# Mon, 27 Dec 2021 19:10:22 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 27 Dec 2021 19:10:23 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 27 Dec 2021 19:10:23 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:59bf1c3509f33515622619af21ed55bbe26d24913cedbca106468a5fb37a50c3`  
		Last Modified: Wed, 24 Nov 2021 20:20:05 GMT  
		Size: 2.8 MB (2818413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50c602680384586a0fe7febde9f529aea001928a6d26e84d9a3f7be94049ef27`  
		Last Modified: Mon, 27 Dec 2021 19:10:53 GMT  
		Size: 1.3 KB (1265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee913a58b01d029ed458f92226b5b52747e0877c39585d9f93ec5dd2ef0a8cf9`  
		Last Modified: Mon, 27 Dec 2021 19:10:53 GMT  
		Size: 7.7 KB (7749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd8bf950f1ef1b7c96ba1781b5a87d4044135ae197871b261e86d74bc35a8bf5`  
		Last Modified: Mon, 27 Dec 2021 19:10:54 GMT  
		Size: 1.7 MB (1695862 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56d41f282509324afd98cc83dab31aee8ba6459973698c8ccaf3978cddc4ede4`  
		Last Modified: Mon, 27 Dec 2021 19:10:53 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8ba766abbc809d26737c9cc94fbe15a6311c603bfd673bd6db553169dd0f141`  
		Last Modified: Mon, 27 Dec 2021 19:10:53 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; arm variant v6

```console
$ docker pull spiped@sha256:b6482b55d0b7700b0393783f0ea8e49e6a4329c07187fdf826b6902d0ccfa3e6
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.1 MB (4080480 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1df9593d1c7a93c5f606ef97c05cc8d86e1a5bce25cd9895c104e2e1a7edbe19`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 24 Nov 2021 21:08:16 GMT
ADD file:61137e0aa49ba06f57ac69466fe2fb116f580b5e6159d56f846b1d72c4a3c814 in / 
# Wed, 24 Nov 2021 21:08:16 GMT
CMD ["/bin/sh"]
# Mon, 27 Dec 2021 17:49:44 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Mon, 27 Dec 2021 17:49:46 GMT
RUN apk add --no-cache libssl1.1
# Mon, 27 Dec 2021 17:49:47 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Mon, 27 Dec 2021 17:50:06 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Mon, 27 Dec 2021 17:50:07 GMT
VOLUME [/spiped]
# Mon, 27 Dec 2021 17:50:07 GMT
WORKDIR /spiped
# Mon, 27 Dec 2021 17:50:08 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 27 Dec 2021 17:50:08 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 27 Dec 2021 17:50:09 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:e4a43de54da9e309482f6762f0c11f5f547cd8fd61a49c5f158453066162023e`  
		Last Modified: Wed, 24 Nov 2021 21:09:46 GMT  
		Size: 2.6 MB (2631421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c04f27a458746dfc1d07b0b03b9b8f205b08ebef9d6060ef92027b709fee313e`  
		Last Modified: Mon, 27 Dec 2021 17:50:41 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fffa3b0ec9bb32d2efab9fa903af078baf37201f4ec2026c0afce9c14156229`  
		Last Modified: Mon, 27 Dec 2021 17:50:41 GMT  
		Size: 7.7 KB (7743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e2344d51f830abe738f710343c04e056b2ec80e33a48522878caa568c9f553c`  
		Last Modified: Mon, 27 Dec 2021 17:50:42 GMT  
		Size: 1.4 MB (1439576 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd3eeeb2545dce6884a99d866ca20bd742d7e133aacf869b4cddbe974bfde627`  
		Last Modified: Mon, 27 Dec 2021 17:50:41 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2681e39729f29c202bc97138be5a28bb84d92220ffe45df47fb643301eef46aa`  
		Last Modified: Mon, 27 Dec 2021 17:50:41 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; arm variant v7

```console
$ docker pull spiped@sha256:277d22d33ab8cd23ff5bf04d4e60841c8a335de8fdb772173601e9a4d4cb00bf
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.8 MB (3802328 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2f94c64b2c706a58b82aa60bafca69c1fd15fb76714e5ca4aae0f1e4a47e3f1d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 24 Nov 2021 21:42:11 GMT
ADD file:ca436da5b0bfc9c0e2fc685533c6628918000c8fff109fe9a8da625b9a798002 in / 
# Wed, 24 Nov 2021 21:42:11 GMT
CMD ["/bin/sh"]
# Mon, 27 Dec 2021 18:00:04 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Mon, 27 Dec 2021 18:00:06 GMT
RUN apk add --no-cache libssl1.1
# Mon, 27 Dec 2021 18:00:06 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Mon, 27 Dec 2021 18:00:25 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Mon, 27 Dec 2021 18:00:26 GMT
VOLUME [/spiped]
# Mon, 27 Dec 2021 18:00:26 GMT
WORKDIR /spiped
# Mon, 27 Dec 2021 18:00:27 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 27 Dec 2021 18:00:27 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 27 Dec 2021 18:00:28 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:5480d2ca1740c20ce17652e01ed2265cdc914458acd41256a2b1ccff28f2762c`  
		Last Modified: Wed, 24 Nov 2021 21:43:40 GMT  
		Size: 2.4 MB (2434764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fca194041621ab40d8e7f24b7f7e82aa07760b2dafcd26472bd7fae96171989a`  
		Last Modified: Mon, 27 Dec 2021 18:01:41 GMT  
		Size: 1.3 KB (1267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7e934f04cb0ca6a107389bcb614eb02143fb079eef09a47a9248e3c4ff07864`  
		Last Modified: Mon, 27 Dec 2021 18:01:41 GMT  
		Size: 7.7 KB (7749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4111e5d44f2316d799c8b9144d8f35765b0bf330b8d596d99e504969cd48e07a`  
		Last Modified: Mon, 27 Dec 2021 18:01:42 GMT  
		Size: 1.4 MB (1358077 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f46d751b026ad913b2a48630c96460959a733e75728d55aafbd389197bf81857`  
		Last Modified: Mon, 27 Dec 2021 18:01:41 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5140561b01c4c6ae8b47c729fd289d7eef4a2b0e9c427a6bd35a86747e966206`  
		Last Modified: Mon, 27 Dec 2021 18:01:41 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:cbaa0533059fb17c768fe05790c3675b5b5cecf35f0b461e5347d763b1322af8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 MB (2932006 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a49787cc7861893f9d6020342db1639e60d7af6850ca4866d08840d8438a2b0c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 12 Nov 2021 16:39:58 GMT
ADD file:400c0466b29ccad54e0f6c0acef22542992828678c96693ef1f9f4d0551935d8 in / 
# Fri, 12 Nov 2021 16:39:58 GMT
CMD ["/bin/sh"]
# Fri, 12 Nov 2021 18:19:31 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 12 Nov 2021 18:19:33 GMT
RUN apk add --no-cache libssl1.1
# Fri, 12 Nov 2021 18:19:34 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 12 Nov 2021 18:19:54 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 12 Nov 2021 18:19:55 GMT
VOLUME [/spiped]
# Fri, 12 Nov 2021 18:19:56 GMT
WORKDIR /spiped
# Fri, 12 Nov 2021 18:19:58 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 12 Nov 2021 18:19:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 12 Nov 2021 18:19:59 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:be307f383ecc62b27a29b599c3fc9d3129693a798e7fcce614f09174cfe2d354`  
		Last Modified: Fri, 12 Nov 2021 16:40:59 GMT  
		Size: 2.7 MB (2717700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffbcce6bf922e4817964b0a9575d547fbb39004874a87c290658dcbb8939209e`  
		Last Modified: Fri, 12 Nov 2021 18:20:41 GMT  
		Size: 1.2 KB (1239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b342172a90f6f6a837eeb8f0025e02facad5a97fdd12c0aeac68c2411928d16f`  
		Last Modified: Fri, 12 Nov 2021 18:20:41 GMT  
		Size: 7.8 KB (7751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd8a670bc36ab2f74e650d7cb573c4c3542673b9488e2659efbc0d6b9db67529`  
		Last Modified: Fri, 12 Nov 2021 18:20:41 GMT  
		Size: 204.9 KB (204879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:698de19c09a4c9763fb04c4946f3bffafe6556fcfe73a3d55bbb4255f65bd458`  
		Last Modified: Fri, 12 Nov 2021 18:20:41 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1d1aa9a890181cdc95e60ea01849306cb72c967e13716722baa68c7bca76fdb`  
		Last Modified: Fri, 12 Nov 2021 18:20:42 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; 386

```console
$ docker pull spiped@sha256:fc962e82018b393667a7d2b43c9bee0b19c4650fadcc16335cf984b44d859d65
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4539662 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:64dc6529164f107ee83f0edafa6bcf506960ffc646e0e9e161cb2640feb90f96`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 24 Nov 2021 20:53:48 GMT
ADD file:b9a17131c440053f2f67e127b447645f25fd7de2d6caca42f569cafab6291855 in / 
# Wed, 24 Nov 2021 20:53:48 GMT
CMD ["/bin/sh"]
# Mon, 27 Dec 2021 18:39:31 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Mon, 27 Dec 2021 18:39:32 GMT
RUN apk add --no-cache libssl1.1
# Mon, 27 Dec 2021 18:39:33 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Mon, 27 Dec 2021 18:39:45 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Mon, 27 Dec 2021 18:39:45 GMT
VOLUME [/spiped]
# Mon, 27 Dec 2021 18:39:45 GMT
WORKDIR /spiped
# Mon, 27 Dec 2021 18:39:46 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 27 Dec 2021 18:39:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 27 Dec 2021 18:39:46 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:e6889e0d66307a4b916fc844f2dcbc03245c63bc4189dd3e88126d9dcf2f9231`  
		Last Modified: Wed, 24 Nov 2021 20:54:48 GMT  
		Size: 2.8 MB (2827117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc39bdf14cf5dcbf704b50f736d82a339b1879574765ef87fbbf5ecb8d7d574e`  
		Last Modified: Mon, 27 Dec 2021 18:40:32 GMT  
		Size: 1.3 KB (1266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7128f9e1b03ce01ba1b51bce7aa1bc585b6c3e6ce1650259721463f363e9aaab`  
		Last Modified: Mon, 27 Dec 2021 18:40:32 GMT  
		Size: 7.8 KB (7750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb2ebf4c9a2525659cebde6ee501a457c4a31d364f3f568be0f076191d96855d`  
		Last Modified: Mon, 27 Dec 2021 18:40:33 GMT  
		Size: 1.7 MB (1703060 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75adf8fe66ad441b9c8e209efcc7d5b68b61c6a33e05b3aed401756e55493d07`  
		Last Modified: Mon, 27 Dec 2021 18:40:32 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99b656b54398310f3a0f295c7737034732b9ee5c7e294ad5df27230309fff8ae`  
		Last Modified: Mon, 27 Dec 2021 18:40:32 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; ppc64le

```console
$ docker pull spiped@sha256:bdb5c0f748fb29dd4c96f71d1eec1c471f348b68e39063a5674e88c6655400ac
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.4 MB (4447359 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c2ab0ba82f0f9badd5246249195a67d4e12bc4f6cfb1822b3454aca1c3dae586`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 24 Nov 2021 20:20:16 GMT
ADD file:57115dca2eb707f46b6301e75174e6aa316fb02ac28643b91429b75be51bd8c8 in / 
# Wed, 24 Nov 2021 20:20:20 GMT
CMD ["/bin/sh"]
# Mon, 27 Dec 2021 18:18:59 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Mon, 27 Dec 2021 18:19:06 GMT
RUN apk add --no-cache libssl1.1
# Mon, 27 Dec 2021 18:19:08 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Mon, 27 Dec 2021 18:19:22 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Mon, 27 Dec 2021 18:19:25 GMT
VOLUME [/spiped]
# Mon, 27 Dec 2021 18:19:28 GMT
WORKDIR /spiped
# Mon, 27 Dec 2021 18:19:28 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 27 Dec 2021 18:19:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 27 Dec 2021 18:19:33 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:159b5dcb1717c815c76ff5ea1db730e18e8609c9090238e43282856db9e71f47`  
		Last Modified: Wed, 24 Nov 2021 20:21:14 GMT  
		Size: 2.8 MB (2814780 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5ef2b17ec4445a63d712289fc62b0e3e30ab15992e0a0d38ab25e290abcb38e`  
		Last Modified: Mon, 27 Dec 2021 18:20:21 GMT  
		Size: 1.3 KB (1274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:210460e69fcfc508eae94f5666c4fc57c0cdf6163c3a6e39710f5da7a2e5ceb6`  
		Last Modified: Mon, 27 Dec 2021 18:20:21 GMT  
		Size: 7.7 KB (7737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0860c3c69dcd2673558f15fc9c46c8447274ce23c207e936804fe5a268e5e7f`  
		Last Modified: Mon, 27 Dec 2021 18:20:22 GMT  
		Size: 1.6 MB (1623097 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13cd96844150db5d01e32349b5f650aafd01dd1789c2a11fee82b6f55bd43560`  
		Last Modified: Mon, 27 Dec 2021 18:20:21 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a52b1de785dfc0bc3d07ee3d3f619d0681bc34b7eeee205db16da01946663a91`  
		Last Modified: Mon, 27 Dec 2021 18:20:21 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; s390x

```console
$ docker pull spiped@sha256:e5972c57d035e42883aca7354deb92cd65a9bbbc8d5d6aaa8b364891cbdba20d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.0 MB (4034365 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6b297cc2c896c2d11d20abe50ce763f606504b9aad55d18a6c8bcf3407db63c8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 24 Nov 2021 20:41:23 GMT
ADD file:cd24c711a2ef431b3ff94f9a02bfc42f159bc60de1d0eceecafea4e8af02441d in / 
# Wed, 24 Nov 2021 20:41:23 GMT
CMD ["/bin/sh"]
# Mon, 27 Dec 2021 18:42:02 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Mon, 27 Dec 2021 18:42:04 GMT
RUN apk add --no-cache libssl1.1
# Mon, 27 Dec 2021 18:42:04 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Mon, 27 Dec 2021 18:42:09 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Mon, 27 Dec 2021 18:42:09 GMT
VOLUME [/spiped]
# Mon, 27 Dec 2021 18:42:09 GMT
WORKDIR /spiped
# Mon, 27 Dec 2021 18:42:10 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 27 Dec 2021 18:42:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 27 Dec 2021 18:42:10 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:d6baca485f3d0f7c77221be60fbef5db014a5ef9d8f53db4a310c947c690d189`  
		Last Modified: Wed, 24 Nov 2021 20:42:15 GMT  
		Size: 2.6 MB (2605944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:631b52683dec736314bc4a995e6d4aa8fe70ccec0ccb0b4f0349543c0b9d315d`  
		Last Modified: Mon, 27 Dec 2021 18:42:54 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8a99397842c922d6589a78e8df8f8b4feac626485047c36e902a2966e19dfe2`  
		Last Modified: Mon, 27 Dec 2021 18:42:54 GMT  
		Size: 7.7 KB (7743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:556dc6882e78ba3518dbab7eaae8412b06f9ad7e09122f6478d9d1cc80b978e4`  
		Last Modified: Mon, 27 Dec 2021 18:42:55 GMT  
		Size: 1.4 MB (1418939 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9680c33180071ffeb1ac5cfe629daff266a5cf86a4072e251e4b0bef70d20b3`  
		Last Modified: Mon, 27 Dec 2021 18:42:54 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2742416115dba0ead2f2dc1f9aa438a1ef9179b4e11cfd9d665c918f92b53c55`  
		Last Modified: Mon, 27 Dec 2021 18:42:54 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:1.6.2`

```console
$ docker pull spiped@sha256:ac9d0de9a19e6966e0f4b8ff0a78e865413307568ff7df071cc68a2cad09ac15
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 7
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; 386
	-	linux; mips64le
	-	linux; ppc64le
	-	linux; s390x

### `spiped:1.6.2` - linux; amd64

```console
$ docker pull spiped@sha256:27655c03e38daa8aa4afed06a3d4c9f6127f971fe9ed16b98c8f48cc902ef314
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.3 MB (37327359 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:03b1412c46e8325a0589c93bac2d1990523e7e07b13698c2a9cb573fed4960bd`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 21 Dec 2021 01:22:43 GMT
ADD file:09675d11695f65c55efdc393ff0cd32f30194cd7d0fbef4631eebfed4414ac97 in / 
# Tue, 21 Dec 2021 01:22:43 GMT
CMD ["bash"]
# Mon, 27 Dec 2021 19:09:37 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Mon, 27 Dec 2021 19:09:40 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Mon, 27 Dec 2021 19:09:40 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Mon, 27 Dec 2021 19:10:01 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Mon, 27 Dec 2021 19:10:01 GMT
VOLUME [/spiped]
# Mon, 27 Dec 2021 19:10:01 GMT
WORKDIR /spiped
# Mon, 27 Dec 2021 19:10:02 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 27 Dec 2021 19:10:02 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 27 Dec 2021 19:10:02 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:a2abf6c4d29d43a4bf9fbb769f524d0fb36a2edab49819c1bf3e76f409f953ea`  
		Last Modified: Tue, 21 Dec 2021 01:27:48 GMT  
		Size: 31.4 MB (31357624 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d547106b69c042e6267b4030a20ff577bcfc9917ebf0a49d697c1d2819992416`  
		Last Modified: Mon, 27 Dec 2021 19:10:37 GMT  
		Size: 1.7 KB (1733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eda7224a790705cc7b53c6c57deb18f74ceeddf1a6a748cb1c59dd1d4f8b7c03`  
		Last Modified: Mon, 27 Dec 2021 19:10:37 GMT  
		Size: 1.1 KB (1055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7082f5785f33700aa63be5c0b314767d2b6039850a3dfcba2547dc823a464fff`  
		Last Modified: Mon, 27 Dec 2021 19:10:38 GMT  
		Size: 6.0 MB (5966475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8ceb17a2971caaf21db95998adb68b036ca18a5890dede0280840f93e2dabcb`  
		Last Modified: Mon, 27 Dec 2021 19:10:37 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7aed5299a2faa639446a4fc16f9364a4b444cae0a4c9855837063682ec7e4a88`  
		Last Modified: Mon, 27 Dec 2021 19:10:37 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.2` - linux; arm variant v5

```console
$ docker pull spiped@sha256:2bb8d6f9786620cb6d809309fe172b33c989c54afa2e70963dc028539cc711de
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.9 MB (33930835 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cb20a687f8f10c7552075675e860628f3cabd9d85426df4168e2085074497125`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 21 Dec 2021 01:50:31 GMT
ADD file:a3023f71bd93966e7db1419adda3ccde4fcc5e2e8cf58e7b13c51036ed5ff796 in / 
# Tue, 21 Dec 2021 01:50:32 GMT
CMD ["bash"]
# Mon, 27 Dec 2021 17:48:37 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Mon, 27 Dec 2021 17:48:47 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Mon, 27 Dec 2021 17:48:47 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Mon, 27 Dec 2021 17:49:39 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Mon, 27 Dec 2021 17:49:39 GMT
VOLUME [/spiped]
# Mon, 27 Dec 2021 17:49:40 GMT
WORKDIR /spiped
# Mon, 27 Dec 2021 17:49:40 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 27 Dec 2021 17:49:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 27 Dec 2021 17:49:41 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:054429d0cf4038fef39a3b5eb6ce52f600f9a2cbb71a4fb3e95ecf9b2da62581`  
		Last Modified: Tue, 21 Dec 2021 02:05:52 GMT  
		Size: 28.9 MB (28900253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:464a6f781a7abbf2236545af22e3b305148755b938eb4b3f80acfddda83fb330`  
		Last Modified: Mon, 27 Dec 2021 17:50:13 GMT  
		Size: 1.7 KB (1729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:901947b41fdff91f97c93d69ea6510e742f77e91ebe42dfb3151adcdaf03441a`  
		Last Modified: Mon, 27 Dec 2021 17:50:13 GMT  
		Size: 1.1 KB (1056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f468550fb64a624779d011e733e2288492ceeefbf1195d64f8bd54e57f57e4f`  
		Last Modified: Mon, 27 Dec 2021 17:50:18 GMT  
		Size: 5.0 MB (5027325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5aa37e6545912e2b7148568d33bbf517e5deadd118df40ce2ebe5f74710c2d66`  
		Last Modified: Mon, 27 Dec 2021 17:50:13 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18b0df784f0906422ce5e4c8eb5ee379506682e1ad31e783eeca4525c79ba55c`  
		Last Modified: Mon, 27 Dec 2021 17:50:13 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.2` - linux; arm variant v7

```console
$ docker pull spiped@sha256:5ff37adf5b2ffdb562129ff2c4c257c774150b80d954a9a0de388a5cd9c14ab4
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.3 MB (31311461 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:07fa1788ed3cfcc665390b07c5ea81b3818793dc7e8cd3cff01c89fc109cb0be`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 21 Dec 2021 01:59:48 GMT
ADD file:6a5555c3e40db91fae5bb112464a4c405a976de17ff64c98f25d3033a6a608d8 in / 
# Tue, 21 Dec 2021 01:59:48 GMT
CMD ["bash"]
# Mon, 27 Dec 2021 17:58:52 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Mon, 27 Dec 2021 17:58:59 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Mon, 27 Dec 2021 17:58:59 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Mon, 27 Dec 2021 17:59:46 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Mon, 27 Dec 2021 17:59:47 GMT
VOLUME [/spiped]
# Mon, 27 Dec 2021 17:59:47 GMT
WORKDIR /spiped
# Mon, 27 Dec 2021 17:59:48 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 27 Dec 2021 17:59:48 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 27 Dec 2021 17:59:49 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:d0061d6703dc4975804c3419e00c85efbe3f1b79c86d87e048fa14a683e88e31`  
		Last Modified: Tue, 21 Dec 2021 02:15:26 GMT  
		Size: 26.6 MB (26560815 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:379d1aaaf5cba2bb5aa182cc038a59938629d1ad6ec388340be3e8f34e5e65b0`  
		Last Modified: Mon, 27 Dec 2021 18:01:17 GMT  
		Size: 1.7 KB (1730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f6950d1ddd5e954a00fd9b56a607f737d4394ec2519f9c9d47ce2820e12bcfb`  
		Last Modified: Mon, 27 Dec 2021 18:01:17 GMT  
		Size: 1.1 KB (1054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6424dc46a62a8c5530fa74a2aaddc612ea6e099df67cfbe39b49dad4b2416fa4`  
		Last Modified: Mon, 27 Dec 2021 18:01:21 GMT  
		Size: 4.7 MB (4747390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b16a5e406437b655a5c55e8e9027607ad607deb3047cf60539ca94a8a6dd8be`  
		Last Modified: Mon, 27 Dec 2021 18:01:18 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c526844e52b7ac486211e17526f3bd96806de407bdad85bbace1e9268e01d2c`  
		Last Modified: Mon, 27 Dec 2021 18:01:17 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.2` - linux; 386

```console
$ docker pull spiped@sha256:126609a7885028d241e5a5879a81db1e409324ad4299d35fa13d8cb81db7741b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.3 MB (40265566 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e63888bbd27971f057151d0bfa298298857717efa83c94412e8ccc0a77dd65d5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 21 Dec 2021 01:40:06 GMT
ADD file:6b67a0d4d176747cc8cefbd105facde82f1795467bf02eb45e8385c91cdc9c41 in / 
# Tue, 21 Dec 2021 01:40:09 GMT
CMD ["bash"]
# Mon, 27 Dec 2021 18:38:49 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Mon, 27 Dec 2021 18:38:53 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Mon, 27 Dec 2021 18:38:53 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Mon, 27 Dec 2021 18:39:18 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Mon, 27 Dec 2021 18:39:19 GMT
VOLUME [/spiped]
# Mon, 27 Dec 2021 18:39:19 GMT
WORKDIR /spiped
# Mon, 27 Dec 2021 18:39:19 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 27 Dec 2021 18:39:20 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 27 Dec 2021 18:39:20 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:9b9a100d632569e96aeb2d7b0bc45bc436609bb61335815f207994f3b557f0f7`  
		Last Modified: Tue, 21 Dec 2021 01:48:45 GMT  
		Size: 32.4 MB (32370850 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bacb6a90485f91c14c0461997a7afe3993a50f138c22f09ce39f21024c2062b8`  
		Last Modified: Mon, 27 Dec 2021 18:40:12 GMT  
		Size: 1.7 KB (1730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15dd5efb02f26ea602aaebe8f67a9f3a6947dad763a495fef3a9318f12fface9`  
		Last Modified: Mon, 27 Dec 2021 18:40:12 GMT  
		Size: 1.1 KB (1058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82f0e51dee85e4dcfc46978558a24091bc87a2559c3f2a36c3543893184a4c43`  
		Last Modified: Mon, 27 Dec 2021 18:40:14 GMT  
		Size: 7.9 MB (7891457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8925f3c59859f8e255f517eb2391360847148d17eb2715caa30753707600716`  
		Last Modified: Mon, 27 Dec 2021 18:40:12 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce7c6638e6c8f4a87a2847736b51b3093f589a601733574eb08c60e0c4707d43`  
		Last Modified: Mon, 27 Dec 2021 18:40:12 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.2` - linux; mips64le

```console
$ docker pull spiped@sha256:130c01d2a02859608af1ff69b512e606c6b0afab129f4f55f3b214e4439a961e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.3 MB (35327767 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8059d8a507f312d8d77dc186576b8b33cbc65306a9ff8fd918ca17b2b9163198`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 21 Dec 2021 02:09:07 GMT
ADD file:9e5931d5ed32a23b2e93bd8846258c647613637c581b6813bbc7d7e6b86bbdf5 in / 
# Tue, 21 Dec 2021 02:09:08 GMT
CMD ["bash"]
# Mon, 27 Dec 2021 18:07:30 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Mon, 27 Dec 2021 18:07:41 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Mon, 27 Dec 2021 18:07:41 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Mon, 27 Dec 2021 18:08:36 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Mon, 27 Dec 2021 18:08:36 GMT
VOLUME [/spiped]
# Mon, 27 Dec 2021 18:08:37 GMT
WORKDIR /spiped
# Mon, 27 Dec 2021 18:08:37 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 27 Dec 2021 18:08:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 27 Dec 2021 18:08:38 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:6a6edb95e2485a5b9b3c44b27b7ebad16384c0e08a3d61b7e48c65d7278763cf`  
		Last Modified: Tue, 21 Dec 2021 02:18:14 GMT  
		Size: 29.6 MB (29619177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffc41050c10fb28c363303084d216e4a84358c365e0c0c3ea780e76094ac5b62`  
		Last Modified: Mon, 27 Dec 2021 18:08:50 GMT  
		Size: 1.7 KB (1735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ccfed374e34e3e33bb1dac88ddd7d7bd1e7f5274368492e37c693a71768d15b`  
		Last Modified: Mon, 27 Dec 2021 18:08:50 GMT  
		Size: 1.0 KB (1028 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13d7546f5c1590f88787a1fc6a1c2e0d48c67af85dd4b7e8249ff573bee2daad`  
		Last Modified: Mon, 27 Dec 2021 18:08:55 GMT  
		Size: 5.7 MB (5705389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e85af9afd2d869bd928b4990f6fd908f635c5421d1dc8083fc5fd377b8bbd90`  
		Last Modified: Mon, 27 Dec 2021 18:08:50 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:870f16daf77f715fb9dc96eccb5b8d4af6d8b166fa70454d7fab605bd39d022b`  
		Last Modified: Mon, 27 Dec 2021 18:08:50 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.2` - linux; ppc64le

```console
$ docker pull spiped@sha256:60a73d5603e4031736039ecc463577365c1f717538d9abebaffc2f8772464669
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.3 MB (41260220 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:33b349656fc3b5caf98e066d0fdb6c40beca910e76b65314e5f1f5cfea9fc2c5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 21 Dec 2021 02:20:24 GMT
ADD file:078a17bf7e519cb7a60fbbf743ba7e5897554201cb44957154ab518d6991a033 in / 
# Tue, 21 Dec 2021 02:20:28 GMT
CMD ["bash"]
# Mon, 27 Dec 2021 18:16:48 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Mon, 27 Dec 2021 18:16:58 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Mon, 27 Dec 2021 18:17:00 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Mon, 27 Dec 2021 18:18:26 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Mon, 27 Dec 2021 18:18:28 GMT
VOLUME [/spiped]
# Mon, 27 Dec 2021 18:18:31 GMT
WORKDIR /spiped
# Mon, 27 Dec 2021 18:18:32 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 27 Dec 2021 18:18:34 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 27 Dec 2021 18:18:37 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:3345479fea0cdce1382b927b0908af4f239b288b30efa203c50edf7ac0cb055e`  
		Last Modified: Tue, 21 Dec 2021 02:29:20 GMT  
		Size: 35.3 MB (35258992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45821758d9ac9ef7ddf59278b25a098454da513ab2a4469079d31efd2872e496`  
		Last Modified: Mon, 27 Dec 2021 18:20:01 GMT  
		Size: 1.7 KB (1734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6621a4339ab8321307888b642f6c34ede9ba4af6ac0ed96e946ac50ec1227849`  
		Last Modified: Mon, 27 Dec 2021 18:20:01 GMT  
		Size: 1.1 KB (1057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2eb85ea75c9e8b313cfbfc6e4cfef155d0183d2f926c786afe58fc17f96afdae`  
		Last Modified: Mon, 27 Dec 2021 18:20:03 GMT  
		Size: 6.0 MB (5997966 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92b8831f840f6baaf8d56f6cae0b098c6a56d239108b4ae79ca3788881609e16`  
		Last Modified: Mon, 27 Dec 2021 18:20:01 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:918e7af5ea63b6fcb7ce923b4e73eaf873a1247710e432fc8214fd19aad04405`  
		Last Modified: Mon, 27 Dec 2021 18:20:01 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.2` - linux; s390x

```console
$ docker pull spiped@sha256:85d5e0719445d2cdab3cbf858a459655e3240a92ee8d2f2f802f6ac1b211f948
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.8 MB (34830564 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c2df5426aa3ed82a47988087e8347fbcad4453d2a97b19988ddb6026a0947c78`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 21 Dec 2021 01:42:27 GMT
ADD file:c8a482d41bf09dfb6484bf2a6e38535bf0594d26dd6eedd5abde4e3cc811fa6c in / 
# Tue, 21 Dec 2021 01:42:29 GMT
CMD ["bash"]
# Mon, 27 Dec 2021 18:41:39 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Mon, 27 Dec 2021 18:41:42 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Mon, 27 Dec 2021 18:41:42 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Mon, 27 Dec 2021 18:41:54 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Mon, 27 Dec 2021 18:41:55 GMT
VOLUME [/spiped]
# Mon, 27 Dec 2021 18:41:55 GMT
WORKDIR /spiped
# Mon, 27 Dec 2021 18:41:55 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 27 Dec 2021 18:41:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 27 Dec 2021 18:41:55 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:12562551722a758d23ceea9abcdc2bee737e38c8f62a0f3d3afb2cc2626c28b1`  
		Last Modified: Tue, 21 Dec 2021 01:48:15 GMT  
		Size: 29.6 MB (29641636 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e50be5fdb0a5e34432208396d23522b1701f3dff2f0ad3d78fbd79b6b41b6ce`  
		Last Modified: Mon, 27 Dec 2021 18:42:37 GMT  
		Size: 1.7 KB (1739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a42e79bc5e5489f7b5513adce4e87bffd082bb140296c35dd729fa90a5a4868`  
		Last Modified: Mon, 27 Dec 2021 18:42:37 GMT  
		Size: 1.1 KB (1052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e1da3833503470ef9b807b846f2ff4fbaaab0831b1447b2f18bba93952c3435`  
		Last Modified: Mon, 27 Dec 2021 18:42:38 GMT  
		Size: 5.2 MB (5185667 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4c82c9810dbf5e873e822ea28782e813bd5277a73013e0e015bf69827be95f1`  
		Last Modified: Mon, 27 Dec 2021 18:42:37 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51b12ef5c112d47a91c90766ac49e1b42fd0a2a3a6c3d6af4b2349c285ea742c`  
		Last Modified: Mon, 27 Dec 2021 18:42:37 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:1.6.2-alpine`

```console
$ docker pull spiped@sha256:caddf79bab3a4499b3ca12d46539950b4a5a284ee5b2327cd69b1909f59af92c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `spiped:1.6.2-alpine` - linux; amd64

```console
$ docker pull spiped@sha256:f4aaae543ff5aba181d531aa5504251d883a40559812a85cff78c7526d3f713e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4523758 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d71e35e9a762b19f1a767061f3cf181454d7090d64dec7acef852f68d4c01262`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 24 Nov 2021 20:19:40 GMT
ADD file:9233f6f2237d79659a9521f7e390df217cec49f1a8aa3a12147bbca1956acdb9 in / 
# Wed, 24 Nov 2021 20:19:40 GMT
CMD ["/bin/sh"]
# Mon, 27 Dec 2021 19:10:10 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Mon, 27 Dec 2021 19:10:11 GMT
RUN apk add --no-cache libssl1.1
# Mon, 27 Dec 2021 19:10:11 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Mon, 27 Dec 2021 19:10:22 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Mon, 27 Dec 2021 19:10:22 GMT
VOLUME [/spiped]
# Mon, 27 Dec 2021 19:10:22 GMT
WORKDIR /spiped
# Mon, 27 Dec 2021 19:10:22 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 27 Dec 2021 19:10:23 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 27 Dec 2021 19:10:23 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:59bf1c3509f33515622619af21ed55bbe26d24913cedbca106468a5fb37a50c3`  
		Last Modified: Wed, 24 Nov 2021 20:20:05 GMT  
		Size: 2.8 MB (2818413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50c602680384586a0fe7febde9f529aea001928a6d26e84d9a3f7be94049ef27`  
		Last Modified: Mon, 27 Dec 2021 19:10:53 GMT  
		Size: 1.3 KB (1265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee913a58b01d029ed458f92226b5b52747e0877c39585d9f93ec5dd2ef0a8cf9`  
		Last Modified: Mon, 27 Dec 2021 19:10:53 GMT  
		Size: 7.7 KB (7749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd8bf950f1ef1b7c96ba1781b5a87d4044135ae197871b261e86d74bc35a8bf5`  
		Last Modified: Mon, 27 Dec 2021 19:10:54 GMT  
		Size: 1.7 MB (1695862 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56d41f282509324afd98cc83dab31aee8ba6459973698c8ccaf3978cddc4ede4`  
		Last Modified: Mon, 27 Dec 2021 19:10:53 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8ba766abbc809d26737c9cc94fbe15a6311c603bfd673bd6db553169dd0f141`  
		Last Modified: Mon, 27 Dec 2021 19:10:53 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.2-alpine` - linux; arm variant v6

```console
$ docker pull spiped@sha256:b6482b55d0b7700b0393783f0ea8e49e6a4329c07187fdf826b6902d0ccfa3e6
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.1 MB (4080480 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1df9593d1c7a93c5f606ef97c05cc8d86e1a5bce25cd9895c104e2e1a7edbe19`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 24 Nov 2021 21:08:16 GMT
ADD file:61137e0aa49ba06f57ac69466fe2fb116f580b5e6159d56f846b1d72c4a3c814 in / 
# Wed, 24 Nov 2021 21:08:16 GMT
CMD ["/bin/sh"]
# Mon, 27 Dec 2021 17:49:44 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Mon, 27 Dec 2021 17:49:46 GMT
RUN apk add --no-cache libssl1.1
# Mon, 27 Dec 2021 17:49:47 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Mon, 27 Dec 2021 17:50:06 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Mon, 27 Dec 2021 17:50:07 GMT
VOLUME [/spiped]
# Mon, 27 Dec 2021 17:50:07 GMT
WORKDIR /spiped
# Mon, 27 Dec 2021 17:50:08 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 27 Dec 2021 17:50:08 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 27 Dec 2021 17:50:09 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:e4a43de54da9e309482f6762f0c11f5f547cd8fd61a49c5f158453066162023e`  
		Last Modified: Wed, 24 Nov 2021 21:09:46 GMT  
		Size: 2.6 MB (2631421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c04f27a458746dfc1d07b0b03b9b8f205b08ebef9d6060ef92027b709fee313e`  
		Last Modified: Mon, 27 Dec 2021 17:50:41 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fffa3b0ec9bb32d2efab9fa903af078baf37201f4ec2026c0afce9c14156229`  
		Last Modified: Mon, 27 Dec 2021 17:50:41 GMT  
		Size: 7.7 KB (7743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e2344d51f830abe738f710343c04e056b2ec80e33a48522878caa568c9f553c`  
		Last Modified: Mon, 27 Dec 2021 17:50:42 GMT  
		Size: 1.4 MB (1439576 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd3eeeb2545dce6884a99d866ca20bd742d7e133aacf869b4cddbe974bfde627`  
		Last Modified: Mon, 27 Dec 2021 17:50:41 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2681e39729f29c202bc97138be5a28bb84d92220ffe45df47fb643301eef46aa`  
		Last Modified: Mon, 27 Dec 2021 17:50:41 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.2-alpine` - linux; arm variant v7

```console
$ docker pull spiped@sha256:277d22d33ab8cd23ff5bf04d4e60841c8a335de8fdb772173601e9a4d4cb00bf
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.8 MB (3802328 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2f94c64b2c706a58b82aa60bafca69c1fd15fb76714e5ca4aae0f1e4a47e3f1d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 24 Nov 2021 21:42:11 GMT
ADD file:ca436da5b0bfc9c0e2fc685533c6628918000c8fff109fe9a8da625b9a798002 in / 
# Wed, 24 Nov 2021 21:42:11 GMT
CMD ["/bin/sh"]
# Mon, 27 Dec 2021 18:00:04 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Mon, 27 Dec 2021 18:00:06 GMT
RUN apk add --no-cache libssl1.1
# Mon, 27 Dec 2021 18:00:06 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Mon, 27 Dec 2021 18:00:25 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Mon, 27 Dec 2021 18:00:26 GMT
VOLUME [/spiped]
# Mon, 27 Dec 2021 18:00:26 GMT
WORKDIR /spiped
# Mon, 27 Dec 2021 18:00:27 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 27 Dec 2021 18:00:27 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 27 Dec 2021 18:00:28 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:5480d2ca1740c20ce17652e01ed2265cdc914458acd41256a2b1ccff28f2762c`  
		Last Modified: Wed, 24 Nov 2021 21:43:40 GMT  
		Size: 2.4 MB (2434764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fca194041621ab40d8e7f24b7f7e82aa07760b2dafcd26472bd7fae96171989a`  
		Last Modified: Mon, 27 Dec 2021 18:01:41 GMT  
		Size: 1.3 KB (1267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7e934f04cb0ca6a107389bcb614eb02143fb079eef09a47a9248e3c4ff07864`  
		Last Modified: Mon, 27 Dec 2021 18:01:41 GMT  
		Size: 7.7 KB (7749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4111e5d44f2316d799c8b9144d8f35765b0bf330b8d596d99e504969cd48e07a`  
		Last Modified: Mon, 27 Dec 2021 18:01:42 GMT  
		Size: 1.4 MB (1358077 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f46d751b026ad913b2a48630c96460959a733e75728d55aafbd389197bf81857`  
		Last Modified: Mon, 27 Dec 2021 18:01:41 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5140561b01c4c6ae8b47c729fd289d7eef4a2b0e9c427a6bd35a86747e966206`  
		Last Modified: Mon, 27 Dec 2021 18:01:41 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.2-alpine` - linux; 386

```console
$ docker pull spiped@sha256:fc962e82018b393667a7d2b43c9bee0b19c4650fadcc16335cf984b44d859d65
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4539662 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:64dc6529164f107ee83f0edafa6bcf506960ffc646e0e9e161cb2640feb90f96`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 24 Nov 2021 20:53:48 GMT
ADD file:b9a17131c440053f2f67e127b447645f25fd7de2d6caca42f569cafab6291855 in / 
# Wed, 24 Nov 2021 20:53:48 GMT
CMD ["/bin/sh"]
# Mon, 27 Dec 2021 18:39:31 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Mon, 27 Dec 2021 18:39:32 GMT
RUN apk add --no-cache libssl1.1
# Mon, 27 Dec 2021 18:39:33 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Mon, 27 Dec 2021 18:39:45 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Mon, 27 Dec 2021 18:39:45 GMT
VOLUME [/spiped]
# Mon, 27 Dec 2021 18:39:45 GMT
WORKDIR /spiped
# Mon, 27 Dec 2021 18:39:46 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 27 Dec 2021 18:39:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 27 Dec 2021 18:39:46 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:e6889e0d66307a4b916fc844f2dcbc03245c63bc4189dd3e88126d9dcf2f9231`  
		Last Modified: Wed, 24 Nov 2021 20:54:48 GMT  
		Size: 2.8 MB (2827117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc39bdf14cf5dcbf704b50f736d82a339b1879574765ef87fbbf5ecb8d7d574e`  
		Last Modified: Mon, 27 Dec 2021 18:40:32 GMT  
		Size: 1.3 KB (1266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7128f9e1b03ce01ba1b51bce7aa1bc585b6c3e6ce1650259721463f363e9aaab`  
		Last Modified: Mon, 27 Dec 2021 18:40:32 GMT  
		Size: 7.8 KB (7750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb2ebf4c9a2525659cebde6ee501a457c4a31d364f3f568be0f076191d96855d`  
		Last Modified: Mon, 27 Dec 2021 18:40:33 GMT  
		Size: 1.7 MB (1703060 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75adf8fe66ad441b9c8e209efcc7d5b68b61c6a33e05b3aed401756e55493d07`  
		Last Modified: Mon, 27 Dec 2021 18:40:32 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99b656b54398310f3a0f295c7737034732b9ee5c7e294ad5df27230309fff8ae`  
		Last Modified: Mon, 27 Dec 2021 18:40:32 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.2-alpine` - linux; ppc64le

```console
$ docker pull spiped@sha256:bdb5c0f748fb29dd4c96f71d1eec1c471f348b68e39063a5674e88c6655400ac
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.4 MB (4447359 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c2ab0ba82f0f9badd5246249195a67d4e12bc4f6cfb1822b3454aca1c3dae586`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 24 Nov 2021 20:20:16 GMT
ADD file:57115dca2eb707f46b6301e75174e6aa316fb02ac28643b91429b75be51bd8c8 in / 
# Wed, 24 Nov 2021 20:20:20 GMT
CMD ["/bin/sh"]
# Mon, 27 Dec 2021 18:18:59 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Mon, 27 Dec 2021 18:19:06 GMT
RUN apk add --no-cache libssl1.1
# Mon, 27 Dec 2021 18:19:08 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Mon, 27 Dec 2021 18:19:22 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Mon, 27 Dec 2021 18:19:25 GMT
VOLUME [/spiped]
# Mon, 27 Dec 2021 18:19:28 GMT
WORKDIR /spiped
# Mon, 27 Dec 2021 18:19:28 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 27 Dec 2021 18:19:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 27 Dec 2021 18:19:33 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:159b5dcb1717c815c76ff5ea1db730e18e8609c9090238e43282856db9e71f47`  
		Last Modified: Wed, 24 Nov 2021 20:21:14 GMT  
		Size: 2.8 MB (2814780 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5ef2b17ec4445a63d712289fc62b0e3e30ab15992e0a0d38ab25e290abcb38e`  
		Last Modified: Mon, 27 Dec 2021 18:20:21 GMT  
		Size: 1.3 KB (1274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:210460e69fcfc508eae94f5666c4fc57c0cdf6163c3a6e39710f5da7a2e5ceb6`  
		Last Modified: Mon, 27 Dec 2021 18:20:21 GMT  
		Size: 7.7 KB (7737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0860c3c69dcd2673558f15fc9c46c8447274ce23c207e936804fe5a268e5e7f`  
		Last Modified: Mon, 27 Dec 2021 18:20:22 GMT  
		Size: 1.6 MB (1623097 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13cd96844150db5d01e32349b5f650aafd01dd1789c2a11fee82b6f55bd43560`  
		Last Modified: Mon, 27 Dec 2021 18:20:21 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a52b1de785dfc0bc3d07ee3d3f619d0681bc34b7eeee205db16da01946663a91`  
		Last Modified: Mon, 27 Dec 2021 18:20:21 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.2-alpine` - linux; s390x

```console
$ docker pull spiped@sha256:e5972c57d035e42883aca7354deb92cd65a9bbbc8d5d6aaa8b364891cbdba20d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.0 MB (4034365 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6b297cc2c896c2d11d20abe50ce763f606504b9aad55d18a6c8bcf3407db63c8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 24 Nov 2021 20:41:23 GMT
ADD file:cd24c711a2ef431b3ff94f9a02bfc42f159bc60de1d0eceecafea4e8af02441d in / 
# Wed, 24 Nov 2021 20:41:23 GMT
CMD ["/bin/sh"]
# Mon, 27 Dec 2021 18:42:02 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Mon, 27 Dec 2021 18:42:04 GMT
RUN apk add --no-cache libssl1.1
# Mon, 27 Dec 2021 18:42:04 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Mon, 27 Dec 2021 18:42:09 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Mon, 27 Dec 2021 18:42:09 GMT
VOLUME [/spiped]
# Mon, 27 Dec 2021 18:42:09 GMT
WORKDIR /spiped
# Mon, 27 Dec 2021 18:42:10 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 27 Dec 2021 18:42:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 27 Dec 2021 18:42:10 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:d6baca485f3d0f7c77221be60fbef5db014a5ef9d8f53db4a310c947c690d189`  
		Last Modified: Wed, 24 Nov 2021 20:42:15 GMT  
		Size: 2.6 MB (2605944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:631b52683dec736314bc4a995e6d4aa8fe70ccec0ccb0b4f0349543c0b9d315d`  
		Last Modified: Mon, 27 Dec 2021 18:42:54 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8a99397842c922d6589a78e8df8f8b4feac626485047c36e902a2966e19dfe2`  
		Last Modified: Mon, 27 Dec 2021 18:42:54 GMT  
		Size: 7.7 KB (7743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:556dc6882e78ba3518dbab7eaae8412b06f9ad7e09122f6478d9d1cc80b978e4`  
		Last Modified: Mon, 27 Dec 2021 18:42:55 GMT  
		Size: 1.4 MB (1418939 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9680c33180071ffeb1ac5cfe629daff266a5cf86a4072e251e4b0bef70d20b3`  
		Last Modified: Mon, 27 Dec 2021 18:42:54 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2742416115dba0ead2f2dc1f9aa438a1ef9179b4e11cfd9d665c918f92b53c55`  
		Last Modified: Mon, 27 Dec 2021 18:42:54 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:alpine`

```console
$ docker pull spiped@sha256:35234b9a4b8b07015b0a9b6712fd3440cc9738a2ac14760483e070c75a602e70
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
$ docker pull spiped@sha256:f4aaae543ff5aba181d531aa5504251d883a40559812a85cff78c7526d3f713e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4523758 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d71e35e9a762b19f1a767061f3cf181454d7090d64dec7acef852f68d4c01262`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 24 Nov 2021 20:19:40 GMT
ADD file:9233f6f2237d79659a9521f7e390df217cec49f1a8aa3a12147bbca1956acdb9 in / 
# Wed, 24 Nov 2021 20:19:40 GMT
CMD ["/bin/sh"]
# Mon, 27 Dec 2021 19:10:10 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Mon, 27 Dec 2021 19:10:11 GMT
RUN apk add --no-cache libssl1.1
# Mon, 27 Dec 2021 19:10:11 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Mon, 27 Dec 2021 19:10:22 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Mon, 27 Dec 2021 19:10:22 GMT
VOLUME [/spiped]
# Mon, 27 Dec 2021 19:10:22 GMT
WORKDIR /spiped
# Mon, 27 Dec 2021 19:10:22 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 27 Dec 2021 19:10:23 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 27 Dec 2021 19:10:23 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:59bf1c3509f33515622619af21ed55bbe26d24913cedbca106468a5fb37a50c3`  
		Last Modified: Wed, 24 Nov 2021 20:20:05 GMT  
		Size: 2.8 MB (2818413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50c602680384586a0fe7febde9f529aea001928a6d26e84d9a3f7be94049ef27`  
		Last Modified: Mon, 27 Dec 2021 19:10:53 GMT  
		Size: 1.3 KB (1265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee913a58b01d029ed458f92226b5b52747e0877c39585d9f93ec5dd2ef0a8cf9`  
		Last Modified: Mon, 27 Dec 2021 19:10:53 GMT  
		Size: 7.7 KB (7749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd8bf950f1ef1b7c96ba1781b5a87d4044135ae197871b261e86d74bc35a8bf5`  
		Last Modified: Mon, 27 Dec 2021 19:10:54 GMT  
		Size: 1.7 MB (1695862 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56d41f282509324afd98cc83dab31aee8ba6459973698c8ccaf3978cddc4ede4`  
		Last Modified: Mon, 27 Dec 2021 19:10:53 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8ba766abbc809d26737c9cc94fbe15a6311c603bfd673bd6db553169dd0f141`  
		Last Modified: Mon, 27 Dec 2021 19:10:53 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; arm variant v6

```console
$ docker pull spiped@sha256:b6482b55d0b7700b0393783f0ea8e49e6a4329c07187fdf826b6902d0ccfa3e6
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.1 MB (4080480 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1df9593d1c7a93c5f606ef97c05cc8d86e1a5bce25cd9895c104e2e1a7edbe19`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 24 Nov 2021 21:08:16 GMT
ADD file:61137e0aa49ba06f57ac69466fe2fb116f580b5e6159d56f846b1d72c4a3c814 in / 
# Wed, 24 Nov 2021 21:08:16 GMT
CMD ["/bin/sh"]
# Mon, 27 Dec 2021 17:49:44 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Mon, 27 Dec 2021 17:49:46 GMT
RUN apk add --no-cache libssl1.1
# Mon, 27 Dec 2021 17:49:47 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Mon, 27 Dec 2021 17:50:06 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Mon, 27 Dec 2021 17:50:07 GMT
VOLUME [/spiped]
# Mon, 27 Dec 2021 17:50:07 GMT
WORKDIR /spiped
# Mon, 27 Dec 2021 17:50:08 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 27 Dec 2021 17:50:08 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 27 Dec 2021 17:50:09 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:e4a43de54da9e309482f6762f0c11f5f547cd8fd61a49c5f158453066162023e`  
		Last Modified: Wed, 24 Nov 2021 21:09:46 GMT  
		Size: 2.6 MB (2631421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c04f27a458746dfc1d07b0b03b9b8f205b08ebef9d6060ef92027b709fee313e`  
		Last Modified: Mon, 27 Dec 2021 17:50:41 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fffa3b0ec9bb32d2efab9fa903af078baf37201f4ec2026c0afce9c14156229`  
		Last Modified: Mon, 27 Dec 2021 17:50:41 GMT  
		Size: 7.7 KB (7743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e2344d51f830abe738f710343c04e056b2ec80e33a48522878caa568c9f553c`  
		Last Modified: Mon, 27 Dec 2021 17:50:42 GMT  
		Size: 1.4 MB (1439576 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd3eeeb2545dce6884a99d866ca20bd742d7e133aacf869b4cddbe974bfde627`  
		Last Modified: Mon, 27 Dec 2021 17:50:41 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2681e39729f29c202bc97138be5a28bb84d92220ffe45df47fb643301eef46aa`  
		Last Modified: Mon, 27 Dec 2021 17:50:41 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; arm variant v7

```console
$ docker pull spiped@sha256:277d22d33ab8cd23ff5bf04d4e60841c8a335de8fdb772173601e9a4d4cb00bf
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.8 MB (3802328 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2f94c64b2c706a58b82aa60bafca69c1fd15fb76714e5ca4aae0f1e4a47e3f1d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 24 Nov 2021 21:42:11 GMT
ADD file:ca436da5b0bfc9c0e2fc685533c6628918000c8fff109fe9a8da625b9a798002 in / 
# Wed, 24 Nov 2021 21:42:11 GMT
CMD ["/bin/sh"]
# Mon, 27 Dec 2021 18:00:04 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Mon, 27 Dec 2021 18:00:06 GMT
RUN apk add --no-cache libssl1.1
# Mon, 27 Dec 2021 18:00:06 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Mon, 27 Dec 2021 18:00:25 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Mon, 27 Dec 2021 18:00:26 GMT
VOLUME [/spiped]
# Mon, 27 Dec 2021 18:00:26 GMT
WORKDIR /spiped
# Mon, 27 Dec 2021 18:00:27 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 27 Dec 2021 18:00:27 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 27 Dec 2021 18:00:28 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:5480d2ca1740c20ce17652e01ed2265cdc914458acd41256a2b1ccff28f2762c`  
		Last Modified: Wed, 24 Nov 2021 21:43:40 GMT  
		Size: 2.4 MB (2434764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fca194041621ab40d8e7f24b7f7e82aa07760b2dafcd26472bd7fae96171989a`  
		Last Modified: Mon, 27 Dec 2021 18:01:41 GMT  
		Size: 1.3 KB (1267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7e934f04cb0ca6a107389bcb614eb02143fb079eef09a47a9248e3c4ff07864`  
		Last Modified: Mon, 27 Dec 2021 18:01:41 GMT  
		Size: 7.7 KB (7749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4111e5d44f2316d799c8b9144d8f35765b0bf330b8d596d99e504969cd48e07a`  
		Last Modified: Mon, 27 Dec 2021 18:01:42 GMT  
		Size: 1.4 MB (1358077 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f46d751b026ad913b2a48630c96460959a733e75728d55aafbd389197bf81857`  
		Last Modified: Mon, 27 Dec 2021 18:01:41 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5140561b01c4c6ae8b47c729fd289d7eef4a2b0e9c427a6bd35a86747e966206`  
		Last Modified: Mon, 27 Dec 2021 18:01:41 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:cbaa0533059fb17c768fe05790c3675b5b5cecf35f0b461e5347d763b1322af8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 MB (2932006 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a49787cc7861893f9d6020342db1639e60d7af6850ca4866d08840d8438a2b0c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 12 Nov 2021 16:39:58 GMT
ADD file:400c0466b29ccad54e0f6c0acef22542992828678c96693ef1f9f4d0551935d8 in / 
# Fri, 12 Nov 2021 16:39:58 GMT
CMD ["/bin/sh"]
# Fri, 12 Nov 2021 18:19:31 GMT
RUN addgroup -S spiped &&	adduser -S -G spiped spiped
# Fri, 12 Nov 2021 18:19:33 GMT
RUN apk add --no-cache libssl1.1
# Fri, 12 Nov 2021 18:19:34 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Fri, 12 Nov 2021 18:19:54 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del .build-deps
# Fri, 12 Nov 2021 18:19:55 GMT
VOLUME [/spiped]
# Fri, 12 Nov 2021 18:19:56 GMT
WORKDIR /spiped
# Fri, 12 Nov 2021 18:19:58 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 12 Nov 2021 18:19:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 12 Nov 2021 18:19:59 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:be307f383ecc62b27a29b599c3fc9d3129693a798e7fcce614f09174cfe2d354`  
		Last Modified: Fri, 12 Nov 2021 16:40:59 GMT  
		Size: 2.7 MB (2717700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffbcce6bf922e4817964b0a9575d547fbb39004874a87c290658dcbb8939209e`  
		Last Modified: Fri, 12 Nov 2021 18:20:41 GMT  
		Size: 1.2 KB (1239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b342172a90f6f6a837eeb8f0025e02facad5a97fdd12c0aeac68c2411928d16f`  
		Last Modified: Fri, 12 Nov 2021 18:20:41 GMT  
		Size: 7.8 KB (7751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd8a670bc36ab2f74e650d7cb573c4c3542673b9488e2659efbc0d6b9db67529`  
		Last Modified: Fri, 12 Nov 2021 18:20:41 GMT  
		Size: 204.9 KB (204879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:698de19c09a4c9763fb04c4946f3bffafe6556fcfe73a3d55bbb4255f65bd458`  
		Last Modified: Fri, 12 Nov 2021 18:20:41 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1d1aa9a890181cdc95e60ea01849306cb72c967e13716722baa68c7bca76fdb`  
		Last Modified: Fri, 12 Nov 2021 18:20:42 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; 386

```console
$ docker pull spiped@sha256:fc962e82018b393667a7d2b43c9bee0b19c4650fadcc16335cf984b44d859d65
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4539662 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:64dc6529164f107ee83f0edafa6bcf506960ffc646e0e9e161cb2640feb90f96`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 24 Nov 2021 20:53:48 GMT
ADD file:b9a17131c440053f2f67e127b447645f25fd7de2d6caca42f569cafab6291855 in / 
# Wed, 24 Nov 2021 20:53:48 GMT
CMD ["/bin/sh"]
# Mon, 27 Dec 2021 18:39:31 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Mon, 27 Dec 2021 18:39:32 GMT
RUN apk add --no-cache libssl1.1
# Mon, 27 Dec 2021 18:39:33 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Mon, 27 Dec 2021 18:39:45 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Mon, 27 Dec 2021 18:39:45 GMT
VOLUME [/spiped]
# Mon, 27 Dec 2021 18:39:45 GMT
WORKDIR /spiped
# Mon, 27 Dec 2021 18:39:46 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 27 Dec 2021 18:39:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 27 Dec 2021 18:39:46 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:e6889e0d66307a4b916fc844f2dcbc03245c63bc4189dd3e88126d9dcf2f9231`  
		Last Modified: Wed, 24 Nov 2021 20:54:48 GMT  
		Size: 2.8 MB (2827117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc39bdf14cf5dcbf704b50f736d82a339b1879574765ef87fbbf5ecb8d7d574e`  
		Last Modified: Mon, 27 Dec 2021 18:40:32 GMT  
		Size: 1.3 KB (1266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7128f9e1b03ce01ba1b51bce7aa1bc585b6c3e6ce1650259721463f363e9aaab`  
		Last Modified: Mon, 27 Dec 2021 18:40:32 GMT  
		Size: 7.8 KB (7750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb2ebf4c9a2525659cebde6ee501a457c4a31d364f3f568be0f076191d96855d`  
		Last Modified: Mon, 27 Dec 2021 18:40:33 GMT  
		Size: 1.7 MB (1703060 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75adf8fe66ad441b9c8e209efcc7d5b68b61c6a33e05b3aed401756e55493d07`  
		Last Modified: Mon, 27 Dec 2021 18:40:32 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99b656b54398310f3a0f295c7737034732b9ee5c7e294ad5df27230309fff8ae`  
		Last Modified: Mon, 27 Dec 2021 18:40:32 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; ppc64le

```console
$ docker pull spiped@sha256:bdb5c0f748fb29dd4c96f71d1eec1c471f348b68e39063a5674e88c6655400ac
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.4 MB (4447359 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c2ab0ba82f0f9badd5246249195a67d4e12bc4f6cfb1822b3454aca1c3dae586`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 24 Nov 2021 20:20:16 GMT
ADD file:57115dca2eb707f46b6301e75174e6aa316fb02ac28643b91429b75be51bd8c8 in / 
# Wed, 24 Nov 2021 20:20:20 GMT
CMD ["/bin/sh"]
# Mon, 27 Dec 2021 18:18:59 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Mon, 27 Dec 2021 18:19:06 GMT
RUN apk add --no-cache libssl1.1
# Mon, 27 Dec 2021 18:19:08 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Mon, 27 Dec 2021 18:19:22 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Mon, 27 Dec 2021 18:19:25 GMT
VOLUME [/spiped]
# Mon, 27 Dec 2021 18:19:28 GMT
WORKDIR /spiped
# Mon, 27 Dec 2021 18:19:28 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 27 Dec 2021 18:19:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 27 Dec 2021 18:19:33 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:159b5dcb1717c815c76ff5ea1db730e18e8609c9090238e43282856db9e71f47`  
		Last Modified: Wed, 24 Nov 2021 20:21:14 GMT  
		Size: 2.8 MB (2814780 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5ef2b17ec4445a63d712289fc62b0e3e30ab15992e0a0d38ab25e290abcb38e`  
		Last Modified: Mon, 27 Dec 2021 18:20:21 GMT  
		Size: 1.3 KB (1274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:210460e69fcfc508eae94f5666c4fc57c0cdf6163c3a6e39710f5da7a2e5ceb6`  
		Last Modified: Mon, 27 Dec 2021 18:20:21 GMT  
		Size: 7.7 KB (7737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0860c3c69dcd2673558f15fc9c46c8447274ce23c207e936804fe5a268e5e7f`  
		Last Modified: Mon, 27 Dec 2021 18:20:22 GMT  
		Size: 1.6 MB (1623097 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13cd96844150db5d01e32349b5f650aafd01dd1789c2a11fee82b6f55bd43560`  
		Last Modified: Mon, 27 Dec 2021 18:20:21 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a52b1de785dfc0bc3d07ee3d3f619d0681bc34b7eeee205db16da01946663a91`  
		Last Modified: Mon, 27 Dec 2021 18:20:21 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; s390x

```console
$ docker pull spiped@sha256:e5972c57d035e42883aca7354deb92cd65a9bbbc8d5d6aaa8b364891cbdba20d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.0 MB (4034365 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6b297cc2c896c2d11d20abe50ce763f606504b9aad55d18a6c8bcf3407db63c8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 24 Nov 2021 20:41:23 GMT
ADD file:cd24c711a2ef431b3ff94f9a02bfc42f159bc60de1d0eceecafea4e8af02441d in / 
# Wed, 24 Nov 2021 20:41:23 GMT
CMD ["/bin/sh"]
# Mon, 27 Dec 2021 18:42:02 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Mon, 27 Dec 2021 18:42:04 GMT
RUN apk add --no-cache libssl1.1
# Mon, 27 Dec 2021 18:42:04 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Mon, 27 Dec 2021 18:42:09 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Mon, 27 Dec 2021 18:42:09 GMT
VOLUME [/spiped]
# Mon, 27 Dec 2021 18:42:09 GMT
WORKDIR /spiped
# Mon, 27 Dec 2021 18:42:10 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 27 Dec 2021 18:42:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 27 Dec 2021 18:42:10 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:d6baca485f3d0f7c77221be60fbef5db014a5ef9d8f53db4a310c947c690d189`  
		Last Modified: Wed, 24 Nov 2021 20:42:15 GMT  
		Size: 2.6 MB (2605944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:631b52683dec736314bc4a995e6d4aa8fe70ccec0ccb0b4f0349543c0b9d315d`  
		Last Modified: Mon, 27 Dec 2021 18:42:54 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8a99397842c922d6589a78e8df8f8b4feac626485047c36e902a2966e19dfe2`  
		Last Modified: Mon, 27 Dec 2021 18:42:54 GMT  
		Size: 7.7 KB (7743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:556dc6882e78ba3518dbab7eaae8412b06f9ad7e09122f6478d9d1cc80b978e4`  
		Last Modified: Mon, 27 Dec 2021 18:42:55 GMT  
		Size: 1.4 MB (1418939 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9680c33180071ffeb1ac5cfe629daff266a5cf86a4072e251e4b0bef70d20b3`  
		Last Modified: Mon, 27 Dec 2021 18:42:54 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2742416115dba0ead2f2dc1f9aa438a1ef9179b4e11cfd9d665c918f92b53c55`  
		Last Modified: Mon, 27 Dec 2021 18:42:54 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:latest`

```console
$ docker pull spiped@sha256:fcecfb6a9c0c1da84943ba03f5f53edcf5508eadd518ba6f671ed2d1a34f3241
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
$ docker pull spiped@sha256:27655c03e38daa8aa4afed06a3d4c9f6127f971fe9ed16b98c8f48cc902ef314
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.3 MB (37327359 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:03b1412c46e8325a0589c93bac2d1990523e7e07b13698c2a9cb573fed4960bd`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 21 Dec 2021 01:22:43 GMT
ADD file:09675d11695f65c55efdc393ff0cd32f30194cd7d0fbef4631eebfed4414ac97 in / 
# Tue, 21 Dec 2021 01:22:43 GMT
CMD ["bash"]
# Mon, 27 Dec 2021 19:09:37 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Mon, 27 Dec 2021 19:09:40 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Mon, 27 Dec 2021 19:09:40 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Mon, 27 Dec 2021 19:10:01 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Mon, 27 Dec 2021 19:10:01 GMT
VOLUME [/spiped]
# Mon, 27 Dec 2021 19:10:01 GMT
WORKDIR /spiped
# Mon, 27 Dec 2021 19:10:02 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 27 Dec 2021 19:10:02 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 27 Dec 2021 19:10:02 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:a2abf6c4d29d43a4bf9fbb769f524d0fb36a2edab49819c1bf3e76f409f953ea`  
		Last Modified: Tue, 21 Dec 2021 01:27:48 GMT  
		Size: 31.4 MB (31357624 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d547106b69c042e6267b4030a20ff577bcfc9917ebf0a49d697c1d2819992416`  
		Last Modified: Mon, 27 Dec 2021 19:10:37 GMT  
		Size: 1.7 KB (1733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eda7224a790705cc7b53c6c57deb18f74ceeddf1a6a748cb1c59dd1d4f8b7c03`  
		Last Modified: Mon, 27 Dec 2021 19:10:37 GMT  
		Size: 1.1 KB (1055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7082f5785f33700aa63be5c0b314767d2b6039850a3dfcba2547dc823a464fff`  
		Last Modified: Mon, 27 Dec 2021 19:10:38 GMT  
		Size: 6.0 MB (5966475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8ceb17a2971caaf21db95998adb68b036ca18a5890dede0280840f93e2dabcb`  
		Last Modified: Mon, 27 Dec 2021 19:10:37 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7aed5299a2faa639446a4fc16f9364a4b444cae0a4c9855837063682ec7e4a88`  
		Last Modified: Mon, 27 Dec 2021 19:10:37 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; arm variant v5

```console
$ docker pull spiped@sha256:2bb8d6f9786620cb6d809309fe172b33c989c54afa2e70963dc028539cc711de
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.9 MB (33930835 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cb20a687f8f10c7552075675e860628f3cabd9d85426df4168e2085074497125`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 21 Dec 2021 01:50:31 GMT
ADD file:a3023f71bd93966e7db1419adda3ccde4fcc5e2e8cf58e7b13c51036ed5ff796 in / 
# Tue, 21 Dec 2021 01:50:32 GMT
CMD ["bash"]
# Mon, 27 Dec 2021 17:48:37 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Mon, 27 Dec 2021 17:48:47 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Mon, 27 Dec 2021 17:48:47 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Mon, 27 Dec 2021 17:49:39 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Mon, 27 Dec 2021 17:49:39 GMT
VOLUME [/spiped]
# Mon, 27 Dec 2021 17:49:40 GMT
WORKDIR /spiped
# Mon, 27 Dec 2021 17:49:40 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 27 Dec 2021 17:49:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 27 Dec 2021 17:49:41 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:054429d0cf4038fef39a3b5eb6ce52f600f9a2cbb71a4fb3e95ecf9b2da62581`  
		Last Modified: Tue, 21 Dec 2021 02:05:52 GMT  
		Size: 28.9 MB (28900253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:464a6f781a7abbf2236545af22e3b305148755b938eb4b3f80acfddda83fb330`  
		Last Modified: Mon, 27 Dec 2021 17:50:13 GMT  
		Size: 1.7 KB (1729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:901947b41fdff91f97c93d69ea6510e742f77e91ebe42dfb3151adcdaf03441a`  
		Last Modified: Mon, 27 Dec 2021 17:50:13 GMT  
		Size: 1.1 KB (1056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f468550fb64a624779d011e733e2288492ceeefbf1195d64f8bd54e57f57e4f`  
		Last Modified: Mon, 27 Dec 2021 17:50:18 GMT  
		Size: 5.0 MB (5027325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5aa37e6545912e2b7148568d33bbf517e5deadd118df40ce2ebe5f74710c2d66`  
		Last Modified: Mon, 27 Dec 2021 17:50:13 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18b0df784f0906422ce5e4c8eb5ee379506682e1ad31e783eeca4525c79ba55c`  
		Last Modified: Mon, 27 Dec 2021 17:50:13 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; arm variant v7

```console
$ docker pull spiped@sha256:5ff37adf5b2ffdb562129ff2c4c257c774150b80d954a9a0de388a5cd9c14ab4
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.3 MB (31311461 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:07fa1788ed3cfcc665390b07c5ea81b3818793dc7e8cd3cff01c89fc109cb0be`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 21 Dec 2021 01:59:48 GMT
ADD file:6a5555c3e40db91fae5bb112464a4c405a976de17ff64c98f25d3033a6a608d8 in / 
# Tue, 21 Dec 2021 01:59:48 GMT
CMD ["bash"]
# Mon, 27 Dec 2021 17:58:52 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Mon, 27 Dec 2021 17:58:59 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Mon, 27 Dec 2021 17:58:59 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Mon, 27 Dec 2021 17:59:46 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Mon, 27 Dec 2021 17:59:47 GMT
VOLUME [/spiped]
# Mon, 27 Dec 2021 17:59:47 GMT
WORKDIR /spiped
# Mon, 27 Dec 2021 17:59:48 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 27 Dec 2021 17:59:48 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 27 Dec 2021 17:59:49 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:d0061d6703dc4975804c3419e00c85efbe3f1b79c86d87e048fa14a683e88e31`  
		Last Modified: Tue, 21 Dec 2021 02:15:26 GMT  
		Size: 26.6 MB (26560815 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:379d1aaaf5cba2bb5aa182cc038a59938629d1ad6ec388340be3e8f34e5e65b0`  
		Last Modified: Mon, 27 Dec 2021 18:01:17 GMT  
		Size: 1.7 KB (1730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f6950d1ddd5e954a00fd9b56a607f737d4394ec2519f9c9d47ce2820e12bcfb`  
		Last Modified: Mon, 27 Dec 2021 18:01:17 GMT  
		Size: 1.1 KB (1054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6424dc46a62a8c5530fa74a2aaddc612ea6e099df67cfbe39b49dad4b2416fa4`  
		Last Modified: Mon, 27 Dec 2021 18:01:21 GMT  
		Size: 4.7 MB (4747390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b16a5e406437b655a5c55e8e9027607ad607deb3047cf60539ca94a8a6dd8be`  
		Last Modified: Mon, 27 Dec 2021 18:01:18 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c526844e52b7ac486211e17526f3bd96806de407bdad85bbace1e9268e01d2c`  
		Last Modified: Mon, 27 Dec 2021 18:01:17 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:076eed23d69622023465551277b292c4b20c7e53ff970f4ec2c0c88c721002a3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.3 MB (35310451 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:558381a048e4dd5c28f2a72bdfb28f021302afc0b9044d17373f8513e2c57b64`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 21 Dec 2021 01:42:23 GMT
ADD file:986f91febed4aa8e2072081ff8419d52ba2060510822e717086d3b3d9469e4d7 in / 
# Tue, 21 Dec 2021 01:42:24 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 13:37:31 GMT
RUN groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 21 Dec 2021 13:37:35 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 13:37:35 GMT
ENV SPIPED_VERSION=1.6.1 SPIPED_DOWNLOAD_SHA256=8d7089979db79a531a0ecc507b113ac6f2cf5f19305571eff1d3413e0ab33713
# Tue, 21 Dec 2021 13:37:56 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 21 Dec 2021 13:37:57 GMT
VOLUME [/spiped]
# Tue, 21 Dec 2021 13:37:58 GMT
WORKDIR /spiped
# Tue, 21 Dec 2021 13:38:00 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 21 Dec 2021 13:38:00 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 21 Dec 2021 13:38:01 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:927a35006d93ea08499b57046904046d7926cd76fb17be193e3e74f56d634a08`  
		Last Modified: Tue, 21 Dec 2021 01:48:54 GMT  
		Size: 30.0 MB (30043793 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11307cfb62981d1477c624d0946d440cae59b97d5241be5622b4a1a2170b7087`  
		Last Modified: Tue, 21 Dec 2021 13:38:28 GMT  
		Size: 1.6 KB (1618 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a0b4f4a9f9d7183fa8a6390427dd6151121434bd32d1539e46a81b5b7195e9e`  
		Last Modified: Tue, 21 Dec 2021 13:38:28 GMT  
		Size: 924.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:498cf759f2f5ad49bf12c6c9162ea1c630f9fba1005c0a5cd96d9d40f3c3bc9c`  
		Last Modified: Tue, 21 Dec 2021 13:38:30 GMT  
		Size: 5.3 MB (5263680 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7310cca9b3933670873fa963c55ba0370617e570124050a904a3eabfd50f0b8a`  
		Last Modified: Tue, 21 Dec 2021 13:38:29 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3ebb7feec0bee35aea3ecb3f98485656fa38f1ef9c1c9faccf4d07b68e3ebbe`  
		Last Modified: Tue, 21 Dec 2021 13:38:28 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; 386

```console
$ docker pull spiped@sha256:126609a7885028d241e5a5879a81db1e409324ad4299d35fa13d8cb81db7741b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.3 MB (40265566 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e63888bbd27971f057151d0bfa298298857717efa83c94412e8ccc0a77dd65d5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 21 Dec 2021 01:40:06 GMT
ADD file:6b67a0d4d176747cc8cefbd105facde82f1795467bf02eb45e8385c91cdc9c41 in / 
# Tue, 21 Dec 2021 01:40:09 GMT
CMD ["bash"]
# Mon, 27 Dec 2021 18:38:49 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Mon, 27 Dec 2021 18:38:53 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Mon, 27 Dec 2021 18:38:53 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Mon, 27 Dec 2021 18:39:18 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Mon, 27 Dec 2021 18:39:19 GMT
VOLUME [/spiped]
# Mon, 27 Dec 2021 18:39:19 GMT
WORKDIR /spiped
# Mon, 27 Dec 2021 18:39:19 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 27 Dec 2021 18:39:20 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 27 Dec 2021 18:39:20 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:9b9a100d632569e96aeb2d7b0bc45bc436609bb61335815f207994f3b557f0f7`  
		Last Modified: Tue, 21 Dec 2021 01:48:45 GMT  
		Size: 32.4 MB (32370850 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bacb6a90485f91c14c0461997a7afe3993a50f138c22f09ce39f21024c2062b8`  
		Last Modified: Mon, 27 Dec 2021 18:40:12 GMT  
		Size: 1.7 KB (1730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15dd5efb02f26ea602aaebe8f67a9f3a6947dad763a495fef3a9318f12fface9`  
		Last Modified: Mon, 27 Dec 2021 18:40:12 GMT  
		Size: 1.1 KB (1058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82f0e51dee85e4dcfc46978558a24091bc87a2559c3f2a36c3543893184a4c43`  
		Last Modified: Mon, 27 Dec 2021 18:40:14 GMT  
		Size: 7.9 MB (7891457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8925f3c59859f8e255f517eb2391360847148d17eb2715caa30753707600716`  
		Last Modified: Mon, 27 Dec 2021 18:40:12 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce7c6638e6c8f4a87a2847736b51b3093f589a601733574eb08c60e0c4707d43`  
		Last Modified: Mon, 27 Dec 2021 18:40:12 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; mips64le

```console
$ docker pull spiped@sha256:130c01d2a02859608af1ff69b512e606c6b0afab129f4f55f3b214e4439a961e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.3 MB (35327767 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8059d8a507f312d8d77dc186576b8b33cbc65306a9ff8fd918ca17b2b9163198`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 21 Dec 2021 02:09:07 GMT
ADD file:9e5931d5ed32a23b2e93bd8846258c647613637c581b6813bbc7d7e6b86bbdf5 in / 
# Tue, 21 Dec 2021 02:09:08 GMT
CMD ["bash"]
# Mon, 27 Dec 2021 18:07:30 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Mon, 27 Dec 2021 18:07:41 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Mon, 27 Dec 2021 18:07:41 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Mon, 27 Dec 2021 18:08:36 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Mon, 27 Dec 2021 18:08:36 GMT
VOLUME [/spiped]
# Mon, 27 Dec 2021 18:08:37 GMT
WORKDIR /spiped
# Mon, 27 Dec 2021 18:08:37 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 27 Dec 2021 18:08:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 27 Dec 2021 18:08:38 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:6a6edb95e2485a5b9b3c44b27b7ebad16384c0e08a3d61b7e48c65d7278763cf`  
		Last Modified: Tue, 21 Dec 2021 02:18:14 GMT  
		Size: 29.6 MB (29619177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffc41050c10fb28c363303084d216e4a84358c365e0c0c3ea780e76094ac5b62`  
		Last Modified: Mon, 27 Dec 2021 18:08:50 GMT  
		Size: 1.7 KB (1735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ccfed374e34e3e33bb1dac88ddd7d7bd1e7f5274368492e37c693a71768d15b`  
		Last Modified: Mon, 27 Dec 2021 18:08:50 GMT  
		Size: 1.0 KB (1028 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13d7546f5c1590f88787a1fc6a1c2e0d48c67af85dd4b7e8249ff573bee2daad`  
		Last Modified: Mon, 27 Dec 2021 18:08:55 GMT  
		Size: 5.7 MB (5705389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e85af9afd2d869bd928b4990f6fd908f635c5421d1dc8083fc5fd377b8bbd90`  
		Last Modified: Mon, 27 Dec 2021 18:08:50 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:870f16daf77f715fb9dc96eccb5b8d4af6d8b166fa70454d7fab605bd39d022b`  
		Last Modified: Mon, 27 Dec 2021 18:08:50 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; ppc64le

```console
$ docker pull spiped@sha256:60a73d5603e4031736039ecc463577365c1f717538d9abebaffc2f8772464669
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.3 MB (41260220 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:33b349656fc3b5caf98e066d0fdb6c40beca910e76b65314e5f1f5cfea9fc2c5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 21 Dec 2021 02:20:24 GMT
ADD file:078a17bf7e519cb7a60fbbf743ba7e5897554201cb44957154ab518d6991a033 in / 
# Tue, 21 Dec 2021 02:20:28 GMT
CMD ["bash"]
# Mon, 27 Dec 2021 18:16:48 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Mon, 27 Dec 2021 18:16:58 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Mon, 27 Dec 2021 18:17:00 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Mon, 27 Dec 2021 18:18:26 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Mon, 27 Dec 2021 18:18:28 GMT
VOLUME [/spiped]
# Mon, 27 Dec 2021 18:18:31 GMT
WORKDIR /spiped
# Mon, 27 Dec 2021 18:18:32 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 27 Dec 2021 18:18:34 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 27 Dec 2021 18:18:37 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:3345479fea0cdce1382b927b0908af4f239b288b30efa203c50edf7ac0cb055e`  
		Last Modified: Tue, 21 Dec 2021 02:29:20 GMT  
		Size: 35.3 MB (35258992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45821758d9ac9ef7ddf59278b25a098454da513ab2a4469079d31efd2872e496`  
		Last Modified: Mon, 27 Dec 2021 18:20:01 GMT  
		Size: 1.7 KB (1734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6621a4339ab8321307888b642f6c34ede9ba4af6ac0ed96e946ac50ec1227849`  
		Last Modified: Mon, 27 Dec 2021 18:20:01 GMT  
		Size: 1.1 KB (1057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2eb85ea75c9e8b313cfbfc6e4cfef155d0183d2f926c786afe58fc17f96afdae`  
		Last Modified: Mon, 27 Dec 2021 18:20:03 GMT  
		Size: 6.0 MB (5997966 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92b8831f840f6baaf8d56f6cae0b098c6a56d239108b4ae79ca3788881609e16`  
		Last Modified: Mon, 27 Dec 2021 18:20:01 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:918e7af5ea63b6fcb7ce923b4e73eaf873a1247710e432fc8214fd19aad04405`  
		Last Modified: Mon, 27 Dec 2021 18:20:01 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; s390x

```console
$ docker pull spiped@sha256:85d5e0719445d2cdab3cbf858a459655e3240a92ee8d2f2f802f6ac1b211f948
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.8 MB (34830564 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c2df5426aa3ed82a47988087e8347fbcad4453d2a97b19988ddb6026a0947c78`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 21 Dec 2021 01:42:27 GMT
ADD file:c8a482d41bf09dfb6484bf2a6e38535bf0594d26dd6eedd5abde4e3cc811fa6c in / 
# Tue, 21 Dec 2021 01:42:29 GMT
CMD ["bash"]
# Mon, 27 Dec 2021 18:41:39 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Mon, 27 Dec 2021 18:41:42 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Mon, 27 Dec 2021 18:41:42 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Mon, 27 Dec 2021 18:41:54 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Mon, 27 Dec 2021 18:41:55 GMT
VOLUME [/spiped]
# Mon, 27 Dec 2021 18:41:55 GMT
WORKDIR /spiped
# Mon, 27 Dec 2021 18:41:55 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 27 Dec 2021 18:41:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 27 Dec 2021 18:41:55 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:12562551722a758d23ceea9abcdc2bee737e38c8f62a0f3d3afb2cc2626c28b1`  
		Last Modified: Tue, 21 Dec 2021 01:48:15 GMT  
		Size: 29.6 MB (29641636 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e50be5fdb0a5e34432208396d23522b1701f3dff2f0ad3d78fbd79b6b41b6ce`  
		Last Modified: Mon, 27 Dec 2021 18:42:37 GMT  
		Size: 1.7 KB (1739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a42e79bc5e5489f7b5513adce4e87bffd082bb140296c35dd729fa90a5a4868`  
		Last Modified: Mon, 27 Dec 2021 18:42:37 GMT  
		Size: 1.1 KB (1052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e1da3833503470ef9b807b846f2ff4fbaaab0831b1447b2f18bba93952c3435`  
		Last Modified: Mon, 27 Dec 2021 18:42:38 GMT  
		Size: 5.2 MB (5185667 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4c82c9810dbf5e873e822ea28782e813bd5277a73013e0e015bf69827be95f1`  
		Last Modified: Mon, 27 Dec 2021 18:42:37 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51b12ef5c112d47a91c90766ac49e1b42fd0a2a3a6c3d6af4b2349c285ea742c`  
		Last Modified: Mon, 27 Dec 2021 18:42:37 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
