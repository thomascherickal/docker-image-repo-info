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
$ docker pull spiped@sha256:7a1276ab6a9bd4e55b8313b8cd13c2feabdc32369f047a82db7b499c42206a14
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
$ docker pull spiped@sha256:a66911a787746637e44a865f64e731ea404d2266efa5d987ee58d6d535a3999b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.3 MB (37349901 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4b801341ea8d054b7b965f35306e02a25be57d78de5177ed30cfb7af2b0267b7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 11 May 2022 01:20:16 GMT
ADD file:4a0bb88956083aa56032fdd9601d9b66c39b18c896ba35ea33594cd75621640a in / 
# Wed, 11 May 2022 01:20:16 GMT
CMD ["bash"]
# Wed, 11 May 2022 09:31:09 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 11 May 2022 09:31:12 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 09:31:12 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 11 May 2022 09:31:32 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 11 May 2022 09:31:32 GMT
VOLUME [/spiped]
# Wed, 11 May 2022 09:31:32 GMT
WORKDIR /spiped
# Wed, 11 May 2022 09:31:32 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 11 May 2022 09:31:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 11 May 2022 09:31:32 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:214ca5fb90323fe769c63a12af092f2572bf1c6b300263e09883909fc865d260`  
		Last Modified: Wed, 11 May 2022 01:25:13 GMT  
		Size: 31.4 MB (31379476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:080576f9a12bf8fca30a9653a7d9a0772acec767c26a2330bcdd92e5be0cfe95`  
		Last Modified: Wed, 11 May 2022 09:31:50 GMT  
		Size: 1.7 KB (1732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38bcb584eb7cb0f5bd593db63ab12b7b34bea2aa958fde7434a9b859ec903c08`  
		Last Modified: Wed, 11 May 2022 09:31:49 GMT  
		Size: 1.1 KB (1051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5664b9af48e8dd5dd00adb4691215c987017dbdb64998cdc9c30c22786d136d`  
		Last Modified: Wed, 11 May 2022 09:31:51 GMT  
		Size: 6.0 MB (5967174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6affb70c27746eb9c197393a54cd9b606353628e04424d0b4935ac195b6674a`  
		Last Modified: Wed, 11 May 2022 09:31:49 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01cd4accaf294c916a8ef636747fa575dbaa0f547f8bd5c7001c0112a9507dc2`  
		Last Modified: Wed, 11 May 2022 09:31:49 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; arm variant v5

```console
$ docker pull spiped@sha256:6b56704713f5efb9e393f0c751fe4e3ecfc3762033496269972dbb442a70972d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.0 MB (33952053 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6b14d990d1127fdf382852ac149cf58dd872a968df8176e8a74a5778ea0738c1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 11 May 2022 00:50:34 GMT
ADD file:72357b75d7e4546f06abf4648ab600980e742a3017f36da3c7a6c086f2f5fb56 in / 
# Wed, 11 May 2022 00:50:35 GMT
CMD ["bash"]
# Thu, 12 May 2022 01:35:14 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Thu, 12 May 2022 01:35:23 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Thu, 12 May 2022 01:35:23 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 12 May 2022 01:36:14 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 12 May 2022 01:36:15 GMT
VOLUME [/spiped]
# Thu, 12 May 2022 01:36:15 GMT
WORKDIR /spiped
# Thu, 12 May 2022 01:36:16 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 12 May 2022 01:36:16 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 12 May 2022 01:36:17 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:f7b69be15db1cb94a249f74b27edd4f5e5923a8701b026179a593f6888e897aa`  
		Last Modified: Wed, 11 May 2022 01:05:51 GMT  
		Size: 28.9 MB (28921122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a5a9157aa645038e20cfd8d939540308935a2f448009504b4b50f55ebe7fcc8`  
		Last Modified: Thu, 12 May 2022 01:36:50 GMT  
		Size: 1.7 KB (1725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:379d8521d9bd468b1d6a357f9682b3e0efc683bb7ce8c61b98639d89a6e5a9d3`  
		Last Modified: Thu, 12 May 2022 01:36:50 GMT  
		Size: 1.1 KB (1050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94258b91da89ba5bcfb0b99e7a7224030f4fbc734a79e19488d7b2e198797278`  
		Last Modified: Thu, 12 May 2022 01:36:55 GMT  
		Size: 5.0 MB (5027685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8ecd42d03f9650c45b9f15fb17188211b89f7ea6683a8aa6d8cf3ea08653577`  
		Last Modified: Thu, 12 May 2022 01:36:50 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82055141d6a68a71687d6ce1c4aa739a9d6fa527bf54e1eb9120550413add7ea`  
		Last Modified: Thu, 12 May 2022 01:36:50 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; arm variant v7

```console
$ docker pull spiped@sha256:426553dc9b38cdd633ce43cdf604b956d3d21c098bc256d936f9154132930908
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.3 MB (31327127 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7e6ef92e514ca9a3a7a716f84914ba360321d707df4255203a53390721630843`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 11 May 2022 01:49:07 GMT
ADD file:7c0451fffe8a520c2ab23048948d76bfe0dc0d90298c3d859279ccd8815b84f6 in / 
# Wed, 11 May 2022 01:49:08 GMT
CMD ["bash"]
# Thu, 12 May 2022 09:57:40 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Thu, 12 May 2022 09:57:47 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Thu, 12 May 2022 09:57:48 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 12 May 2022 09:58:33 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 12 May 2022 09:58:34 GMT
VOLUME [/spiped]
# Thu, 12 May 2022 09:58:34 GMT
WORKDIR /spiped
# Thu, 12 May 2022 09:58:35 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 12 May 2022 09:58:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 12 May 2022 09:58:36 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:1a9427b75b1c1db800cae7a9199bb4e508702e6761b17cc904d21441df43016c`  
		Last Modified: Wed, 11 May 2022 02:04:35 GMT  
		Size: 26.6 MB (26575672 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:666c704c2d2710e68360474f0cd959985e4418ee1bf3da5f69155679a1aae5e3`  
		Last Modified: Thu, 12 May 2022 09:59:35 GMT  
		Size: 1.7 KB (1736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:997d8d681765c85ae870076561eed251de76347cf9bf8d4fe9ca8bea5ee94d7e`  
		Last Modified: Thu, 12 May 2022 09:59:36 GMT  
		Size: 1.1 KB (1051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:666b40dc8c26e1e531689caf804a1d968693ea152f3580588acd62cd67aba309`  
		Last Modified: Thu, 12 May 2022 09:59:39 GMT  
		Size: 4.7 MB (4748197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d352d4363ba035dd50fa29f21ce08e12bdee48d3e9801fad5ae5d27d2e842c2`  
		Last Modified: Thu, 12 May 2022 09:59:35 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe1a6862d97ef70fbc74954b3f2e128027ea3142115032009c75b79794fedebb`  
		Last Modified: Thu, 12 May 2022 09:59:35 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:572906adb8bf287a02331ed2dc6b70d40c1795ce56eb514a7b873ac8b0b07782
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.3 MB (35339551 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:df8ebf44dc7acf424cbe762be8778cd542ccc7006e183a616763d3b92f5af2cc`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 11 May 2022 00:46:59 GMT
ADD file:158a0e401328bd7c0d49b9e8539186098967218f1b1a8c811f4398d29b74397f in / 
# Wed, 11 May 2022 00:47:00 GMT
CMD ["bash"]
# Wed, 11 May 2022 12:24:33 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 11 May 2022 12:24:36 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 12:24:37 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 11 May 2022 12:24:55 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 11 May 2022 12:24:56 GMT
VOLUME [/spiped]
# Wed, 11 May 2022 12:24:57 GMT
WORKDIR /spiped
# Wed, 11 May 2022 12:24:59 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 11 May 2022 12:24:59 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 11 May 2022 12:25:00 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:dfdd5ffb257742b891ccad9400a77dad2a6260b2451e0f5e48a9ade1d17a87ec`  
		Last Modified: Wed, 11 May 2022 00:53:46 GMT  
		Size: 30.1 MB (30065693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e25366de1af948b0eef7cad0d0d1fbc56648a743854da03fc57dc121c2384213`  
		Last Modified: Wed, 11 May 2022 12:25:32 GMT  
		Size: 1.6 KB (1621 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aef033e02dd13ee59e5336850b85b81cbd2ccd353a033415114d010d6a8254df`  
		Last Modified: Wed, 11 May 2022 12:25:32 GMT  
		Size: 922.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dac510a96382ea09a86f8f4cadc73653a8177516d4771a4a7e3bccbdeeb326de`  
		Last Modified: Wed, 11 May 2022 12:25:33 GMT  
		Size: 5.3 MB (5270881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1616a14c0096a1c7108f1fe3372296010619c2f7c502e1802e6d3855dfdf0ebd`  
		Last Modified: Wed, 11 May 2022 12:25:32 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcaa87e60ef72bc3e5eab8bd8a81a9cee650735736cd7c760f4366260b5461d2`  
		Last Modified: Wed, 11 May 2022 12:25:32 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; 386

```console
$ docker pull spiped@sha256:d933a3ef2f835e9d32f01babb2f55693ab6f3b2150d76a4e72d6fdec66739208
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.3 MB (40284215 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8994e3dd3df7e9fdbd0d51ca1e620fa69f6efd232ff5d5d2b381cd6b22fbc13c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 11 May 2022 01:39:14 GMT
ADD file:9eecb0fd311177f9d226e914c411aef49b5de1930e73019d2ee24afed515b5a2 in / 
# Wed, 11 May 2022 01:39:14 GMT
CMD ["bash"]
# Wed, 11 May 2022 15:51:27 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 11 May 2022 15:51:30 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 15:51:31 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 11 May 2022 15:51:52 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 11 May 2022 15:51:52 GMT
VOLUME [/spiped]
# Wed, 11 May 2022 15:51:53 GMT
WORKDIR /spiped
# Wed, 11 May 2022 15:51:55 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 11 May 2022 15:51:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 11 May 2022 15:51:56 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:91c5bdbe4bf9f1970dd54ba71e2523649adce4e5240c2ff8a87711bf389ecba3`  
		Last Modified: Wed, 11 May 2022 01:46:25 GMT  
		Size: 32.4 MB (32389776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa9bc810ed14e83b2b6c2de848151a8aac3442608851df4e4ba4f35402048a54`  
		Last Modified: Wed, 11 May 2022 15:52:27 GMT  
		Size: 1.6 KB (1608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ddd23897c0dc65364a8fda9129fe87c608a02ac54bdd3002e70407c7dff7b8a`  
		Last Modified: Wed, 11 May 2022 15:52:27 GMT  
		Size: 923.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a55bc0fd5c56c871a37888a72d560d40d0364889e86b54c791bea4bb7c85887`  
		Last Modified: Wed, 11 May 2022 15:52:28 GMT  
		Size: 7.9 MB (7891471 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad4fc1778cbfb42cc882687278e3d3bb64b10572a3b56cf12d7ba9b128537d21`  
		Last Modified: Wed, 11 May 2022 15:52:27 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cc951e82cef08be37b45eba1592c940f1a946d625884f3e80794061addeb20a`  
		Last Modified: Wed, 11 May 2022 15:52:27 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; mips64le

```console
$ docker pull spiped@sha256:98dafc6cf00b4ae4723240a88ce5bed8cc462c78e6e05aa1fdea9727db128735
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.3 MB (35349146 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:008c2d2ba6ac1949b574aa0cd913d936ebd6fadc503e85c425e3052ef113387d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 11 May 2022 02:23:35 GMT
ADD file:d47dce2adbc9352ef1d437730bab3b579dd8d2bf29dd60cd8a8b65396b39e36e in / 
# Wed, 11 May 2022 02:23:40 GMT
CMD ["bash"]
# Thu, 12 May 2022 04:11:52 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Thu, 12 May 2022 04:12:07 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Thu, 12 May 2022 04:12:09 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 12 May 2022 04:13:33 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 12 May 2022 04:13:36 GMT
VOLUME [/spiped]
# Thu, 12 May 2022 04:13:39 GMT
WORKDIR /spiped
# Thu, 12 May 2022 04:13:41 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 12 May 2022 04:13:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 12 May 2022 04:13:46 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:438a36bf0b6e75ff6f0fbb2b7669dfb86361416f4d808912d30cf5b91ad2eea9`  
		Last Modified: Wed, 11 May 2022 02:33:43 GMT  
		Size: 29.6 MB (29641051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b968eb568ff8a2acb36380ccbf842b116d8f7251fe76b4d4c05350e872efe8f`  
		Last Modified: Thu, 12 May 2022 04:14:11 GMT  
		Size: 1.6 KB (1614 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e0c58081df5c4242f571acbbce6534a045404bc2c44eab75dbe2bfa721606fc`  
		Last Modified: Thu, 12 May 2022 04:14:11 GMT  
		Size: 925.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2c0fc303ca2ffd0acaaa4421f936b6d1cdcbd87e50ae67c64e5d2f003a022f8`  
		Last Modified: Thu, 12 May 2022 04:14:16 GMT  
		Size: 5.7 MB (5705117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a84b67927c5aea3805e90f18768e6338fd392e91c3618805526b3ff7c776b824`  
		Last Modified: Thu, 12 May 2022 04:14:11 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c4229b76d1a9cdc6812c0c3734a7d00ca0f098edeb70043fce974697a9d2a4c`  
		Last Modified: Thu, 12 May 2022 04:14:11 GMT  
		Size: 344.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; ppc64le

```console
$ docker pull spiped@sha256:e338e5b4a068b2c06d20548b51e98cf9e6711b5ba3f91a55f33517103107db26
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.3 MB (41288815 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:54eb4238d8977094c460b01a31bf18ab2865f97d34da09adaf33454df8e1a99f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 11 May 2022 01:32:29 GMT
ADD file:1e94716789ec21981460f74be38a668bc212bd804c1d41cecf90036a5bccac5a in / 
# Wed, 11 May 2022 01:32:34 GMT
CMD ["bash"]
# Wed, 11 May 2022 14:18:46 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 11 May 2022 14:18:57 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 14:19:00 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 11 May 2022 14:21:35 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 11 May 2022 14:21:45 GMT
VOLUME [/spiped]
# Wed, 11 May 2022 14:21:59 GMT
WORKDIR /spiped
# Wed, 11 May 2022 14:22:09 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 11 May 2022 14:22:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 11 May 2022 14:22:21 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:2533109ed11eefd6415e0370d6d7a3ea879b582b1887c98b819a598ad18fca24`  
		Last Modified: Wed, 11 May 2022 01:43:03 GMT  
		Size: 35.3 MB (35286467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e371d58c256a557b6f8f7b903d8a39345ccc364236516cb3ec208e9e40e92c5`  
		Last Modified: Wed, 11 May 2022 14:23:02 GMT  
		Size: 1.7 KB (1743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b4caf1ad053d6d5585c461ca9b8d4c6a14a963b94b0d13bb0594b2244f15a8b`  
		Last Modified: Wed, 11 May 2022 14:23:02 GMT  
		Size: 1.1 KB (1054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb23602e10ec58354d8276b2a6d7549e7f11c523d76e28603f149ca4c0e1e951`  
		Last Modified: Wed, 11 May 2022 14:23:04 GMT  
		Size: 6.0 MB (5999080 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fa6bf1315149ea1738416c3df58107d0e9c60aae5cb546cfdcbb50aa6855062`  
		Last Modified: Wed, 11 May 2022 14:23:02 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82539badabc1522bce1e3acd0e092aceb9818dd6904d2ab5fe8a10ab39a0f6b5`  
		Last Modified: Wed, 11 May 2022 14:23:02 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1` - linux; s390x

```console
$ docker pull spiped@sha256:a2261239d98aaef54af72737a4aa30c1a01f4089439604c977e606d06e5eb317
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.8 MB (34844727 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d218c6ec1b1cc03c92a160497f19dc4deed41827aaf7bef061ddc8ca4c8f6fac`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 11 May 2022 00:44:17 GMT
ADD file:d93a1cf64a813d01774cd628dfd683c006e20159e2ab3464c2159c8d9897c725 in / 
# Wed, 11 May 2022 00:44:19 GMT
CMD ["bash"]
# Wed, 11 May 2022 06:26:51 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 11 May 2022 06:26:54 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 06:26:54 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 11 May 2022 06:27:06 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 11 May 2022 06:27:07 GMT
VOLUME [/spiped]
# Wed, 11 May 2022 06:27:07 GMT
WORKDIR /spiped
# Wed, 11 May 2022 06:27:07 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 11 May 2022 06:27:07 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 11 May 2022 06:27:07 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:9f3750f6094217808e26d471752341db88153c8d5b5f9bb11577b74671303bbc`  
		Last Modified: Wed, 11 May 2022 00:50:03 GMT  
		Size: 29.7 MB (29654739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:873c48057acd3a3e859a48bcca0c21842c182414ce09c34a3cc1c1886f7de52a`  
		Last Modified: Wed, 11 May 2022 06:27:39 GMT  
		Size: 1.7 KB (1734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09c3eb03701aaff2a58238f35a586fbc044102b129292492a02c7479e57440b3`  
		Last Modified: Wed, 11 May 2022 06:27:39 GMT  
		Size: 1.1 KB (1052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c22498c1d73103d486b8e69a684b02839606786d6cff45d0dfbdbdc6e26ce68c`  
		Last Modified: Wed, 11 May 2022 06:27:40 GMT  
		Size: 5.2 MB (5186734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6758dfdb3a7588b70d2a3af8806cc9cea3dee7221cfe99f32973d6c0eee71d46`  
		Last Modified: Wed, 11 May 2022 06:27:39 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6fcc234dd9c90350b33b0e204d793aec0e7ee86952bb815ce76739eced0d2a7`  
		Last Modified: Wed, 11 May 2022 06:27:39 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:1-alpine`

```console
$ docker pull spiped@sha256:e803772f3cd77bd5eb74c25cebf7dbe58c1490172affec2756736f01297e2ad6
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
$ docker pull spiped@sha256:b1000f43786f16a20a805fa353f6e29da279735ce16fc397001fde0e351cadab
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (3038963 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:319549bf17a1c296f365e261889f2573a629fda0ca36fa2dac3efc79c233dc4d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 05 Apr 2022 00:19:59 GMT
ADD file:5d673d25da3a14ce1f6cf66e4c7fd4f4b85a3759a9d93efb3fd9ff852b5b56e4 in / 
# Tue, 05 Apr 2022 00:19:59 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 09:41:12 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Tue, 05 Apr 2022 09:41:13 GMT
RUN apk add --no-cache libssl1.1
# Tue, 05 Apr 2022 09:41:13 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 05 Apr 2022 09:41:22 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Tue, 05 Apr 2022 09:41:22 GMT
VOLUME [/spiped]
# Tue, 05 Apr 2022 09:41:23 GMT
WORKDIR /spiped
# Tue, 05 Apr 2022 09:41:23 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 05 Apr 2022 09:41:23 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 05 Apr 2022 09:41:23 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:df9b9388f04ad6279a7410b85cedfdcb2208c0a003da7ab5613af71079148139`  
		Last Modified: Mon, 04 Apr 2022 19:10:16 GMT  
		Size: 2.8 MB (2814559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:735044c06e8b73c2bb88467804d54b359bfc8226cf975772cc666adc9f029f5c`  
		Last Modified: Tue, 05 Apr 2022 09:41:38 GMT  
		Size: 1.3 KB (1271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd8b16fcaec70a3de42b4e850be4a851eaffa96a04fb49668b0d55b15bdf9675`  
		Last Modified: Tue, 05 Apr 2022 09:41:38 GMT  
		Size: 7.8 KB (7783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79236b25532d68c328b81af71a0f8c4eca102b7030a98d650ffc9a7e35d113be`  
		Last Modified: Tue, 05 Apr 2022 09:41:38 GMT  
		Size: 214.9 KB (214880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f429bef29fed68fb012179a10893c62fd5167934a7d62e7d3db15361601d47e9`  
		Last Modified: Tue, 05 Apr 2022 09:41:38 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1703108ce26f514d42179cf03051a6082b57e184d89f7bab08377819025c74d9`  
		Last Modified: Tue, 05 Apr 2022 09:41:38 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; arm variant v6

```console
$ docker pull spiped@sha256:44fa18e7d3af978bedc72ce9110a2217004554deec585dfcdafffb4c761a1661
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 MB (2830637 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b21bdc008b33d69d3d83d8292f28384b56c4166b1ef0c3f5c05eac33a48df2a7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Mon, 04 Apr 2022 23:49:42 GMT
ADD file:159dcddaab900372df882a4e94615ed84250e9cea3e74bc0479d98280342f596 in / 
# Mon, 04 Apr 2022 23:49:42 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 11:42:28 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Tue, 05 Apr 2022 11:42:30 GMT
RUN apk add --no-cache libssl1.1
# Tue, 05 Apr 2022 11:42:30 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 05 Apr 2022 11:42:49 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Tue, 05 Apr 2022 11:42:50 GMT
VOLUME [/spiped]
# Tue, 05 Apr 2022 11:42:50 GMT
WORKDIR /spiped
# Tue, 05 Apr 2022 11:42:51 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 05 Apr 2022 11:42:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 05 Apr 2022 11:42:52 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:c319b1fc4ed70b8241a7ce6ac0c4015d354bf5cf8c01eb73c50b6709c0c46e49`  
		Last Modified: Mon, 04 Apr 2022 19:09:22 GMT  
		Size: 2.6 MB (2621972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b279880cad38890c6b22622a3cecb67733556ec9965319ffa327afec8900ad3`  
		Last Modified: Tue, 05 Apr 2022 11:43:27 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27045425770040b89c6aeadebc232d3bd49690ccc505ec5a20336cbfa650b899`  
		Last Modified: Tue, 05 Apr 2022 11:43:27 GMT  
		Size: 7.8 KB (7767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfe17e03d9a44e0c737a4484821d473ab6476046270059fab5ebad88fdbfcce7`  
		Last Modified: Tue, 05 Apr 2022 11:43:27 GMT  
		Size: 199.2 KB (199161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2979a2148a9f161c6f6ae02c8bdc6b41f1f18da7a66d2db5addec2e19752388b`  
		Last Modified: Tue, 05 Apr 2022 11:43:26 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5863282bd4052a3bc2b39bb2d4cc46b864b2e4214edba85c572e7f55f95d7ee1`  
		Last Modified: Tue, 05 Apr 2022 11:43:26 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; arm variant v7

```console
$ docker pull spiped@sha256:41ea58744c279880bd672731168c41728c367a5558010a8b15109a53651aed8b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 MB (2626540 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fa3a26053023e3df6fe0ab2fdfc9b5c0e7806a837bdf8aeeebed934566092f5f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Mon, 04 Apr 2022 23:57:34 GMT
ADD file:20f8cdddc53a4a8bd78945fc32fe08e9f80ab3b16dc20a9aa4ba73b79f2bc71c in / 
# Mon, 04 Apr 2022 23:57:35 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 15:38:30 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Tue, 05 Apr 2022 15:38:32 GMT
RUN apk add --no-cache libssl1.1
# Tue, 05 Apr 2022 15:38:33 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 05 Apr 2022 15:38:51 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Tue, 05 Apr 2022 15:38:51 GMT
VOLUME [/spiped]
# Tue, 05 Apr 2022 15:38:52 GMT
WORKDIR /spiped
# Tue, 05 Apr 2022 15:38:52 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 05 Apr 2022 15:38:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 05 Apr 2022 15:38:53 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:57fb4b5f1a47c953ca5703f0f81ce14e5d01cf23aa79558b5adb961cc526e320`  
		Last Modified: Mon, 04 Apr 2022 19:09:36 GMT  
		Size: 2.4 MB (2424323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c34bb3a817bf019eff75e990b3ee9f75b0d33a5070d140d69adcd81bc3c61d4`  
		Last Modified: Tue, 05 Apr 2022 15:39:47 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50ddc3edc7d50bace02b581239b3d2096bbdd43b8d5cca77199c023788b7bab9`  
		Last Modified: Tue, 05 Apr 2022 15:39:47 GMT  
		Size: 7.8 KB (7779 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e4b14e7f868497bf35a981b97fa3d6c40d44c373e6207c0e73aa3292319b6e8`  
		Last Modified: Tue, 05 Apr 2022 15:39:47 GMT  
		Size: 192.7 KB (192698 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c22a92e8f54240f73e546662dc34d0aa6b83ec1617f18fa8e178c93138c0b72e`  
		Last Modified: Tue, 05 Apr 2022 15:39:47 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98ad3607e9857b6fb1bb4fbf10d6e9ed9e787343edd64901dc0ecaadd3ff55db`  
		Last Modified: Tue, 05 Apr 2022 15:39:47 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:6b7fd2442f6dcd71561982dfb157122343a4c720493a891274c64d2c577ce4ab
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 MB (2933135 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8dc39b7901f2654c939cb1c1d44ff3a6e036a4bcf2cef396786768da4de2f658`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Mon, 04 Apr 2022 23:39:31 GMT
ADD file:90e56af13188c7f0283d244a0d70b853d8bef8587a41f1da8eac3a2aba8964ef in / 
# Mon, 04 Apr 2022 23:39:31 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 14:38:03 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Tue, 05 Apr 2022 14:38:04 GMT
RUN apk add --no-cache libssl1.1
# Tue, 05 Apr 2022 14:38:05 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 05 Apr 2022 14:38:15 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Tue, 05 Apr 2022 14:38:16 GMT
VOLUME [/spiped]
# Tue, 05 Apr 2022 14:38:17 GMT
WORKDIR /spiped
# Tue, 05 Apr 2022 14:38:19 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 05 Apr 2022 14:38:19 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 05 Apr 2022 14:38:20 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:9981e73032c8833e387a8f96986e560edbed12c38119e0edb0439c9c2234eac9`  
		Last Modified: Mon, 04 Apr 2022 19:09:10 GMT  
		Size: 2.7 MB (2716477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe4c0758a179cd25e16e078f253517cd4f315287416c3ce781a852e456da3093`  
		Last Modified: Tue, 05 Apr 2022 14:38:47 GMT  
		Size: 1.2 KB (1240 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ad68b994955132db089d9decfe3c1abb1e0d937a743641a82ff97b1ad0de230`  
		Last Modified: Tue, 05 Apr 2022 14:38:47 GMT  
		Size: 7.7 KB (7749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2412b85fbb446b18863d0276c285a9f15c5506327e253be647ba7c7e323d01e0`  
		Last Modified: Tue, 05 Apr 2022 14:38:47 GMT  
		Size: 207.2 KB (207235 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff9b28798cece086f58205831a8c06e9be4d79eb185eb2a5566b692c6bb0aa1f`  
		Last Modified: Tue, 05 Apr 2022 14:38:47 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9aa51b8e1739c24bc53b08bbda05fba07af4b69550a9c5ac36ea5be1bb7d5b1`  
		Last Modified: Tue, 05 Apr 2022 14:38:47 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; 386

```console
$ docker pull spiped@sha256:dcbb93128deb3206337ac10573e41e27b4a95816cd3f931412c655201fef2396
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.1 MB (3053817 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fdb9526919356b65e45d7bc9a9bd2aaddd7da8a1e62f023b9511a320a431df64`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Mon, 04 Apr 2022 23:38:25 GMT
ADD file:7d51a0f8691eb78c9062fd31984423a93d276a67b4ed5d1a706e1c2cd9fea23a in / 
# Mon, 04 Apr 2022 23:38:25 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 06:51:23 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Tue, 05 Apr 2022 06:51:24 GMT
RUN apk add --no-cache libssl1.1
# Tue, 05 Apr 2022 06:51:24 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 05 Apr 2022 06:51:34 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Tue, 05 Apr 2022 06:51:35 GMT
VOLUME [/spiped]
# Tue, 05 Apr 2022 06:51:36 GMT
WORKDIR /spiped
# Tue, 05 Apr 2022 06:51:38 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 05 Apr 2022 06:51:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 05 Apr 2022 06:51:39 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:73b28a5955ec7fb46f2cf0434e4901a889f7dda3f8c9ec496300feb256c7eda8`  
		Last Modified: Mon, 04 Apr 2022 19:10:03 GMT  
		Size: 2.8 MB (2818974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5043c44edf55100d2df153f657912b53abf987ef0c6286b113dcef298998f359`  
		Last Modified: Tue, 05 Apr 2022 06:52:09 GMT  
		Size: 1.2 KB (1240 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfc9d36e654ea336dd74dc00574768a6502edd5ef5cd785b695e516f6254be55`  
		Last Modified: Tue, 05 Apr 2022 06:52:08 GMT  
		Size: 7.8 KB (7750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0401735f1a5cdc5a0248a778049579b8858a6f7cc0fc6fdcdaea211930d4a386`  
		Last Modified: Tue, 05 Apr 2022 06:52:08 GMT  
		Size: 225.4 KB (225416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5a85e3f263e110e3fa50aada2a3ca6314a5a6e67e8f211881a826585a5db409`  
		Last Modified: Tue, 05 Apr 2022 06:52:08 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a0f113efbe13d3511b57cb0428e99f2725a51cb3980e75b1f1be3fc0d715b19`  
		Last Modified: Tue, 05 Apr 2022 06:52:08 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; ppc64le

```console
$ docker pull spiped@sha256:6d1206f429c5113ac4fbd6820b913ec32aa3cb826c65e5446d05eb57c3bfd7f4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (3033860 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:64a17da88fc17c158a4b17b8a85a6b534482d5b9fe198bee0a961886519d4811`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 05 Apr 2022 00:23:30 GMT
ADD file:960cf6f9d3d1cfcb36c2d67dd4c3eaba7db1d0c7afe97968512248d7f234ad47 in / 
# Tue, 05 Apr 2022 00:23:32 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 20:07:37 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Tue, 05 Apr 2022 20:08:01 GMT
RUN apk add --no-cache libssl1.1
# Tue, 05 Apr 2022 20:08:06 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 05 Apr 2022 20:08:35 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Tue, 05 Apr 2022 20:08:41 GMT
VOLUME [/spiped]
# Tue, 05 Apr 2022 20:08:46 GMT
WORKDIR /spiped
# Tue, 05 Apr 2022 20:08:48 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 05 Apr 2022 20:08:49 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 05 Apr 2022 20:08:52 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:1877acf2d48ed8bcb5bd9756a95aca0c077457be7cf4fcef25807f4e9be88db1`  
		Last Modified: Mon, 04 Apr 2022 19:09:49 GMT  
		Size: 2.8 MB (2811186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:898122ed2d1fcbc53be831191766c1b47d98b8cb2251d70dcc91e5ecad3bf34e`  
		Last Modified: Tue, 05 Apr 2022 20:09:25 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0cdc12b8854b22d6407eaece31ad74f6d0d2f322236c0d02a0074aef7944b93`  
		Last Modified: Tue, 05 Apr 2022 20:09:25 GMT  
		Size: 7.8 KB (7771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc1f84e0deee708d9995b37beb5b3923a9091dcc0ee670f7d784de701af40e2e`  
		Last Modified: Tue, 05 Apr 2022 20:09:25 GMT  
		Size: 213.2 KB (213160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67c77cab4a7338ba5a131c568ed153eb1fd0151dbb6108fae4fd3234a699f6ac`  
		Last Modified: Tue, 05 Apr 2022 20:09:25 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e03666b6f800b3362553b44e783b6eff051c84c4ae25bdb3d1da279626fc8bb9`  
		Last Modified: Tue, 05 Apr 2022 20:09:25 GMT  
		Size: 345.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1-alpine` - linux; s390x

```console
$ docker pull spiped@sha256:851d4d1e8b82de6d455e9a562bd6b75539fe737213c9f3cf01ce7b44e11abeb4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 MB (2811594 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e240f56e6000d053b4d3e20632b54b88daaa8dad76ecda720ce9f76c82bfe394`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Mon, 04 Apr 2022 23:41:39 GMT
ADD file:f22e4b2be87d3c59c8c609acf79015938dc1fba0b26d7c1b59bd0fc36d63a906 in / 
# Mon, 04 Apr 2022 23:41:39 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 06:09:44 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Tue, 05 Apr 2022 06:09:45 GMT
RUN apk add --no-cache libssl1.1
# Tue, 05 Apr 2022 06:09:45 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 05 Apr 2022 06:09:50 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Tue, 05 Apr 2022 06:09:50 GMT
VOLUME [/spiped]
# Tue, 05 Apr 2022 06:09:51 GMT
WORKDIR /spiped
# Tue, 05 Apr 2022 06:09:51 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 05 Apr 2022 06:09:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 05 Apr 2022 06:09:51 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:a27b630f446c3da376a30cf610e4bfa6847f8b87c83702c29e72b986f4e52d28`  
		Last Modified: Mon, 04 Apr 2022 23:42:37 GMT  
		Size: 2.6 MB (2600375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ffc8ec477cbe2d575e99a9232e9328db8cc40109dbe067d93c2033302576850`  
		Last Modified: Tue, 05 Apr 2022 06:10:22 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ee008c7ec71319091cda7b7cbf1063414ee758f739581409a2e7089e90882c9`  
		Last Modified: Tue, 05 Apr 2022 06:10:21 GMT  
		Size: 7.8 KB (7788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3edcb5212f084eabfd1bad6e332d8b53bd7756099c4da3e410ee23f869a701b`  
		Last Modified: Tue, 05 Apr 2022 06:10:21 GMT  
		Size: 201.7 KB (201693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd099e1efb05ce5fa06c5e18ba7d057b5df318c462022f1ac443f45e86fdc809`  
		Last Modified: Tue, 05 Apr 2022 06:10:21 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afbab95e29c022d6828d869e5e4442b139373571c747f8fc6470b8bd257337a4`  
		Last Modified: Tue, 05 Apr 2022 06:10:21 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:1.6`

```console
$ docker pull spiped@sha256:7a1276ab6a9bd4e55b8313b8cd13c2feabdc32369f047a82db7b499c42206a14
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
$ docker pull spiped@sha256:a66911a787746637e44a865f64e731ea404d2266efa5d987ee58d6d535a3999b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.3 MB (37349901 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4b801341ea8d054b7b965f35306e02a25be57d78de5177ed30cfb7af2b0267b7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 11 May 2022 01:20:16 GMT
ADD file:4a0bb88956083aa56032fdd9601d9b66c39b18c896ba35ea33594cd75621640a in / 
# Wed, 11 May 2022 01:20:16 GMT
CMD ["bash"]
# Wed, 11 May 2022 09:31:09 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 11 May 2022 09:31:12 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 09:31:12 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 11 May 2022 09:31:32 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 11 May 2022 09:31:32 GMT
VOLUME [/spiped]
# Wed, 11 May 2022 09:31:32 GMT
WORKDIR /spiped
# Wed, 11 May 2022 09:31:32 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 11 May 2022 09:31:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 11 May 2022 09:31:32 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:214ca5fb90323fe769c63a12af092f2572bf1c6b300263e09883909fc865d260`  
		Last Modified: Wed, 11 May 2022 01:25:13 GMT  
		Size: 31.4 MB (31379476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:080576f9a12bf8fca30a9653a7d9a0772acec767c26a2330bcdd92e5be0cfe95`  
		Last Modified: Wed, 11 May 2022 09:31:50 GMT  
		Size: 1.7 KB (1732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38bcb584eb7cb0f5bd593db63ab12b7b34bea2aa958fde7434a9b859ec903c08`  
		Last Modified: Wed, 11 May 2022 09:31:49 GMT  
		Size: 1.1 KB (1051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5664b9af48e8dd5dd00adb4691215c987017dbdb64998cdc9c30c22786d136d`  
		Last Modified: Wed, 11 May 2022 09:31:51 GMT  
		Size: 6.0 MB (5967174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6affb70c27746eb9c197393a54cd9b606353628e04424d0b4935ac195b6674a`  
		Last Modified: Wed, 11 May 2022 09:31:49 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01cd4accaf294c916a8ef636747fa575dbaa0f547f8bd5c7001c0112a9507dc2`  
		Last Modified: Wed, 11 May 2022 09:31:49 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; arm variant v5

```console
$ docker pull spiped@sha256:6b56704713f5efb9e393f0c751fe4e3ecfc3762033496269972dbb442a70972d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.0 MB (33952053 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6b14d990d1127fdf382852ac149cf58dd872a968df8176e8a74a5778ea0738c1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 11 May 2022 00:50:34 GMT
ADD file:72357b75d7e4546f06abf4648ab600980e742a3017f36da3c7a6c086f2f5fb56 in / 
# Wed, 11 May 2022 00:50:35 GMT
CMD ["bash"]
# Thu, 12 May 2022 01:35:14 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Thu, 12 May 2022 01:35:23 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Thu, 12 May 2022 01:35:23 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 12 May 2022 01:36:14 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 12 May 2022 01:36:15 GMT
VOLUME [/spiped]
# Thu, 12 May 2022 01:36:15 GMT
WORKDIR /spiped
# Thu, 12 May 2022 01:36:16 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 12 May 2022 01:36:16 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 12 May 2022 01:36:17 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:f7b69be15db1cb94a249f74b27edd4f5e5923a8701b026179a593f6888e897aa`  
		Last Modified: Wed, 11 May 2022 01:05:51 GMT  
		Size: 28.9 MB (28921122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a5a9157aa645038e20cfd8d939540308935a2f448009504b4b50f55ebe7fcc8`  
		Last Modified: Thu, 12 May 2022 01:36:50 GMT  
		Size: 1.7 KB (1725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:379d8521d9bd468b1d6a357f9682b3e0efc683bb7ce8c61b98639d89a6e5a9d3`  
		Last Modified: Thu, 12 May 2022 01:36:50 GMT  
		Size: 1.1 KB (1050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94258b91da89ba5bcfb0b99e7a7224030f4fbc734a79e19488d7b2e198797278`  
		Last Modified: Thu, 12 May 2022 01:36:55 GMT  
		Size: 5.0 MB (5027685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8ecd42d03f9650c45b9f15fb17188211b89f7ea6683a8aa6d8cf3ea08653577`  
		Last Modified: Thu, 12 May 2022 01:36:50 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82055141d6a68a71687d6ce1c4aa739a9d6fa527bf54e1eb9120550413add7ea`  
		Last Modified: Thu, 12 May 2022 01:36:50 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; arm variant v7

```console
$ docker pull spiped@sha256:426553dc9b38cdd633ce43cdf604b956d3d21c098bc256d936f9154132930908
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.3 MB (31327127 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7e6ef92e514ca9a3a7a716f84914ba360321d707df4255203a53390721630843`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 11 May 2022 01:49:07 GMT
ADD file:7c0451fffe8a520c2ab23048948d76bfe0dc0d90298c3d859279ccd8815b84f6 in / 
# Wed, 11 May 2022 01:49:08 GMT
CMD ["bash"]
# Thu, 12 May 2022 09:57:40 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Thu, 12 May 2022 09:57:47 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Thu, 12 May 2022 09:57:48 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 12 May 2022 09:58:33 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 12 May 2022 09:58:34 GMT
VOLUME [/spiped]
# Thu, 12 May 2022 09:58:34 GMT
WORKDIR /spiped
# Thu, 12 May 2022 09:58:35 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 12 May 2022 09:58:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 12 May 2022 09:58:36 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:1a9427b75b1c1db800cae7a9199bb4e508702e6761b17cc904d21441df43016c`  
		Last Modified: Wed, 11 May 2022 02:04:35 GMT  
		Size: 26.6 MB (26575672 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:666c704c2d2710e68360474f0cd959985e4418ee1bf3da5f69155679a1aae5e3`  
		Last Modified: Thu, 12 May 2022 09:59:35 GMT  
		Size: 1.7 KB (1736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:997d8d681765c85ae870076561eed251de76347cf9bf8d4fe9ca8bea5ee94d7e`  
		Last Modified: Thu, 12 May 2022 09:59:36 GMT  
		Size: 1.1 KB (1051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:666b40dc8c26e1e531689caf804a1d968693ea152f3580588acd62cd67aba309`  
		Last Modified: Thu, 12 May 2022 09:59:39 GMT  
		Size: 4.7 MB (4748197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d352d4363ba035dd50fa29f21ce08e12bdee48d3e9801fad5ae5d27d2e842c2`  
		Last Modified: Thu, 12 May 2022 09:59:35 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe1a6862d97ef70fbc74954b3f2e128027ea3142115032009c75b79794fedebb`  
		Last Modified: Thu, 12 May 2022 09:59:35 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:572906adb8bf287a02331ed2dc6b70d40c1795ce56eb514a7b873ac8b0b07782
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.3 MB (35339551 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:df8ebf44dc7acf424cbe762be8778cd542ccc7006e183a616763d3b92f5af2cc`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 11 May 2022 00:46:59 GMT
ADD file:158a0e401328bd7c0d49b9e8539186098967218f1b1a8c811f4398d29b74397f in / 
# Wed, 11 May 2022 00:47:00 GMT
CMD ["bash"]
# Wed, 11 May 2022 12:24:33 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 11 May 2022 12:24:36 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 12:24:37 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 11 May 2022 12:24:55 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 11 May 2022 12:24:56 GMT
VOLUME [/spiped]
# Wed, 11 May 2022 12:24:57 GMT
WORKDIR /spiped
# Wed, 11 May 2022 12:24:59 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 11 May 2022 12:24:59 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 11 May 2022 12:25:00 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:dfdd5ffb257742b891ccad9400a77dad2a6260b2451e0f5e48a9ade1d17a87ec`  
		Last Modified: Wed, 11 May 2022 00:53:46 GMT  
		Size: 30.1 MB (30065693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e25366de1af948b0eef7cad0d0d1fbc56648a743854da03fc57dc121c2384213`  
		Last Modified: Wed, 11 May 2022 12:25:32 GMT  
		Size: 1.6 KB (1621 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aef033e02dd13ee59e5336850b85b81cbd2ccd353a033415114d010d6a8254df`  
		Last Modified: Wed, 11 May 2022 12:25:32 GMT  
		Size: 922.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dac510a96382ea09a86f8f4cadc73653a8177516d4771a4a7e3bccbdeeb326de`  
		Last Modified: Wed, 11 May 2022 12:25:33 GMT  
		Size: 5.3 MB (5270881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1616a14c0096a1c7108f1fe3372296010619c2f7c502e1802e6d3855dfdf0ebd`  
		Last Modified: Wed, 11 May 2022 12:25:32 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcaa87e60ef72bc3e5eab8bd8a81a9cee650735736cd7c760f4366260b5461d2`  
		Last Modified: Wed, 11 May 2022 12:25:32 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; 386

```console
$ docker pull spiped@sha256:d933a3ef2f835e9d32f01babb2f55693ab6f3b2150d76a4e72d6fdec66739208
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.3 MB (40284215 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8994e3dd3df7e9fdbd0d51ca1e620fa69f6efd232ff5d5d2b381cd6b22fbc13c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 11 May 2022 01:39:14 GMT
ADD file:9eecb0fd311177f9d226e914c411aef49b5de1930e73019d2ee24afed515b5a2 in / 
# Wed, 11 May 2022 01:39:14 GMT
CMD ["bash"]
# Wed, 11 May 2022 15:51:27 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 11 May 2022 15:51:30 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 15:51:31 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 11 May 2022 15:51:52 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 11 May 2022 15:51:52 GMT
VOLUME [/spiped]
# Wed, 11 May 2022 15:51:53 GMT
WORKDIR /spiped
# Wed, 11 May 2022 15:51:55 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 11 May 2022 15:51:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 11 May 2022 15:51:56 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:91c5bdbe4bf9f1970dd54ba71e2523649adce4e5240c2ff8a87711bf389ecba3`  
		Last Modified: Wed, 11 May 2022 01:46:25 GMT  
		Size: 32.4 MB (32389776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa9bc810ed14e83b2b6c2de848151a8aac3442608851df4e4ba4f35402048a54`  
		Last Modified: Wed, 11 May 2022 15:52:27 GMT  
		Size: 1.6 KB (1608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ddd23897c0dc65364a8fda9129fe87c608a02ac54bdd3002e70407c7dff7b8a`  
		Last Modified: Wed, 11 May 2022 15:52:27 GMT  
		Size: 923.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a55bc0fd5c56c871a37888a72d560d40d0364889e86b54c791bea4bb7c85887`  
		Last Modified: Wed, 11 May 2022 15:52:28 GMT  
		Size: 7.9 MB (7891471 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad4fc1778cbfb42cc882687278e3d3bb64b10572a3b56cf12d7ba9b128537d21`  
		Last Modified: Wed, 11 May 2022 15:52:27 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cc951e82cef08be37b45eba1592c940f1a946d625884f3e80794061addeb20a`  
		Last Modified: Wed, 11 May 2022 15:52:27 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; mips64le

```console
$ docker pull spiped@sha256:98dafc6cf00b4ae4723240a88ce5bed8cc462c78e6e05aa1fdea9727db128735
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.3 MB (35349146 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:008c2d2ba6ac1949b574aa0cd913d936ebd6fadc503e85c425e3052ef113387d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 11 May 2022 02:23:35 GMT
ADD file:d47dce2adbc9352ef1d437730bab3b579dd8d2bf29dd60cd8a8b65396b39e36e in / 
# Wed, 11 May 2022 02:23:40 GMT
CMD ["bash"]
# Thu, 12 May 2022 04:11:52 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Thu, 12 May 2022 04:12:07 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Thu, 12 May 2022 04:12:09 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 12 May 2022 04:13:33 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 12 May 2022 04:13:36 GMT
VOLUME [/spiped]
# Thu, 12 May 2022 04:13:39 GMT
WORKDIR /spiped
# Thu, 12 May 2022 04:13:41 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 12 May 2022 04:13:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 12 May 2022 04:13:46 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:438a36bf0b6e75ff6f0fbb2b7669dfb86361416f4d808912d30cf5b91ad2eea9`  
		Last Modified: Wed, 11 May 2022 02:33:43 GMT  
		Size: 29.6 MB (29641051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b968eb568ff8a2acb36380ccbf842b116d8f7251fe76b4d4c05350e872efe8f`  
		Last Modified: Thu, 12 May 2022 04:14:11 GMT  
		Size: 1.6 KB (1614 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e0c58081df5c4242f571acbbce6534a045404bc2c44eab75dbe2bfa721606fc`  
		Last Modified: Thu, 12 May 2022 04:14:11 GMT  
		Size: 925.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2c0fc303ca2ffd0acaaa4421f936b6d1cdcbd87e50ae67c64e5d2f003a022f8`  
		Last Modified: Thu, 12 May 2022 04:14:16 GMT  
		Size: 5.7 MB (5705117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a84b67927c5aea3805e90f18768e6338fd392e91c3618805526b3ff7c776b824`  
		Last Modified: Thu, 12 May 2022 04:14:11 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c4229b76d1a9cdc6812c0c3734a7d00ca0f098edeb70043fce974697a9d2a4c`  
		Last Modified: Thu, 12 May 2022 04:14:11 GMT  
		Size: 344.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; ppc64le

```console
$ docker pull spiped@sha256:e338e5b4a068b2c06d20548b51e98cf9e6711b5ba3f91a55f33517103107db26
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.3 MB (41288815 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:54eb4238d8977094c460b01a31bf18ab2865f97d34da09adaf33454df8e1a99f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 11 May 2022 01:32:29 GMT
ADD file:1e94716789ec21981460f74be38a668bc212bd804c1d41cecf90036a5bccac5a in / 
# Wed, 11 May 2022 01:32:34 GMT
CMD ["bash"]
# Wed, 11 May 2022 14:18:46 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 11 May 2022 14:18:57 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 14:19:00 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 11 May 2022 14:21:35 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 11 May 2022 14:21:45 GMT
VOLUME [/spiped]
# Wed, 11 May 2022 14:21:59 GMT
WORKDIR /spiped
# Wed, 11 May 2022 14:22:09 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 11 May 2022 14:22:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 11 May 2022 14:22:21 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:2533109ed11eefd6415e0370d6d7a3ea879b582b1887c98b819a598ad18fca24`  
		Last Modified: Wed, 11 May 2022 01:43:03 GMT  
		Size: 35.3 MB (35286467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e371d58c256a557b6f8f7b903d8a39345ccc364236516cb3ec208e9e40e92c5`  
		Last Modified: Wed, 11 May 2022 14:23:02 GMT  
		Size: 1.7 KB (1743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b4caf1ad053d6d5585c461ca9b8d4c6a14a963b94b0d13bb0594b2244f15a8b`  
		Last Modified: Wed, 11 May 2022 14:23:02 GMT  
		Size: 1.1 KB (1054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb23602e10ec58354d8276b2a6d7549e7f11c523d76e28603f149ca4c0e1e951`  
		Last Modified: Wed, 11 May 2022 14:23:04 GMT  
		Size: 6.0 MB (5999080 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fa6bf1315149ea1738416c3df58107d0e9c60aae5cb546cfdcbb50aa6855062`  
		Last Modified: Wed, 11 May 2022 14:23:02 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82539badabc1522bce1e3acd0e092aceb9818dd6904d2ab5fe8a10ab39a0f6b5`  
		Last Modified: Wed, 11 May 2022 14:23:02 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6` - linux; s390x

```console
$ docker pull spiped@sha256:a2261239d98aaef54af72737a4aa30c1a01f4089439604c977e606d06e5eb317
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.8 MB (34844727 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d218c6ec1b1cc03c92a160497f19dc4deed41827aaf7bef061ddc8ca4c8f6fac`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 11 May 2022 00:44:17 GMT
ADD file:d93a1cf64a813d01774cd628dfd683c006e20159e2ab3464c2159c8d9897c725 in / 
# Wed, 11 May 2022 00:44:19 GMT
CMD ["bash"]
# Wed, 11 May 2022 06:26:51 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 11 May 2022 06:26:54 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 06:26:54 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 11 May 2022 06:27:06 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 11 May 2022 06:27:07 GMT
VOLUME [/spiped]
# Wed, 11 May 2022 06:27:07 GMT
WORKDIR /spiped
# Wed, 11 May 2022 06:27:07 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 11 May 2022 06:27:07 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 11 May 2022 06:27:07 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:9f3750f6094217808e26d471752341db88153c8d5b5f9bb11577b74671303bbc`  
		Last Modified: Wed, 11 May 2022 00:50:03 GMT  
		Size: 29.7 MB (29654739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:873c48057acd3a3e859a48bcca0c21842c182414ce09c34a3cc1c1886f7de52a`  
		Last Modified: Wed, 11 May 2022 06:27:39 GMT  
		Size: 1.7 KB (1734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09c3eb03701aaff2a58238f35a586fbc044102b129292492a02c7479e57440b3`  
		Last Modified: Wed, 11 May 2022 06:27:39 GMT  
		Size: 1.1 KB (1052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c22498c1d73103d486b8e69a684b02839606786d6cff45d0dfbdbdc6e26ce68c`  
		Last Modified: Wed, 11 May 2022 06:27:40 GMT  
		Size: 5.2 MB (5186734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6758dfdb3a7588b70d2a3af8806cc9cea3dee7221cfe99f32973d6c0eee71d46`  
		Last Modified: Wed, 11 May 2022 06:27:39 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6fcc234dd9c90350b33b0e204d793aec0e7ee86952bb815ce76739eced0d2a7`  
		Last Modified: Wed, 11 May 2022 06:27:39 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:1.6-alpine`

```console
$ docker pull spiped@sha256:e803772f3cd77bd5eb74c25cebf7dbe58c1490172affec2756736f01297e2ad6
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
$ docker pull spiped@sha256:b1000f43786f16a20a805fa353f6e29da279735ce16fc397001fde0e351cadab
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (3038963 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:319549bf17a1c296f365e261889f2573a629fda0ca36fa2dac3efc79c233dc4d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 05 Apr 2022 00:19:59 GMT
ADD file:5d673d25da3a14ce1f6cf66e4c7fd4f4b85a3759a9d93efb3fd9ff852b5b56e4 in / 
# Tue, 05 Apr 2022 00:19:59 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 09:41:12 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Tue, 05 Apr 2022 09:41:13 GMT
RUN apk add --no-cache libssl1.1
# Tue, 05 Apr 2022 09:41:13 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 05 Apr 2022 09:41:22 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Tue, 05 Apr 2022 09:41:22 GMT
VOLUME [/spiped]
# Tue, 05 Apr 2022 09:41:23 GMT
WORKDIR /spiped
# Tue, 05 Apr 2022 09:41:23 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 05 Apr 2022 09:41:23 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 05 Apr 2022 09:41:23 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:df9b9388f04ad6279a7410b85cedfdcb2208c0a003da7ab5613af71079148139`  
		Last Modified: Mon, 04 Apr 2022 19:10:16 GMT  
		Size: 2.8 MB (2814559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:735044c06e8b73c2bb88467804d54b359bfc8226cf975772cc666adc9f029f5c`  
		Last Modified: Tue, 05 Apr 2022 09:41:38 GMT  
		Size: 1.3 KB (1271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd8b16fcaec70a3de42b4e850be4a851eaffa96a04fb49668b0d55b15bdf9675`  
		Last Modified: Tue, 05 Apr 2022 09:41:38 GMT  
		Size: 7.8 KB (7783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79236b25532d68c328b81af71a0f8c4eca102b7030a98d650ffc9a7e35d113be`  
		Last Modified: Tue, 05 Apr 2022 09:41:38 GMT  
		Size: 214.9 KB (214880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f429bef29fed68fb012179a10893c62fd5167934a7d62e7d3db15361601d47e9`  
		Last Modified: Tue, 05 Apr 2022 09:41:38 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1703108ce26f514d42179cf03051a6082b57e184d89f7bab08377819025c74d9`  
		Last Modified: Tue, 05 Apr 2022 09:41:38 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; arm variant v6

```console
$ docker pull spiped@sha256:44fa18e7d3af978bedc72ce9110a2217004554deec585dfcdafffb4c761a1661
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 MB (2830637 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b21bdc008b33d69d3d83d8292f28384b56c4166b1ef0c3f5c05eac33a48df2a7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Mon, 04 Apr 2022 23:49:42 GMT
ADD file:159dcddaab900372df882a4e94615ed84250e9cea3e74bc0479d98280342f596 in / 
# Mon, 04 Apr 2022 23:49:42 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 11:42:28 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Tue, 05 Apr 2022 11:42:30 GMT
RUN apk add --no-cache libssl1.1
# Tue, 05 Apr 2022 11:42:30 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 05 Apr 2022 11:42:49 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Tue, 05 Apr 2022 11:42:50 GMT
VOLUME [/spiped]
# Tue, 05 Apr 2022 11:42:50 GMT
WORKDIR /spiped
# Tue, 05 Apr 2022 11:42:51 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 05 Apr 2022 11:42:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 05 Apr 2022 11:42:52 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:c319b1fc4ed70b8241a7ce6ac0c4015d354bf5cf8c01eb73c50b6709c0c46e49`  
		Last Modified: Mon, 04 Apr 2022 19:09:22 GMT  
		Size: 2.6 MB (2621972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b279880cad38890c6b22622a3cecb67733556ec9965319ffa327afec8900ad3`  
		Last Modified: Tue, 05 Apr 2022 11:43:27 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27045425770040b89c6aeadebc232d3bd49690ccc505ec5a20336cbfa650b899`  
		Last Modified: Tue, 05 Apr 2022 11:43:27 GMT  
		Size: 7.8 KB (7767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfe17e03d9a44e0c737a4484821d473ab6476046270059fab5ebad88fdbfcce7`  
		Last Modified: Tue, 05 Apr 2022 11:43:27 GMT  
		Size: 199.2 KB (199161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2979a2148a9f161c6f6ae02c8bdc6b41f1f18da7a66d2db5addec2e19752388b`  
		Last Modified: Tue, 05 Apr 2022 11:43:26 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5863282bd4052a3bc2b39bb2d4cc46b864b2e4214edba85c572e7f55f95d7ee1`  
		Last Modified: Tue, 05 Apr 2022 11:43:26 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; arm variant v7

```console
$ docker pull spiped@sha256:41ea58744c279880bd672731168c41728c367a5558010a8b15109a53651aed8b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 MB (2626540 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fa3a26053023e3df6fe0ab2fdfc9b5c0e7806a837bdf8aeeebed934566092f5f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Mon, 04 Apr 2022 23:57:34 GMT
ADD file:20f8cdddc53a4a8bd78945fc32fe08e9f80ab3b16dc20a9aa4ba73b79f2bc71c in / 
# Mon, 04 Apr 2022 23:57:35 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 15:38:30 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Tue, 05 Apr 2022 15:38:32 GMT
RUN apk add --no-cache libssl1.1
# Tue, 05 Apr 2022 15:38:33 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 05 Apr 2022 15:38:51 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Tue, 05 Apr 2022 15:38:51 GMT
VOLUME [/spiped]
# Tue, 05 Apr 2022 15:38:52 GMT
WORKDIR /spiped
# Tue, 05 Apr 2022 15:38:52 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 05 Apr 2022 15:38:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 05 Apr 2022 15:38:53 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:57fb4b5f1a47c953ca5703f0f81ce14e5d01cf23aa79558b5adb961cc526e320`  
		Last Modified: Mon, 04 Apr 2022 19:09:36 GMT  
		Size: 2.4 MB (2424323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c34bb3a817bf019eff75e990b3ee9f75b0d33a5070d140d69adcd81bc3c61d4`  
		Last Modified: Tue, 05 Apr 2022 15:39:47 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50ddc3edc7d50bace02b581239b3d2096bbdd43b8d5cca77199c023788b7bab9`  
		Last Modified: Tue, 05 Apr 2022 15:39:47 GMT  
		Size: 7.8 KB (7779 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e4b14e7f868497bf35a981b97fa3d6c40d44c373e6207c0e73aa3292319b6e8`  
		Last Modified: Tue, 05 Apr 2022 15:39:47 GMT  
		Size: 192.7 KB (192698 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c22a92e8f54240f73e546662dc34d0aa6b83ec1617f18fa8e178c93138c0b72e`  
		Last Modified: Tue, 05 Apr 2022 15:39:47 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98ad3607e9857b6fb1bb4fbf10d6e9ed9e787343edd64901dc0ecaadd3ff55db`  
		Last Modified: Tue, 05 Apr 2022 15:39:47 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:6b7fd2442f6dcd71561982dfb157122343a4c720493a891274c64d2c577ce4ab
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 MB (2933135 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8dc39b7901f2654c939cb1c1d44ff3a6e036a4bcf2cef396786768da4de2f658`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Mon, 04 Apr 2022 23:39:31 GMT
ADD file:90e56af13188c7f0283d244a0d70b853d8bef8587a41f1da8eac3a2aba8964ef in / 
# Mon, 04 Apr 2022 23:39:31 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 14:38:03 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Tue, 05 Apr 2022 14:38:04 GMT
RUN apk add --no-cache libssl1.1
# Tue, 05 Apr 2022 14:38:05 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 05 Apr 2022 14:38:15 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Tue, 05 Apr 2022 14:38:16 GMT
VOLUME [/spiped]
# Tue, 05 Apr 2022 14:38:17 GMT
WORKDIR /spiped
# Tue, 05 Apr 2022 14:38:19 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 05 Apr 2022 14:38:19 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 05 Apr 2022 14:38:20 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:9981e73032c8833e387a8f96986e560edbed12c38119e0edb0439c9c2234eac9`  
		Last Modified: Mon, 04 Apr 2022 19:09:10 GMT  
		Size: 2.7 MB (2716477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe4c0758a179cd25e16e078f253517cd4f315287416c3ce781a852e456da3093`  
		Last Modified: Tue, 05 Apr 2022 14:38:47 GMT  
		Size: 1.2 KB (1240 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ad68b994955132db089d9decfe3c1abb1e0d937a743641a82ff97b1ad0de230`  
		Last Modified: Tue, 05 Apr 2022 14:38:47 GMT  
		Size: 7.7 KB (7749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2412b85fbb446b18863d0276c285a9f15c5506327e253be647ba7c7e323d01e0`  
		Last Modified: Tue, 05 Apr 2022 14:38:47 GMT  
		Size: 207.2 KB (207235 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff9b28798cece086f58205831a8c06e9be4d79eb185eb2a5566b692c6bb0aa1f`  
		Last Modified: Tue, 05 Apr 2022 14:38:47 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9aa51b8e1739c24bc53b08bbda05fba07af4b69550a9c5ac36ea5be1bb7d5b1`  
		Last Modified: Tue, 05 Apr 2022 14:38:47 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; 386

```console
$ docker pull spiped@sha256:dcbb93128deb3206337ac10573e41e27b4a95816cd3f931412c655201fef2396
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.1 MB (3053817 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fdb9526919356b65e45d7bc9a9bd2aaddd7da8a1e62f023b9511a320a431df64`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Mon, 04 Apr 2022 23:38:25 GMT
ADD file:7d51a0f8691eb78c9062fd31984423a93d276a67b4ed5d1a706e1c2cd9fea23a in / 
# Mon, 04 Apr 2022 23:38:25 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 06:51:23 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Tue, 05 Apr 2022 06:51:24 GMT
RUN apk add --no-cache libssl1.1
# Tue, 05 Apr 2022 06:51:24 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 05 Apr 2022 06:51:34 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Tue, 05 Apr 2022 06:51:35 GMT
VOLUME [/spiped]
# Tue, 05 Apr 2022 06:51:36 GMT
WORKDIR /spiped
# Tue, 05 Apr 2022 06:51:38 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 05 Apr 2022 06:51:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 05 Apr 2022 06:51:39 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:73b28a5955ec7fb46f2cf0434e4901a889f7dda3f8c9ec496300feb256c7eda8`  
		Last Modified: Mon, 04 Apr 2022 19:10:03 GMT  
		Size: 2.8 MB (2818974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5043c44edf55100d2df153f657912b53abf987ef0c6286b113dcef298998f359`  
		Last Modified: Tue, 05 Apr 2022 06:52:09 GMT  
		Size: 1.2 KB (1240 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfc9d36e654ea336dd74dc00574768a6502edd5ef5cd785b695e516f6254be55`  
		Last Modified: Tue, 05 Apr 2022 06:52:08 GMT  
		Size: 7.8 KB (7750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0401735f1a5cdc5a0248a778049579b8858a6f7cc0fc6fdcdaea211930d4a386`  
		Last Modified: Tue, 05 Apr 2022 06:52:08 GMT  
		Size: 225.4 KB (225416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5a85e3f263e110e3fa50aada2a3ca6314a5a6e67e8f211881a826585a5db409`  
		Last Modified: Tue, 05 Apr 2022 06:52:08 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a0f113efbe13d3511b57cb0428e99f2725a51cb3980e75b1f1be3fc0d715b19`  
		Last Modified: Tue, 05 Apr 2022 06:52:08 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; ppc64le

```console
$ docker pull spiped@sha256:6d1206f429c5113ac4fbd6820b913ec32aa3cb826c65e5446d05eb57c3bfd7f4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (3033860 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:64a17da88fc17c158a4b17b8a85a6b534482d5b9fe198bee0a961886519d4811`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 05 Apr 2022 00:23:30 GMT
ADD file:960cf6f9d3d1cfcb36c2d67dd4c3eaba7db1d0c7afe97968512248d7f234ad47 in / 
# Tue, 05 Apr 2022 00:23:32 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 20:07:37 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Tue, 05 Apr 2022 20:08:01 GMT
RUN apk add --no-cache libssl1.1
# Tue, 05 Apr 2022 20:08:06 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 05 Apr 2022 20:08:35 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Tue, 05 Apr 2022 20:08:41 GMT
VOLUME [/spiped]
# Tue, 05 Apr 2022 20:08:46 GMT
WORKDIR /spiped
# Tue, 05 Apr 2022 20:08:48 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 05 Apr 2022 20:08:49 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 05 Apr 2022 20:08:52 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:1877acf2d48ed8bcb5bd9756a95aca0c077457be7cf4fcef25807f4e9be88db1`  
		Last Modified: Mon, 04 Apr 2022 19:09:49 GMT  
		Size: 2.8 MB (2811186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:898122ed2d1fcbc53be831191766c1b47d98b8cb2251d70dcc91e5ecad3bf34e`  
		Last Modified: Tue, 05 Apr 2022 20:09:25 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0cdc12b8854b22d6407eaece31ad74f6d0d2f322236c0d02a0074aef7944b93`  
		Last Modified: Tue, 05 Apr 2022 20:09:25 GMT  
		Size: 7.8 KB (7771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc1f84e0deee708d9995b37beb5b3923a9091dcc0ee670f7d784de701af40e2e`  
		Last Modified: Tue, 05 Apr 2022 20:09:25 GMT  
		Size: 213.2 KB (213160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67c77cab4a7338ba5a131c568ed153eb1fd0151dbb6108fae4fd3234a699f6ac`  
		Last Modified: Tue, 05 Apr 2022 20:09:25 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e03666b6f800b3362553b44e783b6eff051c84c4ae25bdb3d1da279626fc8bb9`  
		Last Modified: Tue, 05 Apr 2022 20:09:25 GMT  
		Size: 345.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6-alpine` - linux; s390x

```console
$ docker pull spiped@sha256:851d4d1e8b82de6d455e9a562bd6b75539fe737213c9f3cf01ce7b44e11abeb4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 MB (2811594 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e240f56e6000d053b4d3e20632b54b88daaa8dad76ecda720ce9f76c82bfe394`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Mon, 04 Apr 2022 23:41:39 GMT
ADD file:f22e4b2be87d3c59c8c609acf79015938dc1fba0b26d7c1b59bd0fc36d63a906 in / 
# Mon, 04 Apr 2022 23:41:39 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 06:09:44 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Tue, 05 Apr 2022 06:09:45 GMT
RUN apk add --no-cache libssl1.1
# Tue, 05 Apr 2022 06:09:45 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 05 Apr 2022 06:09:50 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Tue, 05 Apr 2022 06:09:50 GMT
VOLUME [/spiped]
# Tue, 05 Apr 2022 06:09:51 GMT
WORKDIR /spiped
# Tue, 05 Apr 2022 06:09:51 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 05 Apr 2022 06:09:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 05 Apr 2022 06:09:51 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:a27b630f446c3da376a30cf610e4bfa6847f8b87c83702c29e72b986f4e52d28`  
		Last Modified: Mon, 04 Apr 2022 23:42:37 GMT  
		Size: 2.6 MB (2600375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ffc8ec477cbe2d575e99a9232e9328db8cc40109dbe067d93c2033302576850`  
		Last Modified: Tue, 05 Apr 2022 06:10:22 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ee008c7ec71319091cda7b7cbf1063414ee758f739581409a2e7089e90882c9`  
		Last Modified: Tue, 05 Apr 2022 06:10:21 GMT  
		Size: 7.8 KB (7788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3edcb5212f084eabfd1bad6e332d8b53bd7756099c4da3e410ee23f869a701b`  
		Last Modified: Tue, 05 Apr 2022 06:10:21 GMT  
		Size: 201.7 KB (201693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd099e1efb05ce5fa06c5e18ba7d057b5df318c462022f1ac443f45e86fdc809`  
		Last Modified: Tue, 05 Apr 2022 06:10:21 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afbab95e29c022d6828d869e5e4442b139373571c747f8fc6470b8bd257337a4`  
		Last Modified: Tue, 05 Apr 2022 06:10:21 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:1.6.2`

```console
$ docker pull spiped@sha256:7a1276ab6a9bd4e55b8313b8cd13c2feabdc32369f047a82db7b499c42206a14
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
$ docker pull spiped@sha256:a66911a787746637e44a865f64e731ea404d2266efa5d987ee58d6d535a3999b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.3 MB (37349901 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4b801341ea8d054b7b965f35306e02a25be57d78de5177ed30cfb7af2b0267b7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 11 May 2022 01:20:16 GMT
ADD file:4a0bb88956083aa56032fdd9601d9b66c39b18c896ba35ea33594cd75621640a in / 
# Wed, 11 May 2022 01:20:16 GMT
CMD ["bash"]
# Wed, 11 May 2022 09:31:09 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 11 May 2022 09:31:12 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 09:31:12 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 11 May 2022 09:31:32 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 11 May 2022 09:31:32 GMT
VOLUME [/spiped]
# Wed, 11 May 2022 09:31:32 GMT
WORKDIR /spiped
# Wed, 11 May 2022 09:31:32 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 11 May 2022 09:31:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 11 May 2022 09:31:32 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:214ca5fb90323fe769c63a12af092f2572bf1c6b300263e09883909fc865d260`  
		Last Modified: Wed, 11 May 2022 01:25:13 GMT  
		Size: 31.4 MB (31379476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:080576f9a12bf8fca30a9653a7d9a0772acec767c26a2330bcdd92e5be0cfe95`  
		Last Modified: Wed, 11 May 2022 09:31:50 GMT  
		Size: 1.7 KB (1732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38bcb584eb7cb0f5bd593db63ab12b7b34bea2aa958fde7434a9b859ec903c08`  
		Last Modified: Wed, 11 May 2022 09:31:49 GMT  
		Size: 1.1 KB (1051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5664b9af48e8dd5dd00adb4691215c987017dbdb64998cdc9c30c22786d136d`  
		Last Modified: Wed, 11 May 2022 09:31:51 GMT  
		Size: 6.0 MB (5967174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6affb70c27746eb9c197393a54cd9b606353628e04424d0b4935ac195b6674a`  
		Last Modified: Wed, 11 May 2022 09:31:49 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01cd4accaf294c916a8ef636747fa575dbaa0f547f8bd5c7001c0112a9507dc2`  
		Last Modified: Wed, 11 May 2022 09:31:49 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.2` - linux; arm variant v5

```console
$ docker pull spiped@sha256:6b56704713f5efb9e393f0c751fe4e3ecfc3762033496269972dbb442a70972d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.0 MB (33952053 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6b14d990d1127fdf382852ac149cf58dd872a968df8176e8a74a5778ea0738c1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 11 May 2022 00:50:34 GMT
ADD file:72357b75d7e4546f06abf4648ab600980e742a3017f36da3c7a6c086f2f5fb56 in / 
# Wed, 11 May 2022 00:50:35 GMT
CMD ["bash"]
# Thu, 12 May 2022 01:35:14 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Thu, 12 May 2022 01:35:23 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Thu, 12 May 2022 01:35:23 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 12 May 2022 01:36:14 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 12 May 2022 01:36:15 GMT
VOLUME [/spiped]
# Thu, 12 May 2022 01:36:15 GMT
WORKDIR /spiped
# Thu, 12 May 2022 01:36:16 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 12 May 2022 01:36:16 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 12 May 2022 01:36:17 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:f7b69be15db1cb94a249f74b27edd4f5e5923a8701b026179a593f6888e897aa`  
		Last Modified: Wed, 11 May 2022 01:05:51 GMT  
		Size: 28.9 MB (28921122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a5a9157aa645038e20cfd8d939540308935a2f448009504b4b50f55ebe7fcc8`  
		Last Modified: Thu, 12 May 2022 01:36:50 GMT  
		Size: 1.7 KB (1725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:379d8521d9bd468b1d6a357f9682b3e0efc683bb7ce8c61b98639d89a6e5a9d3`  
		Last Modified: Thu, 12 May 2022 01:36:50 GMT  
		Size: 1.1 KB (1050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94258b91da89ba5bcfb0b99e7a7224030f4fbc734a79e19488d7b2e198797278`  
		Last Modified: Thu, 12 May 2022 01:36:55 GMT  
		Size: 5.0 MB (5027685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8ecd42d03f9650c45b9f15fb17188211b89f7ea6683a8aa6d8cf3ea08653577`  
		Last Modified: Thu, 12 May 2022 01:36:50 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82055141d6a68a71687d6ce1c4aa739a9d6fa527bf54e1eb9120550413add7ea`  
		Last Modified: Thu, 12 May 2022 01:36:50 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.2` - linux; arm variant v7

```console
$ docker pull spiped@sha256:426553dc9b38cdd633ce43cdf604b956d3d21c098bc256d936f9154132930908
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.3 MB (31327127 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7e6ef92e514ca9a3a7a716f84914ba360321d707df4255203a53390721630843`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 11 May 2022 01:49:07 GMT
ADD file:7c0451fffe8a520c2ab23048948d76bfe0dc0d90298c3d859279ccd8815b84f6 in / 
# Wed, 11 May 2022 01:49:08 GMT
CMD ["bash"]
# Thu, 12 May 2022 09:57:40 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Thu, 12 May 2022 09:57:47 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Thu, 12 May 2022 09:57:48 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 12 May 2022 09:58:33 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 12 May 2022 09:58:34 GMT
VOLUME [/spiped]
# Thu, 12 May 2022 09:58:34 GMT
WORKDIR /spiped
# Thu, 12 May 2022 09:58:35 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 12 May 2022 09:58:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 12 May 2022 09:58:36 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:1a9427b75b1c1db800cae7a9199bb4e508702e6761b17cc904d21441df43016c`  
		Last Modified: Wed, 11 May 2022 02:04:35 GMT  
		Size: 26.6 MB (26575672 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:666c704c2d2710e68360474f0cd959985e4418ee1bf3da5f69155679a1aae5e3`  
		Last Modified: Thu, 12 May 2022 09:59:35 GMT  
		Size: 1.7 KB (1736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:997d8d681765c85ae870076561eed251de76347cf9bf8d4fe9ca8bea5ee94d7e`  
		Last Modified: Thu, 12 May 2022 09:59:36 GMT  
		Size: 1.1 KB (1051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:666b40dc8c26e1e531689caf804a1d968693ea152f3580588acd62cd67aba309`  
		Last Modified: Thu, 12 May 2022 09:59:39 GMT  
		Size: 4.7 MB (4748197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d352d4363ba035dd50fa29f21ce08e12bdee48d3e9801fad5ae5d27d2e842c2`  
		Last Modified: Thu, 12 May 2022 09:59:35 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe1a6862d97ef70fbc74954b3f2e128027ea3142115032009c75b79794fedebb`  
		Last Modified: Thu, 12 May 2022 09:59:35 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.2` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:572906adb8bf287a02331ed2dc6b70d40c1795ce56eb514a7b873ac8b0b07782
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.3 MB (35339551 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:df8ebf44dc7acf424cbe762be8778cd542ccc7006e183a616763d3b92f5af2cc`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 11 May 2022 00:46:59 GMT
ADD file:158a0e401328bd7c0d49b9e8539186098967218f1b1a8c811f4398d29b74397f in / 
# Wed, 11 May 2022 00:47:00 GMT
CMD ["bash"]
# Wed, 11 May 2022 12:24:33 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 11 May 2022 12:24:36 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 12:24:37 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 11 May 2022 12:24:55 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 11 May 2022 12:24:56 GMT
VOLUME [/spiped]
# Wed, 11 May 2022 12:24:57 GMT
WORKDIR /spiped
# Wed, 11 May 2022 12:24:59 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 11 May 2022 12:24:59 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 11 May 2022 12:25:00 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:dfdd5ffb257742b891ccad9400a77dad2a6260b2451e0f5e48a9ade1d17a87ec`  
		Last Modified: Wed, 11 May 2022 00:53:46 GMT  
		Size: 30.1 MB (30065693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e25366de1af948b0eef7cad0d0d1fbc56648a743854da03fc57dc121c2384213`  
		Last Modified: Wed, 11 May 2022 12:25:32 GMT  
		Size: 1.6 KB (1621 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aef033e02dd13ee59e5336850b85b81cbd2ccd353a033415114d010d6a8254df`  
		Last Modified: Wed, 11 May 2022 12:25:32 GMT  
		Size: 922.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dac510a96382ea09a86f8f4cadc73653a8177516d4771a4a7e3bccbdeeb326de`  
		Last Modified: Wed, 11 May 2022 12:25:33 GMT  
		Size: 5.3 MB (5270881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1616a14c0096a1c7108f1fe3372296010619c2f7c502e1802e6d3855dfdf0ebd`  
		Last Modified: Wed, 11 May 2022 12:25:32 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcaa87e60ef72bc3e5eab8bd8a81a9cee650735736cd7c760f4366260b5461d2`  
		Last Modified: Wed, 11 May 2022 12:25:32 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.2` - linux; 386

```console
$ docker pull spiped@sha256:d933a3ef2f835e9d32f01babb2f55693ab6f3b2150d76a4e72d6fdec66739208
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.3 MB (40284215 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8994e3dd3df7e9fdbd0d51ca1e620fa69f6efd232ff5d5d2b381cd6b22fbc13c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 11 May 2022 01:39:14 GMT
ADD file:9eecb0fd311177f9d226e914c411aef49b5de1930e73019d2ee24afed515b5a2 in / 
# Wed, 11 May 2022 01:39:14 GMT
CMD ["bash"]
# Wed, 11 May 2022 15:51:27 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 11 May 2022 15:51:30 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 15:51:31 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 11 May 2022 15:51:52 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 11 May 2022 15:51:52 GMT
VOLUME [/spiped]
# Wed, 11 May 2022 15:51:53 GMT
WORKDIR /spiped
# Wed, 11 May 2022 15:51:55 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 11 May 2022 15:51:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 11 May 2022 15:51:56 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:91c5bdbe4bf9f1970dd54ba71e2523649adce4e5240c2ff8a87711bf389ecba3`  
		Last Modified: Wed, 11 May 2022 01:46:25 GMT  
		Size: 32.4 MB (32389776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa9bc810ed14e83b2b6c2de848151a8aac3442608851df4e4ba4f35402048a54`  
		Last Modified: Wed, 11 May 2022 15:52:27 GMT  
		Size: 1.6 KB (1608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ddd23897c0dc65364a8fda9129fe87c608a02ac54bdd3002e70407c7dff7b8a`  
		Last Modified: Wed, 11 May 2022 15:52:27 GMT  
		Size: 923.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a55bc0fd5c56c871a37888a72d560d40d0364889e86b54c791bea4bb7c85887`  
		Last Modified: Wed, 11 May 2022 15:52:28 GMT  
		Size: 7.9 MB (7891471 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad4fc1778cbfb42cc882687278e3d3bb64b10572a3b56cf12d7ba9b128537d21`  
		Last Modified: Wed, 11 May 2022 15:52:27 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cc951e82cef08be37b45eba1592c940f1a946d625884f3e80794061addeb20a`  
		Last Modified: Wed, 11 May 2022 15:52:27 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.2` - linux; mips64le

```console
$ docker pull spiped@sha256:98dafc6cf00b4ae4723240a88ce5bed8cc462c78e6e05aa1fdea9727db128735
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.3 MB (35349146 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:008c2d2ba6ac1949b574aa0cd913d936ebd6fadc503e85c425e3052ef113387d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 11 May 2022 02:23:35 GMT
ADD file:d47dce2adbc9352ef1d437730bab3b579dd8d2bf29dd60cd8a8b65396b39e36e in / 
# Wed, 11 May 2022 02:23:40 GMT
CMD ["bash"]
# Thu, 12 May 2022 04:11:52 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Thu, 12 May 2022 04:12:07 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Thu, 12 May 2022 04:12:09 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 12 May 2022 04:13:33 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 12 May 2022 04:13:36 GMT
VOLUME [/spiped]
# Thu, 12 May 2022 04:13:39 GMT
WORKDIR /spiped
# Thu, 12 May 2022 04:13:41 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 12 May 2022 04:13:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 12 May 2022 04:13:46 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:438a36bf0b6e75ff6f0fbb2b7669dfb86361416f4d808912d30cf5b91ad2eea9`  
		Last Modified: Wed, 11 May 2022 02:33:43 GMT  
		Size: 29.6 MB (29641051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b968eb568ff8a2acb36380ccbf842b116d8f7251fe76b4d4c05350e872efe8f`  
		Last Modified: Thu, 12 May 2022 04:14:11 GMT  
		Size: 1.6 KB (1614 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e0c58081df5c4242f571acbbce6534a045404bc2c44eab75dbe2bfa721606fc`  
		Last Modified: Thu, 12 May 2022 04:14:11 GMT  
		Size: 925.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2c0fc303ca2ffd0acaaa4421f936b6d1cdcbd87e50ae67c64e5d2f003a022f8`  
		Last Modified: Thu, 12 May 2022 04:14:16 GMT  
		Size: 5.7 MB (5705117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a84b67927c5aea3805e90f18768e6338fd392e91c3618805526b3ff7c776b824`  
		Last Modified: Thu, 12 May 2022 04:14:11 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c4229b76d1a9cdc6812c0c3734a7d00ca0f098edeb70043fce974697a9d2a4c`  
		Last Modified: Thu, 12 May 2022 04:14:11 GMT  
		Size: 344.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.2` - linux; ppc64le

```console
$ docker pull spiped@sha256:e338e5b4a068b2c06d20548b51e98cf9e6711b5ba3f91a55f33517103107db26
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.3 MB (41288815 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:54eb4238d8977094c460b01a31bf18ab2865f97d34da09adaf33454df8e1a99f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 11 May 2022 01:32:29 GMT
ADD file:1e94716789ec21981460f74be38a668bc212bd804c1d41cecf90036a5bccac5a in / 
# Wed, 11 May 2022 01:32:34 GMT
CMD ["bash"]
# Wed, 11 May 2022 14:18:46 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 11 May 2022 14:18:57 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 14:19:00 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 11 May 2022 14:21:35 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 11 May 2022 14:21:45 GMT
VOLUME [/spiped]
# Wed, 11 May 2022 14:21:59 GMT
WORKDIR /spiped
# Wed, 11 May 2022 14:22:09 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 11 May 2022 14:22:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 11 May 2022 14:22:21 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:2533109ed11eefd6415e0370d6d7a3ea879b582b1887c98b819a598ad18fca24`  
		Last Modified: Wed, 11 May 2022 01:43:03 GMT  
		Size: 35.3 MB (35286467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e371d58c256a557b6f8f7b903d8a39345ccc364236516cb3ec208e9e40e92c5`  
		Last Modified: Wed, 11 May 2022 14:23:02 GMT  
		Size: 1.7 KB (1743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b4caf1ad053d6d5585c461ca9b8d4c6a14a963b94b0d13bb0594b2244f15a8b`  
		Last Modified: Wed, 11 May 2022 14:23:02 GMT  
		Size: 1.1 KB (1054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb23602e10ec58354d8276b2a6d7549e7f11c523d76e28603f149ca4c0e1e951`  
		Last Modified: Wed, 11 May 2022 14:23:04 GMT  
		Size: 6.0 MB (5999080 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fa6bf1315149ea1738416c3df58107d0e9c60aae5cb546cfdcbb50aa6855062`  
		Last Modified: Wed, 11 May 2022 14:23:02 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82539badabc1522bce1e3acd0e092aceb9818dd6904d2ab5fe8a10ab39a0f6b5`  
		Last Modified: Wed, 11 May 2022 14:23:02 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.2` - linux; s390x

```console
$ docker pull spiped@sha256:a2261239d98aaef54af72737a4aa30c1a01f4089439604c977e606d06e5eb317
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.8 MB (34844727 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d218c6ec1b1cc03c92a160497f19dc4deed41827aaf7bef061ddc8ca4c8f6fac`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 11 May 2022 00:44:17 GMT
ADD file:d93a1cf64a813d01774cd628dfd683c006e20159e2ab3464c2159c8d9897c725 in / 
# Wed, 11 May 2022 00:44:19 GMT
CMD ["bash"]
# Wed, 11 May 2022 06:26:51 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 11 May 2022 06:26:54 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 06:26:54 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 11 May 2022 06:27:06 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 11 May 2022 06:27:07 GMT
VOLUME [/spiped]
# Wed, 11 May 2022 06:27:07 GMT
WORKDIR /spiped
# Wed, 11 May 2022 06:27:07 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 11 May 2022 06:27:07 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 11 May 2022 06:27:07 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:9f3750f6094217808e26d471752341db88153c8d5b5f9bb11577b74671303bbc`  
		Last Modified: Wed, 11 May 2022 00:50:03 GMT  
		Size: 29.7 MB (29654739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:873c48057acd3a3e859a48bcca0c21842c182414ce09c34a3cc1c1886f7de52a`  
		Last Modified: Wed, 11 May 2022 06:27:39 GMT  
		Size: 1.7 KB (1734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09c3eb03701aaff2a58238f35a586fbc044102b129292492a02c7479e57440b3`  
		Last Modified: Wed, 11 May 2022 06:27:39 GMT  
		Size: 1.1 KB (1052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c22498c1d73103d486b8e69a684b02839606786d6cff45d0dfbdbdc6e26ce68c`  
		Last Modified: Wed, 11 May 2022 06:27:40 GMT  
		Size: 5.2 MB (5186734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6758dfdb3a7588b70d2a3af8806cc9cea3dee7221cfe99f32973d6c0eee71d46`  
		Last Modified: Wed, 11 May 2022 06:27:39 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6fcc234dd9c90350b33b0e204d793aec0e7ee86952bb815ce76739eced0d2a7`  
		Last Modified: Wed, 11 May 2022 06:27:39 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:1.6.2-alpine`

```console
$ docker pull spiped@sha256:e803772f3cd77bd5eb74c25cebf7dbe58c1490172affec2756736f01297e2ad6
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
$ docker pull spiped@sha256:b1000f43786f16a20a805fa353f6e29da279735ce16fc397001fde0e351cadab
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (3038963 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:319549bf17a1c296f365e261889f2573a629fda0ca36fa2dac3efc79c233dc4d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 05 Apr 2022 00:19:59 GMT
ADD file:5d673d25da3a14ce1f6cf66e4c7fd4f4b85a3759a9d93efb3fd9ff852b5b56e4 in / 
# Tue, 05 Apr 2022 00:19:59 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 09:41:12 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Tue, 05 Apr 2022 09:41:13 GMT
RUN apk add --no-cache libssl1.1
# Tue, 05 Apr 2022 09:41:13 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 05 Apr 2022 09:41:22 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Tue, 05 Apr 2022 09:41:22 GMT
VOLUME [/spiped]
# Tue, 05 Apr 2022 09:41:23 GMT
WORKDIR /spiped
# Tue, 05 Apr 2022 09:41:23 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 05 Apr 2022 09:41:23 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 05 Apr 2022 09:41:23 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:df9b9388f04ad6279a7410b85cedfdcb2208c0a003da7ab5613af71079148139`  
		Last Modified: Mon, 04 Apr 2022 19:10:16 GMT  
		Size: 2.8 MB (2814559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:735044c06e8b73c2bb88467804d54b359bfc8226cf975772cc666adc9f029f5c`  
		Last Modified: Tue, 05 Apr 2022 09:41:38 GMT  
		Size: 1.3 KB (1271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd8b16fcaec70a3de42b4e850be4a851eaffa96a04fb49668b0d55b15bdf9675`  
		Last Modified: Tue, 05 Apr 2022 09:41:38 GMT  
		Size: 7.8 KB (7783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79236b25532d68c328b81af71a0f8c4eca102b7030a98d650ffc9a7e35d113be`  
		Last Modified: Tue, 05 Apr 2022 09:41:38 GMT  
		Size: 214.9 KB (214880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f429bef29fed68fb012179a10893c62fd5167934a7d62e7d3db15361601d47e9`  
		Last Modified: Tue, 05 Apr 2022 09:41:38 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1703108ce26f514d42179cf03051a6082b57e184d89f7bab08377819025c74d9`  
		Last Modified: Tue, 05 Apr 2022 09:41:38 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.2-alpine` - linux; arm variant v6

```console
$ docker pull spiped@sha256:44fa18e7d3af978bedc72ce9110a2217004554deec585dfcdafffb4c761a1661
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 MB (2830637 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b21bdc008b33d69d3d83d8292f28384b56c4166b1ef0c3f5c05eac33a48df2a7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Mon, 04 Apr 2022 23:49:42 GMT
ADD file:159dcddaab900372df882a4e94615ed84250e9cea3e74bc0479d98280342f596 in / 
# Mon, 04 Apr 2022 23:49:42 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 11:42:28 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Tue, 05 Apr 2022 11:42:30 GMT
RUN apk add --no-cache libssl1.1
# Tue, 05 Apr 2022 11:42:30 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 05 Apr 2022 11:42:49 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Tue, 05 Apr 2022 11:42:50 GMT
VOLUME [/spiped]
# Tue, 05 Apr 2022 11:42:50 GMT
WORKDIR /spiped
# Tue, 05 Apr 2022 11:42:51 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 05 Apr 2022 11:42:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 05 Apr 2022 11:42:52 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:c319b1fc4ed70b8241a7ce6ac0c4015d354bf5cf8c01eb73c50b6709c0c46e49`  
		Last Modified: Mon, 04 Apr 2022 19:09:22 GMT  
		Size: 2.6 MB (2621972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b279880cad38890c6b22622a3cecb67733556ec9965319ffa327afec8900ad3`  
		Last Modified: Tue, 05 Apr 2022 11:43:27 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27045425770040b89c6aeadebc232d3bd49690ccc505ec5a20336cbfa650b899`  
		Last Modified: Tue, 05 Apr 2022 11:43:27 GMT  
		Size: 7.8 KB (7767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfe17e03d9a44e0c737a4484821d473ab6476046270059fab5ebad88fdbfcce7`  
		Last Modified: Tue, 05 Apr 2022 11:43:27 GMT  
		Size: 199.2 KB (199161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2979a2148a9f161c6f6ae02c8bdc6b41f1f18da7a66d2db5addec2e19752388b`  
		Last Modified: Tue, 05 Apr 2022 11:43:26 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5863282bd4052a3bc2b39bb2d4cc46b864b2e4214edba85c572e7f55f95d7ee1`  
		Last Modified: Tue, 05 Apr 2022 11:43:26 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.2-alpine` - linux; arm variant v7

```console
$ docker pull spiped@sha256:41ea58744c279880bd672731168c41728c367a5558010a8b15109a53651aed8b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 MB (2626540 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fa3a26053023e3df6fe0ab2fdfc9b5c0e7806a837bdf8aeeebed934566092f5f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Mon, 04 Apr 2022 23:57:34 GMT
ADD file:20f8cdddc53a4a8bd78945fc32fe08e9f80ab3b16dc20a9aa4ba73b79f2bc71c in / 
# Mon, 04 Apr 2022 23:57:35 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 15:38:30 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Tue, 05 Apr 2022 15:38:32 GMT
RUN apk add --no-cache libssl1.1
# Tue, 05 Apr 2022 15:38:33 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 05 Apr 2022 15:38:51 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Tue, 05 Apr 2022 15:38:51 GMT
VOLUME [/spiped]
# Tue, 05 Apr 2022 15:38:52 GMT
WORKDIR /spiped
# Tue, 05 Apr 2022 15:38:52 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 05 Apr 2022 15:38:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 05 Apr 2022 15:38:53 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:57fb4b5f1a47c953ca5703f0f81ce14e5d01cf23aa79558b5adb961cc526e320`  
		Last Modified: Mon, 04 Apr 2022 19:09:36 GMT  
		Size: 2.4 MB (2424323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c34bb3a817bf019eff75e990b3ee9f75b0d33a5070d140d69adcd81bc3c61d4`  
		Last Modified: Tue, 05 Apr 2022 15:39:47 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50ddc3edc7d50bace02b581239b3d2096bbdd43b8d5cca77199c023788b7bab9`  
		Last Modified: Tue, 05 Apr 2022 15:39:47 GMT  
		Size: 7.8 KB (7779 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e4b14e7f868497bf35a981b97fa3d6c40d44c373e6207c0e73aa3292319b6e8`  
		Last Modified: Tue, 05 Apr 2022 15:39:47 GMT  
		Size: 192.7 KB (192698 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c22a92e8f54240f73e546662dc34d0aa6b83ec1617f18fa8e178c93138c0b72e`  
		Last Modified: Tue, 05 Apr 2022 15:39:47 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98ad3607e9857b6fb1bb4fbf10d6e9ed9e787343edd64901dc0ecaadd3ff55db`  
		Last Modified: Tue, 05 Apr 2022 15:39:47 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.2-alpine` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:6b7fd2442f6dcd71561982dfb157122343a4c720493a891274c64d2c577ce4ab
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 MB (2933135 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8dc39b7901f2654c939cb1c1d44ff3a6e036a4bcf2cef396786768da4de2f658`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Mon, 04 Apr 2022 23:39:31 GMT
ADD file:90e56af13188c7f0283d244a0d70b853d8bef8587a41f1da8eac3a2aba8964ef in / 
# Mon, 04 Apr 2022 23:39:31 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 14:38:03 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Tue, 05 Apr 2022 14:38:04 GMT
RUN apk add --no-cache libssl1.1
# Tue, 05 Apr 2022 14:38:05 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 05 Apr 2022 14:38:15 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Tue, 05 Apr 2022 14:38:16 GMT
VOLUME [/spiped]
# Tue, 05 Apr 2022 14:38:17 GMT
WORKDIR /spiped
# Tue, 05 Apr 2022 14:38:19 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 05 Apr 2022 14:38:19 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 05 Apr 2022 14:38:20 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:9981e73032c8833e387a8f96986e560edbed12c38119e0edb0439c9c2234eac9`  
		Last Modified: Mon, 04 Apr 2022 19:09:10 GMT  
		Size: 2.7 MB (2716477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe4c0758a179cd25e16e078f253517cd4f315287416c3ce781a852e456da3093`  
		Last Modified: Tue, 05 Apr 2022 14:38:47 GMT  
		Size: 1.2 KB (1240 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ad68b994955132db089d9decfe3c1abb1e0d937a743641a82ff97b1ad0de230`  
		Last Modified: Tue, 05 Apr 2022 14:38:47 GMT  
		Size: 7.7 KB (7749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2412b85fbb446b18863d0276c285a9f15c5506327e253be647ba7c7e323d01e0`  
		Last Modified: Tue, 05 Apr 2022 14:38:47 GMT  
		Size: 207.2 KB (207235 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff9b28798cece086f58205831a8c06e9be4d79eb185eb2a5566b692c6bb0aa1f`  
		Last Modified: Tue, 05 Apr 2022 14:38:47 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9aa51b8e1739c24bc53b08bbda05fba07af4b69550a9c5ac36ea5be1bb7d5b1`  
		Last Modified: Tue, 05 Apr 2022 14:38:47 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.2-alpine` - linux; 386

```console
$ docker pull spiped@sha256:dcbb93128deb3206337ac10573e41e27b4a95816cd3f931412c655201fef2396
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.1 MB (3053817 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fdb9526919356b65e45d7bc9a9bd2aaddd7da8a1e62f023b9511a320a431df64`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Mon, 04 Apr 2022 23:38:25 GMT
ADD file:7d51a0f8691eb78c9062fd31984423a93d276a67b4ed5d1a706e1c2cd9fea23a in / 
# Mon, 04 Apr 2022 23:38:25 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 06:51:23 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Tue, 05 Apr 2022 06:51:24 GMT
RUN apk add --no-cache libssl1.1
# Tue, 05 Apr 2022 06:51:24 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 05 Apr 2022 06:51:34 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Tue, 05 Apr 2022 06:51:35 GMT
VOLUME [/spiped]
# Tue, 05 Apr 2022 06:51:36 GMT
WORKDIR /spiped
# Tue, 05 Apr 2022 06:51:38 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 05 Apr 2022 06:51:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 05 Apr 2022 06:51:39 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:73b28a5955ec7fb46f2cf0434e4901a889f7dda3f8c9ec496300feb256c7eda8`  
		Last Modified: Mon, 04 Apr 2022 19:10:03 GMT  
		Size: 2.8 MB (2818974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5043c44edf55100d2df153f657912b53abf987ef0c6286b113dcef298998f359`  
		Last Modified: Tue, 05 Apr 2022 06:52:09 GMT  
		Size: 1.2 KB (1240 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfc9d36e654ea336dd74dc00574768a6502edd5ef5cd785b695e516f6254be55`  
		Last Modified: Tue, 05 Apr 2022 06:52:08 GMT  
		Size: 7.8 KB (7750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0401735f1a5cdc5a0248a778049579b8858a6f7cc0fc6fdcdaea211930d4a386`  
		Last Modified: Tue, 05 Apr 2022 06:52:08 GMT  
		Size: 225.4 KB (225416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5a85e3f263e110e3fa50aada2a3ca6314a5a6e67e8f211881a826585a5db409`  
		Last Modified: Tue, 05 Apr 2022 06:52:08 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a0f113efbe13d3511b57cb0428e99f2725a51cb3980e75b1f1be3fc0d715b19`  
		Last Modified: Tue, 05 Apr 2022 06:52:08 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.2-alpine` - linux; ppc64le

```console
$ docker pull spiped@sha256:6d1206f429c5113ac4fbd6820b913ec32aa3cb826c65e5446d05eb57c3bfd7f4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (3033860 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:64a17da88fc17c158a4b17b8a85a6b534482d5b9fe198bee0a961886519d4811`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 05 Apr 2022 00:23:30 GMT
ADD file:960cf6f9d3d1cfcb36c2d67dd4c3eaba7db1d0c7afe97968512248d7f234ad47 in / 
# Tue, 05 Apr 2022 00:23:32 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 20:07:37 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Tue, 05 Apr 2022 20:08:01 GMT
RUN apk add --no-cache libssl1.1
# Tue, 05 Apr 2022 20:08:06 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 05 Apr 2022 20:08:35 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Tue, 05 Apr 2022 20:08:41 GMT
VOLUME [/spiped]
# Tue, 05 Apr 2022 20:08:46 GMT
WORKDIR /spiped
# Tue, 05 Apr 2022 20:08:48 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 05 Apr 2022 20:08:49 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 05 Apr 2022 20:08:52 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:1877acf2d48ed8bcb5bd9756a95aca0c077457be7cf4fcef25807f4e9be88db1`  
		Last Modified: Mon, 04 Apr 2022 19:09:49 GMT  
		Size: 2.8 MB (2811186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:898122ed2d1fcbc53be831191766c1b47d98b8cb2251d70dcc91e5ecad3bf34e`  
		Last Modified: Tue, 05 Apr 2022 20:09:25 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0cdc12b8854b22d6407eaece31ad74f6d0d2f322236c0d02a0074aef7944b93`  
		Last Modified: Tue, 05 Apr 2022 20:09:25 GMT  
		Size: 7.8 KB (7771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc1f84e0deee708d9995b37beb5b3923a9091dcc0ee670f7d784de701af40e2e`  
		Last Modified: Tue, 05 Apr 2022 20:09:25 GMT  
		Size: 213.2 KB (213160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67c77cab4a7338ba5a131c568ed153eb1fd0151dbb6108fae4fd3234a699f6ac`  
		Last Modified: Tue, 05 Apr 2022 20:09:25 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e03666b6f800b3362553b44e783b6eff051c84c4ae25bdb3d1da279626fc8bb9`  
		Last Modified: Tue, 05 Apr 2022 20:09:25 GMT  
		Size: 345.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:1.6.2-alpine` - linux; s390x

```console
$ docker pull spiped@sha256:851d4d1e8b82de6d455e9a562bd6b75539fe737213c9f3cf01ce7b44e11abeb4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 MB (2811594 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e240f56e6000d053b4d3e20632b54b88daaa8dad76ecda720ce9f76c82bfe394`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Mon, 04 Apr 2022 23:41:39 GMT
ADD file:f22e4b2be87d3c59c8c609acf79015938dc1fba0b26d7c1b59bd0fc36d63a906 in / 
# Mon, 04 Apr 2022 23:41:39 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 06:09:44 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Tue, 05 Apr 2022 06:09:45 GMT
RUN apk add --no-cache libssl1.1
# Tue, 05 Apr 2022 06:09:45 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 05 Apr 2022 06:09:50 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Tue, 05 Apr 2022 06:09:50 GMT
VOLUME [/spiped]
# Tue, 05 Apr 2022 06:09:51 GMT
WORKDIR /spiped
# Tue, 05 Apr 2022 06:09:51 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 05 Apr 2022 06:09:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 05 Apr 2022 06:09:51 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:a27b630f446c3da376a30cf610e4bfa6847f8b87c83702c29e72b986f4e52d28`  
		Last Modified: Mon, 04 Apr 2022 23:42:37 GMT  
		Size: 2.6 MB (2600375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ffc8ec477cbe2d575e99a9232e9328db8cc40109dbe067d93c2033302576850`  
		Last Modified: Tue, 05 Apr 2022 06:10:22 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ee008c7ec71319091cda7b7cbf1063414ee758f739581409a2e7089e90882c9`  
		Last Modified: Tue, 05 Apr 2022 06:10:21 GMT  
		Size: 7.8 KB (7788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3edcb5212f084eabfd1bad6e332d8b53bd7756099c4da3e410ee23f869a701b`  
		Last Modified: Tue, 05 Apr 2022 06:10:21 GMT  
		Size: 201.7 KB (201693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd099e1efb05ce5fa06c5e18ba7d057b5df318c462022f1ac443f45e86fdc809`  
		Last Modified: Tue, 05 Apr 2022 06:10:21 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afbab95e29c022d6828d869e5e4442b139373571c747f8fc6470b8bd257337a4`  
		Last Modified: Tue, 05 Apr 2022 06:10:21 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:alpine`

```console
$ docker pull spiped@sha256:e803772f3cd77bd5eb74c25cebf7dbe58c1490172affec2756736f01297e2ad6
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
$ docker pull spiped@sha256:b1000f43786f16a20a805fa353f6e29da279735ce16fc397001fde0e351cadab
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (3038963 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:319549bf17a1c296f365e261889f2573a629fda0ca36fa2dac3efc79c233dc4d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 05 Apr 2022 00:19:59 GMT
ADD file:5d673d25da3a14ce1f6cf66e4c7fd4f4b85a3759a9d93efb3fd9ff852b5b56e4 in / 
# Tue, 05 Apr 2022 00:19:59 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 09:41:12 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Tue, 05 Apr 2022 09:41:13 GMT
RUN apk add --no-cache libssl1.1
# Tue, 05 Apr 2022 09:41:13 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 05 Apr 2022 09:41:22 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Tue, 05 Apr 2022 09:41:22 GMT
VOLUME [/spiped]
# Tue, 05 Apr 2022 09:41:23 GMT
WORKDIR /spiped
# Tue, 05 Apr 2022 09:41:23 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 05 Apr 2022 09:41:23 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 05 Apr 2022 09:41:23 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:df9b9388f04ad6279a7410b85cedfdcb2208c0a003da7ab5613af71079148139`  
		Last Modified: Mon, 04 Apr 2022 19:10:16 GMT  
		Size: 2.8 MB (2814559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:735044c06e8b73c2bb88467804d54b359bfc8226cf975772cc666adc9f029f5c`  
		Last Modified: Tue, 05 Apr 2022 09:41:38 GMT  
		Size: 1.3 KB (1271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd8b16fcaec70a3de42b4e850be4a851eaffa96a04fb49668b0d55b15bdf9675`  
		Last Modified: Tue, 05 Apr 2022 09:41:38 GMT  
		Size: 7.8 KB (7783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79236b25532d68c328b81af71a0f8c4eca102b7030a98d650ffc9a7e35d113be`  
		Last Modified: Tue, 05 Apr 2022 09:41:38 GMT  
		Size: 214.9 KB (214880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f429bef29fed68fb012179a10893c62fd5167934a7d62e7d3db15361601d47e9`  
		Last Modified: Tue, 05 Apr 2022 09:41:38 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1703108ce26f514d42179cf03051a6082b57e184d89f7bab08377819025c74d9`  
		Last Modified: Tue, 05 Apr 2022 09:41:38 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; arm variant v6

```console
$ docker pull spiped@sha256:44fa18e7d3af978bedc72ce9110a2217004554deec585dfcdafffb4c761a1661
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 MB (2830637 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b21bdc008b33d69d3d83d8292f28384b56c4166b1ef0c3f5c05eac33a48df2a7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Mon, 04 Apr 2022 23:49:42 GMT
ADD file:159dcddaab900372df882a4e94615ed84250e9cea3e74bc0479d98280342f596 in / 
# Mon, 04 Apr 2022 23:49:42 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 11:42:28 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Tue, 05 Apr 2022 11:42:30 GMT
RUN apk add --no-cache libssl1.1
# Tue, 05 Apr 2022 11:42:30 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 05 Apr 2022 11:42:49 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Tue, 05 Apr 2022 11:42:50 GMT
VOLUME [/spiped]
# Tue, 05 Apr 2022 11:42:50 GMT
WORKDIR /spiped
# Tue, 05 Apr 2022 11:42:51 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 05 Apr 2022 11:42:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 05 Apr 2022 11:42:52 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:c319b1fc4ed70b8241a7ce6ac0c4015d354bf5cf8c01eb73c50b6709c0c46e49`  
		Last Modified: Mon, 04 Apr 2022 19:09:22 GMT  
		Size: 2.6 MB (2621972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b279880cad38890c6b22622a3cecb67733556ec9965319ffa327afec8900ad3`  
		Last Modified: Tue, 05 Apr 2022 11:43:27 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27045425770040b89c6aeadebc232d3bd49690ccc505ec5a20336cbfa650b899`  
		Last Modified: Tue, 05 Apr 2022 11:43:27 GMT  
		Size: 7.8 KB (7767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfe17e03d9a44e0c737a4484821d473ab6476046270059fab5ebad88fdbfcce7`  
		Last Modified: Tue, 05 Apr 2022 11:43:27 GMT  
		Size: 199.2 KB (199161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2979a2148a9f161c6f6ae02c8bdc6b41f1f18da7a66d2db5addec2e19752388b`  
		Last Modified: Tue, 05 Apr 2022 11:43:26 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5863282bd4052a3bc2b39bb2d4cc46b864b2e4214edba85c572e7f55f95d7ee1`  
		Last Modified: Tue, 05 Apr 2022 11:43:26 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; arm variant v7

```console
$ docker pull spiped@sha256:41ea58744c279880bd672731168c41728c367a5558010a8b15109a53651aed8b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 MB (2626540 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fa3a26053023e3df6fe0ab2fdfc9b5c0e7806a837bdf8aeeebed934566092f5f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Mon, 04 Apr 2022 23:57:34 GMT
ADD file:20f8cdddc53a4a8bd78945fc32fe08e9f80ab3b16dc20a9aa4ba73b79f2bc71c in / 
# Mon, 04 Apr 2022 23:57:35 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 15:38:30 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Tue, 05 Apr 2022 15:38:32 GMT
RUN apk add --no-cache libssl1.1
# Tue, 05 Apr 2022 15:38:33 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 05 Apr 2022 15:38:51 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Tue, 05 Apr 2022 15:38:51 GMT
VOLUME [/spiped]
# Tue, 05 Apr 2022 15:38:52 GMT
WORKDIR /spiped
# Tue, 05 Apr 2022 15:38:52 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 05 Apr 2022 15:38:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 05 Apr 2022 15:38:53 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:57fb4b5f1a47c953ca5703f0f81ce14e5d01cf23aa79558b5adb961cc526e320`  
		Last Modified: Mon, 04 Apr 2022 19:09:36 GMT  
		Size: 2.4 MB (2424323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c34bb3a817bf019eff75e990b3ee9f75b0d33a5070d140d69adcd81bc3c61d4`  
		Last Modified: Tue, 05 Apr 2022 15:39:47 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50ddc3edc7d50bace02b581239b3d2096bbdd43b8d5cca77199c023788b7bab9`  
		Last Modified: Tue, 05 Apr 2022 15:39:47 GMT  
		Size: 7.8 KB (7779 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e4b14e7f868497bf35a981b97fa3d6c40d44c373e6207c0e73aa3292319b6e8`  
		Last Modified: Tue, 05 Apr 2022 15:39:47 GMT  
		Size: 192.7 KB (192698 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c22a92e8f54240f73e546662dc34d0aa6b83ec1617f18fa8e178c93138c0b72e`  
		Last Modified: Tue, 05 Apr 2022 15:39:47 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98ad3607e9857b6fb1bb4fbf10d6e9ed9e787343edd64901dc0ecaadd3ff55db`  
		Last Modified: Tue, 05 Apr 2022 15:39:47 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:6b7fd2442f6dcd71561982dfb157122343a4c720493a891274c64d2c577ce4ab
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 MB (2933135 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8dc39b7901f2654c939cb1c1d44ff3a6e036a4bcf2cef396786768da4de2f658`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Mon, 04 Apr 2022 23:39:31 GMT
ADD file:90e56af13188c7f0283d244a0d70b853d8bef8587a41f1da8eac3a2aba8964ef in / 
# Mon, 04 Apr 2022 23:39:31 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 14:38:03 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Tue, 05 Apr 2022 14:38:04 GMT
RUN apk add --no-cache libssl1.1
# Tue, 05 Apr 2022 14:38:05 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 05 Apr 2022 14:38:15 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Tue, 05 Apr 2022 14:38:16 GMT
VOLUME [/spiped]
# Tue, 05 Apr 2022 14:38:17 GMT
WORKDIR /spiped
# Tue, 05 Apr 2022 14:38:19 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 05 Apr 2022 14:38:19 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 05 Apr 2022 14:38:20 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:9981e73032c8833e387a8f96986e560edbed12c38119e0edb0439c9c2234eac9`  
		Last Modified: Mon, 04 Apr 2022 19:09:10 GMT  
		Size: 2.7 MB (2716477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe4c0758a179cd25e16e078f253517cd4f315287416c3ce781a852e456da3093`  
		Last Modified: Tue, 05 Apr 2022 14:38:47 GMT  
		Size: 1.2 KB (1240 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ad68b994955132db089d9decfe3c1abb1e0d937a743641a82ff97b1ad0de230`  
		Last Modified: Tue, 05 Apr 2022 14:38:47 GMT  
		Size: 7.7 KB (7749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2412b85fbb446b18863d0276c285a9f15c5506327e253be647ba7c7e323d01e0`  
		Last Modified: Tue, 05 Apr 2022 14:38:47 GMT  
		Size: 207.2 KB (207235 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff9b28798cece086f58205831a8c06e9be4d79eb185eb2a5566b692c6bb0aa1f`  
		Last Modified: Tue, 05 Apr 2022 14:38:47 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9aa51b8e1739c24bc53b08bbda05fba07af4b69550a9c5ac36ea5be1bb7d5b1`  
		Last Modified: Tue, 05 Apr 2022 14:38:47 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; 386

```console
$ docker pull spiped@sha256:dcbb93128deb3206337ac10573e41e27b4a95816cd3f931412c655201fef2396
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.1 MB (3053817 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fdb9526919356b65e45d7bc9a9bd2aaddd7da8a1e62f023b9511a320a431df64`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Mon, 04 Apr 2022 23:38:25 GMT
ADD file:7d51a0f8691eb78c9062fd31984423a93d276a67b4ed5d1a706e1c2cd9fea23a in / 
# Mon, 04 Apr 2022 23:38:25 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 06:51:23 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Tue, 05 Apr 2022 06:51:24 GMT
RUN apk add --no-cache libssl1.1
# Tue, 05 Apr 2022 06:51:24 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 05 Apr 2022 06:51:34 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Tue, 05 Apr 2022 06:51:35 GMT
VOLUME [/spiped]
# Tue, 05 Apr 2022 06:51:36 GMT
WORKDIR /spiped
# Tue, 05 Apr 2022 06:51:38 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 05 Apr 2022 06:51:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 05 Apr 2022 06:51:39 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:73b28a5955ec7fb46f2cf0434e4901a889f7dda3f8c9ec496300feb256c7eda8`  
		Last Modified: Mon, 04 Apr 2022 19:10:03 GMT  
		Size: 2.8 MB (2818974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5043c44edf55100d2df153f657912b53abf987ef0c6286b113dcef298998f359`  
		Last Modified: Tue, 05 Apr 2022 06:52:09 GMT  
		Size: 1.2 KB (1240 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfc9d36e654ea336dd74dc00574768a6502edd5ef5cd785b695e516f6254be55`  
		Last Modified: Tue, 05 Apr 2022 06:52:08 GMT  
		Size: 7.8 KB (7750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0401735f1a5cdc5a0248a778049579b8858a6f7cc0fc6fdcdaea211930d4a386`  
		Last Modified: Tue, 05 Apr 2022 06:52:08 GMT  
		Size: 225.4 KB (225416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5a85e3f263e110e3fa50aada2a3ca6314a5a6e67e8f211881a826585a5db409`  
		Last Modified: Tue, 05 Apr 2022 06:52:08 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a0f113efbe13d3511b57cb0428e99f2725a51cb3980e75b1f1be3fc0d715b19`  
		Last Modified: Tue, 05 Apr 2022 06:52:08 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; ppc64le

```console
$ docker pull spiped@sha256:6d1206f429c5113ac4fbd6820b913ec32aa3cb826c65e5446d05eb57c3bfd7f4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (3033860 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:64a17da88fc17c158a4b17b8a85a6b534482d5b9fe198bee0a961886519d4811`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Tue, 05 Apr 2022 00:23:30 GMT
ADD file:960cf6f9d3d1cfcb36c2d67dd4c3eaba7db1d0c7afe97968512248d7f234ad47 in / 
# Tue, 05 Apr 2022 00:23:32 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 20:07:37 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Tue, 05 Apr 2022 20:08:01 GMT
RUN apk add --no-cache libssl1.1
# Tue, 05 Apr 2022 20:08:06 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 05 Apr 2022 20:08:35 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Tue, 05 Apr 2022 20:08:41 GMT
VOLUME [/spiped]
# Tue, 05 Apr 2022 20:08:46 GMT
WORKDIR /spiped
# Tue, 05 Apr 2022 20:08:48 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 05 Apr 2022 20:08:49 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 05 Apr 2022 20:08:52 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:1877acf2d48ed8bcb5bd9756a95aca0c077457be7cf4fcef25807f4e9be88db1`  
		Last Modified: Mon, 04 Apr 2022 19:09:49 GMT  
		Size: 2.8 MB (2811186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:898122ed2d1fcbc53be831191766c1b47d98b8cb2251d70dcc91e5ecad3bf34e`  
		Last Modified: Tue, 05 Apr 2022 20:09:25 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0cdc12b8854b22d6407eaece31ad74f6d0d2f322236c0d02a0074aef7944b93`  
		Last Modified: Tue, 05 Apr 2022 20:09:25 GMT  
		Size: 7.8 KB (7771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc1f84e0deee708d9995b37beb5b3923a9091dcc0ee670f7d784de701af40e2e`  
		Last Modified: Tue, 05 Apr 2022 20:09:25 GMT  
		Size: 213.2 KB (213160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67c77cab4a7338ba5a131c568ed153eb1fd0151dbb6108fae4fd3234a699f6ac`  
		Last Modified: Tue, 05 Apr 2022 20:09:25 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e03666b6f800b3362553b44e783b6eff051c84c4ae25bdb3d1da279626fc8bb9`  
		Last Modified: Tue, 05 Apr 2022 20:09:25 GMT  
		Size: 345.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:alpine` - linux; s390x

```console
$ docker pull spiped@sha256:851d4d1e8b82de6d455e9a562bd6b75539fe737213c9f3cf01ce7b44e11abeb4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 MB (2811594 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e240f56e6000d053b4d3e20632b54b88daaa8dad76ecda720ce9f76c82bfe394`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Mon, 04 Apr 2022 23:41:39 GMT
ADD file:f22e4b2be87d3c59c8c609acf79015938dc1fba0b26d7c1b59bd0fc36d63a906 in / 
# Mon, 04 Apr 2022 23:41:39 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 06:09:44 GMT
RUN set -x &&	addgroup -S spiped &&	adduser -S -G spiped spiped
# Tue, 05 Apr 2022 06:09:45 GMT
RUN apk add --no-cache libssl1.1
# Tue, 05 Apr 2022 06:09:45 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Tue, 05 Apr 2022 06:09:50 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 		curl 		gcc 		make 		musl-dev 		openssl-dev 		tar &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apk del --no-network .build-deps
# Tue, 05 Apr 2022 06:09:50 GMT
VOLUME [/spiped]
# Tue, 05 Apr 2022 06:09:51 GMT
WORKDIR /spiped
# Tue, 05 Apr 2022 06:09:51 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Tue, 05 Apr 2022 06:09:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 05 Apr 2022 06:09:51 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:a27b630f446c3da376a30cf610e4bfa6847f8b87c83702c29e72b986f4e52d28`  
		Last Modified: Mon, 04 Apr 2022 23:42:37 GMT  
		Size: 2.6 MB (2600375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ffc8ec477cbe2d575e99a9232e9328db8cc40109dbe067d93c2033302576850`  
		Last Modified: Tue, 05 Apr 2022 06:10:22 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ee008c7ec71319091cda7b7cbf1063414ee758f739581409a2e7089e90882c9`  
		Last Modified: Tue, 05 Apr 2022 06:10:21 GMT  
		Size: 7.8 KB (7788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3edcb5212f084eabfd1bad6e332d8b53bd7756099c4da3e410ee23f869a701b`  
		Last Modified: Tue, 05 Apr 2022 06:10:21 GMT  
		Size: 201.7 KB (201693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd099e1efb05ce5fa06c5e18ba7d057b5df318c462022f1ac443f45e86fdc809`  
		Last Modified: Tue, 05 Apr 2022 06:10:21 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afbab95e29c022d6828d869e5e4442b139373571c747f8fc6470b8bd257337a4`  
		Last Modified: Tue, 05 Apr 2022 06:10:21 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `spiped:latest`

```console
$ docker pull spiped@sha256:7a1276ab6a9bd4e55b8313b8cd13c2feabdc32369f047a82db7b499c42206a14
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
$ docker pull spiped@sha256:a66911a787746637e44a865f64e731ea404d2266efa5d987ee58d6d535a3999b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.3 MB (37349901 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4b801341ea8d054b7b965f35306e02a25be57d78de5177ed30cfb7af2b0267b7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 11 May 2022 01:20:16 GMT
ADD file:4a0bb88956083aa56032fdd9601d9b66c39b18c896ba35ea33594cd75621640a in / 
# Wed, 11 May 2022 01:20:16 GMT
CMD ["bash"]
# Wed, 11 May 2022 09:31:09 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 11 May 2022 09:31:12 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 09:31:12 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 11 May 2022 09:31:32 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 11 May 2022 09:31:32 GMT
VOLUME [/spiped]
# Wed, 11 May 2022 09:31:32 GMT
WORKDIR /spiped
# Wed, 11 May 2022 09:31:32 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 11 May 2022 09:31:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 11 May 2022 09:31:32 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:214ca5fb90323fe769c63a12af092f2572bf1c6b300263e09883909fc865d260`  
		Last Modified: Wed, 11 May 2022 01:25:13 GMT  
		Size: 31.4 MB (31379476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:080576f9a12bf8fca30a9653a7d9a0772acec767c26a2330bcdd92e5be0cfe95`  
		Last Modified: Wed, 11 May 2022 09:31:50 GMT  
		Size: 1.7 KB (1732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38bcb584eb7cb0f5bd593db63ab12b7b34bea2aa958fde7434a9b859ec903c08`  
		Last Modified: Wed, 11 May 2022 09:31:49 GMT  
		Size: 1.1 KB (1051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5664b9af48e8dd5dd00adb4691215c987017dbdb64998cdc9c30c22786d136d`  
		Last Modified: Wed, 11 May 2022 09:31:51 GMT  
		Size: 6.0 MB (5967174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6affb70c27746eb9c197393a54cd9b606353628e04424d0b4935ac195b6674a`  
		Last Modified: Wed, 11 May 2022 09:31:49 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01cd4accaf294c916a8ef636747fa575dbaa0f547f8bd5c7001c0112a9507dc2`  
		Last Modified: Wed, 11 May 2022 09:31:49 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; arm variant v5

```console
$ docker pull spiped@sha256:6b56704713f5efb9e393f0c751fe4e3ecfc3762033496269972dbb442a70972d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.0 MB (33952053 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6b14d990d1127fdf382852ac149cf58dd872a968df8176e8a74a5778ea0738c1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 11 May 2022 00:50:34 GMT
ADD file:72357b75d7e4546f06abf4648ab600980e742a3017f36da3c7a6c086f2f5fb56 in / 
# Wed, 11 May 2022 00:50:35 GMT
CMD ["bash"]
# Thu, 12 May 2022 01:35:14 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Thu, 12 May 2022 01:35:23 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Thu, 12 May 2022 01:35:23 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 12 May 2022 01:36:14 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 12 May 2022 01:36:15 GMT
VOLUME [/spiped]
# Thu, 12 May 2022 01:36:15 GMT
WORKDIR /spiped
# Thu, 12 May 2022 01:36:16 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 12 May 2022 01:36:16 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 12 May 2022 01:36:17 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:f7b69be15db1cb94a249f74b27edd4f5e5923a8701b026179a593f6888e897aa`  
		Last Modified: Wed, 11 May 2022 01:05:51 GMT  
		Size: 28.9 MB (28921122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a5a9157aa645038e20cfd8d939540308935a2f448009504b4b50f55ebe7fcc8`  
		Last Modified: Thu, 12 May 2022 01:36:50 GMT  
		Size: 1.7 KB (1725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:379d8521d9bd468b1d6a357f9682b3e0efc683bb7ce8c61b98639d89a6e5a9d3`  
		Last Modified: Thu, 12 May 2022 01:36:50 GMT  
		Size: 1.1 KB (1050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94258b91da89ba5bcfb0b99e7a7224030f4fbc734a79e19488d7b2e198797278`  
		Last Modified: Thu, 12 May 2022 01:36:55 GMT  
		Size: 5.0 MB (5027685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8ecd42d03f9650c45b9f15fb17188211b89f7ea6683a8aa6d8cf3ea08653577`  
		Last Modified: Thu, 12 May 2022 01:36:50 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82055141d6a68a71687d6ce1c4aa739a9d6fa527bf54e1eb9120550413add7ea`  
		Last Modified: Thu, 12 May 2022 01:36:50 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; arm variant v7

```console
$ docker pull spiped@sha256:426553dc9b38cdd633ce43cdf604b956d3d21c098bc256d936f9154132930908
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.3 MB (31327127 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7e6ef92e514ca9a3a7a716f84914ba360321d707df4255203a53390721630843`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 11 May 2022 01:49:07 GMT
ADD file:7c0451fffe8a520c2ab23048948d76bfe0dc0d90298c3d859279ccd8815b84f6 in / 
# Wed, 11 May 2022 01:49:08 GMT
CMD ["bash"]
# Thu, 12 May 2022 09:57:40 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Thu, 12 May 2022 09:57:47 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Thu, 12 May 2022 09:57:48 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 12 May 2022 09:58:33 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 12 May 2022 09:58:34 GMT
VOLUME [/spiped]
# Thu, 12 May 2022 09:58:34 GMT
WORKDIR /spiped
# Thu, 12 May 2022 09:58:35 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 12 May 2022 09:58:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 12 May 2022 09:58:36 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:1a9427b75b1c1db800cae7a9199bb4e508702e6761b17cc904d21441df43016c`  
		Last Modified: Wed, 11 May 2022 02:04:35 GMT  
		Size: 26.6 MB (26575672 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:666c704c2d2710e68360474f0cd959985e4418ee1bf3da5f69155679a1aae5e3`  
		Last Modified: Thu, 12 May 2022 09:59:35 GMT  
		Size: 1.7 KB (1736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:997d8d681765c85ae870076561eed251de76347cf9bf8d4fe9ca8bea5ee94d7e`  
		Last Modified: Thu, 12 May 2022 09:59:36 GMT  
		Size: 1.1 KB (1051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:666b40dc8c26e1e531689caf804a1d968693ea152f3580588acd62cd67aba309`  
		Last Modified: Thu, 12 May 2022 09:59:39 GMT  
		Size: 4.7 MB (4748197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d352d4363ba035dd50fa29f21ce08e12bdee48d3e9801fad5ae5d27d2e842c2`  
		Last Modified: Thu, 12 May 2022 09:59:35 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe1a6862d97ef70fbc74954b3f2e128027ea3142115032009c75b79794fedebb`  
		Last Modified: Thu, 12 May 2022 09:59:35 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; arm64 variant v8

```console
$ docker pull spiped@sha256:572906adb8bf287a02331ed2dc6b70d40c1795ce56eb514a7b873ac8b0b07782
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.3 MB (35339551 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:df8ebf44dc7acf424cbe762be8778cd542ccc7006e183a616763d3b92f5af2cc`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 11 May 2022 00:46:59 GMT
ADD file:158a0e401328bd7c0d49b9e8539186098967218f1b1a8c811f4398d29b74397f in / 
# Wed, 11 May 2022 00:47:00 GMT
CMD ["bash"]
# Wed, 11 May 2022 12:24:33 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 11 May 2022 12:24:36 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 12:24:37 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 11 May 2022 12:24:55 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 11 May 2022 12:24:56 GMT
VOLUME [/spiped]
# Wed, 11 May 2022 12:24:57 GMT
WORKDIR /spiped
# Wed, 11 May 2022 12:24:59 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 11 May 2022 12:24:59 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 11 May 2022 12:25:00 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:dfdd5ffb257742b891ccad9400a77dad2a6260b2451e0f5e48a9ade1d17a87ec`  
		Last Modified: Wed, 11 May 2022 00:53:46 GMT  
		Size: 30.1 MB (30065693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e25366de1af948b0eef7cad0d0d1fbc56648a743854da03fc57dc121c2384213`  
		Last Modified: Wed, 11 May 2022 12:25:32 GMT  
		Size: 1.6 KB (1621 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aef033e02dd13ee59e5336850b85b81cbd2ccd353a033415114d010d6a8254df`  
		Last Modified: Wed, 11 May 2022 12:25:32 GMT  
		Size: 922.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dac510a96382ea09a86f8f4cadc73653a8177516d4771a4a7e3bccbdeeb326de`  
		Last Modified: Wed, 11 May 2022 12:25:33 GMT  
		Size: 5.3 MB (5270881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1616a14c0096a1c7108f1fe3372296010619c2f7c502e1802e6d3855dfdf0ebd`  
		Last Modified: Wed, 11 May 2022 12:25:32 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcaa87e60ef72bc3e5eab8bd8a81a9cee650735736cd7c760f4366260b5461d2`  
		Last Modified: Wed, 11 May 2022 12:25:32 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; 386

```console
$ docker pull spiped@sha256:d933a3ef2f835e9d32f01babb2f55693ab6f3b2150d76a4e72d6fdec66739208
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.3 MB (40284215 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8994e3dd3df7e9fdbd0d51ca1e620fa69f6efd232ff5d5d2b381cd6b22fbc13c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 11 May 2022 01:39:14 GMT
ADD file:9eecb0fd311177f9d226e914c411aef49b5de1930e73019d2ee24afed515b5a2 in / 
# Wed, 11 May 2022 01:39:14 GMT
CMD ["bash"]
# Wed, 11 May 2022 15:51:27 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 11 May 2022 15:51:30 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 15:51:31 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 11 May 2022 15:51:52 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 11 May 2022 15:51:52 GMT
VOLUME [/spiped]
# Wed, 11 May 2022 15:51:53 GMT
WORKDIR /spiped
# Wed, 11 May 2022 15:51:55 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 11 May 2022 15:51:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 11 May 2022 15:51:56 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:91c5bdbe4bf9f1970dd54ba71e2523649adce4e5240c2ff8a87711bf389ecba3`  
		Last Modified: Wed, 11 May 2022 01:46:25 GMT  
		Size: 32.4 MB (32389776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa9bc810ed14e83b2b6c2de848151a8aac3442608851df4e4ba4f35402048a54`  
		Last Modified: Wed, 11 May 2022 15:52:27 GMT  
		Size: 1.6 KB (1608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ddd23897c0dc65364a8fda9129fe87c608a02ac54bdd3002e70407c7dff7b8a`  
		Last Modified: Wed, 11 May 2022 15:52:27 GMT  
		Size: 923.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a55bc0fd5c56c871a37888a72d560d40d0364889e86b54c791bea4bb7c85887`  
		Last Modified: Wed, 11 May 2022 15:52:28 GMT  
		Size: 7.9 MB (7891471 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad4fc1778cbfb42cc882687278e3d3bb64b10572a3b56cf12d7ba9b128537d21`  
		Last Modified: Wed, 11 May 2022 15:52:27 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cc951e82cef08be37b45eba1592c940f1a946d625884f3e80794061addeb20a`  
		Last Modified: Wed, 11 May 2022 15:52:27 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; mips64le

```console
$ docker pull spiped@sha256:98dafc6cf00b4ae4723240a88ce5bed8cc462c78e6e05aa1fdea9727db128735
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.3 MB (35349146 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:008c2d2ba6ac1949b574aa0cd913d936ebd6fadc503e85c425e3052ef113387d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 11 May 2022 02:23:35 GMT
ADD file:d47dce2adbc9352ef1d437730bab3b579dd8d2bf29dd60cd8a8b65396b39e36e in / 
# Wed, 11 May 2022 02:23:40 GMT
CMD ["bash"]
# Thu, 12 May 2022 04:11:52 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Thu, 12 May 2022 04:12:07 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Thu, 12 May 2022 04:12:09 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Thu, 12 May 2022 04:13:33 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 12 May 2022 04:13:36 GMT
VOLUME [/spiped]
# Thu, 12 May 2022 04:13:39 GMT
WORKDIR /spiped
# Thu, 12 May 2022 04:13:41 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Thu, 12 May 2022 04:13:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 12 May 2022 04:13:46 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:438a36bf0b6e75ff6f0fbb2b7669dfb86361416f4d808912d30cf5b91ad2eea9`  
		Last Modified: Wed, 11 May 2022 02:33:43 GMT  
		Size: 29.6 MB (29641051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b968eb568ff8a2acb36380ccbf842b116d8f7251fe76b4d4c05350e872efe8f`  
		Last Modified: Thu, 12 May 2022 04:14:11 GMT  
		Size: 1.6 KB (1614 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e0c58081df5c4242f571acbbce6534a045404bc2c44eab75dbe2bfa721606fc`  
		Last Modified: Thu, 12 May 2022 04:14:11 GMT  
		Size: 925.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2c0fc303ca2ffd0acaaa4421f936b6d1cdcbd87e50ae67c64e5d2f003a022f8`  
		Last Modified: Thu, 12 May 2022 04:14:16 GMT  
		Size: 5.7 MB (5705117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a84b67927c5aea3805e90f18768e6338fd392e91c3618805526b3ff7c776b824`  
		Last Modified: Thu, 12 May 2022 04:14:11 GMT  
		Size: 95.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c4229b76d1a9cdc6812c0c3734a7d00ca0f098edeb70043fce974697a9d2a4c`  
		Last Modified: Thu, 12 May 2022 04:14:11 GMT  
		Size: 344.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; ppc64le

```console
$ docker pull spiped@sha256:e338e5b4a068b2c06d20548b51e98cf9e6711b5ba3f91a55f33517103107db26
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.3 MB (41288815 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:54eb4238d8977094c460b01a31bf18ab2865f97d34da09adaf33454df8e1a99f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 11 May 2022 01:32:29 GMT
ADD file:1e94716789ec21981460f74be38a668bc212bd804c1d41cecf90036a5bccac5a in / 
# Wed, 11 May 2022 01:32:34 GMT
CMD ["bash"]
# Wed, 11 May 2022 14:18:46 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 11 May 2022 14:18:57 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 14:19:00 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 11 May 2022 14:21:35 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 11 May 2022 14:21:45 GMT
VOLUME [/spiped]
# Wed, 11 May 2022 14:21:59 GMT
WORKDIR /spiped
# Wed, 11 May 2022 14:22:09 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 11 May 2022 14:22:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 11 May 2022 14:22:21 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:2533109ed11eefd6415e0370d6d7a3ea879b582b1887c98b819a598ad18fca24`  
		Last Modified: Wed, 11 May 2022 01:43:03 GMT  
		Size: 35.3 MB (35286467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e371d58c256a557b6f8f7b903d8a39345ccc364236516cb3ec208e9e40e92c5`  
		Last Modified: Wed, 11 May 2022 14:23:02 GMT  
		Size: 1.7 KB (1743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b4caf1ad053d6d5585c461ca9b8d4c6a14a963b94b0d13bb0594b2244f15a8b`  
		Last Modified: Wed, 11 May 2022 14:23:02 GMT  
		Size: 1.1 KB (1054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb23602e10ec58354d8276b2a6d7549e7f11c523d76e28603f149ca4c0e1e951`  
		Last Modified: Wed, 11 May 2022 14:23:04 GMT  
		Size: 6.0 MB (5999080 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fa6bf1315149ea1738416c3df58107d0e9c60aae5cb546cfdcbb50aa6855062`  
		Last Modified: Wed, 11 May 2022 14:23:02 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82539badabc1522bce1e3acd0e092aceb9818dd6904d2ab5fe8a10ab39a0f6b5`  
		Last Modified: Wed, 11 May 2022 14:23:02 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `spiped:latest` - linux; s390x

```console
$ docker pull spiped@sha256:a2261239d98aaef54af72737a4aa30c1a01f4089439604c977e606d06e5eb317
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.8 MB (34844727 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d218c6ec1b1cc03c92a160497f19dc4deed41827aaf7bef061ddc8ca4c8f6fac`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["spiped"]`

```dockerfile
# Wed, 11 May 2022 00:44:17 GMT
ADD file:d93a1cf64a813d01774cd628dfd683c006e20159e2ab3464c2159c8d9897c725 in / 
# Wed, 11 May 2022 00:44:19 GMT
CMD ["bash"]
# Wed, 11 May 2022 06:26:51 GMT
RUN set -x &&	groupadd -r spiped &&	useradd -r -g spiped spiped
# Wed, 11 May 2022 06:26:54 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y libssl1.1 --no-install-recommends &&	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 06:26:54 GMT
ENV SPIPED_VERSION=1.6.2 SPIPED_DOWNLOAD_SHA256=05d4687d12d11d7f9888d43f3d80c541b7721c987038d085f71c91bb06204567
# Wed, 11 May 2022 06:27:06 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='libssl-dev libc-dev gcc make curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://www.tarsnap.com/spiped/spiped-$SPIPED_VERSION.tgz" -o spiped.tar.gz &&	echo "$SPIPED_DOWNLOAD_SHA256 *spiped.tar.gz" |sha256sum -c - &&	mkdir -p /usr/local/src/spiped &&	tar xzf "spiped.tar.gz" -C /usr/local/src/spiped --strip-components=1 &&	rm "spiped.tar.gz" &&	CC=gcc make -C /usr/local/src/spiped &&	make -C /usr/local/src/spiped install &&	rm -rf /usr/local/src/spiped &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 11 May 2022 06:27:07 GMT
VOLUME [/spiped]
# Wed, 11 May 2022 06:27:07 GMT
WORKDIR /spiped
# Wed, 11 May 2022 06:27:07 GMT
COPY multi:5bc169de21988025d207318e8462faac29a47f22ea391b38427ea86b5aba8f5a in /usr/local/bin/ 
# Wed, 11 May 2022 06:27:07 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 11 May 2022 06:27:07 GMT
CMD ["spiped"]
```

-	Layers:
	-	`sha256:9f3750f6094217808e26d471752341db88153c8d5b5f9bb11577b74671303bbc`  
		Last Modified: Wed, 11 May 2022 00:50:03 GMT  
		Size: 29.7 MB (29654739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:873c48057acd3a3e859a48bcca0c21842c182414ce09c34a3cc1c1886f7de52a`  
		Last Modified: Wed, 11 May 2022 06:27:39 GMT  
		Size: 1.7 KB (1734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09c3eb03701aaff2a58238f35a586fbc044102b129292492a02c7479e57440b3`  
		Last Modified: Wed, 11 May 2022 06:27:39 GMT  
		Size: 1.1 KB (1052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c22498c1d73103d486b8e69a684b02839606786d6cff45d0dfbdbdc6e26ce68c`  
		Last Modified: Wed, 11 May 2022 06:27:40 GMT  
		Size: 5.2 MB (5186734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6758dfdb3a7588b70d2a3af8806cc9cea3dee7221cfe99f32973d6c0eee71d46`  
		Last Modified: Wed, 11 May 2022 06:27:39 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6fcc234dd9c90350b33b0e204d793aec0e7ee86952bb815ce76739eced0d2a7`  
		Last Modified: Wed, 11 May 2022 06:27:39 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
