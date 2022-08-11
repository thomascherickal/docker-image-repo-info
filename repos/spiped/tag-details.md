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
$ docker pull spiped@sha256:6442d9ca640a1475fe7f8827406c94ab677a48776e9653472bd6523a120609dc
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
$ docker pull spiped@sha256:dad19d6d4fd551afedb73402fbe587665af498a94aab95d1f1c65b6fca26b254
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.3 MB (37337269 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ad8d035bd9a75027ee1fd4c3aa1157c358bb1ffceba1d2ae6cee8caa104b286a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 02 Aug 2022 01:20:04 GMT
ADD file:0eae0dca665c7044bf242cb1fc92cb8ea744f5af2dd376a558c90bc47349aefe in / 
# Tue, 02 Aug 2022 01:20:05 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 14:59:44 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 02 Aug 2022 14:59:47 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 14:59:47 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 02 Aug 2022 15:00:07 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 02 Aug 2022 15:00:08 GMT
VOLUME [/spiped]
# Tue, 02 Aug 2022 15:00:08 GMT
WORKDIR /spiped
# Tue, 02 Aug 2022 15:00:08 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 02 Aug 2022 15:00:08 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 02 Aug 2022 15:00:08 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:1efc276f4ff952c055dea726cfc96ec6a4fdb8b62d9eed816bd2b788f2860ad7`  
		Last Modified: Tue, 02 Aug 2022 01:24:13 GMT  
		Size: 31.4 MB (31366757 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71902ff87bbf89a7cab2e1efdfe743d124a3eb6896b31675c52ab90dd16095e9`  
		Last Modified: Tue, 02 Aug 2022 15:00:25 GMT  
		Size: 1.7 KB (1733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a4a4f0063093cdc07df60de1a6d30e856a4ed528faac41e365607eb44758cec`  
		Last Modified: Tue, 02 Aug 2022 15:00:25 GMT  
		Size: 1.0 KB (1049 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33ba4d77b594746542f2e71dd52678ddd883c436d88b72e2465c4eb7e01809da`  
		Last Modified: Tue, 02 Aug 2022 15:00:26 GMT  
		Size: 6.0 MB (5967261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71bba1d841b515de61167758f804ee176e5ae08c5d1171a8fda3781007b78158`  
		Last Modified: Tue, 02 Aug 2022 15:00:25 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:634b21022fb2ad7cfda5a174c30da9483511cea6cc668b1c7b925613d777cfb2`  
		Last Modified: Tue, 02 Aug 2022 15:00:25 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; arm variant v5

```console
$ docker pull spiped@sha256:6af880d390673b3da576db810a3f341c7e097879fd5b825384cf454c94209ca3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.9 MB (33936434 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1c3ede774f72c0efbe443d6545abe99b06d36efbdac21a941da05cf12db4dd78`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 02 Aug 2022 00:49:10 GMT
ADD file:4cd2f95737fd3007912428eeac56036c9e67e989e66cec08a8be99da47f88494 in / 
# Tue, 02 Aug 2022 00:49:10 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 19:51:33 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 02 Aug 2022 19:51:40 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 19:51:40 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 02 Aug 2022 19:52:11 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 02 Aug 2022 19:52:11 GMT
VOLUME [/spiped]
# Tue, 02 Aug 2022 19:52:11 GMT
WORKDIR /spiped
# Tue, 02 Aug 2022 19:52:12 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 02 Aug 2022 19:52:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 02 Aug 2022 19:52:12 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:5890b0ca6af5e8467a488e68716691950496a8f247d0495c2d595ddcb1893aff`  
		Last Modified: Tue, 02 Aug 2022 00:56:06 GMT  
		Size: 28.9 MB (28905515 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5914210ab5e9d450cc5cc817ba9a969a99a1bba9caff02b44bcf07b6daa99101`  
		Last Modified: Tue, 02 Aug 2022 19:52:38 GMT  
		Size: 1.7 KB (1726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:591059447642cb76dea322da399255cce3dfc35a2ab27142398a6c0b76c7db1a`  
		Last Modified: Tue, 02 Aug 2022 19:52:38 GMT  
		Size: 1.1 KB (1053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b596d1e863582490afb5019016264b3b75d44f08716d556cd395a4286210a5d`  
		Last Modified: Tue, 02 Aug 2022 19:52:41 GMT  
		Size: 5.0 MB (5027669 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:786bcf276f826fa83f9eef22ee3dd243c1b03582f76dcf0d838c8036997e795e`  
		Last Modified: Tue, 02 Aug 2022 19:52:38 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17e2aa3589894439340437bb0befccb5068c4051e6cc7b57e53f7e764bf4beb0`  
		Last Modified: Tue, 02 Aug 2022 19:52:39 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; arm variant v7

```console
$ docker pull spiped@sha256:05546f55c08afb1515cfc5708756ed4940307346ba553f0f975bf31140ab7573
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.3 MB (31311995 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fe18f0b13d76c9fe4af1797ce9d740ef87d42b1ce2094b53680be65b310394ed`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 02 Aug 2022 00:58:59 GMT
ADD file:1575b776a15adacebc0875642e97a80807d42dcfc8917e1406d47af7ac244c97 in / 
# Tue, 02 Aug 2022 00:58:59 GMT
CMD ["bash"]
# Wed, 03 Aug 2022 21:56:42 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 03 Aug 2022 21:56:45 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 03 Aug 2022 21:56:45 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 03 Aug 2022 21:57:01 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 03 Aug 2022 21:57:01 GMT
VOLUME [/spiped]
# Wed, 03 Aug 2022 21:57:01 GMT
WORKDIR /spiped
# Wed, 03 Aug 2022 21:57:01 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 03 Aug 2022 21:57:01 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 03 Aug 2022 21:57:01 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:1dd75a3a9c893a7dc313f683dd62464b7eab6c6d522ee62c8a17022631830f32`  
		Last Modified: Tue, 02 Aug 2022 01:06:45 GMT  
		Size: 26.6 MB (26560586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bcaffbe5be1966b473b328a91c40df9286228c74466eea7154a543527b6fae1`  
		Last Modified: Wed, 03 Aug 2022 21:57:45 GMT  
		Size: 1.7 KB (1726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2917d25466b0b307ff25a0fc7718a5e32785e7eef826f642b28d0439be6adc9e`  
		Last Modified: Wed, 03 Aug 2022 21:57:45 GMT  
		Size: 1.1 KB (1053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7caa787abd6178478de179d6cc5db9a07a792b29b34b9fc9486347a7c1b017f`  
		Last Modified: Wed, 03 Aug 2022 21:57:46 GMT  
		Size: 4.7 MB (4748161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3801153d36fffb70fcfc49890ef5d327bfc8b15f3a1cc6fa4d0d9b12eb27ff9`  
		Last Modified: Wed, 03 Aug 2022 21:57:45 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a742fab32925896cf7cffe6ca60ee420e328f9391fe5bcfc9f1f46e7f631ce3a`  
		Last Modified: Wed, 03 Aug 2022 21:57:45 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:4835debf7fbae32c4cc4cdc11e8792dc97767b8916ed69b695839b47ce2c5b49
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.3 MB (35328219 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:11bb3a1dd6e7229d9d7d203d5f015250cd44ab7d412ae6d00adbe3817b938ceb`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 02 Aug 2022 00:40:38 GMT
ADD file:6039adfbca55ed34a719c37672c664e3524130a0e2a3b8663629b8120b81b790 in / 
# Tue, 02 Aug 2022 00:40:39 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 16:47:23 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 02 Aug 2022 16:47:26 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 16:47:27 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 02 Aug 2022 16:47:45 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 02 Aug 2022 16:47:45 GMT
VOLUME [/spiped]
# Tue, 02 Aug 2022 16:47:46 GMT
WORKDIR /spiped
# Tue, 02 Aug 2022 16:47:48 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 02 Aug 2022 16:47:48 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 02 Aug 2022 16:47:49 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:a9fe95647e78b5516c7e2327355b6996e2ea295cd76ae242cbfe87f016b4e760`  
		Last Modified: Tue, 02 Aug 2022 00:46:05 GMT  
		Size: 30.1 MB (30054304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0215749fa5edad97431836093e99ce69829b4a2b18c351fe7e22c9bf90cb3fef`  
		Last Modified: Tue, 02 Aug 2022 16:48:17 GMT  
		Size: 1.6 KB (1617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6a61c46ac9b56671e11f61590184265582230b634537e091aa7515746a2ba70`  
		Last Modified: Tue, 02 Aug 2022 16:48:17 GMT  
		Size: 923.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:569abb15b59f2ea4b1fe7a95bda8247ac40c93685ac62b8029db8474d42f79cb`  
		Last Modified: Tue, 02 Aug 2022 16:48:18 GMT  
		Size: 5.3 MB (5270939 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:251fbe05e0ceba0f0f43f71ba704ee1b264165c62e3d7f999b3c597690886a75`  
		Last Modified: Tue, 02 Aug 2022 16:48:17 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10996acb338f32bf51751686febf31fd3fab4b1d46b4b8d7a7d5dfc7f05b4cee`  
		Last Modified: Tue, 02 Aug 2022 16:48:17 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; 386

```console
$ docker pull spiped@sha256:7a7dbde9446433fedc12b55ed6d0d73bbbf800753f0b4fc8c677bfd9f5d6f1fd
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.3 MB (40268619 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8544e7c71f7ba6f5ac7741eec3a5f49bd5d384c7d708d24631e0ce7e8af09460`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 02 Aug 2022 00:39:20 GMT
ADD file:f771e2286465694126158821089d801c7296376be2a56189e6041a15d2fe79f5 in / 
# Tue, 02 Aug 2022 00:39:21 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 15:45:02 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 02 Aug 2022 15:45:06 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 15:45:07 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 02 Aug 2022 15:45:28 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 02 Aug 2022 15:45:28 GMT
VOLUME [/spiped]
# Tue, 02 Aug 2022 15:45:29 GMT
WORKDIR /spiped
# Tue, 02 Aug 2022 15:45:31 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 02 Aug 2022 15:45:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 02 Aug 2022 15:45:32 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:90eb7f0ce9f33cf5dcd67d54c2fa606186dbaa5f95b6046f36145097267f9e53`  
		Last Modified: Tue, 02 Aug 2022 00:45:14 GMT  
		Size: 32.4 MB (32374054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:746b1fc4bab3964ac48dbe2fb0761a50ec33f467093556cf01fd8444415d8d11`  
		Last Modified: Tue, 02 Aug 2022 15:46:02 GMT  
		Size: 1.6 KB (1606 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2441fccbf951fe6e18f386cdd0c3cabaa845fde7d0bf966cf03f04f756510e6a`  
		Last Modified: Tue, 02 Aug 2022 15:46:02 GMT  
		Size: 924.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:231b6d32c27ff4a17c9587d6b1f9b787bb6d78e3d656a8c9467df93a850bd66f`  
		Last Modified: Tue, 02 Aug 2022 15:46:03 GMT  
		Size: 7.9 MB (7891596 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:072a58cf67fb04afdb3086a5a441fa938a2ede9871a6088da9f6bfd36cc65467`  
		Last Modified: Tue, 02 Aug 2022 15:46:02 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cac32ec13523eeeefcd7dcfb5c9f5cbd39875a916b3fa22df5b9af8f12e83aba`  
		Last Modified: Tue, 02 Aug 2022 15:46:02 GMT  
		Size: 344.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; mips64le

```console
$ docker pull spiped@sha256:9e5c7480cebb7266cbc6cd8cde915e916cea44f839c3d45827ee4b32b9d1f361
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.3 MB (35337243 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6d937f2142b4729449865145c0bd382f2880465d957aac461a860e13e82a8527`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 02 Aug 2022 01:10:34 GMT
ADD file:6dc22a1e5b5fcf23f2549406ddcc45c4e244f46e21eafa881de81fa87438e5d8 in / 
# Tue, 02 Aug 2022 01:10:38 GMT
CMD ["bash"]
# Thu, 04 Aug 2022 02:58:17 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Thu, 04 Aug 2022 02:58:32 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Thu, 04 Aug 2022 02:58:34 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 04 Aug 2022 03:00:04 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 04 Aug 2022 03:00:07 GMT
VOLUME [/spiped]
# Thu, 04 Aug 2022 03:00:09 GMT
WORKDIR /spiped
# Thu, 04 Aug 2022 03:00:12 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 04 Aug 2022 03:00:14 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 04 Aug 2022 03:00:17 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:88350749a27614c791450c256b051f023d81cdd256211274b1efac493779d2be`  
		Last Modified: Tue, 02 Aug 2022 01:21:02 GMT  
		Size: 29.6 MB (29628964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a980b8d4c4081e06e63d932cacd2a2bcb9ae4455ec1d8a0edfd5e7b976a41cfe`  
		Last Modified: Thu, 04 Aug 2022 03:00:33 GMT  
		Size: 1.6 KB (1619 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e926997286379c4294d14e53409efda33e6b135fe7e1090595de1c642b53a3b2`  
		Last Modified: Thu, 04 Aug 2022 03:00:34 GMT  
		Size: 923.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28c8df0b5ceb34f25514a9e6cfc3c5e4d4fa32daaa3e805d0e78bade747962e7`  
		Last Modified: Thu, 04 Aug 2022 03:00:38 GMT  
		Size: 5.7 MB (5705299 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe20d03337baf8ea0077260b2c5f5754fca122b1397f8ac922fb9db8dff5995b`  
		Last Modified: Thu, 04 Aug 2022 03:00:33 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca8d9c536c2096001a16837bafc47410185a740c029f1aad11b395642de38f34`  
		Last Modified: Thu, 04 Aug 2022 03:00:33 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; ppc64le

```console
$ docker pull spiped@sha256:27f881ff0e1f5e61d9dc98bfdaf60bde63f0b7c46ea39da2ac2c9814dcde8dd6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.3 MB (41274919 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9792967c333043140e04ed3704d0407abc333122050747da7546fc815c45542e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 02 Aug 2022 01:17:30 GMT
ADD file:3a95a896d463569ce82199957052b3467123a4bd3385a0a4e397cf08402a99c3 in / 
# Tue, 02 Aug 2022 01:17:32 GMT
CMD ["bash"]
# Wed, 03 Aug 2022 01:28:12 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 03 Aug 2022 01:28:18 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 03 Aug 2022 01:28:18 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 03 Aug 2022 01:28:56 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 03 Aug 2022 01:28:57 GMT
VOLUME [/spiped]
# Wed, 03 Aug 2022 01:28:57 GMT
WORKDIR /spiped
# Wed, 03 Aug 2022 01:28:58 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 03 Aug 2022 01:28:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 03 Aug 2022 01:28:59 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:5241cd116d6e6e2d62f3d8c2245b74daca9f6cc154eaccd738feb41984c74714`  
		Last Modified: Tue, 02 Aug 2022 01:24:39 GMT  
		Size: 35.3 MB (35272771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52f7bfa7322f80f7fbf327da4c4244442a6121cd2aa6a0c35b98493dff99cd50`  
		Last Modified: Wed, 03 Aug 2022 01:29:58 GMT  
		Size: 1.7 KB (1731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4737eb981cc3c529f234636741599c9b27a9f5b4973f8f9b6a7628649aab6726`  
		Last Modified: Wed, 03 Aug 2022 01:29:58 GMT  
		Size: 1.1 KB (1051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69e43d769614f6318ed658c891a70ce2668635f025c326b0b52a83b54ca1498b`  
		Last Modified: Wed, 03 Aug 2022 01:30:00 GMT  
		Size: 6.0 MB (5998895 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e492fc4ffd0f67e0a0b76b694e326dce271e5ad1bbf157bfb0c9097c0c7df653`  
		Last Modified: Wed, 03 Aug 2022 01:29:58 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2606cce249be48bbc9ec4f0d08c2920e38e1b3a0735446d0a03dd275279ca1cb`  
		Last Modified: Wed, 03 Aug 2022 01:29:58 GMT  
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
$ docker pull spiped@sha256:acddecb1628480a3371f5c7990076e0d894c6a9a2e7612d844e800178fabe8ba
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
$ docker pull spiped@sha256:66b3d848f73df6532c49bb456c441a37691db14797c1288fa9cd5deb9cf9bdb6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (3036703 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ebcb8fdfbde39b2b89abb4cdfac48560f245fff78fc822e3daac086fd5b29f78`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 09 Aug 2022 17:19:53 GMT
ADD file:2a949686d9886ac7c10582a6c29116fd29d3077d02755e87e111870d63607725 in / 
# Tue, 09 Aug 2022 17:19:53 GMT
CMD ["/bin/sh"]
# Wed, 10 Aug 2022 02:25:05 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Wed, 10 Aug 2022 02:25:06 GMT
RUN apk add --no-cache libssl1.1
# Wed, 10 Aug 2022 02:25:06 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 10 Aug 2022 02:25:16 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Wed, 10 Aug 2022 02:25:17 GMT
VOLUME [/spiped]
# Wed, 10 Aug 2022 02:25:17 GMT
WORKDIR /spiped
# Wed, 10 Aug 2022 02:25:17 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 10 Aug 2022 02:25:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 10 Aug 2022 02:25:17 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:213ec9aee27d8be045c6a92b7eac22c9a64b44558193775a1a7f626352392b49`  
		Last Modified: Tue, 09 Aug 2022 14:25:13 GMT  
		Size: 2.8 MB (2806054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:210040c27162008830a83da8ed96f452757ffa50050398230f525b2f22a4541a`  
		Last Modified: Wed, 10 Aug 2022 02:25:34 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b05b54e70388210c7ffd8a9fbb864ca9f878f8ad3dc1613e4b96b107919baadc`  
		Last Modified: Wed, 10 Aug 2022 02:25:34 GMT  
		Size: 7.7 KB (7735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28b8ff19a9777e30476c0a48eab4bc4817e9a96226faf7b42870225d69a37ba8`  
		Last Modified: Wed, 10 Aug 2022 02:25:34 GMT  
		Size: 221.2 KB (221175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:700f71a1b577cfb700f72058dad655d1ec9161da01b7fe6e8bb2b2461d1ddbbe`  
		Last Modified: Wed, 10 Aug 2022 02:25:34 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6c2f8d0b8416d1c553517142cd373249cbbdc3a03229d96604cd32b318a1195`  
		Last Modified: Wed, 10 Aug 2022 02:25:34 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; arm variant v6

```console
$ docker pull spiped@sha256:9bf39d60020a139fa461ebb060df6df01d5164425285c6bfc1b3113ef2242277
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 MB (2829328 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:88197140375c26dcc5aa5dad079e8343608e24c8a03e91eb5d2fb13c9e09deec`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 09 Aug 2022 17:49:22 GMT
ADD file:e8733e8cc0a81e15ca4041760b6e27392c34171512d34405a9b262b1fff5c687 in / 
# Tue, 09 Aug 2022 17:49:22 GMT
CMD ["/bin/sh"]
# Thu, 11 Aug 2022 00:37:38 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 11 Aug 2022 00:37:39 GMT
RUN apk add --no-cache libssl1.1
# Thu, 11 Aug 2022 00:37:39 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 11 Aug 2022 00:37:47 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Thu, 11 Aug 2022 00:37:47 GMT
VOLUME [/spiped]
# Thu, 11 Aug 2022 00:37:47 GMT
WORKDIR /spiped
# Thu, 11 Aug 2022 00:37:47 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 11 Aug 2022 00:37:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 11 Aug 2022 00:37:47 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:9506b835437abb4d8ba1683e00c500b8f77e1975e930b356fbb72f2dbdc274d9`  
		Last Modified: Tue, 09 Aug 2022 17:50:33 GMT  
		Size: 2.6 MB (2613965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3f8a3e1b897eaae3127b4c0c6bf167dc3d7740bbf9596a97a994f1249716538`  
		Last Modified: Thu, 11 Aug 2022 00:38:06 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fa63959f901bfbea0a7da0112a6c04fe32edaaf453bc28bc784d942ef8a1c01`  
		Last Modified: Thu, 11 Aug 2022 00:38:06 GMT  
		Size: 7.7 KB (7736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb53413b98987994a206c07b7c3ba39980d1dd0149f4a1be509beab0c15b75da`  
		Last Modified: Thu, 11 Aug 2022 00:38:06 GMT  
		Size: 205.9 KB (205888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe12872e965332f5c42d1844aa3dfdbae46eda912838801110e130b89cc181ca`  
		Last Modified: Thu, 11 Aug 2022 00:38:06 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a33b8651215087c0b9c9d0edc3a3fb9e0d18f0eaf36a0c0bfcddce94e338d57`  
		Last Modified: Thu, 11 Aug 2022 00:38:06 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; arm variant v7

```console
$ docker pull spiped@sha256:0e746939643dcaba40d0c1f15f4d142129555ff4d3a187e755c3643cb387bca1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 MB (2621321 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:af5a28036aaca6f3accc02f7ab66d26c0d7ef2c544316b0df54081730f89391e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Mon, 18 Jul 2022 21:24:47 GMT
ADD file:68590e866bc6db27ad54d23de7dd275d0389cb86e4e6291a1243fcc234f2f7a1 in / 
# Mon, 18 Jul 2022 21:24:47 GMT
CMD ["/bin/sh"]
# Wed, 03 Aug 2022 21:57:08 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Wed, 03 Aug 2022 21:57:09 GMT
RUN apk add --no-cache libssl1.1
# Wed, 03 Aug 2022 21:57:09 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 03 Aug 2022 21:57:16 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Wed, 03 Aug 2022 21:57:17 GMT
VOLUME [/spiped]
# Wed, 03 Aug 2022 21:57:17 GMT
WORKDIR /spiped
# Wed, 03 Aug 2022 21:57:17 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 03 Aug 2022 21:57:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 03 Aug 2022 21:57:17 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:a6b45ace95f42a930d15c33679ab9c85d46019b7e73954cadc73bb9ba176509b`  
		Last Modified: Mon, 18 Jul 2022 19:08:56 GMT  
		Size: 2.4 MB (2412307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a223ea05945b5c5ea98e31d53b7924f548e24abe646453181a3b73f940a52de`  
		Last Modified: Wed, 03 Aug 2022 21:58:06 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:868bbc51d36bab84123a304360d9b4bc7db9f0714c2281b34b7585ff494ab1c8`  
		Last Modified: Wed, 03 Aug 2022 21:58:06 GMT  
		Size: 7.7 KB (7730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18353dabcadb1dc2dc0b669eeff1d9dd8d42a815bd9f860e8ff08c8f2191131f`  
		Last Modified: Wed, 03 Aug 2022 21:58:06 GMT  
		Size: 199.5 KB (199542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:330712fbce762a1e0c7e7bcf9c36a39c454fa780a6901be6761dd588dc043f5f`  
		Last Modified: Wed, 03 Aug 2022 21:58:06 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:221966fcc255ad5deb2fa5ce1fc0b504eff307dc6e7aaebe7db90698290052eb`  
		Last Modified: Wed, 03 Aug 2022 21:58:06 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:31d9f2978a4900b825028e1c399cd7d0638f75f91f2400f6c6bc1d83d6274fb6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 MB (2931313 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:031699f5a5efac86682c564a2c655c7eab52ce5aa91a856923d2032ea0517c52`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 09 Aug 2022 17:39:41 GMT
ADD file:960fd469d48cf79ba14bbda71f3192074ed860c112e30e0bc92bff3440cb45ab in / 
# Tue, 09 Aug 2022 17:39:42 GMT
CMD ["/bin/sh"]
# Wed, 10 Aug 2022 06:09:41 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Wed, 10 Aug 2022 06:09:42 GMT
RUN apk add --no-cache libssl1.1
# Wed, 10 Aug 2022 06:09:43 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 10 Aug 2022 06:09:54 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Wed, 10 Aug 2022 06:09:55 GMT
VOLUME [/spiped]
# Wed, 10 Aug 2022 06:09:56 GMT
WORKDIR /spiped
# Wed, 10 Aug 2022 06:09:58 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 10 Aug 2022 06:09:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 10 Aug 2022 06:09:59 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:9b18e9b68314027565b90ff6189d65942c0f7986da80df008b8431276885218e`  
		Last Modified: Tue, 09 Aug 2022 17:40:38 GMT  
		Size: 2.7 MB (2707663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bf9d3ec407b6270ec79bb3c0552c48d0afd7888773c72f1b25bfc396d4c3eb7`  
		Last Modified: Wed, 10 Aug 2022 06:10:25 GMT  
		Size: 1.2 KB (1244 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99f1183a0c8143435d389abc100d22d7289e4a81f966ca3b9d8301cfb01947b2`  
		Last Modified: Wed, 10 Aug 2022 06:10:25 GMT  
		Size: 7.7 KB (7710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8abc3813fe4a6ffebb8bdde4bd9005230c2935072094662e52a3a81cc9a9c3fa`  
		Last Modified: Wed, 10 Aug 2022 06:10:26 GMT  
		Size: 214.3 KB (214262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab3f496ad70b8f2f8ea93c54500ad75fb9fa4b72d7868ae964cce858765988a4`  
		Last Modified: Wed, 10 Aug 2022 06:10:26 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46086b9ffd0c9eed5aadecf28229d0ab4532a26add5be2f474ced21cf4f25f7e`  
		Last Modified: Wed, 10 Aug 2022 06:10:25 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; 386

```console
$ docker pull spiped@sha256:ee4833bbef16308d250de2dac9ad7a6019a6f2e42880ed8eb3dfd4fcecc4ced4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (3047835 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:75c145e337e061db2f783bf06d6d6b2f1e63cf3e7dedb8ada91bc1744b707620`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 09 Aug 2022 17:38:39 GMT
ADD file:b828bc14bc5ff03c8f7310fe0aed6ac5df19a393622d5d1d779a523234d07c0a in / 
# Tue, 09 Aug 2022 17:38:39 GMT
CMD ["/bin/sh"]
# Wed, 10 Aug 2022 00:02:16 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Wed, 10 Aug 2022 00:02:18 GMT
RUN apk add --no-cache libssl1.1
# Wed, 10 Aug 2022 00:02:19 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 10 Aug 2022 00:02:30 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Wed, 10 Aug 2022 00:02:31 GMT
VOLUME [/spiped]
# Wed, 10 Aug 2022 00:02:32 GMT
WORKDIR /spiped
# Wed, 10 Aug 2022 00:02:34 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 10 Aug 2022 00:02:34 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 10 Aug 2022 00:02:35 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:6c0d3b419d848ea31ca748254611d5d5ce3b76e3d7bba520fd87400fbb75f3b9`  
		Last Modified: Tue, 09 Aug 2022 17:39:33 GMT  
		Size: 2.8 MB (2807121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:072149e09853327c1921fc351fbf7a93e1056edfefc5daa66cbdc6e48843cd13`  
		Last Modified: Wed, 10 Aug 2022 00:03:04 GMT  
		Size: 1.2 KB (1243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34965b4906426a2b44e36dc3fd455d5da36569c3a0c3de199beecfc03c85244c`  
		Last Modified: Wed, 10 Aug 2022 00:03:04 GMT  
		Size: 7.7 KB (7710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ddeae6e8a846e3df57fb016e864191c85342272b8c766aea5b9cd0e001b0332`  
		Last Modified: Wed, 10 Aug 2022 00:03:05 GMT  
		Size: 231.3 KB (231325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:463f4e96eadc8d28add083b4c188fcdde9cecb3831b8c5427343441c383e1136`  
		Last Modified: Wed, 10 Aug 2022 00:03:04 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3648573cf3f78bda63b9ea60198dd66926dda5cbd250025fbf6c5c0f08bbbcb4`  
		Last Modified: Wed, 10 Aug 2022 00:03:04 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; ppc64le

```console
$ docker pull spiped@sha256:d67f02f9e68884fbd145362c4f490cdfb403437bcf89d1135ad1a15c92052a5a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (3033050 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:14fd901b20c0f04f13ac388776797050b3e6a48903ceeccca414c16f53e1c29f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 09 Aug 2022 17:17:09 GMT
ADD file:66b351666e41834033d334aeb3dc6998dea77aa22e8e254028c923fee67a41a8 in / 
# Tue, 09 Aug 2022 17:17:10 GMT
CMD ["/bin/sh"]
# Wed, 10 Aug 2022 02:55:17 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Wed, 10 Aug 2022 02:55:19 GMT
RUN apk add --no-cache libssl1.1
# Wed, 10 Aug 2022 02:55:19 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 10 Aug 2022 02:55:34 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Wed, 10 Aug 2022 02:55:34 GMT
VOLUME [/spiped]
# Wed, 10 Aug 2022 02:55:35 GMT
WORKDIR /spiped
# Wed, 10 Aug 2022 02:55:36 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 10 Aug 2022 02:55:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 10 Aug 2022 02:55:36 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:c79e5d1a8c89b87020a754c8a5c8370faaa37bfb5bca1d8af66770d522ef1caf`  
		Last Modified: Tue, 09 Aug 2022 17:18:26 GMT  
		Size: 2.8 MB (2803320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cd8832ea95a37bc42923d861cfefd27ec973fed3564060fce137b8d54f75e02`  
		Last Modified: Wed, 10 Aug 2022 02:56:11 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ab0760cebdd26f5d818b164fe30701e72c6ec6c6c6b97b100ed16bc24fcf653`  
		Last Modified: Wed, 10 Aug 2022 02:56:11 GMT  
		Size: 7.7 KB (7739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8cdb874eec093d50ac091467e93cb88955a1ee87db0d0dd84cc6344ad829323`  
		Last Modified: Wed, 10 Aug 2022 02:56:11 GMT  
		Size: 220.3 KB (220255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a349e85c23948cd849a1a373c684ee566e0544af2297f9904d664dbb41dc8a6`  
		Last Modified: Wed, 10 Aug 2022 02:56:22 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bd274005021e79dbc526fb1fd7ad0d420d2e5c10abf68e3c7ae46021ae45cbf`  
		Last Modified: Wed, 10 Aug 2022 02:56:11 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; s390x

```console
$ docker pull spiped@sha256:936312a4e0595fc377ed5e910f12d52cfc4fae63a6190fe388481f204758a480
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 MB (2808502 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:afa6705ab1cc71e7aa223e1b9c9ba81f85eacacdba00737aa34a7014d8d94163`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 09 Aug 2022 17:41:46 GMT
ADD file:b43a065471bc4711415d3c67cd5b6559b0c48ee7ffe9761530477cf457a6dc34 in / 
# Tue, 09 Aug 2022 17:41:46 GMT
CMD ["/bin/sh"]
# Wed, 10 Aug 2022 05:46:33 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Wed, 10 Aug 2022 05:46:34 GMT
RUN apk add --no-cache libssl1.1
# Wed, 10 Aug 2022 05:46:34 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 10 Aug 2022 05:46:39 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Wed, 10 Aug 2022 05:46:39 GMT
VOLUME [/spiped]
# Wed, 10 Aug 2022 05:46:39 GMT
WORKDIR /spiped
# Wed, 10 Aug 2022 05:46:39 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 10 Aug 2022 05:46:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 10 Aug 2022 05:46:40 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:790c84f1f3409eab952345157df7fa804ba6b5f06d4ceb6f2dfa3c6de2064397`  
		Last Modified: Tue, 09 Aug 2022 17:42:45 GMT  
		Size: 2.6 MB (2590597 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e997054cff6af24fce535516fc4358eabc7dace5f52f427e6a19340c04f6adfe`  
		Last Modified: Wed, 10 Aug 2022 05:47:31 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b78da263b8c9f381935ae64289597db6f2e0d7e77fa388ce819ba7afecd17ef1`  
		Last Modified: Wed, 10 Aug 2022 05:47:35 GMT  
		Size: 7.7 KB (7742 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1acce323c9898120275bb4b4763b7a8971f71720bf7cafb55201dc313247560c`  
		Last Modified: Wed, 10 Aug 2022 05:47:35 GMT  
		Size: 208.4 KB (208429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98b550d52792a92d7c50d7e5102763598d59d41f0c34d5bd928fbd55e16de8f8`  
		Last Modified: Wed, 10 Aug 2022 05:47:35 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:130443af95b4efa2ff2d4d039066967531a4e10357d515888d55082f26340a52`  
		Last Modified: Wed, 10 Aug 2022 05:47:35 GMT  
		Size: 336.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:1.6`

```console
$ docker pull spiped@sha256:6442d9ca640a1475fe7f8827406c94ab677a48776e9653472bd6523a120609dc
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
$ docker pull spiped@sha256:dad19d6d4fd551afedb73402fbe587665af498a94aab95d1f1c65b6fca26b254
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.3 MB (37337269 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ad8d035bd9a75027ee1fd4c3aa1157c358bb1ffceba1d2ae6cee8caa104b286a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 02 Aug 2022 01:20:04 GMT
ADD file:0eae0dca665c7044bf242cb1fc92cb8ea744f5af2dd376a558c90bc47349aefe in / 
# Tue, 02 Aug 2022 01:20:05 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 14:59:44 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 02 Aug 2022 14:59:47 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 14:59:47 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 02 Aug 2022 15:00:07 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 02 Aug 2022 15:00:08 GMT
VOLUME [/spiped]
# Tue, 02 Aug 2022 15:00:08 GMT
WORKDIR /spiped
# Tue, 02 Aug 2022 15:00:08 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 02 Aug 2022 15:00:08 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 02 Aug 2022 15:00:08 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:1efc276f4ff952c055dea726cfc96ec6a4fdb8b62d9eed816bd2b788f2860ad7`  
		Last Modified: Tue, 02 Aug 2022 01:24:13 GMT  
		Size: 31.4 MB (31366757 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71902ff87bbf89a7cab2e1efdfe743d124a3eb6896b31675c52ab90dd16095e9`  
		Last Modified: Tue, 02 Aug 2022 15:00:25 GMT  
		Size: 1.7 KB (1733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a4a4f0063093cdc07df60de1a6d30e856a4ed528faac41e365607eb44758cec`  
		Last Modified: Tue, 02 Aug 2022 15:00:25 GMT  
		Size: 1.0 KB (1049 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33ba4d77b594746542f2e71dd52678ddd883c436d88b72e2465c4eb7e01809da`  
		Last Modified: Tue, 02 Aug 2022 15:00:26 GMT  
		Size: 6.0 MB (5967261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71bba1d841b515de61167758f804ee176e5ae08c5d1171a8fda3781007b78158`  
		Last Modified: Tue, 02 Aug 2022 15:00:25 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:634b21022fb2ad7cfda5a174c30da9483511cea6cc668b1c7b925613d777cfb2`  
		Last Modified: Tue, 02 Aug 2022 15:00:25 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; arm variant v5

```console
$ docker pull spiped@sha256:6af880d390673b3da576db810a3f341c7e097879fd5b825384cf454c94209ca3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.9 MB (33936434 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1c3ede774f72c0efbe443d6545abe99b06d36efbdac21a941da05cf12db4dd78`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 02 Aug 2022 00:49:10 GMT
ADD file:4cd2f95737fd3007912428eeac56036c9e67e989e66cec08a8be99da47f88494 in / 
# Tue, 02 Aug 2022 00:49:10 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 19:51:33 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 02 Aug 2022 19:51:40 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 19:51:40 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 02 Aug 2022 19:52:11 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 02 Aug 2022 19:52:11 GMT
VOLUME [/spiped]
# Tue, 02 Aug 2022 19:52:11 GMT
WORKDIR /spiped
# Tue, 02 Aug 2022 19:52:12 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 02 Aug 2022 19:52:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 02 Aug 2022 19:52:12 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:5890b0ca6af5e8467a488e68716691950496a8f247d0495c2d595ddcb1893aff`  
		Last Modified: Tue, 02 Aug 2022 00:56:06 GMT  
		Size: 28.9 MB (28905515 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5914210ab5e9d450cc5cc817ba9a969a99a1bba9caff02b44bcf07b6daa99101`  
		Last Modified: Tue, 02 Aug 2022 19:52:38 GMT  
		Size: 1.7 KB (1726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:591059447642cb76dea322da399255cce3dfc35a2ab27142398a6c0b76c7db1a`  
		Last Modified: Tue, 02 Aug 2022 19:52:38 GMT  
		Size: 1.1 KB (1053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b596d1e863582490afb5019016264b3b75d44f08716d556cd395a4286210a5d`  
		Last Modified: Tue, 02 Aug 2022 19:52:41 GMT  
		Size: 5.0 MB (5027669 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:786bcf276f826fa83f9eef22ee3dd243c1b03582f76dcf0d838c8036997e795e`  
		Last Modified: Tue, 02 Aug 2022 19:52:38 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17e2aa3589894439340437bb0befccb5068c4051e6cc7b57e53f7e764bf4beb0`  
		Last Modified: Tue, 02 Aug 2022 19:52:39 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; arm variant v7

```console
$ docker pull spiped@sha256:05546f55c08afb1515cfc5708756ed4940307346ba553f0f975bf31140ab7573
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.3 MB (31311995 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fe18f0b13d76c9fe4af1797ce9d740ef87d42b1ce2094b53680be65b310394ed`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 02 Aug 2022 00:58:59 GMT
ADD file:1575b776a15adacebc0875642e97a80807d42dcfc8917e1406d47af7ac244c97 in / 
# Tue, 02 Aug 2022 00:58:59 GMT
CMD ["bash"]
# Wed, 03 Aug 2022 21:56:42 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 03 Aug 2022 21:56:45 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 03 Aug 2022 21:56:45 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 03 Aug 2022 21:57:01 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 03 Aug 2022 21:57:01 GMT
VOLUME [/spiped]
# Wed, 03 Aug 2022 21:57:01 GMT
WORKDIR /spiped
# Wed, 03 Aug 2022 21:57:01 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 03 Aug 2022 21:57:01 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 03 Aug 2022 21:57:01 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:1dd75a3a9c893a7dc313f683dd62464b7eab6c6d522ee62c8a17022631830f32`  
		Last Modified: Tue, 02 Aug 2022 01:06:45 GMT  
		Size: 26.6 MB (26560586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bcaffbe5be1966b473b328a91c40df9286228c74466eea7154a543527b6fae1`  
		Last Modified: Wed, 03 Aug 2022 21:57:45 GMT  
		Size: 1.7 KB (1726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2917d25466b0b307ff25a0fc7718a5e32785e7eef826f642b28d0439be6adc9e`  
		Last Modified: Wed, 03 Aug 2022 21:57:45 GMT  
		Size: 1.1 KB (1053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7caa787abd6178478de179d6cc5db9a07a792b29b34b9fc9486347a7c1b017f`  
		Last Modified: Wed, 03 Aug 2022 21:57:46 GMT  
		Size: 4.7 MB (4748161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3801153d36fffb70fcfc49890ef5d327bfc8b15f3a1cc6fa4d0d9b12eb27ff9`  
		Last Modified: Wed, 03 Aug 2022 21:57:45 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a742fab32925896cf7cffe6ca60ee420e328f9391fe5bcfc9f1f46e7f631ce3a`  
		Last Modified: Wed, 03 Aug 2022 21:57:45 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:4835debf7fbae32c4cc4cdc11e8792dc97767b8916ed69b695839b47ce2c5b49
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.3 MB (35328219 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:11bb3a1dd6e7229d9d7d203d5f015250cd44ab7d412ae6d00adbe3817b938ceb`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 02 Aug 2022 00:40:38 GMT
ADD file:6039adfbca55ed34a719c37672c664e3524130a0e2a3b8663629b8120b81b790 in / 
# Tue, 02 Aug 2022 00:40:39 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 16:47:23 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 02 Aug 2022 16:47:26 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 16:47:27 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 02 Aug 2022 16:47:45 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 02 Aug 2022 16:47:45 GMT
VOLUME [/spiped]
# Tue, 02 Aug 2022 16:47:46 GMT
WORKDIR /spiped
# Tue, 02 Aug 2022 16:47:48 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 02 Aug 2022 16:47:48 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 02 Aug 2022 16:47:49 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:a9fe95647e78b5516c7e2327355b6996e2ea295cd76ae242cbfe87f016b4e760`  
		Last Modified: Tue, 02 Aug 2022 00:46:05 GMT  
		Size: 30.1 MB (30054304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0215749fa5edad97431836093e99ce69829b4a2b18c351fe7e22c9bf90cb3fef`  
		Last Modified: Tue, 02 Aug 2022 16:48:17 GMT  
		Size: 1.6 KB (1617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6a61c46ac9b56671e11f61590184265582230b634537e091aa7515746a2ba70`  
		Last Modified: Tue, 02 Aug 2022 16:48:17 GMT  
		Size: 923.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:569abb15b59f2ea4b1fe7a95bda8247ac40c93685ac62b8029db8474d42f79cb`  
		Last Modified: Tue, 02 Aug 2022 16:48:18 GMT  
		Size: 5.3 MB (5270939 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:251fbe05e0ceba0f0f43f71ba704ee1b264165c62e3d7f999b3c597690886a75`  
		Last Modified: Tue, 02 Aug 2022 16:48:17 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10996acb338f32bf51751686febf31fd3fab4b1d46b4b8d7a7d5dfc7f05b4cee`  
		Last Modified: Tue, 02 Aug 2022 16:48:17 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; 386

```console
$ docker pull spiped@sha256:7a7dbde9446433fedc12b55ed6d0d73bbbf800753f0b4fc8c677bfd9f5d6f1fd
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.3 MB (40268619 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8544e7c71f7ba6f5ac7741eec3a5f49bd5d384c7d708d24631e0ce7e8af09460`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 02 Aug 2022 00:39:20 GMT
ADD file:f771e2286465694126158821089d801c7296376be2a56189e6041a15d2fe79f5 in / 
# Tue, 02 Aug 2022 00:39:21 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 15:45:02 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 02 Aug 2022 15:45:06 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 15:45:07 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 02 Aug 2022 15:45:28 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 02 Aug 2022 15:45:28 GMT
VOLUME [/spiped]
# Tue, 02 Aug 2022 15:45:29 GMT
WORKDIR /spiped
# Tue, 02 Aug 2022 15:45:31 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 02 Aug 2022 15:45:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 02 Aug 2022 15:45:32 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:90eb7f0ce9f33cf5dcd67d54c2fa606186dbaa5f95b6046f36145097267f9e53`  
		Last Modified: Tue, 02 Aug 2022 00:45:14 GMT  
		Size: 32.4 MB (32374054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:746b1fc4bab3964ac48dbe2fb0761a50ec33f467093556cf01fd8444415d8d11`  
		Last Modified: Tue, 02 Aug 2022 15:46:02 GMT  
		Size: 1.6 KB (1606 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2441fccbf951fe6e18f386cdd0c3cabaa845fde7d0bf966cf03f04f756510e6a`  
		Last Modified: Tue, 02 Aug 2022 15:46:02 GMT  
		Size: 924.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:231b6d32c27ff4a17c9587d6b1f9b787bb6d78e3d656a8c9467df93a850bd66f`  
		Last Modified: Tue, 02 Aug 2022 15:46:03 GMT  
		Size: 7.9 MB (7891596 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:072a58cf67fb04afdb3086a5a441fa938a2ede9871a6088da9f6bfd36cc65467`  
		Last Modified: Tue, 02 Aug 2022 15:46:02 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cac32ec13523eeeefcd7dcfb5c9f5cbd39875a916b3fa22df5b9af8f12e83aba`  
		Last Modified: Tue, 02 Aug 2022 15:46:02 GMT  
		Size: 344.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; mips64le

```console
$ docker pull spiped@sha256:9e5c7480cebb7266cbc6cd8cde915e916cea44f839c3d45827ee4b32b9d1f361
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.3 MB (35337243 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6d937f2142b4729449865145c0bd382f2880465d957aac461a860e13e82a8527`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 02 Aug 2022 01:10:34 GMT
ADD file:6dc22a1e5b5fcf23f2549406ddcc45c4e244f46e21eafa881de81fa87438e5d8 in / 
# Tue, 02 Aug 2022 01:10:38 GMT
CMD ["bash"]
# Thu, 04 Aug 2022 02:58:17 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Thu, 04 Aug 2022 02:58:32 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Thu, 04 Aug 2022 02:58:34 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 04 Aug 2022 03:00:04 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 04 Aug 2022 03:00:07 GMT
VOLUME [/spiped]
# Thu, 04 Aug 2022 03:00:09 GMT
WORKDIR /spiped
# Thu, 04 Aug 2022 03:00:12 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 04 Aug 2022 03:00:14 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 04 Aug 2022 03:00:17 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:88350749a27614c791450c256b051f023d81cdd256211274b1efac493779d2be`  
		Last Modified: Tue, 02 Aug 2022 01:21:02 GMT  
		Size: 29.6 MB (29628964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a980b8d4c4081e06e63d932cacd2a2bcb9ae4455ec1d8a0edfd5e7b976a41cfe`  
		Last Modified: Thu, 04 Aug 2022 03:00:33 GMT  
		Size: 1.6 KB (1619 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e926997286379c4294d14e53409efda33e6b135fe7e1090595de1c642b53a3b2`  
		Last Modified: Thu, 04 Aug 2022 03:00:34 GMT  
		Size: 923.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28c8df0b5ceb34f25514a9e6cfc3c5e4d4fa32daaa3e805d0e78bade747962e7`  
		Last Modified: Thu, 04 Aug 2022 03:00:38 GMT  
		Size: 5.7 MB (5705299 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe20d03337baf8ea0077260b2c5f5754fca122b1397f8ac922fb9db8dff5995b`  
		Last Modified: Thu, 04 Aug 2022 03:00:33 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca8d9c536c2096001a16837bafc47410185a740c029f1aad11b395642de38f34`  
		Last Modified: Thu, 04 Aug 2022 03:00:33 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; ppc64le

```console
$ docker pull spiped@sha256:27f881ff0e1f5e61d9dc98bfdaf60bde63f0b7c46ea39da2ac2c9814dcde8dd6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.3 MB (41274919 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9792967c333043140e04ed3704d0407abc333122050747da7546fc815c45542e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 02 Aug 2022 01:17:30 GMT
ADD file:3a95a896d463569ce82199957052b3467123a4bd3385a0a4e397cf08402a99c3 in / 
# Tue, 02 Aug 2022 01:17:32 GMT
CMD ["bash"]
# Wed, 03 Aug 2022 01:28:12 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 03 Aug 2022 01:28:18 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 03 Aug 2022 01:28:18 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 03 Aug 2022 01:28:56 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 03 Aug 2022 01:28:57 GMT
VOLUME [/spiped]
# Wed, 03 Aug 2022 01:28:57 GMT
WORKDIR /spiped
# Wed, 03 Aug 2022 01:28:58 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 03 Aug 2022 01:28:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 03 Aug 2022 01:28:59 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:5241cd116d6e6e2d62f3d8c2245b74daca9f6cc154eaccd738feb41984c74714`  
		Last Modified: Tue, 02 Aug 2022 01:24:39 GMT  
		Size: 35.3 MB (35272771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52f7bfa7322f80f7fbf327da4c4244442a6121cd2aa6a0c35b98493dff99cd50`  
		Last Modified: Wed, 03 Aug 2022 01:29:58 GMT  
		Size: 1.7 KB (1731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4737eb981cc3c529f234636741599c9b27a9f5b4973f8f9b6a7628649aab6726`  
		Last Modified: Wed, 03 Aug 2022 01:29:58 GMT  
		Size: 1.1 KB (1051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69e43d769614f6318ed658c891a70ce2668635f025c326b0b52a83b54ca1498b`  
		Last Modified: Wed, 03 Aug 2022 01:30:00 GMT  
		Size: 6.0 MB (5998895 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e492fc4ffd0f67e0a0b76b694e326dce271e5ad1bbf157bfb0c9097c0c7df653`  
		Last Modified: Wed, 03 Aug 2022 01:29:58 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2606cce249be48bbc9ec4f0d08c2920e38e1b3a0735446d0a03dd275279ca1cb`  
		Last Modified: Wed, 03 Aug 2022 01:29:58 GMT  
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
$ docker pull spiped@sha256:acddecb1628480a3371f5c7990076e0d894c6a9a2e7612d844e800178fabe8ba
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
$ docker pull spiped@sha256:66b3d848f73df6532c49bb456c441a37691db14797c1288fa9cd5deb9cf9bdb6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (3036703 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ebcb8fdfbde39b2b89abb4cdfac48560f245fff78fc822e3daac086fd5b29f78`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 09 Aug 2022 17:19:53 GMT
ADD file:2a949686d9886ac7c10582a6c29116fd29d3077d02755e87e111870d63607725 in / 
# Tue, 09 Aug 2022 17:19:53 GMT
CMD ["/bin/sh"]
# Wed, 10 Aug 2022 02:25:05 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Wed, 10 Aug 2022 02:25:06 GMT
RUN apk add --no-cache libssl1.1
# Wed, 10 Aug 2022 02:25:06 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 10 Aug 2022 02:25:16 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Wed, 10 Aug 2022 02:25:17 GMT
VOLUME [/spiped]
# Wed, 10 Aug 2022 02:25:17 GMT
WORKDIR /spiped
# Wed, 10 Aug 2022 02:25:17 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 10 Aug 2022 02:25:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 10 Aug 2022 02:25:17 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:213ec9aee27d8be045c6a92b7eac22c9a64b44558193775a1a7f626352392b49`  
		Last Modified: Tue, 09 Aug 2022 14:25:13 GMT  
		Size: 2.8 MB (2806054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:210040c27162008830a83da8ed96f452757ffa50050398230f525b2f22a4541a`  
		Last Modified: Wed, 10 Aug 2022 02:25:34 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b05b54e70388210c7ffd8a9fbb864ca9f878f8ad3dc1613e4b96b107919baadc`  
		Last Modified: Wed, 10 Aug 2022 02:25:34 GMT  
		Size: 7.7 KB (7735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28b8ff19a9777e30476c0a48eab4bc4817e9a96226faf7b42870225d69a37ba8`  
		Last Modified: Wed, 10 Aug 2022 02:25:34 GMT  
		Size: 221.2 KB (221175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:700f71a1b577cfb700f72058dad655d1ec9161da01b7fe6e8bb2b2461d1ddbbe`  
		Last Modified: Wed, 10 Aug 2022 02:25:34 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6c2f8d0b8416d1c553517142cd373249cbbdc3a03229d96604cd32b318a1195`  
		Last Modified: Wed, 10 Aug 2022 02:25:34 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; arm variant v6

```console
$ docker pull spiped@sha256:9bf39d60020a139fa461ebb060df6df01d5164425285c6bfc1b3113ef2242277
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 MB (2829328 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:88197140375c26dcc5aa5dad079e8343608e24c8a03e91eb5d2fb13c9e09deec`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 09 Aug 2022 17:49:22 GMT
ADD file:e8733e8cc0a81e15ca4041760b6e27392c34171512d34405a9b262b1fff5c687 in / 
# Tue, 09 Aug 2022 17:49:22 GMT
CMD ["/bin/sh"]
# Thu, 11 Aug 2022 00:37:38 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 11 Aug 2022 00:37:39 GMT
RUN apk add --no-cache libssl1.1
# Thu, 11 Aug 2022 00:37:39 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 11 Aug 2022 00:37:47 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Thu, 11 Aug 2022 00:37:47 GMT
VOLUME [/spiped]
# Thu, 11 Aug 2022 00:37:47 GMT
WORKDIR /spiped
# Thu, 11 Aug 2022 00:37:47 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 11 Aug 2022 00:37:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 11 Aug 2022 00:37:47 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:9506b835437abb4d8ba1683e00c500b8f77e1975e930b356fbb72f2dbdc274d9`  
		Last Modified: Tue, 09 Aug 2022 17:50:33 GMT  
		Size: 2.6 MB (2613965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3f8a3e1b897eaae3127b4c0c6bf167dc3d7740bbf9596a97a994f1249716538`  
		Last Modified: Thu, 11 Aug 2022 00:38:06 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fa63959f901bfbea0a7da0112a6c04fe32edaaf453bc28bc784d942ef8a1c01`  
		Last Modified: Thu, 11 Aug 2022 00:38:06 GMT  
		Size: 7.7 KB (7736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb53413b98987994a206c07b7c3ba39980d1dd0149f4a1be509beab0c15b75da`  
		Last Modified: Thu, 11 Aug 2022 00:38:06 GMT  
		Size: 205.9 KB (205888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe12872e965332f5c42d1844aa3dfdbae46eda912838801110e130b89cc181ca`  
		Last Modified: Thu, 11 Aug 2022 00:38:06 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a33b8651215087c0b9c9d0edc3a3fb9e0d18f0eaf36a0c0bfcddce94e338d57`  
		Last Modified: Thu, 11 Aug 2022 00:38:06 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; arm variant v7

```console
$ docker pull spiped@sha256:0e746939643dcaba40d0c1f15f4d142129555ff4d3a187e755c3643cb387bca1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 MB (2621321 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:af5a28036aaca6f3accc02f7ab66d26c0d7ef2c544316b0df54081730f89391e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Mon, 18 Jul 2022 21:24:47 GMT
ADD file:68590e866bc6db27ad54d23de7dd275d0389cb86e4e6291a1243fcc234f2f7a1 in / 
# Mon, 18 Jul 2022 21:24:47 GMT
CMD ["/bin/sh"]
# Wed, 03 Aug 2022 21:57:08 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Wed, 03 Aug 2022 21:57:09 GMT
RUN apk add --no-cache libssl1.1
# Wed, 03 Aug 2022 21:57:09 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 03 Aug 2022 21:57:16 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Wed, 03 Aug 2022 21:57:17 GMT
VOLUME [/spiped]
# Wed, 03 Aug 2022 21:57:17 GMT
WORKDIR /spiped
# Wed, 03 Aug 2022 21:57:17 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 03 Aug 2022 21:57:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 03 Aug 2022 21:57:17 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:a6b45ace95f42a930d15c33679ab9c85d46019b7e73954cadc73bb9ba176509b`  
		Last Modified: Mon, 18 Jul 2022 19:08:56 GMT  
		Size: 2.4 MB (2412307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a223ea05945b5c5ea98e31d53b7924f548e24abe646453181a3b73f940a52de`  
		Last Modified: Wed, 03 Aug 2022 21:58:06 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:868bbc51d36bab84123a304360d9b4bc7db9f0714c2281b34b7585ff494ab1c8`  
		Last Modified: Wed, 03 Aug 2022 21:58:06 GMT  
		Size: 7.7 KB (7730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18353dabcadb1dc2dc0b669eeff1d9dd8d42a815bd9f860e8ff08c8f2191131f`  
		Last Modified: Wed, 03 Aug 2022 21:58:06 GMT  
		Size: 199.5 KB (199542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:330712fbce762a1e0c7e7bcf9c36a39c454fa780a6901be6761dd588dc043f5f`  
		Last Modified: Wed, 03 Aug 2022 21:58:06 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:221966fcc255ad5deb2fa5ce1fc0b504eff307dc6e7aaebe7db90698290052eb`  
		Last Modified: Wed, 03 Aug 2022 21:58:06 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:31d9f2978a4900b825028e1c399cd7d0638f75f91f2400f6c6bc1d83d6274fb6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 MB (2931313 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:031699f5a5efac86682c564a2c655c7eab52ce5aa91a856923d2032ea0517c52`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 09 Aug 2022 17:39:41 GMT
ADD file:960fd469d48cf79ba14bbda71f3192074ed860c112e30e0bc92bff3440cb45ab in / 
# Tue, 09 Aug 2022 17:39:42 GMT
CMD ["/bin/sh"]
# Wed, 10 Aug 2022 06:09:41 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Wed, 10 Aug 2022 06:09:42 GMT
RUN apk add --no-cache libssl1.1
# Wed, 10 Aug 2022 06:09:43 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 10 Aug 2022 06:09:54 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Wed, 10 Aug 2022 06:09:55 GMT
VOLUME [/spiped]
# Wed, 10 Aug 2022 06:09:56 GMT
WORKDIR /spiped
# Wed, 10 Aug 2022 06:09:58 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 10 Aug 2022 06:09:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 10 Aug 2022 06:09:59 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:9b18e9b68314027565b90ff6189d65942c0f7986da80df008b8431276885218e`  
		Last Modified: Tue, 09 Aug 2022 17:40:38 GMT  
		Size: 2.7 MB (2707663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bf9d3ec407b6270ec79bb3c0552c48d0afd7888773c72f1b25bfc396d4c3eb7`  
		Last Modified: Wed, 10 Aug 2022 06:10:25 GMT  
		Size: 1.2 KB (1244 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99f1183a0c8143435d389abc100d22d7289e4a81f966ca3b9d8301cfb01947b2`  
		Last Modified: Wed, 10 Aug 2022 06:10:25 GMT  
		Size: 7.7 KB (7710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8abc3813fe4a6ffebb8bdde4bd9005230c2935072094662e52a3a81cc9a9c3fa`  
		Last Modified: Wed, 10 Aug 2022 06:10:26 GMT  
		Size: 214.3 KB (214262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab3f496ad70b8f2f8ea93c54500ad75fb9fa4b72d7868ae964cce858765988a4`  
		Last Modified: Wed, 10 Aug 2022 06:10:26 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46086b9ffd0c9eed5aadecf28229d0ab4532a26add5be2f474ced21cf4f25f7e`  
		Last Modified: Wed, 10 Aug 2022 06:10:25 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; 386

```console
$ docker pull spiped@sha256:ee4833bbef16308d250de2dac9ad7a6019a6f2e42880ed8eb3dfd4fcecc4ced4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (3047835 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:75c145e337e061db2f783bf06d6d6b2f1e63cf3e7dedb8ada91bc1744b707620`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 09 Aug 2022 17:38:39 GMT
ADD file:b828bc14bc5ff03c8f7310fe0aed6ac5df19a393622d5d1d779a523234d07c0a in / 
# Tue, 09 Aug 2022 17:38:39 GMT
CMD ["/bin/sh"]
# Wed, 10 Aug 2022 00:02:16 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Wed, 10 Aug 2022 00:02:18 GMT
RUN apk add --no-cache libssl1.1
# Wed, 10 Aug 2022 00:02:19 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 10 Aug 2022 00:02:30 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Wed, 10 Aug 2022 00:02:31 GMT
VOLUME [/spiped]
# Wed, 10 Aug 2022 00:02:32 GMT
WORKDIR /spiped
# Wed, 10 Aug 2022 00:02:34 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 10 Aug 2022 00:02:34 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 10 Aug 2022 00:02:35 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:6c0d3b419d848ea31ca748254611d5d5ce3b76e3d7bba520fd87400fbb75f3b9`  
		Last Modified: Tue, 09 Aug 2022 17:39:33 GMT  
		Size: 2.8 MB (2807121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:072149e09853327c1921fc351fbf7a93e1056edfefc5daa66cbdc6e48843cd13`  
		Last Modified: Wed, 10 Aug 2022 00:03:04 GMT  
		Size: 1.2 KB (1243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34965b4906426a2b44e36dc3fd455d5da36569c3a0c3de199beecfc03c85244c`  
		Last Modified: Wed, 10 Aug 2022 00:03:04 GMT  
		Size: 7.7 KB (7710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ddeae6e8a846e3df57fb016e864191c85342272b8c766aea5b9cd0e001b0332`  
		Last Modified: Wed, 10 Aug 2022 00:03:05 GMT  
		Size: 231.3 KB (231325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:463f4e96eadc8d28add083b4c188fcdde9cecb3831b8c5427343441c383e1136`  
		Last Modified: Wed, 10 Aug 2022 00:03:04 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3648573cf3f78bda63b9ea60198dd66926dda5cbd250025fbf6c5c0f08bbbcb4`  
		Last Modified: Wed, 10 Aug 2022 00:03:04 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; ppc64le

```console
$ docker pull spiped@sha256:d67f02f9e68884fbd145362c4f490cdfb403437bcf89d1135ad1a15c92052a5a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (3033050 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:14fd901b20c0f04f13ac388776797050b3e6a48903ceeccca414c16f53e1c29f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 09 Aug 2022 17:17:09 GMT
ADD file:66b351666e41834033d334aeb3dc6998dea77aa22e8e254028c923fee67a41a8 in / 
# Tue, 09 Aug 2022 17:17:10 GMT
CMD ["/bin/sh"]
# Wed, 10 Aug 2022 02:55:17 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Wed, 10 Aug 2022 02:55:19 GMT
RUN apk add --no-cache libssl1.1
# Wed, 10 Aug 2022 02:55:19 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 10 Aug 2022 02:55:34 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Wed, 10 Aug 2022 02:55:34 GMT
VOLUME [/spiped]
# Wed, 10 Aug 2022 02:55:35 GMT
WORKDIR /spiped
# Wed, 10 Aug 2022 02:55:36 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 10 Aug 2022 02:55:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 10 Aug 2022 02:55:36 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:c79e5d1a8c89b87020a754c8a5c8370faaa37bfb5bca1d8af66770d522ef1caf`  
		Last Modified: Tue, 09 Aug 2022 17:18:26 GMT  
		Size: 2.8 MB (2803320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cd8832ea95a37bc42923d861cfefd27ec973fed3564060fce137b8d54f75e02`  
		Last Modified: Wed, 10 Aug 2022 02:56:11 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ab0760cebdd26f5d818b164fe30701e72c6ec6c6c6b97b100ed16bc24fcf653`  
		Last Modified: Wed, 10 Aug 2022 02:56:11 GMT  
		Size: 7.7 KB (7739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8cdb874eec093d50ac091467e93cb88955a1ee87db0d0dd84cc6344ad829323`  
		Last Modified: Wed, 10 Aug 2022 02:56:11 GMT  
		Size: 220.3 KB (220255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a349e85c23948cd849a1a373c684ee566e0544af2297f9904d664dbb41dc8a6`  
		Last Modified: Wed, 10 Aug 2022 02:56:22 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bd274005021e79dbc526fb1fd7ad0d420d2e5c10abf68e3c7ae46021ae45cbf`  
		Last Modified: Wed, 10 Aug 2022 02:56:11 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; s390x

```console
$ docker pull spiped@sha256:936312a4e0595fc377ed5e910f12d52cfc4fae63a6190fe388481f204758a480
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 MB (2808502 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:afa6705ab1cc71e7aa223e1b9c9ba81f85eacacdba00737aa34a7014d8d94163`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 09 Aug 2022 17:41:46 GMT
ADD file:b43a065471bc4711415d3c67cd5b6559b0c48ee7ffe9761530477cf457a6dc34 in / 
# Tue, 09 Aug 2022 17:41:46 GMT
CMD ["/bin/sh"]
# Wed, 10 Aug 2022 05:46:33 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Wed, 10 Aug 2022 05:46:34 GMT
RUN apk add --no-cache libssl1.1
# Wed, 10 Aug 2022 05:46:34 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 10 Aug 2022 05:46:39 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Wed, 10 Aug 2022 05:46:39 GMT
VOLUME [/spiped]
# Wed, 10 Aug 2022 05:46:39 GMT
WORKDIR /spiped
# Wed, 10 Aug 2022 05:46:39 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 10 Aug 2022 05:46:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 10 Aug 2022 05:46:40 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:790c84f1f3409eab952345157df7fa804ba6b5f06d4ceb6f2dfa3c6de2064397`  
		Last Modified: Tue, 09 Aug 2022 17:42:45 GMT  
		Size: 2.6 MB (2590597 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e997054cff6af24fce535516fc4358eabc7dace5f52f427e6a19340c04f6adfe`  
		Last Modified: Wed, 10 Aug 2022 05:47:31 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b78da263b8c9f381935ae64289597db6f2e0d7e77fa388ce819ba7afecd17ef1`  
		Last Modified: Wed, 10 Aug 2022 05:47:35 GMT  
		Size: 7.7 KB (7742 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1acce323c9898120275bb4b4763b7a8971f71720bf7cafb55201dc313247560c`  
		Last Modified: Wed, 10 Aug 2022 05:47:35 GMT  
		Size: 208.4 KB (208429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98b550d52792a92d7c50d7e5102763598d59d41f0c34d5bd928fbd55e16de8f8`  
		Last Modified: Wed, 10 Aug 2022 05:47:35 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:130443af95b4efa2ff2d4d039066967531a4e10357d515888d55082f26340a52`  
		Last Modified: Wed, 10 Aug 2022 05:47:35 GMT  
		Size: 336.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:1.6.2`

```console
$ docker pull spiped@sha256:6442d9ca640a1475fe7f8827406c94ab677a48776e9653472bd6523a120609dc
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
$ docker pull spiped@sha256:dad19d6d4fd551afedb73402fbe587665af498a94aab95d1f1c65b6fca26b254
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.3 MB (37337269 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ad8d035bd9a75027ee1fd4c3aa1157c358bb1ffceba1d2ae6cee8caa104b286a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 02 Aug 2022 01:20:04 GMT
ADD file:0eae0dca665c7044bf242cb1fc92cb8ea744f5af2dd376a558c90bc47349aefe in / 
# Tue, 02 Aug 2022 01:20:05 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 14:59:44 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 02 Aug 2022 14:59:47 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 14:59:47 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 02 Aug 2022 15:00:07 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 02 Aug 2022 15:00:08 GMT
VOLUME [/spiped]
# Tue, 02 Aug 2022 15:00:08 GMT
WORKDIR /spiped
# Tue, 02 Aug 2022 15:00:08 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 02 Aug 2022 15:00:08 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 02 Aug 2022 15:00:08 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:1efc276f4ff952c055dea726cfc96ec6a4fdb8b62d9eed816bd2b788f2860ad7`  
		Last Modified: Tue, 02 Aug 2022 01:24:13 GMT  
		Size: 31.4 MB (31366757 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71902ff87bbf89a7cab2e1efdfe743d124a3eb6896b31675c52ab90dd16095e9`  
		Last Modified: Tue, 02 Aug 2022 15:00:25 GMT  
		Size: 1.7 KB (1733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a4a4f0063093cdc07df60de1a6d30e856a4ed528faac41e365607eb44758cec`  
		Last Modified: Tue, 02 Aug 2022 15:00:25 GMT  
		Size: 1.0 KB (1049 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33ba4d77b594746542f2e71dd52678ddd883c436d88b72e2465c4eb7e01809da`  
		Last Modified: Tue, 02 Aug 2022 15:00:26 GMT  
		Size: 6.0 MB (5967261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71bba1d841b515de61167758f804ee176e5ae08c5d1171a8fda3781007b78158`  
		Last Modified: Tue, 02 Aug 2022 15:00:25 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:634b21022fb2ad7cfda5a174c30da9483511cea6cc668b1c7b925613d777cfb2`  
		Last Modified: Tue, 02 Aug 2022 15:00:25 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.2` - linux; arm variant v5

```console
$ docker pull spiped@sha256:6af880d390673b3da576db810a3f341c7e097879fd5b825384cf454c94209ca3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.9 MB (33936434 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1c3ede774f72c0efbe443d6545abe99b06d36efbdac21a941da05cf12db4dd78`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 02 Aug 2022 00:49:10 GMT
ADD file:4cd2f95737fd3007912428eeac56036c9e67e989e66cec08a8be99da47f88494 in / 
# Tue, 02 Aug 2022 00:49:10 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 19:51:33 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 02 Aug 2022 19:51:40 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 19:51:40 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 02 Aug 2022 19:52:11 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 02 Aug 2022 19:52:11 GMT
VOLUME [/spiped]
# Tue, 02 Aug 2022 19:52:11 GMT
WORKDIR /spiped
# Tue, 02 Aug 2022 19:52:12 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 02 Aug 2022 19:52:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 02 Aug 2022 19:52:12 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:5890b0ca6af5e8467a488e68716691950496a8f247d0495c2d595ddcb1893aff`  
		Last Modified: Tue, 02 Aug 2022 00:56:06 GMT  
		Size: 28.9 MB (28905515 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5914210ab5e9d450cc5cc817ba9a969a99a1bba9caff02b44bcf07b6daa99101`  
		Last Modified: Tue, 02 Aug 2022 19:52:38 GMT  
		Size: 1.7 KB (1726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:591059447642cb76dea322da399255cce3dfc35a2ab27142398a6c0b76c7db1a`  
		Last Modified: Tue, 02 Aug 2022 19:52:38 GMT  
		Size: 1.1 KB (1053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b596d1e863582490afb5019016264b3b75d44f08716d556cd395a4286210a5d`  
		Last Modified: Tue, 02 Aug 2022 19:52:41 GMT  
		Size: 5.0 MB (5027669 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:786bcf276f826fa83f9eef22ee3dd243c1b03582f76dcf0d838c8036997e795e`  
		Last Modified: Tue, 02 Aug 2022 19:52:38 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17e2aa3589894439340437bb0befccb5068c4051e6cc7b57e53f7e764bf4beb0`  
		Last Modified: Tue, 02 Aug 2022 19:52:39 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.2` - linux; arm variant v7

```console
$ docker pull spiped@sha256:05546f55c08afb1515cfc5708756ed4940307346ba553f0f975bf31140ab7573
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.3 MB (31311995 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fe18f0b13d76c9fe4af1797ce9d740ef87d42b1ce2094b53680be65b310394ed`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 02 Aug 2022 00:58:59 GMT
ADD file:1575b776a15adacebc0875642e97a80807d42dcfc8917e1406d47af7ac244c97 in / 
# Tue, 02 Aug 2022 00:58:59 GMT
CMD ["bash"]
# Wed, 03 Aug 2022 21:56:42 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 03 Aug 2022 21:56:45 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 03 Aug 2022 21:56:45 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 03 Aug 2022 21:57:01 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 03 Aug 2022 21:57:01 GMT
VOLUME [/spiped]
# Wed, 03 Aug 2022 21:57:01 GMT
WORKDIR /spiped
# Wed, 03 Aug 2022 21:57:01 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 03 Aug 2022 21:57:01 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 03 Aug 2022 21:57:01 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:1dd75a3a9c893a7dc313f683dd62464b7eab6c6d522ee62c8a17022631830f32`  
		Last Modified: Tue, 02 Aug 2022 01:06:45 GMT  
		Size: 26.6 MB (26560586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bcaffbe5be1966b473b328a91c40df9286228c74466eea7154a543527b6fae1`  
		Last Modified: Wed, 03 Aug 2022 21:57:45 GMT  
		Size: 1.7 KB (1726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2917d25466b0b307ff25a0fc7718a5e32785e7eef826f642b28d0439be6adc9e`  
		Last Modified: Wed, 03 Aug 2022 21:57:45 GMT  
		Size: 1.1 KB (1053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7caa787abd6178478de179d6cc5db9a07a792b29b34b9fc9486347a7c1b017f`  
		Last Modified: Wed, 03 Aug 2022 21:57:46 GMT  
		Size: 4.7 MB (4748161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3801153d36fffb70fcfc49890ef5d327bfc8b15f3a1cc6fa4d0d9b12eb27ff9`  
		Last Modified: Wed, 03 Aug 2022 21:57:45 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a742fab32925896cf7cffe6ca60ee420e328f9391fe5bcfc9f1f46e7f631ce3a`  
		Last Modified: Wed, 03 Aug 2022 21:57:45 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.2` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:4835debf7fbae32c4cc4cdc11e8792dc97767b8916ed69b695839b47ce2c5b49
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.3 MB (35328219 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:11bb3a1dd6e7229d9d7d203d5f015250cd44ab7d412ae6d00adbe3817b938ceb`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 02 Aug 2022 00:40:38 GMT
ADD file:6039adfbca55ed34a719c37672c664e3524130a0e2a3b8663629b8120b81b790 in / 
# Tue, 02 Aug 2022 00:40:39 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 16:47:23 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 02 Aug 2022 16:47:26 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 16:47:27 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 02 Aug 2022 16:47:45 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 02 Aug 2022 16:47:45 GMT
VOLUME [/spiped]
# Tue, 02 Aug 2022 16:47:46 GMT
WORKDIR /spiped
# Tue, 02 Aug 2022 16:47:48 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 02 Aug 2022 16:47:48 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 02 Aug 2022 16:47:49 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:a9fe95647e78b5516c7e2327355b6996e2ea295cd76ae242cbfe87f016b4e760`  
		Last Modified: Tue, 02 Aug 2022 00:46:05 GMT  
		Size: 30.1 MB (30054304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0215749fa5edad97431836093e99ce69829b4a2b18c351fe7e22c9bf90cb3fef`  
		Last Modified: Tue, 02 Aug 2022 16:48:17 GMT  
		Size: 1.6 KB (1617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6a61c46ac9b56671e11f61590184265582230b634537e091aa7515746a2ba70`  
		Last Modified: Tue, 02 Aug 2022 16:48:17 GMT  
		Size: 923.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:569abb15b59f2ea4b1fe7a95bda8247ac40c93685ac62b8029db8474d42f79cb`  
		Last Modified: Tue, 02 Aug 2022 16:48:18 GMT  
		Size: 5.3 MB (5270939 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:251fbe05e0ceba0f0f43f71ba704ee1b264165c62e3d7f999b3c597690886a75`  
		Last Modified: Tue, 02 Aug 2022 16:48:17 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10996acb338f32bf51751686febf31fd3fab4b1d46b4b8d7a7d5dfc7f05b4cee`  
		Last Modified: Tue, 02 Aug 2022 16:48:17 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.2` - linux; 386

```console
$ docker pull spiped@sha256:7a7dbde9446433fedc12b55ed6d0d73bbbf800753f0b4fc8c677bfd9f5d6f1fd
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.3 MB (40268619 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8544e7c71f7ba6f5ac7741eec3a5f49bd5d384c7d708d24631e0ce7e8af09460`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 02 Aug 2022 00:39:20 GMT
ADD file:f771e2286465694126158821089d801c7296376be2a56189e6041a15d2fe79f5 in / 
# Tue, 02 Aug 2022 00:39:21 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 15:45:02 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 02 Aug 2022 15:45:06 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 15:45:07 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 02 Aug 2022 15:45:28 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 02 Aug 2022 15:45:28 GMT
VOLUME [/spiped]
# Tue, 02 Aug 2022 15:45:29 GMT
WORKDIR /spiped
# Tue, 02 Aug 2022 15:45:31 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 02 Aug 2022 15:45:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 02 Aug 2022 15:45:32 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:90eb7f0ce9f33cf5dcd67d54c2fa606186dbaa5f95b6046f36145097267f9e53`  
		Last Modified: Tue, 02 Aug 2022 00:45:14 GMT  
		Size: 32.4 MB (32374054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:746b1fc4bab3964ac48dbe2fb0761a50ec33f467093556cf01fd8444415d8d11`  
		Last Modified: Tue, 02 Aug 2022 15:46:02 GMT  
		Size: 1.6 KB (1606 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2441fccbf951fe6e18f386cdd0c3cabaa845fde7d0bf966cf03f04f756510e6a`  
		Last Modified: Tue, 02 Aug 2022 15:46:02 GMT  
		Size: 924.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:231b6d32c27ff4a17c9587d6b1f9b787bb6d78e3d656a8c9467df93a850bd66f`  
		Last Modified: Tue, 02 Aug 2022 15:46:03 GMT  
		Size: 7.9 MB (7891596 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:072a58cf67fb04afdb3086a5a441fa938a2ede9871a6088da9f6bfd36cc65467`  
		Last Modified: Tue, 02 Aug 2022 15:46:02 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cac32ec13523eeeefcd7dcfb5c9f5cbd39875a916b3fa22df5b9af8f12e83aba`  
		Last Modified: Tue, 02 Aug 2022 15:46:02 GMT  
		Size: 344.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.2` - linux; mips64le

```console
$ docker pull spiped@sha256:9e5c7480cebb7266cbc6cd8cde915e916cea44f839c3d45827ee4b32b9d1f361
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.3 MB (35337243 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6d937f2142b4729449865145c0bd382f2880465d957aac461a860e13e82a8527`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 02 Aug 2022 01:10:34 GMT
ADD file:6dc22a1e5b5fcf23f2549406ddcc45c4e244f46e21eafa881de81fa87438e5d8 in / 
# Tue, 02 Aug 2022 01:10:38 GMT
CMD ["bash"]
# Thu, 04 Aug 2022 02:58:17 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Thu, 04 Aug 2022 02:58:32 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Thu, 04 Aug 2022 02:58:34 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 04 Aug 2022 03:00:04 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 04 Aug 2022 03:00:07 GMT
VOLUME [/spiped]
# Thu, 04 Aug 2022 03:00:09 GMT
WORKDIR /spiped
# Thu, 04 Aug 2022 03:00:12 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 04 Aug 2022 03:00:14 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 04 Aug 2022 03:00:17 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:88350749a27614c791450c256b051f023d81cdd256211274b1efac493779d2be`  
		Last Modified: Tue, 02 Aug 2022 01:21:02 GMT  
		Size: 29.6 MB (29628964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a980b8d4c4081e06e63d932cacd2a2bcb9ae4455ec1d8a0edfd5e7b976a41cfe`  
		Last Modified: Thu, 04 Aug 2022 03:00:33 GMT  
		Size: 1.6 KB (1619 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e926997286379c4294d14e53409efda33e6b135fe7e1090595de1c642b53a3b2`  
		Last Modified: Thu, 04 Aug 2022 03:00:34 GMT  
		Size: 923.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28c8df0b5ceb34f25514a9e6cfc3c5e4d4fa32daaa3e805d0e78bade747962e7`  
		Last Modified: Thu, 04 Aug 2022 03:00:38 GMT  
		Size: 5.7 MB (5705299 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe20d03337baf8ea0077260b2c5f5754fca122b1397f8ac922fb9db8dff5995b`  
		Last Modified: Thu, 04 Aug 2022 03:00:33 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca8d9c536c2096001a16837bafc47410185a740c029f1aad11b395642de38f34`  
		Last Modified: Thu, 04 Aug 2022 03:00:33 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.2` - linux; ppc64le

```console
$ docker pull spiped@sha256:27f881ff0e1f5e61d9dc98bfdaf60bde63f0b7c46ea39da2ac2c9814dcde8dd6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.3 MB (41274919 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9792967c333043140e04ed3704d0407abc333122050747da7546fc815c45542e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 02 Aug 2022 01:17:30 GMT
ADD file:3a95a896d463569ce82199957052b3467123a4bd3385a0a4e397cf08402a99c3 in / 
# Tue, 02 Aug 2022 01:17:32 GMT
CMD ["bash"]
# Wed, 03 Aug 2022 01:28:12 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 03 Aug 2022 01:28:18 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 03 Aug 2022 01:28:18 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 03 Aug 2022 01:28:56 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 03 Aug 2022 01:28:57 GMT
VOLUME [/spiped]
# Wed, 03 Aug 2022 01:28:57 GMT
WORKDIR /spiped
# Wed, 03 Aug 2022 01:28:58 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 03 Aug 2022 01:28:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 03 Aug 2022 01:28:59 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:5241cd116d6e6e2d62f3d8c2245b74daca9f6cc154eaccd738feb41984c74714`  
		Last Modified: Tue, 02 Aug 2022 01:24:39 GMT  
		Size: 35.3 MB (35272771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52f7bfa7322f80f7fbf327da4c4244442a6121cd2aa6a0c35b98493dff99cd50`  
		Last Modified: Wed, 03 Aug 2022 01:29:58 GMT  
		Size: 1.7 KB (1731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4737eb981cc3c529f234636741599c9b27a9f5b4973f8f9b6a7628649aab6726`  
		Last Modified: Wed, 03 Aug 2022 01:29:58 GMT  
		Size: 1.1 KB (1051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69e43d769614f6318ed658c891a70ce2668635f025c326b0b52a83b54ca1498b`  
		Last Modified: Wed, 03 Aug 2022 01:30:00 GMT  
		Size: 6.0 MB (5998895 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e492fc4ffd0f67e0a0b76b694e326dce271e5ad1bbf157bfb0c9097c0c7df653`  
		Last Modified: Wed, 03 Aug 2022 01:29:58 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2606cce249be48bbc9ec4f0d08c2920e38e1b3a0735446d0a03dd275279ca1cb`  
		Last Modified: Wed, 03 Aug 2022 01:29:58 GMT  
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
$ docker pull spiped@sha256:acddecb1628480a3371f5c7990076e0d894c6a9a2e7612d844e800178fabe8ba
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
$ docker pull spiped@sha256:66b3d848f73df6532c49bb456c441a37691db14797c1288fa9cd5deb9cf9bdb6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (3036703 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ebcb8fdfbde39b2b89abb4cdfac48560f245fff78fc822e3daac086fd5b29f78`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 09 Aug 2022 17:19:53 GMT
ADD file:2a949686d9886ac7c10582a6c29116fd29d3077d02755e87e111870d63607725 in / 
# Tue, 09 Aug 2022 17:19:53 GMT
CMD ["/bin/sh"]
# Wed, 10 Aug 2022 02:25:05 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Wed, 10 Aug 2022 02:25:06 GMT
RUN apk add --no-cache libssl1.1
# Wed, 10 Aug 2022 02:25:06 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 10 Aug 2022 02:25:16 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Wed, 10 Aug 2022 02:25:17 GMT
VOLUME [/spiped]
# Wed, 10 Aug 2022 02:25:17 GMT
WORKDIR /spiped
# Wed, 10 Aug 2022 02:25:17 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 10 Aug 2022 02:25:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 10 Aug 2022 02:25:17 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:213ec9aee27d8be045c6a92b7eac22c9a64b44558193775a1a7f626352392b49`  
		Last Modified: Tue, 09 Aug 2022 14:25:13 GMT  
		Size: 2.8 MB (2806054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:210040c27162008830a83da8ed96f452757ffa50050398230f525b2f22a4541a`  
		Last Modified: Wed, 10 Aug 2022 02:25:34 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b05b54e70388210c7ffd8a9fbb864ca9f878f8ad3dc1613e4b96b107919baadc`  
		Last Modified: Wed, 10 Aug 2022 02:25:34 GMT  
		Size: 7.7 KB (7735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28b8ff19a9777e30476c0a48eab4bc4817e9a96226faf7b42870225d69a37ba8`  
		Last Modified: Wed, 10 Aug 2022 02:25:34 GMT  
		Size: 221.2 KB (221175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:700f71a1b577cfb700f72058dad655d1ec9161da01b7fe6e8bb2b2461d1ddbbe`  
		Last Modified: Wed, 10 Aug 2022 02:25:34 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6c2f8d0b8416d1c553517142cd373249cbbdc3a03229d96604cd32b318a1195`  
		Last Modified: Wed, 10 Aug 2022 02:25:34 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.2-alpine` - linux; arm variant v6

```console
$ docker pull spiped@sha256:9bf39d60020a139fa461ebb060df6df01d5164425285c6bfc1b3113ef2242277
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 MB (2829328 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:88197140375c26dcc5aa5dad079e8343608e24c8a03e91eb5d2fb13c9e09deec`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 09 Aug 2022 17:49:22 GMT
ADD file:e8733e8cc0a81e15ca4041760b6e27392c34171512d34405a9b262b1fff5c687 in / 
# Tue, 09 Aug 2022 17:49:22 GMT
CMD ["/bin/sh"]
# Thu, 11 Aug 2022 00:37:38 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 11 Aug 2022 00:37:39 GMT
RUN apk add --no-cache libssl1.1
# Thu, 11 Aug 2022 00:37:39 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 11 Aug 2022 00:37:47 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Thu, 11 Aug 2022 00:37:47 GMT
VOLUME [/spiped]
# Thu, 11 Aug 2022 00:37:47 GMT
WORKDIR /spiped
# Thu, 11 Aug 2022 00:37:47 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 11 Aug 2022 00:37:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 11 Aug 2022 00:37:47 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:9506b835437abb4d8ba1683e00c500b8f77e1975e930b356fbb72f2dbdc274d9`  
		Last Modified: Tue, 09 Aug 2022 17:50:33 GMT  
		Size: 2.6 MB (2613965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3f8a3e1b897eaae3127b4c0c6bf167dc3d7740bbf9596a97a994f1249716538`  
		Last Modified: Thu, 11 Aug 2022 00:38:06 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fa63959f901bfbea0a7da0112a6c04fe32edaaf453bc28bc784d942ef8a1c01`  
		Last Modified: Thu, 11 Aug 2022 00:38:06 GMT  
		Size: 7.7 KB (7736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb53413b98987994a206c07b7c3ba39980d1dd0149f4a1be509beab0c15b75da`  
		Last Modified: Thu, 11 Aug 2022 00:38:06 GMT  
		Size: 205.9 KB (205888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe12872e965332f5c42d1844aa3dfdbae46eda912838801110e130b89cc181ca`  
		Last Modified: Thu, 11 Aug 2022 00:38:06 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a33b8651215087c0b9c9d0edc3a3fb9e0d18f0eaf36a0c0bfcddce94e338d57`  
		Last Modified: Thu, 11 Aug 2022 00:38:06 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.2-alpine` - linux; arm variant v7

```console
$ docker pull spiped@sha256:0e746939643dcaba40d0c1f15f4d142129555ff4d3a187e755c3643cb387bca1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 MB (2621321 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:af5a28036aaca6f3accc02f7ab66d26c0d7ef2c544316b0df54081730f89391e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Mon, 18 Jul 2022 21:24:47 GMT
ADD file:68590e866bc6db27ad54d23de7dd275d0389cb86e4e6291a1243fcc234f2f7a1 in / 
# Mon, 18 Jul 2022 21:24:47 GMT
CMD ["/bin/sh"]
# Wed, 03 Aug 2022 21:57:08 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Wed, 03 Aug 2022 21:57:09 GMT
RUN apk add --no-cache libssl1.1
# Wed, 03 Aug 2022 21:57:09 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 03 Aug 2022 21:57:16 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Wed, 03 Aug 2022 21:57:17 GMT
VOLUME [/spiped]
# Wed, 03 Aug 2022 21:57:17 GMT
WORKDIR /spiped
# Wed, 03 Aug 2022 21:57:17 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 03 Aug 2022 21:57:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 03 Aug 2022 21:57:17 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:a6b45ace95f42a930d15c33679ab9c85d46019b7e73954cadc73bb9ba176509b`  
		Last Modified: Mon, 18 Jul 2022 19:08:56 GMT  
		Size: 2.4 MB (2412307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a223ea05945b5c5ea98e31d53b7924f548e24abe646453181a3b73f940a52de`  
		Last Modified: Wed, 03 Aug 2022 21:58:06 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:868bbc51d36bab84123a304360d9b4bc7db9f0714c2281b34b7585ff494ab1c8`  
		Last Modified: Wed, 03 Aug 2022 21:58:06 GMT  
		Size: 7.7 KB (7730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18353dabcadb1dc2dc0b669eeff1d9dd8d42a815bd9f860e8ff08c8f2191131f`  
		Last Modified: Wed, 03 Aug 2022 21:58:06 GMT  
		Size: 199.5 KB (199542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:330712fbce762a1e0c7e7bcf9c36a39c454fa780a6901be6761dd588dc043f5f`  
		Last Modified: Wed, 03 Aug 2022 21:58:06 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:221966fcc255ad5deb2fa5ce1fc0b504eff307dc6e7aaebe7db90698290052eb`  
		Last Modified: Wed, 03 Aug 2022 21:58:06 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.2-alpine` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:31d9f2978a4900b825028e1c399cd7d0638f75f91f2400f6c6bc1d83d6274fb6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 MB (2931313 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:031699f5a5efac86682c564a2c655c7eab52ce5aa91a856923d2032ea0517c52`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 09 Aug 2022 17:39:41 GMT
ADD file:960fd469d48cf79ba14bbda71f3192074ed860c112e30e0bc92bff3440cb45ab in / 
# Tue, 09 Aug 2022 17:39:42 GMT
CMD ["/bin/sh"]
# Wed, 10 Aug 2022 06:09:41 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Wed, 10 Aug 2022 06:09:42 GMT
RUN apk add --no-cache libssl1.1
# Wed, 10 Aug 2022 06:09:43 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 10 Aug 2022 06:09:54 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Wed, 10 Aug 2022 06:09:55 GMT
VOLUME [/spiped]
# Wed, 10 Aug 2022 06:09:56 GMT
WORKDIR /spiped
# Wed, 10 Aug 2022 06:09:58 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 10 Aug 2022 06:09:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 10 Aug 2022 06:09:59 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:9b18e9b68314027565b90ff6189d65942c0f7986da80df008b8431276885218e`  
		Last Modified: Tue, 09 Aug 2022 17:40:38 GMT  
		Size: 2.7 MB (2707663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bf9d3ec407b6270ec79bb3c0552c48d0afd7888773c72f1b25bfc396d4c3eb7`  
		Last Modified: Wed, 10 Aug 2022 06:10:25 GMT  
		Size: 1.2 KB (1244 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99f1183a0c8143435d389abc100d22d7289e4a81f966ca3b9d8301cfb01947b2`  
		Last Modified: Wed, 10 Aug 2022 06:10:25 GMT  
		Size: 7.7 KB (7710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8abc3813fe4a6ffebb8bdde4bd9005230c2935072094662e52a3a81cc9a9c3fa`  
		Last Modified: Wed, 10 Aug 2022 06:10:26 GMT  
		Size: 214.3 KB (214262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab3f496ad70b8f2f8ea93c54500ad75fb9fa4b72d7868ae964cce858765988a4`  
		Last Modified: Wed, 10 Aug 2022 06:10:26 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46086b9ffd0c9eed5aadecf28229d0ab4532a26add5be2f474ced21cf4f25f7e`  
		Last Modified: Wed, 10 Aug 2022 06:10:25 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.2-alpine` - linux; 386

```console
$ docker pull spiped@sha256:ee4833bbef16308d250de2dac9ad7a6019a6f2e42880ed8eb3dfd4fcecc4ced4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (3047835 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:75c145e337e061db2f783bf06d6d6b2f1e63cf3e7dedb8ada91bc1744b707620`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 09 Aug 2022 17:38:39 GMT
ADD file:b828bc14bc5ff03c8f7310fe0aed6ac5df19a393622d5d1d779a523234d07c0a in / 
# Tue, 09 Aug 2022 17:38:39 GMT
CMD ["/bin/sh"]
# Wed, 10 Aug 2022 00:02:16 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Wed, 10 Aug 2022 00:02:18 GMT
RUN apk add --no-cache libssl1.1
# Wed, 10 Aug 2022 00:02:19 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 10 Aug 2022 00:02:30 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Wed, 10 Aug 2022 00:02:31 GMT
VOLUME [/spiped]
# Wed, 10 Aug 2022 00:02:32 GMT
WORKDIR /spiped
# Wed, 10 Aug 2022 00:02:34 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 10 Aug 2022 00:02:34 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 10 Aug 2022 00:02:35 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:6c0d3b419d848ea31ca748254611d5d5ce3b76e3d7bba520fd87400fbb75f3b9`  
		Last Modified: Tue, 09 Aug 2022 17:39:33 GMT  
		Size: 2.8 MB (2807121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:072149e09853327c1921fc351fbf7a93e1056edfefc5daa66cbdc6e48843cd13`  
		Last Modified: Wed, 10 Aug 2022 00:03:04 GMT  
		Size: 1.2 KB (1243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34965b4906426a2b44e36dc3fd455d5da36569c3a0c3de199beecfc03c85244c`  
		Last Modified: Wed, 10 Aug 2022 00:03:04 GMT  
		Size: 7.7 KB (7710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ddeae6e8a846e3df57fb016e864191c85342272b8c766aea5b9cd0e001b0332`  
		Last Modified: Wed, 10 Aug 2022 00:03:05 GMT  
		Size: 231.3 KB (231325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:463f4e96eadc8d28add083b4c188fcdde9cecb3831b8c5427343441c383e1136`  
		Last Modified: Wed, 10 Aug 2022 00:03:04 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3648573cf3f78bda63b9ea60198dd66926dda5cbd250025fbf6c5c0f08bbbcb4`  
		Last Modified: Wed, 10 Aug 2022 00:03:04 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.2-alpine` - linux; ppc64le

```console
$ docker pull spiped@sha256:d67f02f9e68884fbd145362c4f490cdfb403437bcf89d1135ad1a15c92052a5a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (3033050 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:14fd901b20c0f04f13ac388776797050b3e6a48903ceeccca414c16f53e1c29f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 09 Aug 2022 17:17:09 GMT
ADD file:66b351666e41834033d334aeb3dc6998dea77aa22e8e254028c923fee67a41a8 in / 
# Tue, 09 Aug 2022 17:17:10 GMT
CMD ["/bin/sh"]
# Wed, 10 Aug 2022 02:55:17 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Wed, 10 Aug 2022 02:55:19 GMT
RUN apk add --no-cache libssl1.1
# Wed, 10 Aug 2022 02:55:19 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 10 Aug 2022 02:55:34 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Wed, 10 Aug 2022 02:55:34 GMT
VOLUME [/spiped]
# Wed, 10 Aug 2022 02:55:35 GMT
WORKDIR /spiped
# Wed, 10 Aug 2022 02:55:36 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 10 Aug 2022 02:55:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 10 Aug 2022 02:55:36 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:c79e5d1a8c89b87020a754c8a5c8370faaa37bfb5bca1d8af66770d522ef1caf`  
		Last Modified: Tue, 09 Aug 2022 17:18:26 GMT  
		Size: 2.8 MB (2803320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cd8832ea95a37bc42923d861cfefd27ec973fed3564060fce137b8d54f75e02`  
		Last Modified: Wed, 10 Aug 2022 02:56:11 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ab0760cebdd26f5d818b164fe30701e72c6ec6c6c6b97b100ed16bc24fcf653`  
		Last Modified: Wed, 10 Aug 2022 02:56:11 GMT  
		Size: 7.7 KB (7739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8cdb874eec093d50ac091467e93cb88955a1ee87db0d0dd84cc6344ad829323`  
		Last Modified: Wed, 10 Aug 2022 02:56:11 GMT  
		Size: 220.3 KB (220255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a349e85c23948cd849a1a373c684ee566e0544af2297f9904d664dbb41dc8a6`  
		Last Modified: Wed, 10 Aug 2022 02:56:22 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bd274005021e79dbc526fb1fd7ad0d420d2e5c10abf68e3c7ae46021ae45cbf`  
		Last Modified: Wed, 10 Aug 2022 02:56:11 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.2-alpine` - linux; s390x

```console
$ docker pull spiped@sha256:936312a4e0595fc377ed5e910f12d52cfc4fae63a6190fe388481f204758a480
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 MB (2808502 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:afa6705ab1cc71e7aa223e1b9c9ba81f85eacacdba00737aa34a7014d8d94163`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 09 Aug 2022 17:41:46 GMT
ADD file:b43a065471bc4711415d3c67cd5b6559b0c48ee7ffe9761530477cf457a6dc34 in / 
# Tue, 09 Aug 2022 17:41:46 GMT
CMD ["/bin/sh"]
# Wed, 10 Aug 2022 05:46:33 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Wed, 10 Aug 2022 05:46:34 GMT
RUN apk add --no-cache libssl1.1
# Wed, 10 Aug 2022 05:46:34 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 10 Aug 2022 05:46:39 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Wed, 10 Aug 2022 05:46:39 GMT
VOLUME [/spiped]
# Wed, 10 Aug 2022 05:46:39 GMT
WORKDIR /spiped
# Wed, 10 Aug 2022 05:46:39 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 10 Aug 2022 05:46:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 10 Aug 2022 05:46:40 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:790c84f1f3409eab952345157df7fa804ba6b5f06d4ceb6f2dfa3c6de2064397`  
		Last Modified: Tue, 09 Aug 2022 17:42:45 GMT  
		Size: 2.6 MB (2590597 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e997054cff6af24fce535516fc4358eabc7dace5f52f427e6a19340c04f6adfe`  
		Last Modified: Wed, 10 Aug 2022 05:47:31 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b78da263b8c9f381935ae64289597db6f2e0d7e77fa388ce819ba7afecd17ef1`  
		Last Modified: Wed, 10 Aug 2022 05:47:35 GMT  
		Size: 7.7 KB (7742 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1acce323c9898120275bb4b4763b7a8971f71720bf7cafb55201dc313247560c`  
		Last Modified: Wed, 10 Aug 2022 05:47:35 GMT  
		Size: 208.4 KB (208429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98b550d52792a92d7c50d7e5102763598d59d41f0c34d5bd928fbd55e16de8f8`  
		Last Modified: Wed, 10 Aug 2022 05:47:35 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:130443af95b4efa2ff2d4d039066967531a4e10357d515888d55082f26340a52`  
		Last Modified: Wed, 10 Aug 2022 05:47:35 GMT  
		Size: 336.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:alpine`

```console
$ docker pull spiped@sha256:acddecb1628480a3371f5c7990076e0d894c6a9a2e7612d844e800178fabe8ba
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
$ docker pull spiped@sha256:66b3d848f73df6532c49bb456c441a37691db14797c1288fa9cd5deb9cf9bdb6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (3036703 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ebcb8fdfbde39b2b89abb4cdfac48560f245fff78fc822e3daac086fd5b29f78`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 09 Aug 2022 17:19:53 GMT
ADD file:2a949686d9886ac7c10582a6c29116fd29d3077d02755e87e111870d63607725 in / 
# Tue, 09 Aug 2022 17:19:53 GMT
CMD ["/bin/sh"]
# Wed, 10 Aug 2022 02:25:05 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Wed, 10 Aug 2022 02:25:06 GMT
RUN apk add --no-cache libssl1.1
# Wed, 10 Aug 2022 02:25:06 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 10 Aug 2022 02:25:16 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Wed, 10 Aug 2022 02:25:17 GMT
VOLUME [/spiped]
# Wed, 10 Aug 2022 02:25:17 GMT
WORKDIR /spiped
# Wed, 10 Aug 2022 02:25:17 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 10 Aug 2022 02:25:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 10 Aug 2022 02:25:17 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:213ec9aee27d8be045c6a92b7eac22c9a64b44558193775a1a7f626352392b49`  
		Last Modified: Tue, 09 Aug 2022 14:25:13 GMT  
		Size: 2.8 MB (2806054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:210040c27162008830a83da8ed96f452757ffa50050398230f525b2f22a4541a`  
		Last Modified: Wed, 10 Aug 2022 02:25:34 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b05b54e70388210c7ffd8a9fbb864ca9f878f8ad3dc1613e4b96b107919baadc`  
		Last Modified: Wed, 10 Aug 2022 02:25:34 GMT  
		Size: 7.7 KB (7735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28b8ff19a9777e30476c0a48eab4bc4817e9a96226faf7b42870225d69a37ba8`  
		Last Modified: Wed, 10 Aug 2022 02:25:34 GMT  
		Size: 221.2 KB (221175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:700f71a1b577cfb700f72058dad655d1ec9161da01b7fe6e8bb2b2461d1ddbbe`  
		Last Modified: Wed, 10 Aug 2022 02:25:34 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6c2f8d0b8416d1c553517142cd373249cbbdc3a03229d96604cd32b318a1195`  
		Last Modified: Wed, 10 Aug 2022 02:25:34 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; arm variant v6

```console
$ docker pull spiped@sha256:9bf39d60020a139fa461ebb060df6df01d5164425285c6bfc1b3113ef2242277
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 MB (2829328 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:88197140375c26dcc5aa5dad079e8343608e24c8a03e91eb5d2fb13c9e09deec`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 09 Aug 2022 17:49:22 GMT
ADD file:e8733e8cc0a81e15ca4041760b6e27392c34171512d34405a9b262b1fff5c687 in / 
# Tue, 09 Aug 2022 17:49:22 GMT
CMD ["/bin/sh"]
# Thu, 11 Aug 2022 00:37:38 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 11 Aug 2022 00:37:39 GMT
RUN apk add --no-cache libssl1.1
# Thu, 11 Aug 2022 00:37:39 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 11 Aug 2022 00:37:47 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Thu, 11 Aug 2022 00:37:47 GMT
VOLUME [/spiped]
# Thu, 11 Aug 2022 00:37:47 GMT
WORKDIR /spiped
# Thu, 11 Aug 2022 00:37:47 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 11 Aug 2022 00:37:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 11 Aug 2022 00:37:47 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:9506b835437abb4d8ba1683e00c500b8f77e1975e930b356fbb72f2dbdc274d9`  
		Last Modified: Tue, 09 Aug 2022 17:50:33 GMT  
		Size: 2.6 MB (2613965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3f8a3e1b897eaae3127b4c0c6bf167dc3d7740bbf9596a97a994f1249716538`  
		Last Modified: Thu, 11 Aug 2022 00:38:06 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fa63959f901bfbea0a7da0112a6c04fe32edaaf453bc28bc784d942ef8a1c01`  
		Last Modified: Thu, 11 Aug 2022 00:38:06 GMT  
		Size: 7.7 KB (7736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb53413b98987994a206c07b7c3ba39980d1dd0149f4a1be509beab0c15b75da`  
		Last Modified: Thu, 11 Aug 2022 00:38:06 GMT  
		Size: 205.9 KB (205888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe12872e965332f5c42d1844aa3dfdbae46eda912838801110e130b89cc181ca`  
		Last Modified: Thu, 11 Aug 2022 00:38:06 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a33b8651215087c0b9c9d0edc3a3fb9e0d18f0eaf36a0c0bfcddce94e338d57`  
		Last Modified: Thu, 11 Aug 2022 00:38:06 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; arm variant v7

```console
$ docker pull spiped@sha256:0e746939643dcaba40d0c1f15f4d142129555ff4d3a187e755c3643cb387bca1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 MB (2621321 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:af5a28036aaca6f3accc02f7ab66d26c0d7ef2c544316b0df54081730f89391e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Mon, 18 Jul 2022 21:24:47 GMT
ADD file:68590e866bc6db27ad54d23de7dd275d0389cb86e4e6291a1243fcc234f2f7a1 in / 
# Mon, 18 Jul 2022 21:24:47 GMT
CMD ["/bin/sh"]
# Wed, 03 Aug 2022 21:57:08 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Wed, 03 Aug 2022 21:57:09 GMT
RUN apk add --no-cache libssl1.1
# Wed, 03 Aug 2022 21:57:09 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 03 Aug 2022 21:57:16 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Wed, 03 Aug 2022 21:57:17 GMT
VOLUME [/spiped]
# Wed, 03 Aug 2022 21:57:17 GMT
WORKDIR /spiped
# Wed, 03 Aug 2022 21:57:17 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 03 Aug 2022 21:57:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 03 Aug 2022 21:57:17 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:a6b45ace95f42a930d15c33679ab9c85d46019b7e73954cadc73bb9ba176509b`  
		Last Modified: Mon, 18 Jul 2022 19:08:56 GMT  
		Size: 2.4 MB (2412307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a223ea05945b5c5ea98e31d53b7924f548e24abe646453181a3b73f940a52de`  
		Last Modified: Wed, 03 Aug 2022 21:58:06 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:868bbc51d36bab84123a304360d9b4bc7db9f0714c2281b34b7585ff494ab1c8`  
		Last Modified: Wed, 03 Aug 2022 21:58:06 GMT  
		Size: 7.7 KB (7730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18353dabcadb1dc2dc0b669eeff1d9dd8d42a815bd9f860e8ff08c8f2191131f`  
		Last Modified: Wed, 03 Aug 2022 21:58:06 GMT  
		Size: 199.5 KB (199542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:330712fbce762a1e0c7e7bcf9c36a39c454fa780a6901be6761dd588dc043f5f`  
		Last Modified: Wed, 03 Aug 2022 21:58:06 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:221966fcc255ad5deb2fa5ce1fc0b504eff307dc6e7aaebe7db90698290052eb`  
		Last Modified: Wed, 03 Aug 2022 21:58:06 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:31d9f2978a4900b825028e1c399cd7d0638f75f91f2400f6c6bc1d83d6274fb6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 MB (2931313 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:031699f5a5efac86682c564a2c655c7eab52ce5aa91a856923d2032ea0517c52`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 09 Aug 2022 17:39:41 GMT
ADD file:960fd469d48cf79ba14bbda71f3192074ed860c112e30e0bc92bff3440cb45ab in / 
# Tue, 09 Aug 2022 17:39:42 GMT
CMD ["/bin/sh"]
# Wed, 10 Aug 2022 06:09:41 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Wed, 10 Aug 2022 06:09:42 GMT
RUN apk add --no-cache libssl1.1
# Wed, 10 Aug 2022 06:09:43 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 10 Aug 2022 06:09:54 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Wed, 10 Aug 2022 06:09:55 GMT
VOLUME [/spiped]
# Wed, 10 Aug 2022 06:09:56 GMT
WORKDIR /spiped
# Wed, 10 Aug 2022 06:09:58 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 10 Aug 2022 06:09:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 10 Aug 2022 06:09:59 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:9b18e9b68314027565b90ff6189d65942c0f7986da80df008b8431276885218e`  
		Last Modified: Tue, 09 Aug 2022 17:40:38 GMT  
		Size: 2.7 MB (2707663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bf9d3ec407b6270ec79bb3c0552c48d0afd7888773c72f1b25bfc396d4c3eb7`  
		Last Modified: Wed, 10 Aug 2022 06:10:25 GMT  
		Size: 1.2 KB (1244 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99f1183a0c8143435d389abc100d22d7289e4a81f966ca3b9d8301cfb01947b2`  
		Last Modified: Wed, 10 Aug 2022 06:10:25 GMT  
		Size: 7.7 KB (7710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8abc3813fe4a6ffebb8bdde4bd9005230c2935072094662e52a3a81cc9a9c3fa`  
		Last Modified: Wed, 10 Aug 2022 06:10:26 GMT  
		Size: 214.3 KB (214262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab3f496ad70b8f2f8ea93c54500ad75fb9fa4b72d7868ae964cce858765988a4`  
		Last Modified: Wed, 10 Aug 2022 06:10:26 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46086b9ffd0c9eed5aadecf28229d0ab4532a26add5be2f474ced21cf4f25f7e`  
		Last Modified: Wed, 10 Aug 2022 06:10:25 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; 386

```console
$ docker pull spiped@sha256:ee4833bbef16308d250de2dac9ad7a6019a6f2e42880ed8eb3dfd4fcecc4ced4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (3047835 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:75c145e337e061db2f783bf06d6d6b2f1e63cf3e7dedb8ada91bc1744b707620`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 09 Aug 2022 17:38:39 GMT
ADD file:b828bc14bc5ff03c8f7310fe0aed6ac5df19a393622d5d1d779a523234d07c0a in / 
# Tue, 09 Aug 2022 17:38:39 GMT
CMD ["/bin/sh"]
# Wed, 10 Aug 2022 00:02:16 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Wed, 10 Aug 2022 00:02:18 GMT
RUN apk add --no-cache libssl1.1
# Wed, 10 Aug 2022 00:02:19 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 10 Aug 2022 00:02:30 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Wed, 10 Aug 2022 00:02:31 GMT
VOLUME [/spiped]
# Wed, 10 Aug 2022 00:02:32 GMT
WORKDIR /spiped
# Wed, 10 Aug 2022 00:02:34 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 10 Aug 2022 00:02:34 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 10 Aug 2022 00:02:35 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:6c0d3b419d848ea31ca748254611d5d5ce3b76e3d7bba520fd87400fbb75f3b9`  
		Last Modified: Tue, 09 Aug 2022 17:39:33 GMT  
		Size: 2.8 MB (2807121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:072149e09853327c1921fc351fbf7a93e1056edfefc5daa66cbdc6e48843cd13`  
		Last Modified: Wed, 10 Aug 2022 00:03:04 GMT  
		Size: 1.2 KB (1243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34965b4906426a2b44e36dc3fd455d5da36569c3a0c3de199beecfc03c85244c`  
		Last Modified: Wed, 10 Aug 2022 00:03:04 GMT  
		Size: 7.7 KB (7710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ddeae6e8a846e3df57fb016e864191c85342272b8c766aea5b9cd0e001b0332`  
		Last Modified: Wed, 10 Aug 2022 00:03:05 GMT  
		Size: 231.3 KB (231325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:463f4e96eadc8d28add083b4c188fcdde9cecb3831b8c5427343441c383e1136`  
		Last Modified: Wed, 10 Aug 2022 00:03:04 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3648573cf3f78bda63b9ea60198dd66926dda5cbd250025fbf6c5c0f08bbbcb4`  
		Last Modified: Wed, 10 Aug 2022 00:03:04 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; ppc64le

```console
$ docker pull spiped@sha256:d67f02f9e68884fbd145362c4f490cdfb403437bcf89d1135ad1a15c92052a5a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (3033050 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:14fd901b20c0f04f13ac388776797050b3e6a48903ceeccca414c16f53e1c29f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 09 Aug 2022 17:17:09 GMT
ADD file:66b351666e41834033d334aeb3dc6998dea77aa22e8e254028c923fee67a41a8 in / 
# Tue, 09 Aug 2022 17:17:10 GMT
CMD ["/bin/sh"]
# Wed, 10 Aug 2022 02:55:17 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Wed, 10 Aug 2022 02:55:19 GMT
RUN apk add --no-cache libssl1.1
# Wed, 10 Aug 2022 02:55:19 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 10 Aug 2022 02:55:34 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Wed, 10 Aug 2022 02:55:34 GMT
VOLUME [/spiped]
# Wed, 10 Aug 2022 02:55:35 GMT
WORKDIR /spiped
# Wed, 10 Aug 2022 02:55:36 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 10 Aug 2022 02:55:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 10 Aug 2022 02:55:36 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:c79e5d1a8c89b87020a754c8a5c8370faaa37bfb5bca1d8af66770d522ef1caf`  
		Last Modified: Tue, 09 Aug 2022 17:18:26 GMT  
		Size: 2.8 MB (2803320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cd8832ea95a37bc42923d861cfefd27ec973fed3564060fce137b8d54f75e02`  
		Last Modified: Wed, 10 Aug 2022 02:56:11 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ab0760cebdd26f5d818b164fe30701e72c6ec6c6c6b97b100ed16bc24fcf653`  
		Last Modified: Wed, 10 Aug 2022 02:56:11 GMT  
		Size: 7.7 KB (7739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8cdb874eec093d50ac091467e93cb88955a1ee87db0d0dd84cc6344ad829323`  
		Last Modified: Wed, 10 Aug 2022 02:56:11 GMT  
		Size: 220.3 KB (220255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a349e85c23948cd849a1a373c684ee566e0544af2297f9904d664dbb41dc8a6`  
		Last Modified: Wed, 10 Aug 2022 02:56:22 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bd274005021e79dbc526fb1fd7ad0d420d2e5c10abf68e3c7ae46021ae45cbf`  
		Last Modified: Wed, 10 Aug 2022 02:56:11 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; s390x

```console
$ docker pull spiped@sha256:936312a4e0595fc377ed5e910f12d52cfc4fae63a6190fe388481f204758a480
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 MB (2808502 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:afa6705ab1cc71e7aa223e1b9c9ba81f85eacacdba00737aa34a7014d8d94163`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 09 Aug 2022 17:41:46 GMT
ADD file:b43a065471bc4711415d3c67cd5b6559b0c48ee7ffe9761530477cf457a6dc34 in / 
# Tue, 09 Aug 2022 17:41:46 GMT
CMD ["/bin/sh"]
# Wed, 10 Aug 2022 05:46:33 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Wed, 10 Aug 2022 05:46:34 GMT
RUN apk add --no-cache libssl1.1
# Wed, 10 Aug 2022 05:46:34 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 10 Aug 2022 05:46:39 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Wed, 10 Aug 2022 05:46:39 GMT
VOLUME [/spiped]
# Wed, 10 Aug 2022 05:46:39 GMT
WORKDIR /spiped
# Wed, 10 Aug 2022 05:46:39 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 10 Aug 2022 05:46:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 10 Aug 2022 05:46:40 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:790c84f1f3409eab952345157df7fa804ba6b5f06d4ceb6f2dfa3c6de2064397`  
		Last Modified: Tue, 09 Aug 2022 17:42:45 GMT  
		Size: 2.6 MB (2590597 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e997054cff6af24fce535516fc4358eabc7dace5f52f427e6a19340c04f6adfe`  
		Last Modified: Wed, 10 Aug 2022 05:47:31 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b78da263b8c9f381935ae64289597db6f2e0d7e77fa388ce819ba7afecd17ef1`  
		Last Modified: Wed, 10 Aug 2022 05:47:35 GMT  
		Size: 7.7 KB (7742 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1acce323c9898120275bb4b4763b7a8971f71720bf7cafb55201dc313247560c`  
		Last Modified: Wed, 10 Aug 2022 05:47:35 GMT  
		Size: 208.4 KB (208429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98b550d52792a92d7c50d7e5102763598d59d41f0c34d5bd928fbd55e16de8f8`  
		Last Modified: Wed, 10 Aug 2022 05:47:35 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:130443af95b4efa2ff2d4d039066967531a4e10357d515888d55082f26340a52`  
		Last Modified: Wed, 10 Aug 2022 05:47:35 GMT  
		Size: 336.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:latest`

```console
$ docker pull spiped@sha256:6442d9ca640a1475fe7f8827406c94ab677a48776e9653472bd6523a120609dc
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
$ docker pull spiped@sha256:dad19d6d4fd551afedb73402fbe587665af498a94aab95d1f1c65b6fca26b254
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.3 MB (37337269 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ad8d035bd9a75027ee1fd4c3aa1157c358bb1ffceba1d2ae6cee8caa104b286a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 02 Aug 2022 01:20:04 GMT
ADD file:0eae0dca665c7044bf242cb1fc92cb8ea744f5af2dd376a558c90bc47349aefe in / 
# Tue, 02 Aug 2022 01:20:05 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 14:59:44 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 02 Aug 2022 14:59:47 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 14:59:47 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 02 Aug 2022 15:00:07 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 02 Aug 2022 15:00:08 GMT
VOLUME [/spiped]
# Tue, 02 Aug 2022 15:00:08 GMT
WORKDIR /spiped
# Tue, 02 Aug 2022 15:00:08 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 02 Aug 2022 15:00:08 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 02 Aug 2022 15:00:08 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:1efc276f4ff952c055dea726cfc96ec6a4fdb8b62d9eed816bd2b788f2860ad7`  
		Last Modified: Tue, 02 Aug 2022 01:24:13 GMT  
		Size: 31.4 MB (31366757 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71902ff87bbf89a7cab2e1efdfe743d124a3eb6896b31675c52ab90dd16095e9`  
		Last Modified: Tue, 02 Aug 2022 15:00:25 GMT  
		Size: 1.7 KB (1733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a4a4f0063093cdc07df60de1a6d30e856a4ed528faac41e365607eb44758cec`  
		Last Modified: Tue, 02 Aug 2022 15:00:25 GMT  
		Size: 1.0 KB (1049 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33ba4d77b594746542f2e71dd52678ddd883c436d88b72e2465c4eb7e01809da`  
		Last Modified: Tue, 02 Aug 2022 15:00:26 GMT  
		Size: 6.0 MB (5967261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71bba1d841b515de61167758f804ee176e5ae08c5d1171a8fda3781007b78158`  
		Last Modified: Tue, 02 Aug 2022 15:00:25 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:634b21022fb2ad7cfda5a174c30da9483511cea6cc668b1c7b925613d777cfb2`  
		Last Modified: Tue, 02 Aug 2022 15:00:25 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; arm variant v5

```console
$ docker pull spiped@sha256:6af880d390673b3da576db810a3f341c7e097879fd5b825384cf454c94209ca3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.9 MB (33936434 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1c3ede774f72c0efbe443d6545abe99b06d36efbdac21a941da05cf12db4dd78`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 02 Aug 2022 00:49:10 GMT
ADD file:4cd2f95737fd3007912428eeac56036c9e67e989e66cec08a8be99da47f88494 in / 
# Tue, 02 Aug 2022 00:49:10 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 19:51:33 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 02 Aug 2022 19:51:40 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 19:51:40 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 02 Aug 2022 19:52:11 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 02 Aug 2022 19:52:11 GMT
VOLUME [/spiped]
# Tue, 02 Aug 2022 19:52:11 GMT
WORKDIR /spiped
# Tue, 02 Aug 2022 19:52:12 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 02 Aug 2022 19:52:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 02 Aug 2022 19:52:12 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:5890b0ca6af5e8467a488e68716691950496a8f247d0495c2d595ddcb1893aff`  
		Last Modified: Tue, 02 Aug 2022 00:56:06 GMT  
		Size: 28.9 MB (28905515 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5914210ab5e9d450cc5cc817ba9a969a99a1bba9caff02b44bcf07b6daa99101`  
		Last Modified: Tue, 02 Aug 2022 19:52:38 GMT  
		Size: 1.7 KB (1726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:591059447642cb76dea322da399255cce3dfc35a2ab27142398a6c0b76c7db1a`  
		Last Modified: Tue, 02 Aug 2022 19:52:38 GMT  
		Size: 1.1 KB (1053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b596d1e863582490afb5019016264b3b75d44f08716d556cd395a4286210a5d`  
		Last Modified: Tue, 02 Aug 2022 19:52:41 GMT  
		Size: 5.0 MB (5027669 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:786bcf276f826fa83f9eef22ee3dd243c1b03582f76dcf0d838c8036997e795e`  
		Last Modified: Tue, 02 Aug 2022 19:52:38 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17e2aa3589894439340437bb0befccb5068c4051e6cc7b57e53f7e764bf4beb0`  
		Last Modified: Tue, 02 Aug 2022 19:52:39 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; arm variant v7

```console
$ docker pull spiped@sha256:05546f55c08afb1515cfc5708756ed4940307346ba553f0f975bf31140ab7573
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.3 MB (31311995 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fe18f0b13d76c9fe4af1797ce9d740ef87d42b1ce2094b53680be65b310394ed`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 02 Aug 2022 00:58:59 GMT
ADD file:1575b776a15adacebc0875642e97a80807d42dcfc8917e1406d47af7ac244c97 in / 
# Tue, 02 Aug 2022 00:58:59 GMT
CMD ["bash"]
# Wed, 03 Aug 2022 21:56:42 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 03 Aug 2022 21:56:45 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 03 Aug 2022 21:56:45 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 03 Aug 2022 21:57:01 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 03 Aug 2022 21:57:01 GMT
VOLUME [/spiped]
# Wed, 03 Aug 2022 21:57:01 GMT
WORKDIR /spiped
# Wed, 03 Aug 2022 21:57:01 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 03 Aug 2022 21:57:01 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 03 Aug 2022 21:57:01 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:1dd75a3a9c893a7dc313f683dd62464b7eab6c6d522ee62c8a17022631830f32`  
		Last Modified: Tue, 02 Aug 2022 01:06:45 GMT  
		Size: 26.6 MB (26560586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bcaffbe5be1966b473b328a91c40df9286228c74466eea7154a543527b6fae1`  
		Last Modified: Wed, 03 Aug 2022 21:57:45 GMT  
		Size: 1.7 KB (1726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2917d25466b0b307ff25a0fc7718a5e32785e7eef826f642b28d0439be6adc9e`  
		Last Modified: Wed, 03 Aug 2022 21:57:45 GMT  
		Size: 1.1 KB (1053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7caa787abd6178478de179d6cc5db9a07a792b29b34b9fc9486347a7c1b017f`  
		Last Modified: Wed, 03 Aug 2022 21:57:46 GMT  
		Size: 4.7 MB (4748161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3801153d36fffb70fcfc49890ef5d327bfc8b15f3a1cc6fa4d0d9b12eb27ff9`  
		Last Modified: Wed, 03 Aug 2022 21:57:45 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a742fab32925896cf7cffe6ca60ee420e328f9391fe5bcfc9f1f46e7f631ce3a`  
		Last Modified: Wed, 03 Aug 2022 21:57:45 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:4835debf7fbae32c4cc4cdc11e8792dc97767b8916ed69b695839b47ce2c5b49
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.3 MB (35328219 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:11bb3a1dd6e7229d9d7d203d5f015250cd44ab7d412ae6d00adbe3817b938ceb`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 02 Aug 2022 00:40:38 GMT
ADD file:6039adfbca55ed34a719c37672c664e3524130a0e2a3b8663629b8120b81b790 in / 
# Tue, 02 Aug 2022 00:40:39 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 16:47:23 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 02 Aug 2022 16:47:26 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 16:47:27 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 02 Aug 2022 16:47:45 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 02 Aug 2022 16:47:45 GMT
VOLUME [/spiped]
# Tue, 02 Aug 2022 16:47:46 GMT
WORKDIR /spiped
# Tue, 02 Aug 2022 16:47:48 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 02 Aug 2022 16:47:48 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 02 Aug 2022 16:47:49 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:a9fe95647e78b5516c7e2327355b6996e2ea295cd76ae242cbfe87f016b4e760`  
		Last Modified: Tue, 02 Aug 2022 00:46:05 GMT  
		Size: 30.1 MB (30054304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0215749fa5edad97431836093e99ce69829b4a2b18c351fe7e22c9bf90cb3fef`  
		Last Modified: Tue, 02 Aug 2022 16:48:17 GMT  
		Size: 1.6 KB (1617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6a61c46ac9b56671e11f61590184265582230b634537e091aa7515746a2ba70`  
		Last Modified: Tue, 02 Aug 2022 16:48:17 GMT  
		Size: 923.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:569abb15b59f2ea4b1fe7a95bda8247ac40c93685ac62b8029db8474d42f79cb`  
		Last Modified: Tue, 02 Aug 2022 16:48:18 GMT  
		Size: 5.3 MB (5270939 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:251fbe05e0ceba0f0f43f71ba704ee1b264165c62e3d7f999b3c597690886a75`  
		Last Modified: Tue, 02 Aug 2022 16:48:17 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10996acb338f32bf51751686febf31fd3fab4b1d46b4b8d7a7d5dfc7f05b4cee`  
		Last Modified: Tue, 02 Aug 2022 16:48:17 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; 386

```console
$ docker pull spiped@sha256:7a7dbde9446433fedc12b55ed6d0d73bbbf800753f0b4fc8c677bfd9f5d6f1fd
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.3 MB (40268619 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8544e7c71f7ba6f5ac7741eec3a5f49bd5d384c7d708d24631e0ce7e8af09460`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 02 Aug 2022 00:39:20 GMT
ADD file:f771e2286465694126158821089d801c7296376be2a56189e6041a15d2fe79f5 in / 
# Tue, 02 Aug 2022 00:39:21 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 15:45:02 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Tue, 02 Aug 2022 15:45:06 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 15:45:07 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 02 Aug 2022 15:45:28 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 02 Aug 2022 15:45:28 GMT
VOLUME [/spiped]
# Tue, 02 Aug 2022 15:45:29 GMT
WORKDIR /spiped
# Tue, 02 Aug 2022 15:45:31 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 02 Aug 2022 15:45:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 02 Aug 2022 15:45:32 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:90eb7f0ce9f33cf5dcd67d54c2fa606186dbaa5f95b6046f36145097267f9e53`  
		Last Modified: Tue, 02 Aug 2022 00:45:14 GMT  
		Size: 32.4 MB (32374054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:746b1fc4bab3964ac48dbe2fb0761a50ec33f467093556cf01fd8444415d8d11`  
		Last Modified: Tue, 02 Aug 2022 15:46:02 GMT  
		Size: 1.6 KB (1606 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2441fccbf951fe6e18f386cdd0c3cabaa845fde7d0bf966cf03f04f756510e6a`  
		Last Modified: Tue, 02 Aug 2022 15:46:02 GMT  
		Size: 924.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:231b6d32c27ff4a17c9587d6b1f9b787bb6d78e3d656a8c9467df93a850bd66f`  
		Last Modified: Tue, 02 Aug 2022 15:46:03 GMT  
		Size: 7.9 MB (7891596 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:072a58cf67fb04afdb3086a5a441fa938a2ede9871a6088da9f6bfd36cc65467`  
		Last Modified: Tue, 02 Aug 2022 15:46:02 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cac32ec13523eeeefcd7dcfb5c9f5cbd39875a916b3fa22df5b9af8f12e83aba`  
		Last Modified: Tue, 02 Aug 2022 15:46:02 GMT  
		Size: 344.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; mips64le

```console
$ docker pull spiped@sha256:9e5c7480cebb7266cbc6cd8cde915e916cea44f839c3d45827ee4b32b9d1f361
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.3 MB (35337243 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6d937f2142b4729449865145c0bd382f2880465d957aac461a860e13e82a8527`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 02 Aug 2022 01:10:34 GMT
ADD file:6dc22a1e5b5fcf23f2549406ddcc45c4e244f46e21eafa881de81fa87438e5d8 in / 
# Tue, 02 Aug 2022 01:10:38 GMT
CMD ["bash"]
# Thu, 04 Aug 2022 02:58:17 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Thu, 04 Aug 2022 02:58:32 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Thu, 04 Aug 2022 02:58:34 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 04 Aug 2022 03:00:04 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 04 Aug 2022 03:00:07 GMT
VOLUME [/spiped]
# Thu, 04 Aug 2022 03:00:09 GMT
WORKDIR /spiped
# Thu, 04 Aug 2022 03:00:12 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 04 Aug 2022 03:00:14 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 04 Aug 2022 03:00:17 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:88350749a27614c791450c256b051f023d81cdd256211274b1efac493779d2be`  
		Last Modified: Tue, 02 Aug 2022 01:21:02 GMT  
		Size: 29.6 MB (29628964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a980b8d4c4081e06e63d932cacd2a2bcb9ae4455ec1d8a0edfd5e7b976a41cfe`  
		Last Modified: Thu, 04 Aug 2022 03:00:33 GMT  
		Size: 1.6 KB (1619 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e926997286379c4294d14e53409efda33e6b135fe7e1090595de1c642b53a3b2`  
		Last Modified: Thu, 04 Aug 2022 03:00:34 GMT  
		Size: 923.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28c8df0b5ceb34f25514a9e6cfc3c5e4d4fa32daaa3e805d0e78bade747962e7`  
		Last Modified: Thu, 04 Aug 2022 03:00:38 GMT  
		Size: 5.7 MB (5705299 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe20d03337baf8ea0077260b2c5f5754fca122b1397f8ac922fb9db8dff5995b`  
		Last Modified: Thu, 04 Aug 2022 03:00:33 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca8d9c536c2096001a16837bafc47410185a740c029f1aad11b395642de38f34`  
		Last Modified: Thu, 04 Aug 2022 03:00:33 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; ppc64le

```console
$ docker pull spiped@sha256:27f881ff0e1f5e61d9dc98bfdaf60bde63f0b7c46ea39da2ac2c9814dcde8dd6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.3 MB (41274919 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9792967c333043140e04ed3704d0407abc333122050747da7546fc815c45542e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 02 Aug 2022 01:17:30 GMT
ADD file:3a95a896d463569ce82199957052b3467123a4bd3385a0a4e397cf08402a99c3 in / 
# Tue, 02 Aug 2022 01:17:32 GMT
CMD ["bash"]
# Wed, 03 Aug 2022 01:28:12 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 03 Aug 2022 01:28:18 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 03 Aug 2022 01:28:18 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 03 Aug 2022 01:28:56 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 03 Aug 2022 01:28:57 GMT
VOLUME [/spiped]
# Wed, 03 Aug 2022 01:28:57 GMT
WORKDIR /spiped
# Wed, 03 Aug 2022 01:28:58 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 03 Aug 2022 01:28:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 03 Aug 2022 01:28:59 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:5241cd116d6e6e2d62f3d8c2245b74daca9f6cc154eaccd738feb41984c74714`  
		Last Modified: Tue, 02 Aug 2022 01:24:39 GMT  
		Size: 35.3 MB (35272771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52f7bfa7322f80f7fbf327da4c4244442a6121cd2aa6a0c35b98493dff99cd50`  
		Last Modified: Wed, 03 Aug 2022 01:29:58 GMT  
		Size: 1.7 KB (1731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4737eb981cc3c529f234636741599c9b27a9f5b4973f8f9b6a7628649aab6726`  
		Last Modified: Wed, 03 Aug 2022 01:29:58 GMT  
		Size: 1.1 KB (1051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69e43d769614f6318ed658c891a70ce2668635f025c326b0b52a83b54ca1498b`  
		Last Modified: Wed, 03 Aug 2022 01:30:00 GMT  
		Size: 6.0 MB (5998895 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e492fc4ffd0f67e0a0b76b694e326dce271e5ad1bbf157bfb0c9097c0c7df653`  
		Last Modified: Wed, 03 Aug 2022 01:29:58 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2606cce249be48bbc9ec4f0d08c2920e38e1b3a0735446d0a03dd275279ca1cb`  
		Last Modified: Wed, 03 Aug 2022 01:29:58 GMT  
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
