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
$ docker pull spiped@sha256:20f18baf1351de70d6928b2a59b422a949eff8afba4f76bd0540c1e6b2952da1
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
$ docker pull spiped@sha256:2b04395676c417cf5dfb5b0f3c8e3c46fdf74f8877a8be349b4e4b8fa80e5c99
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.9 MB (33947457 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f1a108ba39d682af914151c33589b0fbb63c729edf128d9d89d35abca7ec4327`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 23 Mar 2023 00:48:44 GMT
ADD file:7595c7bfa6b3741f57a3ec7790e3108bb526244e52bb4a54548b8b5541e66616 in / 
# Thu, 23 Mar 2023 00:48:44 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 06:37:36 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Thu, 23 Mar 2023 06:37:40 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 06:37:40 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 23 Mar 2023 06:37:58 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 23 Mar 2023 06:37:58 GMT
VOLUME [/spiped]
# Thu, 23 Mar 2023 06:37:58 GMT
WORKDIR /spiped
# Thu, 23 Mar 2023 06:37:59 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 23 Mar 2023 06:37:59 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Mar 2023 06:37:59 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:b83d345710cdef1626d1940689dd3160e5ce3e4f63b3154cf612c52b704baa66`  
		Last Modified: Thu, 23 Mar 2023 02:22:00 GMT  
		Size: 28.9 MB (28915852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:329d3f48a6fd036ecccccba243d4cbd4a787a423a8acc7639ba39540cf1b4fef`  
		Last Modified: Fri, 24 Mar 2023 23:23:27 GMT  
		Size: 1.7 KB (1727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12ad0943836229229b35e9edffdd27381f53c79bf072a5c1d29a918edb1f9117`  
		Last Modified: Fri, 24 Mar 2023 23:23:27 GMT  
		Size: 1.1 KB (1055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e857a2b241c18b160e6bcfcde1014a4856fbb46f294a23ea436633b8c39de44`  
		Last Modified: Fri, 24 Mar 2023 23:23:28 GMT  
		Size: 5.0 MB (5028355 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a5a75981281f867a3883db65263ee0f882090d04e05f406625d1f0d8b6cf451`  
		Last Modified: Fri, 24 Mar 2023 23:23:27 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a02c78b876cc7c0d690105ab4a4062d4638a02f8758d22097c2de7db5522f6e9`  
		Last Modified: Fri, 24 Mar 2023 23:23:27 GMT  
		Size: 341.0 B  
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
$ docker pull spiped@sha256:83a2dfc12408a55b715b9d45db88323ca6ffa0c02f99863cebca86e185075f77
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.3 MB (35338624 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b179408f8deba9e064252982f9cd7dd1c620b39b9f92fe944f11f41fe6ee4034`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 23 Mar 2023 00:45:10 GMT
ADD file:83beb883b699cd442f1dbd4baf29c23f4cd15f7a5f9f120979df16a77455c69f in / 
# Thu, 23 Mar 2023 00:45:10 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 13:43:39 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Thu, 23 Mar 2023 13:43:42 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 13:43:42 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 23 Mar 2023 13:43:59 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 23 Mar 2023 13:43:59 GMT
VOLUME [/spiped]
# Thu, 23 Mar 2023 13:43:59 GMT
WORKDIR /spiped
# Thu, 23 Mar 2023 13:43:59 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 23 Mar 2023 13:43:59 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Mar 2023 13:43:59 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:fcdb9667c46b09d1c1d058681ea4a1db41e66bbc1a71d873a0c9da4f7a92947d`  
		Last Modified: Thu, 23 Mar 2023 00:48:09 GMT  
		Size: 30.1 MB (30062700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2effc6a047059b8e9cffce6fae471147dc3693bf3de5cbee776045031cc39d2a`  
		Last Modified: Thu, 23 Mar 2023 13:44:09 GMT  
		Size: 1.7 KB (1737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a693eec838be9148554badd7c7f9a4450637a59296cad5c8f29f01f7a94eb06`  
		Last Modified: Thu, 23 Mar 2023 13:44:09 GMT  
		Size: 1.1 KB (1053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e50b6e48b07af8f02ad556b18d717ea2f6582892cc92ca245a00673615d997d`  
		Last Modified: Thu, 23 Mar 2023 13:44:10 GMT  
		Size: 5.3 MB (5272665 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd251d4d636a1c0f0e831386315fc92c1077818d633e6534dc0bca9b32f9583d`  
		Last Modified: Thu, 23 Mar 2023 13:44:09 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b721c1e413d37abb114efa0264c82557f95c59c8900f30795680795dd8425050`  
		Last Modified: Thu, 23 Mar 2023 13:44:09 GMT  
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
$ docker pull spiped@sha256:5052a882da69e191760a75d37205ff0a1edd8edf21ae507a22d93c6b1672215a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.8 MB (34837546 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4be5954f5bff77d2a4e04836cc5938d850a56e7ee023f169242f1226e121a558`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 23 Mar 2023 00:44:06 GMT
ADD file:8b6d3f57adaa8af2e0599a6468c50b713d281165b4e61150850bedf587f7ad4f in / 
# Thu, 23 Mar 2023 00:44:08 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 12:15:46 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Thu, 23 Mar 2023 12:15:49 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 12:15:49 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 23 Mar 2023 12:16:07 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 23 Mar 2023 12:16:08 GMT
VOLUME [/spiped]
# Thu, 23 Mar 2023 12:16:08 GMT
WORKDIR /spiped
# Thu, 23 Mar 2023 12:16:08 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 23 Mar 2023 12:16:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Mar 2023 12:16:09 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:25d08e051bb75230bad82e3a7a054083beec6b4f6a46c8345c731582c297a408`  
		Last Modified: Thu, 23 Mar 2023 00:47:20 GMT  
		Size: 29.6 MB (29646820 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3388e32dd1b77d93d6b62ba801fb658ac69c6eebde8b030476caac13f83542be`  
		Last Modified: Thu, 23 Mar 2023 12:16:29 GMT  
		Size: 1.7 KB (1736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a701ac09c5ac118d050e81f6139936da77a346003315c4444e1939a6b9fbf5a`  
		Last Modified: Thu, 23 Mar 2023 12:16:29 GMT  
		Size: 1.1 KB (1050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76c28eecb90a4ce4306f2ee104c3b7a26ed907a1d7b4ffe9ee9f404860df7d2f`  
		Last Modified: Thu, 23 Mar 2023 12:16:30 GMT  
		Size: 5.2 MB (5187470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:851271a85236c408b9e2df7b62a45c37bc5552fb05fc8fb30a87d4f40e207d26`  
		Last Modified: Thu, 23 Mar 2023 12:16:29 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30749340374b1df790439fe4c7b71b610b3d0ae3aef3705de18f2472f5933c06`  
		Last Modified: Thu, 23 Mar 2023 12:16:29 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:1-alpine`

```console
$ docker pull spiped@sha256:3d145fc39678828e58c91872b3866181b9ab0139b75f2be21b8086b6ed121bd1
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
$ docker pull spiped@sha256:361539f7f9277859ba382de7be4afe676210140f53c3c5cd85d5ae3985f905c0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4237927 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2e899581be5421f50eb7e6339c7512ab16c114d8213f09e8aca52c68f0bcc311`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 10 Feb 2023 21:51:31 GMT
ADD file:143b601fcc6b5d7d95d3e5ccad3fec7081191a47e28d4f9294a7fb2499cab1af in / 
# Fri, 10 Feb 2023 21:51:31 GMT
CMD ["/bin/sh"]
# Wed, 01 Mar 2023 17:00:05 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Wed, 01 Mar 2023 17:00:07 GMT
RUN apk add --no-cache libssl1.1
# Wed, 01 Mar 2023 17:00:07 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 01 Mar 2023 17:00:14 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Wed, 01 Mar 2023 17:00:14 GMT
VOLUME [/spiped]
# Wed, 01 Mar 2023 17:00:14 GMT
WORKDIR /spiped
# Wed, 01 Mar 2023 17:00:14 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 01 Mar 2023 17:00:14 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 01 Mar 2023 17:00:15 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:6fb81ff47bd6d7db0ed86c9b951ad6417ec73ab60af6d22daa604076a902629c`  
		Last Modified: Fri, 10 Feb 2023 21:52:33 GMT  
		Size: 2.9 MB (2868494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bcf9acc5eeca77f6d435380f4f1fea53c3643c4cc9042daf13fdd9b6b72d9f5`  
		Last Modified: Wed, 01 Mar 2023 17:00:57 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f34e65da889251051ec9481b5d6cb0d428c45c8861fb2948b0c38c07470bba59`  
		Last Modified: Wed, 01 Mar 2023 17:00:57 GMT  
		Size: 1.2 MB (1167579 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0412dc4bafb0f9dabcfd28a3c0b4454de2db5c81112fdbb51bf5c883f4a6925`  
		Last Modified: Wed, 01 Mar 2023 17:00:57 GMT  
		Size: 200.1 KB (200120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70011259fd33df6da621cfb9142329c3c7a89b4bc5bfe91a87f7335995930ff9`  
		Last Modified: Wed, 01 Mar 2023 17:00:57 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99d3fd9f335e89a8501d7008f1bbaf813f4a5b26227452ecfc0001613be1ee7f`  
		Last Modified: Wed, 01 Mar 2023 17:00:57 GMT  
		Size: 337.0 B  
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
$ docker pull spiped@sha256:1718408d282e2785554de5dd41b1935a8fd740cad6fa42ddeac2fafad4e15148
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.1 MB (5131990 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e81769d87082a52703eb2f30d09dbe3c289d1e6956af04796da66cf8ec2e5a5b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 10 Feb 2023 21:24:23 GMT
ADD file:125f3514520a5cd29df2830a409aa026a2bc06a77a7a5d150133436404b33d41 in / 
# Fri, 10 Feb 2023 21:24:24 GMT
CMD ["/bin/sh"]
# Wed, 01 Mar 2023 20:35:30 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Wed, 01 Mar 2023 20:35:32 GMT
RUN apk add --no-cache libssl1.1
# Wed, 01 Mar 2023 20:35:32 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 01 Mar 2023 20:35:44 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Wed, 01 Mar 2023 20:35:44 GMT
VOLUME [/spiped]
# Wed, 01 Mar 2023 20:35:44 GMT
WORKDIR /spiped
# Wed, 01 Mar 2023 20:35:44 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 01 Mar 2023 20:35:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 01 Mar 2023 20:35:44 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:b3e346c15c2377ec0e75cc9efa98baecd58b0e9bb92f0ec07eeda0bcc7e67fc7`  
		Last Modified: Fri, 10 Feb 2023 21:25:13 GMT  
		Size: 3.4 MB (3412353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9ddea08df82e419c862a82c04a7b6027073e509f79247aaab6fcb9a2d66e4bc`  
		Last Modified: Wed, 01 Mar 2023 20:36:27 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7baff4523d8b5b8d72311936f6b35a74dc61f50af8ceb150e8a464755ed3ff76`  
		Last Modified: Wed, 01 Mar 2023 20:36:27 GMT  
		Size: 1.5 MB (1486288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de00b81755546779184cb3998ef43c5c0445cd5871998c7feb92240ab36aeb5e`  
		Last Modified: Wed, 01 Mar 2023 20:36:27 GMT  
		Size: 231.6 KB (231613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:568814bee4cca693df73f2ed16adcc10335f014f7606b67b33d08c3abf12b51a`  
		Last Modified: Wed, 01 Mar 2023 20:36:27 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da028d97e3da3f51bb23a54f50dc51e00a905208ac487c94ae446e20f926b63c`  
		Last Modified: Wed, 01 Mar 2023 20:36:27 GMT  
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
$ docker pull spiped@sha256:20f18baf1351de70d6928b2a59b422a949eff8afba4f76bd0540c1e6b2952da1
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
$ docker pull spiped@sha256:2b04395676c417cf5dfb5b0f3c8e3c46fdf74f8877a8be349b4e4b8fa80e5c99
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.9 MB (33947457 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f1a108ba39d682af914151c33589b0fbb63c729edf128d9d89d35abca7ec4327`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 23 Mar 2023 00:48:44 GMT
ADD file:7595c7bfa6b3741f57a3ec7790e3108bb526244e52bb4a54548b8b5541e66616 in / 
# Thu, 23 Mar 2023 00:48:44 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 06:37:36 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Thu, 23 Mar 2023 06:37:40 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 06:37:40 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 23 Mar 2023 06:37:58 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 23 Mar 2023 06:37:58 GMT
VOLUME [/spiped]
# Thu, 23 Mar 2023 06:37:58 GMT
WORKDIR /spiped
# Thu, 23 Mar 2023 06:37:59 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 23 Mar 2023 06:37:59 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Mar 2023 06:37:59 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:b83d345710cdef1626d1940689dd3160e5ce3e4f63b3154cf612c52b704baa66`  
		Last Modified: Thu, 23 Mar 2023 02:22:00 GMT  
		Size: 28.9 MB (28915852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:329d3f48a6fd036ecccccba243d4cbd4a787a423a8acc7639ba39540cf1b4fef`  
		Last Modified: Fri, 24 Mar 2023 23:23:27 GMT  
		Size: 1.7 KB (1727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12ad0943836229229b35e9edffdd27381f53c79bf072a5c1d29a918edb1f9117`  
		Last Modified: Fri, 24 Mar 2023 23:23:27 GMT  
		Size: 1.1 KB (1055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e857a2b241c18b160e6bcfcde1014a4856fbb46f294a23ea436633b8c39de44`  
		Last Modified: Fri, 24 Mar 2023 23:23:28 GMT  
		Size: 5.0 MB (5028355 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a5a75981281f867a3883db65263ee0f882090d04e05f406625d1f0d8b6cf451`  
		Last Modified: Fri, 24 Mar 2023 23:23:27 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a02c78b876cc7c0d690105ab4a4062d4638a02f8758d22097c2de7db5522f6e9`  
		Last Modified: Fri, 24 Mar 2023 23:23:27 GMT  
		Size: 341.0 B  
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
$ docker pull spiped@sha256:83a2dfc12408a55b715b9d45db88323ca6ffa0c02f99863cebca86e185075f77
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.3 MB (35338624 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b179408f8deba9e064252982f9cd7dd1c620b39b9f92fe944f11f41fe6ee4034`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 23 Mar 2023 00:45:10 GMT
ADD file:83beb883b699cd442f1dbd4baf29c23f4cd15f7a5f9f120979df16a77455c69f in / 
# Thu, 23 Mar 2023 00:45:10 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 13:43:39 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Thu, 23 Mar 2023 13:43:42 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 13:43:42 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 23 Mar 2023 13:43:59 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 23 Mar 2023 13:43:59 GMT
VOLUME [/spiped]
# Thu, 23 Mar 2023 13:43:59 GMT
WORKDIR /spiped
# Thu, 23 Mar 2023 13:43:59 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 23 Mar 2023 13:43:59 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Mar 2023 13:43:59 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:fcdb9667c46b09d1c1d058681ea4a1db41e66bbc1a71d873a0c9da4f7a92947d`  
		Last Modified: Thu, 23 Mar 2023 00:48:09 GMT  
		Size: 30.1 MB (30062700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2effc6a047059b8e9cffce6fae471147dc3693bf3de5cbee776045031cc39d2a`  
		Last Modified: Thu, 23 Mar 2023 13:44:09 GMT  
		Size: 1.7 KB (1737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a693eec838be9148554badd7c7f9a4450637a59296cad5c8f29f01f7a94eb06`  
		Last Modified: Thu, 23 Mar 2023 13:44:09 GMT  
		Size: 1.1 KB (1053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e50b6e48b07af8f02ad556b18d717ea2f6582892cc92ca245a00673615d997d`  
		Last Modified: Thu, 23 Mar 2023 13:44:10 GMT  
		Size: 5.3 MB (5272665 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd251d4d636a1c0f0e831386315fc92c1077818d633e6534dc0bca9b32f9583d`  
		Last Modified: Thu, 23 Mar 2023 13:44:09 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b721c1e413d37abb114efa0264c82557f95c59c8900f30795680795dd8425050`  
		Last Modified: Thu, 23 Mar 2023 13:44:09 GMT  
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
$ docker pull spiped@sha256:5052a882da69e191760a75d37205ff0a1edd8edf21ae507a22d93c6b1672215a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.8 MB (34837546 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4be5954f5bff77d2a4e04836cc5938d850a56e7ee023f169242f1226e121a558`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 23 Mar 2023 00:44:06 GMT
ADD file:8b6d3f57adaa8af2e0599a6468c50b713d281165b4e61150850bedf587f7ad4f in / 
# Thu, 23 Mar 2023 00:44:08 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 12:15:46 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Thu, 23 Mar 2023 12:15:49 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 12:15:49 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 23 Mar 2023 12:16:07 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 23 Mar 2023 12:16:08 GMT
VOLUME [/spiped]
# Thu, 23 Mar 2023 12:16:08 GMT
WORKDIR /spiped
# Thu, 23 Mar 2023 12:16:08 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 23 Mar 2023 12:16:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Mar 2023 12:16:09 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:25d08e051bb75230bad82e3a7a054083beec6b4f6a46c8345c731582c297a408`  
		Last Modified: Thu, 23 Mar 2023 00:47:20 GMT  
		Size: 29.6 MB (29646820 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3388e32dd1b77d93d6b62ba801fb658ac69c6eebde8b030476caac13f83542be`  
		Last Modified: Thu, 23 Mar 2023 12:16:29 GMT  
		Size: 1.7 KB (1736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a701ac09c5ac118d050e81f6139936da77a346003315c4444e1939a6b9fbf5a`  
		Last Modified: Thu, 23 Mar 2023 12:16:29 GMT  
		Size: 1.1 KB (1050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76c28eecb90a4ce4306f2ee104c3b7a26ed907a1d7b4ffe9ee9f404860df7d2f`  
		Last Modified: Thu, 23 Mar 2023 12:16:30 GMT  
		Size: 5.2 MB (5187470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:851271a85236c408b9e2df7b62a45c37bc5552fb05fc8fb30a87d4f40e207d26`  
		Last Modified: Thu, 23 Mar 2023 12:16:29 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30749340374b1df790439fe4c7b71b610b3d0ae3aef3705de18f2472f5933c06`  
		Last Modified: Thu, 23 Mar 2023 12:16:29 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:1.6-alpine`

```console
$ docker pull spiped@sha256:3d145fc39678828e58c91872b3866181b9ab0139b75f2be21b8086b6ed121bd1
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
$ docker pull spiped@sha256:361539f7f9277859ba382de7be4afe676210140f53c3c5cd85d5ae3985f905c0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4237927 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2e899581be5421f50eb7e6339c7512ab16c114d8213f09e8aca52c68f0bcc311`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 10 Feb 2023 21:51:31 GMT
ADD file:143b601fcc6b5d7d95d3e5ccad3fec7081191a47e28d4f9294a7fb2499cab1af in / 
# Fri, 10 Feb 2023 21:51:31 GMT
CMD ["/bin/sh"]
# Wed, 01 Mar 2023 17:00:05 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Wed, 01 Mar 2023 17:00:07 GMT
RUN apk add --no-cache libssl1.1
# Wed, 01 Mar 2023 17:00:07 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 01 Mar 2023 17:00:14 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Wed, 01 Mar 2023 17:00:14 GMT
VOLUME [/spiped]
# Wed, 01 Mar 2023 17:00:14 GMT
WORKDIR /spiped
# Wed, 01 Mar 2023 17:00:14 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 01 Mar 2023 17:00:14 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 01 Mar 2023 17:00:15 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:6fb81ff47bd6d7db0ed86c9b951ad6417ec73ab60af6d22daa604076a902629c`  
		Last Modified: Fri, 10 Feb 2023 21:52:33 GMT  
		Size: 2.9 MB (2868494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bcf9acc5eeca77f6d435380f4f1fea53c3643c4cc9042daf13fdd9b6b72d9f5`  
		Last Modified: Wed, 01 Mar 2023 17:00:57 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f34e65da889251051ec9481b5d6cb0d428c45c8861fb2948b0c38c07470bba59`  
		Last Modified: Wed, 01 Mar 2023 17:00:57 GMT  
		Size: 1.2 MB (1167579 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0412dc4bafb0f9dabcfd28a3c0b4454de2db5c81112fdbb51bf5c883f4a6925`  
		Last Modified: Wed, 01 Mar 2023 17:00:57 GMT  
		Size: 200.1 KB (200120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70011259fd33df6da621cfb9142329c3c7a89b4bc5bfe91a87f7335995930ff9`  
		Last Modified: Wed, 01 Mar 2023 17:00:57 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99d3fd9f335e89a8501d7008f1bbaf813f4a5b26227452ecfc0001613be1ee7f`  
		Last Modified: Wed, 01 Mar 2023 17:00:57 GMT  
		Size: 337.0 B  
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
$ docker pull spiped@sha256:1718408d282e2785554de5dd41b1935a8fd740cad6fa42ddeac2fafad4e15148
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.1 MB (5131990 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e81769d87082a52703eb2f30d09dbe3c289d1e6956af04796da66cf8ec2e5a5b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 10 Feb 2023 21:24:23 GMT
ADD file:125f3514520a5cd29df2830a409aa026a2bc06a77a7a5d150133436404b33d41 in / 
# Fri, 10 Feb 2023 21:24:24 GMT
CMD ["/bin/sh"]
# Wed, 01 Mar 2023 20:35:30 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Wed, 01 Mar 2023 20:35:32 GMT
RUN apk add --no-cache libssl1.1
# Wed, 01 Mar 2023 20:35:32 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 01 Mar 2023 20:35:44 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Wed, 01 Mar 2023 20:35:44 GMT
VOLUME [/spiped]
# Wed, 01 Mar 2023 20:35:44 GMT
WORKDIR /spiped
# Wed, 01 Mar 2023 20:35:44 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 01 Mar 2023 20:35:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 01 Mar 2023 20:35:44 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:b3e346c15c2377ec0e75cc9efa98baecd58b0e9bb92f0ec07eeda0bcc7e67fc7`  
		Last Modified: Fri, 10 Feb 2023 21:25:13 GMT  
		Size: 3.4 MB (3412353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9ddea08df82e419c862a82c04a7b6027073e509f79247aaab6fcb9a2d66e4bc`  
		Last Modified: Wed, 01 Mar 2023 20:36:27 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7baff4523d8b5b8d72311936f6b35a74dc61f50af8ceb150e8a464755ed3ff76`  
		Last Modified: Wed, 01 Mar 2023 20:36:27 GMT  
		Size: 1.5 MB (1486288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de00b81755546779184cb3998ef43c5c0445cd5871998c7feb92240ab36aeb5e`  
		Last Modified: Wed, 01 Mar 2023 20:36:27 GMT  
		Size: 231.6 KB (231613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:568814bee4cca693df73f2ed16adcc10335f014f7606b67b33d08c3abf12b51a`  
		Last Modified: Wed, 01 Mar 2023 20:36:27 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da028d97e3da3f51bb23a54f50dc51e00a905208ac487c94ae446e20f926b63c`  
		Last Modified: Wed, 01 Mar 2023 20:36:27 GMT  
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
$ docker pull spiped@sha256:20f18baf1351de70d6928b2a59b422a949eff8afba4f76bd0540c1e6b2952da1
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
$ docker pull spiped@sha256:2b04395676c417cf5dfb5b0f3c8e3c46fdf74f8877a8be349b4e4b8fa80e5c99
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.9 MB (33947457 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f1a108ba39d682af914151c33589b0fbb63c729edf128d9d89d35abca7ec4327`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 23 Mar 2023 00:48:44 GMT
ADD file:7595c7bfa6b3741f57a3ec7790e3108bb526244e52bb4a54548b8b5541e66616 in / 
# Thu, 23 Mar 2023 00:48:44 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 06:37:36 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Thu, 23 Mar 2023 06:37:40 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 06:37:40 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 23 Mar 2023 06:37:58 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 23 Mar 2023 06:37:58 GMT
VOLUME [/spiped]
# Thu, 23 Mar 2023 06:37:58 GMT
WORKDIR /spiped
# Thu, 23 Mar 2023 06:37:59 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 23 Mar 2023 06:37:59 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Mar 2023 06:37:59 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:b83d345710cdef1626d1940689dd3160e5ce3e4f63b3154cf612c52b704baa66`  
		Last Modified: Thu, 23 Mar 2023 02:22:00 GMT  
		Size: 28.9 MB (28915852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:329d3f48a6fd036ecccccba243d4cbd4a787a423a8acc7639ba39540cf1b4fef`  
		Last Modified: Fri, 24 Mar 2023 23:23:27 GMT  
		Size: 1.7 KB (1727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12ad0943836229229b35e9edffdd27381f53c79bf072a5c1d29a918edb1f9117`  
		Last Modified: Fri, 24 Mar 2023 23:23:27 GMT  
		Size: 1.1 KB (1055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e857a2b241c18b160e6bcfcde1014a4856fbb46f294a23ea436633b8c39de44`  
		Last Modified: Fri, 24 Mar 2023 23:23:28 GMT  
		Size: 5.0 MB (5028355 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a5a75981281f867a3883db65263ee0f882090d04e05f406625d1f0d8b6cf451`  
		Last Modified: Fri, 24 Mar 2023 23:23:27 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a02c78b876cc7c0d690105ab4a4062d4638a02f8758d22097c2de7db5522f6e9`  
		Last Modified: Fri, 24 Mar 2023 23:23:27 GMT  
		Size: 341.0 B  
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
$ docker pull spiped@sha256:83a2dfc12408a55b715b9d45db88323ca6ffa0c02f99863cebca86e185075f77
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.3 MB (35338624 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b179408f8deba9e064252982f9cd7dd1c620b39b9f92fe944f11f41fe6ee4034`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 23 Mar 2023 00:45:10 GMT
ADD file:83beb883b699cd442f1dbd4baf29c23f4cd15f7a5f9f120979df16a77455c69f in / 
# Thu, 23 Mar 2023 00:45:10 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 13:43:39 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Thu, 23 Mar 2023 13:43:42 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 13:43:42 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 23 Mar 2023 13:43:59 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 23 Mar 2023 13:43:59 GMT
VOLUME [/spiped]
# Thu, 23 Mar 2023 13:43:59 GMT
WORKDIR /spiped
# Thu, 23 Mar 2023 13:43:59 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 23 Mar 2023 13:43:59 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Mar 2023 13:43:59 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:fcdb9667c46b09d1c1d058681ea4a1db41e66bbc1a71d873a0c9da4f7a92947d`  
		Last Modified: Thu, 23 Mar 2023 00:48:09 GMT  
		Size: 30.1 MB (30062700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2effc6a047059b8e9cffce6fae471147dc3693bf3de5cbee776045031cc39d2a`  
		Last Modified: Thu, 23 Mar 2023 13:44:09 GMT  
		Size: 1.7 KB (1737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a693eec838be9148554badd7c7f9a4450637a59296cad5c8f29f01f7a94eb06`  
		Last Modified: Thu, 23 Mar 2023 13:44:09 GMT  
		Size: 1.1 KB (1053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e50b6e48b07af8f02ad556b18d717ea2f6582892cc92ca245a00673615d997d`  
		Last Modified: Thu, 23 Mar 2023 13:44:10 GMT  
		Size: 5.3 MB (5272665 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd251d4d636a1c0f0e831386315fc92c1077818d633e6534dc0bca9b32f9583d`  
		Last Modified: Thu, 23 Mar 2023 13:44:09 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b721c1e413d37abb114efa0264c82557f95c59c8900f30795680795dd8425050`  
		Last Modified: Thu, 23 Mar 2023 13:44:09 GMT  
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
$ docker pull spiped@sha256:5052a882da69e191760a75d37205ff0a1edd8edf21ae507a22d93c6b1672215a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.8 MB (34837546 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4be5954f5bff77d2a4e04836cc5938d850a56e7ee023f169242f1226e121a558`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 23 Mar 2023 00:44:06 GMT
ADD file:8b6d3f57adaa8af2e0599a6468c50b713d281165b4e61150850bedf587f7ad4f in / 
# Thu, 23 Mar 2023 00:44:08 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 12:15:46 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Thu, 23 Mar 2023 12:15:49 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 12:15:49 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 23 Mar 2023 12:16:07 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 23 Mar 2023 12:16:08 GMT
VOLUME [/spiped]
# Thu, 23 Mar 2023 12:16:08 GMT
WORKDIR /spiped
# Thu, 23 Mar 2023 12:16:08 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 23 Mar 2023 12:16:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Mar 2023 12:16:09 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:25d08e051bb75230bad82e3a7a054083beec6b4f6a46c8345c731582c297a408`  
		Last Modified: Thu, 23 Mar 2023 00:47:20 GMT  
		Size: 29.6 MB (29646820 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3388e32dd1b77d93d6b62ba801fb658ac69c6eebde8b030476caac13f83542be`  
		Last Modified: Thu, 23 Mar 2023 12:16:29 GMT  
		Size: 1.7 KB (1736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a701ac09c5ac118d050e81f6139936da77a346003315c4444e1939a6b9fbf5a`  
		Last Modified: Thu, 23 Mar 2023 12:16:29 GMT  
		Size: 1.1 KB (1050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76c28eecb90a4ce4306f2ee104c3b7a26ed907a1d7b4ffe9ee9f404860df7d2f`  
		Last Modified: Thu, 23 Mar 2023 12:16:30 GMT  
		Size: 5.2 MB (5187470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:851271a85236c408b9e2df7b62a45c37bc5552fb05fc8fb30a87d4f40e207d26`  
		Last Modified: Thu, 23 Mar 2023 12:16:29 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30749340374b1df790439fe4c7b71b610b3d0ae3aef3705de18f2472f5933c06`  
		Last Modified: Thu, 23 Mar 2023 12:16:29 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:1.6.2-alpine`

```console
$ docker pull spiped@sha256:3d145fc39678828e58c91872b3866181b9ab0139b75f2be21b8086b6ed121bd1
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
$ docker pull spiped@sha256:361539f7f9277859ba382de7be4afe676210140f53c3c5cd85d5ae3985f905c0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4237927 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2e899581be5421f50eb7e6339c7512ab16c114d8213f09e8aca52c68f0bcc311`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 10 Feb 2023 21:51:31 GMT
ADD file:143b601fcc6b5d7d95d3e5ccad3fec7081191a47e28d4f9294a7fb2499cab1af in / 
# Fri, 10 Feb 2023 21:51:31 GMT
CMD ["/bin/sh"]
# Wed, 01 Mar 2023 17:00:05 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Wed, 01 Mar 2023 17:00:07 GMT
RUN apk add --no-cache libssl1.1
# Wed, 01 Mar 2023 17:00:07 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 01 Mar 2023 17:00:14 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Wed, 01 Mar 2023 17:00:14 GMT
VOLUME [/spiped]
# Wed, 01 Mar 2023 17:00:14 GMT
WORKDIR /spiped
# Wed, 01 Mar 2023 17:00:14 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 01 Mar 2023 17:00:14 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 01 Mar 2023 17:00:15 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:6fb81ff47bd6d7db0ed86c9b951ad6417ec73ab60af6d22daa604076a902629c`  
		Last Modified: Fri, 10 Feb 2023 21:52:33 GMT  
		Size: 2.9 MB (2868494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bcf9acc5eeca77f6d435380f4f1fea53c3643c4cc9042daf13fdd9b6b72d9f5`  
		Last Modified: Wed, 01 Mar 2023 17:00:57 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f34e65da889251051ec9481b5d6cb0d428c45c8861fb2948b0c38c07470bba59`  
		Last Modified: Wed, 01 Mar 2023 17:00:57 GMT  
		Size: 1.2 MB (1167579 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0412dc4bafb0f9dabcfd28a3c0b4454de2db5c81112fdbb51bf5c883f4a6925`  
		Last Modified: Wed, 01 Mar 2023 17:00:57 GMT  
		Size: 200.1 KB (200120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70011259fd33df6da621cfb9142329c3c7a89b4bc5bfe91a87f7335995930ff9`  
		Last Modified: Wed, 01 Mar 2023 17:00:57 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99d3fd9f335e89a8501d7008f1bbaf813f4a5b26227452ecfc0001613be1ee7f`  
		Last Modified: Wed, 01 Mar 2023 17:00:57 GMT  
		Size: 337.0 B  
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
$ docker pull spiped@sha256:1718408d282e2785554de5dd41b1935a8fd740cad6fa42ddeac2fafad4e15148
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.1 MB (5131990 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e81769d87082a52703eb2f30d09dbe3c289d1e6956af04796da66cf8ec2e5a5b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 10 Feb 2023 21:24:23 GMT
ADD file:125f3514520a5cd29df2830a409aa026a2bc06a77a7a5d150133436404b33d41 in / 
# Fri, 10 Feb 2023 21:24:24 GMT
CMD ["/bin/sh"]
# Wed, 01 Mar 2023 20:35:30 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Wed, 01 Mar 2023 20:35:32 GMT
RUN apk add --no-cache libssl1.1
# Wed, 01 Mar 2023 20:35:32 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 01 Mar 2023 20:35:44 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Wed, 01 Mar 2023 20:35:44 GMT
VOLUME [/spiped]
# Wed, 01 Mar 2023 20:35:44 GMT
WORKDIR /spiped
# Wed, 01 Mar 2023 20:35:44 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 01 Mar 2023 20:35:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 01 Mar 2023 20:35:44 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:b3e346c15c2377ec0e75cc9efa98baecd58b0e9bb92f0ec07eeda0bcc7e67fc7`  
		Last Modified: Fri, 10 Feb 2023 21:25:13 GMT  
		Size: 3.4 MB (3412353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9ddea08df82e419c862a82c04a7b6027073e509f79247aaab6fcb9a2d66e4bc`  
		Last Modified: Wed, 01 Mar 2023 20:36:27 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7baff4523d8b5b8d72311936f6b35a74dc61f50af8ceb150e8a464755ed3ff76`  
		Last Modified: Wed, 01 Mar 2023 20:36:27 GMT  
		Size: 1.5 MB (1486288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de00b81755546779184cb3998ef43c5c0445cd5871998c7feb92240ab36aeb5e`  
		Last Modified: Wed, 01 Mar 2023 20:36:27 GMT  
		Size: 231.6 KB (231613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:568814bee4cca693df73f2ed16adcc10335f014f7606b67b33d08c3abf12b51a`  
		Last Modified: Wed, 01 Mar 2023 20:36:27 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da028d97e3da3f51bb23a54f50dc51e00a905208ac487c94ae446e20f926b63c`  
		Last Modified: Wed, 01 Mar 2023 20:36:27 GMT  
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
$ docker pull spiped@sha256:3d145fc39678828e58c91872b3866181b9ab0139b75f2be21b8086b6ed121bd1
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
$ docker pull spiped@sha256:361539f7f9277859ba382de7be4afe676210140f53c3c5cd85d5ae3985f905c0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4237927 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2e899581be5421f50eb7e6339c7512ab16c114d8213f09e8aca52c68f0bcc311`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 10 Feb 2023 21:51:31 GMT
ADD file:143b601fcc6b5d7d95d3e5ccad3fec7081191a47e28d4f9294a7fb2499cab1af in / 
# Fri, 10 Feb 2023 21:51:31 GMT
CMD ["/bin/sh"]
# Wed, 01 Mar 2023 17:00:05 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Wed, 01 Mar 2023 17:00:07 GMT
RUN apk add --no-cache libssl1.1
# Wed, 01 Mar 2023 17:00:07 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 01 Mar 2023 17:00:14 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Wed, 01 Mar 2023 17:00:14 GMT
VOLUME [/spiped]
# Wed, 01 Mar 2023 17:00:14 GMT
WORKDIR /spiped
# Wed, 01 Mar 2023 17:00:14 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 01 Mar 2023 17:00:14 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 01 Mar 2023 17:00:15 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:6fb81ff47bd6d7db0ed86c9b951ad6417ec73ab60af6d22daa604076a902629c`  
		Last Modified: Fri, 10 Feb 2023 21:52:33 GMT  
		Size: 2.9 MB (2868494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bcf9acc5eeca77f6d435380f4f1fea53c3643c4cc9042daf13fdd9b6b72d9f5`  
		Last Modified: Wed, 01 Mar 2023 17:00:57 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f34e65da889251051ec9481b5d6cb0d428c45c8861fb2948b0c38c07470bba59`  
		Last Modified: Wed, 01 Mar 2023 17:00:57 GMT  
		Size: 1.2 MB (1167579 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0412dc4bafb0f9dabcfd28a3c0b4454de2db5c81112fdbb51bf5c883f4a6925`  
		Last Modified: Wed, 01 Mar 2023 17:00:57 GMT  
		Size: 200.1 KB (200120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70011259fd33df6da621cfb9142329c3c7a89b4bc5bfe91a87f7335995930ff9`  
		Last Modified: Wed, 01 Mar 2023 17:00:57 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99d3fd9f335e89a8501d7008f1bbaf813f4a5b26227452ecfc0001613be1ee7f`  
		Last Modified: Wed, 01 Mar 2023 17:00:57 GMT  
		Size: 337.0 B  
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
$ docker pull spiped@sha256:1718408d282e2785554de5dd41b1935a8fd740cad6fa42ddeac2fafad4e15148
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.1 MB (5131990 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e81769d87082a52703eb2f30d09dbe3c289d1e6956af04796da66cf8ec2e5a5b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Fri, 10 Feb 2023 21:24:23 GMT
ADD file:125f3514520a5cd29df2830a409aa026a2bc06a77a7a5d150133436404b33d41 in / 
# Fri, 10 Feb 2023 21:24:24 GMT
CMD ["/bin/sh"]
# Wed, 01 Mar 2023 20:35:30 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Wed, 01 Mar 2023 20:35:32 GMT
RUN apk add --no-cache libssl1.1
# Wed, 01 Mar 2023 20:35:32 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 01 Mar 2023 20:35:44 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Wed, 01 Mar 2023 20:35:44 GMT
VOLUME [/spiped]
# Wed, 01 Mar 2023 20:35:44 GMT
WORKDIR /spiped
# Wed, 01 Mar 2023 20:35:44 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 01 Mar 2023 20:35:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 01 Mar 2023 20:35:44 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:b3e346c15c2377ec0e75cc9efa98baecd58b0e9bb92f0ec07eeda0bcc7e67fc7`  
		Last Modified: Fri, 10 Feb 2023 21:25:13 GMT  
		Size: 3.4 MB (3412353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9ddea08df82e419c862a82c04a7b6027073e509f79247aaab6fcb9a2d66e4bc`  
		Last Modified: Wed, 01 Mar 2023 20:36:27 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7baff4523d8b5b8d72311936f6b35a74dc61f50af8ceb150e8a464755ed3ff76`  
		Last Modified: Wed, 01 Mar 2023 20:36:27 GMT  
		Size: 1.5 MB (1486288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de00b81755546779184cb3998ef43c5c0445cd5871998c7feb92240ab36aeb5e`  
		Last Modified: Wed, 01 Mar 2023 20:36:27 GMT  
		Size: 231.6 KB (231613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:568814bee4cca693df73f2ed16adcc10335f014f7606b67b33d08c3abf12b51a`  
		Last Modified: Wed, 01 Mar 2023 20:36:27 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da028d97e3da3f51bb23a54f50dc51e00a905208ac487c94ae446e20f926b63c`  
		Last Modified: Wed, 01 Mar 2023 20:36:27 GMT  
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
$ docker pull spiped@sha256:20f18baf1351de70d6928b2a59b422a949eff8afba4f76bd0540c1e6b2952da1
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
$ docker pull spiped@sha256:2b04395676c417cf5dfb5b0f3c8e3c46fdf74f8877a8be349b4e4b8fa80e5c99
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.9 MB (33947457 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f1a108ba39d682af914151c33589b0fbb63c729edf128d9d89d35abca7ec4327`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 23 Mar 2023 00:48:44 GMT
ADD file:7595c7bfa6b3741f57a3ec7790e3108bb526244e52bb4a54548b8b5541e66616 in / 
# Thu, 23 Mar 2023 00:48:44 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 06:37:36 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Thu, 23 Mar 2023 06:37:40 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 06:37:40 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 23 Mar 2023 06:37:58 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 23 Mar 2023 06:37:58 GMT
VOLUME [/spiped]
# Thu, 23 Mar 2023 06:37:58 GMT
WORKDIR /spiped
# Thu, 23 Mar 2023 06:37:59 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 23 Mar 2023 06:37:59 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Mar 2023 06:37:59 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:b83d345710cdef1626d1940689dd3160e5ce3e4f63b3154cf612c52b704baa66`  
		Last Modified: Thu, 23 Mar 2023 02:22:00 GMT  
		Size: 28.9 MB (28915852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:329d3f48a6fd036ecccccba243d4cbd4a787a423a8acc7639ba39540cf1b4fef`  
		Last Modified: Fri, 24 Mar 2023 23:23:27 GMT  
		Size: 1.7 KB (1727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12ad0943836229229b35e9edffdd27381f53c79bf072a5c1d29a918edb1f9117`  
		Last Modified: Fri, 24 Mar 2023 23:23:27 GMT  
		Size: 1.1 KB (1055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e857a2b241c18b160e6bcfcde1014a4856fbb46f294a23ea436633b8c39de44`  
		Last Modified: Fri, 24 Mar 2023 23:23:28 GMT  
		Size: 5.0 MB (5028355 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a5a75981281f867a3883db65263ee0f882090d04e05f406625d1f0d8b6cf451`  
		Last Modified: Fri, 24 Mar 2023 23:23:27 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a02c78b876cc7c0d690105ab4a4062d4638a02f8758d22097c2de7db5522f6e9`  
		Last Modified: Fri, 24 Mar 2023 23:23:27 GMT  
		Size: 341.0 B  
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
$ docker pull spiped@sha256:83a2dfc12408a55b715b9d45db88323ca6ffa0c02f99863cebca86e185075f77
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.3 MB (35338624 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b179408f8deba9e064252982f9cd7dd1c620b39b9f92fe944f11f41fe6ee4034`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 23 Mar 2023 00:45:10 GMT
ADD file:83beb883b699cd442f1dbd4baf29c23f4cd15f7a5f9f120979df16a77455c69f in / 
# Thu, 23 Mar 2023 00:45:10 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 13:43:39 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Thu, 23 Mar 2023 13:43:42 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 13:43:42 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 23 Mar 2023 13:43:59 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 23 Mar 2023 13:43:59 GMT
VOLUME [/spiped]
# Thu, 23 Mar 2023 13:43:59 GMT
WORKDIR /spiped
# Thu, 23 Mar 2023 13:43:59 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 23 Mar 2023 13:43:59 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Mar 2023 13:43:59 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:fcdb9667c46b09d1c1d058681ea4a1db41e66bbc1a71d873a0c9da4f7a92947d`  
		Last Modified: Thu, 23 Mar 2023 00:48:09 GMT  
		Size: 30.1 MB (30062700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2effc6a047059b8e9cffce6fae471147dc3693bf3de5cbee776045031cc39d2a`  
		Last Modified: Thu, 23 Mar 2023 13:44:09 GMT  
		Size: 1.7 KB (1737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a693eec838be9148554badd7c7f9a4450637a59296cad5c8f29f01f7a94eb06`  
		Last Modified: Thu, 23 Mar 2023 13:44:09 GMT  
		Size: 1.1 KB (1053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e50b6e48b07af8f02ad556b18d717ea2f6582892cc92ca245a00673615d997d`  
		Last Modified: Thu, 23 Mar 2023 13:44:10 GMT  
		Size: 5.3 MB (5272665 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd251d4d636a1c0f0e831386315fc92c1077818d633e6534dc0bca9b32f9583d`  
		Last Modified: Thu, 23 Mar 2023 13:44:09 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b721c1e413d37abb114efa0264c82557f95c59c8900f30795680795dd8425050`  
		Last Modified: Thu, 23 Mar 2023 13:44:09 GMT  
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
$ docker pull spiped@sha256:5052a882da69e191760a75d37205ff0a1edd8edf21ae507a22d93c6b1672215a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.8 MB (34837546 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4be5954f5bff77d2a4e04836cc5938d850a56e7ee023f169242f1226e121a558`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Thu, 23 Mar 2023 00:44:06 GMT
ADD file:8b6d3f57adaa8af2e0599a6468c50b713d281165b4e61150850bedf587f7ad4f in / 
# Thu, 23 Mar 2023 00:44:08 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 12:15:46 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Thu, 23 Mar 2023 12:15:49 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 12:15:49 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 23 Mar 2023 12:16:07 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 23 Mar 2023 12:16:08 GMT
VOLUME [/spiped]
# Thu, 23 Mar 2023 12:16:08 GMT
WORKDIR /spiped
# Thu, 23 Mar 2023 12:16:08 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 23 Mar 2023 12:16:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Mar 2023 12:16:09 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:25d08e051bb75230bad82e3a7a054083beec6b4f6a46c8345c731582c297a408`  
		Last Modified: Thu, 23 Mar 2023 00:47:20 GMT  
		Size: 29.6 MB (29646820 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3388e32dd1b77d93d6b62ba801fb658ac69c6eebde8b030476caac13f83542be`  
		Last Modified: Thu, 23 Mar 2023 12:16:29 GMT  
		Size: 1.7 KB (1736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a701ac09c5ac118d050e81f6139936da77a346003315c4444e1939a6b9fbf5a`  
		Last Modified: Thu, 23 Mar 2023 12:16:29 GMT  
		Size: 1.1 KB (1050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76c28eecb90a4ce4306f2ee104c3b7a26ed907a1d7b4ffe9ee9f404860df7d2f`  
		Last Modified: Thu, 23 Mar 2023 12:16:30 GMT  
		Size: 5.2 MB (5187470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:851271a85236c408b9e2df7b62a45c37bc5552fb05fc8fb30a87d4f40e207d26`  
		Last Modified: Thu, 23 Mar 2023 12:16:29 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30749340374b1df790439fe4c7b71b610b3d0ae3aef3705de18f2472f5933c06`  
		Last Modified: Thu, 23 Mar 2023 12:16:29 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
