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
$ docker pull spiped@sha256:3803fdc1e42df38ec09699a69d983e0c24277804803d456099a8989cefe72ace
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
$ docker pull spiped@sha256:721c9e3ecb57ab885c003700665c787207861ed892989be757c330a07a4c697c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.4 MB (37412915 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:be5ba0f72c5d2a07deab8c81f022c0d0da6de183e5be45bf75e5d2a765ce1241`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 23 Mar 2023 01:30:27 GMT
ADD file:60911afdacfdc216e44115addb5f3cc07f4166e8a4adf7be94a58aacc327ad63 in / 
# Thu, 23 Mar 2023 01:30:27 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 14:21:59 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Thu, 23 Mar 2023 14:22:02 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 14:22:03 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 23 Mar 2023 14:22:22 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 23 Mar 2023 14:22:22 GMT
VOLUME [/spiped]
# Thu, 23 Mar 2023 14:22:22 GMT
WORKDIR /spiped
# Thu, 23 Mar 2023 14:22:22 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 23 Mar 2023 14:22:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Mar 2023 14:22:22 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:f1f26f5702560b7e591bef5c4d840f76a232bf13fd5aefc4e22077a1ae4440c7`  
		Last Modified: Thu, 23 Mar 2023 01:34:23 GMT  
		Size: 31.4 MB (31411405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eba658cb120bd99022c7cf87e1a7e097de79f5861fc1b445ecbae4edeec1dfe4`  
		Last Modified: Thu, 23 Mar 2023 14:22:35 GMT  
		Size: 1.7 KB (1734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa69edd47542d8a3cf149d1bb36059f8c0e848ad433b8c659de5c1155781e12e`  
		Last Modified: Thu, 23 Mar 2023 14:22:35 GMT  
		Size: 1.1 KB (1050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:187bd75bf46234bc1609024e05712a659839202cc73b40db694672a1aff8b2c6`  
		Last Modified: Thu, 23 Mar 2023 14:22:36 GMT  
		Size: 6.0 MB (5998257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b9f50c988f7a169cc12e6566f824e86960bc77d0e2714a2ff2ddb919bec84f4`  
		Last Modified: Thu, 23 Mar 2023 14:22:35 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:866a419d38e59257252937a0d01999799ffb71213ebab6f7c0ba412832f7fbbe`  
		Last Modified: Thu, 23 Mar 2023 14:22:35 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; arm variant v5

```console
$ docker pull spiped@sha256:c56ad02f7a635dc4d379610e1a1095f9c487573ef61de595cba27525df82e0f0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.0 MB (33951316 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3289615005289139cb049ad1aaeaa83f924744ae842e267446c978996e7f8843`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 12 Apr 2023 00:48:41 GMT
ADD file:11004b5308adcb1c41526eac7071d373a5c42ca2e457a2e9e8b3a9d621c4e8e1 in / 
# Wed, 12 Apr 2023 00:48:41 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 04:13:45 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 12 Apr 2023 04:13:49 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 04:13:49 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 12 Apr 2023 04:14:09 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 12 Apr 2023 04:14:10 GMT
VOLUME [/spiped]
# Wed, 12 Apr 2023 04:14:10 GMT
WORKDIR /spiped
# Wed, 12 Apr 2023 04:14:10 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 12 Apr 2023 04:14:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 12 Apr 2023 04:14:10 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:5303309ebdb5d711447ed8a4ea072653ca7445c193060ec0aea30a89e92cda7e`  
		Last Modified: Wed, 12 Apr 2023 00:51:08 GMT  
		Size: 28.9 MB (28919551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c6d1cdee0b3069d6a9bbf71705b647047aa3718658646508ea3895abc295acd`  
		Last Modified: Wed, 12 Apr 2023 04:14:22 GMT  
		Size: 1.7 KB (1726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:413f2bdfff2530854dc8be54292587aacb28c20e08fbec5a75cd1c650b3ca0c6`  
		Last Modified: Wed, 12 Apr 2023 04:14:22 GMT  
		Size: 1.1 KB (1051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a772c2e19b2b59b3653449c3d87f10b14cad2ada0f4da89454a5d4216fb591c`  
		Last Modified: Wed, 12 Apr 2023 04:14:23 GMT  
		Size: 5.0 MB (5028515 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c462f1e36902eb29b25d02f2e17f167c04a3e4f838a3a5ab2227124fded03fb`  
		Last Modified: Wed, 12 Apr 2023 04:14:22 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edfdf45255e0c1a8dcac1dd2d2e36c424b51561ba09b234321f4589bcdab730d`  
		Last Modified: Wed, 12 Apr 2023 04:14:22 GMT  
		Size: 344.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; arm variant v7

```console
$ docker pull spiped@sha256:cf39f3bb40dcde6b5bf8478c9adb7d2539f890a17b9c12197f7ae968a28420f6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.3 MB (31329618 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1767501b8e0bc0f4d13978feac2b18de6af1c59fc29879fb0d1c08f1f85fcf84`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 23 Mar 2023 01:16:59 GMT
ADD file:1c83b99ee21091150a1c9ee8ef7c40bec3d6cb0d64b8bc0ef40fb97e6233aa5b in / 
# Thu, 23 Mar 2023 01:17:00 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 12:26:37 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Thu, 23 Mar 2023 12:26:40 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 12:26:40 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 23 Mar 2023 12:26:56 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 23 Mar 2023 12:26:56 GMT
VOLUME [/spiped]
# Thu, 23 Mar 2023 12:26:56 GMT
WORKDIR /spiped
# Thu, 23 Mar 2023 12:26:56 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 23 Mar 2023 12:26:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Mar 2023 12:26:56 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:2bc24e24d213c286ca4011c8b5cb7a3cf2a51f3bbedee8eeced46382bb5507bc`  
		Last Modified: Thu, 23 Mar 2023 01:33:18 GMT  
		Size: 26.6 MB (26577330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19061e17258a1ab423b9751a507a87e3c84da5eaffe1923ad2abc7aa5bf00be5`  
		Last Modified: Thu, 23 Mar 2023 12:27:07 GMT  
		Size: 1.7 KB (1727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0722d57fbb2b9577a072039b5f829c50b186b9d21b626777d773449488488fdc`  
		Last Modified: Thu, 23 Mar 2023 12:27:07 GMT  
		Size: 1.1 KB (1052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45c6b3401d253fee03596d2a401a84ebd8e4a340950690b66204e12a04889674`  
		Last Modified: Thu, 23 Mar 2023 12:27:08 GMT  
		Size: 4.7 MB (4749039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b000b28b92c3a6f78c372224d409ad90c989e6f0a43e4d9b72ae8ad4ccd28734`  
		Last Modified: Thu, 23 Mar 2023 12:27:07 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c563d03992865638f6480cdb6704eb9b8204b1c402024e2a101a161ede86290`  
		Last Modified: Thu, 23 Mar 2023 12:27:07 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:59a7ac95f3c86cfcda52266517687440ee833af0cfcd7bac7560d43faa690d52
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.3 MB (35339898 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:48134ae14be7815e330e696d68f5ce9f78018354a0b2aeef3cf707a462d57153`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 12 Apr 2023 00:39:49 GMT
ADD file:7b3c55926db26568f849247e80abdec3cfd6642929a40f0bbee95e4cb176051e in / 
# Wed, 12 Apr 2023 00:39:49 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 05:09:45 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 12 Apr 2023 05:09:48 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 05:09:48 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 12 Apr 2023 05:10:03 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 12 Apr 2023 05:10:03 GMT
VOLUME [/spiped]
# Wed, 12 Apr 2023 05:10:03 GMT
WORKDIR /spiped
# Wed, 12 Apr 2023 05:10:03 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 12 Apr 2023 05:10:03 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 12 Apr 2023 05:10:03 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:ebc3dc5a2d72427c585c8cda7574a75d96e04b9a37572bd3af0bff905abefbb9`  
		Last Modified: Wed, 12 Apr 2023 00:42:35 GMT  
		Size: 30.1 MB (30063826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3875f32a5967d63af0264c7e837f0ec1af397174340c608406c8dc1c4efd6d0`  
		Last Modified: Wed, 12 Apr 2023 05:10:15 GMT  
		Size: 1.7 KB (1734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d3c045802f338371900f62902ca0526fcbe0f103f1782134df45d785ec50a3b`  
		Last Modified: Wed, 12 Apr 2023 05:10:15 GMT  
		Size: 1.1 KB (1052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2cf02c8c59a3d5dfbb72551bda146e124e152fc03ddae5703249f6dfce3a7db`  
		Last Modified: Wed, 12 Apr 2023 05:10:16 GMT  
		Size: 5.3 MB (5272817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eafbdd4f6fdf5ed1c3903c9d26f47af77dcbde36fd86079557354b0153d0fd7b`  
		Last Modified: Wed, 12 Apr 2023 05:10:15 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9422d8f8fafc31168cc5eaebe935dfc7fde33c3e800595ec728d2d9fe52717fc`  
		Last Modified: Wed, 12 Apr 2023 05:10:16 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; 386

```console
$ docker pull spiped@sha256:74d7f5c8f3f3d9c67ac2694a397c85180e9414b6092e41e394b39054f2029c92
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.3 MB (40291472 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cd42d521cfced48016618daf00f5e6976442656bf9c4005a7c8200ef734bcbd4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 23 Mar 2023 00:39:18 GMT
ADD file:315d843eefd4a8bb2345366dcd6bab00a06fca4a7970e220ae8946123d07d7ed in / 
# Thu, 23 Mar 2023 00:39:19 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 12:10:30 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Thu, 23 Mar 2023 12:10:33 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 12:10:33 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 23 Mar 2023 12:10:56 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 23 Mar 2023 12:10:56 GMT
VOLUME [/spiped]
# Thu, 23 Mar 2023 12:10:56 GMT
WORKDIR /spiped
# Thu, 23 Mar 2023 12:10:56 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 23 Mar 2023 12:10:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Mar 2023 12:10:57 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:3e638a975ea99fe8646002726dcb1ccdccc49ad33967b30337b9b2413e0619b5`  
		Last Modified: Thu, 23 Mar 2023 00:43:09 GMT  
		Size: 32.4 MB (32396277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8c70cbb4c8fd8326cfa3a38bcadaebdcf624fcd76381d57288eb687694073d1`  
		Last Modified: Thu, 23 Mar 2023 12:11:11 GMT  
		Size: 1.7 KB (1725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b85e36913d82a6dadb0781c7ab440ef652976cc8995f5f0a0bd0541b9b620373`  
		Last Modified: Thu, 23 Mar 2023 12:11:11 GMT  
		Size: 1.1 KB (1054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bec8a50af228e59f346840b516f8f52a3b22b0be6d31a71d1341b272cc16d2ad`  
		Last Modified: Thu, 23 Mar 2023 12:11:13 GMT  
		Size: 7.9 MB (7891948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af275a5a028f320d08a155a1238d5121d8a0198cebf123d479cfab9a01aafd10`  
		Last Modified: Thu, 23 Mar 2023 12:11:11 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:409fcb43c7b4c77abd48e9757bd49eadd9c1aade55294cd9145e4f451a2a7a75`  
		Last Modified: Thu, 23 Mar 2023 12:11:11 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; mips64le

```console
$ docker pull spiped@sha256:62230d57630eb194945dc5756f3ee3712d046b75a1dd34bf2492a6418d46c0c5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.3 MB (35342788 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8418f829109d61f98060ab82e69f86501a87342a4f87913c3caeeb250c189e00`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 23 Mar 2023 05:17:57 GMT
ADD file:fd3a8eec4ae8f6058f522536ca9af1b391f3032504c085d8ddb6f4878ca478d5 in / 
# Thu, 23 Mar 2023 05:18:02 GMT
CMD ["bash"]
# Fri, 24 Mar 2023 05:00:18 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Fri, 24 Mar 2023 05:00:32 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Fri, 24 Mar 2023 05:00:34 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Fri, 24 Mar 2023 05:02:12 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Fri, 24 Mar 2023 05:02:15 GMT
VOLUME [/spiped]
# Fri, 24 Mar 2023 05:02:18 GMT
WORKDIR /spiped
# Fri, 24 Mar 2023 05:02:20 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 24 Mar 2023 05:02:23 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Mar 2023 05:02:25 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:735f9e60414e17ec59baef702f7013b7327899801df2ecf10123ce2727d8dea5`  
		Last Modified: Thu, 23 Mar 2023 05:25:53 GMT  
		Size: 29.6 MB (29634483 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9a95c8da754e637392a1172bcb5e591bcfcee63c2487be6f26b2c7489db5a7a`  
		Last Modified: Fri, 24 Mar 2023 05:02:46 GMT  
		Size: 1.6 KB (1622 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd933d8bf0d5ecf038fba2d2a35b694d9bf219c863351085755e909ab6c35b68`  
		Last Modified: Fri, 24 Mar 2023 05:02:46 GMT  
		Size: 926.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5db34c43bd622971b73a1d85c07581e353bf4e2ea607f6d6fcccd6a01f4fe2af`  
		Last Modified: Fri, 24 Mar 2023 05:02:51 GMT  
		Size: 5.7 MB (5705322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:476c1e9034825a9660cd4864a260cd15699063d1ed614ca97343aa9e139f1a36`  
		Last Modified: Fri, 24 Mar 2023 05:02:46 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ce2516d3dc94f7447fdff0b2538709c3ea3641cea323cd4d781e63909477f18`  
		Last Modified: Fri, 24 Mar 2023 05:02:46 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; ppc64le

```console
$ docker pull spiped@sha256:f401ab547830f955399b7c0c1037926954410f08e2308f97b2f1e114bf6c259b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.3 MB (41290962 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e8453ca71665e6fc2f4410696c68b7f0e85ba0d198b69afe7a94b47804fa1b94`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 23 Mar 2023 01:19:48 GMT
ADD file:fbd36b7667327dd30171fc49b8e028b8371fdbc7d30ee673808d508557f78bf1 in / 
# Thu, 23 Mar 2023 01:19:49 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 16:21:57 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Thu, 23 Mar 2023 16:22:03 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 16:22:03 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 23 Mar 2023 16:22:48 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 23 Mar 2023 16:22:49 GMT
VOLUME [/spiped]
# Thu, 23 Mar 2023 16:22:49 GMT
WORKDIR /spiped
# Thu, 23 Mar 2023 16:22:49 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 23 Mar 2023 16:22:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Mar 2023 16:22:50 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:8f472ad0a3fa58b4e304d1a974f25615d5bd3b7a99dff9c8202bd30facef0155`  
		Last Modified: Thu, 23 Mar 2023 01:24:22 GMT  
		Size: 35.3 MB (35288050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4167de1b2f5e0621dc4ea93047f68b495e3ff1d47ad708aeb47dacc4d98e4d6a`  
		Last Modified: Thu, 23 Mar 2023 16:23:05 GMT  
		Size: 1.7 KB (1732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:268241dc91792d1ad06458566222f09588696272408743915b59f8f440290b1c`  
		Last Modified: Thu, 23 Mar 2023 16:23:05 GMT  
		Size: 1.1 KB (1054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8dae255202559b344f349ed2396795c7dbc31726de4c1f57564193a10a4737e`  
		Last Modified: Thu, 23 Mar 2023 16:23:07 GMT  
		Size: 6.0 MB (5999654 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:047050eb0511c54c1aed11a944fdd94382d4abf66190b183f205e829e05e92b3`  
		Last Modified: Thu, 23 Mar 2023 16:23:05 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42ed775b429742a2b9aa4f680d2104804ccaac99aeccda29c0e231896875d5dc`  
		Last Modified: Thu, 23 Mar 2023 16:23:05 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; s390x

```console
$ docker pull spiped@sha256:bd0f6a8ba4b8c11fe888fee6860ea1d54be076bfe5957b43344b7b62dec0f47c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.8 MB (34844023 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:434b1ada99c83de5816075c26b07f7e49e021c25d4e40b80ddaf363ced468b65`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 12 Apr 2023 00:01:00 GMT
ADD file:b6463dba97ba9c0a29bacfafc4d67bc603ab57e80b75e23cd42d7ef4b0f8e6ae in / 
# Wed, 12 Apr 2023 00:01:04 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 07:13:35 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 12 Apr 2023 07:13:37 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 07:13:37 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 12 Apr 2023 07:13:53 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 12 Apr 2023 07:13:54 GMT
VOLUME [/spiped]
# Wed, 12 Apr 2023 07:13:54 GMT
WORKDIR /spiped
# Wed, 12 Apr 2023 07:13:54 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 12 Apr 2023 07:13:54 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 12 Apr 2023 07:13:54 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:97fe10bc7def58e7938e97e41eec4788ec7a45b6ef2cb1770cec02fa831fd19d`  
		Last Modified: Wed, 12 Apr 2023 00:05:18 GMT  
		Size: 29.7 MB (29653156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60661451feca33d0d1fc43f91b66dabebcd27f2ad19153400d0feafc64799c08`  
		Last Modified: Wed, 12 Apr 2023 07:14:13 GMT  
		Size: 1.7 KB (1736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28a1ae3818d2c3bcea0558356a7a736f1cc9b24645b2ad17f5a548b75d857b3b`  
		Last Modified: Wed, 12 Apr 2023 07:14:13 GMT  
		Size: 1.1 KB (1050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f4048da853c0e9dbdd6b2016bd4357a1c880ae93bc8c8567bbd675caccd414b`  
		Last Modified: Wed, 12 Apr 2023 07:14:14 GMT  
		Size: 5.2 MB (5187613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:302aa23f2c1ca3a68f99772fae7ea836cbcbc3330cca4b8604b18889c292b96d`  
		Last Modified: Wed, 12 Apr 2023 07:14:13 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74dc85c46ada57925ebdfcf7391a313ed62367842185b9add5f65f61a2945c2c`  
		Last Modified: Wed, 12 Apr 2023 07:14:13 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:1-alpine`

```console
$ docker pull spiped@sha256:657bd49b462533d254e7d5b3216fde01bc59a24c4f6277b050ae5bdc8f548a87
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
$ docker pull spiped@sha256:7b7f7844dc68c4b9728d9185d906025f7565df88ca9612aaaf420ac91523f405
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.1 MB (5080949 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2b60c5b50be16ba58852d923ea4e7d5224aecb355eb4588ab08b2f70c72ad851`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 29 Mar 2023 18:19:24 GMT
ADD file:9a4f77dfaba7fd2aa78186e4ef0e7486ad55101cefc1fabbc1b385601bb38920 in / 
# Wed, 29 Mar 2023 18:19:24 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 02:36:50 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 30 Mar 2023 02:36:51 GMT
RUN apk add --no-cache libssl1.1
# Thu, 30 Mar 2023 02:36:51 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 30 Mar 2023 02:37:01 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Thu, 30 Mar 2023 02:37:01 GMT
VOLUME [/spiped]
# Thu, 30 Mar 2023 02:37:02 GMT
WORKDIR /spiped
# Thu, 30 Mar 2023 02:37:02 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 30 Mar 2023 02:37:02 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 30 Mar 2023 02:37:02 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:f56be85fc22e46face30e2c3de3f7fe7c15f8fd7c4e5add29d7f64b87abdaa09`  
		Last Modified: Wed, 29 Mar 2023 18:19:57 GMT  
		Size: 3.4 MB (3374563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:833c4ea98211ab2b826b6d62f250a61b8c5ae407b5de38776cc5bc31d895d3fa`  
		Last Modified: Thu, 30 Mar 2023 02:37:13 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:870359eb3ab308a11eaf9cfc6782cd2bea0c513f3920492180bd5f5cbbea54eb`  
		Last Modified: Thu, 30 Mar 2023 02:37:13 GMT  
		Size: 1.5 MB (1483362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4afeb4ec06ad120774f5e7a75610323bda25b84d5957c8bac3f5c90ea7fdd17`  
		Last Modified: Thu, 30 Mar 2023 02:37:13 GMT  
		Size: 221.3 KB (221284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9641a8793752f42f60dcbb12e857125ba41995c02e48630112ef3f6d5747a28`  
		Last Modified: Thu, 30 Mar 2023 02:37:13 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb90b001556af3810279377523e96a71161f2dc727b628cb3d284764e5e847fd`  
		Last Modified: Thu, 30 Mar 2023 02:37:13 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; arm variant v6

```console
$ docker pull spiped@sha256:98e69abcdbbbc31f8223857ec6529b855f8e21be02602fe6763b73403a252650
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.6 MB (4560042 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c4871452a88018819e0282cc73c7c17274cbea4b4fd8f73619664078771460b6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 29 Mar 2023 18:01:09 GMT
ADD file:2dd294d20c0b500c8fed6b410b059429b36f51cd48a45eaf7a06ecbef9e2a3bb in / 
# Wed, 29 Mar 2023 18:01:09 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 00:22:48 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 30 Mar 2023 00:22:50 GMT
RUN apk add --no-cache libssl1.1
# Thu, 30 Mar 2023 00:22:50 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 30 Mar 2023 00:22:58 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Thu, 30 Mar 2023 00:22:58 GMT
VOLUME [/spiped]
# Thu, 30 Mar 2023 00:22:58 GMT
WORKDIR /spiped
# Thu, 30 Mar 2023 00:22:58 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 30 Mar 2023 00:22:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 30 Mar 2023 00:22:58 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:75257e753735e4ff78fae2d44018022a6ac775290e02103713a70699ece7576e`  
		Last Modified: Wed, 29 Mar 2023 18:01:52 GMT  
		Size: 3.1 MB (3110802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76f18e2ef9b0aa3ce161a88dbc21a7f6e04c161889cd2e9a48db6753f539a908`  
		Last Modified: Thu, 30 Mar 2023 00:24:29 GMT  
		Size: 1.3 KB (1267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f98080b1dde5f78f59c30b4e0ecd3d8755ce81a51335edb1f928872b6ea2758`  
		Last Modified: Thu, 30 Mar 2023 00:24:29 GMT  
		Size: 1.2 MB (1241151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2aaabfafc343e9926cb7046e859064ad3777e2fc8cddcb7e477dde08175094e7`  
		Last Modified: Thu, 30 Mar 2023 00:24:29 GMT  
		Size: 206.4 KB (206355 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e41f7588b8c91b544e8c7d054c90e59b7a9bd11c4e88918abb84a283000e0017`  
		Last Modified: Thu, 30 Mar 2023 00:24:29 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17cd529e07580d9750fa02477c2004129b10b554d974efb4047239df64df3a24`  
		Last Modified: Thu, 30 Mar 2023 00:24:29 GMT  
		Size: 338.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; arm variant v7

```console
$ docker pull spiped@sha256:6c2a2f1aeafd6139364938089caba1b87ad68bedb26cd1880228677d027a8a71
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4237992 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7a9eb306d4124eb8e1c6195849bb2b723860dae03a03f9bae43f0cb32e1462fd`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 29 Mar 2023 18:03:38 GMT
ADD file:959fa0ffb60c37c4fdc0d32ac31511f8dead32ef7f4bd848b11ff144a6b37012 in / 
# Wed, 29 Mar 2023 18:03:38 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 00:08:21 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 30 Mar 2023 00:08:22 GMT
RUN apk add --no-cache libssl1.1
# Thu, 30 Mar 2023 00:08:22 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 30 Mar 2023 00:08:30 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Thu, 30 Mar 2023 00:08:30 GMT
VOLUME [/spiped]
# Thu, 30 Mar 2023 00:08:30 GMT
WORKDIR /spiped
# Thu, 30 Mar 2023 00:08:30 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 30 Mar 2023 00:08:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 30 Mar 2023 00:08:31 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:fd4b2aeb476b6c2c0c3049dae919de20fe09e90deac95e3181d717055cbe6707`  
		Last Modified: Wed, 29 Mar 2023 18:06:56 GMT  
		Size: 2.9 MB (2868519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7df1c1b7ee69f0ffebff840bb383923a8a217c78132af46a52a21f12e14482c`  
		Last Modified: Sat, 08 Apr 2023 02:48:08 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e7fa369f75c521bfa073b091a994479792b5e564a5c37699be2008acad03c72`  
		Last Modified: Sat, 08 Apr 2023 02:48:09 GMT  
		Size: 1.2 MB (1167611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c21f3a95209349c9b1a3a521865cce5d3c5b7d5c8ff6ff9da5c62bb698fbf9c`  
		Last Modified: Sat, 08 Apr 2023 02:48:08 GMT  
		Size: 200.1 KB (200127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cd163e2f331db36950fd2761a2e3546fb04b46eba66cc2de8d5491d403e4be9`  
		Last Modified: Sat, 08 Apr 2023 02:48:08 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9e4936ce3183df5af3ef7fa3066376cab728047d4e40c1541aad098e3d01fb5`  
		Last Modified: Sat, 08 Apr 2023 02:48:08 GMT  
		Size: 336.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:b21f6104cf4f986ae42d2548c5a3e8edfeac1672739642c0051b1ce2e7ddc5dd
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.8 MB (4842828 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:306f5b9d541620eedadaec0c057f09c6db34da10d9378cae2f5155b0081420a9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 29 Mar 2023 17:39:18 GMT
ADD file:e51d4089e73ad6dee52b31f0c8059a00c17df6e23f6741fe11b43bd84cc99008 in / 
# Wed, 29 Mar 2023 17:39:18 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 05:50:31 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 30 Mar 2023 05:50:33 GMT
RUN apk add --no-cache libssl1.1
# Thu, 30 Mar 2023 05:50:33 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 30 Mar 2023 05:50:40 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Thu, 30 Mar 2023 05:50:40 GMT
VOLUME [/spiped]
# Thu, 30 Mar 2023 05:50:40 GMT
WORKDIR /spiped
# Thu, 30 Mar 2023 05:50:40 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 30 Mar 2023 05:50:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 30 Mar 2023 05:50:41 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:c41833b44d910632b415cd89a9cdaa4d62c9725dc56c99a7ddadafd6719960f9`  
		Last Modified: Wed, 29 Mar 2023 17:39:44 GMT  
		Size: 3.3 MB (3261854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46a75b9333a53162c1a5789a4c7973a5cc525b738e1a394e58db69d0c32fa089`  
		Last Modified: Thu, 30 Mar 2023 05:50:49 GMT  
		Size: 1.3 KB (1266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a905f71ab7e32bea70c662b413534aa7f764438f72937d84176a7b21115e19e`  
		Last Modified: Thu, 30 Mar 2023 05:50:50 GMT  
		Size: 1.4 MB (1363548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8364c9ed77705e5bab6f7d3ebcefe334f2401e4822779b17ceb1bb94d7510ce7`  
		Last Modified: Thu, 30 Mar 2023 05:50:50 GMT  
		Size: 215.7 KB (215692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d28a0bb75b3c36c6b1f0df28be9d91f3073dfcc4b0701cd2dffcafc2d8834c55`  
		Last Modified: Thu, 30 Mar 2023 05:50:49 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed9fdfb5809799657c2cc38eac53edd7e1105371601d7e1c155b00bf07f8f3d0`  
		Last Modified: Thu, 30 Mar 2023 05:50:49 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; 386

```console
$ docker pull spiped@sha256:0e5f49d56599b01f5aa0c4d6ebedb8fe9e52f5d2a66e094700b5f7703cc3f26e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.1 MB (5132057 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9fa9e52e3f82d57652b3398c82d896ea0c351c189b78a1daa85740fc04413b4d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 29 Mar 2023 17:38:30 GMT
ADD file:61bc44c9685b610d18bddd05d2ea1e57b4313f5f433a0a0b7e5269ec24f108b0 in / 
# Wed, 29 Mar 2023 17:38:30 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 01:33:08 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 30 Mar 2023 01:33:10 GMT
RUN apk add --no-cache libssl1.1
# Thu, 30 Mar 2023 01:33:10 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 30 Mar 2023 01:33:22 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Thu, 30 Mar 2023 01:33:22 GMT
VOLUME [/spiped]
# Thu, 30 Mar 2023 01:33:22 GMT
WORKDIR /spiped
# Thu, 30 Mar 2023 01:33:22 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 30 Mar 2023 01:33:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 30 Mar 2023 01:33:22 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:b2b0f0faedf1b87a3c77cf90d027fb7a25aa67f35400244a4655ad5842a757e4`  
		Last Modified: Wed, 29 Mar 2023 17:39:00 GMT  
		Size: 3.4 MB (3412260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09a513a8526f3d62fd7ec1e80a76b26d4cf8c8c37ea534b10e2c0060eb3cb6f0`  
		Last Modified: Thu, 30 Mar 2023 01:33:31 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa7fa7db70396ccd0f7c43ec98f7831c11a443d8d0f9ae5383bd39a0256cd39d`  
		Last Modified: Thu, 30 Mar 2023 01:33:32 GMT  
		Size: 1.5 MB (1486443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1d342e0d74297744901c335be2694a48a287375cc57389ee49fc329b6093f5a`  
		Last Modified: Thu, 30 Mar 2023 01:33:31 GMT  
		Size: 231.6 KB (231615 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1dc5bf7a2360503d1b51116e389e689406594d6295129a36524b8e4f7bad02d7`  
		Last Modified: Thu, 30 Mar 2023 01:33:31 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eae5cb4f4de570095d623ebcde4ca7cf3062c366c24ad3595d5108c7111c29af`  
		Last Modified: Thu, 30 Mar 2023 01:33:31 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; ppc64le

```console
$ docker pull spiped@sha256:8b13ec4b458ac31fb096b22da921ddc5f982ca84907ae2ad42dfc9935e69a793
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.0 MB (5025754 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:70983caa08c37ccc9d7968473ced65e5b8ee6cc50feff3049de378aee313e62f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 29 Mar 2023 18:16:27 GMT
ADD file:e95c1f256ba4bda85c5cbc0d8e84e6f329aa17c9dd2715b2da043e2139049124 in / 
# Wed, 29 Mar 2023 18:16:28 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 04:32:24 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 30 Mar 2023 04:32:26 GMT
RUN apk add --no-cache libssl1.1
# Thu, 30 Mar 2023 04:32:26 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 30 Mar 2023 04:32:41 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Thu, 30 Mar 2023 04:32:42 GMT
VOLUME [/spiped]
# Thu, 30 Mar 2023 04:32:43 GMT
WORKDIR /spiped
# Thu, 30 Mar 2023 04:32:43 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 30 Mar 2023 04:32:43 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 30 Mar 2023 04:32:44 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:1b7d25764eb3d3c55d73f5dfb9e3e9d75f3f39132e1b16142319de2a062dd673`  
		Last Modified: Wed, 29 Mar 2023 18:17:14 GMT  
		Size: 3.4 MB (3390935 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6abd914c752b02f6f79b7ef1571ed87d4130a25ed21a1d3892a23e3c2c1cfbec`  
		Last Modified: Thu, 30 Mar 2023 04:32:57 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3cc8ae50d4833e170ee7dc2db705d37cc39c4e228e121c72a14cd9620b4847c`  
		Last Modified: Thu, 30 Mar 2023 04:32:57 GMT  
		Size: 1.4 MB (1413051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac183c495785747e187a666506a1c63aeb182e3c511beaa79f82f4c86278a170`  
		Last Modified: Thu, 30 Mar 2023 04:32:57 GMT  
		Size: 220.0 KB (220030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8a70723c954d9ac5e16090c8b3aa6668bfab3384b6ce30cab8e10925bd1cd6c`  
		Last Modified: Thu, 30 Mar 2023 04:32:57 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85a4bf70a1b07cf55ae9e8498ca917bc7a43613629d823f0e1fa9b6c689b47b7`  
		Last Modified: Thu, 30 Mar 2023 04:32:57 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; s390x

```console
$ docker pull spiped@sha256:604fdf074de91d3fb86a39f54c9e130aeae2855ef71419e51d46b3fdbf10d3de
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.6 MB (4608998 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b8a0724e4059c76aefa5294b08af1999e786b6c97b94942a93375b39f74ec82a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 29 Mar 2023 17:41:57 GMT
ADD file:675ad8acf4b076e34aeeba26dd482be7640df5912b1ec5e3183b7eb69c01e83e in / 
# Wed, 29 Mar 2023 17:41:57 GMT
CMD ["/bin/sh"]
# Wed, 29 Mar 2023 22:37:24 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Wed, 29 Mar 2023 22:37:25 GMT
RUN apk add --no-cache libssl1.1
# Wed, 29 Mar 2023 22:37:25 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 29 Mar 2023 22:37:31 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Wed, 29 Mar 2023 22:37:31 GMT
VOLUME [/spiped]
# Wed, 29 Mar 2023 22:37:31 GMT
WORKDIR /spiped
# Wed, 29 Mar 2023 22:37:32 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 29 Mar 2023 22:37:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 29 Mar 2023 22:37:32 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:a76f78d8854217635d8049ec8501edb806f961e72989cfff8503982e6ff2579d`  
		Last Modified: Wed, 29 Mar 2023 17:42:31 GMT  
		Size: 3.2 MB (3175187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d252736c81578b3badb86bd65e11e8c42a3eced9b84da155c5d277746787398`  
		Last Modified: Wed, 29 Mar 2023 22:37:46 GMT  
		Size: 1.3 KB (1272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc4b9cdd39312641949e882585794aca9deab09fa611f8acf8a7b6c157519893`  
		Last Modified: Wed, 29 Mar 2023 22:37:46 GMT  
		Size: 1.2 MB (1223431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1da4a09ddda6c10edd737c5f0240c12ce3c655fe0cf8717062fdf0ab72f20285`  
		Last Modified: Wed, 29 Mar 2023 22:37:46 GMT  
		Size: 208.6 KB (208640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e3df4963fb4aa70acb7774a679b92580dffeb32ff4899e3ec8919a9feff0338`  
		Last Modified: Wed, 29 Mar 2023 22:37:46 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6af10966e7af681719def4af18b191e9fbdc7723fbc3c8f645089965679fe6c7`  
		Last Modified: Wed, 29 Mar 2023 22:37:46 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:1.6`

```console
$ docker pull spiped@sha256:3803fdc1e42df38ec09699a69d983e0c24277804803d456099a8989cefe72ace
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
$ docker pull spiped@sha256:721c9e3ecb57ab885c003700665c787207861ed892989be757c330a07a4c697c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.4 MB (37412915 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:be5ba0f72c5d2a07deab8c81f022c0d0da6de183e5be45bf75e5d2a765ce1241`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 23 Mar 2023 01:30:27 GMT
ADD file:60911afdacfdc216e44115addb5f3cc07f4166e8a4adf7be94a58aacc327ad63 in / 
# Thu, 23 Mar 2023 01:30:27 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 14:21:59 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Thu, 23 Mar 2023 14:22:02 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 14:22:03 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 23 Mar 2023 14:22:22 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 23 Mar 2023 14:22:22 GMT
VOLUME [/spiped]
# Thu, 23 Mar 2023 14:22:22 GMT
WORKDIR /spiped
# Thu, 23 Mar 2023 14:22:22 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 23 Mar 2023 14:22:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Mar 2023 14:22:22 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:f1f26f5702560b7e591bef5c4d840f76a232bf13fd5aefc4e22077a1ae4440c7`  
		Last Modified: Thu, 23 Mar 2023 01:34:23 GMT  
		Size: 31.4 MB (31411405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eba658cb120bd99022c7cf87e1a7e097de79f5861fc1b445ecbae4edeec1dfe4`  
		Last Modified: Thu, 23 Mar 2023 14:22:35 GMT  
		Size: 1.7 KB (1734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa69edd47542d8a3cf149d1bb36059f8c0e848ad433b8c659de5c1155781e12e`  
		Last Modified: Thu, 23 Mar 2023 14:22:35 GMT  
		Size: 1.1 KB (1050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:187bd75bf46234bc1609024e05712a659839202cc73b40db694672a1aff8b2c6`  
		Last Modified: Thu, 23 Mar 2023 14:22:36 GMT  
		Size: 6.0 MB (5998257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b9f50c988f7a169cc12e6566f824e86960bc77d0e2714a2ff2ddb919bec84f4`  
		Last Modified: Thu, 23 Mar 2023 14:22:35 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:866a419d38e59257252937a0d01999799ffb71213ebab6f7c0ba412832f7fbbe`  
		Last Modified: Thu, 23 Mar 2023 14:22:35 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; arm variant v5

```console
$ docker pull spiped@sha256:c56ad02f7a635dc4d379610e1a1095f9c487573ef61de595cba27525df82e0f0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.0 MB (33951316 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3289615005289139cb049ad1aaeaa83f924744ae842e267446c978996e7f8843`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 12 Apr 2023 00:48:41 GMT
ADD file:11004b5308adcb1c41526eac7071d373a5c42ca2e457a2e9e8b3a9d621c4e8e1 in / 
# Wed, 12 Apr 2023 00:48:41 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 04:13:45 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 12 Apr 2023 04:13:49 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 04:13:49 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 12 Apr 2023 04:14:09 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 12 Apr 2023 04:14:10 GMT
VOLUME [/spiped]
# Wed, 12 Apr 2023 04:14:10 GMT
WORKDIR /spiped
# Wed, 12 Apr 2023 04:14:10 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 12 Apr 2023 04:14:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 12 Apr 2023 04:14:10 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:5303309ebdb5d711447ed8a4ea072653ca7445c193060ec0aea30a89e92cda7e`  
		Last Modified: Wed, 12 Apr 2023 00:51:08 GMT  
		Size: 28.9 MB (28919551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c6d1cdee0b3069d6a9bbf71705b647047aa3718658646508ea3895abc295acd`  
		Last Modified: Wed, 12 Apr 2023 04:14:22 GMT  
		Size: 1.7 KB (1726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:413f2bdfff2530854dc8be54292587aacb28c20e08fbec5a75cd1c650b3ca0c6`  
		Last Modified: Wed, 12 Apr 2023 04:14:22 GMT  
		Size: 1.1 KB (1051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a772c2e19b2b59b3653449c3d87f10b14cad2ada0f4da89454a5d4216fb591c`  
		Last Modified: Wed, 12 Apr 2023 04:14:23 GMT  
		Size: 5.0 MB (5028515 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c462f1e36902eb29b25d02f2e17f167c04a3e4f838a3a5ab2227124fded03fb`  
		Last Modified: Wed, 12 Apr 2023 04:14:22 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edfdf45255e0c1a8dcac1dd2d2e36c424b51561ba09b234321f4589bcdab730d`  
		Last Modified: Wed, 12 Apr 2023 04:14:22 GMT  
		Size: 344.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; arm variant v7

```console
$ docker pull spiped@sha256:cf39f3bb40dcde6b5bf8478c9adb7d2539f890a17b9c12197f7ae968a28420f6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.3 MB (31329618 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1767501b8e0bc0f4d13978feac2b18de6af1c59fc29879fb0d1c08f1f85fcf84`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 23 Mar 2023 01:16:59 GMT
ADD file:1c83b99ee21091150a1c9ee8ef7c40bec3d6cb0d64b8bc0ef40fb97e6233aa5b in / 
# Thu, 23 Mar 2023 01:17:00 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 12:26:37 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Thu, 23 Mar 2023 12:26:40 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 12:26:40 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 23 Mar 2023 12:26:56 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 23 Mar 2023 12:26:56 GMT
VOLUME [/spiped]
# Thu, 23 Mar 2023 12:26:56 GMT
WORKDIR /spiped
# Thu, 23 Mar 2023 12:26:56 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 23 Mar 2023 12:26:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Mar 2023 12:26:56 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:2bc24e24d213c286ca4011c8b5cb7a3cf2a51f3bbedee8eeced46382bb5507bc`  
		Last Modified: Thu, 23 Mar 2023 01:33:18 GMT  
		Size: 26.6 MB (26577330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19061e17258a1ab423b9751a507a87e3c84da5eaffe1923ad2abc7aa5bf00be5`  
		Last Modified: Thu, 23 Mar 2023 12:27:07 GMT  
		Size: 1.7 KB (1727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0722d57fbb2b9577a072039b5f829c50b186b9d21b626777d773449488488fdc`  
		Last Modified: Thu, 23 Mar 2023 12:27:07 GMT  
		Size: 1.1 KB (1052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45c6b3401d253fee03596d2a401a84ebd8e4a340950690b66204e12a04889674`  
		Last Modified: Thu, 23 Mar 2023 12:27:08 GMT  
		Size: 4.7 MB (4749039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b000b28b92c3a6f78c372224d409ad90c989e6f0a43e4d9b72ae8ad4ccd28734`  
		Last Modified: Thu, 23 Mar 2023 12:27:07 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c563d03992865638f6480cdb6704eb9b8204b1c402024e2a101a161ede86290`  
		Last Modified: Thu, 23 Mar 2023 12:27:07 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:59a7ac95f3c86cfcda52266517687440ee833af0cfcd7bac7560d43faa690d52
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.3 MB (35339898 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:48134ae14be7815e330e696d68f5ce9f78018354a0b2aeef3cf707a462d57153`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 12 Apr 2023 00:39:49 GMT
ADD file:7b3c55926db26568f849247e80abdec3cfd6642929a40f0bbee95e4cb176051e in / 
# Wed, 12 Apr 2023 00:39:49 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 05:09:45 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 12 Apr 2023 05:09:48 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 05:09:48 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 12 Apr 2023 05:10:03 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 12 Apr 2023 05:10:03 GMT
VOLUME [/spiped]
# Wed, 12 Apr 2023 05:10:03 GMT
WORKDIR /spiped
# Wed, 12 Apr 2023 05:10:03 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 12 Apr 2023 05:10:03 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 12 Apr 2023 05:10:03 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:ebc3dc5a2d72427c585c8cda7574a75d96e04b9a37572bd3af0bff905abefbb9`  
		Last Modified: Wed, 12 Apr 2023 00:42:35 GMT  
		Size: 30.1 MB (30063826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3875f32a5967d63af0264c7e837f0ec1af397174340c608406c8dc1c4efd6d0`  
		Last Modified: Wed, 12 Apr 2023 05:10:15 GMT  
		Size: 1.7 KB (1734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d3c045802f338371900f62902ca0526fcbe0f103f1782134df45d785ec50a3b`  
		Last Modified: Wed, 12 Apr 2023 05:10:15 GMT  
		Size: 1.1 KB (1052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2cf02c8c59a3d5dfbb72551bda146e124e152fc03ddae5703249f6dfce3a7db`  
		Last Modified: Wed, 12 Apr 2023 05:10:16 GMT  
		Size: 5.3 MB (5272817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eafbdd4f6fdf5ed1c3903c9d26f47af77dcbde36fd86079557354b0153d0fd7b`  
		Last Modified: Wed, 12 Apr 2023 05:10:15 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9422d8f8fafc31168cc5eaebe935dfc7fde33c3e800595ec728d2d9fe52717fc`  
		Last Modified: Wed, 12 Apr 2023 05:10:16 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; 386

```console
$ docker pull spiped@sha256:74d7f5c8f3f3d9c67ac2694a397c85180e9414b6092e41e394b39054f2029c92
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.3 MB (40291472 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cd42d521cfced48016618daf00f5e6976442656bf9c4005a7c8200ef734bcbd4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 23 Mar 2023 00:39:18 GMT
ADD file:315d843eefd4a8bb2345366dcd6bab00a06fca4a7970e220ae8946123d07d7ed in / 
# Thu, 23 Mar 2023 00:39:19 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 12:10:30 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Thu, 23 Mar 2023 12:10:33 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 12:10:33 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 23 Mar 2023 12:10:56 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 23 Mar 2023 12:10:56 GMT
VOLUME [/spiped]
# Thu, 23 Mar 2023 12:10:56 GMT
WORKDIR /spiped
# Thu, 23 Mar 2023 12:10:56 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 23 Mar 2023 12:10:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Mar 2023 12:10:57 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:3e638a975ea99fe8646002726dcb1ccdccc49ad33967b30337b9b2413e0619b5`  
		Last Modified: Thu, 23 Mar 2023 00:43:09 GMT  
		Size: 32.4 MB (32396277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8c70cbb4c8fd8326cfa3a38bcadaebdcf624fcd76381d57288eb687694073d1`  
		Last Modified: Thu, 23 Mar 2023 12:11:11 GMT  
		Size: 1.7 KB (1725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b85e36913d82a6dadb0781c7ab440ef652976cc8995f5f0a0bd0541b9b620373`  
		Last Modified: Thu, 23 Mar 2023 12:11:11 GMT  
		Size: 1.1 KB (1054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bec8a50af228e59f346840b516f8f52a3b22b0be6d31a71d1341b272cc16d2ad`  
		Last Modified: Thu, 23 Mar 2023 12:11:13 GMT  
		Size: 7.9 MB (7891948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af275a5a028f320d08a155a1238d5121d8a0198cebf123d479cfab9a01aafd10`  
		Last Modified: Thu, 23 Mar 2023 12:11:11 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:409fcb43c7b4c77abd48e9757bd49eadd9c1aade55294cd9145e4f451a2a7a75`  
		Last Modified: Thu, 23 Mar 2023 12:11:11 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; mips64le

```console
$ docker pull spiped@sha256:62230d57630eb194945dc5756f3ee3712d046b75a1dd34bf2492a6418d46c0c5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.3 MB (35342788 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8418f829109d61f98060ab82e69f86501a87342a4f87913c3caeeb250c189e00`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 23 Mar 2023 05:17:57 GMT
ADD file:fd3a8eec4ae8f6058f522536ca9af1b391f3032504c085d8ddb6f4878ca478d5 in / 
# Thu, 23 Mar 2023 05:18:02 GMT
CMD ["bash"]
# Fri, 24 Mar 2023 05:00:18 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Fri, 24 Mar 2023 05:00:32 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Fri, 24 Mar 2023 05:00:34 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Fri, 24 Mar 2023 05:02:12 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Fri, 24 Mar 2023 05:02:15 GMT
VOLUME [/spiped]
# Fri, 24 Mar 2023 05:02:18 GMT
WORKDIR /spiped
# Fri, 24 Mar 2023 05:02:20 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 24 Mar 2023 05:02:23 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Mar 2023 05:02:25 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:735f9e60414e17ec59baef702f7013b7327899801df2ecf10123ce2727d8dea5`  
		Last Modified: Thu, 23 Mar 2023 05:25:53 GMT  
		Size: 29.6 MB (29634483 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9a95c8da754e637392a1172bcb5e591bcfcee63c2487be6f26b2c7489db5a7a`  
		Last Modified: Fri, 24 Mar 2023 05:02:46 GMT  
		Size: 1.6 KB (1622 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd933d8bf0d5ecf038fba2d2a35b694d9bf219c863351085755e909ab6c35b68`  
		Last Modified: Fri, 24 Mar 2023 05:02:46 GMT  
		Size: 926.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5db34c43bd622971b73a1d85c07581e353bf4e2ea607f6d6fcccd6a01f4fe2af`  
		Last Modified: Fri, 24 Mar 2023 05:02:51 GMT  
		Size: 5.7 MB (5705322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:476c1e9034825a9660cd4864a260cd15699063d1ed614ca97343aa9e139f1a36`  
		Last Modified: Fri, 24 Mar 2023 05:02:46 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ce2516d3dc94f7447fdff0b2538709c3ea3641cea323cd4d781e63909477f18`  
		Last Modified: Fri, 24 Mar 2023 05:02:46 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; ppc64le

```console
$ docker pull spiped@sha256:f401ab547830f955399b7c0c1037926954410f08e2308f97b2f1e114bf6c259b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.3 MB (41290962 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e8453ca71665e6fc2f4410696c68b7f0e85ba0d198b69afe7a94b47804fa1b94`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 23 Mar 2023 01:19:48 GMT
ADD file:fbd36b7667327dd30171fc49b8e028b8371fdbc7d30ee673808d508557f78bf1 in / 
# Thu, 23 Mar 2023 01:19:49 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 16:21:57 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Thu, 23 Mar 2023 16:22:03 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 16:22:03 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 23 Mar 2023 16:22:48 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 23 Mar 2023 16:22:49 GMT
VOLUME [/spiped]
# Thu, 23 Mar 2023 16:22:49 GMT
WORKDIR /spiped
# Thu, 23 Mar 2023 16:22:49 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 23 Mar 2023 16:22:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Mar 2023 16:22:50 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:8f472ad0a3fa58b4e304d1a974f25615d5bd3b7a99dff9c8202bd30facef0155`  
		Last Modified: Thu, 23 Mar 2023 01:24:22 GMT  
		Size: 35.3 MB (35288050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4167de1b2f5e0621dc4ea93047f68b495e3ff1d47ad708aeb47dacc4d98e4d6a`  
		Last Modified: Thu, 23 Mar 2023 16:23:05 GMT  
		Size: 1.7 KB (1732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:268241dc91792d1ad06458566222f09588696272408743915b59f8f440290b1c`  
		Last Modified: Thu, 23 Mar 2023 16:23:05 GMT  
		Size: 1.1 KB (1054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8dae255202559b344f349ed2396795c7dbc31726de4c1f57564193a10a4737e`  
		Last Modified: Thu, 23 Mar 2023 16:23:07 GMT  
		Size: 6.0 MB (5999654 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:047050eb0511c54c1aed11a944fdd94382d4abf66190b183f205e829e05e92b3`  
		Last Modified: Thu, 23 Mar 2023 16:23:05 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42ed775b429742a2b9aa4f680d2104804ccaac99aeccda29c0e231896875d5dc`  
		Last Modified: Thu, 23 Mar 2023 16:23:05 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; s390x

```console
$ docker pull spiped@sha256:bd0f6a8ba4b8c11fe888fee6860ea1d54be076bfe5957b43344b7b62dec0f47c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.8 MB (34844023 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:434b1ada99c83de5816075c26b07f7e49e021c25d4e40b80ddaf363ced468b65`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 12 Apr 2023 00:01:00 GMT
ADD file:b6463dba97ba9c0a29bacfafc4d67bc603ab57e80b75e23cd42d7ef4b0f8e6ae in / 
# Wed, 12 Apr 2023 00:01:04 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 07:13:35 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 12 Apr 2023 07:13:37 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 07:13:37 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 12 Apr 2023 07:13:53 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 12 Apr 2023 07:13:54 GMT
VOLUME [/spiped]
# Wed, 12 Apr 2023 07:13:54 GMT
WORKDIR /spiped
# Wed, 12 Apr 2023 07:13:54 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 12 Apr 2023 07:13:54 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 12 Apr 2023 07:13:54 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:97fe10bc7def58e7938e97e41eec4788ec7a45b6ef2cb1770cec02fa831fd19d`  
		Last Modified: Wed, 12 Apr 2023 00:05:18 GMT  
		Size: 29.7 MB (29653156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60661451feca33d0d1fc43f91b66dabebcd27f2ad19153400d0feafc64799c08`  
		Last Modified: Wed, 12 Apr 2023 07:14:13 GMT  
		Size: 1.7 KB (1736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28a1ae3818d2c3bcea0558356a7a736f1cc9b24645b2ad17f5a548b75d857b3b`  
		Last Modified: Wed, 12 Apr 2023 07:14:13 GMT  
		Size: 1.1 KB (1050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f4048da853c0e9dbdd6b2016bd4357a1c880ae93bc8c8567bbd675caccd414b`  
		Last Modified: Wed, 12 Apr 2023 07:14:14 GMT  
		Size: 5.2 MB (5187613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:302aa23f2c1ca3a68f99772fae7ea836cbcbc3330cca4b8604b18889c292b96d`  
		Last Modified: Wed, 12 Apr 2023 07:14:13 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74dc85c46ada57925ebdfcf7391a313ed62367842185b9add5f65f61a2945c2c`  
		Last Modified: Wed, 12 Apr 2023 07:14:13 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:1.6-alpine`

```console
$ docker pull spiped@sha256:657bd49b462533d254e7d5b3216fde01bc59a24c4f6277b050ae5bdc8f548a87
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
$ docker pull spiped@sha256:7b7f7844dc68c4b9728d9185d906025f7565df88ca9612aaaf420ac91523f405
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.1 MB (5080949 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2b60c5b50be16ba58852d923ea4e7d5224aecb355eb4588ab08b2f70c72ad851`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 29 Mar 2023 18:19:24 GMT
ADD file:9a4f77dfaba7fd2aa78186e4ef0e7486ad55101cefc1fabbc1b385601bb38920 in / 
# Wed, 29 Mar 2023 18:19:24 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 02:36:50 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 30 Mar 2023 02:36:51 GMT
RUN apk add --no-cache libssl1.1
# Thu, 30 Mar 2023 02:36:51 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 30 Mar 2023 02:37:01 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Thu, 30 Mar 2023 02:37:01 GMT
VOLUME [/spiped]
# Thu, 30 Mar 2023 02:37:02 GMT
WORKDIR /spiped
# Thu, 30 Mar 2023 02:37:02 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 30 Mar 2023 02:37:02 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 30 Mar 2023 02:37:02 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:f56be85fc22e46face30e2c3de3f7fe7c15f8fd7c4e5add29d7f64b87abdaa09`  
		Last Modified: Wed, 29 Mar 2023 18:19:57 GMT  
		Size: 3.4 MB (3374563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:833c4ea98211ab2b826b6d62f250a61b8c5ae407b5de38776cc5bc31d895d3fa`  
		Last Modified: Thu, 30 Mar 2023 02:37:13 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:870359eb3ab308a11eaf9cfc6782cd2bea0c513f3920492180bd5f5cbbea54eb`  
		Last Modified: Thu, 30 Mar 2023 02:37:13 GMT  
		Size: 1.5 MB (1483362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4afeb4ec06ad120774f5e7a75610323bda25b84d5957c8bac3f5c90ea7fdd17`  
		Last Modified: Thu, 30 Mar 2023 02:37:13 GMT  
		Size: 221.3 KB (221284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9641a8793752f42f60dcbb12e857125ba41995c02e48630112ef3f6d5747a28`  
		Last Modified: Thu, 30 Mar 2023 02:37:13 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb90b001556af3810279377523e96a71161f2dc727b628cb3d284764e5e847fd`  
		Last Modified: Thu, 30 Mar 2023 02:37:13 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; arm variant v6

```console
$ docker pull spiped@sha256:98e69abcdbbbc31f8223857ec6529b855f8e21be02602fe6763b73403a252650
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.6 MB (4560042 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c4871452a88018819e0282cc73c7c17274cbea4b4fd8f73619664078771460b6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 29 Mar 2023 18:01:09 GMT
ADD file:2dd294d20c0b500c8fed6b410b059429b36f51cd48a45eaf7a06ecbef9e2a3bb in / 
# Wed, 29 Mar 2023 18:01:09 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 00:22:48 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 30 Mar 2023 00:22:50 GMT
RUN apk add --no-cache libssl1.1
# Thu, 30 Mar 2023 00:22:50 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 30 Mar 2023 00:22:58 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Thu, 30 Mar 2023 00:22:58 GMT
VOLUME [/spiped]
# Thu, 30 Mar 2023 00:22:58 GMT
WORKDIR /spiped
# Thu, 30 Mar 2023 00:22:58 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 30 Mar 2023 00:22:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 30 Mar 2023 00:22:58 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:75257e753735e4ff78fae2d44018022a6ac775290e02103713a70699ece7576e`  
		Last Modified: Wed, 29 Mar 2023 18:01:52 GMT  
		Size: 3.1 MB (3110802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76f18e2ef9b0aa3ce161a88dbc21a7f6e04c161889cd2e9a48db6753f539a908`  
		Last Modified: Thu, 30 Mar 2023 00:24:29 GMT  
		Size: 1.3 KB (1267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f98080b1dde5f78f59c30b4e0ecd3d8755ce81a51335edb1f928872b6ea2758`  
		Last Modified: Thu, 30 Mar 2023 00:24:29 GMT  
		Size: 1.2 MB (1241151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2aaabfafc343e9926cb7046e859064ad3777e2fc8cddcb7e477dde08175094e7`  
		Last Modified: Thu, 30 Mar 2023 00:24:29 GMT  
		Size: 206.4 KB (206355 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e41f7588b8c91b544e8c7d054c90e59b7a9bd11c4e88918abb84a283000e0017`  
		Last Modified: Thu, 30 Mar 2023 00:24:29 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17cd529e07580d9750fa02477c2004129b10b554d974efb4047239df64df3a24`  
		Last Modified: Thu, 30 Mar 2023 00:24:29 GMT  
		Size: 338.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; arm variant v7

```console
$ docker pull spiped@sha256:6c2a2f1aeafd6139364938089caba1b87ad68bedb26cd1880228677d027a8a71
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4237992 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7a9eb306d4124eb8e1c6195849bb2b723860dae03a03f9bae43f0cb32e1462fd`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 29 Mar 2023 18:03:38 GMT
ADD file:959fa0ffb60c37c4fdc0d32ac31511f8dead32ef7f4bd848b11ff144a6b37012 in / 
# Wed, 29 Mar 2023 18:03:38 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 00:08:21 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 30 Mar 2023 00:08:22 GMT
RUN apk add --no-cache libssl1.1
# Thu, 30 Mar 2023 00:08:22 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 30 Mar 2023 00:08:30 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Thu, 30 Mar 2023 00:08:30 GMT
VOLUME [/spiped]
# Thu, 30 Mar 2023 00:08:30 GMT
WORKDIR /spiped
# Thu, 30 Mar 2023 00:08:30 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 30 Mar 2023 00:08:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 30 Mar 2023 00:08:31 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:fd4b2aeb476b6c2c0c3049dae919de20fe09e90deac95e3181d717055cbe6707`  
		Last Modified: Wed, 29 Mar 2023 18:06:56 GMT  
		Size: 2.9 MB (2868519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7df1c1b7ee69f0ffebff840bb383923a8a217c78132af46a52a21f12e14482c`  
		Last Modified: Sat, 08 Apr 2023 02:48:08 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e7fa369f75c521bfa073b091a994479792b5e564a5c37699be2008acad03c72`  
		Last Modified: Sat, 08 Apr 2023 02:48:09 GMT  
		Size: 1.2 MB (1167611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c21f3a95209349c9b1a3a521865cce5d3c5b7d5c8ff6ff9da5c62bb698fbf9c`  
		Last Modified: Sat, 08 Apr 2023 02:48:08 GMT  
		Size: 200.1 KB (200127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cd163e2f331db36950fd2761a2e3546fb04b46eba66cc2de8d5491d403e4be9`  
		Last Modified: Sat, 08 Apr 2023 02:48:08 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9e4936ce3183df5af3ef7fa3066376cab728047d4e40c1541aad098e3d01fb5`  
		Last Modified: Sat, 08 Apr 2023 02:48:08 GMT  
		Size: 336.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:b21f6104cf4f986ae42d2548c5a3e8edfeac1672739642c0051b1ce2e7ddc5dd
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.8 MB (4842828 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:306f5b9d541620eedadaec0c057f09c6db34da10d9378cae2f5155b0081420a9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 29 Mar 2023 17:39:18 GMT
ADD file:e51d4089e73ad6dee52b31f0c8059a00c17df6e23f6741fe11b43bd84cc99008 in / 
# Wed, 29 Mar 2023 17:39:18 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 05:50:31 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 30 Mar 2023 05:50:33 GMT
RUN apk add --no-cache libssl1.1
# Thu, 30 Mar 2023 05:50:33 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 30 Mar 2023 05:50:40 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Thu, 30 Mar 2023 05:50:40 GMT
VOLUME [/spiped]
# Thu, 30 Mar 2023 05:50:40 GMT
WORKDIR /spiped
# Thu, 30 Mar 2023 05:50:40 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 30 Mar 2023 05:50:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 30 Mar 2023 05:50:41 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:c41833b44d910632b415cd89a9cdaa4d62c9725dc56c99a7ddadafd6719960f9`  
		Last Modified: Wed, 29 Mar 2023 17:39:44 GMT  
		Size: 3.3 MB (3261854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46a75b9333a53162c1a5789a4c7973a5cc525b738e1a394e58db69d0c32fa089`  
		Last Modified: Thu, 30 Mar 2023 05:50:49 GMT  
		Size: 1.3 KB (1266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a905f71ab7e32bea70c662b413534aa7f764438f72937d84176a7b21115e19e`  
		Last Modified: Thu, 30 Mar 2023 05:50:50 GMT  
		Size: 1.4 MB (1363548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8364c9ed77705e5bab6f7d3ebcefe334f2401e4822779b17ceb1bb94d7510ce7`  
		Last Modified: Thu, 30 Mar 2023 05:50:50 GMT  
		Size: 215.7 KB (215692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d28a0bb75b3c36c6b1f0df28be9d91f3073dfcc4b0701cd2dffcafc2d8834c55`  
		Last Modified: Thu, 30 Mar 2023 05:50:49 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed9fdfb5809799657c2cc38eac53edd7e1105371601d7e1c155b00bf07f8f3d0`  
		Last Modified: Thu, 30 Mar 2023 05:50:49 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; 386

```console
$ docker pull spiped@sha256:0e5f49d56599b01f5aa0c4d6ebedb8fe9e52f5d2a66e094700b5f7703cc3f26e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.1 MB (5132057 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9fa9e52e3f82d57652b3398c82d896ea0c351c189b78a1daa85740fc04413b4d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 29 Mar 2023 17:38:30 GMT
ADD file:61bc44c9685b610d18bddd05d2ea1e57b4313f5f433a0a0b7e5269ec24f108b0 in / 
# Wed, 29 Mar 2023 17:38:30 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 01:33:08 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 30 Mar 2023 01:33:10 GMT
RUN apk add --no-cache libssl1.1
# Thu, 30 Mar 2023 01:33:10 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 30 Mar 2023 01:33:22 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Thu, 30 Mar 2023 01:33:22 GMT
VOLUME [/spiped]
# Thu, 30 Mar 2023 01:33:22 GMT
WORKDIR /spiped
# Thu, 30 Mar 2023 01:33:22 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 30 Mar 2023 01:33:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 30 Mar 2023 01:33:22 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:b2b0f0faedf1b87a3c77cf90d027fb7a25aa67f35400244a4655ad5842a757e4`  
		Last Modified: Wed, 29 Mar 2023 17:39:00 GMT  
		Size: 3.4 MB (3412260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09a513a8526f3d62fd7ec1e80a76b26d4cf8c8c37ea534b10e2c0060eb3cb6f0`  
		Last Modified: Thu, 30 Mar 2023 01:33:31 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa7fa7db70396ccd0f7c43ec98f7831c11a443d8d0f9ae5383bd39a0256cd39d`  
		Last Modified: Thu, 30 Mar 2023 01:33:32 GMT  
		Size: 1.5 MB (1486443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1d342e0d74297744901c335be2694a48a287375cc57389ee49fc329b6093f5a`  
		Last Modified: Thu, 30 Mar 2023 01:33:31 GMT  
		Size: 231.6 KB (231615 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1dc5bf7a2360503d1b51116e389e689406594d6295129a36524b8e4f7bad02d7`  
		Last Modified: Thu, 30 Mar 2023 01:33:31 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eae5cb4f4de570095d623ebcde4ca7cf3062c366c24ad3595d5108c7111c29af`  
		Last Modified: Thu, 30 Mar 2023 01:33:31 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; ppc64le

```console
$ docker pull spiped@sha256:8b13ec4b458ac31fb096b22da921ddc5f982ca84907ae2ad42dfc9935e69a793
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.0 MB (5025754 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:70983caa08c37ccc9d7968473ced65e5b8ee6cc50feff3049de378aee313e62f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 29 Mar 2023 18:16:27 GMT
ADD file:e95c1f256ba4bda85c5cbc0d8e84e6f329aa17c9dd2715b2da043e2139049124 in / 
# Wed, 29 Mar 2023 18:16:28 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 04:32:24 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 30 Mar 2023 04:32:26 GMT
RUN apk add --no-cache libssl1.1
# Thu, 30 Mar 2023 04:32:26 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 30 Mar 2023 04:32:41 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Thu, 30 Mar 2023 04:32:42 GMT
VOLUME [/spiped]
# Thu, 30 Mar 2023 04:32:43 GMT
WORKDIR /spiped
# Thu, 30 Mar 2023 04:32:43 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 30 Mar 2023 04:32:43 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 30 Mar 2023 04:32:44 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:1b7d25764eb3d3c55d73f5dfb9e3e9d75f3f39132e1b16142319de2a062dd673`  
		Last Modified: Wed, 29 Mar 2023 18:17:14 GMT  
		Size: 3.4 MB (3390935 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6abd914c752b02f6f79b7ef1571ed87d4130a25ed21a1d3892a23e3c2c1cfbec`  
		Last Modified: Thu, 30 Mar 2023 04:32:57 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3cc8ae50d4833e170ee7dc2db705d37cc39c4e228e121c72a14cd9620b4847c`  
		Last Modified: Thu, 30 Mar 2023 04:32:57 GMT  
		Size: 1.4 MB (1413051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac183c495785747e187a666506a1c63aeb182e3c511beaa79f82f4c86278a170`  
		Last Modified: Thu, 30 Mar 2023 04:32:57 GMT  
		Size: 220.0 KB (220030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8a70723c954d9ac5e16090c8b3aa6668bfab3384b6ce30cab8e10925bd1cd6c`  
		Last Modified: Thu, 30 Mar 2023 04:32:57 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85a4bf70a1b07cf55ae9e8498ca917bc7a43613629d823f0e1fa9b6c689b47b7`  
		Last Modified: Thu, 30 Mar 2023 04:32:57 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; s390x

```console
$ docker pull spiped@sha256:604fdf074de91d3fb86a39f54c9e130aeae2855ef71419e51d46b3fdbf10d3de
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.6 MB (4608998 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b8a0724e4059c76aefa5294b08af1999e786b6c97b94942a93375b39f74ec82a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 29 Mar 2023 17:41:57 GMT
ADD file:675ad8acf4b076e34aeeba26dd482be7640df5912b1ec5e3183b7eb69c01e83e in / 
# Wed, 29 Mar 2023 17:41:57 GMT
CMD ["/bin/sh"]
# Wed, 29 Mar 2023 22:37:24 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Wed, 29 Mar 2023 22:37:25 GMT
RUN apk add --no-cache libssl1.1
# Wed, 29 Mar 2023 22:37:25 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 29 Mar 2023 22:37:31 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Wed, 29 Mar 2023 22:37:31 GMT
VOLUME [/spiped]
# Wed, 29 Mar 2023 22:37:31 GMT
WORKDIR /spiped
# Wed, 29 Mar 2023 22:37:32 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 29 Mar 2023 22:37:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 29 Mar 2023 22:37:32 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:a76f78d8854217635d8049ec8501edb806f961e72989cfff8503982e6ff2579d`  
		Last Modified: Wed, 29 Mar 2023 17:42:31 GMT  
		Size: 3.2 MB (3175187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d252736c81578b3badb86bd65e11e8c42a3eced9b84da155c5d277746787398`  
		Last Modified: Wed, 29 Mar 2023 22:37:46 GMT  
		Size: 1.3 KB (1272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc4b9cdd39312641949e882585794aca9deab09fa611f8acf8a7b6c157519893`  
		Last Modified: Wed, 29 Mar 2023 22:37:46 GMT  
		Size: 1.2 MB (1223431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1da4a09ddda6c10edd737c5f0240c12ce3c655fe0cf8717062fdf0ab72f20285`  
		Last Modified: Wed, 29 Mar 2023 22:37:46 GMT  
		Size: 208.6 KB (208640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e3df4963fb4aa70acb7774a679b92580dffeb32ff4899e3ec8919a9feff0338`  
		Last Modified: Wed, 29 Mar 2023 22:37:46 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6af10966e7af681719def4af18b191e9fbdc7723fbc3c8f645089965679fe6c7`  
		Last Modified: Wed, 29 Mar 2023 22:37:46 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:1.6.2`

```console
$ docker pull spiped@sha256:3803fdc1e42df38ec09699a69d983e0c24277804803d456099a8989cefe72ace
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
$ docker pull spiped@sha256:721c9e3ecb57ab885c003700665c787207861ed892989be757c330a07a4c697c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.4 MB (37412915 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:be5ba0f72c5d2a07deab8c81f022c0d0da6de183e5be45bf75e5d2a765ce1241`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 23 Mar 2023 01:30:27 GMT
ADD file:60911afdacfdc216e44115addb5f3cc07f4166e8a4adf7be94a58aacc327ad63 in / 
# Thu, 23 Mar 2023 01:30:27 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 14:21:59 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Thu, 23 Mar 2023 14:22:02 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 14:22:03 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 23 Mar 2023 14:22:22 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 23 Mar 2023 14:22:22 GMT
VOLUME [/spiped]
# Thu, 23 Mar 2023 14:22:22 GMT
WORKDIR /spiped
# Thu, 23 Mar 2023 14:22:22 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 23 Mar 2023 14:22:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Mar 2023 14:22:22 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:f1f26f5702560b7e591bef5c4d840f76a232bf13fd5aefc4e22077a1ae4440c7`  
		Last Modified: Thu, 23 Mar 2023 01:34:23 GMT  
		Size: 31.4 MB (31411405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eba658cb120bd99022c7cf87e1a7e097de79f5861fc1b445ecbae4edeec1dfe4`  
		Last Modified: Thu, 23 Mar 2023 14:22:35 GMT  
		Size: 1.7 KB (1734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa69edd47542d8a3cf149d1bb36059f8c0e848ad433b8c659de5c1155781e12e`  
		Last Modified: Thu, 23 Mar 2023 14:22:35 GMT  
		Size: 1.1 KB (1050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:187bd75bf46234bc1609024e05712a659839202cc73b40db694672a1aff8b2c6`  
		Last Modified: Thu, 23 Mar 2023 14:22:36 GMT  
		Size: 6.0 MB (5998257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b9f50c988f7a169cc12e6566f824e86960bc77d0e2714a2ff2ddb919bec84f4`  
		Last Modified: Thu, 23 Mar 2023 14:22:35 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:866a419d38e59257252937a0d01999799ffb71213ebab6f7c0ba412832f7fbbe`  
		Last Modified: Thu, 23 Mar 2023 14:22:35 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.2` - linux; arm variant v5

```console
$ docker pull spiped@sha256:c56ad02f7a635dc4d379610e1a1095f9c487573ef61de595cba27525df82e0f0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.0 MB (33951316 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3289615005289139cb049ad1aaeaa83f924744ae842e267446c978996e7f8843`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 12 Apr 2023 00:48:41 GMT
ADD file:11004b5308adcb1c41526eac7071d373a5c42ca2e457a2e9e8b3a9d621c4e8e1 in / 
# Wed, 12 Apr 2023 00:48:41 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 04:13:45 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 12 Apr 2023 04:13:49 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 04:13:49 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 12 Apr 2023 04:14:09 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 12 Apr 2023 04:14:10 GMT
VOLUME [/spiped]
# Wed, 12 Apr 2023 04:14:10 GMT
WORKDIR /spiped
# Wed, 12 Apr 2023 04:14:10 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 12 Apr 2023 04:14:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 12 Apr 2023 04:14:10 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:5303309ebdb5d711447ed8a4ea072653ca7445c193060ec0aea30a89e92cda7e`  
		Last Modified: Wed, 12 Apr 2023 00:51:08 GMT  
		Size: 28.9 MB (28919551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c6d1cdee0b3069d6a9bbf71705b647047aa3718658646508ea3895abc295acd`  
		Last Modified: Wed, 12 Apr 2023 04:14:22 GMT  
		Size: 1.7 KB (1726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:413f2bdfff2530854dc8be54292587aacb28c20e08fbec5a75cd1c650b3ca0c6`  
		Last Modified: Wed, 12 Apr 2023 04:14:22 GMT  
		Size: 1.1 KB (1051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a772c2e19b2b59b3653449c3d87f10b14cad2ada0f4da89454a5d4216fb591c`  
		Last Modified: Wed, 12 Apr 2023 04:14:23 GMT  
		Size: 5.0 MB (5028515 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c462f1e36902eb29b25d02f2e17f167c04a3e4f838a3a5ab2227124fded03fb`  
		Last Modified: Wed, 12 Apr 2023 04:14:22 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edfdf45255e0c1a8dcac1dd2d2e36c424b51561ba09b234321f4589bcdab730d`  
		Last Modified: Wed, 12 Apr 2023 04:14:22 GMT  
		Size: 344.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.2` - linux; arm variant v7

```console
$ docker pull spiped@sha256:cf39f3bb40dcde6b5bf8478c9adb7d2539f890a17b9c12197f7ae968a28420f6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.3 MB (31329618 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1767501b8e0bc0f4d13978feac2b18de6af1c59fc29879fb0d1c08f1f85fcf84`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 23 Mar 2023 01:16:59 GMT
ADD file:1c83b99ee21091150a1c9ee8ef7c40bec3d6cb0d64b8bc0ef40fb97e6233aa5b in / 
# Thu, 23 Mar 2023 01:17:00 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 12:26:37 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Thu, 23 Mar 2023 12:26:40 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 12:26:40 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 23 Mar 2023 12:26:56 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 23 Mar 2023 12:26:56 GMT
VOLUME [/spiped]
# Thu, 23 Mar 2023 12:26:56 GMT
WORKDIR /spiped
# Thu, 23 Mar 2023 12:26:56 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 23 Mar 2023 12:26:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Mar 2023 12:26:56 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:2bc24e24d213c286ca4011c8b5cb7a3cf2a51f3bbedee8eeced46382bb5507bc`  
		Last Modified: Thu, 23 Mar 2023 01:33:18 GMT  
		Size: 26.6 MB (26577330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19061e17258a1ab423b9751a507a87e3c84da5eaffe1923ad2abc7aa5bf00be5`  
		Last Modified: Thu, 23 Mar 2023 12:27:07 GMT  
		Size: 1.7 KB (1727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0722d57fbb2b9577a072039b5f829c50b186b9d21b626777d773449488488fdc`  
		Last Modified: Thu, 23 Mar 2023 12:27:07 GMT  
		Size: 1.1 KB (1052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45c6b3401d253fee03596d2a401a84ebd8e4a340950690b66204e12a04889674`  
		Last Modified: Thu, 23 Mar 2023 12:27:08 GMT  
		Size: 4.7 MB (4749039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b000b28b92c3a6f78c372224d409ad90c989e6f0a43e4d9b72ae8ad4ccd28734`  
		Last Modified: Thu, 23 Mar 2023 12:27:07 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c563d03992865638f6480cdb6704eb9b8204b1c402024e2a101a161ede86290`  
		Last Modified: Thu, 23 Mar 2023 12:27:07 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.2` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:59a7ac95f3c86cfcda52266517687440ee833af0cfcd7bac7560d43faa690d52
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.3 MB (35339898 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:48134ae14be7815e330e696d68f5ce9f78018354a0b2aeef3cf707a462d57153`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 12 Apr 2023 00:39:49 GMT
ADD file:7b3c55926db26568f849247e80abdec3cfd6642929a40f0bbee95e4cb176051e in / 
# Wed, 12 Apr 2023 00:39:49 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 05:09:45 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 12 Apr 2023 05:09:48 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 05:09:48 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 12 Apr 2023 05:10:03 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 12 Apr 2023 05:10:03 GMT
VOLUME [/spiped]
# Wed, 12 Apr 2023 05:10:03 GMT
WORKDIR /spiped
# Wed, 12 Apr 2023 05:10:03 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 12 Apr 2023 05:10:03 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 12 Apr 2023 05:10:03 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:ebc3dc5a2d72427c585c8cda7574a75d96e04b9a37572bd3af0bff905abefbb9`  
		Last Modified: Wed, 12 Apr 2023 00:42:35 GMT  
		Size: 30.1 MB (30063826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3875f32a5967d63af0264c7e837f0ec1af397174340c608406c8dc1c4efd6d0`  
		Last Modified: Wed, 12 Apr 2023 05:10:15 GMT  
		Size: 1.7 KB (1734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d3c045802f338371900f62902ca0526fcbe0f103f1782134df45d785ec50a3b`  
		Last Modified: Wed, 12 Apr 2023 05:10:15 GMT  
		Size: 1.1 KB (1052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2cf02c8c59a3d5dfbb72551bda146e124e152fc03ddae5703249f6dfce3a7db`  
		Last Modified: Wed, 12 Apr 2023 05:10:16 GMT  
		Size: 5.3 MB (5272817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eafbdd4f6fdf5ed1c3903c9d26f47af77dcbde36fd86079557354b0153d0fd7b`  
		Last Modified: Wed, 12 Apr 2023 05:10:15 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9422d8f8fafc31168cc5eaebe935dfc7fde33c3e800595ec728d2d9fe52717fc`  
		Last Modified: Wed, 12 Apr 2023 05:10:16 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.2` - linux; 386

```console
$ docker pull spiped@sha256:74d7f5c8f3f3d9c67ac2694a397c85180e9414b6092e41e394b39054f2029c92
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.3 MB (40291472 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cd42d521cfced48016618daf00f5e6976442656bf9c4005a7c8200ef734bcbd4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 23 Mar 2023 00:39:18 GMT
ADD file:315d843eefd4a8bb2345366dcd6bab00a06fca4a7970e220ae8946123d07d7ed in / 
# Thu, 23 Mar 2023 00:39:19 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 12:10:30 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Thu, 23 Mar 2023 12:10:33 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 12:10:33 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 23 Mar 2023 12:10:56 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 23 Mar 2023 12:10:56 GMT
VOLUME [/spiped]
# Thu, 23 Mar 2023 12:10:56 GMT
WORKDIR /spiped
# Thu, 23 Mar 2023 12:10:56 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 23 Mar 2023 12:10:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Mar 2023 12:10:57 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:3e638a975ea99fe8646002726dcb1ccdccc49ad33967b30337b9b2413e0619b5`  
		Last Modified: Thu, 23 Mar 2023 00:43:09 GMT  
		Size: 32.4 MB (32396277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8c70cbb4c8fd8326cfa3a38bcadaebdcf624fcd76381d57288eb687694073d1`  
		Last Modified: Thu, 23 Mar 2023 12:11:11 GMT  
		Size: 1.7 KB (1725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b85e36913d82a6dadb0781c7ab440ef652976cc8995f5f0a0bd0541b9b620373`  
		Last Modified: Thu, 23 Mar 2023 12:11:11 GMT  
		Size: 1.1 KB (1054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bec8a50af228e59f346840b516f8f52a3b22b0be6d31a71d1341b272cc16d2ad`  
		Last Modified: Thu, 23 Mar 2023 12:11:13 GMT  
		Size: 7.9 MB (7891948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af275a5a028f320d08a155a1238d5121d8a0198cebf123d479cfab9a01aafd10`  
		Last Modified: Thu, 23 Mar 2023 12:11:11 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:409fcb43c7b4c77abd48e9757bd49eadd9c1aade55294cd9145e4f451a2a7a75`  
		Last Modified: Thu, 23 Mar 2023 12:11:11 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.2` - linux; mips64le

```console
$ docker pull spiped@sha256:62230d57630eb194945dc5756f3ee3712d046b75a1dd34bf2492a6418d46c0c5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.3 MB (35342788 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8418f829109d61f98060ab82e69f86501a87342a4f87913c3caeeb250c189e00`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 23 Mar 2023 05:17:57 GMT
ADD file:fd3a8eec4ae8f6058f522536ca9af1b391f3032504c085d8ddb6f4878ca478d5 in / 
# Thu, 23 Mar 2023 05:18:02 GMT
CMD ["bash"]
# Fri, 24 Mar 2023 05:00:18 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Fri, 24 Mar 2023 05:00:32 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Fri, 24 Mar 2023 05:00:34 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Fri, 24 Mar 2023 05:02:12 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Fri, 24 Mar 2023 05:02:15 GMT
VOLUME [/spiped]
# Fri, 24 Mar 2023 05:02:18 GMT
WORKDIR /spiped
# Fri, 24 Mar 2023 05:02:20 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 24 Mar 2023 05:02:23 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Mar 2023 05:02:25 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:735f9e60414e17ec59baef702f7013b7327899801df2ecf10123ce2727d8dea5`  
		Last Modified: Thu, 23 Mar 2023 05:25:53 GMT  
		Size: 29.6 MB (29634483 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9a95c8da754e637392a1172bcb5e591bcfcee63c2487be6f26b2c7489db5a7a`  
		Last Modified: Fri, 24 Mar 2023 05:02:46 GMT  
		Size: 1.6 KB (1622 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd933d8bf0d5ecf038fba2d2a35b694d9bf219c863351085755e909ab6c35b68`  
		Last Modified: Fri, 24 Mar 2023 05:02:46 GMT  
		Size: 926.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5db34c43bd622971b73a1d85c07581e353bf4e2ea607f6d6fcccd6a01f4fe2af`  
		Last Modified: Fri, 24 Mar 2023 05:02:51 GMT  
		Size: 5.7 MB (5705322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:476c1e9034825a9660cd4864a260cd15699063d1ed614ca97343aa9e139f1a36`  
		Last Modified: Fri, 24 Mar 2023 05:02:46 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ce2516d3dc94f7447fdff0b2538709c3ea3641cea323cd4d781e63909477f18`  
		Last Modified: Fri, 24 Mar 2023 05:02:46 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.2` - linux; ppc64le

```console
$ docker pull spiped@sha256:f401ab547830f955399b7c0c1037926954410f08e2308f97b2f1e114bf6c259b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.3 MB (41290962 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e8453ca71665e6fc2f4410696c68b7f0e85ba0d198b69afe7a94b47804fa1b94`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 23 Mar 2023 01:19:48 GMT
ADD file:fbd36b7667327dd30171fc49b8e028b8371fdbc7d30ee673808d508557f78bf1 in / 
# Thu, 23 Mar 2023 01:19:49 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 16:21:57 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Thu, 23 Mar 2023 16:22:03 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 16:22:03 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 23 Mar 2023 16:22:48 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 23 Mar 2023 16:22:49 GMT
VOLUME [/spiped]
# Thu, 23 Mar 2023 16:22:49 GMT
WORKDIR /spiped
# Thu, 23 Mar 2023 16:22:49 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 23 Mar 2023 16:22:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Mar 2023 16:22:50 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:8f472ad0a3fa58b4e304d1a974f25615d5bd3b7a99dff9c8202bd30facef0155`  
		Last Modified: Thu, 23 Mar 2023 01:24:22 GMT  
		Size: 35.3 MB (35288050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4167de1b2f5e0621dc4ea93047f68b495e3ff1d47ad708aeb47dacc4d98e4d6a`  
		Last Modified: Thu, 23 Mar 2023 16:23:05 GMT  
		Size: 1.7 KB (1732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:268241dc91792d1ad06458566222f09588696272408743915b59f8f440290b1c`  
		Last Modified: Thu, 23 Mar 2023 16:23:05 GMT  
		Size: 1.1 KB (1054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8dae255202559b344f349ed2396795c7dbc31726de4c1f57564193a10a4737e`  
		Last Modified: Thu, 23 Mar 2023 16:23:07 GMT  
		Size: 6.0 MB (5999654 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:047050eb0511c54c1aed11a944fdd94382d4abf66190b183f205e829e05e92b3`  
		Last Modified: Thu, 23 Mar 2023 16:23:05 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42ed775b429742a2b9aa4f680d2104804ccaac99aeccda29c0e231896875d5dc`  
		Last Modified: Thu, 23 Mar 2023 16:23:05 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.2` - linux; s390x

```console
$ docker pull spiped@sha256:bd0f6a8ba4b8c11fe888fee6860ea1d54be076bfe5957b43344b7b62dec0f47c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.8 MB (34844023 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:434b1ada99c83de5816075c26b07f7e49e021c25d4e40b80ddaf363ced468b65`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 12 Apr 2023 00:01:00 GMT
ADD file:b6463dba97ba9c0a29bacfafc4d67bc603ab57e80b75e23cd42d7ef4b0f8e6ae in / 
# Wed, 12 Apr 2023 00:01:04 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 07:13:35 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 12 Apr 2023 07:13:37 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 07:13:37 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 12 Apr 2023 07:13:53 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 12 Apr 2023 07:13:54 GMT
VOLUME [/spiped]
# Wed, 12 Apr 2023 07:13:54 GMT
WORKDIR /spiped
# Wed, 12 Apr 2023 07:13:54 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 12 Apr 2023 07:13:54 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 12 Apr 2023 07:13:54 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:97fe10bc7def58e7938e97e41eec4788ec7a45b6ef2cb1770cec02fa831fd19d`  
		Last Modified: Wed, 12 Apr 2023 00:05:18 GMT  
		Size: 29.7 MB (29653156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60661451feca33d0d1fc43f91b66dabebcd27f2ad19153400d0feafc64799c08`  
		Last Modified: Wed, 12 Apr 2023 07:14:13 GMT  
		Size: 1.7 KB (1736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28a1ae3818d2c3bcea0558356a7a736f1cc9b24645b2ad17f5a548b75d857b3b`  
		Last Modified: Wed, 12 Apr 2023 07:14:13 GMT  
		Size: 1.1 KB (1050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f4048da853c0e9dbdd6b2016bd4357a1c880ae93bc8c8567bbd675caccd414b`  
		Last Modified: Wed, 12 Apr 2023 07:14:14 GMT  
		Size: 5.2 MB (5187613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:302aa23f2c1ca3a68f99772fae7ea836cbcbc3330cca4b8604b18889c292b96d`  
		Last Modified: Wed, 12 Apr 2023 07:14:13 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74dc85c46ada57925ebdfcf7391a313ed62367842185b9add5f65f61a2945c2c`  
		Last Modified: Wed, 12 Apr 2023 07:14:13 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:1.6.2-alpine`

```console
$ docker pull spiped@sha256:657bd49b462533d254e7d5b3216fde01bc59a24c4f6277b050ae5bdc8f548a87
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
$ docker pull spiped@sha256:7b7f7844dc68c4b9728d9185d906025f7565df88ca9612aaaf420ac91523f405
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.1 MB (5080949 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2b60c5b50be16ba58852d923ea4e7d5224aecb355eb4588ab08b2f70c72ad851`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 29 Mar 2023 18:19:24 GMT
ADD file:9a4f77dfaba7fd2aa78186e4ef0e7486ad55101cefc1fabbc1b385601bb38920 in / 
# Wed, 29 Mar 2023 18:19:24 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 02:36:50 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 30 Mar 2023 02:36:51 GMT
RUN apk add --no-cache libssl1.1
# Thu, 30 Mar 2023 02:36:51 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 30 Mar 2023 02:37:01 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Thu, 30 Mar 2023 02:37:01 GMT
VOLUME [/spiped]
# Thu, 30 Mar 2023 02:37:02 GMT
WORKDIR /spiped
# Thu, 30 Mar 2023 02:37:02 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 30 Mar 2023 02:37:02 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 30 Mar 2023 02:37:02 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:f56be85fc22e46face30e2c3de3f7fe7c15f8fd7c4e5add29d7f64b87abdaa09`  
		Last Modified: Wed, 29 Mar 2023 18:19:57 GMT  
		Size: 3.4 MB (3374563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:833c4ea98211ab2b826b6d62f250a61b8c5ae407b5de38776cc5bc31d895d3fa`  
		Last Modified: Thu, 30 Mar 2023 02:37:13 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:870359eb3ab308a11eaf9cfc6782cd2bea0c513f3920492180bd5f5cbbea54eb`  
		Last Modified: Thu, 30 Mar 2023 02:37:13 GMT  
		Size: 1.5 MB (1483362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4afeb4ec06ad120774f5e7a75610323bda25b84d5957c8bac3f5c90ea7fdd17`  
		Last Modified: Thu, 30 Mar 2023 02:37:13 GMT  
		Size: 221.3 KB (221284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9641a8793752f42f60dcbb12e857125ba41995c02e48630112ef3f6d5747a28`  
		Last Modified: Thu, 30 Mar 2023 02:37:13 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb90b001556af3810279377523e96a71161f2dc727b628cb3d284764e5e847fd`  
		Last Modified: Thu, 30 Mar 2023 02:37:13 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.2-alpine` - linux; arm variant v6

```console
$ docker pull spiped@sha256:98e69abcdbbbc31f8223857ec6529b855f8e21be02602fe6763b73403a252650
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.6 MB (4560042 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c4871452a88018819e0282cc73c7c17274cbea4b4fd8f73619664078771460b6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 29 Mar 2023 18:01:09 GMT
ADD file:2dd294d20c0b500c8fed6b410b059429b36f51cd48a45eaf7a06ecbef9e2a3bb in / 
# Wed, 29 Mar 2023 18:01:09 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 00:22:48 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 30 Mar 2023 00:22:50 GMT
RUN apk add --no-cache libssl1.1
# Thu, 30 Mar 2023 00:22:50 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 30 Mar 2023 00:22:58 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Thu, 30 Mar 2023 00:22:58 GMT
VOLUME [/spiped]
# Thu, 30 Mar 2023 00:22:58 GMT
WORKDIR /spiped
# Thu, 30 Mar 2023 00:22:58 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 30 Mar 2023 00:22:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 30 Mar 2023 00:22:58 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:75257e753735e4ff78fae2d44018022a6ac775290e02103713a70699ece7576e`  
		Last Modified: Wed, 29 Mar 2023 18:01:52 GMT  
		Size: 3.1 MB (3110802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76f18e2ef9b0aa3ce161a88dbc21a7f6e04c161889cd2e9a48db6753f539a908`  
		Last Modified: Thu, 30 Mar 2023 00:24:29 GMT  
		Size: 1.3 KB (1267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f98080b1dde5f78f59c30b4e0ecd3d8755ce81a51335edb1f928872b6ea2758`  
		Last Modified: Thu, 30 Mar 2023 00:24:29 GMT  
		Size: 1.2 MB (1241151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2aaabfafc343e9926cb7046e859064ad3777e2fc8cddcb7e477dde08175094e7`  
		Last Modified: Thu, 30 Mar 2023 00:24:29 GMT  
		Size: 206.4 KB (206355 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e41f7588b8c91b544e8c7d054c90e59b7a9bd11c4e88918abb84a283000e0017`  
		Last Modified: Thu, 30 Mar 2023 00:24:29 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17cd529e07580d9750fa02477c2004129b10b554d974efb4047239df64df3a24`  
		Last Modified: Thu, 30 Mar 2023 00:24:29 GMT  
		Size: 338.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.2-alpine` - linux; arm variant v7

```console
$ docker pull spiped@sha256:6c2a2f1aeafd6139364938089caba1b87ad68bedb26cd1880228677d027a8a71
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4237992 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7a9eb306d4124eb8e1c6195849bb2b723860dae03a03f9bae43f0cb32e1462fd`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 29 Mar 2023 18:03:38 GMT
ADD file:959fa0ffb60c37c4fdc0d32ac31511f8dead32ef7f4bd848b11ff144a6b37012 in / 
# Wed, 29 Mar 2023 18:03:38 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 00:08:21 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 30 Mar 2023 00:08:22 GMT
RUN apk add --no-cache libssl1.1
# Thu, 30 Mar 2023 00:08:22 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 30 Mar 2023 00:08:30 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Thu, 30 Mar 2023 00:08:30 GMT
VOLUME [/spiped]
# Thu, 30 Mar 2023 00:08:30 GMT
WORKDIR /spiped
# Thu, 30 Mar 2023 00:08:30 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 30 Mar 2023 00:08:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 30 Mar 2023 00:08:31 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:fd4b2aeb476b6c2c0c3049dae919de20fe09e90deac95e3181d717055cbe6707`  
		Last Modified: Wed, 29 Mar 2023 18:06:56 GMT  
		Size: 2.9 MB (2868519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7df1c1b7ee69f0ffebff840bb383923a8a217c78132af46a52a21f12e14482c`  
		Last Modified: Sat, 08 Apr 2023 02:48:08 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e7fa369f75c521bfa073b091a994479792b5e564a5c37699be2008acad03c72`  
		Last Modified: Sat, 08 Apr 2023 02:48:09 GMT  
		Size: 1.2 MB (1167611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c21f3a95209349c9b1a3a521865cce5d3c5b7d5c8ff6ff9da5c62bb698fbf9c`  
		Last Modified: Sat, 08 Apr 2023 02:48:08 GMT  
		Size: 200.1 KB (200127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cd163e2f331db36950fd2761a2e3546fb04b46eba66cc2de8d5491d403e4be9`  
		Last Modified: Sat, 08 Apr 2023 02:48:08 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9e4936ce3183df5af3ef7fa3066376cab728047d4e40c1541aad098e3d01fb5`  
		Last Modified: Sat, 08 Apr 2023 02:48:08 GMT  
		Size: 336.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.2-alpine` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:b21f6104cf4f986ae42d2548c5a3e8edfeac1672739642c0051b1ce2e7ddc5dd
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.8 MB (4842828 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:306f5b9d541620eedadaec0c057f09c6db34da10d9378cae2f5155b0081420a9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 29 Mar 2023 17:39:18 GMT
ADD file:e51d4089e73ad6dee52b31f0c8059a00c17df6e23f6741fe11b43bd84cc99008 in / 
# Wed, 29 Mar 2023 17:39:18 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 05:50:31 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 30 Mar 2023 05:50:33 GMT
RUN apk add --no-cache libssl1.1
# Thu, 30 Mar 2023 05:50:33 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 30 Mar 2023 05:50:40 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Thu, 30 Mar 2023 05:50:40 GMT
VOLUME [/spiped]
# Thu, 30 Mar 2023 05:50:40 GMT
WORKDIR /spiped
# Thu, 30 Mar 2023 05:50:40 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 30 Mar 2023 05:50:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 30 Mar 2023 05:50:41 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:c41833b44d910632b415cd89a9cdaa4d62c9725dc56c99a7ddadafd6719960f9`  
		Last Modified: Wed, 29 Mar 2023 17:39:44 GMT  
		Size: 3.3 MB (3261854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46a75b9333a53162c1a5789a4c7973a5cc525b738e1a394e58db69d0c32fa089`  
		Last Modified: Thu, 30 Mar 2023 05:50:49 GMT  
		Size: 1.3 KB (1266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a905f71ab7e32bea70c662b413534aa7f764438f72937d84176a7b21115e19e`  
		Last Modified: Thu, 30 Mar 2023 05:50:50 GMT  
		Size: 1.4 MB (1363548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8364c9ed77705e5bab6f7d3ebcefe334f2401e4822779b17ceb1bb94d7510ce7`  
		Last Modified: Thu, 30 Mar 2023 05:50:50 GMT  
		Size: 215.7 KB (215692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d28a0bb75b3c36c6b1f0df28be9d91f3073dfcc4b0701cd2dffcafc2d8834c55`  
		Last Modified: Thu, 30 Mar 2023 05:50:49 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed9fdfb5809799657c2cc38eac53edd7e1105371601d7e1c155b00bf07f8f3d0`  
		Last Modified: Thu, 30 Mar 2023 05:50:49 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.2-alpine` - linux; 386

```console
$ docker pull spiped@sha256:0e5f49d56599b01f5aa0c4d6ebedb8fe9e52f5d2a66e094700b5f7703cc3f26e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.1 MB (5132057 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9fa9e52e3f82d57652b3398c82d896ea0c351c189b78a1daa85740fc04413b4d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 29 Mar 2023 17:38:30 GMT
ADD file:61bc44c9685b610d18bddd05d2ea1e57b4313f5f433a0a0b7e5269ec24f108b0 in / 
# Wed, 29 Mar 2023 17:38:30 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 01:33:08 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 30 Mar 2023 01:33:10 GMT
RUN apk add --no-cache libssl1.1
# Thu, 30 Mar 2023 01:33:10 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 30 Mar 2023 01:33:22 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Thu, 30 Mar 2023 01:33:22 GMT
VOLUME [/spiped]
# Thu, 30 Mar 2023 01:33:22 GMT
WORKDIR /spiped
# Thu, 30 Mar 2023 01:33:22 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 30 Mar 2023 01:33:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 30 Mar 2023 01:33:22 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:b2b0f0faedf1b87a3c77cf90d027fb7a25aa67f35400244a4655ad5842a757e4`  
		Last Modified: Wed, 29 Mar 2023 17:39:00 GMT  
		Size: 3.4 MB (3412260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09a513a8526f3d62fd7ec1e80a76b26d4cf8c8c37ea534b10e2c0060eb3cb6f0`  
		Last Modified: Thu, 30 Mar 2023 01:33:31 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa7fa7db70396ccd0f7c43ec98f7831c11a443d8d0f9ae5383bd39a0256cd39d`  
		Last Modified: Thu, 30 Mar 2023 01:33:32 GMT  
		Size: 1.5 MB (1486443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1d342e0d74297744901c335be2694a48a287375cc57389ee49fc329b6093f5a`  
		Last Modified: Thu, 30 Mar 2023 01:33:31 GMT  
		Size: 231.6 KB (231615 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1dc5bf7a2360503d1b51116e389e689406594d6295129a36524b8e4f7bad02d7`  
		Last Modified: Thu, 30 Mar 2023 01:33:31 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eae5cb4f4de570095d623ebcde4ca7cf3062c366c24ad3595d5108c7111c29af`  
		Last Modified: Thu, 30 Mar 2023 01:33:31 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.2-alpine` - linux; ppc64le

```console
$ docker pull spiped@sha256:8b13ec4b458ac31fb096b22da921ddc5f982ca84907ae2ad42dfc9935e69a793
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.0 MB (5025754 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:70983caa08c37ccc9d7968473ced65e5b8ee6cc50feff3049de378aee313e62f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 29 Mar 2023 18:16:27 GMT
ADD file:e95c1f256ba4bda85c5cbc0d8e84e6f329aa17c9dd2715b2da043e2139049124 in / 
# Wed, 29 Mar 2023 18:16:28 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 04:32:24 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 30 Mar 2023 04:32:26 GMT
RUN apk add --no-cache libssl1.1
# Thu, 30 Mar 2023 04:32:26 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 30 Mar 2023 04:32:41 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Thu, 30 Mar 2023 04:32:42 GMT
VOLUME [/spiped]
# Thu, 30 Mar 2023 04:32:43 GMT
WORKDIR /spiped
# Thu, 30 Mar 2023 04:32:43 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 30 Mar 2023 04:32:43 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 30 Mar 2023 04:32:44 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:1b7d25764eb3d3c55d73f5dfb9e3e9d75f3f39132e1b16142319de2a062dd673`  
		Last Modified: Wed, 29 Mar 2023 18:17:14 GMT  
		Size: 3.4 MB (3390935 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6abd914c752b02f6f79b7ef1571ed87d4130a25ed21a1d3892a23e3c2c1cfbec`  
		Last Modified: Thu, 30 Mar 2023 04:32:57 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3cc8ae50d4833e170ee7dc2db705d37cc39c4e228e121c72a14cd9620b4847c`  
		Last Modified: Thu, 30 Mar 2023 04:32:57 GMT  
		Size: 1.4 MB (1413051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac183c495785747e187a666506a1c63aeb182e3c511beaa79f82f4c86278a170`  
		Last Modified: Thu, 30 Mar 2023 04:32:57 GMT  
		Size: 220.0 KB (220030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8a70723c954d9ac5e16090c8b3aa6668bfab3384b6ce30cab8e10925bd1cd6c`  
		Last Modified: Thu, 30 Mar 2023 04:32:57 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85a4bf70a1b07cf55ae9e8498ca917bc7a43613629d823f0e1fa9b6c689b47b7`  
		Last Modified: Thu, 30 Mar 2023 04:32:57 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.2-alpine` - linux; s390x

```console
$ docker pull spiped@sha256:604fdf074de91d3fb86a39f54c9e130aeae2855ef71419e51d46b3fdbf10d3de
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.6 MB (4608998 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b8a0724e4059c76aefa5294b08af1999e786b6c97b94942a93375b39f74ec82a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 29 Mar 2023 17:41:57 GMT
ADD file:675ad8acf4b076e34aeeba26dd482be7640df5912b1ec5e3183b7eb69c01e83e in / 
# Wed, 29 Mar 2023 17:41:57 GMT
CMD ["/bin/sh"]
# Wed, 29 Mar 2023 22:37:24 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Wed, 29 Mar 2023 22:37:25 GMT
RUN apk add --no-cache libssl1.1
# Wed, 29 Mar 2023 22:37:25 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 29 Mar 2023 22:37:31 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Wed, 29 Mar 2023 22:37:31 GMT
VOLUME [/spiped]
# Wed, 29 Mar 2023 22:37:31 GMT
WORKDIR /spiped
# Wed, 29 Mar 2023 22:37:32 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 29 Mar 2023 22:37:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 29 Mar 2023 22:37:32 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:a76f78d8854217635d8049ec8501edb806f961e72989cfff8503982e6ff2579d`  
		Last Modified: Wed, 29 Mar 2023 17:42:31 GMT  
		Size: 3.2 MB (3175187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d252736c81578b3badb86bd65e11e8c42a3eced9b84da155c5d277746787398`  
		Last Modified: Wed, 29 Mar 2023 22:37:46 GMT  
		Size: 1.3 KB (1272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc4b9cdd39312641949e882585794aca9deab09fa611f8acf8a7b6c157519893`  
		Last Modified: Wed, 29 Mar 2023 22:37:46 GMT  
		Size: 1.2 MB (1223431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1da4a09ddda6c10edd737c5f0240c12ce3c655fe0cf8717062fdf0ab72f20285`  
		Last Modified: Wed, 29 Mar 2023 22:37:46 GMT  
		Size: 208.6 KB (208640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e3df4963fb4aa70acb7774a679b92580dffeb32ff4899e3ec8919a9feff0338`  
		Last Modified: Wed, 29 Mar 2023 22:37:46 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6af10966e7af681719def4af18b191e9fbdc7723fbc3c8f645089965679fe6c7`  
		Last Modified: Wed, 29 Mar 2023 22:37:46 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:alpine`

```console
$ docker pull spiped@sha256:657bd49b462533d254e7d5b3216fde01bc59a24c4f6277b050ae5bdc8f548a87
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
$ docker pull spiped@sha256:7b7f7844dc68c4b9728d9185d906025f7565df88ca9612aaaf420ac91523f405
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.1 MB (5080949 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2b60c5b50be16ba58852d923ea4e7d5224aecb355eb4588ab08b2f70c72ad851`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 29 Mar 2023 18:19:24 GMT
ADD file:9a4f77dfaba7fd2aa78186e4ef0e7486ad55101cefc1fabbc1b385601bb38920 in / 
# Wed, 29 Mar 2023 18:19:24 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 02:36:50 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 30 Mar 2023 02:36:51 GMT
RUN apk add --no-cache libssl1.1
# Thu, 30 Mar 2023 02:36:51 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 30 Mar 2023 02:37:01 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Thu, 30 Mar 2023 02:37:01 GMT
VOLUME [/spiped]
# Thu, 30 Mar 2023 02:37:02 GMT
WORKDIR /spiped
# Thu, 30 Mar 2023 02:37:02 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 30 Mar 2023 02:37:02 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 30 Mar 2023 02:37:02 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:f56be85fc22e46face30e2c3de3f7fe7c15f8fd7c4e5add29d7f64b87abdaa09`  
		Last Modified: Wed, 29 Mar 2023 18:19:57 GMT  
		Size: 3.4 MB (3374563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:833c4ea98211ab2b826b6d62f250a61b8c5ae407b5de38776cc5bc31d895d3fa`  
		Last Modified: Thu, 30 Mar 2023 02:37:13 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:870359eb3ab308a11eaf9cfc6782cd2bea0c513f3920492180bd5f5cbbea54eb`  
		Last Modified: Thu, 30 Mar 2023 02:37:13 GMT  
		Size: 1.5 MB (1483362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4afeb4ec06ad120774f5e7a75610323bda25b84d5957c8bac3f5c90ea7fdd17`  
		Last Modified: Thu, 30 Mar 2023 02:37:13 GMT  
		Size: 221.3 KB (221284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9641a8793752f42f60dcbb12e857125ba41995c02e48630112ef3f6d5747a28`  
		Last Modified: Thu, 30 Mar 2023 02:37:13 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb90b001556af3810279377523e96a71161f2dc727b628cb3d284764e5e847fd`  
		Last Modified: Thu, 30 Mar 2023 02:37:13 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; arm variant v6

```console
$ docker pull spiped@sha256:98e69abcdbbbc31f8223857ec6529b855f8e21be02602fe6763b73403a252650
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.6 MB (4560042 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c4871452a88018819e0282cc73c7c17274cbea4b4fd8f73619664078771460b6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 29 Mar 2023 18:01:09 GMT
ADD file:2dd294d20c0b500c8fed6b410b059429b36f51cd48a45eaf7a06ecbef9e2a3bb in / 
# Wed, 29 Mar 2023 18:01:09 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 00:22:48 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 30 Mar 2023 00:22:50 GMT
RUN apk add --no-cache libssl1.1
# Thu, 30 Mar 2023 00:22:50 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 30 Mar 2023 00:22:58 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Thu, 30 Mar 2023 00:22:58 GMT
VOLUME [/spiped]
# Thu, 30 Mar 2023 00:22:58 GMT
WORKDIR /spiped
# Thu, 30 Mar 2023 00:22:58 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 30 Mar 2023 00:22:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 30 Mar 2023 00:22:58 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:75257e753735e4ff78fae2d44018022a6ac775290e02103713a70699ece7576e`  
		Last Modified: Wed, 29 Mar 2023 18:01:52 GMT  
		Size: 3.1 MB (3110802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76f18e2ef9b0aa3ce161a88dbc21a7f6e04c161889cd2e9a48db6753f539a908`  
		Last Modified: Thu, 30 Mar 2023 00:24:29 GMT  
		Size: 1.3 KB (1267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f98080b1dde5f78f59c30b4e0ecd3d8755ce81a51335edb1f928872b6ea2758`  
		Last Modified: Thu, 30 Mar 2023 00:24:29 GMT  
		Size: 1.2 MB (1241151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2aaabfafc343e9926cb7046e859064ad3777e2fc8cddcb7e477dde08175094e7`  
		Last Modified: Thu, 30 Mar 2023 00:24:29 GMT  
		Size: 206.4 KB (206355 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e41f7588b8c91b544e8c7d054c90e59b7a9bd11c4e88918abb84a283000e0017`  
		Last Modified: Thu, 30 Mar 2023 00:24:29 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17cd529e07580d9750fa02477c2004129b10b554d974efb4047239df64df3a24`  
		Last Modified: Thu, 30 Mar 2023 00:24:29 GMT  
		Size: 338.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; arm variant v7

```console
$ docker pull spiped@sha256:6c2a2f1aeafd6139364938089caba1b87ad68bedb26cd1880228677d027a8a71
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4237992 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7a9eb306d4124eb8e1c6195849bb2b723860dae03a03f9bae43f0cb32e1462fd`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 29 Mar 2023 18:03:38 GMT
ADD file:959fa0ffb60c37c4fdc0d32ac31511f8dead32ef7f4bd848b11ff144a6b37012 in / 
# Wed, 29 Mar 2023 18:03:38 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 00:08:21 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 30 Mar 2023 00:08:22 GMT
RUN apk add --no-cache libssl1.1
# Thu, 30 Mar 2023 00:08:22 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 30 Mar 2023 00:08:30 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Thu, 30 Mar 2023 00:08:30 GMT
VOLUME [/spiped]
# Thu, 30 Mar 2023 00:08:30 GMT
WORKDIR /spiped
# Thu, 30 Mar 2023 00:08:30 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 30 Mar 2023 00:08:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 30 Mar 2023 00:08:31 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:fd4b2aeb476b6c2c0c3049dae919de20fe09e90deac95e3181d717055cbe6707`  
		Last Modified: Wed, 29 Mar 2023 18:06:56 GMT  
		Size: 2.9 MB (2868519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7df1c1b7ee69f0ffebff840bb383923a8a217c78132af46a52a21f12e14482c`  
		Last Modified: Sat, 08 Apr 2023 02:48:08 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e7fa369f75c521bfa073b091a994479792b5e564a5c37699be2008acad03c72`  
		Last Modified: Sat, 08 Apr 2023 02:48:09 GMT  
		Size: 1.2 MB (1167611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c21f3a95209349c9b1a3a521865cce5d3c5b7d5c8ff6ff9da5c62bb698fbf9c`  
		Last Modified: Sat, 08 Apr 2023 02:48:08 GMT  
		Size: 200.1 KB (200127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cd163e2f331db36950fd2761a2e3546fb04b46eba66cc2de8d5491d403e4be9`  
		Last Modified: Sat, 08 Apr 2023 02:48:08 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9e4936ce3183df5af3ef7fa3066376cab728047d4e40c1541aad098e3d01fb5`  
		Last Modified: Sat, 08 Apr 2023 02:48:08 GMT  
		Size: 336.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:b21f6104cf4f986ae42d2548c5a3e8edfeac1672739642c0051b1ce2e7ddc5dd
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.8 MB (4842828 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:306f5b9d541620eedadaec0c057f09c6db34da10d9378cae2f5155b0081420a9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 29 Mar 2023 17:39:18 GMT
ADD file:e51d4089e73ad6dee52b31f0c8059a00c17df6e23f6741fe11b43bd84cc99008 in / 
# Wed, 29 Mar 2023 17:39:18 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 05:50:31 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 30 Mar 2023 05:50:33 GMT
RUN apk add --no-cache libssl1.1
# Thu, 30 Mar 2023 05:50:33 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 30 Mar 2023 05:50:40 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Thu, 30 Mar 2023 05:50:40 GMT
VOLUME [/spiped]
# Thu, 30 Mar 2023 05:50:40 GMT
WORKDIR /spiped
# Thu, 30 Mar 2023 05:50:40 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 30 Mar 2023 05:50:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 30 Mar 2023 05:50:41 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:c41833b44d910632b415cd89a9cdaa4d62c9725dc56c99a7ddadafd6719960f9`  
		Last Modified: Wed, 29 Mar 2023 17:39:44 GMT  
		Size: 3.3 MB (3261854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46a75b9333a53162c1a5789a4c7973a5cc525b738e1a394e58db69d0c32fa089`  
		Last Modified: Thu, 30 Mar 2023 05:50:49 GMT  
		Size: 1.3 KB (1266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a905f71ab7e32bea70c662b413534aa7f764438f72937d84176a7b21115e19e`  
		Last Modified: Thu, 30 Mar 2023 05:50:50 GMT  
		Size: 1.4 MB (1363548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8364c9ed77705e5bab6f7d3ebcefe334f2401e4822779b17ceb1bb94d7510ce7`  
		Last Modified: Thu, 30 Mar 2023 05:50:50 GMT  
		Size: 215.7 KB (215692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d28a0bb75b3c36c6b1f0df28be9d91f3073dfcc4b0701cd2dffcafc2d8834c55`  
		Last Modified: Thu, 30 Mar 2023 05:50:49 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed9fdfb5809799657c2cc38eac53edd7e1105371601d7e1c155b00bf07f8f3d0`  
		Last Modified: Thu, 30 Mar 2023 05:50:49 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; 386

```console
$ docker pull spiped@sha256:0e5f49d56599b01f5aa0c4d6ebedb8fe9e52f5d2a66e094700b5f7703cc3f26e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.1 MB (5132057 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9fa9e52e3f82d57652b3398c82d896ea0c351c189b78a1daa85740fc04413b4d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 29 Mar 2023 17:38:30 GMT
ADD file:61bc44c9685b610d18bddd05d2ea1e57b4313f5f433a0a0b7e5269ec24f108b0 in / 
# Wed, 29 Mar 2023 17:38:30 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 01:33:08 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 30 Mar 2023 01:33:10 GMT
RUN apk add --no-cache libssl1.1
# Thu, 30 Mar 2023 01:33:10 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 30 Mar 2023 01:33:22 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Thu, 30 Mar 2023 01:33:22 GMT
VOLUME [/spiped]
# Thu, 30 Mar 2023 01:33:22 GMT
WORKDIR /spiped
# Thu, 30 Mar 2023 01:33:22 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 30 Mar 2023 01:33:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 30 Mar 2023 01:33:22 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:b2b0f0faedf1b87a3c77cf90d027fb7a25aa67f35400244a4655ad5842a757e4`  
		Last Modified: Wed, 29 Mar 2023 17:39:00 GMT  
		Size: 3.4 MB (3412260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09a513a8526f3d62fd7ec1e80a76b26d4cf8c8c37ea534b10e2c0060eb3cb6f0`  
		Last Modified: Thu, 30 Mar 2023 01:33:31 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa7fa7db70396ccd0f7c43ec98f7831c11a443d8d0f9ae5383bd39a0256cd39d`  
		Last Modified: Thu, 30 Mar 2023 01:33:32 GMT  
		Size: 1.5 MB (1486443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1d342e0d74297744901c335be2694a48a287375cc57389ee49fc329b6093f5a`  
		Last Modified: Thu, 30 Mar 2023 01:33:31 GMT  
		Size: 231.6 KB (231615 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1dc5bf7a2360503d1b51116e389e689406594d6295129a36524b8e4f7bad02d7`  
		Last Modified: Thu, 30 Mar 2023 01:33:31 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eae5cb4f4de570095d623ebcde4ca7cf3062c366c24ad3595d5108c7111c29af`  
		Last Modified: Thu, 30 Mar 2023 01:33:31 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; ppc64le

```console
$ docker pull spiped@sha256:8b13ec4b458ac31fb096b22da921ddc5f982ca84907ae2ad42dfc9935e69a793
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.0 MB (5025754 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:70983caa08c37ccc9d7968473ced65e5b8ee6cc50feff3049de378aee313e62f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 29 Mar 2023 18:16:27 GMT
ADD file:e95c1f256ba4bda85c5cbc0d8e84e6f329aa17c9dd2715b2da043e2139049124 in / 
# Wed, 29 Mar 2023 18:16:28 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 04:32:24 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Thu, 30 Mar 2023 04:32:26 GMT
RUN apk add --no-cache libssl1.1
# Thu, 30 Mar 2023 04:32:26 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 30 Mar 2023 04:32:41 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Thu, 30 Mar 2023 04:32:42 GMT
VOLUME [/spiped]
# Thu, 30 Mar 2023 04:32:43 GMT
WORKDIR /spiped
# Thu, 30 Mar 2023 04:32:43 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 30 Mar 2023 04:32:43 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 30 Mar 2023 04:32:44 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:1b7d25764eb3d3c55d73f5dfb9e3e9d75f3f39132e1b16142319de2a062dd673`  
		Last Modified: Wed, 29 Mar 2023 18:17:14 GMT  
		Size: 3.4 MB (3390935 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6abd914c752b02f6f79b7ef1571ed87d4130a25ed21a1d3892a23e3c2c1cfbec`  
		Last Modified: Thu, 30 Mar 2023 04:32:57 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3cc8ae50d4833e170ee7dc2db705d37cc39c4e228e121c72a14cd9620b4847c`  
		Last Modified: Thu, 30 Mar 2023 04:32:57 GMT  
		Size: 1.4 MB (1413051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac183c495785747e187a666506a1c63aeb182e3c511beaa79f82f4c86278a170`  
		Last Modified: Thu, 30 Mar 2023 04:32:57 GMT  
		Size: 220.0 KB (220030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8a70723c954d9ac5e16090c8b3aa6668bfab3384b6ce30cab8e10925bd1cd6c`  
		Last Modified: Thu, 30 Mar 2023 04:32:57 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85a4bf70a1b07cf55ae9e8498ca917bc7a43613629d823f0e1fa9b6c689b47b7`  
		Last Modified: Thu, 30 Mar 2023 04:32:57 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; s390x

```console
$ docker pull spiped@sha256:604fdf074de91d3fb86a39f54c9e130aeae2855ef71419e51d46b3fdbf10d3de
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.6 MB (4608998 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b8a0724e4059c76aefa5294b08af1999e786b6c97b94942a93375b39f74ec82a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 29 Mar 2023 17:41:57 GMT
ADD file:675ad8acf4b076e34aeeba26dd482be7640df5912b1ec5e3183b7eb69c01e83e in / 
# Wed, 29 Mar 2023 17:41:57 GMT
CMD ["/bin/sh"]
# Wed, 29 Mar 2023 22:37:24 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Wed, 29 Mar 2023 22:37:25 GMT
RUN apk add --no-cache libssl1.1
# Wed, 29 Mar 2023 22:37:25 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 29 Mar 2023 22:37:31 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Wed, 29 Mar 2023 22:37:31 GMT
VOLUME [/spiped]
# Wed, 29 Mar 2023 22:37:31 GMT
WORKDIR /spiped
# Wed, 29 Mar 2023 22:37:32 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 29 Mar 2023 22:37:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 29 Mar 2023 22:37:32 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:a76f78d8854217635d8049ec8501edb806f961e72989cfff8503982e6ff2579d`  
		Last Modified: Wed, 29 Mar 2023 17:42:31 GMT  
		Size: 3.2 MB (3175187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d252736c81578b3badb86bd65e11e8c42a3eced9b84da155c5d277746787398`  
		Last Modified: Wed, 29 Mar 2023 22:37:46 GMT  
		Size: 1.3 KB (1272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc4b9cdd39312641949e882585794aca9deab09fa611f8acf8a7b6c157519893`  
		Last Modified: Wed, 29 Mar 2023 22:37:46 GMT  
		Size: 1.2 MB (1223431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1da4a09ddda6c10edd737c5f0240c12ce3c655fe0cf8717062fdf0ab72f20285`  
		Last Modified: Wed, 29 Mar 2023 22:37:46 GMT  
		Size: 208.6 KB (208640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e3df4963fb4aa70acb7774a679b92580dffeb32ff4899e3ec8919a9feff0338`  
		Last Modified: Wed, 29 Mar 2023 22:37:46 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6af10966e7af681719def4af18b191e9fbdc7723fbc3c8f645089965679fe6c7`  
		Last Modified: Wed, 29 Mar 2023 22:37:46 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:latest`

```console
$ docker pull spiped@sha256:3803fdc1e42df38ec09699a69d983e0c24277804803d456099a8989cefe72ace
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
$ docker pull spiped@sha256:721c9e3ecb57ab885c003700665c787207861ed892989be757c330a07a4c697c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.4 MB (37412915 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:be5ba0f72c5d2a07deab8c81f022c0d0da6de183e5be45bf75e5d2a765ce1241`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 23 Mar 2023 01:30:27 GMT
ADD file:60911afdacfdc216e44115addb5f3cc07f4166e8a4adf7be94a58aacc327ad63 in / 
# Thu, 23 Mar 2023 01:30:27 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 14:21:59 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Thu, 23 Mar 2023 14:22:02 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 14:22:03 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 23 Mar 2023 14:22:22 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 23 Mar 2023 14:22:22 GMT
VOLUME [/spiped]
# Thu, 23 Mar 2023 14:22:22 GMT
WORKDIR /spiped
# Thu, 23 Mar 2023 14:22:22 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 23 Mar 2023 14:22:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Mar 2023 14:22:22 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:f1f26f5702560b7e591bef5c4d840f76a232bf13fd5aefc4e22077a1ae4440c7`  
		Last Modified: Thu, 23 Mar 2023 01:34:23 GMT  
		Size: 31.4 MB (31411405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eba658cb120bd99022c7cf87e1a7e097de79f5861fc1b445ecbae4edeec1dfe4`  
		Last Modified: Thu, 23 Mar 2023 14:22:35 GMT  
		Size: 1.7 KB (1734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa69edd47542d8a3cf149d1bb36059f8c0e848ad433b8c659de5c1155781e12e`  
		Last Modified: Thu, 23 Mar 2023 14:22:35 GMT  
		Size: 1.1 KB (1050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:187bd75bf46234bc1609024e05712a659839202cc73b40db694672a1aff8b2c6`  
		Last Modified: Thu, 23 Mar 2023 14:22:36 GMT  
		Size: 6.0 MB (5998257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b9f50c988f7a169cc12e6566f824e86960bc77d0e2714a2ff2ddb919bec84f4`  
		Last Modified: Thu, 23 Mar 2023 14:22:35 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:866a419d38e59257252937a0d01999799ffb71213ebab6f7c0ba412832f7fbbe`  
		Last Modified: Thu, 23 Mar 2023 14:22:35 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; arm variant v5

```console
$ docker pull spiped@sha256:c56ad02f7a635dc4d379610e1a1095f9c487573ef61de595cba27525df82e0f0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.0 MB (33951316 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3289615005289139cb049ad1aaeaa83f924744ae842e267446c978996e7f8843`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 12 Apr 2023 00:48:41 GMT
ADD file:11004b5308adcb1c41526eac7071d373a5c42ca2e457a2e9e8b3a9d621c4e8e1 in / 
# Wed, 12 Apr 2023 00:48:41 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 04:13:45 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 12 Apr 2023 04:13:49 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 04:13:49 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 12 Apr 2023 04:14:09 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 12 Apr 2023 04:14:10 GMT
VOLUME [/spiped]
# Wed, 12 Apr 2023 04:14:10 GMT
WORKDIR /spiped
# Wed, 12 Apr 2023 04:14:10 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 12 Apr 2023 04:14:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 12 Apr 2023 04:14:10 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:5303309ebdb5d711447ed8a4ea072653ca7445c193060ec0aea30a89e92cda7e`  
		Last Modified: Wed, 12 Apr 2023 00:51:08 GMT  
		Size: 28.9 MB (28919551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c6d1cdee0b3069d6a9bbf71705b647047aa3718658646508ea3895abc295acd`  
		Last Modified: Wed, 12 Apr 2023 04:14:22 GMT  
		Size: 1.7 KB (1726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:413f2bdfff2530854dc8be54292587aacb28c20e08fbec5a75cd1c650b3ca0c6`  
		Last Modified: Wed, 12 Apr 2023 04:14:22 GMT  
		Size: 1.1 KB (1051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a772c2e19b2b59b3653449c3d87f10b14cad2ada0f4da89454a5d4216fb591c`  
		Last Modified: Wed, 12 Apr 2023 04:14:23 GMT  
		Size: 5.0 MB (5028515 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c462f1e36902eb29b25d02f2e17f167c04a3e4f838a3a5ab2227124fded03fb`  
		Last Modified: Wed, 12 Apr 2023 04:14:22 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edfdf45255e0c1a8dcac1dd2d2e36c424b51561ba09b234321f4589bcdab730d`  
		Last Modified: Wed, 12 Apr 2023 04:14:22 GMT  
		Size: 344.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; arm variant v7

```console
$ docker pull spiped@sha256:cf39f3bb40dcde6b5bf8478c9adb7d2539f890a17b9c12197f7ae968a28420f6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.3 MB (31329618 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1767501b8e0bc0f4d13978feac2b18de6af1c59fc29879fb0d1c08f1f85fcf84`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 23 Mar 2023 01:16:59 GMT
ADD file:1c83b99ee21091150a1c9ee8ef7c40bec3d6cb0d64b8bc0ef40fb97e6233aa5b in / 
# Thu, 23 Mar 2023 01:17:00 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 12:26:37 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Thu, 23 Mar 2023 12:26:40 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 12:26:40 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 23 Mar 2023 12:26:56 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 23 Mar 2023 12:26:56 GMT
VOLUME [/spiped]
# Thu, 23 Mar 2023 12:26:56 GMT
WORKDIR /spiped
# Thu, 23 Mar 2023 12:26:56 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 23 Mar 2023 12:26:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Mar 2023 12:26:56 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:2bc24e24d213c286ca4011c8b5cb7a3cf2a51f3bbedee8eeced46382bb5507bc`  
		Last Modified: Thu, 23 Mar 2023 01:33:18 GMT  
		Size: 26.6 MB (26577330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19061e17258a1ab423b9751a507a87e3c84da5eaffe1923ad2abc7aa5bf00be5`  
		Last Modified: Thu, 23 Mar 2023 12:27:07 GMT  
		Size: 1.7 KB (1727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0722d57fbb2b9577a072039b5f829c50b186b9d21b626777d773449488488fdc`  
		Last Modified: Thu, 23 Mar 2023 12:27:07 GMT  
		Size: 1.1 KB (1052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45c6b3401d253fee03596d2a401a84ebd8e4a340950690b66204e12a04889674`  
		Last Modified: Thu, 23 Mar 2023 12:27:08 GMT  
		Size: 4.7 MB (4749039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b000b28b92c3a6f78c372224d409ad90c989e6f0a43e4d9b72ae8ad4ccd28734`  
		Last Modified: Thu, 23 Mar 2023 12:27:07 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c563d03992865638f6480cdb6704eb9b8204b1c402024e2a101a161ede86290`  
		Last Modified: Thu, 23 Mar 2023 12:27:07 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:59a7ac95f3c86cfcda52266517687440ee833af0cfcd7bac7560d43faa690d52
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.3 MB (35339898 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:48134ae14be7815e330e696d68f5ce9f78018354a0b2aeef3cf707a462d57153`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 12 Apr 2023 00:39:49 GMT
ADD file:7b3c55926db26568f849247e80abdec3cfd6642929a40f0bbee95e4cb176051e in / 
# Wed, 12 Apr 2023 00:39:49 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 05:09:45 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 12 Apr 2023 05:09:48 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 05:09:48 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 12 Apr 2023 05:10:03 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 12 Apr 2023 05:10:03 GMT
VOLUME [/spiped]
# Wed, 12 Apr 2023 05:10:03 GMT
WORKDIR /spiped
# Wed, 12 Apr 2023 05:10:03 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 12 Apr 2023 05:10:03 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 12 Apr 2023 05:10:03 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:ebc3dc5a2d72427c585c8cda7574a75d96e04b9a37572bd3af0bff905abefbb9`  
		Last Modified: Wed, 12 Apr 2023 00:42:35 GMT  
		Size: 30.1 MB (30063826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3875f32a5967d63af0264c7e837f0ec1af397174340c608406c8dc1c4efd6d0`  
		Last Modified: Wed, 12 Apr 2023 05:10:15 GMT  
		Size: 1.7 KB (1734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d3c045802f338371900f62902ca0526fcbe0f103f1782134df45d785ec50a3b`  
		Last Modified: Wed, 12 Apr 2023 05:10:15 GMT  
		Size: 1.1 KB (1052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2cf02c8c59a3d5dfbb72551bda146e124e152fc03ddae5703249f6dfce3a7db`  
		Last Modified: Wed, 12 Apr 2023 05:10:16 GMT  
		Size: 5.3 MB (5272817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eafbdd4f6fdf5ed1c3903c9d26f47af77dcbde36fd86079557354b0153d0fd7b`  
		Last Modified: Wed, 12 Apr 2023 05:10:15 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9422d8f8fafc31168cc5eaebe935dfc7fde33c3e800595ec728d2d9fe52717fc`  
		Last Modified: Wed, 12 Apr 2023 05:10:16 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; 386

```console
$ docker pull spiped@sha256:74d7f5c8f3f3d9c67ac2694a397c85180e9414b6092e41e394b39054f2029c92
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.3 MB (40291472 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cd42d521cfced48016618daf00f5e6976442656bf9c4005a7c8200ef734bcbd4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 23 Mar 2023 00:39:18 GMT
ADD file:315d843eefd4a8bb2345366dcd6bab00a06fca4a7970e220ae8946123d07d7ed in / 
# Thu, 23 Mar 2023 00:39:19 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 12:10:30 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Thu, 23 Mar 2023 12:10:33 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 12:10:33 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 23 Mar 2023 12:10:56 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 23 Mar 2023 12:10:56 GMT
VOLUME [/spiped]
# Thu, 23 Mar 2023 12:10:56 GMT
WORKDIR /spiped
# Thu, 23 Mar 2023 12:10:56 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 23 Mar 2023 12:10:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Mar 2023 12:10:57 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:3e638a975ea99fe8646002726dcb1ccdccc49ad33967b30337b9b2413e0619b5`  
		Last Modified: Thu, 23 Mar 2023 00:43:09 GMT  
		Size: 32.4 MB (32396277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8c70cbb4c8fd8326cfa3a38bcadaebdcf624fcd76381d57288eb687694073d1`  
		Last Modified: Thu, 23 Mar 2023 12:11:11 GMT  
		Size: 1.7 KB (1725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b85e36913d82a6dadb0781c7ab440ef652976cc8995f5f0a0bd0541b9b620373`  
		Last Modified: Thu, 23 Mar 2023 12:11:11 GMT  
		Size: 1.1 KB (1054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bec8a50af228e59f346840b516f8f52a3b22b0be6d31a71d1341b272cc16d2ad`  
		Last Modified: Thu, 23 Mar 2023 12:11:13 GMT  
		Size: 7.9 MB (7891948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af275a5a028f320d08a155a1238d5121d8a0198cebf123d479cfab9a01aafd10`  
		Last Modified: Thu, 23 Mar 2023 12:11:11 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:409fcb43c7b4c77abd48e9757bd49eadd9c1aade55294cd9145e4f451a2a7a75`  
		Last Modified: Thu, 23 Mar 2023 12:11:11 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; mips64le

```console
$ docker pull spiped@sha256:62230d57630eb194945dc5756f3ee3712d046b75a1dd34bf2492a6418d46c0c5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.3 MB (35342788 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8418f829109d61f98060ab82e69f86501a87342a4f87913c3caeeb250c189e00`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 23 Mar 2023 05:17:57 GMT
ADD file:fd3a8eec4ae8f6058f522536ca9af1b391f3032504c085d8ddb6f4878ca478d5 in / 
# Thu, 23 Mar 2023 05:18:02 GMT
CMD ["bash"]
# Fri, 24 Mar 2023 05:00:18 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Fri, 24 Mar 2023 05:00:32 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Fri, 24 Mar 2023 05:00:34 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Fri, 24 Mar 2023 05:02:12 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Fri, 24 Mar 2023 05:02:15 GMT
VOLUME [/spiped]
# Fri, 24 Mar 2023 05:02:18 GMT
WORKDIR /spiped
# Fri, 24 Mar 2023 05:02:20 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Fri, 24 Mar 2023 05:02:23 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Mar 2023 05:02:25 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:735f9e60414e17ec59baef702f7013b7327899801df2ecf10123ce2727d8dea5`  
		Last Modified: Thu, 23 Mar 2023 05:25:53 GMT  
		Size: 29.6 MB (29634483 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9a95c8da754e637392a1172bcb5e591bcfcee63c2487be6f26b2c7489db5a7a`  
		Last Modified: Fri, 24 Mar 2023 05:02:46 GMT  
		Size: 1.6 KB (1622 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd933d8bf0d5ecf038fba2d2a35b694d9bf219c863351085755e909ab6c35b68`  
		Last Modified: Fri, 24 Mar 2023 05:02:46 GMT  
		Size: 926.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5db34c43bd622971b73a1d85c07581e353bf4e2ea607f6d6fcccd6a01f4fe2af`  
		Last Modified: Fri, 24 Mar 2023 05:02:51 GMT  
		Size: 5.7 MB (5705322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:476c1e9034825a9660cd4864a260cd15699063d1ed614ca97343aa9e139f1a36`  
		Last Modified: Fri, 24 Mar 2023 05:02:46 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ce2516d3dc94f7447fdff0b2538709c3ea3641cea323cd4d781e63909477f18`  
		Last Modified: Fri, 24 Mar 2023 05:02:46 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; ppc64le

```console
$ docker pull spiped@sha256:f401ab547830f955399b7c0c1037926954410f08e2308f97b2f1e114bf6c259b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.3 MB (41290962 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e8453ca71665e6fc2f4410696c68b7f0e85ba0d198b69afe7a94b47804fa1b94`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 23 Mar 2023 01:19:48 GMT
ADD file:fbd36b7667327dd30171fc49b8e028b8371fdbc7d30ee673808d508557f78bf1 in / 
# Thu, 23 Mar 2023 01:19:49 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 16:21:57 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Thu, 23 Mar 2023 16:22:03 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 16:22:03 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 23 Mar 2023 16:22:48 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 23 Mar 2023 16:22:49 GMT
VOLUME [/spiped]
# Thu, 23 Mar 2023 16:22:49 GMT
WORKDIR /spiped
# Thu, 23 Mar 2023 16:22:49 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 23 Mar 2023 16:22:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Mar 2023 16:22:50 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:8f472ad0a3fa58b4e304d1a974f25615d5bd3b7a99dff9c8202bd30facef0155`  
		Last Modified: Thu, 23 Mar 2023 01:24:22 GMT  
		Size: 35.3 MB (35288050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4167de1b2f5e0621dc4ea93047f68b495e3ff1d47ad708aeb47dacc4d98e4d6a`  
		Last Modified: Thu, 23 Mar 2023 16:23:05 GMT  
		Size: 1.7 KB (1732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:268241dc91792d1ad06458566222f09588696272408743915b59f8f440290b1c`  
		Last Modified: Thu, 23 Mar 2023 16:23:05 GMT  
		Size: 1.1 KB (1054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8dae255202559b344f349ed2396795c7dbc31726de4c1f57564193a10a4737e`  
		Last Modified: Thu, 23 Mar 2023 16:23:07 GMT  
		Size: 6.0 MB (5999654 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:047050eb0511c54c1aed11a944fdd94382d4abf66190b183f205e829e05e92b3`  
		Last Modified: Thu, 23 Mar 2023 16:23:05 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42ed775b429742a2b9aa4f680d2104804ccaac99aeccda29c0e231896875d5dc`  
		Last Modified: Thu, 23 Mar 2023 16:23:05 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; s390x

```console
$ docker pull spiped@sha256:bd0f6a8ba4b8c11fe888fee6860ea1d54be076bfe5957b43344b7b62dec0f47c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.8 MB (34844023 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:434b1ada99c83de5816075c26b07f7e49e021c25d4e40b80ddaf363ced468b65`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 12 Apr 2023 00:01:00 GMT
ADD file:b6463dba97ba9c0a29bacfafc4d67bc603ab57e80b75e23cd42d7ef4b0f8e6ae in / 
# Wed, 12 Apr 2023 00:01:04 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 07:13:35 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 12 Apr 2023 07:13:37 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 07:13:37 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 12 Apr 2023 07:13:53 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 12 Apr 2023 07:13:54 GMT
VOLUME [/spiped]
# Wed, 12 Apr 2023 07:13:54 GMT
WORKDIR /spiped
# Wed, 12 Apr 2023 07:13:54 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 12 Apr 2023 07:13:54 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 12 Apr 2023 07:13:54 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:97fe10bc7def58e7938e97e41eec4788ec7a45b6ef2cb1770cec02fa831fd19d`  
		Last Modified: Wed, 12 Apr 2023 00:05:18 GMT  
		Size: 29.7 MB (29653156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60661451feca33d0d1fc43f91b66dabebcd27f2ad19153400d0feafc64799c08`  
		Last Modified: Wed, 12 Apr 2023 07:14:13 GMT  
		Size: 1.7 KB (1736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28a1ae3818d2c3bcea0558356a7a736f1cc9b24645b2ad17f5a548b75d857b3b`  
		Last Modified: Wed, 12 Apr 2023 07:14:13 GMT  
		Size: 1.1 KB (1050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f4048da853c0e9dbdd6b2016bd4357a1c880ae93bc8c8567bbd675caccd414b`  
		Last Modified: Wed, 12 Apr 2023 07:14:14 GMT  
		Size: 5.2 MB (5187613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:302aa23f2c1ca3a68f99772fae7ea836cbcbc3330cca4b8604b18889c292b96d`  
		Last Modified: Wed, 12 Apr 2023 07:14:13 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74dc85c46ada57925ebdfcf7391a313ed62367842185b9add5f65f61a2945c2c`  
		Last Modified: Wed, 12 Apr 2023 07:14:13 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
