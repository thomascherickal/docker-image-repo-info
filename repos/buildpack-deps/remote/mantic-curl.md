## `buildpack-deps:mantic-curl`

```console
$ docker pull buildpack-deps@sha256:1a3e487623346261603db0f203a84daf1259e84828605400f1a8d93bbd87281a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `buildpack-deps:mantic-curl` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:cd3ff14aac5bd8abbcebc29597cbe8f4da268fed31446be6c300643c6cc3a132
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.6 MB (41640733 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:08e7fea7440d087befe1a7723ef76adf9307317fb275ffdd2ab732c581234314`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 01 Aug 2023 05:32:47 GMT
ARG RELEASE
# Tue, 01 Aug 2023 05:32:47 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 01 Aug 2023 05:32:47 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 01 Aug 2023 05:32:47 GMT
LABEL org.opencontainers.image.version=23.10
# Tue, 01 Aug 2023 05:32:49 GMT
ADD file:7d5373d4ccc5f70f68afa885a495329e33f2bf9f97a437251cfc79e7b85a1a88 in / 
# Tue, 01 Aug 2023 05:32:49 GMT
CMD ["/bin/bash"]
# Thu, 03 Aug 2023 03:33:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:316675922a661ce4c35389bdeea6e9ec8d4708e41f08671b586c7aaea469b2c1`  
		Last Modified: Thu, 03 Aug 2023 03:40:24 GMT  
		Size: 27.9 MB (27857084 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07a7def12313ae9d69537ed1d4ea003f137f16c5789329735bfd447f8c86cfca`  
		Last Modified: Thu, 03 Aug 2023 03:40:22 GMT  
		Size: 13.8 MB (13783649 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:mantic-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:b6b70fc65a86ef181308b9d4483306a21297953e302338b8b98dd429a421775c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.1 MB (38148463 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:682824261387f5531a8beaef8be345112bc3551257c13812203c72ed136de890`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 07 Aug 2023 16:43:12 GMT
ARG RELEASE
# Mon, 07 Aug 2023 16:43:12 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 07 Aug 2023 16:43:12 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 07 Aug 2023 16:43:12 GMT
LABEL org.opencontainers.image.version=23.10
# Mon, 07 Aug 2023 16:43:20 GMT
ADD file:443a623a513d24fb17f92fecba92ab4b48c5cd58f4c71a4d1017f68cb28ed803 in / 
# Mon, 07 Aug 2023 16:43:20 GMT
CMD ["/bin/bash"]
# Wed, 16 Aug 2023 05:42:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:9a882830b71793138cc20048eb0866464a2a925cea19f5d96e75bef586f07b01`  
		Last Modified: Wed, 16 Aug 2023 05:52:57 GMT  
		Size: 25.5 MB (25451971 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c69c48a8564dd51e9033d498988912470fd0761ce0f5546103b27b81cf550ee6`  
		Last Modified: Wed, 16 Aug 2023 05:52:54 GMT  
		Size: 12.7 MB (12696492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:mantic-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:d9e5dc452e6b36370b11f94dbac9bae37e89073a8e9713c787528a7d5cbeb3f5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.6 MB (40636151 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:022e8f743594afe234ab66c579a551aff038aca5f366902e789b487cf05867a9`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 07 Aug 2023 16:59:38 GMT
ARG RELEASE
# Mon, 07 Aug 2023 16:59:38 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 07 Aug 2023 16:59:39 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 07 Aug 2023 16:59:39 GMT
LABEL org.opencontainers.image.version=23.10
# Mon, 07 Aug 2023 16:59:47 GMT
ADD file:a621d5a90b1c5e05eb41dfa44616425f9e9c474acc76e148c36a525e99ff2bac in / 
# Mon, 07 Aug 2023 16:59:48 GMT
CMD ["/bin/bash"]
# Wed, 16 Aug 2023 01:33:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:4b4647be7125cb643de6d0a75158905d697da4afc1e9edcd35dbb27a43edf604`  
		Last Modified: Wed, 16 Aug 2023 01:42:51 GMT  
		Size: 27.3 MB (27266349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14f74bc0fb029a079dcd558844cc26c5973e7ec9efc2db4555c60ab536a1a11f`  
		Last Modified: Wed, 16 Aug 2023 01:42:49 GMT  
		Size: 13.4 MB (13369802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:mantic-curl` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:49e1f7029605cde20671acc2e750197dfa84e8b1749902240630c8d61fd2b0df
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.1 MB (48118121 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:449f6529b4a74a21fda38d95eddd728bdb55d7eb1d0711936f509b804ca3dbe9`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 07 Aug 2023 16:57:20 GMT
ARG RELEASE
# Mon, 07 Aug 2023 16:57:20 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 07 Aug 2023 16:57:20 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 07 Aug 2023 16:57:20 GMT
LABEL org.opencontainers.image.version=23.10
# Mon, 07 Aug 2023 16:57:23 GMT
ADD file:4cb180718bb451f8c264f3c3ca17e21c2f353537e1350e7285186274e7c13aa1 in / 
# Mon, 07 Aug 2023 16:57:23 GMT
CMD ["/bin/bash"]
# Wed, 16 Aug 2023 02:01:44 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:fdf3d625c5c62f16c8647b6f71fb3627aa49027d553c24dfb5bb5fe384576e06`  
		Last Modified: Wed, 16 Aug 2023 02:16:46 GMT  
		Size: 32.2 MB (32220285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4266d044f5749871179995f4d16bfab0f930c8a7fc456be89d9dde4ff53c9a04`  
		Last Modified: Wed, 16 Aug 2023 02:16:42 GMT  
		Size: 15.9 MB (15897836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:mantic-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:219327f643dbe2a1a1e0cbbd61e31d93a8f2cad220aa3635e0bb34e4622ff1b4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.0 MB (41043202 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:99b11ab01ff2a750bdff354d4b274b8bfb22158a267a03ebda2ed609b5e32241`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 07 Aug 2023 16:41:40 GMT
ARG RELEASE
# Mon, 07 Aug 2023 16:41:40 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 07 Aug 2023 16:41:40 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 07 Aug 2023 16:41:40 GMT
LABEL org.opencontainers.image.version=23.10
# Mon, 07 Aug 2023 16:41:42 GMT
ADD file:7038e8b287279d65872808b33572bb449a981ceacdc4533e8e1047544044f524 in / 
# Mon, 07 Aug 2023 16:41:42 GMT
CMD ["/bin/bash"]
# Wed, 16 Aug 2023 04:32:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:6e4b480e7bad6fd35ac328034bc72b280c0019028bc95dd0dbf78d168750430e`  
		Last Modified: Wed, 16 Aug 2023 04:39:53 GMT  
		Size: 26.9 MB (26884397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44867c9f8a414f35f7e550468ffda8aadf82a61ad02779247fe2d748d28e5390`  
		Last Modified: Wed, 16 Aug 2023 04:39:51 GMT  
		Size: 14.2 MB (14158805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
