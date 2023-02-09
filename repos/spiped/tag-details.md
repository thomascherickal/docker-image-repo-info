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
$ docker pull spiped@sha256:36792922d2b08e1d321e2dbc07eca0f7ee6b7477a145b88bc02a54c493712763
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
$ docker pull spiped@sha256:4a8875107a0ae5b2a99a15a14d48ebeb0053b2d6fc7f9539eb0d2a223121d98e
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.9 MB (33947843 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d002918607a70e5bef0dd6d3afe1b10e682eb276fd30be897c5102a77a6dfe82`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 09 Feb 2023 02:00:32 GMT
ADD file:fcf4deede0eb98d96d8657dfb1b0918a2c3d35f16d4858dd9e75c843edeff166 in / 
# Thu, 09 Feb 2023 02:00:33 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 07:42:30 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Thu, 09 Feb 2023 07:42:35 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 07:42:35 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 09 Feb 2023 07:42:56 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 09 Feb 2023 07:42:56 GMT
VOLUME [/spiped]
# Thu, 09 Feb 2023 07:42:56 GMT
WORKDIR /spiped
# Thu, 09 Feb 2023 07:42:56 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 09 Feb 2023 07:42:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 09 Feb 2023 07:42:56 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:886a7482403a267f98b84e4a9f9ede516bac1fe7eb82ff570dabbb0b297d5b53`  
		Last Modified: Thu, 09 Feb 2023 02:05:42 GMT  
		Size: 28.9 MB (28916292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f0b4c916377c6dbb908da122fa96bfa0ce286cc9da628adef55639296163add`  
		Last Modified: Thu, 09 Feb 2023 07:43:14 GMT  
		Size: 1.7 KB (1730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:067ecc9df0a048cbcda29c8daee40da43959b1c7053eda96b2a81b869cecb54d`  
		Last Modified: Thu, 09 Feb 2023 07:43:15 GMT  
		Size: 1.0 KB (1023 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31a0779e11296c1c17feadfa2d00251940d442709616b2f2ad4761144806351b`  
		Last Modified: Thu, 09 Feb 2023 07:43:15 GMT  
		Size: 5.0 MB (5028362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fa3cff81fceb3cb7558134cae0d1dd81dd0687cc27dc747d8a38c557b289787`  
		Last Modified: Thu, 09 Feb 2023 07:43:14 GMT  
		Size: 92.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ec878da2996777c7363b616dfbe74e27b6506978d8674a1883c3cb4690921d3`  
		Last Modified: Thu, 09 Feb 2023 07:43:14 GMT  
		Size: 344.0 B  
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
$ docker pull spiped@sha256:c412ab17dbe7c382e310a9a62f8cfb32bc706a2a9f03ba267b24ee44bb6830fd
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.8 MB (34838196 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:009dd6f9dd0b116d48899f5168c6848918483e4be4b6f7797ccf9c37d1c65f40`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 09 Feb 2023 02:41:45 GMT
ADD file:dc3c16b50baeac5b9644e607c8df9606e9583f8598e3ba34bcdd69c669a5904c in / 
# Thu, 09 Feb 2023 02:41:46 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 04:29:04 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Thu, 09 Feb 2023 04:29:06 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 04:29:06 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 09 Feb 2023 04:29:19 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 09 Feb 2023 04:29:19 GMT
VOLUME [/spiped]
# Thu, 09 Feb 2023 04:29:19 GMT
WORKDIR /spiped
# Thu, 09 Feb 2023 04:29:20 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 09 Feb 2023 04:29:20 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 09 Feb 2023 04:29:20 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:c2f78940fdfbfc5ce5d1d3cff3c27a319451aeb3ec12ff2473073516907fbce9`  
		Last Modified: Thu, 09 Feb 2023 02:46:06 GMT  
		Size: 29.6 MB (29647513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68bbc75b754860161ae6344fc9d8438ebb45bf74a809cf2eacc1eed1f69360f5`  
		Last Modified: Thu, 09 Feb 2023 04:29:50 GMT  
		Size: 1.7 KB (1740 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1ed99a2553aedd84386b5162ec3d7cbd85e263d67a7f880f0c22455ffc703ba`  
		Last Modified: Thu, 09 Feb 2023 04:29:50 GMT  
		Size: 1.1 KB (1051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db7bd105f0e3167c684db4a568d0891a9f72b7680fb5acc641f111250789be6d`  
		Last Modified: Thu, 09 Feb 2023 04:29:51 GMT  
		Size: 5.2 MB (5187421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9be9021fdd8bee9e348b198d87e955c3786ae17048cf4acbcd219b030ba7f369`  
		Last Modified: Thu, 09 Feb 2023 04:29:50 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91bc0b6a48c2e0be6fe8929b92f3fb8b514edc9ba7564792af2d1553b598a035`  
		Last Modified: Thu, 09 Feb 2023 04:29:50 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:1-alpine`

```console
$ docker pull spiped@sha256:e8982ce4c33ed5c5fdf992ccf6c890b82d7806e41d8778ea6777610d0e4e4719
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
$ docker pull spiped@sha256:8eb40fb8e554b827563f599dd3e61da57293486cae87cd856a891b4e8dba353e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.1 MB (5075384 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2dda802d4535ce910f8e00126e80c79abb0825f3bf7caf66a4bb950cb589cc74`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Mon, 09 Jan 2023 17:05:20 GMT
ADD file:e4d600fc4c9c293efe360be7b30ee96579925d1b4634c94332e2ec73f7d8eca1 in / 
# Mon, 09 Jan 2023 17:05:20 GMT
CMD ["/bin/sh"]
# Mon, 09 Jan 2023 20:03:04 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Mon, 09 Jan 2023 20:03:05 GMT
RUN apk add --no-cache libssl1.1
# Mon, 09 Jan 2023 20:03:05 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Mon, 09 Jan 2023 20:03:16 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Mon, 09 Jan 2023 20:03:16 GMT
VOLUME [/spiped]
# Mon, 09 Jan 2023 20:03:16 GMT
WORKDIR /spiped
# Mon, 09 Jan 2023 20:03:16 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 09 Jan 2023 20:03:16 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 09 Jan 2023 20:03:16 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:8921db27df2831fa6eaa85321205a2470c669b855f3ec95d5a3c2b46de0442c9`  
		Last Modified: Mon, 09 Jan 2023 17:05:45 GMT  
		Size: 3.4 MB (3370628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e9fb896348696d642ef5674956097b03540bea28f8454d6287f5d9cb10b5b19`  
		Last Modified: Mon, 09 Jan 2023 20:03:32 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f1fb67340ae0e377cfa3a1ee1218a1ba6d31cf9f7cb2a302542d4354c848991`  
		Last Modified: Mon, 09 Jan 2023 20:03:33 GMT  
		Size: 1.5 MB (1481738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e228854dc2c8d78fdfe84ed1b99903b8567e21eff2fcf86757e6fdfa823872a`  
		Last Modified: Mon, 09 Jan 2023 20:03:32 GMT  
		Size: 221.3 KB (221283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f486af83d26d338661f9edfe85a3574704c4d8e4a08cdea692294588749dde0`  
		Last Modified: Mon, 09 Jan 2023 20:03:32 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35820a44b4998d9547534e80870c2e2a59cad7f381a4d6a82609d3f67126045d`  
		Last Modified: Mon, 09 Jan 2023 20:03:32 GMT  
		Size: 338.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; arm variant v6

```console
$ docker pull spiped@sha256:cb751a21eae14bec751c4cd688311f6eafc98d6d1769aa245711e63d7182e21a
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.6 MB (4554176 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:341ba40bb3f41e998727f9c4967f67b001703e78dafe41ad92a70bf2791fca9b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Mon, 09 Jan 2023 17:04:54 GMT
ADD file:b15fd8e9f996815394e25f20c8459bfb4c2a8c4074592d6f4c75f4fe79ce537e in / 
# Mon, 09 Jan 2023 17:04:55 GMT
CMD ["/bin/sh"]
# Mon, 09 Jan 2023 20:52:14 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Mon, 09 Jan 2023 20:52:16 GMT
RUN apk add --no-cache libssl1.1
# Mon, 09 Jan 2023 20:52:16 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Mon, 09 Jan 2023 20:52:25 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Mon, 09 Jan 2023 20:52:25 GMT
VOLUME [/spiped]
# Mon, 09 Jan 2023 20:52:25 GMT
WORKDIR /spiped
# Mon, 09 Jan 2023 20:52:25 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 09 Jan 2023 20:52:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 09 Jan 2023 20:52:25 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:0269c10e600f3a375f36ddabdbd264ce9503a455f0d0969ce8a00f24eaecc032`  
		Last Modified: Mon, 09 Jan 2023 17:05:45 GMT  
		Size: 3.1 MB (3107243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9fcf4fe7db4264a8e664de4d52478f1d4ba98146c38a7672ed85c122a2ec9ea`  
		Last Modified: Mon, 09 Jan 2023 20:52:44 GMT  
		Size: 1.2 KB (1242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:252aa0c5aa375a984c376376752105d7908cccb2ad2078305d2f12c857e58688`  
		Last Modified: Mon, 09 Jan 2023 20:52:45 GMT  
		Size: 1.2 MB (1238925 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90bcc6c04b36698f2894107a3dcd168ebf74dcadfaada1feb7c909e6d7d2e48c`  
		Last Modified: Mon, 09 Jan 2023 20:52:45 GMT  
		Size: 206.3 KB (206330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac2b1d7fdda8e63c8009adec27201adf5aef01cb0be8ae5e126525f70f6ff253`  
		Last Modified: Mon, 09 Jan 2023 20:52:44 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3cc764eff90255e712b5e4a850166371f439ffce5e23ec5a3902aeca546fce4`  
		Last Modified: Mon, 09 Jan 2023 20:52:44 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; arm variant v7

```console
$ docker pull spiped@sha256:5350876a3890b8b4c1a7262c4c48345b4046feb2b93df0f849b165f6d3862d43
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4233507 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5a136cbdcf03b9c140acc83ef95bd48dcdb73507ee82d16eed4339281865ff3e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Mon, 09 Jan 2023 17:06:27 GMT
ADD file:4696f25d0f019b27457c55b3b128b70bf153f38e3e4eb5bdfc21058543313e94 in / 
# Mon, 09 Jan 2023 17:06:27 GMT
CMD ["/bin/sh"]
# Tue, 10 Jan 2023 01:03:19 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Tue, 10 Jan 2023 01:03:20 GMT
RUN apk add --no-cache libssl1.1
# Tue, 10 Jan 2023 01:03:21 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 10 Jan 2023 01:03:29 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Tue, 10 Jan 2023 01:03:29 GMT
VOLUME [/spiped]
# Tue, 10 Jan 2023 01:03:29 GMT
WORKDIR /spiped
# Tue, 10 Jan 2023 01:03:29 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 10 Jan 2023 01:03:29 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 10 Jan 2023 01:03:29 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:c527615e4ffa2d5b9b777fd469b3b5ba7c1b1e9201c065be2c43569de48a3754`  
		Last Modified: Mon, 09 Jan 2023 17:07:17 GMT  
		Size: 2.9 MB (2865208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c30dc917313d61894ccb7cfad12c5f3a278e251ca506df448c9f8e2a16ba910`  
		Last Modified: Tue, 10 Jan 2023 01:04:01 GMT  
		Size: 1.2 KB (1241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b4704616a59a25f4e6a3979312202c02302fb7db16765696efeaf0136d5d871`  
		Last Modified: Tue, 10 Jan 2023 01:04:01 GMT  
		Size: 1.2 MB (1166534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d943eecb9e0495c260d5786a0e7109c2f3f4c07c93eed00e71667a8fd3cd0a7`  
		Last Modified: Tue, 10 Jan 2023 01:04:01 GMT  
		Size: 200.1 KB (200087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30309affe27d04051a0e8f9d361029624d0957f51f95f351a76921b3d10aa00e`  
		Last Modified: Tue, 10 Jan 2023 01:04:01 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40cb5d940651ed07d3a8a9b5d7bb45557f66f56eb842f0db2c34496a0b49b3be`  
		Last Modified: Tue, 10 Jan 2023 01:04:01 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:0213ccc252b274961ca65d4810e3e3adbfd0a45802938a1fc17b5260a5766747
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.8 MB (4838993 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5f334562e83a3560fd096b7555b628adde3f65f35e7d7f88d92cef036aa3b80e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Mon, 09 Jan 2023 17:04:48 GMT
ADD file:3080f19f39259a4b77cc53975de0184c78d4335ceb9ffb77a2838d0539ad6f85 in / 
# Mon, 09 Jan 2023 17:04:49 GMT
CMD ["/bin/sh"]
# Mon, 09 Jan 2023 21:54:38 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Mon, 09 Jan 2023 21:54:40 GMT
RUN apk add --no-cache libssl1.1
# Mon, 09 Jan 2023 21:54:40 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Mon, 09 Jan 2023 21:54:48 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Mon, 09 Jan 2023 21:54:48 GMT
VOLUME [/spiped]
# Mon, 09 Jan 2023 21:54:48 GMT
WORKDIR /spiped
# Mon, 09 Jan 2023 21:54:48 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 09 Jan 2023 21:54:48 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 09 Jan 2023 21:54:48 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:a9eaa45ef418e883481a13c7d84fa9904f2ec56789c52a87ba5a9e6483f2b74f`  
		Last Modified: Mon, 09 Jan 2023 17:05:12 GMT  
		Size: 3.3 MB (3259241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8a57c503886d17fc3a18ad5ac652d01a19c1d114d10d95fbbb6962eb5141a3c`  
		Last Modified: Mon, 09 Jan 2023 21:55:05 GMT  
		Size: 1.3 KB (1266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7deb227b2dbf5691407192d6e6164c40a313d06c2d63a713bcec3bfb588a82f1`  
		Last Modified: Mon, 09 Jan 2023 21:55:05 GMT  
		Size: 1.4 MB (1362327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:136d1ea11d30612c79aa77675c78fb75feede08c3a75327ad85af71c6acc55cc`  
		Last Modified: Mon, 09 Jan 2023 21:55:05 GMT  
		Size: 215.7 KB (215692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12c3012f3cfaea50c1e653e77ff8a01ac59681255c473f52fc3d3087f2ec06f1`  
		Last Modified: Mon, 09 Jan 2023 21:55:05 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78ff7343264af5878ae4a177e19ca1bc3ef5ed246ba09fa1c3c6e4e80c2c09b2`  
		Last Modified: Mon, 09 Jan 2023 21:55:05 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; 386

```console
$ docker pull spiped@sha256:d8a38312632b028320e1705047e9f772afc0badca532e45181c287df1ef83910
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.1 MB (5125102 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8462fd88246d8334a88562d226243c2b45ed34c1f68d1e222efac09016792383`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Mon, 09 Jan 2023 17:05:00 GMT
ADD file:d03619a0ef81726c34189e849b80cc92da908eb36e116f28275d5765e6d0919a in / 
# Mon, 09 Jan 2023 17:05:00 GMT
CMD ["/bin/sh"]
# Mon, 09 Jan 2023 19:07:22 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Mon, 09 Jan 2023 19:07:24 GMT
RUN apk add --no-cache libssl1.1
# Mon, 09 Jan 2023 19:07:25 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Mon, 09 Jan 2023 19:07:36 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Mon, 09 Jan 2023 19:07:37 GMT
VOLUME [/spiped]
# Mon, 09 Jan 2023 19:07:38 GMT
WORKDIR /spiped
# Mon, 09 Jan 2023 19:07:40 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 09 Jan 2023 19:07:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 09 Jan 2023 19:07:41 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:40e5b0b2e2bde18974628cadecd8a2f190f45f06c32846c16885d69b2908bf68`  
		Last Modified: Mon, 09 Jan 2023 17:05:42 GMT  
		Size: 3.4 MB (3408318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:beb4d578ecfd8ec0e5b44d6f231ae75cd33c39c4d21f5b01b80e80019344904e`  
		Last Modified: Mon, 09 Jan 2023 19:08:10 GMT  
		Size: 1.2 KB (1240 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d5141406d2cea5667b65a83cfc84fe7c8eef2aa49d6c549ec8acb7e97c32f89`  
		Last Modified: Mon, 09 Jan 2023 19:08:10 GMT  
		Size: 1.5 MB (1483729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ac653492946b43047544c01ac378096ae6c6d8856996b5de736547a2fafaf68`  
		Last Modified: Mon, 09 Jan 2023 19:08:10 GMT  
		Size: 231.4 KB (231382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95e2203d634caaf6243a81ca591d7aa9c925d62488c2290d0d6c57a46eeac8f8`  
		Last Modified: Mon, 09 Jan 2023 19:08:10 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb7ad0075ba728f545bdda81f2b8cc4d645b41f8ab2dac39cebca27927c444b2`  
		Last Modified: Mon, 09 Jan 2023 19:08:10 GMT  
		Size: 338.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; ppc64le

```console
$ docker pull spiped@sha256:6287dba41a56cf9c39be27c62b7a3bde3479b303d63e9230b446113020881fa9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.0 MB (5017699 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2ef59306a962c0b86d594be1281ca3dd3e91c0b16a046ee09218d60231e3a9cb`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Mon, 09 Jan 2023 17:05:13 GMT
ADD file:9a1d27fdc0c915f387f2446c85193d5215b18020b313114f0bf2799efcc1baae in / 
# Mon, 09 Jan 2023 17:05:13 GMT
CMD ["/bin/sh"]
# Mon, 09 Jan 2023 21:32:14 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Mon, 09 Jan 2023 21:32:16 GMT
RUN apk add --no-cache libssl1.1
# Mon, 09 Jan 2023 21:32:16 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Mon, 09 Jan 2023 21:32:30 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Mon, 09 Jan 2023 21:32:31 GMT
VOLUME [/spiped]
# Mon, 09 Jan 2023 21:32:31 GMT
WORKDIR /spiped
# Mon, 09 Jan 2023 21:32:32 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 09 Jan 2023 21:32:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 09 Jan 2023 21:32:32 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:f45bfda3aa14e255d9eb4c9a108eb3d8c6721946b4aa2e5808e5092242344a1c`  
		Last Modified: Mon, 09 Jan 2023 17:05:56 GMT  
		Size: 3.4 MB (3384562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd46f789ced0eaea980007a2e6a0f6b02b7711749489fdc0a30de08d248c3325`  
		Last Modified: Mon, 09 Jan 2023 21:33:00 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cc9ef36d078710c0c6d69a2d1c19bc6701be12e5c554ec9fa1546fe495e59eb`  
		Last Modified: Mon, 09 Jan 2023 21:32:59 GMT  
		Size: 1.4 MB (1411372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9e8744b0f13a67b1002a7a426a2b3635f0b4a28fd095ef061c0f1fd5d85d909`  
		Last Modified: Mon, 09 Jan 2023 21:32:59 GMT  
		Size: 220.0 KB (220028 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cc209dab70185705e5eee1e1710197c9bc735498e476d6719c4b850ae44fdaa`  
		Last Modified: Mon, 09 Jan 2023 21:32:59 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe41dcc405bef6ddd7bb480eadf45d92a9cfd583bee884d68eb41037c93e1e23`  
		Last Modified: Mon, 09 Jan 2023 21:32:59 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; s390x

```console
$ docker pull spiped@sha256:5a87be0c5f3e288adf33abd9c67087730cd729e12ac28ae4b107955683edff20
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.6 MB (4602294 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:63961a94a731d4f9e0005f5fd83043126c5546496fa856ea125a5c2e51c6979c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Mon, 09 Jan 2023 17:05:44 GMT
ADD file:eabe7c3c368e65478b53ac35c1daf3b703f2bca4ecdab2d080a65e8b981d7d4a in / 
# Mon, 09 Jan 2023 17:05:46 GMT
CMD ["/bin/sh"]
# Tue, 10 Jan 2023 01:32:49 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Tue, 10 Jan 2023 01:32:52 GMT
RUN apk add --no-cache libssl1.1
# Tue, 10 Jan 2023 01:32:52 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 10 Jan 2023 01:33:01 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Tue, 10 Jan 2023 01:33:02 GMT
VOLUME [/spiped]
# Tue, 10 Jan 2023 01:33:03 GMT
WORKDIR /spiped
# Tue, 10 Jan 2023 01:33:03 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 10 Jan 2023 01:33:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 10 Jan 2023 01:33:05 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:ae982806674c51a962c0fdd6e19f464ebd673df529c5cfb7c1d049e0b618d384`  
		Last Modified: Mon, 09 Jan 2023 17:06:50 GMT  
		Size: 3.2 MB (3170744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f659d5259c21b4ce33d18c83c0251b9d66d58281847f63904bed75a5683b3fde`  
		Last Modified: Tue, 10 Jan 2023 01:33:39 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9decaf35186276ee535aac72c69938baded768609a2bb148ca4d5c0a1788a984`  
		Last Modified: Tue, 10 Jan 2023 01:33:39 GMT  
		Size: 1.2 MB (1221175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93194a8cc16c2fcd24da284630284cd3fbf877fc323c8dc65e3d256d777ac04a`  
		Last Modified: Tue, 10 Jan 2023 01:33:39 GMT  
		Size: 208.6 KB (208637 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02decf839b354e56295448b1f40e50f813a1879598a091e766908a8f70b21671`  
		Last Modified: Tue, 10 Jan 2023 01:33:39 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07f2035a6bfb730bee20ac317d153b1061a4002ce6a450bb74f34bebcfa04369`  
		Last Modified: Tue, 10 Jan 2023 01:33:39 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:1.6`

```console
$ docker pull spiped@sha256:36792922d2b08e1d321e2dbc07eca0f7ee6b7477a145b88bc02a54c493712763
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
$ docker pull spiped@sha256:4a8875107a0ae5b2a99a15a14d48ebeb0053b2d6fc7f9539eb0d2a223121d98e
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.9 MB (33947843 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d002918607a70e5bef0dd6d3afe1b10e682eb276fd30be897c5102a77a6dfe82`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 09 Feb 2023 02:00:32 GMT
ADD file:fcf4deede0eb98d96d8657dfb1b0918a2c3d35f16d4858dd9e75c843edeff166 in / 
# Thu, 09 Feb 2023 02:00:33 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 07:42:30 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Thu, 09 Feb 2023 07:42:35 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 07:42:35 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 09 Feb 2023 07:42:56 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 09 Feb 2023 07:42:56 GMT
VOLUME [/spiped]
# Thu, 09 Feb 2023 07:42:56 GMT
WORKDIR /spiped
# Thu, 09 Feb 2023 07:42:56 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 09 Feb 2023 07:42:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 09 Feb 2023 07:42:56 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:886a7482403a267f98b84e4a9f9ede516bac1fe7eb82ff570dabbb0b297d5b53`  
		Last Modified: Thu, 09 Feb 2023 02:05:42 GMT  
		Size: 28.9 MB (28916292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f0b4c916377c6dbb908da122fa96bfa0ce286cc9da628adef55639296163add`  
		Last Modified: Thu, 09 Feb 2023 07:43:14 GMT  
		Size: 1.7 KB (1730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:067ecc9df0a048cbcda29c8daee40da43959b1c7053eda96b2a81b869cecb54d`  
		Last Modified: Thu, 09 Feb 2023 07:43:15 GMT  
		Size: 1.0 KB (1023 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31a0779e11296c1c17feadfa2d00251940d442709616b2f2ad4761144806351b`  
		Last Modified: Thu, 09 Feb 2023 07:43:15 GMT  
		Size: 5.0 MB (5028362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fa3cff81fceb3cb7558134cae0d1dd81dd0687cc27dc747d8a38c557b289787`  
		Last Modified: Thu, 09 Feb 2023 07:43:14 GMT  
		Size: 92.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ec878da2996777c7363b616dfbe74e27b6506978d8674a1883c3cb4690921d3`  
		Last Modified: Thu, 09 Feb 2023 07:43:14 GMT  
		Size: 344.0 B  
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
$ docker pull spiped@sha256:c412ab17dbe7c382e310a9a62f8cfb32bc706a2a9f03ba267b24ee44bb6830fd
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.8 MB (34838196 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:009dd6f9dd0b116d48899f5168c6848918483e4be4b6f7797ccf9c37d1c65f40`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 09 Feb 2023 02:41:45 GMT
ADD file:dc3c16b50baeac5b9644e607c8df9606e9583f8598e3ba34bcdd69c669a5904c in / 
# Thu, 09 Feb 2023 02:41:46 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 04:29:04 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Thu, 09 Feb 2023 04:29:06 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 04:29:06 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 09 Feb 2023 04:29:19 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 09 Feb 2023 04:29:19 GMT
VOLUME [/spiped]
# Thu, 09 Feb 2023 04:29:19 GMT
WORKDIR /spiped
# Thu, 09 Feb 2023 04:29:20 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 09 Feb 2023 04:29:20 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 09 Feb 2023 04:29:20 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:c2f78940fdfbfc5ce5d1d3cff3c27a319451aeb3ec12ff2473073516907fbce9`  
		Last Modified: Thu, 09 Feb 2023 02:46:06 GMT  
		Size: 29.6 MB (29647513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68bbc75b754860161ae6344fc9d8438ebb45bf74a809cf2eacc1eed1f69360f5`  
		Last Modified: Thu, 09 Feb 2023 04:29:50 GMT  
		Size: 1.7 KB (1740 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1ed99a2553aedd84386b5162ec3d7cbd85e263d67a7f880f0c22455ffc703ba`  
		Last Modified: Thu, 09 Feb 2023 04:29:50 GMT  
		Size: 1.1 KB (1051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db7bd105f0e3167c684db4a568d0891a9f72b7680fb5acc641f111250789be6d`  
		Last Modified: Thu, 09 Feb 2023 04:29:51 GMT  
		Size: 5.2 MB (5187421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9be9021fdd8bee9e348b198d87e955c3786ae17048cf4acbcd219b030ba7f369`  
		Last Modified: Thu, 09 Feb 2023 04:29:50 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91bc0b6a48c2e0be6fe8929b92f3fb8b514edc9ba7564792af2d1553b598a035`  
		Last Modified: Thu, 09 Feb 2023 04:29:50 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:1.6-alpine`

```console
$ docker pull spiped@sha256:e8982ce4c33ed5c5fdf992ccf6c890b82d7806e41d8778ea6777610d0e4e4719
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
$ docker pull spiped@sha256:8eb40fb8e554b827563f599dd3e61da57293486cae87cd856a891b4e8dba353e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.1 MB (5075384 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2dda802d4535ce910f8e00126e80c79abb0825f3bf7caf66a4bb950cb589cc74`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Mon, 09 Jan 2023 17:05:20 GMT
ADD file:e4d600fc4c9c293efe360be7b30ee96579925d1b4634c94332e2ec73f7d8eca1 in / 
# Mon, 09 Jan 2023 17:05:20 GMT
CMD ["/bin/sh"]
# Mon, 09 Jan 2023 20:03:04 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Mon, 09 Jan 2023 20:03:05 GMT
RUN apk add --no-cache libssl1.1
# Mon, 09 Jan 2023 20:03:05 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Mon, 09 Jan 2023 20:03:16 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Mon, 09 Jan 2023 20:03:16 GMT
VOLUME [/spiped]
# Mon, 09 Jan 2023 20:03:16 GMT
WORKDIR /spiped
# Mon, 09 Jan 2023 20:03:16 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 09 Jan 2023 20:03:16 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 09 Jan 2023 20:03:16 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:8921db27df2831fa6eaa85321205a2470c669b855f3ec95d5a3c2b46de0442c9`  
		Last Modified: Mon, 09 Jan 2023 17:05:45 GMT  
		Size: 3.4 MB (3370628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e9fb896348696d642ef5674956097b03540bea28f8454d6287f5d9cb10b5b19`  
		Last Modified: Mon, 09 Jan 2023 20:03:32 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f1fb67340ae0e377cfa3a1ee1218a1ba6d31cf9f7cb2a302542d4354c848991`  
		Last Modified: Mon, 09 Jan 2023 20:03:33 GMT  
		Size: 1.5 MB (1481738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e228854dc2c8d78fdfe84ed1b99903b8567e21eff2fcf86757e6fdfa823872a`  
		Last Modified: Mon, 09 Jan 2023 20:03:32 GMT  
		Size: 221.3 KB (221283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f486af83d26d338661f9edfe85a3574704c4d8e4a08cdea692294588749dde0`  
		Last Modified: Mon, 09 Jan 2023 20:03:32 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35820a44b4998d9547534e80870c2e2a59cad7f381a4d6a82609d3f67126045d`  
		Last Modified: Mon, 09 Jan 2023 20:03:32 GMT  
		Size: 338.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; arm variant v6

```console
$ docker pull spiped@sha256:cb751a21eae14bec751c4cd688311f6eafc98d6d1769aa245711e63d7182e21a
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.6 MB (4554176 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:341ba40bb3f41e998727f9c4967f67b001703e78dafe41ad92a70bf2791fca9b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Mon, 09 Jan 2023 17:04:54 GMT
ADD file:b15fd8e9f996815394e25f20c8459bfb4c2a8c4074592d6f4c75f4fe79ce537e in / 
# Mon, 09 Jan 2023 17:04:55 GMT
CMD ["/bin/sh"]
# Mon, 09 Jan 2023 20:52:14 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Mon, 09 Jan 2023 20:52:16 GMT
RUN apk add --no-cache libssl1.1
# Mon, 09 Jan 2023 20:52:16 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Mon, 09 Jan 2023 20:52:25 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Mon, 09 Jan 2023 20:52:25 GMT
VOLUME [/spiped]
# Mon, 09 Jan 2023 20:52:25 GMT
WORKDIR /spiped
# Mon, 09 Jan 2023 20:52:25 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 09 Jan 2023 20:52:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 09 Jan 2023 20:52:25 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:0269c10e600f3a375f36ddabdbd264ce9503a455f0d0969ce8a00f24eaecc032`  
		Last Modified: Mon, 09 Jan 2023 17:05:45 GMT  
		Size: 3.1 MB (3107243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9fcf4fe7db4264a8e664de4d52478f1d4ba98146c38a7672ed85c122a2ec9ea`  
		Last Modified: Mon, 09 Jan 2023 20:52:44 GMT  
		Size: 1.2 KB (1242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:252aa0c5aa375a984c376376752105d7908cccb2ad2078305d2f12c857e58688`  
		Last Modified: Mon, 09 Jan 2023 20:52:45 GMT  
		Size: 1.2 MB (1238925 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90bcc6c04b36698f2894107a3dcd168ebf74dcadfaada1feb7c909e6d7d2e48c`  
		Last Modified: Mon, 09 Jan 2023 20:52:45 GMT  
		Size: 206.3 KB (206330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac2b1d7fdda8e63c8009adec27201adf5aef01cb0be8ae5e126525f70f6ff253`  
		Last Modified: Mon, 09 Jan 2023 20:52:44 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3cc764eff90255e712b5e4a850166371f439ffce5e23ec5a3902aeca546fce4`  
		Last Modified: Mon, 09 Jan 2023 20:52:44 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; arm variant v7

```console
$ docker pull spiped@sha256:5350876a3890b8b4c1a7262c4c48345b4046feb2b93df0f849b165f6d3862d43
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4233507 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5a136cbdcf03b9c140acc83ef95bd48dcdb73507ee82d16eed4339281865ff3e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Mon, 09 Jan 2023 17:06:27 GMT
ADD file:4696f25d0f019b27457c55b3b128b70bf153f38e3e4eb5bdfc21058543313e94 in / 
# Mon, 09 Jan 2023 17:06:27 GMT
CMD ["/bin/sh"]
# Tue, 10 Jan 2023 01:03:19 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Tue, 10 Jan 2023 01:03:20 GMT
RUN apk add --no-cache libssl1.1
# Tue, 10 Jan 2023 01:03:21 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 10 Jan 2023 01:03:29 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Tue, 10 Jan 2023 01:03:29 GMT
VOLUME [/spiped]
# Tue, 10 Jan 2023 01:03:29 GMT
WORKDIR /spiped
# Tue, 10 Jan 2023 01:03:29 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 10 Jan 2023 01:03:29 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 10 Jan 2023 01:03:29 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:c527615e4ffa2d5b9b777fd469b3b5ba7c1b1e9201c065be2c43569de48a3754`  
		Last Modified: Mon, 09 Jan 2023 17:07:17 GMT  
		Size: 2.9 MB (2865208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c30dc917313d61894ccb7cfad12c5f3a278e251ca506df448c9f8e2a16ba910`  
		Last Modified: Tue, 10 Jan 2023 01:04:01 GMT  
		Size: 1.2 KB (1241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b4704616a59a25f4e6a3979312202c02302fb7db16765696efeaf0136d5d871`  
		Last Modified: Tue, 10 Jan 2023 01:04:01 GMT  
		Size: 1.2 MB (1166534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d943eecb9e0495c260d5786a0e7109c2f3f4c07c93eed00e71667a8fd3cd0a7`  
		Last Modified: Tue, 10 Jan 2023 01:04:01 GMT  
		Size: 200.1 KB (200087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30309affe27d04051a0e8f9d361029624d0957f51f95f351a76921b3d10aa00e`  
		Last Modified: Tue, 10 Jan 2023 01:04:01 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40cb5d940651ed07d3a8a9b5d7bb45557f66f56eb842f0db2c34496a0b49b3be`  
		Last Modified: Tue, 10 Jan 2023 01:04:01 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:0213ccc252b274961ca65d4810e3e3adbfd0a45802938a1fc17b5260a5766747
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.8 MB (4838993 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5f334562e83a3560fd096b7555b628adde3f65f35e7d7f88d92cef036aa3b80e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Mon, 09 Jan 2023 17:04:48 GMT
ADD file:3080f19f39259a4b77cc53975de0184c78d4335ceb9ffb77a2838d0539ad6f85 in / 
# Mon, 09 Jan 2023 17:04:49 GMT
CMD ["/bin/sh"]
# Mon, 09 Jan 2023 21:54:38 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Mon, 09 Jan 2023 21:54:40 GMT
RUN apk add --no-cache libssl1.1
# Mon, 09 Jan 2023 21:54:40 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Mon, 09 Jan 2023 21:54:48 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Mon, 09 Jan 2023 21:54:48 GMT
VOLUME [/spiped]
# Mon, 09 Jan 2023 21:54:48 GMT
WORKDIR /spiped
# Mon, 09 Jan 2023 21:54:48 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 09 Jan 2023 21:54:48 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 09 Jan 2023 21:54:48 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:a9eaa45ef418e883481a13c7d84fa9904f2ec56789c52a87ba5a9e6483f2b74f`  
		Last Modified: Mon, 09 Jan 2023 17:05:12 GMT  
		Size: 3.3 MB (3259241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8a57c503886d17fc3a18ad5ac652d01a19c1d114d10d95fbbb6962eb5141a3c`  
		Last Modified: Mon, 09 Jan 2023 21:55:05 GMT  
		Size: 1.3 KB (1266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7deb227b2dbf5691407192d6e6164c40a313d06c2d63a713bcec3bfb588a82f1`  
		Last Modified: Mon, 09 Jan 2023 21:55:05 GMT  
		Size: 1.4 MB (1362327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:136d1ea11d30612c79aa77675c78fb75feede08c3a75327ad85af71c6acc55cc`  
		Last Modified: Mon, 09 Jan 2023 21:55:05 GMT  
		Size: 215.7 KB (215692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12c3012f3cfaea50c1e653e77ff8a01ac59681255c473f52fc3d3087f2ec06f1`  
		Last Modified: Mon, 09 Jan 2023 21:55:05 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78ff7343264af5878ae4a177e19ca1bc3ef5ed246ba09fa1c3c6e4e80c2c09b2`  
		Last Modified: Mon, 09 Jan 2023 21:55:05 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; 386

```console
$ docker pull spiped@sha256:d8a38312632b028320e1705047e9f772afc0badca532e45181c287df1ef83910
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.1 MB (5125102 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8462fd88246d8334a88562d226243c2b45ed34c1f68d1e222efac09016792383`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Mon, 09 Jan 2023 17:05:00 GMT
ADD file:d03619a0ef81726c34189e849b80cc92da908eb36e116f28275d5765e6d0919a in / 
# Mon, 09 Jan 2023 17:05:00 GMT
CMD ["/bin/sh"]
# Mon, 09 Jan 2023 19:07:22 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Mon, 09 Jan 2023 19:07:24 GMT
RUN apk add --no-cache libssl1.1
# Mon, 09 Jan 2023 19:07:25 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Mon, 09 Jan 2023 19:07:36 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Mon, 09 Jan 2023 19:07:37 GMT
VOLUME [/spiped]
# Mon, 09 Jan 2023 19:07:38 GMT
WORKDIR /spiped
# Mon, 09 Jan 2023 19:07:40 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 09 Jan 2023 19:07:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 09 Jan 2023 19:07:41 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:40e5b0b2e2bde18974628cadecd8a2f190f45f06c32846c16885d69b2908bf68`  
		Last Modified: Mon, 09 Jan 2023 17:05:42 GMT  
		Size: 3.4 MB (3408318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:beb4d578ecfd8ec0e5b44d6f231ae75cd33c39c4d21f5b01b80e80019344904e`  
		Last Modified: Mon, 09 Jan 2023 19:08:10 GMT  
		Size: 1.2 KB (1240 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d5141406d2cea5667b65a83cfc84fe7c8eef2aa49d6c549ec8acb7e97c32f89`  
		Last Modified: Mon, 09 Jan 2023 19:08:10 GMT  
		Size: 1.5 MB (1483729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ac653492946b43047544c01ac378096ae6c6d8856996b5de736547a2fafaf68`  
		Last Modified: Mon, 09 Jan 2023 19:08:10 GMT  
		Size: 231.4 KB (231382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95e2203d634caaf6243a81ca591d7aa9c925d62488c2290d0d6c57a46eeac8f8`  
		Last Modified: Mon, 09 Jan 2023 19:08:10 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb7ad0075ba728f545bdda81f2b8cc4d645b41f8ab2dac39cebca27927c444b2`  
		Last Modified: Mon, 09 Jan 2023 19:08:10 GMT  
		Size: 338.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; ppc64le

```console
$ docker pull spiped@sha256:6287dba41a56cf9c39be27c62b7a3bde3479b303d63e9230b446113020881fa9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.0 MB (5017699 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2ef59306a962c0b86d594be1281ca3dd3e91c0b16a046ee09218d60231e3a9cb`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Mon, 09 Jan 2023 17:05:13 GMT
ADD file:9a1d27fdc0c915f387f2446c85193d5215b18020b313114f0bf2799efcc1baae in / 
# Mon, 09 Jan 2023 17:05:13 GMT
CMD ["/bin/sh"]
# Mon, 09 Jan 2023 21:32:14 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Mon, 09 Jan 2023 21:32:16 GMT
RUN apk add --no-cache libssl1.1
# Mon, 09 Jan 2023 21:32:16 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Mon, 09 Jan 2023 21:32:30 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Mon, 09 Jan 2023 21:32:31 GMT
VOLUME [/spiped]
# Mon, 09 Jan 2023 21:32:31 GMT
WORKDIR /spiped
# Mon, 09 Jan 2023 21:32:32 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 09 Jan 2023 21:32:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 09 Jan 2023 21:32:32 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:f45bfda3aa14e255d9eb4c9a108eb3d8c6721946b4aa2e5808e5092242344a1c`  
		Last Modified: Mon, 09 Jan 2023 17:05:56 GMT  
		Size: 3.4 MB (3384562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd46f789ced0eaea980007a2e6a0f6b02b7711749489fdc0a30de08d248c3325`  
		Last Modified: Mon, 09 Jan 2023 21:33:00 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cc9ef36d078710c0c6d69a2d1c19bc6701be12e5c554ec9fa1546fe495e59eb`  
		Last Modified: Mon, 09 Jan 2023 21:32:59 GMT  
		Size: 1.4 MB (1411372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9e8744b0f13a67b1002a7a426a2b3635f0b4a28fd095ef061c0f1fd5d85d909`  
		Last Modified: Mon, 09 Jan 2023 21:32:59 GMT  
		Size: 220.0 KB (220028 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cc209dab70185705e5eee1e1710197c9bc735498e476d6719c4b850ae44fdaa`  
		Last Modified: Mon, 09 Jan 2023 21:32:59 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe41dcc405bef6ddd7bb480eadf45d92a9cfd583bee884d68eb41037c93e1e23`  
		Last Modified: Mon, 09 Jan 2023 21:32:59 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; s390x

```console
$ docker pull spiped@sha256:5a87be0c5f3e288adf33abd9c67087730cd729e12ac28ae4b107955683edff20
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.6 MB (4602294 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:63961a94a731d4f9e0005f5fd83043126c5546496fa856ea125a5c2e51c6979c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Mon, 09 Jan 2023 17:05:44 GMT
ADD file:eabe7c3c368e65478b53ac35c1daf3b703f2bca4ecdab2d080a65e8b981d7d4a in / 
# Mon, 09 Jan 2023 17:05:46 GMT
CMD ["/bin/sh"]
# Tue, 10 Jan 2023 01:32:49 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Tue, 10 Jan 2023 01:32:52 GMT
RUN apk add --no-cache libssl1.1
# Tue, 10 Jan 2023 01:32:52 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 10 Jan 2023 01:33:01 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Tue, 10 Jan 2023 01:33:02 GMT
VOLUME [/spiped]
# Tue, 10 Jan 2023 01:33:03 GMT
WORKDIR /spiped
# Tue, 10 Jan 2023 01:33:03 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 10 Jan 2023 01:33:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 10 Jan 2023 01:33:05 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:ae982806674c51a962c0fdd6e19f464ebd673df529c5cfb7c1d049e0b618d384`  
		Last Modified: Mon, 09 Jan 2023 17:06:50 GMT  
		Size: 3.2 MB (3170744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f659d5259c21b4ce33d18c83c0251b9d66d58281847f63904bed75a5683b3fde`  
		Last Modified: Tue, 10 Jan 2023 01:33:39 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9decaf35186276ee535aac72c69938baded768609a2bb148ca4d5c0a1788a984`  
		Last Modified: Tue, 10 Jan 2023 01:33:39 GMT  
		Size: 1.2 MB (1221175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93194a8cc16c2fcd24da284630284cd3fbf877fc323c8dc65e3d256d777ac04a`  
		Last Modified: Tue, 10 Jan 2023 01:33:39 GMT  
		Size: 208.6 KB (208637 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02decf839b354e56295448b1f40e50f813a1879598a091e766908a8f70b21671`  
		Last Modified: Tue, 10 Jan 2023 01:33:39 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07f2035a6bfb730bee20ac317d153b1061a4002ce6a450bb74f34bebcfa04369`  
		Last Modified: Tue, 10 Jan 2023 01:33:39 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:1.6.2`

```console
$ docker pull spiped@sha256:36792922d2b08e1d321e2dbc07eca0f7ee6b7477a145b88bc02a54c493712763
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
$ docker pull spiped@sha256:4a8875107a0ae5b2a99a15a14d48ebeb0053b2d6fc7f9539eb0d2a223121d98e
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.9 MB (33947843 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d002918607a70e5bef0dd6d3afe1b10e682eb276fd30be897c5102a77a6dfe82`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 09 Feb 2023 02:00:32 GMT
ADD file:fcf4deede0eb98d96d8657dfb1b0918a2c3d35f16d4858dd9e75c843edeff166 in / 
# Thu, 09 Feb 2023 02:00:33 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 07:42:30 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Thu, 09 Feb 2023 07:42:35 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 07:42:35 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 09 Feb 2023 07:42:56 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 09 Feb 2023 07:42:56 GMT
VOLUME [/spiped]
# Thu, 09 Feb 2023 07:42:56 GMT
WORKDIR /spiped
# Thu, 09 Feb 2023 07:42:56 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 09 Feb 2023 07:42:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 09 Feb 2023 07:42:56 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:886a7482403a267f98b84e4a9f9ede516bac1fe7eb82ff570dabbb0b297d5b53`  
		Last Modified: Thu, 09 Feb 2023 02:05:42 GMT  
		Size: 28.9 MB (28916292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f0b4c916377c6dbb908da122fa96bfa0ce286cc9da628adef55639296163add`  
		Last Modified: Thu, 09 Feb 2023 07:43:14 GMT  
		Size: 1.7 KB (1730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:067ecc9df0a048cbcda29c8daee40da43959b1c7053eda96b2a81b869cecb54d`  
		Last Modified: Thu, 09 Feb 2023 07:43:15 GMT  
		Size: 1.0 KB (1023 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31a0779e11296c1c17feadfa2d00251940d442709616b2f2ad4761144806351b`  
		Last Modified: Thu, 09 Feb 2023 07:43:15 GMT  
		Size: 5.0 MB (5028362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fa3cff81fceb3cb7558134cae0d1dd81dd0687cc27dc747d8a38c557b289787`  
		Last Modified: Thu, 09 Feb 2023 07:43:14 GMT  
		Size: 92.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ec878da2996777c7363b616dfbe74e27b6506978d8674a1883c3cb4690921d3`  
		Last Modified: Thu, 09 Feb 2023 07:43:14 GMT  
		Size: 344.0 B  
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
$ docker pull spiped@sha256:c412ab17dbe7c382e310a9a62f8cfb32bc706a2a9f03ba267b24ee44bb6830fd
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.8 MB (34838196 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:009dd6f9dd0b116d48899f5168c6848918483e4be4b6f7797ccf9c37d1c65f40`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 09 Feb 2023 02:41:45 GMT
ADD file:dc3c16b50baeac5b9644e607c8df9606e9583f8598e3ba34bcdd69c669a5904c in / 
# Thu, 09 Feb 2023 02:41:46 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 04:29:04 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Thu, 09 Feb 2023 04:29:06 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 04:29:06 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 09 Feb 2023 04:29:19 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 09 Feb 2023 04:29:19 GMT
VOLUME [/spiped]
# Thu, 09 Feb 2023 04:29:19 GMT
WORKDIR /spiped
# Thu, 09 Feb 2023 04:29:20 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 09 Feb 2023 04:29:20 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 09 Feb 2023 04:29:20 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:c2f78940fdfbfc5ce5d1d3cff3c27a319451aeb3ec12ff2473073516907fbce9`  
		Last Modified: Thu, 09 Feb 2023 02:46:06 GMT  
		Size: 29.6 MB (29647513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68bbc75b754860161ae6344fc9d8438ebb45bf74a809cf2eacc1eed1f69360f5`  
		Last Modified: Thu, 09 Feb 2023 04:29:50 GMT  
		Size: 1.7 KB (1740 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1ed99a2553aedd84386b5162ec3d7cbd85e263d67a7f880f0c22455ffc703ba`  
		Last Modified: Thu, 09 Feb 2023 04:29:50 GMT  
		Size: 1.1 KB (1051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db7bd105f0e3167c684db4a568d0891a9f72b7680fb5acc641f111250789be6d`  
		Last Modified: Thu, 09 Feb 2023 04:29:51 GMT  
		Size: 5.2 MB (5187421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9be9021fdd8bee9e348b198d87e955c3786ae17048cf4acbcd219b030ba7f369`  
		Last Modified: Thu, 09 Feb 2023 04:29:50 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91bc0b6a48c2e0be6fe8929b92f3fb8b514edc9ba7564792af2d1553b598a035`  
		Last Modified: Thu, 09 Feb 2023 04:29:50 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:1.6.2-alpine`

```console
$ docker pull spiped@sha256:e8982ce4c33ed5c5fdf992ccf6c890b82d7806e41d8778ea6777610d0e4e4719
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
$ docker pull spiped@sha256:8eb40fb8e554b827563f599dd3e61da57293486cae87cd856a891b4e8dba353e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.1 MB (5075384 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2dda802d4535ce910f8e00126e80c79abb0825f3bf7caf66a4bb950cb589cc74`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Mon, 09 Jan 2023 17:05:20 GMT
ADD file:e4d600fc4c9c293efe360be7b30ee96579925d1b4634c94332e2ec73f7d8eca1 in / 
# Mon, 09 Jan 2023 17:05:20 GMT
CMD ["/bin/sh"]
# Mon, 09 Jan 2023 20:03:04 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Mon, 09 Jan 2023 20:03:05 GMT
RUN apk add --no-cache libssl1.1
# Mon, 09 Jan 2023 20:03:05 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Mon, 09 Jan 2023 20:03:16 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Mon, 09 Jan 2023 20:03:16 GMT
VOLUME [/spiped]
# Mon, 09 Jan 2023 20:03:16 GMT
WORKDIR /spiped
# Mon, 09 Jan 2023 20:03:16 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 09 Jan 2023 20:03:16 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 09 Jan 2023 20:03:16 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:8921db27df2831fa6eaa85321205a2470c669b855f3ec95d5a3c2b46de0442c9`  
		Last Modified: Mon, 09 Jan 2023 17:05:45 GMT  
		Size: 3.4 MB (3370628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e9fb896348696d642ef5674956097b03540bea28f8454d6287f5d9cb10b5b19`  
		Last Modified: Mon, 09 Jan 2023 20:03:32 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f1fb67340ae0e377cfa3a1ee1218a1ba6d31cf9f7cb2a302542d4354c848991`  
		Last Modified: Mon, 09 Jan 2023 20:03:33 GMT  
		Size: 1.5 MB (1481738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e228854dc2c8d78fdfe84ed1b99903b8567e21eff2fcf86757e6fdfa823872a`  
		Last Modified: Mon, 09 Jan 2023 20:03:32 GMT  
		Size: 221.3 KB (221283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f486af83d26d338661f9edfe85a3574704c4d8e4a08cdea692294588749dde0`  
		Last Modified: Mon, 09 Jan 2023 20:03:32 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35820a44b4998d9547534e80870c2e2a59cad7f381a4d6a82609d3f67126045d`  
		Last Modified: Mon, 09 Jan 2023 20:03:32 GMT  
		Size: 338.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.2-alpine` - linux; arm variant v6

```console
$ docker pull spiped@sha256:cb751a21eae14bec751c4cd688311f6eafc98d6d1769aa245711e63d7182e21a
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.6 MB (4554176 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:341ba40bb3f41e998727f9c4967f67b001703e78dafe41ad92a70bf2791fca9b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Mon, 09 Jan 2023 17:04:54 GMT
ADD file:b15fd8e9f996815394e25f20c8459bfb4c2a8c4074592d6f4c75f4fe79ce537e in / 
# Mon, 09 Jan 2023 17:04:55 GMT
CMD ["/bin/sh"]
# Mon, 09 Jan 2023 20:52:14 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Mon, 09 Jan 2023 20:52:16 GMT
RUN apk add --no-cache libssl1.1
# Mon, 09 Jan 2023 20:52:16 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Mon, 09 Jan 2023 20:52:25 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Mon, 09 Jan 2023 20:52:25 GMT
VOLUME [/spiped]
# Mon, 09 Jan 2023 20:52:25 GMT
WORKDIR /spiped
# Mon, 09 Jan 2023 20:52:25 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 09 Jan 2023 20:52:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 09 Jan 2023 20:52:25 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:0269c10e600f3a375f36ddabdbd264ce9503a455f0d0969ce8a00f24eaecc032`  
		Last Modified: Mon, 09 Jan 2023 17:05:45 GMT  
		Size: 3.1 MB (3107243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9fcf4fe7db4264a8e664de4d52478f1d4ba98146c38a7672ed85c122a2ec9ea`  
		Last Modified: Mon, 09 Jan 2023 20:52:44 GMT  
		Size: 1.2 KB (1242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:252aa0c5aa375a984c376376752105d7908cccb2ad2078305d2f12c857e58688`  
		Last Modified: Mon, 09 Jan 2023 20:52:45 GMT  
		Size: 1.2 MB (1238925 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90bcc6c04b36698f2894107a3dcd168ebf74dcadfaada1feb7c909e6d7d2e48c`  
		Last Modified: Mon, 09 Jan 2023 20:52:45 GMT  
		Size: 206.3 KB (206330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac2b1d7fdda8e63c8009adec27201adf5aef01cb0be8ae5e126525f70f6ff253`  
		Last Modified: Mon, 09 Jan 2023 20:52:44 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3cc764eff90255e712b5e4a850166371f439ffce5e23ec5a3902aeca546fce4`  
		Last Modified: Mon, 09 Jan 2023 20:52:44 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.2-alpine` - linux; arm variant v7

```console
$ docker pull spiped@sha256:5350876a3890b8b4c1a7262c4c48345b4046feb2b93df0f849b165f6d3862d43
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4233507 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5a136cbdcf03b9c140acc83ef95bd48dcdb73507ee82d16eed4339281865ff3e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Mon, 09 Jan 2023 17:06:27 GMT
ADD file:4696f25d0f019b27457c55b3b128b70bf153f38e3e4eb5bdfc21058543313e94 in / 
# Mon, 09 Jan 2023 17:06:27 GMT
CMD ["/bin/sh"]
# Tue, 10 Jan 2023 01:03:19 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Tue, 10 Jan 2023 01:03:20 GMT
RUN apk add --no-cache libssl1.1
# Tue, 10 Jan 2023 01:03:21 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 10 Jan 2023 01:03:29 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Tue, 10 Jan 2023 01:03:29 GMT
VOLUME [/spiped]
# Tue, 10 Jan 2023 01:03:29 GMT
WORKDIR /spiped
# Tue, 10 Jan 2023 01:03:29 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 10 Jan 2023 01:03:29 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 10 Jan 2023 01:03:29 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:c527615e4ffa2d5b9b777fd469b3b5ba7c1b1e9201c065be2c43569de48a3754`  
		Last Modified: Mon, 09 Jan 2023 17:07:17 GMT  
		Size: 2.9 MB (2865208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c30dc917313d61894ccb7cfad12c5f3a278e251ca506df448c9f8e2a16ba910`  
		Last Modified: Tue, 10 Jan 2023 01:04:01 GMT  
		Size: 1.2 KB (1241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b4704616a59a25f4e6a3979312202c02302fb7db16765696efeaf0136d5d871`  
		Last Modified: Tue, 10 Jan 2023 01:04:01 GMT  
		Size: 1.2 MB (1166534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d943eecb9e0495c260d5786a0e7109c2f3f4c07c93eed00e71667a8fd3cd0a7`  
		Last Modified: Tue, 10 Jan 2023 01:04:01 GMT  
		Size: 200.1 KB (200087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30309affe27d04051a0e8f9d361029624d0957f51f95f351a76921b3d10aa00e`  
		Last Modified: Tue, 10 Jan 2023 01:04:01 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40cb5d940651ed07d3a8a9b5d7bb45557f66f56eb842f0db2c34496a0b49b3be`  
		Last Modified: Tue, 10 Jan 2023 01:04:01 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.2-alpine` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:0213ccc252b274961ca65d4810e3e3adbfd0a45802938a1fc17b5260a5766747
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.8 MB (4838993 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5f334562e83a3560fd096b7555b628adde3f65f35e7d7f88d92cef036aa3b80e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Mon, 09 Jan 2023 17:04:48 GMT
ADD file:3080f19f39259a4b77cc53975de0184c78d4335ceb9ffb77a2838d0539ad6f85 in / 
# Mon, 09 Jan 2023 17:04:49 GMT
CMD ["/bin/sh"]
# Mon, 09 Jan 2023 21:54:38 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Mon, 09 Jan 2023 21:54:40 GMT
RUN apk add --no-cache libssl1.1
# Mon, 09 Jan 2023 21:54:40 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Mon, 09 Jan 2023 21:54:48 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Mon, 09 Jan 2023 21:54:48 GMT
VOLUME [/spiped]
# Mon, 09 Jan 2023 21:54:48 GMT
WORKDIR /spiped
# Mon, 09 Jan 2023 21:54:48 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 09 Jan 2023 21:54:48 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 09 Jan 2023 21:54:48 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:a9eaa45ef418e883481a13c7d84fa9904f2ec56789c52a87ba5a9e6483f2b74f`  
		Last Modified: Mon, 09 Jan 2023 17:05:12 GMT  
		Size: 3.3 MB (3259241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8a57c503886d17fc3a18ad5ac652d01a19c1d114d10d95fbbb6962eb5141a3c`  
		Last Modified: Mon, 09 Jan 2023 21:55:05 GMT  
		Size: 1.3 KB (1266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7deb227b2dbf5691407192d6e6164c40a313d06c2d63a713bcec3bfb588a82f1`  
		Last Modified: Mon, 09 Jan 2023 21:55:05 GMT  
		Size: 1.4 MB (1362327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:136d1ea11d30612c79aa77675c78fb75feede08c3a75327ad85af71c6acc55cc`  
		Last Modified: Mon, 09 Jan 2023 21:55:05 GMT  
		Size: 215.7 KB (215692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12c3012f3cfaea50c1e653e77ff8a01ac59681255c473f52fc3d3087f2ec06f1`  
		Last Modified: Mon, 09 Jan 2023 21:55:05 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78ff7343264af5878ae4a177e19ca1bc3ef5ed246ba09fa1c3c6e4e80c2c09b2`  
		Last Modified: Mon, 09 Jan 2023 21:55:05 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.2-alpine` - linux; 386

```console
$ docker pull spiped@sha256:d8a38312632b028320e1705047e9f772afc0badca532e45181c287df1ef83910
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.1 MB (5125102 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8462fd88246d8334a88562d226243c2b45ed34c1f68d1e222efac09016792383`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Mon, 09 Jan 2023 17:05:00 GMT
ADD file:d03619a0ef81726c34189e849b80cc92da908eb36e116f28275d5765e6d0919a in / 
# Mon, 09 Jan 2023 17:05:00 GMT
CMD ["/bin/sh"]
# Mon, 09 Jan 2023 19:07:22 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Mon, 09 Jan 2023 19:07:24 GMT
RUN apk add --no-cache libssl1.1
# Mon, 09 Jan 2023 19:07:25 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Mon, 09 Jan 2023 19:07:36 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Mon, 09 Jan 2023 19:07:37 GMT
VOLUME [/spiped]
# Mon, 09 Jan 2023 19:07:38 GMT
WORKDIR /spiped
# Mon, 09 Jan 2023 19:07:40 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 09 Jan 2023 19:07:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 09 Jan 2023 19:07:41 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:40e5b0b2e2bde18974628cadecd8a2f190f45f06c32846c16885d69b2908bf68`  
		Last Modified: Mon, 09 Jan 2023 17:05:42 GMT  
		Size: 3.4 MB (3408318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:beb4d578ecfd8ec0e5b44d6f231ae75cd33c39c4d21f5b01b80e80019344904e`  
		Last Modified: Mon, 09 Jan 2023 19:08:10 GMT  
		Size: 1.2 KB (1240 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d5141406d2cea5667b65a83cfc84fe7c8eef2aa49d6c549ec8acb7e97c32f89`  
		Last Modified: Mon, 09 Jan 2023 19:08:10 GMT  
		Size: 1.5 MB (1483729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ac653492946b43047544c01ac378096ae6c6d8856996b5de736547a2fafaf68`  
		Last Modified: Mon, 09 Jan 2023 19:08:10 GMT  
		Size: 231.4 KB (231382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95e2203d634caaf6243a81ca591d7aa9c925d62488c2290d0d6c57a46eeac8f8`  
		Last Modified: Mon, 09 Jan 2023 19:08:10 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb7ad0075ba728f545bdda81f2b8cc4d645b41f8ab2dac39cebca27927c444b2`  
		Last Modified: Mon, 09 Jan 2023 19:08:10 GMT  
		Size: 338.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.2-alpine` - linux; ppc64le

```console
$ docker pull spiped@sha256:6287dba41a56cf9c39be27c62b7a3bde3479b303d63e9230b446113020881fa9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.0 MB (5017699 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2ef59306a962c0b86d594be1281ca3dd3e91c0b16a046ee09218d60231e3a9cb`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Mon, 09 Jan 2023 17:05:13 GMT
ADD file:9a1d27fdc0c915f387f2446c85193d5215b18020b313114f0bf2799efcc1baae in / 
# Mon, 09 Jan 2023 17:05:13 GMT
CMD ["/bin/sh"]
# Mon, 09 Jan 2023 21:32:14 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Mon, 09 Jan 2023 21:32:16 GMT
RUN apk add --no-cache libssl1.1
# Mon, 09 Jan 2023 21:32:16 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Mon, 09 Jan 2023 21:32:30 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Mon, 09 Jan 2023 21:32:31 GMT
VOLUME [/spiped]
# Mon, 09 Jan 2023 21:32:31 GMT
WORKDIR /spiped
# Mon, 09 Jan 2023 21:32:32 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 09 Jan 2023 21:32:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 09 Jan 2023 21:32:32 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:f45bfda3aa14e255d9eb4c9a108eb3d8c6721946b4aa2e5808e5092242344a1c`  
		Last Modified: Mon, 09 Jan 2023 17:05:56 GMT  
		Size: 3.4 MB (3384562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd46f789ced0eaea980007a2e6a0f6b02b7711749489fdc0a30de08d248c3325`  
		Last Modified: Mon, 09 Jan 2023 21:33:00 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cc9ef36d078710c0c6d69a2d1c19bc6701be12e5c554ec9fa1546fe495e59eb`  
		Last Modified: Mon, 09 Jan 2023 21:32:59 GMT  
		Size: 1.4 MB (1411372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9e8744b0f13a67b1002a7a426a2b3635f0b4a28fd095ef061c0f1fd5d85d909`  
		Last Modified: Mon, 09 Jan 2023 21:32:59 GMT  
		Size: 220.0 KB (220028 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cc209dab70185705e5eee1e1710197c9bc735498e476d6719c4b850ae44fdaa`  
		Last Modified: Mon, 09 Jan 2023 21:32:59 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe41dcc405bef6ddd7bb480eadf45d92a9cfd583bee884d68eb41037c93e1e23`  
		Last Modified: Mon, 09 Jan 2023 21:32:59 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.2-alpine` - linux; s390x

```console
$ docker pull spiped@sha256:5a87be0c5f3e288adf33abd9c67087730cd729e12ac28ae4b107955683edff20
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.6 MB (4602294 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:63961a94a731d4f9e0005f5fd83043126c5546496fa856ea125a5c2e51c6979c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Mon, 09 Jan 2023 17:05:44 GMT
ADD file:eabe7c3c368e65478b53ac35c1daf3b703f2bca4ecdab2d080a65e8b981d7d4a in / 
# Mon, 09 Jan 2023 17:05:46 GMT
CMD ["/bin/sh"]
# Tue, 10 Jan 2023 01:32:49 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Tue, 10 Jan 2023 01:32:52 GMT
RUN apk add --no-cache libssl1.1
# Tue, 10 Jan 2023 01:32:52 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 10 Jan 2023 01:33:01 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Tue, 10 Jan 2023 01:33:02 GMT
VOLUME [/spiped]
# Tue, 10 Jan 2023 01:33:03 GMT
WORKDIR /spiped
# Tue, 10 Jan 2023 01:33:03 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 10 Jan 2023 01:33:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 10 Jan 2023 01:33:05 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:ae982806674c51a962c0fdd6e19f464ebd673df529c5cfb7c1d049e0b618d384`  
		Last Modified: Mon, 09 Jan 2023 17:06:50 GMT  
		Size: 3.2 MB (3170744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f659d5259c21b4ce33d18c83c0251b9d66d58281847f63904bed75a5683b3fde`  
		Last Modified: Tue, 10 Jan 2023 01:33:39 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9decaf35186276ee535aac72c69938baded768609a2bb148ca4d5c0a1788a984`  
		Last Modified: Tue, 10 Jan 2023 01:33:39 GMT  
		Size: 1.2 MB (1221175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93194a8cc16c2fcd24da284630284cd3fbf877fc323c8dc65e3d256d777ac04a`  
		Last Modified: Tue, 10 Jan 2023 01:33:39 GMT  
		Size: 208.6 KB (208637 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02decf839b354e56295448b1f40e50f813a1879598a091e766908a8f70b21671`  
		Last Modified: Tue, 10 Jan 2023 01:33:39 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07f2035a6bfb730bee20ac317d153b1061a4002ce6a450bb74f34bebcfa04369`  
		Last Modified: Tue, 10 Jan 2023 01:33:39 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:alpine`

```console
$ docker pull spiped@sha256:e8982ce4c33ed5c5fdf992ccf6c890b82d7806e41d8778ea6777610d0e4e4719
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
$ docker pull spiped@sha256:8eb40fb8e554b827563f599dd3e61da57293486cae87cd856a891b4e8dba353e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.1 MB (5075384 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2dda802d4535ce910f8e00126e80c79abb0825f3bf7caf66a4bb950cb589cc74`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Mon, 09 Jan 2023 17:05:20 GMT
ADD file:e4d600fc4c9c293efe360be7b30ee96579925d1b4634c94332e2ec73f7d8eca1 in / 
# Mon, 09 Jan 2023 17:05:20 GMT
CMD ["/bin/sh"]
# Mon, 09 Jan 2023 20:03:04 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Mon, 09 Jan 2023 20:03:05 GMT
RUN apk add --no-cache libssl1.1
# Mon, 09 Jan 2023 20:03:05 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Mon, 09 Jan 2023 20:03:16 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Mon, 09 Jan 2023 20:03:16 GMT
VOLUME [/spiped]
# Mon, 09 Jan 2023 20:03:16 GMT
WORKDIR /spiped
# Mon, 09 Jan 2023 20:03:16 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 09 Jan 2023 20:03:16 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 09 Jan 2023 20:03:16 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:8921db27df2831fa6eaa85321205a2470c669b855f3ec95d5a3c2b46de0442c9`  
		Last Modified: Mon, 09 Jan 2023 17:05:45 GMT  
		Size: 3.4 MB (3370628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e9fb896348696d642ef5674956097b03540bea28f8454d6287f5d9cb10b5b19`  
		Last Modified: Mon, 09 Jan 2023 20:03:32 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f1fb67340ae0e377cfa3a1ee1218a1ba6d31cf9f7cb2a302542d4354c848991`  
		Last Modified: Mon, 09 Jan 2023 20:03:33 GMT  
		Size: 1.5 MB (1481738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e228854dc2c8d78fdfe84ed1b99903b8567e21eff2fcf86757e6fdfa823872a`  
		Last Modified: Mon, 09 Jan 2023 20:03:32 GMT  
		Size: 221.3 KB (221283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f486af83d26d338661f9edfe85a3574704c4d8e4a08cdea692294588749dde0`  
		Last Modified: Mon, 09 Jan 2023 20:03:32 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35820a44b4998d9547534e80870c2e2a59cad7f381a4d6a82609d3f67126045d`  
		Last Modified: Mon, 09 Jan 2023 20:03:32 GMT  
		Size: 338.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; arm variant v6

```console
$ docker pull spiped@sha256:cb751a21eae14bec751c4cd688311f6eafc98d6d1769aa245711e63d7182e21a
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.6 MB (4554176 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:341ba40bb3f41e998727f9c4967f67b001703e78dafe41ad92a70bf2791fca9b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Mon, 09 Jan 2023 17:04:54 GMT
ADD file:b15fd8e9f996815394e25f20c8459bfb4c2a8c4074592d6f4c75f4fe79ce537e in / 
# Mon, 09 Jan 2023 17:04:55 GMT
CMD ["/bin/sh"]
# Mon, 09 Jan 2023 20:52:14 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Mon, 09 Jan 2023 20:52:16 GMT
RUN apk add --no-cache libssl1.1
# Mon, 09 Jan 2023 20:52:16 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Mon, 09 Jan 2023 20:52:25 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Mon, 09 Jan 2023 20:52:25 GMT
VOLUME [/spiped]
# Mon, 09 Jan 2023 20:52:25 GMT
WORKDIR /spiped
# Mon, 09 Jan 2023 20:52:25 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 09 Jan 2023 20:52:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 09 Jan 2023 20:52:25 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:0269c10e600f3a375f36ddabdbd264ce9503a455f0d0969ce8a00f24eaecc032`  
		Last Modified: Mon, 09 Jan 2023 17:05:45 GMT  
		Size: 3.1 MB (3107243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9fcf4fe7db4264a8e664de4d52478f1d4ba98146c38a7672ed85c122a2ec9ea`  
		Last Modified: Mon, 09 Jan 2023 20:52:44 GMT  
		Size: 1.2 KB (1242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:252aa0c5aa375a984c376376752105d7908cccb2ad2078305d2f12c857e58688`  
		Last Modified: Mon, 09 Jan 2023 20:52:45 GMT  
		Size: 1.2 MB (1238925 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90bcc6c04b36698f2894107a3dcd168ebf74dcadfaada1feb7c909e6d7d2e48c`  
		Last Modified: Mon, 09 Jan 2023 20:52:45 GMT  
		Size: 206.3 KB (206330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac2b1d7fdda8e63c8009adec27201adf5aef01cb0be8ae5e126525f70f6ff253`  
		Last Modified: Mon, 09 Jan 2023 20:52:44 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3cc764eff90255e712b5e4a850166371f439ffce5e23ec5a3902aeca546fce4`  
		Last Modified: Mon, 09 Jan 2023 20:52:44 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; arm variant v7

```console
$ docker pull spiped@sha256:5350876a3890b8b4c1a7262c4c48345b4046feb2b93df0f849b165f6d3862d43
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4233507 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5a136cbdcf03b9c140acc83ef95bd48dcdb73507ee82d16eed4339281865ff3e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Mon, 09 Jan 2023 17:06:27 GMT
ADD file:4696f25d0f019b27457c55b3b128b70bf153f38e3e4eb5bdfc21058543313e94 in / 
# Mon, 09 Jan 2023 17:06:27 GMT
CMD ["/bin/sh"]
# Tue, 10 Jan 2023 01:03:19 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Tue, 10 Jan 2023 01:03:20 GMT
RUN apk add --no-cache libssl1.1
# Tue, 10 Jan 2023 01:03:21 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 10 Jan 2023 01:03:29 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Tue, 10 Jan 2023 01:03:29 GMT
VOLUME [/spiped]
# Tue, 10 Jan 2023 01:03:29 GMT
WORKDIR /spiped
# Tue, 10 Jan 2023 01:03:29 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 10 Jan 2023 01:03:29 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 10 Jan 2023 01:03:29 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:c527615e4ffa2d5b9b777fd469b3b5ba7c1b1e9201c065be2c43569de48a3754`  
		Last Modified: Mon, 09 Jan 2023 17:07:17 GMT  
		Size: 2.9 MB (2865208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c30dc917313d61894ccb7cfad12c5f3a278e251ca506df448c9f8e2a16ba910`  
		Last Modified: Tue, 10 Jan 2023 01:04:01 GMT  
		Size: 1.2 KB (1241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b4704616a59a25f4e6a3979312202c02302fb7db16765696efeaf0136d5d871`  
		Last Modified: Tue, 10 Jan 2023 01:04:01 GMT  
		Size: 1.2 MB (1166534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d943eecb9e0495c260d5786a0e7109c2f3f4c07c93eed00e71667a8fd3cd0a7`  
		Last Modified: Tue, 10 Jan 2023 01:04:01 GMT  
		Size: 200.1 KB (200087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30309affe27d04051a0e8f9d361029624d0957f51f95f351a76921b3d10aa00e`  
		Last Modified: Tue, 10 Jan 2023 01:04:01 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40cb5d940651ed07d3a8a9b5d7bb45557f66f56eb842f0db2c34496a0b49b3be`  
		Last Modified: Tue, 10 Jan 2023 01:04:01 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:0213ccc252b274961ca65d4810e3e3adbfd0a45802938a1fc17b5260a5766747
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.8 MB (4838993 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5f334562e83a3560fd096b7555b628adde3f65f35e7d7f88d92cef036aa3b80e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Mon, 09 Jan 2023 17:04:48 GMT
ADD file:3080f19f39259a4b77cc53975de0184c78d4335ceb9ffb77a2838d0539ad6f85 in / 
# Mon, 09 Jan 2023 17:04:49 GMT
CMD ["/bin/sh"]
# Mon, 09 Jan 2023 21:54:38 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Mon, 09 Jan 2023 21:54:40 GMT
RUN apk add --no-cache libssl1.1
# Mon, 09 Jan 2023 21:54:40 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Mon, 09 Jan 2023 21:54:48 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Mon, 09 Jan 2023 21:54:48 GMT
VOLUME [/spiped]
# Mon, 09 Jan 2023 21:54:48 GMT
WORKDIR /spiped
# Mon, 09 Jan 2023 21:54:48 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 09 Jan 2023 21:54:48 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 09 Jan 2023 21:54:48 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:a9eaa45ef418e883481a13c7d84fa9904f2ec56789c52a87ba5a9e6483f2b74f`  
		Last Modified: Mon, 09 Jan 2023 17:05:12 GMT  
		Size: 3.3 MB (3259241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8a57c503886d17fc3a18ad5ac652d01a19c1d114d10d95fbbb6962eb5141a3c`  
		Last Modified: Mon, 09 Jan 2023 21:55:05 GMT  
		Size: 1.3 KB (1266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7deb227b2dbf5691407192d6e6164c40a313d06c2d63a713bcec3bfb588a82f1`  
		Last Modified: Mon, 09 Jan 2023 21:55:05 GMT  
		Size: 1.4 MB (1362327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:136d1ea11d30612c79aa77675c78fb75feede08c3a75327ad85af71c6acc55cc`  
		Last Modified: Mon, 09 Jan 2023 21:55:05 GMT  
		Size: 215.7 KB (215692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12c3012f3cfaea50c1e653e77ff8a01ac59681255c473f52fc3d3087f2ec06f1`  
		Last Modified: Mon, 09 Jan 2023 21:55:05 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78ff7343264af5878ae4a177e19ca1bc3ef5ed246ba09fa1c3c6e4e80c2c09b2`  
		Last Modified: Mon, 09 Jan 2023 21:55:05 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; 386

```console
$ docker pull spiped@sha256:d8a38312632b028320e1705047e9f772afc0badca532e45181c287df1ef83910
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.1 MB (5125102 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8462fd88246d8334a88562d226243c2b45ed34c1f68d1e222efac09016792383`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Mon, 09 Jan 2023 17:05:00 GMT
ADD file:d03619a0ef81726c34189e849b80cc92da908eb36e116f28275d5765e6d0919a in / 
# Mon, 09 Jan 2023 17:05:00 GMT
CMD ["/bin/sh"]
# Mon, 09 Jan 2023 19:07:22 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Mon, 09 Jan 2023 19:07:24 GMT
RUN apk add --no-cache libssl1.1
# Mon, 09 Jan 2023 19:07:25 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Mon, 09 Jan 2023 19:07:36 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Mon, 09 Jan 2023 19:07:37 GMT
VOLUME [/spiped]
# Mon, 09 Jan 2023 19:07:38 GMT
WORKDIR /spiped
# Mon, 09 Jan 2023 19:07:40 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 09 Jan 2023 19:07:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 09 Jan 2023 19:07:41 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:40e5b0b2e2bde18974628cadecd8a2f190f45f06c32846c16885d69b2908bf68`  
		Last Modified: Mon, 09 Jan 2023 17:05:42 GMT  
		Size: 3.4 MB (3408318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:beb4d578ecfd8ec0e5b44d6f231ae75cd33c39c4d21f5b01b80e80019344904e`  
		Last Modified: Mon, 09 Jan 2023 19:08:10 GMT  
		Size: 1.2 KB (1240 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d5141406d2cea5667b65a83cfc84fe7c8eef2aa49d6c549ec8acb7e97c32f89`  
		Last Modified: Mon, 09 Jan 2023 19:08:10 GMT  
		Size: 1.5 MB (1483729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ac653492946b43047544c01ac378096ae6c6d8856996b5de736547a2fafaf68`  
		Last Modified: Mon, 09 Jan 2023 19:08:10 GMT  
		Size: 231.4 KB (231382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95e2203d634caaf6243a81ca591d7aa9c925d62488c2290d0d6c57a46eeac8f8`  
		Last Modified: Mon, 09 Jan 2023 19:08:10 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb7ad0075ba728f545bdda81f2b8cc4d645b41f8ab2dac39cebca27927c444b2`  
		Last Modified: Mon, 09 Jan 2023 19:08:10 GMT  
		Size: 338.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; ppc64le

```console
$ docker pull spiped@sha256:6287dba41a56cf9c39be27c62b7a3bde3479b303d63e9230b446113020881fa9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.0 MB (5017699 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2ef59306a962c0b86d594be1281ca3dd3e91c0b16a046ee09218d60231e3a9cb`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Mon, 09 Jan 2023 17:05:13 GMT
ADD file:9a1d27fdc0c915f387f2446c85193d5215b18020b313114f0bf2799efcc1baae in / 
# Mon, 09 Jan 2023 17:05:13 GMT
CMD ["/bin/sh"]
# Mon, 09 Jan 2023 21:32:14 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Mon, 09 Jan 2023 21:32:16 GMT
RUN apk add --no-cache libssl1.1
# Mon, 09 Jan 2023 21:32:16 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Mon, 09 Jan 2023 21:32:30 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Mon, 09 Jan 2023 21:32:31 GMT
VOLUME [/spiped]
# Mon, 09 Jan 2023 21:32:31 GMT
WORKDIR /spiped
# Mon, 09 Jan 2023 21:32:32 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Mon, 09 Jan 2023 21:32:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 09 Jan 2023 21:32:32 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:f45bfda3aa14e255d9eb4c9a108eb3d8c6721946b4aa2e5808e5092242344a1c`  
		Last Modified: Mon, 09 Jan 2023 17:05:56 GMT  
		Size: 3.4 MB (3384562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd46f789ced0eaea980007a2e6a0f6b02b7711749489fdc0a30de08d248c3325`  
		Last Modified: Mon, 09 Jan 2023 21:33:00 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cc9ef36d078710c0c6d69a2d1c19bc6701be12e5c554ec9fa1546fe495e59eb`  
		Last Modified: Mon, 09 Jan 2023 21:32:59 GMT  
		Size: 1.4 MB (1411372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9e8744b0f13a67b1002a7a426a2b3635f0b4a28fd095ef061c0f1fd5d85d909`  
		Last Modified: Mon, 09 Jan 2023 21:32:59 GMT  
		Size: 220.0 KB (220028 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cc209dab70185705e5eee1e1710197c9bc735498e476d6719c4b850ae44fdaa`  
		Last Modified: Mon, 09 Jan 2023 21:32:59 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe41dcc405bef6ddd7bb480eadf45d92a9cfd583bee884d68eb41037c93e1e23`  
		Last Modified: Mon, 09 Jan 2023 21:32:59 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; s390x

```console
$ docker pull spiped@sha256:5a87be0c5f3e288adf33abd9c67087730cd729e12ac28ae4b107955683edff20
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.6 MB (4602294 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:63961a94a731d4f9e0005f5fd83043126c5546496fa856ea125a5c2e51c6979c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Mon, 09 Jan 2023 17:05:44 GMT
ADD file:eabe7c3c368e65478b53ac35c1daf3b703f2bca4ecdab2d080a65e8b981d7d4a in / 
# Mon, 09 Jan 2023 17:05:46 GMT
CMD ["/bin/sh"]
# Tue, 10 Jan 2023 01:32:49 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Tue, 10 Jan 2023 01:32:52 GMT
RUN apk add --no-cache libssl1.1
# Tue, 10 Jan 2023 01:32:52 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 10 Jan 2023 01:33:01 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Tue, 10 Jan 2023 01:33:02 GMT
VOLUME [/spiped]
# Tue, 10 Jan 2023 01:33:03 GMT
WORKDIR /spiped
# Tue, 10 Jan 2023 01:33:03 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 10 Jan 2023 01:33:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 10 Jan 2023 01:33:05 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:ae982806674c51a962c0fdd6e19f464ebd673df529c5cfb7c1d049e0b618d384`  
		Last Modified: Mon, 09 Jan 2023 17:06:50 GMT  
		Size: 3.2 MB (3170744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f659d5259c21b4ce33d18c83c0251b9d66d58281847f63904bed75a5683b3fde`  
		Last Modified: Tue, 10 Jan 2023 01:33:39 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9decaf35186276ee535aac72c69938baded768609a2bb148ca4d5c0a1788a984`  
		Last Modified: Tue, 10 Jan 2023 01:33:39 GMT  
		Size: 1.2 MB (1221175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93194a8cc16c2fcd24da284630284cd3fbf877fc323c8dc65e3d256d777ac04a`  
		Last Modified: Tue, 10 Jan 2023 01:33:39 GMT  
		Size: 208.6 KB (208637 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02decf839b354e56295448b1f40e50f813a1879598a091e766908a8f70b21671`  
		Last Modified: Tue, 10 Jan 2023 01:33:39 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07f2035a6bfb730bee20ac317d153b1061a4002ce6a450bb74f34bebcfa04369`  
		Last Modified: Tue, 10 Jan 2023 01:33:39 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:latest`

```console
$ docker pull spiped@sha256:36792922d2b08e1d321e2dbc07eca0f7ee6b7477a145b88bc02a54c493712763
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
$ docker pull spiped@sha256:4a8875107a0ae5b2a99a15a14d48ebeb0053b2d6fc7f9539eb0d2a223121d98e
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.9 MB (33947843 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d002918607a70e5bef0dd6d3afe1b10e682eb276fd30be897c5102a77a6dfe82`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 09 Feb 2023 02:00:32 GMT
ADD file:fcf4deede0eb98d96d8657dfb1b0918a2c3d35f16d4858dd9e75c843edeff166 in / 
# Thu, 09 Feb 2023 02:00:33 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 07:42:30 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Thu, 09 Feb 2023 07:42:35 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 07:42:35 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 09 Feb 2023 07:42:56 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 09 Feb 2023 07:42:56 GMT
VOLUME [/spiped]
# Thu, 09 Feb 2023 07:42:56 GMT
WORKDIR /spiped
# Thu, 09 Feb 2023 07:42:56 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 09 Feb 2023 07:42:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 09 Feb 2023 07:42:56 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:886a7482403a267f98b84e4a9f9ede516bac1fe7eb82ff570dabbb0b297d5b53`  
		Last Modified: Thu, 09 Feb 2023 02:05:42 GMT  
		Size: 28.9 MB (28916292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f0b4c916377c6dbb908da122fa96bfa0ce286cc9da628adef55639296163add`  
		Last Modified: Thu, 09 Feb 2023 07:43:14 GMT  
		Size: 1.7 KB (1730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:067ecc9df0a048cbcda29c8daee40da43959b1c7053eda96b2a81b869cecb54d`  
		Last Modified: Thu, 09 Feb 2023 07:43:15 GMT  
		Size: 1.0 KB (1023 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31a0779e11296c1c17feadfa2d00251940d442709616b2f2ad4761144806351b`  
		Last Modified: Thu, 09 Feb 2023 07:43:15 GMT  
		Size: 5.0 MB (5028362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fa3cff81fceb3cb7558134cae0d1dd81dd0687cc27dc747d8a38c557b289787`  
		Last Modified: Thu, 09 Feb 2023 07:43:14 GMT  
		Size: 92.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ec878da2996777c7363b616dfbe74e27b6506978d8674a1883c3cb4690921d3`  
		Last Modified: Thu, 09 Feb 2023 07:43:14 GMT  
		Size: 344.0 B  
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
$ docker pull spiped@sha256:c412ab17dbe7c382e310a9a62f8cfb32bc706a2a9f03ba267b24ee44bb6830fd
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.8 MB (34838196 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:009dd6f9dd0b116d48899f5168c6848918483e4be4b6f7797ccf9c37d1c65f40`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 09 Feb 2023 02:41:45 GMT
ADD file:dc3c16b50baeac5b9644e607c8df9606e9583f8598e3ba34bcdd69c669a5904c in / 
# Thu, 09 Feb 2023 02:41:46 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 04:29:04 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Thu, 09 Feb 2023 04:29:06 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 04:29:06 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 09 Feb 2023 04:29:19 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 09 Feb 2023 04:29:19 GMT
VOLUME [/spiped]
# Thu, 09 Feb 2023 04:29:19 GMT
WORKDIR /spiped
# Thu, 09 Feb 2023 04:29:20 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 09 Feb 2023 04:29:20 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 09 Feb 2023 04:29:20 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:c2f78940fdfbfc5ce5d1d3cff3c27a319451aeb3ec12ff2473073516907fbce9`  
		Last Modified: Thu, 09 Feb 2023 02:46:06 GMT  
		Size: 29.6 MB (29647513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68bbc75b754860161ae6344fc9d8438ebb45bf74a809cf2eacc1eed1f69360f5`  
		Last Modified: Thu, 09 Feb 2023 04:29:50 GMT  
		Size: 1.7 KB (1740 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1ed99a2553aedd84386b5162ec3d7cbd85e263d67a7f880f0c22455ffc703ba`  
		Last Modified: Thu, 09 Feb 2023 04:29:50 GMT  
		Size: 1.1 KB (1051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db7bd105f0e3167c684db4a568d0891a9f72b7680fb5acc641f111250789be6d`  
		Last Modified: Thu, 09 Feb 2023 04:29:51 GMT  
		Size: 5.2 MB (5187421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9be9021fdd8bee9e348b198d87e955c3786ae17048cf4acbcd219b030ba7f369`  
		Last Modified: Thu, 09 Feb 2023 04:29:50 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91bc0b6a48c2e0be6fe8929b92f3fb8b514edc9ba7564792af2d1553b598a035`  
		Last Modified: Thu, 09 Feb 2023 04:29:50 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
