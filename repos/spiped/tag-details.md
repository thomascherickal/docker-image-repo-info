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
$ docker pull spiped@sha256:dcd50fdfd27ec8f055329f6100c9237808b11c01a4605564877a8e91c2e240a2
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
$ docker pull spiped@sha256:65d1de8326124f7025322cdba5f11590bf65237b0cb63f400e388e7ec598f533
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.4 MB (37413302 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2e6f8b4beac2d2177806929f949e4e7ae5eca9086100ed06f9464b8f863786ed`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 09 Feb 2023 03:20:20 GMT
ADD file:3ea7c69e4bfac2ebb6f86baaedab31827c86a594dba8080a49928e211ad3c7a0 in / 
# Thu, 09 Feb 2023 03:20:20 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 06:37:17 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Thu, 09 Feb 2023 06:37:20 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 06:37:20 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 09 Feb 2023 06:37:40 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 09 Feb 2023 06:37:41 GMT
VOLUME [/spiped]
# Thu, 09 Feb 2023 06:37:41 GMT
WORKDIR /spiped
# Thu, 09 Feb 2023 06:37:41 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 09 Feb 2023 06:37:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 09 Feb 2023 06:37:41 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:bb263680fed18eecdc67f885094df6f589bafc19004839d7fdf141df236a61aa`  
		Last Modified: Thu, 09 Feb 2023 03:25:13 GMT  
		Size: 31.4 MB (31411810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:904147bf2f8667febed21ce347ecd042f5b9d779a1ac552bd4055ec2d7f060b6`  
		Last Modified: Thu, 09 Feb 2023 06:37:56 GMT  
		Size: 1.7 KB (1737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa73821f4c111ea10583bad55bd382aa4196e36aeca4093bf6ad2e4f27565fb4`  
		Last Modified: Thu, 09 Feb 2023 06:37:56 GMT  
		Size: 1.0 KB (1049 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccbe509202f24ed422baf731f3dd79e740b358183ad10a4d7554c5260d1f74cb`  
		Last Modified: Thu, 09 Feb 2023 06:37:57 GMT  
		Size: 6.0 MB (5998234 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9b81852413d69c15590cca8a24757c58e49244b108abaa2f57a3173de23700a`  
		Last Modified: Thu, 09 Feb 2023 06:37:56 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:714d39b5611de4a84c8a690342eb12e7f1f27cbc13ebfa1aa2d40e6db8e79031`  
		Last Modified: Thu, 09 Feb 2023 06:37:56 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; arm variant v5

```console
$ docker pull spiped@sha256:528e13ba139adf0768024a80cfc79ab5cb3d0ea5e8f9b9f3bc1511f2d698c215
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.9 MB (33947393 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5a1e48f7b0e65652cca9ca80196c861d383ac1f1b0103cc512be95efd00fc6e9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 01 Mar 2023 01:48:54 GMT
ADD file:b4fb1081f6eb8a0560d56d5781bbcedaac1453615d56e0943245dca784785ea2 in / 
# Wed, 01 Mar 2023 01:48:54 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 07:10:40 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 01 Mar 2023 07:10:44 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 07:10:44 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 01 Mar 2023 07:11:03 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 01 Mar 2023 07:11:03 GMT
VOLUME [/spiped]
# Wed, 01 Mar 2023 07:11:03 GMT
WORKDIR /spiped
# Wed, 01 Mar 2023 07:11:03 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 01 Mar 2023 07:11:03 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 01 Mar 2023 07:11:04 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:3c3af56dbec5913ef8aec0f1ca7112eb5914b4ad346ccd48f836dd7ec0621ba5`  
		Last Modified: Wed, 01 Mar 2023 01:52:57 GMT  
		Size: 28.9 MB (28915776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9aca7d992b566279fbac9ecdeffb9ff2db68cf1ffd6f31a2cce852311c28c5ce`  
		Last Modified: Wed, 01 Mar 2023 07:11:20 GMT  
		Size: 1.7 KB (1728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fc3eb64d155ea643dfc7dde1104693192a95033b812f1cf66e286245705de6f`  
		Last Modified: Wed, 01 Mar 2023 07:11:20 GMT  
		Size: 1.1 KB (1050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9169ad29c4b57b416977f34e4cae1ad9b4efb6110e2a150a7cb43b7eab0da3d3`  
		Last Modified: Wed, 01 Mar 2023 07:11:21 GMT  
		Size: 5.0 MB (5028368 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:742f87e7cb263314cfe9b69a92b5fef45b368e04c178942b699311a03503e14c`  
		Last Modified: Wed, 01 Mar 2023 07:11:20 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0dfe2f008531a4616c872689c583cd0c8468b2fb60b07981fc0e20a80f84497`  
		Last Modified: Wed, 01 Mar 2023 07:11:20 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; arm variant v7

```console
$ docker pull spiped@sha256:7017eb815f7e60e8ff5b15b21fe0cbd2ef33396feebd8f7f18bcfd82efcbcdca
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.3 MB (31329871 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5b689ef4b4dc24e15c83f0188d2896b65dfb8ab55d95974313cbac1be6f13df4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 09 Feb 2023 06:12:09 GMT
ADD file:5f1a343224e8486690bd90dd1e50c8d84b3d770c51bb6829544e5cf650c0419c in / 
# Thu, 09 Feb 2023 06:12:10 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 12:59:21 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Thu, 09 Feb 2023 12:59:25 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 12:59:25 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 09 Feb 2023 12:59:43 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 09 Feb 2023 12:59:43 GMT
VOLUME [/spiped]
# Thu, 09 Feb 2023 12:59:43 GMT
WORKDIR /spiped
# Thu, 09 Feb 2023 12:59:44 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 09 Feb 2023 12:59:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 09 Feb 2023 12:59:44 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:e7318f6106ad75d7d482ae9dddf4d927b0872ef3ddb6e1330aa691fc8d17279e`  
		Last Modified: Thu, 09 Feb 2023 06:19:19 GMT  
		Size: 26.6 MB (26577666 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e00b17d2d80b94e1a46f2bf36d6bc77f847e4cd57083ecbb8f84ad55d31d164a`  
		Last Modified: Thu, 09 Feb 2023 13:00:24 GMT  
		Size: 1.7 KB (1730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7293faff8274bf27a2e47ec70c06f8ab91fac589d357fdd3306a81ec075c3fb`  
		Last Modified: Thu, 09 Feb 2023 13:00:24 GMT  
		Size: 1.0 KB (1022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:420c029d7a4f8d85dc09d4d90250267b2137b15106d2fe5623c195ee79fcda5f`  
		Last Modified: Thu, 09 Feb 2023 13:00:27 GMT  
		Size: 4.7 MB (4749016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a8f996daf79da4e6f40d919b8671e3c4b55085710edea0584ea9f11b834bcce`  
		Last Modified: Thu, 09 Feb 2023 13:00:24 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef6016c3c267a148094099843a4bc93c8dc6f172510f577193c40ec9772fa0de`  
		Last Modified: Thu, 09 Feb 2023 13:00:24 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:ba65bbd88dad033e812d648ab5bec4670067246f6c0ff39ae8413e1bbb54b8ce
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.3 MB (35338340 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:40a101e61165070db066921b2c5822a0f2771bfce3632b8b52055fa79ff1a4f8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 09 Feb 2023 03:58:40 GMT
ADD file:3276ac85bb957360f20720da5b37498a6b5f91a017046049f8d2fd791f728a9a in / 
# Thu, 09 Feb 2023 03:58:40 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 08:54:18 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Thu, 09 Feb 2023 08:54:20 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 08:54:20 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 09 Feb 2023 08:54:35 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 09 Feb 2023 08:54:35 GMT
VOLUME [/spiped]
# Thu, 09 Feb 2023 08:54:35 GMT
WORKDIR /spiped
# Thu, 09 Feb 2023 08:54:35 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 09 Feb 2023 08:54:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 09 Feb 2023 08:54:35 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:5731adb3a4abcefe78d75783ea6e5ee87c4604d0c6a4f8c00b50085e162a7f5d`  
		Last Modified: Thu, 09 Feb 2023 04:02:34 GMT  
		Size: 30.1 MB (30062509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8137aa16a21880e530299f722a06622e5b58e5e7096c84fab419a159a7f04091`  
		Last Modified: Thu, 09 Feb 2023 08:54:53 GMT  
		Size: 1.7 KB (1739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2c2269b7f42a74f4a740b49267f4eaed378968aa33615a2a203cb15bc9360c2`  
		Last Modified: Thu, 09 Feb 2023 08:54:54 GMT  
		Size: 1.1 KB (1050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:052457e7f7a0e19dcaacf826e2ca00910c21085d12529627fd618e0d211863de`  
		Last Modified: Thu, 09 Feb 2023 08:54:54 GMT  
		Size: 5.3 MB (5272569 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17ae4ac2dc94d44f270d10320f3a8a057ae7af3d45f1ecf9c808b9a95cde305d`  
		Last Modified: Thu, 09 Feb 2023 08:54:53 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56ed7bfb7f7c49224f53d54b2d403c5be43966bc94394495d4104501b4129c1f`  
		Last Modified: Thu, 09 Feb 2023 08:54:53 GMT  
		Size: 344.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; 386

```console
$ docker pull spiped@sha256:bfa78a9926e73b519ea52984757a09e911d14c2bd9da1ab55972bd9ce2cf2d65
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.3 MB (40290432 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b6568369d320f09cd292f11fd201b8dca3a8cd63acb3bee3c7bb677d1a6a9eb5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 09 Feb 2023 05:12:53 GMT
ADD file:7740abd3129d33122ce51153c0b6c3323b9cbe9ea0e81672e16b2d7b210d24e3 in / 
# Thu, 09 Feb 2023 05:12:53 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 11:27:18 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Thu, 09 Feb 2023 11:27:22 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 11:27:23 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 09 Feb 2023 11:27:44 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 09 Feb 2023 11:27:44 GMT
VOLUME [/spiped]
# Thu, 09 Feb 2023 11:27:45 GMT
WORKDIR /spiped
# Thu, 09 Feb 2023 11:27:47 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 09 Feb 2023 11:27:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 09 Feb 2023 11:27:48 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:20744f4988404b1dee2cd438157b288d16a89da472583c0f04332ed389b258f8`  
		Last Modified: Thu, 09 Feb 2023 05:18:42 GMT  
		Size: 32.4 MB (32396875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37e01fd7049f58e3cf43b9c079e4da2f2b953c4792ee00e77aa6bea9acc10bb6`  
		Last Modified: Thu, 09 Feb 2023 11:28:15 GMT  
		Size: 1.6 KB (1614 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf141110ec25cbcd6fba0b5455ec049cbd33a0c16c1c8374a6b55c49c44290c4`  
		Last Modified: Thu, 09 Feb 2023 11:28:16 GMT  
		Size: 926.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c620d26def5e122b57324d22b9be7126f1aff0ee2808938cbaed2c0188aafe12`  
		Last Modified: Thu, 09 Feb 2023 11:28:17 GMT  
		Size: 7.9 MB (7890579 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b03b58be7cfa61363c0156f3f24fa50f0f503e6b2919c0a00abddbedd7764eda`  
		Last Modified: Thu, 09 Feb 2023 11:28:15 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe17e554449880852355124c22a61e8bcd828562f361f183b7096cbe1cd21a09`  
		Last Modified: Thu, 09 Feb 2023 11:28:15 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; mips64le

```console
$ docker pull spiped@sha256:b2ffe0253c458c187dd8728de9223a1a801ced3878b3304a43e6bb2d6708fd52
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.3 MB (35342689 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:71b26a2c72965d659a81b09281cdf469a7aaceeb51fa5a05e5f25152bfb18426`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 09 Feb 2023 02:45:21 GMT
ADD file:68e11645a37c49c8f8f9d79ba579d0d192aaab78bb28059f07d69d56aa5ace71 in / 
# Thu, 09 Feb 2023 02:45:25 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 09:28:59 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Thu, 09 Feb 2023 09:29:14 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 09:29:16 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 09 Feb 2023 09:30:45 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 09 Feb 2023 09:30:47 GMT
VOLUME [/spiped]
# Thu, 09 Feb 2023 09:30:50 GMT
WORKDIR /spiped
# Thu, 09 Feb 2023 09:30:52 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 09 Feb 2023 09:30:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 09 Feb 2023 09:30:58 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:1b5516936229d6629ab88588210eb90edc2613c94e5952fd1caf9200284f298a`  
		Last Modified: Thu, 09 Feb 2023 02:53:48 GMT  
		Size: 29.6 MB (29634449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3441e9678cbfa1a300965eb223fd19537d15afa6185479f02efb9549b6f90356`  
		Last Modified: Thu, 09 Feb 2023 09:31:13 GMT  
		Size: 1.6 KB (1619 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b9dda8c314f6a9f00c80e8d3774028d4204d754e4c828c2c38917e39f649706`  
		Last Modified: Thu, 09 Feb 2023 09:31:13 GMT  
		Size: 926.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed7b5d79a1e160a892ae3ca9a3585b9a3859b3843800b146b50a6f8dc2e37cea`  
		Last Modified: Thu, 09 Feb 2023 09:31:18 GMT  
		Size: 5.7 MB (5705255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e3972972765aa157621d8d380622fd6d29b61d44fd1b960930a1847ba23bfbb`  
		Last Modified: Thu, 09 Feb 2023 09:31:13 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc249832f7bdc107bfaebf38fb0292b7cacb7518cba7bad019f0d8ff699994c4`  
		Last Modified: Thu, 09 Feb 2023 09:31:13 GMT  
		Size: 345.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; ppc64le

```console
$ docker pull spiped@sha256:c55bb97521e65594872fe76cbfbc246cf4f6f31b3851f51ee61256ba623233de
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.3 MB (41292154 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2584a0abea40abb2a074488d4046bfa1ee2358d7221dcaada6120144742c42a9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 09 Feb 2023 06:21:49 GMT
ADD file:b09577b8131a90731fdfb00b824a97dc65ccb51d484cb9004382035d64a5741c in / 
# Thu, 09 Feb 2023 06:21:52 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 12:13:54 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Thu, 09 Feb 2023 12:14:00 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 12:14:00 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 09 Feb 2023 12:14:49 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 09 Feb 2023 12:14:50 GMT
VOLUME [/spiped]
# Thu, 09 Feb 2023 12:14:50 GMT
WORKDIR /spiped
# Thu, 09 Feb 2023 12:14:51 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 09 Feb 2023 12:14:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 09 Feb 2023 12:14:52 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:4ea90e1a094ae86c7950bbec99e7a79b08fae641ad5f3bc3af9081c925894c41`  
		Last Modified: Thu, 09 Feb 2023 06:28:27 GMT  
		Size: 35.3 MB (35289252 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:695fd45ccd8eac48da176341bba34201c9b8980634c1df9e9e8b4bfbfa220edc`  
		Last Modified: Thu, 09 Feb 2023 12:15:27 GMT  
		Size: 1.7 KB (1735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e02fb49a13103590e46d389b8e81a60bc1d01cbf4395c01b053e5e4e99f6e312`  
		Last Modified: Thu, 09 Feb 2023 12:15:27 GMT  
		Size: 1.0 KB (1049 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e9885ddc7088b14facf6e088ded644fc33dff7b4e6625a92eb87f71975a0703`  
		Last Modified: Thu, 09 Feb 2023 12:15:29 GMT  
		Size: 6.0 MB (5999645 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:300eee5c0fb43c90cd5a5c063707252fce74ce3a8ffc7fcd444c165dfb9753a9`  
		Last Modified: Thu, 09 Feb 2023 12:15:27 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e97c03ba3e8494c9ba2cb5d8837cbdf9d4f38177151f3c344b5459888bc9a2af`  
		Last Modified: Thu, 09 Feb 2023 12:15:27 GMT  
		Size: 344.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; s390x

```console
$ docker pull spiped@sha256:6763f80ffafaec400a9c32713f12023d7cfc9221fe27ded8e22f7668b5695825
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.8 MB (34837535 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e585d1138d7b913b469d1d60a8169d148407b55e74a2ae2fa3670406899e2703`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 01 Mar 2023 02:50:30 GMT
ADD file:01aa3de7444f0716938e0d85522be065193be4ffb6788b3190a0f4fefdbb8d65 in / 
# Wed, 01 Mar 2023 02:50:31 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 09:59:36 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 01 Mar 2023 09:59:39 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 09:59:39 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 01 Mar 2023 09:59:51 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 01 Mar 2023 09:59:51 GMT
VOLUME [/spiped]
# Wed, 01 Mar 2023 09:59:52 GMT
WORKDIR /spiped
# Wed, 01 Mar 2023 09:59:52 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 01 Mar 2023 09:59:52 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 01 Mar 2023 09:59:52 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:7b8d78f42e32e7fa234bcf890ae6603acab2881bca68a9d8c429981c7f42b1d6`  
		Last Modified: Wed, 01 Mar 2023 02:54:48 GMT  
		Size: 29.6 MB (29646854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:407e05b7731593d7281e5af1c1859fd2d47d7464ad6c5dc03ac8c8155a85e98d`  
		Last Modified: Wed, 01 Mar 2023 10:00:28 GMT  
		Size: 1.7 KB (1738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74698444aa451ceea677ff79b9924fe3f417d089f80b716455e9685ecc1306cc`  
		Last Modified: Wed, 01 Mar 2023 10:00:28 GMT  
		Size: 1.1 KB (1055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1e70e3b82bb8b17253bfb319a8144075d6a620afff629c1d1ea44ed93fe7ae2`  
		Last Modified: Wed, 01 Mar 2023 10:00:29 GMT  
		Size: 5.2 MB (5187420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fc09ee195f0d0c9a66b36017beedcd1c8bb0eeed0bc93753b944e58a218b522`  
		Last Modified: Wed, 01 Mar 2023 10:00:28 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cb0d5fb8ca92c7b1a4e4c6943edcc6e6afba039da0f1f566df5c8f887bd2b17`  
		Last Modified: Wed, 01 Mar 2023 10:00:28 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:1-alpine`

```console
$ docker pull spiped@sha256:5e05424b596fce7f7efec601ad9f597fd7e2a724acb9b9b0d26adb4f7db2ab17
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
$ docker pull spiped@sha256:b02340eb97482a93ed8c3997880473f27309e7362e27d06bfbdeb686da9f835f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.1 MB (5080754 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1660f13550a5bd6ce0ec142f4dc1325092450163ee42f52b56572854d7e8c1e3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Sat, 11 Feb 2023 04:46:42 GMT
ADD file:40887ab7c06977737e63c215c9bd297c0c74de8d12d16ebdf1c3d40ac392f62d in / 
# Sat, 11 Feb 2023 04:46:42 GMT
CMD ["/bin/sh"]
# Sat, 11 Feb 2023 14:04:29 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Sat, 11 Feb 2023 14:04:30 GMT
RUN apk add --no-cache libssl1.1
# Sat, 11 Feb 2023 14:04:30 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Sat, 11 Feb 2023 14:04:41 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Sat, 11 Feb 2023 14:04:41 GMT
VOLUME [/spiped]
# Sat, 11 Feb 2023 14:04:41 GMT
WORKDIR /spiped
# Sat, 11 Feb 2023 14:04:41 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 11 Feb 2023 14:04:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 11 Feb 2023 14:04:41 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:63b65145d645c1250c391b2d16ebe53b3747c295ca8ba2fcb6b0cf064a4dc21c`  
		Last Modified: Fri, 10 Feb 2023 22:41:31 GMT  
		Size: 3.4 MB (3374446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1567e533de4a753157026d7ef2c42cfa5f9efd21e25cc7370e4c8f1c8f1c8a47`  
		Last Modified: Sat, 11 Feb 2023 14:04:56 GMT  
		Size: 1.3 KB (1267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1a1fcb595374972f69b5a50bd54f62b80c9214b0f891c62726a3fb6853cf855`  
		Last Modified: Sat, 11 Feb 2023 14:04:56 GMT  
		Size: 1.5 MB (1483289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24f4efb6e81c911655772824a287a9f39d90e069841b4fe5601933b9b0ffe154`  
		Last Modified: Sat, 11 Feb 2023 14:04:56 GMT  
		Size: 221.3 KB (221282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:981056191296cd6f887bc7d5e8e078e1cec12690bc7fc8623b868e6b4023e0ea`  
		Last Modified: Sat, 11 Feb 2023 14:04:56 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:577ef58b3b8b045fa02bbbbd599b6c9d4310c0039e442d91e549dad4f7e556fd`  
		Last Modified: Sat, 11 Feb 2023 14:04:56 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; arm variant v6

```console
$ docker pull spiped@sha256:db9fbdc8e95acdd61baed85bf52d7ab004cb17dee7aa0af49efb381048c748f6
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.6 MB (4559794 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d097d8022015b53fe69632c85f6ae24a781bdbbddb3e23b28bdcc34b321a5303`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 10 Feb 2023 20:49:28 GMT
ADD file:d825d9aef59df0df23c0140a490998407ee0a62a051699b5c050aef7cb03f042 in / 
# Fri, 10 Feb 2023 20:49:28 GMT
CMD ["/bin/sh"]
# Sat, 11 Feb 2023 07:32:24 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Sat, 11 Feb 2023 07:32:25 GMT
RUN apk add --no-cache libssl1.1
# Sat, 11 Feb 2023 07:32:26 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Sat, 11 Feb 2023 07:32:35 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Sat, 11 Feb 2023 07:32:35 GMT
VOLUME [/spiped]
# Sat, 11 Feb 2023 07:32:35 GMT
WORKDIR /spiped
# Sat, 11 Feb 2023 07:32:35 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 11 Feb 2023 07:32:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 11 Feb 2023 07:32:35 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:6a6e4ab63e54442e16400f69d37f662d60cbd67565631eff6bf59b4176e482c3`  
		Last Modified: Fri, 10 Feb 2023 20:50:22 GMT  
		Size: 3.1 MB (3110885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21e65df37e068288828fdd590c704bdba0ca4a8b9872083bdcf0ed938b05bc83`  
		Last Modified: Sat, 11 Feb 2023 07:32:55 GMT  
		Size: 1.2 KB (1242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e14f23472a8ad51e73644e312c9cb85c69854bc3f7259a3863b49c57f09c862`  
		Last Modified: Sat, 11 Feb 2023 07:32:55 GMT  
		Size: 1.2 MB (1240903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df3e94e7304b5459469fc8c8309989eaead5db21667861fb64669ab70d9611e9`  
		Last Modified: Sat, 11 Feb 2023 07:32:55 GMT  
		Size: 206.3 KB (206329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8025107e0a863a04d24b21f3bf9d1f737abc6459904039f3c55da02f034af97`  
		Last Modified: Sat, 11 Feb 2023 07:32:55 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54cb12d0c5007f92277b3cf5469ce48354a5168dca26644088636f1abd9146e9`  
		Last Modified: Sat, 11 Feb 2023 07:32:55 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; arm variant v7

```console
$ docker pull spiped@sha256:e20c83b0b32876e4a85b4fa0a62215f32ef4133754b1cf4f8aa23104887f1cf3
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4237781 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ef3949961d888a47f1cbebc6f1ef749422a6a62131094ad66325f33d8083c8a9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 10 Feb 2023 21:51:31 GMT
ADD file:143b601fcc6b5d7d95d3e5ccad3fec7081191a47e28d4f9294a7fb2499cab1af in / 
# Fri, 10 Feb 2023 21:51:31 GMT
CMD ["/bin/sh"]
# Sat, 11 Feb 2023 06:33:15 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Sat, 11 Feb 2023 06:33:17 GMT
RUN apk add --no-cache libssl1.1
# Sat, 11 Feb 2023 06:33:17 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Sat, 11 Feb 2023 06:33:25 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Sat, 11 Feb 2023 06:33:25 GMT
VOLUME [/spiped]
# Sat, 11 Feb 2023 06:33:25 GMT
WORKDIR /spiped
# Sat, 11 Feb 2023 06:33:25 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 11 Feb 2023 06:33:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 11 Feb 2023 06:33:25 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:6fb81ff47bd6d7db0ed86c9b951ad6417ec73ab60af6d22daa604076a902629c`  
		Last Modified: Fri, 10 Feb 2023 21:52:33 GMT  
		Size: 2.9 MB (2868494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a442f55d4c235667f33954aaf938a7f1714b8d21b2cb808fef9de382589b17e`  
		Last Modified: Sat, 11 Feb 2023 06:33:57 GMT  
		Size: 1.2 KB (1241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09b931fceacae9f7416c4568a8a29feed89107a70cdbb6a5a8e84402bc9006a9`  
		Last Modified: Sat, 11 Feb 2023 06:33:58 GMT  
		Size: 1.2 MB (1167516 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bf5fcf25622eedad4a8b76251c540101849957497e32f268e38fd74749854b2`  
		Last Modified: Sat, 11 Feb 2023 06:33:57 GMT  
		Size: 200.1 KB (200095 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62c1ab78ee707e97bbf4c7ee00e91010a5c9cc6e318131e29021a1a3f1a1b18b`  
		Last Modified: Sat, 11 Feb 2023 06:33:57 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d26766ccb2e9e7597f86a2c98d9e36433e85cc86b8bfed0d16175725ac4cae1`  
		Last Modified: Sat, 11 Feb 2023 06:33:57 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:b202c4e5897cb771f303b85871c6b7a1fb5f025c51e651b30a4415f0e2e4973d
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.8 MB (4842933 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6c3a0f714da4f343e79de4855fa4cdc4a23892d7fe5654dec6710bc79bb2cc2c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 10 Feb 2023 21:24:08 GMT
ADD file:9bd9ea42a9f3bdc769e80c6b8a4b117d65f73ae68e155a6172a1184e7ac8bcc1 in / 
# Fri, 10 Feb 2023 21:24:08 GMT
CMD ["/bin/sh"]
# Sat, 11 Feb 2023 06:39:43 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Sat, 11 Feb 2023 06:39:44 GMT
RUN apk add --no-cache libssl1.1
# Sat, 11 Feb 2023 06:39:44 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Sat, 11 Feb 2023 06:39:52 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Sat, 11 Feb 2023 06:39:52 GMT
VOLUME [/spiped]
# Sat, 11 Feb 2023 06:39:52 GMT
WORKDIR /spiped
# Sat, 11 Feb 2023 06:39:52 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 11 Feb 2023 06:39:52 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 11 Feb 2023 06:39:52 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:af6eaf76a39c2d3e7e0b8a0420486e3df33c4027d696c076a99a3d0ac09026af`  
		Last Modified: Fri, 10 Feb 2023 21:24:39 GMT  
		Size: 3.3 MB (3261959 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32e706a54c37c1524628e434965039ac738ff48a6f151dd2ef6da2cb49958cc0`  
		Last Modified: Sat, 11 Feb 2023 06:40:07 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e99781ddd302da37630cc491b5190c39c7867e6bd96556fad9f613e3411bca0d`  
		Last Modified: Sat, 11 Feb 2023 06:40:07 GMT  
		Size: 1.4 MB (1363548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:768a1af5c81e5cc877ea8cb330527a3924d5f2b5acfc5dd8239f84fdf091e5ed`  
		Last Modified: Sat, 11 Feb 2023 06:40:07 GMT  
		Size: 215.7 KB (215691 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7567bda17775002440a508f6ff25154cb13c9201175281b80186ce38d44e2b7`  
		Last Modified: Sat, 11 Feb 2023 06:40:07 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba17a7f3c3024db40a3e0b478318d1eb5168af1437c2bd502fb302591b78f95a`  
		Last Modified: Sat, 11 Feb 2023 06:40:07 GMT  
		Size: 338.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; 386

```console
$ docker pull spiped@sha256:822b81d156b7c387e1ceda5cee3e6a6edd3268187a6ce26e8b85df4c68e09f5d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.1 MB (5131561 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e4d91ebbd686f96b26164ad7739fcfca17552f6046e879f7ae2d57c3d3892739`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 10 Feb 2023 21:24:23 GMT
ADD file:125f3514520a5cd29df2830a409aa026a2bc06a77a7a5d150133436404b33d41 in / 
# Fri, 10 Feb 2023 21:24:24 GMT
CMD ["/bin/sh"]
# Sat, 11 Feb 2023 03:18:56 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Sat, 11 Feb 2023 03:18:58 GMT
RUN apk add --no-cache libssl1.1
# Sat, 11 Feb 2023 03:18:59 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Sat, 11 Feb 2023 03:19:10 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Sat, 11 Feb 2023 03:19:10 GMT
VOLUME [/spiped]
# Sat, 11 Feb 2023 03:19:11 GMT
WORKDIR /spiped
# Sat, 11 Feb 2023 03:19:13 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 11 Feb 2023 03:19:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 11 Feb 2023 03:19:14 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:b3e346c15c2377ec0e75cc9efa98baecd58b0e9bb92f0ec07eeda0bcc7e67fc7`  
		Last Modified: Fri, 10 Feb 2023 21:25:13 GMT  
		Size: 3.4 MB (3412353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c7d8401c5bd9906ab3609377e9ee6deadd5d9c4ae39ecfa8e9cd01ede0b8281`  
		Last Modified: Sat, 11 Feb 2023 03:19:39 GMT  
		Size: 1.2 KB (1241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:469cab1d7427d43462f6a9628be5d2ff81ee2cd0f9f7541f9539bc00c92429f7`  
		Last Modified: Sat, 11 Feb 2023 03:19:40 GMT  
		Size: 1.5 MB (1486162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:272b1229ae2f459eb6817fe20b02d6f823f26e1e8c76b8ac51eb8934b9143027`  
		Last Modified: Sat, 11 Feb 2023 03:19:39 GMT  
		Size: 231.4 KB (231370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb4adf5f9d6c3c73c3d7546a48714ef20383a01eeb6f321be386524c8e6e4212`  
		Last Modified: Sat, 11 Feb 2023 03:19:39 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35580a675ce6a64cc7a800a1f273d54f02d5e70f9b158be76b5a569da9cdb610`  
		Last Modified: Sat, 11 Feb 2023 03:19:39 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; ppc64le

```console
$ docker pull spiped@sha256:75c7e8ce27d4c68e8862a8e832409e09dbeb2c47fa2163ac0ac7f4e794b6b14c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.0 MB (5025550 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:523cfab6c09a42cd9174ca6dee237febe2f4a72f0c07628ccddab56278968150`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 10 Feb 2023 21:20:36 GMT
ADD file:ec037a0d4b462d12963ac20d9ec49bb73b4bcaf84d4bc7b364ebf93667e585b0 in / 
# Fri, 10 Feb 2023 21:20:36 GMT
CMD ["/bin/sh"]
# Sat, 11 Feb 2023 09:33:46 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Sat, 11 Feb 2023 09:33:49 GMT
RUN apk add --no-cache libssl1.1
# Sat, 11 Feb 2023 09:33:50 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Sat, 11 Feb 2023 09:34:04 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Sat, 11 Feb 2023 09:34:04 GMT
VOLUME [/spiped]
# Sat, 11 Feb 2023 09:34:05 GMT
WORKDIR /spiped
# Sat, 11 Feb 2023 09:34:05 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 11 Feb 2023 09:34:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 11 Feb 2023 09:34:06 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:aa3c56f9c6f127b6c8f628c95db165741ca400d19bdaef2752d80f093e47451e`  
		Last Modified: Fri, 10 Feb 2023 21:21:37 GMT  
		Size: 3.4 MB (3390750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b5d50df2303841e19f748472d51fac8d0695468f1d50516484905b50450aa48`  
		Last Modified: Sat, 11 Feb 2023 09:34:31 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0b54432b9107e6d87810bd116ab5112e27a1f713d4d2c06525f0ed14f102e3c`  
		Last Modified: Sat, 11 Feb 2023 09:34:32 GMT  
		Size: 1.4 MB (1413040 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4bda8ea646857e9e3d0c92c042261af7dba424338abfc7cc1c58eec7b8985be`  
		Last Modified: Sat, 11 Feb 2023 09:34:32 GMT  
		Size: 220.0 KB (220021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e33bc423b9fd5cc84d66be2c92fc2c78368e9b5553d8c6848fab3570115fb66`  
		Last Modified: Sat, 11 Feb 2023 09:34:31 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53a89c5ec31eae84c318581d292f2fdc24ec49bc7692940d54b3b579b04cd2d6`  
		Last Modified: Sat, 11 Feb 2023 09:34:31 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; s390x

```console
$ docker pull spiped@sha256:c224a59dd171160cb9e3b3be6bac31704ad968f23bed4f4f8ae4d04d938951c6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.6 MB (4608839 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:88032fe647cd1b9c54c93549e3978f1e53d8c0df71f2c0c2660b0545fc0b7ae3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 10 Feb 2023 21:41:25 GMT
ADD file:03b2fb4d732a294329449ff55c5d84f7d2735e6510985718979469994f3a607b in / 
# Fri, 10 Feb 2023 21:41:26 GMT
CMD ["/bin/sh"]
# Sat, 11 Feb 2023 05:20:31 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Sat, 11 Feb 2023 05:20:32 GMT
RUN apk add --no-cache libssl1.1
# Sat, 11 Feb 2023 05:20:33 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Sat, 11 Feb 2023 05:20:38 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Sat, 11 Feb 2023 05:20:38 GMT
VOLUME [/spiped]
# Sat, 11 Feb 2023 05:20:38 GMT
WORKDIR /spiped
# Sat, 11 Feb 2023 05:20:39 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 11 Feb 2023 05:20:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 11 Feb 2023 05:20:39 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:24c4f8de3549a39c64b0edc2cfa68769b373f35138d0f13725100160bb32d4e2`  
		Last Modified: Fri, 10 Feb 2023 21:42:16 GMT  
		Size: 3.2 MB (3175116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdb5c0ff1110b4315355f81e38de10bb31ba9fe44d99d3b7598f20a28f2c98e1`  
		Last Modified: Sat, 11 Feb 2023 05:21:04 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9ac27252903c2b21737926a9cd0721ecfa3aba4f2e52da7f7c114aea4da62df`  
		Last Modified: Sat, 11 Feb 2023 05:21:04 GMT  
		Size: 1.2 MB (1223356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df30f40ce9a4931562f50ea55d6450396fd443fed95a0b2c0ea337f53f22ec25`  
		Last Modified: Sat, 11 Feb 2023 05:21:04 GMT  
		Size: 208.6 KB (208631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d9420167a9c04b73e787d02b0fa09ba21ff8b27917d0406146f9bc5a0df3034`  
		Last Modified: Sat, 11 Feb 2023 05:21:04 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea129f4350d878551c457a2192ea0570f86ca7ee5c193a6b0d8e19727570f05b`  
		Last Modified: Sat, 11 Feb 2023 05:21:04 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:1.6`

```console
$ docker pull spiped@sha256:dcd50fdfd27ec8f055329f6100c9237808b11c01a4605564877a8e91c2e240a2
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
$ docker pull spiped@sha256:65d1de8326124f7025322cdba5f11590bf65237b0cb63f400e388e7ec598f533
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.4 MB (37413302 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2e6f8b4beac2d2177806929f949e4e7ae5eca9086100ed06f9464b8f863786ed`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 09 Feb 2023 03:20:20 GMT
ADD file:3ea7c69e4bfac2ebb6f86baaedab31827c86a594dba8080a49928e211ad3c7a0 in / 
# Thu, 09 Feb 2023 03:20:20 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 06:37:17 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Thu, 09 Feb 2023 06:37:20 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 06:37:20 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 09 Feb 2023 06:37:40 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 09 Feb 2023 06:37:41 GMT
VOLUME [/spiped]
# Thu, 09 Feb 2023 06:37:41 GMT
WORKDIR /spiped
# Thu, 09 Feb 2023 06:37:41 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 09 Feb 2023 06:37:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 09 Feb 2023 06:37:41 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:bb263680fed18eecdc67f885094df6f589bafc19004839d7fdf141df236a61aa`  
		Last Modified: Thu, 09 Feb 2023 03:25:13 GMT  
		Size: 31.4 MB (31411810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:904147bf2f8667febed21ce347ecd042f5b9d779a1ac552bd4055ec2d7f060b6`  
		Last Modified: Thu, 09 Feb 2023 06:37:56 GMT  
		Size: 1.7 KB (1737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa73821f4c111ea10583bad55bd382aa4196e36aeca4093bf6ad2e4f27565fb4`  
		Last Modified: Thu, 09 Feb 2023 06:37:56 GMT  
		Size: 1.0 KB (1049 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccbe509202f24ed422baf731f3dd79e740b358183ad10a4d7554c5260d1f74cb`  
		Last Modified: Thu, 09 Feb 2023 06:37:57 GMT  
		Size: 6.0 MB (5998234 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9b81852413d69c15590cca8a24757c58e49244b108abaa2f57a3173de23700a`  
		Last Modified: Thu, 09 Feb 2023 06:37:56 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:714d39b5611de4a84c8a690342eb12e7f1f27cbc13ebfa1aa2d40e6db8e79031`  
		Last Modified: Thu, 09 Feb 2023 06:37:56 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; arm variant v5

```console
$ docker pull spiped@sha256:528e13ba139adf0768024a80cfc79ab5cb3d0ea5e8f9b9f3bc1511f2d698c215
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.9 MB (33947393 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5a1e48f7b0e65652cca9ca80196c861d383ac1f1b0103cc512be95efd00fc6e9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 01 Mar 2023 01:48:54 GMT
ADD file:b4fb1081f6eb8a0560d56d5781bbcedaac1453615d56e0943245dca784785ea2 in / 
# Wed, 01 Mar 2023 01:48:54 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 07:10:40 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 01 Mar 2023 07:10:44 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 07:10:44 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 01 Mar 2023 07:11:03 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 01 Mar 2023 07:11:03 GMT
VOLUME [/spiped]
# Wed, 01 Mar 2023 07:11:03 GMT
WORKDIR /spiped
# Wed, 01 Mar 2023 07:11:03 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 01 Mar 2023 07:11:03 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 01 Mar 2023 07:11:04 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:3c3af56dbec5913ef8aec0f1ca7112eb5914b4ad346ccd48f836dd7ec0621ba5`  
		Last Modified: Wed, 01 Mar 2023 01:52:57 GMT  
		Size: 28.9 MB (28915776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9aca7d992b566279fbac9ecdeffb9ff2db68cf1ffd6f31a2cce852311c28c5ce`  
		Last Modified: Wed, 01 Mar 2023 07:11:20 GMT  
		Size: 1.7 KB (1728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fc3eb64d155ea643dfc7dde1104693192a95033b812f1cf66e286245705de6f`  
		Last Modified: Wed, 01 Mar 2023 07:11:20 GMT  
		Size: 1.1 KB (1050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9169ad29c4b57b416977f34e4cae1ad9b4efb6110e2a150a7cb43b7eab0da3d3`  
		Last Modified: Wed, 01 Mar 2023 07:11:21 GMT  
		Size: 5.0 MB (5028368 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:742f87e7cb263314cfe9b69a92b5fef45b368e04c178942b699311a03503e14c`  
		Last Modified: Wed, 01 Mar 2023 07:11:20 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0dfe2f008531a4616c872689c583cd0c8468b2fb60b07981fc0e20a80f84497`  
		Last Modified: Wed, 01 Mar 2023 07:11:20 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; arm variant v7

```console
$ docker pull spiped@sha256:7017eb815f7e60e8ff5b15b21fe0cbd2ef33396feebd8f7f18bcfd82efcbcdca
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.3 MB (31329871 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5b689ef4b4dc24e15c83f0188d2896b65dfb8ab55d95974313cbac1be6f13df4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 09 Feb 2023 06:12:09 GMT
ADD file:5f1a343224e8486690bd90dd1e50c8d84b3d770c51bb6829544e5cf650c0419c in / 
# Thu, 09 Feb 2023 06:12:10 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 12:59:21 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Thu, 09 Feb 2023 12:59:25 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 12:59:25 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 09 Feb 2023 12:59:43 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 09 Feb 2023 12:59:43 GMT
VOLUME [/spiped]
# Thu, 09 Feb 2023 12:59:43 GMT
WORKDIR /spiped
# Thu, 09 Feb 2023 12:59:44 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 09 Feb 2023 12:59:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 09 Feb 2023 12:59:44 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:e7318f6106ad75d7d482ae9dddf4d927b0872ef3ddb6e1330aa691fc8d17279e`  
		Last Modified: Thu, 09 Feb 2023 06:19:19 GMT  
		Size: 26.6 MB (26577666 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e00b17d2d80b94e1a46f2bf36d6bc77f847e4cd57083ecbb8f84ad55d31d164a`  
		Last Modified: Thu, 09 Feb 2023 13:00:24 GMT  
		Size: 1.7 KB (1730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7293faff8274bf27a2e47ec70c06f8ab91fac589d357fdd3306a81ec075c3fb`  
		Last Modified: Thu, 09 Feb 2023 13:00:24 GMT  
		Size: 1.0 KB (1022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:420c029d7a4f8d85dc09d4d90250267b2137b15106d2fe5623c195ee79fcda5f`  
		Last Modified: Thu, 09 Feb 2023 13:00:27 GMT  
		Size: 4.7 MB (4749016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a8f996daf79da4e6f40d919b8671e3c4b55085710edea0584ea9f11b834bcce`  
		Last Modified: Thu, 09 Feb 2023 13:00:24 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef6016c3c267a148094099843a4bc93c8dc6f172510f577193c40ec9772fa0de`  
		Last Modified: Thu, 09 Feb 2023 13:00:24 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:ba65bbd88dad033e812d648ab5bec4670067246f6c0ff39ae8413e1bbb54b8ce
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.3 MB (35338340 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:40a101e61165070db066921b2c5822a0f2771bfce3632b8b52055fa79ff1a4f8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 09 Feb 2023 03:58:40 GMT
ADD file:3276ac85bb957360f20720da5b37498a6b5f91a017046049f8d2fd791f728a9a in / 
# Thu, 09 Feb 2023 03:58:40 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 08:54:18 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Thu, 09 Feb 2023 08:54:20 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 08:54:20 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 09 Feb 2023 08:54:35 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 09 Feb 2023 08:54:35 GMT
VOLUME [/spiped]
# Thu, 09 Feb 2023 08:54:35 GMT
WORKDIR /spiped
# Thu, 09 Feb 2023 08:54:35 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 09 Feb 2023 08:54:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 09 Feb 2023 08:54:35 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:5731adb3a4abcefe78d75783ea6e5ee87c4604d0c6a4f8c00b50085e162a7f5d`  
		Last Modified: Thu, 09 Feb 2023 04:02:34 GMT  
		Size: 30.1 MB (30062509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8137aa16a21880e530299f722a06622e5b58e5e7096c84fab419a159a7f04091`  
		Last Modified: Thu, 09 Feb 2023 08:54:53 GMT  
		Size: 1.7 KB (1739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2c2269b7f42a74f4a740b49267f4eaed378968aa33615a2a203cb15bc9360c2`  
		Last Modified: Thu, 09 Feb 2023 08:54:54 GMT  
		Size: 1.1 KB (1050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:052457e7f7a0e19dcaacf826e2ca00910c21085d12529627fd618e0d211863de`  
		Last Modified: Thu, 09 Feb 2023 08:54:54 GMT  
		Size: 5.3 MB (5272569 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17ae4ac2dc94d44f270d10320f3a8a057ae7af3d45f1ecf9c808b9a95cde305d`  
		Last Modified: Thu, 09 Feb 2023 08:54:53 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56ed7bfb7f7c49224f53d54b2d403c5be43966bc94394495d4104501b4129c1f`  
		Last Modified: Thu, 09 Feb 2023 08:54:53 GMT  
		Size: 344.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; 386

```console
$ docker pull spiped@sha256:bfa78a9926e73b519ea52984757a09e911d14c2bd9da1ab55972bd9ce2cf2d65
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.3 MB (40290432 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b6568369d320f09cd292f11fd201b8dca3a8cd63acb3bee3c7bb677d1a6a9eb5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 09 Feb 2023 05:12:53 GMT
ADD file:7740abd3129d33122ce51153c0b6c3323b9cbe9ea0e81672e16b2d7b210d24e3 in / 
# Thu, 09 Feb 2023 05:12:53 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 11:27:18 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Thu, 09 Feb 2023 11:27:22 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 11:27:23 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 09 Feb 2023 11:27:44 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 09 Feb 2023 11:27:44 GMT
VOLUME [/spiped]
# Thu, 09 Feb 2023 11:27:45 GMT
WORKDIR /spiped
# Thu, 09 Feb 2023 11:27:47 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 09 Feb 2023 11:27:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 09 Feb 2023 11:27:48 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:20744f4988404b1dee2cd438157b288d16a89da472583c0f04332ed389b258f8`  
		Last Modified: Thu, 09 Feb 2023 05:18:42 GMT  
		Size: 32.4 MB (32396875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37e01fd7049f58e3cf43b9c079e4da2f2b953c4792ee00e77aa6bea9acc10bb6`  
		Last Modified: Thu, 09 Feb 2023 11:28:15 GMT  
		Size: 1.6 KB (1614 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf141110ec25cbcd6fba0b5455ec049cbd33a0c16c1c8374a6b55c49c44290c4`  
		Last Modified: Thu, 09 Feb 2023 11:28:16 GMT  
		Size: 926.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c620d26def5e122b57324d22b9be7126f1aff0ee2808938cbaed2c0188aafe12`  
		Last Modified: Thu, 09 Feb 2023 11:28:17 GMT  
		Size: 7.9 MB (7890579 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b03b58be7cfa61363c0156f3f24fa50f0f503e6b2919c0a00abddbedd7764eda`  
		Last Modified: Thu, 09 Feb 2023 11:28:15 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe17e554449880852355124c22a61e8bcd828562f361f183b7096cbe1cd21a09`  
		Last Modified: Thu, 09 Feb 2023 11:28:15 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; mips64le

```console
$ docker pull spiped@sha256:b2ffe0253c458c187dd8728de9223a1a801ced3878b3304a43e6bb2d6708fd52
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.3 MB (35342689 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:71b26a2c72965d659a81b09281cdf469a7aaceeb51fa5a05e5f25152bfb18426`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 09 Feb 2023 02:45:21 GMT
ADD file:68e11645a37c49c8f8f9d79ba579d0d192aaab78bb28059f07d69d56aa5ace71 in / 
# Thu, 09 Feb 2023 02:45:25 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 09:28:59 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Thu, 09 Feb 2023 09:29:14 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 09:29:16 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 09 Feb 2023 09:30:45 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 09 Feb 2023 09:30:47 GMT
VOLUME [/spiped]
# Thu, 09 Feb 2023 09:30:50 GMT
WORKDIR /spiped
# Thu, 09 Feb 2023 09:30:52 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 09 Feb 2023 09:30:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 09 Feb 2023 09:30:58 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:1b5516936229d6629ab88588210eb90edc2613c94e5952fd1caf9200284f298a`  
		Last Modified: Thu, 09 Feb 2023 02:53:48 GMT  
		Size: 29.6 MB (29634449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3441e9678cbfa1a300965eb223fd19537d15afa6185479f02efb9549b6f90356`  
		Last Modified: Thu, 09 Feb 2023 09:31:13 GMT  
		Size: 1.6 KB (1619 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b9dda8c314f6a9f00c80e8d3774028d4204d754e4c828c2c38917e39f649706`  
		Last Modified: Thu, 09 Feb 2023 09:31:13 GMT  
		Size: 926.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed7b5d79a1e160a892ae3ca9a3585b9a3859b3843800b146b50a6f8dc2e37cea`  
		Last Modified: Thu, 09 Feb 2023 09:31:18 GMT  
		Size: 5.7 MB (5705255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e3972972765aa157621d8d380622fd6d29b61d44fd1b960930a1847ba23bfbb`  
		Last Modified: Thu, 09 Feb 2023 09:31:13 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc249832f7bdc107bfaebf38fb0292b7cacb7518cba7bad019f0d8ff699994c4`  
		Last Modified: Thu, 09 Feb 2023 09:31:13 GMT  
		Size: 345.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; ppc64le

```console
$ docker pull spiped@sha256:c55bb97521e65594872fe76cbfbc246cf4f6f31b3851f51ee61256ba623233de
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.3 MB (41292154 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2584a0abea40abb2a074488d4046bfa1ee2358d7221dcaada6120144742c42a9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 09 Feb 2023 06:21:49 GMT
ADD file:b09577b8131a90731fdfb00b824a97dc65ccb51d484cb9004382035d64a5741c in / 
# Thu, 09 Feb 2023 06:21:52 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 12:13:54 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Thu, 09 Feb 2023 12:14:00 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 12:14:00 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 09 Feb 2023 12:14:49 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 09 Feb 2023 12:14:50 GMT
VOLUME [/spiped]
# Thu, 09 Feb 2023 12:14:50 GMT
WORKDIR /spiped
# Thu, 09 Feb 2023 12:14:51 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 09 Feb 2023 12:14:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 09 Feb 2023 12:14:52 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:4ea90e1a094ae86c7950bbec99e7a79b08fae641ad5f3bc3af9081c925894c41`  
		Last Modified: Thu, 09 Feb 2023 06:28:27 GMT  
		Size: 35.3 MB (35289252 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:695fd45ccd8eac48da176341bba34201c9b8980634c1df9e9e8b4bfbfa220edc`  
		Last Modified: Thu, 09 Feb 2023 12:15:27 GMT  
		Size: 1.7 KB (1735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e02fb49a13103590e46d389b8e81a60bc1d01cbf4395c01b053e5e4e99f6e312`  
		Last Modified: Thu, 09 Feb 2023 12:15:27 GMT  
		Size: 1.0 KB (1049 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e9885ddc7088b14facf6e088ded644fc33dff7b4e6625a92eb87f71975a0703`  
		Last Modified: Thu, 09 Feb 2023 12:15:29 GMT  
		Size: 6.0 MB (5999645 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:300eee5c0fb43c90cd5a5c063707252fce74ce3a8ffc7fcd444c165dfb9753a9`  
		Last Modified: Thu, 09 Feb 2023 12:15:27 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e97c03ba3e8494c9ba2cb5d8837cbdf9d4f38177151f3c344b5459888bc9a2af`  
		Last Modified: Thu, 09 Feb 2023 12:15:27 GMT  
		Size: 344.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; s390x

```console
$ docker pull spiped@sha256:6763f80ffafaec400a9c32713f12023d7cfc9221fe27ded8e22f7668b5695825
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.8 MB (34837535 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e585d1138d7b913b469d1d60a8169d148407b55e74a2ae2fa3670406899e2703`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 01 Mar 2023 02:50:30 GMT
ADD file:01aa3de7444f0716938e0d85522be065193be4ffb6788b3190a0f4fefdbb8d65 in / 
# Wed, 01 Mar 2023 02:50:31 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 09:59:36 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 01 Mar 2023 09:59:39 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 09:59:39 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 01 Mar 2023 09:59:51 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 01 Mar 2023 09:59:51 GMT
VOLUME [/spiped]
# Wed, 01 Mar 2023 09:59:52 GMT
WORKDIR /spiped
# Wed, 01 Mar 2023 09:59:52 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 01 Mar 2023 09:59:52 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 01 Mar 2023 09:59:52 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:7b8d78f42e32e7fa234bcf890ae6603acab2881bca68a9d8c429981c7f42b1d6`  
		Last Modified: Wed, 01 Mar 2023 02:54:48 GMT  
		Size: 29.6 MB (29646854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:407e05b7731593d7281e5af1c1859fd2d47d7464ad6c5dc03ac8c8155a85e98d`  
		Last Modified: Wed, 01 Mar 2023 10:00:28 GMT  
		Size: 1.7 KB (1738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74698444aa451ceea677ff79b9924fe3f417d089f80b716455e9685ecc1306cc`  
		Last Modified: Wed, 01 Mar 2023 10:00:28 GMT  
		Size: 1.1 KB (1055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1e70e3b82bb8b17253bfb319a8144075d6a620afff629c1d1ea44ed93fe7ae2`  
		Last Modified: Wed, 01 Mar 2023 10:00:29 GMT  
		Size: 5.2 MB (5187420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fc09ee195f0d0c9a66b36017beedcd1c8bb0eeed0bc93753b944e58a218b522`  
		Last Modified: Wed, 01 Mar 2023 10:00:28 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cb0d5fb8ca92c7b1a4e4c6943edcc6e6afba039da0f1f566df5c8f887bd2b17`  
		Last Modified: Wed, 01 Mar 2023 10:00:28 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:1.6-alpine`

```console
$ docker pull spiped@sha256:5e05424b596fce7f7efec601ad9f597fd7e2a724acb9b9b0d26adb4f7db2ab17
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
$ docker pull spiped@sha256:b02340eb97482a93ed8c3997880473f27309e7362e27d06bfbdeb686da9f835f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.1 MB (5080754 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1660f13550a5bd6ce0ec142f4dc1325092450163ee42f52b56572854d7e8c1e3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Sat, 11 Feb 2023 04:46:42 GMT
ADD file:40887ab7c06977737e63c215c9bd297c0c74de8d12d16ebdf1c3d40ac392f62d in / 
# Sat, 11 Feb 2023 04:46:42 GMT
CMD ["/bin/sh"]
# Sat, 11 Feb 2023 14:04:29 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Sat, 11 Feb 2023 14:04:30 GMT
RUN apk add --no-cache libssl1.1
# Sat, 11 Feb 2023 14:04:30 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Sat, 11 Feb 2023 14:04:41 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Sat, 11 Feb 2023 14:04:41 GMT
VOLUME [/spiped]
# Sat, 11 Feb 2023 14:04:41 GMT
WORKDIR /spiped
# Sat, 11 Feb 2023 14:04:41 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 11 Feb 2023 14:04:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 11 Feb 2023 14:04:41 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:63b65145d645c1250c391b2d16ebe53b3747c295ca8ba2fcb6b0cf064a4dc21c`  
		Last Modified: Fri, 10 Feb 2023 22:41:31 GMT  
		Size: 3.4 MB (3374446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1567e533de4a753157026d7ef2c42cfa5f9efd21e25cc7370e4c8f1c8f1c8a47`  
		Last Modified: Sat, 11 Feb 2023 14:04:56 GMT  
		Size: 1.3 KB (1267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1a1fcb595374972f69b5a50bd54f62b80c9214b0f891c62726a3fb6853cf855`  
		Last Modified: Sat, 11 Feb 2023 14:04:56 GMT  
		Size: 1.5 MB (1483289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24f4efb6e81c911655772824a287a9f39d90e069841b4fe5601933b9b0ffe154`  
		Last Modified: Sat, 11 Feb 2023 14:04:56 GMT  
		Size: 221.3 KB (221282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:981056191296cd6f887bc7d5e8e078e1cec12690bc7fc8623b868e6b4023e0ea`  
		Last Modified: Sat, 11 Feb 2023 14:04:56 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:577ef58b3b8b045fa02bbbbd599b6c9d4310c0039e442d91e549dad4f7e556fd`  
		Last Modified: Sat, 11 Feb 2023 14:04:56 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; arm variant v6

```console
$ docker pull spiped@sha256:db9fbdc8e95acdd61baed85bf52d7ab004cb17dee7aa0af49efb381048c748f6
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.6 MB (4559794 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d097d8022015b53fe69632c85f6ae24a781bdbbddb3e23b28bdcc34b321a5303`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 10 Feb 2023 20:49:28 GMT
ADD file:d825d9aef59df0df23c0140a490998407ee0a62a051699b5c050aef7cb03f042 in / 
# Fri, 10 Feb 2023 20:49:28 GMT
CMD ["/bin/sh"]
# Sat, 11 Feb 2023 07:32:24 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Sat, 11 Feb 2023 07:32:25 GMT
RUN apk add --no-cache libssl1.1
# Sat, 11 Feb 2023 07:32:26 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Sat, 11 Feb 2023 07:32:35 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Sat, 11 Feb 2023 07:32:35 GMT
VOLUME [/spiped]
# Sat, 11 Feb 2023 07:32:35 GMT
WORKDIR /spiped
# Sat, 11 Feb 2023 07:32:35 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 11 Feb 2023 07:32:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 11 Feb 2023 07:32:35 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:6a6e4ab63e54442e16400f69d37f662d60cbd67565631eff6bf59b4176e482c3`  
		Last Modified: Fri, 10 Feb 2023 20:50:22 GMT  
		Size: 3.1 MB (3110885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21e65df37e068288828fdd590c704bdba0ca4a8b9872083bdcf0ed938b05bc83`  
		Last Modified: Sat, 11 Feb 2023 07:32:55 GMT  
		Size: 1.2 KB (1242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e14f23472a8ad51e73644e312c9cb85c69854bc3f7259a3863b49c57f09c862`  
		Last Modified: Sat, 11 Feb 2023 07:32:55 GMT  
		Size: 1.2 MB (1240903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df3e94e7304b5459469fc8c8309989eaead5db21667861fb64669ab70d9611e9`  
		Last Modified: Sat, 11 Feb 2023 07:32:55 GMT  
		Size: 206.3 KB (206329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8025107e0a863a04d24b21f3bf9d1f737abc6459904039f3c55da02f034af97`  
		Last Modified: Sat, 11 Feb 2023 07:32:55 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54cb12d0c5007f92277b3cf5469ce48354a5168dca26644088636f1abd9146e9`  
		Last Modified: Sat, 11 Feb 2023 07:32:55 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; arm variant v7

```console
$ docker pull spiped@sha256:e20c83b0b32876e4a85b4fa0a62215f32ef4133754b1cf4f8aa23104887f1cf3
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4237781 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ef3949961d888a47f1cbebc6f1ef749422a6a62131094ad66325f33d8083c8a9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 10 Feb 2023 21:51:31 GMT
ADD file:143b601fcc6b5d7d95d3e5ccad3fec7081191a47e28d4f9294a7fb2499cab1af in / 
# Fri, 10 Feb 2023 21:51:31 GMT
CMD ["/bin/sh"]
# Sat, 11 Feb 2023 06:33:15 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Sat, 11 Feb 2023 06:33:17 GMT
RUN apk add --no-cache libssl1.1
# Sat, 11 Feb 2023 06:33:17 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Sat, 11 Feb 2023 06:33:25 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Sat, 11 Feb 2023 06:33:25 GMT
VOLUME [/spiped]
# Sat, 11 Feb 2023 06:33:25 GMT
WORKDIR /spiped
# Sat, 11 Feb 2023 06:33:25 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 11 Feb 2023 06:33:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 11 Feb 2023 06:33:25 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:6fb81ff47bd6d7db0ed86c9b951ad6417ec73ab60af6d22daa604076a902629c`  
		Last Modified: Fri, 10 Feb 2023 21:52:33 GMT  
		Size: 2.9 MB (2868494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a442f55d4c235667f33954aaf938a7f1714b8d21b2cb808fef9de382589b17e`  
		Last Modified: Sat, 11 Feb 2023 06:33:57 GMT  
		Size: 1.2 KB (1241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09b931fceacae9f7416c4568a8a29feed89107a70cdbb6a5a8e84402bc9006a9`  
		Last Modified: Sat, 11 Feb 2023 06:33:58 GMT  
		Size: 1.2 MB (1167516 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bf5fcf25622eedad4a8b76251c540101849957497e32f268e38fd74749854b2`  
		Last Modified: Sat, 11 Feb 2023 06:33:57 GMT  
		Size: 200.1 KB (200095 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62c1ab78ee707e97bbf4c7ee00e91010a5c9cc6e318131e29021a1a3f1a1b18b`  
		Last Modified: Sat, 11 Feb 2023 06:33:57 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d26766ccb2e9e7597f86a2c98d9e36433e85cc86b8bfed0d16175725ac4cae1`  
		Last Modified: Sat, 11 Feb 2023 06:33:57 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:b202c4e5897cb771f303b85871c6b7a1fb5f025c51e651b30a4415f0e2e4973d
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.8 MB (4842933 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6c3a0f714da4f343e79de4855fa4cdc4a23892d7fe5654dec6710bc79bb2cc2c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 10 Feb 2023 21:24:08 GMT
ADD file:9bd9ea42a9f3bdc769e80c6b8a4b117d65f73ae68e155a6172a1184e7ac8bcc1 in / 
# Fri, 10 Feb 2023 21:24:08 GMT
CMD ["/bin/sh"]
# Sat, 11 Feb 2023 06:39:43 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Sat, 11 Feb 2023 06:39:44 GMT
RUN apk add --no-cache libssl1.1
# Sat, 11 Feb 2023 06:39:44 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Sat, 11 Feb 2023 06:39:52 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Sat, 11 Feb 2023 06:39:52 GMT
VOLUME [/spiped]
# Sat, 11 Feb 2023 06:39:52 GMT
WORKDIR /spiped
# Sat, 11 Feb 2023 06:39:52 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 11 Feb 2023 06:39:52 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 11 Feb 2023 06:39:52 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:af6eaf76a39c2d3e7e0b8a0420486e3df33c4027d696c076a99a3d0ac09026af`  
		Last Modified: Fri, 10 Feb 2023 21:24:39 GMT  
		Size: 3.3 MB (3261959 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32e706a54c37c1524628e434965039ac738ff48a6f151dd2ef6da2cb49958cc0`  
		Last Modified: Sat, 11 Feb 2023 06:40:07 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e99781ddd302da37630cc491b5190c39c7867e6bd96556fad9f613e3411bca0d`  
		Last Modified: Sat, 11 Feb 2023 06:40:07 GMT  
		Size: 1.4 MB (1363548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:768a1af5c81e5cc877ea8cb330527a3924d5f2b5acfc5dd8239f84fdf091e5ed`  
		Last Modified: Sat, 11 Feb 2023 06:40:07 GMT  
		Size: 215.7 KB (215691 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7567bda17775002440a508f6ff25154cb13c9201175281b80186ce38d44e2b7`  
		Last Modified: Sat, 11 Feb 2023 06:40:07 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba17a7f3c3024db40a3e0b478318d1eb5168af1437c2bd502fb302591b78f95a`  
		Last Modified: Sat, 11 Feb 2023 06:40:07 GMT  
		Size: 338.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; 386

```console
$ docker pull spiped@sha256:822b81d156b7c387e1ceda5cee3e6a6edd3268187a6ce26e8b85df4c68e09f5d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.1 MB (5131561 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e4d91ebbd686f96b26164ad7739fcfca17552f6046e879f7ae2d57c3d3892739`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 10 Feb 2023 21:24:23 GMT
ADD file:125f3514520a5cd29df2830a409aa026a2bc06a77a7a5d150133436404b33d41 in / 
# Fri, 10 Feb 2023 21:24:24 GMT
CMD ["/bin/sh"]
# Sat, 11 Feb 2023 03:18:56 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Sat, 11 Feb 2023 03:18:58 GMT
RUN apk add --no-cache libssl1.1
# Sat, 11 Feb 2023 03:18:59 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Sat, 11 Feb 2023 03:19:10 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Sat, 11 Feb 2023 03:19:10 GMT
VOLUME [/spiped]
# Sat, 11 Feb 2023 03:19:11 GMT
WORKDIR /spiped
# Sat, 11 Feb 2023 03:19:13 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 11 Feb 2023 03:19:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 11 Feb 2023 03:19:14 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:b3e346c15c2377ec0e75cc9efa98baecd58b0e9bb92f0ec07eeda0bcc7e67fc7`  
		Last Modified: Fri, 10 Feb 2023 21:25:13 GMT  
		Size: 3.4 MB (3412353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c7d8401c5bd9906ab3609377e9ee6deadd5d9c4ae39ecfa8e9cd01ede0b8281`  
		Last Modified: Sat, 11 Feb 2023 03:19:39 GMT  
		Size: 1.2 KB (1241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:469cab1d7427d43462f6a9628be5d2ff81ee2cd0f9f7541f9539bc00c92429f7`  
		Last Modified: Sat, 11 Feb 2023 03:19:40 GMT  
		Size: 1.5 MB (1486162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:272b1229ae2f459eb6817fe20b02d6f823f26e1e8c76b8ac51eb8934b9143027`  
		Last Modified: Sat, 11 Feb 2023 03:19:39 GMT  
		Size: 231.4 KB (231370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb4adf5f9d6c3c73c3d7546a48714ef20383a01eeb6f321be386524c8e6e4212`  
		Last Modified: Sat, 11 Feb 2023 03:19:39 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35580a675ce6a64cc7a800a1f273d54f02d5e70f9b158be76b5a569da9cdb610`  
		Last Modified: Sat, 11 Feb 2023 03:19:39 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; ppc64le

```console
$ docker pull spiped@sha256:75c7e8ce27d4c68e8862a8e832409e09dbeb2c47fa2163ac0ac7f4e794b6b14c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.0 MB (5025550 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:523cfab6c09a42cd9174ca6dee237febe2f4a72f0c07628ccddab56278968150`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 10 Feb 2023 21:20:36 GMT
ADD file:ec037a0d4b462d12963ac20d9ec49bb73b4bcaf84d4bc7b364ebf93667e585b0 in / 
# Fri, 10 Feb 2023 21:20:36 GMT
CMD ["/bin/sh"]
# Sat, 11 Feb 2023 09:33:46 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Sat, 11 Feb 2023 09:33:49 GMT
RUN apk add --no-cache libssl1.1
# Sat, 11 Feb 2023 09:33:50 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Sat, 11 Feb 2023 09:34:04 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Sat, 11 Feb 2023 09:34:04 GMT
VOLUME [/spiped]
# Sat, 11 Feb 2023 09:34:05 GMT
WORKDIR /spiped
# Sat, 11 Feb 2023 09:34:05 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 11 Feb 2023 09:34:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 11 Feb 2023 09:34:06 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:aa3c56f9c6f127b6c8f628c95db165741ca400d19bdaef2752d80f093e47451e`  
		Last Modified: Fri, 10 Feb 2023 21:21:37 GMT  
		Size: 3.4 MB (3390750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b5d50df2303841e19f748472d51fac8d0695468f1d50516484905b50450aa48`  
		Last Modified: Sat, 11 Feb 2023 09:34:31 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0b54432b9107e6d87810bd116ab5112e27a1f713d4d2c06525f0ed14f102e3c`  
		Last Modified: Sat, 11 Feb 2023 09:34:32 GMT  
		Size: 1.4 MB (1413040 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4bda8ea646857e9e3d0c92c042261af7dba424338abfc7cc1c58eec7b8985be`  
		Last Modified: Sat, 11 Feb 2023 09:34:32 GMT  
		Size: 220.0 KB (220021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e33bc423b9fd5cc84d66be2c92fc2c78368e9b5553d8c6848fab3570115fb66`  
		Last Modified: Sat, 11 Feb 2023 09:34:31 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53a89c5ec31eae84c318581d292f2fdc24ec49bc7692940d54b3b579b04cd2d6`  
		Last Modified: Sat, 11 Feb 2023 09:34:31 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; s390x

```console
$ docker pull spiped@sha256:c224a59dd171160cb9e3b3be6bac31704ad968f23bed4f4f8ae4d04d938951c6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.6 MB (4608839 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:88032fe647cd1b9c54c93549e3978f1e53d8c0df71f2c0c2660b0545fc0b7ae3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 10 Feb 2023 21:41:25 GMT
ADD file:03b2fb4d732a294329449ff55c5d84f7d2735e6510985718979469994f3a607b in / 
# Fri, 10 Feb 2023 21:41:26 GMT
CMD ["/bin/sh"]
# Sat, 11 Feb 2023 05:20:31 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Sat, 11 Feb 2023 05:20:32 GMT
RUN apk add --no-cache libssl1.1
# Sat, 11 Feb 2023 05:20:33 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Sat, 11 Feb 2023 05:20:38 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Sat, 11 Feb 2023 05:20:38 GMT
VOLUME [/spiped]
# Sat, 11 Feb 2023 05:20:38 GMT
WORKDIR /spiped
# Sat, 11 Feb 2023 05:20:39 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 11 Feb 2023 05:20:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 11 Feb 2023 05:20:39 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:24c4f8de3549a39c64b0edc2cfa68769b373f35138d0f13725100160bb32d4e2`  
		Last Modified: Fri, 10 Feb 2023 21:42:16 GMT  
		Size: 3.2 MB (3175116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdb5c0ff1110b4315355f81e38de10bb31ba9fe44d99d3b7598f20a28f2c98e1`  
		Last Modified: Sat, 11 Feb 2023 05:21:04 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9ac27252903c2b21737926a9cd0721ecfa3aba4f2e52da7f7c114aea4da62df`  
		Last Modified: Sat, 11 Feb 2023 05:21:04 GMT  
		Size: 1.2 MB (1223356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df30f40ce9a4931562f50ea55d6450396fd443fed95a0b2c0ea337f53f22ec25`  
		Last Modified: Sat, 11 Feb 2023 05:21:04 GMT  
		Size: 208.6 KB (208631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d9420167a9c04b73e787d02b0fa09ba21ff8b27917d0406146f9bc5a0df3034`  
		Last Modified: Sat, 11 Feb 2023 05:21:04 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea129f4350d878551c457a2192ea0570f86ca7ee5c193a6b0d8e19727570f05b`  
		Last Modified: Sat, 11 Feb 2023 05:21:04 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:1.6.2`

```console
$ docker pull spiped@sha256:dcd50fdfd27ec8f055329f6100c9237808b11c01a4605564877a8e91c2e240a2
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
$ docker pull spiped@sha256:65d1de8326124f7025322cdba5f11590bf65237b0cb63f400e388e7ec598f533
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.4 MB (37413302 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2e6f8b4beac2d2177806929f949e4e7ae5eca9086100ed06f9464b8f863786ed`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 09 Feb 2023 03:20:20 GMT
ADD file:3ea7c69e4bfac2ebb6f86baaedab31827c86a594dba8080a49928e211ad3c7a0 in / 
# Thu, 09 Feb 2023 03:20:20 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 06:37:17 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Thu, 09 Feb 2023 06:37:20 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 06:37:20 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 09 Feb 2023 06:37:40 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 09 Feb 2023 06:37:41 GMT
VOLUME [/spiped]
# Thu, 09 Feb 2023 06:37:41 GMT
WORKDIR /spiped
# Thu, 09 Feb 2023 06:37:41 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 09 Feb 2023 06:37:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 09 Feb 2023 06:37:41 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:bb263680fed18eecdc67f885094df6f589bafc19004839d7fdf141df236a61aa`  
		Last Modified: Thu, 09 Feb 2023 03:25:13 GMT  
		Size: 31.4 MB (31411810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:904147bf2f8667febed21ce347ecd042f5b9d779a1ac552bd4055ec2d7f060b6`  
		Last Modified: Thu, 09 Feb 2023 06:37:56 GMT  
		Size: 1.7 KB (1737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa73821f4c111ea10583bad55bd382aa4196e36aeca4093bf6ad2e4f27565fb4`  
		Last Modified: Thu, 09 Feb 2023 06:37:56 GMT  
		Size: 1.0 KB (1049 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccbe509202f24ed422baf731f3dd79e740b358183ad10a4d7554c5260d1f74cb`  
		Last Modified: Thu, 09 Feb 2023 06:37:57 GMT  
		Size: 6.0 MB (5998234 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9b81852413d69c15590cca8a24757c58e49244b108abaa2f57a3173de23700a`  
		Last Modified: Thu, 09 Feb 2023 06:37:56 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:714d39b5611de4a84c8a690342eb12e7f1f27cbc13ebfa1aa2d40e6db8e79031`  
		Last Modified: Thu, 09 Feb 2023 06:37:56 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.2` - linux; arm variant v5

```console
$ docker pull spiped@sha256:528e13ba139adf0768024a80cfc79ab5cb3d0ea5e8f9b9f3bc1511f2d698c215
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.9 MB (33947393 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5a1e48f7b0e65652cca9ca80196c861d383ac1f1b0103cc512be95efd00fc6e9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 01 Mar 2023 01:48:54 GMT
ADD file:b4fb1081f6eb8a0560d56d5781bbcedaac1453615d56e0943245dca784785ea2 in / 
# Wed, 01 Mar 2023 01:48:54 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 07:10:40 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 01 Mar 2023 07:10:44 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 07:10:44 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 01 Mar 2023 07:11:03 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 01 Mar 2023 07:11:03 GMT
VOLUME [/spiped]
# Wed, 01 Mar 2023 07:11:03 GMT
WORKDIR /spiped
# Wed, 01 Mar 2023 07:11:03 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 01 Mar 2023 07:11:03 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 01 Mar 2023 07:11:04 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:3c3af56dbec5913ef8aec0f1ca7112eb5914b4ad346ccd48f836dd7ec0621ba5`  
		Last Modified: Wed, 01 Mar 2023 01:52:57 GMT  
		Size: 28.9 MB (28915776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9aca7d992b566279fbac9ecdeffb9ff2db68cf1ffd6f31a2cce852311c28c5ce`  
		Last Modified: Wed, 01 Mar 2023 07:11:20 GMT  
		Size: 1.7 KB (1728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fc3eb64d155ea643dfc7dde1104693192a95033b812f1cf66e286245705de6f`  
		Last Modified: Wed, 01 Mar 2023 07:11:20 GMT  
		Size: 1.1 KB (1050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9169ad29c4b57b416977f34e4cae1ad9b4efb6110e2a150a7cb43b7eab0da3d3`  
		Last Modified: Wed, 01 Mar 2023 07:11:21 GMT  
		Size: 5.0 MB (5028368 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:742f87e7cb263314cfe9b69a92b5fef45b368e04c178942b699311a03503e14c`  
		Last Modified: Wed, 01 Mar 2023 07:11:20 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0dfe2f008531a4616c872689c583cd0c8468b2fb60b07981fc0e20a80f84497`  
		Last Modified: Wed, 01 Mar 2023 07:11:20 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.2` - linux; arm variant v7

```console
$ docker pull spiped@sha256:7017eb815f7e60e8ff5b15b21fe0cbd2ef33396feebd8f7f18bcfd82efcbcdca
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.3 MB (31329871 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5b689ef4b4dc24e15c83f0188d2896b65dfb8ab55d95974313cbac1be6f13df4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 09 Feb 2023 06:12:09 GMT
ADD file:5f1a343224e8486690bd90dd1e50c8d84b3d770c51bb6829544e5cf650c0419c in / 
# Thu, 09 Feb 2023 06:12:10 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 12:59:21 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Thu, 09 Feb 2023 12:59:25 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 12:59:25 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 09 Feb 2023 12:59:43 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 09 Feb 2023 12:59:43 GMT
VOLUME [/spiped]
# Thu, 09 Feb 2023 12:59:43 GMT
WORKDIR /spiped
# Thu, 09 Feb 2023 12:59:44 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 09 Feb 2023 12:59:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 09 Feb 2023 12:59:44 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:e7318f6106ad75d7d482ae9dddf4d927b0872ef3ddb6e1330aa691fc8d17279e`  
		Last Modified: Thu, 09 Feb 2023 06:19:19 GMT  
		Size: 26.6 MB (26577666 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e00b17d2d80b94e1a46f2bf36d6bc77f847e4cd57083ecbb8f84ad55d31d164a`  
		Last Modified: Thu, 09 Feb 2023 13:00:24 GMT  
		Size: 1.7 KB (1730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7293faff8274bf27a2e47ec70c06f8ab91fac589d357fdd3306a81ec075c3fb`  
		Last Modified: Thu, 09 Feb 2023 13:00:24 GMT  
		Size: 1.0 KB (1022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:420c029d7a4f8d85dc09d4d90250267b2137b15106d2fe5623c195ee79fcda5f`  
		Last Modified: Thu, 09 Feb 2023 13:00:27 GMT  
		Size: 4.7 MB (4749016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a8f996daf79da4e6f40d919b8671e3c4b55085710edea0584ea9f11b834bcce`  
		Last Modified: Thu, 09 Feb 2023 13:00:24 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef6016c3c267a148094099843a4bc93c8dc6f172510f577193c40ec9772fa0de`  
		Last Modified: Thu, 09 Feb 2023 13:00:24 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.2` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:ba65bbd88dad033e812d648ab5bec4670067246f6c0ff39ae8413e1bbb54b8ce
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.3 MB (35338340 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:40a101e61165070db066921b2c5822a0f2771bfce3632b8b52055fa79ff1a4f8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 09 Feb 2023 03:58:40 GMT
ADD file:3276ac85bb957360f20720da5b37498a6b5f91a017046049f8d2fd791f728a9a in / 
# Thu, 09 Feb 2023 03:58:40 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 08:54:18 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Thu, 09 Feb 2023 08:54:20 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 08:54:20 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 09 Feb 2023 08:54:35 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 09 Feb 2023 08:54:35 GMT
VOLUME [/spiped]
# Thu, 09 Feb 2023 08:54:35 GMT
WORKDIR /spiped
# Thu, 09 Feb 2023 08:54:35 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 09 Feb 2023 08:54:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 09 Feb 2023 08:54:35 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:5731adb3a4abcefe78d75783ea6e5ee87c4604d0c6a4f8c00b50085e162a7f5d`  
		Last Modified: Thu, 09 Feb 2023 04:02:34 GMT  
		Size: 30.1 MB (30062509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8137aa16a21880e530299f722a06622e5b58e5e7096c84fab419a159a7f04091`  
		Last Modified: Thu, 09 Feb 2023 08:54:53 GMT  
		Size: 1.7 KB (1739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2c2269b7f42a74f4a740b49267f4eaed378968aa33615a2a203cb15bc9360c2`  
		Last Modified: Thu, 09 Feb 2023 08:54:54 GMT  
		Size: 1.1 KB (1050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:052457e7f7a0e19dcaacf826e2ca00910c21085d12529627fd618e0d211863de`  
		Last Modified: Thu, 09 Feb 2023 08:54:54 GMT  
		Size: 5.3 MB (5272569 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17ae4ac2dc94d44f270d10320f3a8a057ae7af3d45f1ecf9c808b9a95cde305d`  
		Last Modified: Thu, 09 Feb 2023 08:54:53 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56ed7bfb7f7c49224f53d54b2d403c5be43966bc94394495d4104501b4129c1f`  
		Last Modified: Thu, 09 Feb 2023 08:54:53 GMT  
		Size: 344.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.2` - linux; 386

```console
$ docker pull spiped@sha256:bfa78a9926e73b519ea52984757a09e911d14c2bd9da1ab55972bd9ce2cf2d65
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.3 MB (40290432 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b6568369d320f09cd292f11fd201b8dca3a8cd63acb3bee3c7bb677d1a6a9eb5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 09 Feb 2023 05:12:53 GMT
ADD file:7740abd3129d33122ce51153c0b6c3323b9cbe9ea0e81672e16b2d7b210d24e3 in / 
# Thu, 09 Feb 2023 05:12:53 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 11:27:18 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Thu, 09 Feb 2023 11:27:22 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 11:27:23 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 09 Feb 2023 11:27:44 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 09 Feb 2023 11:27:44 GMT
VOLUME [/spiped]
# Thu, 09 Feb 2023 11:27:45 GMT
WORKDIR /spiped
# Thu, 09 Feb 2023 11:27:47 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 09 Feb 2023 11:27:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 09 Feb 2023 11:27:48 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:20744f4988404b1dee2cd438157b288d16a89da472583c0f04332ed389b258f8`  
		Last Modified: Thu, 09 Feb 2023 05:18:42 GMT  
		Size: 32.4 MB (32396875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37e01fd7049f58e3cf43b9c079e4da2f2b953c4792ee00e77aa6bea9acc10bb6`  
		Last Modified: Thu, 09 Feb 2023 11:28:15 GMT  
		Size: 1.6 KB (1614 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf141110ec25cbcd6fba0b5455ec049cbd33a0c16c1c8374a6b55c49c44290c4`  
		Last Modified: Thu, 09 Feb 2023 11:28:16 GMT  
		Size: 926.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c620d26def5e122b57324d22b9be7126f1aff0ee2808938cbaed2c0188aafe12`  
		Last Modified: Thu, 09 Feb 2023 11:28:17 GMT  
		Size: 7.9 MB (7890579 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b03b58be7cfa61363c0156f3f24fa50f0f503e6b2919c0a00abddbedd7764eda`  
		Last Modified: Thu, 09 Feb 2023 11:28:15 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe17e554449880852355124c22a61e8bcd828562f361f183b7096cbe1cd21a09`  
		Last Modified: Thu, 09 Feb 2023 11:28:15 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.2` - linux; mips64le

```console
$ docker pull spiped@sha256:b2ffe0253c458c187dd8728de9223a1a801ced3878b3304a43e6bb2d6708fd52
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.3 MB (35342689 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:71b26a2c72965d659a81b09281cdf469a7aaceeb51fa5a05e5f25152bfb18426`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 09 Feb 2023 02:45:21 GMT
ADD file:68e11645a37c49c8f8f9d79ba579d0d192aaab78bb28059f07d69d56aa5ace71 in / 
# Thu, 09 Feb 2023 02:45:25 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 09:28:59 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Thu, 09 Feb 2023 09:29:14 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 09:29:16 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 09 Feb 2023 09:30:45 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 09 Feb 2023 09:30:47 GMT
VOLUME [/spiped]
# Thu, 09 Feb 2023 09:30:50 GMT
WORKDIR /spiped
# Thu, 09 Feb 2023 09:30:52 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 09 Feb 2023 09:30:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 09 Feb 2023 09:30:58 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:1b5516936229d6629ab88588210eb90edc2613c94e5952fd1caf9200284f298a`  
		Last Modified: Thu, 09 Feb 2023 02:53:48 GMT  
		Size: 29.6 MB (29634449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3441e9678cbfa1a300965eb223fd19537d15afa6185479f02efb9549b6f90356`  
		Last Modified: Thu, 09 Feb 2023 09:31:13 GMT  
		Size: 1.6 KB (1619 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b9dda8c314f6a9f00c80e8d3774028d4204d754e4c828c2c38917e39f649706`  
		Last Modified: Thu, 09 Feb 2023 09:31:13 GMT  
		Size: 926.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed7b5d79a1e160a892ae3ca9a3585b9a3859b3843800b146b50a6f8dc2e37cea`  
		Last Modified: Thu, 09 Feb 2023 09:31:18 GMT  
		Size: 5.7 MB (5705255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e3972972765aa157621d8d380622fd6d29b61d44fd1b960930a1847ba23bfbb`  
		Last Modified: Thu, 09 Feb 2023 09:31:13 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc249832f7bdc107bfaebf38fb0292b7cacb7518cba7bad019f0d8ff699994c4`  
		Last Modified: Thu, 09 Feb 2023 09:31:13 GMT  
		Size: 345.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.2` - linux; ppc64le

```console
$ docker pull spiped@sha256:c55bb97521e65594872fe76cbfbc246cf4f6f31b3851f51ee61256ba623233de
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.3 MB (41292154 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2584a0abea40abb2a074488d4046bfa1ee2358d7221dcaada6120144742c42a9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 09 Feb 2023 06:21:49 GMT
ADD file:b09577b8131a90731fdfb00b824a97dc65ccb51d484cb9004382035d64a5741c in / 
# Thu, 09 Feb 2023 06:21:52 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 12:13:54 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Thu, 09 Feb 2023 12:14:00 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 12:14:00 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 09 Feb 2023 12:14:49 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 09 Feb 2023 12:14:50 GMT
VOLUME [/spiped]
# Thu, 09 Feb 2023 12:14:50 GMT
WORKDIR /spiped
# Thu, 09 Feb 2023 12:14:51 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 09 Feb 2023 12:14:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 09 Feb 2023 12:14:52 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:4ea90e1a094ae86c7950bbec99e7a79b08fae641ad5f3bc3af9081c925894c41`  
		Last Modified: Thu, 09 Feb 2023 06:28:27 GMT  
		Size: 35.3 MB (35289252 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:695fd45ccd8eac48da176341bba34201c9b8980634c1df9e9e8b4bfbfa220edc`  
		Last Modified: Thu, 09 Feb 2023 12:15:27 GMT  
		Size: 1.7 KB (1735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e02fb49a13103590e46d389b8e81a60bc1d01cbf4395c01b053e5e4e99f6e312`  
		Last Modified: Thu, 09 Feb 2023 12:15:27 GMT  
		Size: 1.0 KB (1049 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e9885ddc7088b14facf6e088ded644fc33dff7b4e6625a92eb87f71975a0703`  
		Last Modified: Thu, 09 Feb 2023 12:15:29 GMT  
		Size: 6.0 MB (5999645 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:300eee5c0fb43c90cd5a5c063707252fce74ce3a8ffc7fcd444c165dfb9753a9`  
		Last Modified: Thu, 09 Feb 2023 12:15:27 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e97c03ba3e8494c9ba2cb5d8837cbdf9d4f38177151f3c344b5459888bc9a2af`  
		Last Modified: Thu, 09 Feb 2023 12:15:27 GMT  
		Size: 344.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.2` - linux; s390x

```console
$ docker pull spiped@sha256:6763f80ffafaec400a9c32713f12023d7cfc9221fe27ded8e22f7668b5695825
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.8 MB (34837535 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e585d1138d7b913b469d1d60a8169d148407b55e74a2ae2fa3670406899e2703`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 01 Mar 2023 02:50:30 GMT
ADD file:01aa3de7444f0716938e0d85522be065193be4ffb6788b3190a0f4fefdbb8d65 in / 
# Wed, 01 Mar 2023 02:50:31 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 09:59:36 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 01 Mar 2023 09:59:39 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 09:59:39 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 01 Mar 2023 09:59:51 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 01 Mar 2023 09:59:51 GMT
VOLUME [/spiped]
# Wed, 01 Mar 2023 09:59:52 GMT
WORKDIR /spiped
# Wed, 01 Mar 2023 09:59:52 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 01 Mar 2023 09:59:52 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 01 Mar 2023 09:59:52 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:7b8d78f42e32e7fa234bcf890ae6603acab2881bca68a9d8c429981c7f42b1d6`  
		Last Modified: Wed, 01 Mar 2023 02:54:48 GMT  
		Size: 29.6 MB (29646854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:407e05b7731593d7281e5af1c1859fd2d47d7464ad6c5dc03ac8c8155a85e98d`  
		Last Modified: Wed, 01 Mar 2023 10:00:28 GMT  
		Size: 1.7 KB (1738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74698444aa451ceea677ff79b9924fe3f417d089f80b716455e9685ecc1306cc`  
		Last Modified: Wed, 01 Mar 2023 10:00:28 GMT  
		Size: 1.1 KB (1055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1e70e3b82bb8b17253bfb319a8144075d6a620afff629c1d1ea44ed93fe7ae2`  
		Last Modified: Wed, 01 Mar 2023 10:00:29 GMT  
		Size: 5.2 MB (5187420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fc09ee195f0d0c9a66b36017beedcd1c8bb0eeed0bc93753b944e58a218b522`  
		Last Modified: Wed, 01 Mar 2023 10:00:28 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cb0d5fb8ca92c7b1a4e4c6943edcc6e6afba039da0f1f566df5c8f887bd2b17`  
		Last Modified: Wed, 01 Mar 2023 10:00:28 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:1.6.2-alpine`

```console
$ docker pull spiped@sha256:5e05424b596fce7f7efec601ad9f597fd7e2a724acb9b9b0d26adb4f7db2ab17
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
$ docker pull spiped@sha256:b02340eb97482a93ed8c3997880473f27309e7362e27d06bfbdeb686da9f835f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.1 MB (5080754 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1660f13550a5bd6ce0ec142f4dc1325092450163ee42f52b56572854d7e8c1e3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Sat, 11 Feb 2023 04:46:42 GMT
ADD file:40887ab7c06977737e63c215c9bd297c0c74de8d12d16ebdf1c3d40ac392f62d in / 
# Sat, 11 Feb 2023 04:46:42 GMT
CMD ["/bin/sh"]
# Sat, 11 Feb 2023 14:04:29 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Sat, 11 Feb 2023 14:04:30 GMT
RUN apk add --no-cache libssl1.1
# Sat, 11 Feb 2023 14:04:30 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Sat, 11 Feb 2023 14:04:41 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Sat, 11 Feb 2023 14:04:41 GMT
VOLUME [/spiped]
# Sat, 11 Feb 2023 14:04:41 GMT
WORKDIR /spiped
# Sat, 11 Feb 2023 14:04:41 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 11 Feb 2023 14:04:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 11 Feb 2023 14:04:41 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:63b65145d645c1250c391b2d16ebe53b3747c295ca8ba2fcb6b0cf064a4dc21c`  
		Last Modified: Fri, 10 Feb 2023 22:41:31 GMT  
		Size: 3.4 MB (3374446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1567e533de4a753157026d7ef2c42cfa5f9efd21e25cc7370e4c8f1c8f1c8a47`  
		Last Modified: Sat, 11 Feb 2023 14:04:56 GMT  
		Size: 1.3 KB (1267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1a1fcb595374972f69b5a50bd54f62b80c9214b0f891c62726a3fb6853cf855`  
		Last Modified: Sat, 11 Feb 2023 14:04:56 GMT  
		Size: 1.5 MB (1483289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24f4efb6e81c911655772824a287a9f39d90e069841b4fe5601933b9b0ffe154`  
		Last Modified: Sat, 11 Feb 2023 14:04:56 GMT  
		Size: 221.3 KB (221282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:981056191296cd6f887bc7d5e8e078e1cec12690bc7fc8623b868e6b4023e0ea`  
		Last Modified: Sat, 11 Feb 2023 14:04:56 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:577ef58b3b8b045fa02bbbbd599b6c9d4310c0039e442d91e549dad4f7e556fd`  
		Last Modified: Sat, 11 Feb 2023 14:04:56 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.2-alpine` - linux; arm variant v6

```console
$ docker pull spiped@sha256:db9fbdc8e95acdd61baed85bf52d7ab004cb17dee7aa0af49efb381048c748f6
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.6 MB (4559794 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d097d8022015b53fe69632c85f6ae24a781bdbbddb3e23b28bdcc34b321a5303`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 10 Feb 2023 20:49:28 GMT
ADD file:d825d9aef59df0df23c0140a490998407ee0a62a051699b5c050aef7cb03f042 in / 
# Fri, 10 Feb 2023 20:49:28 GMT
CMD ["/bin/sh"]
# Sat, 11 Feb 2023 07:32:24 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Sat, 11 Feb 2023 07:32:25 GMT
RUN apk add --no-cache libssl1.1
# Sat, 11 Feb 2023 07:32:26 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Sat, 11 Feb 2023 07:32:35 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Sat, 11 Feb 2023 07:32:35 GMT
VOLUME [/spiped]
# Sat, 11 Feb 2023 07:32:35 GMT
WORKDIR /spiped
# Sat, 11 Feb 2023 07:32:35 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 11 Feb 2023 07:32:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 11 Feb 2023 07:32:35 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:6a6e4ab63e54442e16400f69d37f662d60cbd67565631eff6bf59b4176e482c3`  
		Last Modified: Fri, 10 Feb 2023 20:50:22 GMT  
		Size: 3.1 MB (3110885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21e65df37e068288828fdd590c704bdba0ca4a8b9872083bdcf0ed938b05bc83`  
		Last Modified: Sat, 11 Feb 2023 07:32:55 GMT  
		Size: 1.2 KB (1242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e14f23472a8ad51e73644e312c9cb85c69854bc3f7259a3863b49c57f09c862`  
		Last Modified: Sat, 11 Feb 2023 07:32:55 GMT  
		Size: 1.2 MB (1240903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df3e94e7304b5459469fc8c8309989eaead5db21667861fb64669ab70d9611e9`  
		Last Modified: Sat, 11 Feb 2023 07:32:55 GMT  
		Size: 206.3 KB (206329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8025107e0a863a04d24b21f3bf9d1f737abc6459904039f3c55da02f034af97`  
		Last Modified: Sat, 11 Feb 2023 07:32:55 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54cb12d0c5007f92277b3cf5469ce48354a5168dca26644088636f1abd9146e9`  
		Last Modified: Sat, 11 Feb 2023 07:32:55 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.2-alpine` - linux; arm variant v7

```console
$ docker pull spiped@sha256:e20c83b0b32876e4a85b4fa0a62215f32ef4133754b1cf4f8aa23104887f1cf3
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4237781 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ef3949961d888a47f1cbebc6f1ef749422a6a62131094ad66325f33d8083c8a9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 10 Feb 2023 21:51:31 GMT
ADD file:143b601fcc6b5d7d95d3e5ccad3fec7081191a47e28d4f9294a7fb2499cab1af in / 
# Fri, 10 Feb 2023 21:51:31 GMT
CMD ["/bin/sh"]
# Sat, 11 Feb 2023 06:33:15 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Sat, 11 Feb 2023 06:33:17 GMT
RUN apk add --no-cache libssl1.1
# Sat, 11 Feb 2023 06:33:17 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Sat, 11 Feb 2023 06:33:25 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Sat, 11 Feb 2023 06:33:25 GMT
VOLUME [/spiped]
# Sat, 11 Feb 2023 06:33:25 GMT
WORKDIR /spiped
# Sat, 11 Feb 2023 06:33:25 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 11 Feb 2023 06:33:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 11 Feb 2023 06:33:25 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:6fb81ff47bd6d7db0ed86c9b951ad6417ec73ab60af6d22daa604076a902629c`  
		Last Modified: Fri, 10 Feb 2023 21:52:33 GMT  
		Size: 2.9 MB (2868494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a442f55d4c235667f33954aaf938a7f1714b8d21b2cb808fef9de382589b17e`  
		Last Modified: Sat, 11 Feb 2023 06:33:57 GMT  
		Size: 1.2 KB (1241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09b931fceacae9f7416c4568a8a29feed89107a70cdbb6a5a8e84402bc9006a9`  
		Last Modified: Sat, 11 Feb 2023 06:33:58 GMT  
		Size: 1.2 MB (1167516 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bf5fcf25622eedad4a8b76251c540101849957497e32f268e38fd74749854b2`  
		Last Modified: Sat, 11 Feb 2023 06:33:57 GMT  
		Size: 200.1 KB (200095 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62c1ab78ee707e97bbf4c7ee00e91010a5c9cc6e318131e29021a1a3f1a1b18b`  
		Last Modified: Sat, 11 Feb 2023 06:33:57 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d26766ccb2e9e7597f86a2c98d9e36433e85cc86b8bfed0d16175725ac4cae1`  
		Last Modified: Sat, 11 Feb 2023 06:33:57 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.2-alpine` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:b202c4e5897cb771f303b85871c6b7a1fb5f025c51e651b30a4415f0e2e4973d
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.8 MB (4842933 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6c3a0f714da4f343e79de4855fa4cdc4a23892d7fe5654dec6710bc79bb2cc2c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 10 Feb 2023 21:24:08 GMT
ADD file:9bd9ea42a9f3bdc769e80c6b8a4b117d65f73ae68e155a6172a1184e7ac8bcc1 in / 
# Fri, 10 Feb 2023 21:24:08 GMT
CMD ["/bin/sh"]
# Sat, 11 Feb 2023 06:39:43 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Sat, 11 Feb 2023 06:39:44 GMT
RUN apk add --no-cache libssl1.1
# Sat, 11 Feb 2023 06:39:44 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Sat, 11 Feb 2023 06:39:52 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Sat, 11 Feb 2023 06:39:52 GMT
VOLUME [/spiped]
# Sat, 11 Feb 2023 06:39:52 GMT
WORKDIR /spiped
# Sat, 11 Feb 2023 06:39:52 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 11 Feb 2023 06:39:52 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 11 Feb 2023 06:39:52 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:af6eaf76a39c2d3e7e0b8a0420486e3df33c4027d696c076a99a3d0ac09026af`  
		Last Modified: Fri, 10 Feb 2023 21:24:39 GMT  
		Size: 3.3 MB (3261959 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32e706a54c37c1524628e434965039ac738ff48a6f151dd2ef6da2cb49958cc0`  
		Last Modified: Sat, 11 Feb 2023 06:40:07 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e99781ddd302da37630cc491b5190c39c7867e6bd96556fad9f613e3411bca0d`  
		Last Modified: Sat, 11 Feb 2023 06:40:07 GMT  
		Size: 1.4 MB (1363548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:768a1af5c81e5cc877ea8cb330527a3924d5f2b5acfc5dd8239f84fdf091e5ed`  
		Last Modified: Sat, 11 Feb 2023 06:40:07 GMT  
		Size: 215.7 KB (215691 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7567bda17775002440a508f6ff25154cb13c9201175281b80186ce38d44e2b7`  
		Last Modified: Sat, 11 Feb 2023 06:40:07 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba17a7f3c3024db40a3e0b478318d1eb5168af1437c2bd502fb302591b78f95a`  
		Last Modified: Sat, 11 Feb 2023 06:40:07 GMT  
		Size: 338.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.2-alpine` - linux; 386

```console
$ docker pull spiped@sha256:822b81d156b7c387e1ceda5cee3e6a6edd3268187a6ce26e8b85df4c68e09f5d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.1 MB (5131561 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e4d91ebbd686f96b26164ad7739fcfca17552f6046e879f7ae2d57c3d3892739`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 10 Feb 2023 21:24:23 GMT
ADD file:125f3514520a5cd29df2830a409aa026a2bc06a77a7a5d150133436404b33d41 in / 
# Fri, 10 Feb 2023 21:24:24 GMT
CMD ["/bin/sh"]
# Sat, 11 Feb 2023 03:18:56 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Sat, 11 Feb 2023 03:18:58 GMT
RUN apk add --no-cache libssl1.1
# Sat, 11 Feb 2023 03:18:59 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Sat, 11 Feb 2023 03:19:10 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Sat, 11 Feb 2023 03:19:10 GMT
VOLUME [/spiped]
# Sat, 11 Feb 2023 03:19:11 GMT
WORKDIR /spiped
# Sat, 11 Feb 2023 03:19:13 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 11 Feb 2023 03:19:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 11 Feb 2023 03:19:14 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:b3e346c15c2377ec0e75cc9efa98baecd58b0e9bb92f0ec07eeda0bcc7e67fc7`  
		Last Modified: Fri, 10 Feb 2023 21:25:13 GMT  
		Size: 3.4 MB (3412353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c7d8401c5bd9906ab3609377e9ee6deadd5d9c4ae39ecfa8e9cd01ede0b8281`  
		Last Modified: Sat, 11 Feb 2023 03:19:39 GMT  
		Size: 1.2 KB (1241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:469cab1d7427d43462f6a9628be5d2ff81ee2cd0f9f7541f9539bc00c92429f7`  
		Last Modified: Sat, 11 Feb 2023 03:19:40 GMT  
		Size: 1.5 MB (1486162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:272b1229ae2f459eb6817fe20b02d6f823f26e1e8c76b8ac51eb8934b9143027`  
		Last Modified: Sat, 11 Feb 2023 03:19:39 GMT  
		Size: 231.4 KB (231370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb4adf5f9d6c3c73c3d7546a48714ef20383a01eeb6f321be386524c8e6e4212`  
		Last Modified: Sat, 11 Feb 2023 03:19:39 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35580a675ce6a64cc7a800a1f273d54f02d5e70f9b158be76b5a569da9cdb610`  
		Last Modified: Sat, 11 Feb 2023 03:19:39 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.2-alpine` - linux; ppc64le

```console
$ docker pull spiped@sha256:75c7e8ce27d4c68e8862a8e832409e09dbeb2c47fa2163ac0ac7f4e794b6b14c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.0 MB (5025550 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:523cfab6c09a42cd9174ca6dee237febe2f4a72f0c07628ccddab56278968150`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 10 Feb 2023 21:20:36 GMT
ADD file:ec037a0d4b462d12963ac20d9ec49bb73b4bcaf84d4bc7b364ebf93667e585b0 in / 
# Fri, 10 Feb 2023 21:20:36 GMT
CMD ["/bin/sh"]
# Sat, 11 Feb 2023 09:33:46 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Sat, 11 Feb 2023 09:33:49 GMT
RUN apk add --no-cache libssl1.1
# Sat, 11 Feb 2023 09:33:50 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Sat, 11 Feb 2023 09:34:04 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Sat, 11 Feb 2023 09:34:04 GMT
VOLUME [/spiped]
# Sat, 11 Feb 2023 09:34:05 GMT
WORKDIR /spiped
# Sat, 11 Feb 2023 09:34:05 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 11 Feb 2023 09:34:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 11 Feb 2023 09:34:06 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:aa3c56f9c6f127b6c8f628c95db165741ca400d19bdaef2752d80f093e47451e`  
		Last Modified: Fri, 10 Feb 2023 21:21:37 GMT  
		Size: 3.4 MB (3390750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b5d50df2303841e19f748472d51fac8d0695468f1d50516484905b50450aa48`  
		Last Modified: Sat, 11 Feb 2023 09:34:31 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0b54432b9107e6d87810bd116ab5112e27a1f713d4d2c06525f0ed14f102e3c`  
		Last Modified: Sat, 11 Feb 2023 09:34:32 GMT  
		Size: 1.4 MB (1413040 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4bda8ea646857e9e3d0c92c042261af7dba424338abfc7cc1c58eec7b8985be`  
		Last Modified: Sat, 11 Feb 2023 09:34:32 GMT  
		Size: 220.0 KB (220021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e33bc423b9fd5cc84d66be2c92fc2c78368e9b5553d8c6848fab3570115fb66`  
		Last Modified: Sat, 11 Feb 2023 09:34:31 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53a89c5ec31eae84c318581d292f2fdc24ec49bc7692940d54b3b579b04cd2d6`  
		Last Modified: Sat, 11 Feb 2023 09:34:31 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.2-alpine` - linux; s390x

```console
$ docker pull spiped@sha256:c224a59dd171160cb9e3b3be6bac31704ad968f23bed4f4f8ae4d04d938951c6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.6 MB (4608839 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:88032fe647cd1b9c54c93549e3978f1e53d8c0df71f2c0c2660b0545fc0b7ae3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 10 Feb 2023 21:41:25 GMT
ADD file:03b2fb4d732a294329449ff55c5d84f7d2735e6510985718979469994f3a607b in / 
# Fri, 10 Feb 2023 21:41:26 GMT
CMD ["/bin/sh"]
# Sat, 11 Feb 2023 05:20:31 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Sat, 11 Feb 2023 05:20:32 GMT
RUN apk add --no-cache libssl1.1
# Sat, 11 Feb 2023 05:20:33 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Sat, 11 Feb 2023 05:20:38 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Sat, 11 Feb 2023 05:20:38 GMT
VOLUME [/spiped]
# Sat, 11 Feb 2023 05:20:38 GMT
WORKDIR /spiped
# Sat, 11 Feb 2023 05:20:39 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 11 Feb 2023 05:20:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 11 Feb 2023 05:20:39 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:24c4f8de3549a39c64b0edc2cfa68769b373f35138d0f13725100160bb32d4e2`  
		Last Modified: Fri, 10 Feb 2023 21:42:16 GMT  
		Size: 3.2 MB (3175116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdb5c0ff1110b4315355f81e38de10bb31ba9fe44d99d3b7598f20a28f2c98e1`  
		Last Modified: Sat, 11 Feb 2023 05:21:04 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9ac27252903c2b21737926a9cd0721ecfa3aba4f2e52da7f7c114aea4da62df`  
		Last Modified: Sat, 11 Feb 2023 05:21:04 GMT  
		Size: 1.2 MB (1223356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df30f40ce9a4931562f50ea55d6450396fd443fed95a0b2c0ea337f53f22ec25`  
		Last Modified: Sat, 11 Feb 2023 05:21:04 GMT  
		Size: 208.6 KB (208631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d9420167a9c04b73e787d02b0fa09ba21ff8b27917d0406146f9bc5a0df3034`  
		Last Modified: Sat, 11 Feb 2023 05:21:04 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea129f4350d878551c457a2192ea0570f86ca7ee5c193a6b0d8e19727570f05b`  
		Last Modified: Sat, 11 Feb 2023 05:21:04 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:alpine`

```console
$ docker pull spiped@sha256:5e05424b596fce7f7efec601ad9f597fd7e2a724acb9b9b0d26adb4f7db2ab17
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
$ docker pull spiped@sha256:b02340eb97482a93ed8c3997880473f27309e7362e27d06bfbdeb686da9f835f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.1 MB (5080754 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1660f13550a5bd6ce0ec142f4dc1325092450163ee42f52b56572854d7e8c1e3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Sat, 11 Feb 2023 04:46:42 GMT
ADD file:40887ab7c06977737e63c215c9bd297c0c74de8d12d16ebdf1c3d40ac392f62d in / 
# Sat, 11 Feb 2023 04:46:42 GMT
CMD ["/bin/sh"]
# Sat, 11 Feb 2023 14:04:29 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Sat, 11 Feb 2023 14:04:30 GMT
RUN apk add --no-cache libssl1.1
# Sat, 11 Feb 2023 14:04:30 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Sat, 11 Feb 2023 14:04:41 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Sat, 11 Feb 2023 14:04:41 GMT
VOLUME [/spiped]
# Sat, 11 Feb 2023 14:04:41 GMT
WORKDIR /spiped
# Sat, 11 Feb 2023 14:04:41 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 11 Feb 2023 14:04:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 11 Feb 2023 14:04:41 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:63b65145d645c1250c391b2d16ebe53b3747c295ca8ba2fcb6b0cf064a4dc21c`  
		Last Modified: Fri, 10 Feb 2023 22:41:31 GMT  
		Size: 3.4 MB (3374446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1567e533de4a753157026d7ef2c42cfa5f9efd21e25cc7370e4c8f1c8f1c8a47`  
		Last Modified: Sat, 11 Feb 2023 14:04:56 GMT  
		Size: 1.3 KB (1267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1a1fcb595374972f69b5a50bd54f62b80c9214b0f891c62726a3fb6853cf855`  
		Last Modified: Sat, 11 Feb 2023 14:04:56 GMT  
		Size: 1.5 MB (1483289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24f4efb6e81c911655772824a287a9f39d90e069841b4fe5601933b9b0ffe154`  
		Last Modified: Sat, 11 Feb 2023 14:04:56 GMT  
		Size: 221.3 KB (221282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:981056191296cd6f887bc7d5e8e078e1cec12690bc7fc8623b868e6b4023e0ea`  
		Last Modified: Sat, 11 Feb 2023 14:04:56 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:577ef58b3b8b045fa02bbbbd599b6c9d4310c0039e442d91e549dad4f7e556fd`  
		Last Modified: Sat, 11 Feb 2023 14:04:56 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; arm variant v6

```console
$ docker pull spiped@sha256:db9fbdc8e95acdd61baed85bf52d7ab004cb17dee7aa0af49efb381048c748f6
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.6 MB (4559794 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d097d8022015b53fe69632c85f6ae24a781bdbbddb3e23b28bdcc34b321a5303`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 10 Feb 2023 20:49:28 GMT
ADD file:d825d9aef59df0df23c0140a490998407ee0a62a051699b5c050aef7cb03f042 in / 
# Fri, 10 Feb 2023 20:49:28 GMT
CMD ["/bin/sh"]
# Sat, 11 Feb 2023 07:32:24 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Sat, 11 Feb 2023 07:32:25 GMT
RUN apk add --no-cache libssl1.1
# Sat, 11 Feb 2023 07:32:26 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Sat, 11 Feb 2023 07:32:35 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Sat, 11 Feb 2023 07:32:35 GMT
VOLUME [/spiped]
# Sat, 11 Feb 2023 07:32:35 GMT
WORKDIR /spiped
# Sat, 11 Feb 2023 07:32:35 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 11 Feb 2023 07:32:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 11 Feb 2023 07:32:35 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:6a6e4ab63e54442e16400f69d37f662d60cbd67565631eff6bf59b4176e482c3`  
		Last Modified: Fri, 10 Feb 2023 20:50:22 GMT  
		Size: 3.1 MB (3110885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21e65df37e068288828fdd590c704bdba0ca4a8b9872083bdcf0ed938b05bc83`  
		Last Modified: Sat, 11 Feb 2023 07:32:55 GMT  
		Size: 1.2 KB (1242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e14f23472a8ad51e73644e312c9cb85c69854bc3f7259a3863b49c57f09c862`  
		Last Modified: Sat, 11 Feb 2023 07:32:55 GMT  
		Size: 1.2 MB (1240903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df3e94e7304b5459469fc8c8309989eaead5db21667861fb64669ab70d9611e9`  
		Last Modified: Sat, 11 Feb 2023 07:32:55 GMT  
		Size: 206.3 KB (206329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8025107e0a863a04d24b21f3bf9d1f737abc6459904039f3c55da02f034af97`  
		Last Modified: Sat, 11 Feb 2023 07:32:55 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54cb12d0c5007f92277b3cf5469ce48354a5168dca26644088636f1abd9146e9`  
		Last Modified: Sat, 11 Feb 2023 07:32:55 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; arm variant v7

```console
$ docker pull spiped@sha256:e20c83b0b32876e4a85b4fa0a62215f32ef4133754b1cf4f8aa23104887f1cf3
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4237781 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ef3949961d888a47f1cbebc6f1ef749422a6a62131094ad66325f33d8083c8a9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 10 Feb 2023 21:51:31 GMT
ADD file:143b601fcc6b5d7d95d3e5ccad3fec7081191a47e28d4f9294a7fb2499cab1af in / 
# Fri, 10 Feb 2023 21:51:31 GMT
CMD ["/bin/sh"]
# Sat, 11 Feb 2023 06:33:15 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Sat, 11 Feb 2023 06:33:17 GMT
RUN apk add --no-cache libssl1.1
# Sat, 11 Feb 2023 06:33:17 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Sat, 11 Feb 2023 06:33:25 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Sat, 11 Feb 2023 06:33:25 GMT
VOLUME [/spiped]
# Sat, 11 Feb 2023 06:33:25 GMT
WORKDIR /spiped
# Sat, 11 Feb 2023 06:33:25 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 11 Feb 2023 06:33:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 11 Feb 2023 06:33:25 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:6fb81ff47bd6d7db0ed86c9b951ad6417ec73ab60af6d22daa604076a902629c`  
		Last Modified: Fri, 10 Feb 2023 21:52:33 GMT  
		Size: 2.9 MB (2868494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a442f55d4c235667f33954aaf938a7f1714b8d21b2cb808fef9de382589b17e`  
		Last Modified: Sat, 11 Feb 2023 06:33:57 GMT  
		Size: 1.2 KB (1241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09b931fceacae9f7416c4568a8a29feed89107a70cdbb6a5a8e84402bc9006a9`  
		Last Modified: Sat, 11 Feb 2023 06:33:58 GMT  
		Size: 1.2 MB (1167516 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bf5fcf25622eedad4a8b76251c540101849957497e32f268e38fd74749854b2`  
		Last Modified: Sat, 11 Feb 2023 06:33:57 GMT  
		Size: 200.1 KB (200095 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62c1ab78ee707e97bbf4c7ee00e91010a5c9cc6e318131e29021a1a3f1a1b18b`  
		Last Modified: Sat, 11 Feb 2023 06:33:57 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d26766ccb2e9e7597f86a2c98d9e36433e85cc86b8bfed0d16175725ac4cae1`  
		Last Modified: Sat, 11 Feb 2023 06:33:57 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:b202c4e5897cb771f303b85871c6b7a1fb5f025c51e651b30a4415f0e2e4973d
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.8 MB (4842933 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6c3a0f714da4f343e79de4855fa4cdc4a23892d7fe5654dec6710bc79bb2cc2c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 10 Feb 2023 21:24:08 GMT
ADD file:9bd9ea42a9f3bdc769e80c6b8a4b117d65f73ae68e155a6172a1184e7ac8bcc1 in / 
# Fri, 10 Feb 2023 21:24:08 GMT
CMD ["/bin/sh"]
# Sat, 11 Feb 2023 06:39:43 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Sat, 11 Feb 2023 06:39:44 GMT
RUN apk add --no-cache libssl1.1
# Sat, 11 Feb 2023 06:39:44 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Sat, 11 Feb 2023 06:39:52 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Sat, 11 Feb 2023 06:39:52 GMT
VOLUME [/spiped]
# Sat, 11 Feb 2023 06:39:52 GMT
WORKDIR /spiped
# Sat, 11 Feb 2023 06:39:52 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 11 Feb 2023 06:39:52 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 11 Feb 2023 06:39:52 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:af6eaf76a39c2d3e7e0b8a0420486e3df33c4027d696c076a99a3d0ac09026af`  
		Last Modified: Fri, 10 Feb 2023 21:24:39 GMT  
		Size: 3.3 MB (3261959 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32e706a54c37c1524628e434965039ac738ff48a6f151dd2ef6da2cb49958cc0`  
		Last Modified: Sat, 11 Feb 2023 06:40:07 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e99781ddd302da37630cc491b5190c39c7867e6bd96556fad9f613e3411bca0d`  
		Last Modified: Sat, 11 Feb 2023 06:40:07 GMT  
		Size: 1.4 MB (1363548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:768a1af5c81e5cc877ea8cb330527a3924d5f2b5acfc5dd8239f84fdf091e5ed`  
		Last Modified: Sat, 11 Feb 2023 06:40:07 GMT  
		Size: 215.7 KB (215691 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7567bda17775002440a508f6ff25154cb13c9201175281b80186ce38d44e2b7`  
		Last Modified: Sat, 11 Feb 2023 06:40:07 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba17a7f3c3024db40a3e0b478318d1eb5168af1437c2bd502fb302591b78f95a`  
		Last Modified: Sat, 11 Feb 2023 06:40:07 GMT  
		Size: 338.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; 386

```console
$ docker pull spiped@sha256:822b81d156b7c387e1ceda5cee3e6a6edd3268187a6ce26e8b85df4c68e09f5d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.1 MB (5131561 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e4d91ebbd686f96b26164ad7739fcfca17552f6046e879f7ae2d57c3d3892739`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 10 Feb 2023 21:24:23 GMT
ADD file:125f3514520a5cd29df2830a409aa026a2bc06a77a7a5d150133436404b33d41 in / 
# Fri, 10 Feb 2023 21:24:24 GMT
CMD ["/bin/sh"]
# Sat, 11 Feb 2023 03:18:56 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Sat, 11 Feb 2023 03:18:58 GMT
RUN apk add --no-cache libssl1.1
# Sat, 11 Feb 2023 03:18:59 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Sat, 11 Feb 2023 03:19:10 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Sat, 11 Feb 2023 03:19:10 GMT
VOLUME [/spiped]
# Sat, 11 Feb 2023 03:19:11 GMT
WORKDIR /spiped
# Sat, 11 Feb 2023 03:19:13 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 11 Feb 2023 03:19:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 11 Feb 2023 03:19:14 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:b3e346c15c2377ec0e75cc9efa98baecd58b0e9bb92f0ec07eeda0bcc7e67fc7`  
		Last Modified: Fri, 10 Feb 2023 21:25:13 GMT  
		Size: 3.4 MB (3412353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c7d8401c5bd9906ab3609377e9ee6deadd5d9c4ae39ecfa8e9cd01ede0b8281`  
		Last Modified: Sat, 11 Feb 2023 03:19:39 GMT  
		Size: 1.2 KB (1241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:469cab1d7427d43462f6a9628be5d2ff81ee2cd0f9f7541f9539bc00c92429f7`  
		Last Modified: Sat, 11 Feb 2023 03:19:40 GMT  
		Size: 1.5 MB (1486162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:272b1229ae2f459eb6817fe20b02d6f823f26e1e8c76b8ac51eb8934b9143027`  
		Last Modified: Sat, 11 Feb 2023 03:19:39 GMT  
		Size: 231.4 KB (231370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb4adf5f9d6c3c73c3d7546a48714ef20383a01eeb6f321be386524c8e6e4212`  
		Last Modified: Sat, 11 Feb 2023 03:19:39 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35580a675ce6a64cc7a800a1f273d54f02d5e70f9b158be76b5a569da9cdb610`  
		Last Modified: Sat, 11 Feb 2023 03:19:39 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; ppc64le

```console
$ docker pull spiped@sha256:75c7e8ce27d4c68e8862a8e832409e09dbeb2c47fa2163ac0ac7f4e794b6b14c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.0 MB (5025550 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:523cfab6c09a42cd9174ca6dee237febe2f4a72f0c07628ccddab56278968150`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 10 Feb 2023 21:20:36 GMT
ADD file:ec037a0d4b462d12963ac20d9ec49bb73b4bcaf84d4bc7b364ebf93667e585b0 in / 
# Fri, 10 Feb 2023 21:20:36 GMT
CMD ["/bin/sh"]
# Sat, 11 Feb 2023 09:33:46 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Sat, 11 Feb 2023 09:33:49 GMT
RUN apk add --no-cache libssl1.1
# Sat, 11 Feb 2023 09:33:50 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Sat, 11 Feb 2023 09:34:04 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Sat, 11 Feb 2023 09:34:04 GMT
VOLUME [/spiped]
# Sat, 11 Feb 2023 09:34:05 GMT
WORKDIR /spiped
# Sat, 11 Feb 2023 09:34:05 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 11 Feb 2023 09:34:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 11 Feb 2023 09:34:06 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:aa3c56f9c6f127b6c8f628c95db165741ca400d19bdaef2752d80f093e47451e`  
		Last Modified: Fri, 10 Feb 2023 21:21:37 GMT  
		Size: 3.4 MB (3390750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b5d50df2303841e19f748472d51fac8d0695468f1d50516484905b50450aa48`  
		Last Modified: Sat, 11 Feb 2023 09:34:31 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0b54432b9107e6d87810bd116ab5112e27a1f713d4d2c06525f0ed14f102e3c`  
		Last Modified: Sat, 11 Feb 2023 09:34:32 GMT  
		Size: 1.4 MB (1413040 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4bda8ea646857e9e3d0c92c042261af7dba424338abfc7cc1c58eec7b8985be`  
		Last Modified: Sat, 11 Feb 2023 09:34:32 GMT  
		Size: 220.0 KB (220021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e33bc423b9fd5cc84d66be2c92fc2c78368e9b5553d8c6848fab3570115fb66`  
		Last Modified: Sat, 11 Feb 2023 09:34:31 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53a89c5ec31eae84c318581d292f2fdc24ec49bc7692940d54b3b579b04cd2d6`  
		Last Modified: Sat, 11 Feb 2023 09:34:31 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; s390x

```console
$ docker pull spiped@sha256:c224a59dd171160cb9e3b3be6bac31704ad968f23bed4f4f8ae4d04d938951c6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.6 MB (4608839 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:88032fe647cd1b9c54c93549e3978f1e53d8c0df71f2c0c2660b0545fc0b7ae3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 10 Feb 2023 21:41:25 GMT
ADD file:03b2fb4d732a294329449ff55c5d84f7d2735e6510985718979469994f3a607b in / 
# Fri, 10 Feb 2023 21:41:26 GMT
CMD ["/bin/sh"]
# Sat, 11 Feb 2023 05:20:31 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Sat, 11 Feb 2023 05:20:32 GMT
RUN apk add --no-cache libssl1.1
# Sat, 11 Feb 2023 05:20:33 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Sat, 11 Feb 2023 05:20:38 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Sat, 11 Feb 2023 05:20:38 GMT
VOLUME [/spiped]
# Sat, 11 Feb 2023 05:20:38 GMT
WORKDIR /spiped
# Sat, 11 Feb 2023 05:20:39 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Sat, 11 Feb 2023 05:20:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 11 Feb 2023 05:20:39 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:24c4f8de3549a39c64b0edc2cfa68769b373f35138d0f13725100160bb32d4e2`  
		Last Modified: Fri, 10 Feb 2023 21:42:16 GMT  
		Size: 3.2 MB (3175116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdb5c0ff1110b4315355f81e38de10bb31ba9fe44d99d3b7598f20a28f2c98e1`  
		Last Modified: Sat, 11 Feb 2023 05:21:04 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9ac27252903c2b21737926a9cd0721ecfa3aba4f2e52da7f7c114aea4da62df`  
		Last Modified: Sat, 11 Feb 2023 05:21:04 GMT  
		Size: 1.2 MB (1223356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df30f40ce9a4931562f50ea55d6450396fd443fed95a0b2c0ea337f53f22ec25`  
		Last Modified: Sat, 11 Feb 2023 05:21:04 GMT  
		Size: 208.6 KB (208631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d9420167a9c04b73e787d02b0fa09ba21ff8b27917d0406146f9bc5a0df3034`  
		Last Modified: Sat, 11 Feb 2023 05:21:04 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea129f4350d878551c457a2192ea0570f86ca7ee5c193a6b0d8e19727570f05b`  
		Last Modified: Sat, 11 Feb 2023 05:21:04 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:latest`

```console
$ docker pull spiped@sha256:dcd50fdfd27ec8f055329f6100c9237808b11c01a4605564877a8e91c2e240a2
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
$ docker pull spiped@sha256:65d1de8326124f7025322cdba5f11590bf65237b0cb63f400e388e7ec598f533
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.4 MB (37413302 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2e6f8b4beac2d2177806929f949e4e7ae5eca9086100ed06f9464b8f863786ed`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 09 Feb 2023 03:20:20 GMT
ADD file:3ea7c69e4bfac2ebb6f86baaedab31827c86a594dba8080a49928e211ad3c7a0 in / 
# Thu, 09 Feb 2023 03:20:20 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 06:37:17 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Thu, 09 Feb 2023 06:37:20 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 06:37:20 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 09 Feb 2023 06:37:40 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 09 Feb 2023 06:37:41 GMT
VOLUME [/spiped]
# Thu, 09 Feb 2023 06:37:41 GMT
WORKDIR /spiped
# Thu, 09 Feb 2023 06:37:41 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 09 Feb 2023 06:37:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 09 Feb 2023 06:37:41 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:bb263680fed18eecdc67f885094df6f589bafc19004839d7fdf141df236a61aa`  
		Last Modified: Thu, 09 Feb 2023 03:25:13 GMT  
		Size: 31.4 MB (31411810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:904147bf2f8667febed21ce347ecd042f5b9d779a1ac552bd4055ec2d7f060b6`  
		Last Modified: Thu, 09 Feb 2023 06:37:56 GMT  
		Size: 1.7 KB (1737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa73821f4c111ea10583bad55bd382aa4196e36aeca4093bf6ad2e4f27565fb4`  
		Last Modified: Thu, 09 Feb 2023 06:37:56 GMT  
		Size: 1.0 KB (1049 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccbe509202f24ed422baf731f3dd79e740b358183ad10a4d7554c5260d1f74cb`  
		Last Modified: Thu, 09 Feb 2023 06:37:57 GMT  
		Size: 6.0 MB (5998234 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9b81852413d69c15590cca8a24757c58e49244b108abaa2f57a3173de23700a`  
		Last Modified: Thu, 09 Feb 2023 06:37:56 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:714d39b5611de4a84c8a690342eb12e7f1f27cbc13ebfa1aa2d40e6db8e79031`  
		Last Modified: Thu, 09 Feb 2023 06:37:56 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; arm variant v5

```console
$ docker pull spiped@sha256:528e13ba139adf0768024a80cfc79ab5cb3d0ea5e8f9b9f3bc1511f2d698c215
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.9 MB (33947393 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5a1e48f7b0e65652cca9ca80196c861d383ac1f1b0103cc512be95efd00fc6e9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 01 Mar 2023 01:48:54 GMT
ADD file:b4fb1081f6eb8a0560d56d5781bbcedaac1453615d56e0943245dca784785ea2 in / 
# Wed, 01 Mar 2023 01:48:54 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 07:10:40 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 01 Mar 2023 07:10:44 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 07:10:44 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 01 Mar 2023 07:11:03 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 01 Mar 2023 07:11:03 GMT
VOLUME [/spiped]
# Wed, 01 Mar 2023 07:11:03 GMT
WORKDIR /spiped
# Wed, 01 Mar 2023 07:11:03 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 01 Mar 2023 07:11:03 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 01 Mar 2023 07:11:04 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:3c3af56dbec5913ef8aec0f1ca7112eb5914b4ad346ccd48f836dd7ec0621ba5`  
		Last Modified: Wed, 01 Mar 2023 01:52:57 GMT  
		Size: 28.9 MB (28915776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9aca7d992b566279fbac9ecdeffb9ff2db68cf1ffd6f31a2cce852311c28c5ce`  
		Last Modified: Wed, 01 Mar 2023 07:11:20 GMT  
		Size: 1.7 KB (1728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fc3eb64d155ea643dfc7dde1104693192a95033b812f1cf66e286245705de6f`  
		Last Modified: Wed, 01 Mar 2023 07:11:20 GMT  
		Size: 1.1 KB (1050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9169ad29c4b57b416977f34e4cae1ad9b4efb6110e2a150a7cb43b7eab0da3d3`  
		Last Modified: Wed, 01 Mar 2023 07:11:21 GMT  
		Size: 5.0 MB (5028368 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:742f87e7cb263314cfe9b69a92b5fef45b368e04c178942b699311a03503e14c`  
		Last Modified: Wed, 01 Mar 2023 07:11:20 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0dfe2f008531a4616c872689c583cd0c8468b2fb60b07981fc0e20a80f84497`  
		Last Modified: Wed, 01 Mar 2023 07:11:20 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; arm variant v7

```console
$ docker pull spiped@sha256:7017eb815f7e60e8ff5b15b21fe0cbd2ef33396feebd8f7f18bcfd82efcbcdca
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.3 MB (31329871 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5b689ef4b4dc24e15c83f0188d2896b65dfb8ab55d95974313cbac1be6f13df4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 09 Feb 2023 06:12:09 GMT
ADD file:5f1a343224e8486690bd90dd1e50c8d84b3d770c51bb6829544e5cf650c0419c in / 
# Thu, 09 Feb 2023 06:12:10 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 12:59:21 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Thu, 09 Feb 2023 12:59:25 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 12:59:25 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 09 Feb 2023 12:59:43 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 09 Feb 2023 12:59:43 GMT
VOLUME [/spiped]
# Thu, 09 Feb 2023 12:59:43 GMT
WORKDIR /spiped
# Thu, 09 Feb 2023 12:59:44 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 09 Feb 2023 12:59:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 09 Feb 2023 12:59:44 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:e7318f6106ad75d7d482ae9dddf4d927b0872ef3ddb6e1330aa691fc8d17279e`  
		Last Modified: Thu, 09 Feb 2023 06:19:19 GMT  
		Size: 26.6 MB (26577666 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e00b17d2d80b94e1a46f2bf36d6bc77f847e4cd57083ecbb8f84ad55d31d164a`  
		Last Modified: Thu, 09 Feb 2023 13:00:24 GMT  
		Size: 1.7 KB (1730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7293faff8274bf27a2e47ec70c06f8ab91fac589d357fdd3306a81ec075c3fb`  
		Last Modified: Thu, 09 Feb 2023 13:00:24 GMT  
		Size: 1.0 KB (1022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:420c029d7a4f8d85dc09d4d90250267b2137b15106d2fe5623c195ee79fcda5f`  
		Last Modified: Thu, 09 Feb 2023 13:00:27 GMT  
		Size: 4.7 MB (4749016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a8f996daf79da4e6f40d919b8671e3c4b55085710edea0584ea9f11b834bcce`  
		Last Modified: Thu, 09 Feb 2023 13:00:24 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef6016c3c267a148094099843a4bc93c8dc6f172510f577193c40ec9772fa0de`  
		Last Modified: Thu, 09 Feb 2023 13:00:24 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:ba65bbd88dad033e812d648ab5bec4670067246f6c0ff39ae8413e1bbb54b8ce
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.3 MB (35338340 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:40a101e61165070db066921b2c5822a0f2771bfce3632b8b52055fa79ff1a4f8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 09 Feb 2023 03:58:40 GMT
ADD file:3276ac85bb957360f20720da5b37498a6b5f91a017046049f8d2fd791f728a9a in / 
# Thu, 09 Feb 2023 03:58:40 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 08:54:18 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Thu, 09 Feb 2023 08:54:20 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 08:54:20 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 09 Feb 2023 08:54:35 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 09 Feb 2023 08:54:35 GMT
VOLUME [/spiped]
# Thu, 09 Feb 2023 08:54:35 GMT
WORKDIR /spiped
# Thu, 09 Feb 2023 08:54:35 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 09 Feb 2023 08:54:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 09 Feb 2023 08:54:35 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:5731adb3a4abcefe78d75783ea6e5ee87c4604d0c6a4f8c00b50085e162a7f5d`  
		Last Modified: Thu, 09 Feb 2023 04:02:34 GMT  
		Size: 30.1 MB (30062509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8137aa16a21880e530299f722a06622e5b58e5e7096c84fab419a159a7f04091`  
		Last Modified: Thu, 09 Feb 2023 08:54:53 GMT  
		Size: 1.7 KB (1739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2c2269b7f42a74f4a740b49267f4eaed378968aa33615a2a203cb15bc9360c2`  
		Last Modified: Thu, 09 Feb 2023 08:54:54 GMT  
		Size: 1.1 KB (1050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:052457e7f7a0e19dcaacf826e2ca00910c21085d12529627fd618e0d211863de`  
		Last Modified: Thu, 09 Feb 2023 08:54:54 GMT  
		Size: 5.3 MB (5272569 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17ae4ac2dc94d44f270d10320f3a8a057ae7af3d45f1ecf9c808b9a95cde305d`  
		Last Modified: Thu, 09 Feb 2023 08:54:53 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56ed7bfb7f7c49224f53d54b2d403c5be43966bc94394495d4104501b4129c1f`  
		Last Modified: Thu, 09 Feb 2023 08:54:53 GMT  
		Size: 344.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; 386

```console
$ docker pull spiped@sha256:bfa78a9926e73b519ea52984757a09e911d14c2bd9da1ab55972bd9ce2cf2d65
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.3 MB (40290432 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b6568369d320f09cd292f11fd201b8dca3a8cd63acb3bee3c7bb677d1a6a9eb5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 09 Feb 2023 05:12:53 GMT
ADD file:7740abd3129d33122ce51153c0b6c3323b9cbe9ea0e81672e16b2d7b210d24e3 in / 
# Thu, 09 Feb 2023 05:12:53 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 11:27:18 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Thu, 09 Feb 2023 11:27:22 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 11:27:23 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 09 Feb 2023 11:27:44 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 09 Feb 2023 11:27:44 GMT
VOLUME [/spiped]
# Thu, 09 Feb 2023 11:27:45 GMT
WORKDIR /spiped
# Thu, 09 Feb 2023 11:27:47 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 09 Feb 2023 11:27:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 09 Feb 2023 11:27:48 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:20744f4988404b1dee2cd438157b288d16a89da472583c0f04332ed389b258f8`  
		Last Modified: Thu, 09 Feb 2023 05:18:42 GMT  
		Size: 32.4 MB (32396875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37e01fd7049f58e3cf43b9c079e4da2f2b953c4792ee00e77aa6bea9acc10bb6`  
		Last Modified: Thu, 09 Feb 2023 11:28:15 GMT  
		Size: 1.6 KB (1614 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf141110ec25cbcd6fba0b5455ec049cbd33a0c16c1c8374a6b55c49c44290c4`  
		Last Modified: Thu, 09 Feb 2023 11:28:16 GMT  
		Size: 926.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c620d26def5e122b57324d22b9be7126f1aff0ee2808938cbaed2c0188aafe12`  
		Last Modified: Thu, 09 Feb 2023 11:28:17 GMT  
		Size: 7.9 MB (7890579 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b03b58be7cfa61363c0156f3f24fa50f0f503e6b2919c0a00abddbedd7764eda`  
		Last Modified: Thu, 09 Feb 2023 11:28:15 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe17e554449880852355124c22a61e8bcd828562f361f183b7096cbe1cd21a09`  
		Last Modified: Thu, 09 Feb 2023 11:28:15 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; mips64le

```console
$ docker pull spiped@sha256:b2ffe0253c458c187dd8728de9223a1a801ced3878b3304a43e6bb2d6708fd52
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.3 MB (35342689 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:71b26a2c72965d659a81b09281cdf469a7aaceeb51fa5a05e5f25152bfb18426`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 09 Feb 2023 02:45:21 GMT
ADD file:68e11645a37c49c8f8f9d79ba579d0d192aaab78bb28059f07d69d56aa5ace71 in / 
# Thu, 09 Feb 2023 02:45:25 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 09:28:59 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Thu, 09 Feb 2023 09:29:14 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 09:29:16 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 09 Feb 2023 09:30:45 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 09 Feb 2023 09:30:47 GMT
VOLUME [/spiped]
# Thu, 09 Feb 2023 09:30:50 GMT
WORKDIR /spiped
# Thu, 09 Feb 2023 09:30:52 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 09 Feb 2023 09:30:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 09 Feb 2023 09:30:58 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:1b5516936229d6629ab88588210eb90edc2613c94e5952fd1caf9200284f298a`  
		Last Modified: Thu, 09 Feb 2023 02:53:48 GMT  
		Size: 29.6 MB (29634449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3441e9678cbfa1a300965eb223fd19537d15afa6185479f02efb9549b6f90356`  
		Last Modified: Thu, 09 Feb 2023 09:31:13 GMT  
		Size: 1.6 KB (1619 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b9dda8c314f6a9f00c80e8d3774028d4204d754e4c828c2c38917e39f649706`  
		Last Modified: Thu, 09 Feb 2023 09:31:13 GMT  
		Size: 926.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed7b5d79a1e160a892ae3ca9a3585b9a3859b3843800b146b50a6f8dc2e37cea`  
		Last Modified: Thu, 09 Feb 2023 09:31:18 GMT  
		Size: 5.7 MB (5705255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e3972972765aa157621d8d380622fd6d29b61d44fd1b960930a1847ba23bfbb`  
		Last Modified: Thu, 09 Feb 2023 09:31:13 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc249832f7bdc107bfaebf38fb0292b7cacb7518cba7bad019f0d8ff699994c4`  
		Last Modified: Thu, 09 Feb 2023 09:31:13 GMT  
		Size: 345.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; ppc64le

```console
$ docker pull spiped@sha256:c55bb97521e65594872fe76cbfbc246cf4f6f31b3851f51ee61256ba623233de
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.3 MB (41292154 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2584a0abea40abb2a074488d4046bfa1ee2358d7221dcaada6120144742c42a9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 09 Feb 2023 06:21:49 GMT
ADD file:b09577b8131a90731fdfb00b824a97dc65ccb51d484cb9004382035d64a5741c in / 
# Thu, 09 Feb 2023 06:21:52 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 12:13:54 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Thu, 09 Feb 2023 12:14:00 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 12:14:00 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 09 Feb 2023 12:14:49 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 09 Feb 2023 12:14:50 GMT
VOLUME [/spiped]
# Thu, 09 Feb 2023 12:14:50 GMT
WORKDIR /spiped
# Thu, 09 Feb 2023 12:14:51 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 09 Feb 2023 12:14:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 09 Feb 2023 12:14:52 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:4ea90e1a094ae86c7950bbec99e7a79b08fae641ad5f3bc3af9081c925894c41`  
		Last Modified: Thu, 09 Feb 2023 06:28:27 GMT  
		Size: 35.3 MB (35289252 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:695fd45ccd8eac48da176341bba34201c9b8980634c1df9e9e8b4bfbfa220edc`  
		Last Modified: Thu, 09 Feb 2023 12:15:27 GMT  
		Size: 1.7 KB (1735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e02fb49a13103590e46d389b8e81a60bc1d01cbf4395c01b053e5e4e99f6e312`  
		Last Modified: Thu, 09 Feb 2023 12:15:27 GMT  
		Size: 1.0 KB (1049 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e9885ddc7088b14facf6e088ded644fc33dff7b4e6625a92eb87f71975a0703`  
		Last Modified: Thu, 09 Feb 2023 12:15:29 GMT  
		Size: 6.0 MB (5999645 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:300eee5c0fb43c90cd5a5c063707252fce74ce3a8ffc7fcd444c165dfb9753a9`  
		Last Modified: Thu, 09 Feb 2023 12:15:27 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e97c03ba3e8494c9ba2cb5d8837cbdf9d4f38177151f3c344b5459888bc9a2af`  
		Last Modified: Thu, 09 Feb 2023 12:15:27 GMT  
		Size: 344.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; s390x

```console
$ docker pull spiped@sha256:6763f80ffafaec400a9c32713f12023d7cfc9221fe27ded8e22f7668b5695825
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.8 MB (34837535 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e585d1138d7b913b469d1d60a8169d148407b55e74a2ae2fa3670406899e2703`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 01 Mar 2023 02:50:30 GMT
ADD file:01aa3de7444f0716938e0d85522be065193be4ffb6788b3190a0f4fefdbb8d65 in / 
# Wed, 01 Mar 2023 02:50:31 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 09:59:36 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 01 Mar 2023 09:59:39 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 09:59:39 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 01 Mar 2023 09:59:51 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 01 Mar 2023 09:59:51 GMT
VOLUME [/spiped]
# Wed, 01 Mar 2023 09:59:52 GMT
WORKDIR /spiped
# Wed, 01 Mar 2023 09:59:52 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 01 Mar 2023 09:59:52 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 01 Mar 2023 09:59:52 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:7b8d78f42e32e7fa234bcf890ae6603acab2881bca68a9d8c429981c7f42b1d6`  
		Last Modified: Wed, 01 Mar 2023 02:54:48 GMT  
		Size: 29.6 MB (29646854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:407e05b7731593d7281e5af1c1859fd2d47d7464ad6c5dc03ac8c8155a85e98d`  
		Last Modified: Wed, 01 Mar 2023 10:00:28 GMT  
		Size: 1.7 KB (1738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74698444aa451ceea677ff79b9924fe3f417d089f80b716455e9685ecc1306cc`  
		Last Modified: Wed, 01 Mar 2023 10:00:28 GMT  
		Size: 1.1 KB (1055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1e70e3b82bb8b17253bfb319a8144075d6a620afff629c1d1ea44ed93fe7ae2`  
		Last Modified: Wed, 01 Mar 2023 10:00:29 GMT  
		Size: 5.2 MB (5187420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fc09ee195f0d0c9a66b36017beedcd1c8bb0eeed0bc93753b944e58a218b522`  
		Last Modified: Wed, 01 Mar 2023 10:00:28 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cb0d5fb8ca92c7b1a4e4c6943edcc6e6afba039da0f1f566df5c8f887bd2b17`  
		Last Modified: Wed, 01 Mar 2023 10:00:28 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
