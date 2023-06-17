## `buildpack-deps:mantic-curl`

```console
$ docker pull buildpack-deps@sha256:2a6579b66684273efd6ec72432c03f82af3a6d7e1a822989eaed85f5cc01e3c3
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
$ docker pull buildpack-deps@sha256:c5f332e13ca19bc3c3e19b4033f483da85cc1b72bcac89ade819fbc88bdc51fe
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.5 MB (41469384 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c691125580dfbcf1003348c4be92cb5fffb57898f37abb2886adb09844867c88`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 07 Jun 2023 04:39:09 GMT
ARG RELEASE
# Wed, 07 Jun 2023 04:39:09 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 07 Jun 2023 04:39:09 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 07 Jun 2023 04:39:09 GMT
LABEL org.opencontainers.image.version=23.10
# Wed, 07 Jun 2023 04:39:10 GMT
ADD file:d8dc8c4236b9885e64ccd27399ed8dddab7d39915d76378527cb730855aba0e1 in / 
# Wed, 07 Jun 2023 04:39:10 GMT
CMD ["/bin/bash"]
# Fri, 16 Jun 2023 01:51:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:f4bf94e551580f94d5daff5f725b2d31607973745d1b88b4063002a615605d6e`  
		Last Modified: Fri, 16 Jun 2023 01:57:52 GMT  
		Size: 27.7 MB (27718548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5e689be570c2c956ab2de6b43f62c042013af889c34de3a06fa31c8840fd3bd`  
		Last Modified: Fri, 16 Jun 2023 01:57:50 GMT  
		Size: 13.8 MB (13750836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:mantic-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:5b114307fa87536ec11392334596fc7032cb25d612fa7d87f979834f4ee55ce1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.9 MB (37940783 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8c190de988d49e8e1fdbe5bf67cb67246aade085b976a9a21e57b3d2963cc3ea`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 07 Jun 2023 04:48:07 GMT
ARG RELEASE
# Wed, 07 Jun 2023 04:48:07 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 07 Jun 2023 04:48:08 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 07 Jun 2023 04:48:08 GMT
LABEL org.opencontainers.image.version=23.10
# Wed, 07 Jun 2023 04:48:12 GMT
ADD file:65e05498800189bf1f48f5c6df21d144e18e5e069db55d0b88d45c04cc1fe4de in / 
# Wed, 07 Jun 2023 04:48:12 GMT
CMD ["/bin/bash"]
# Fri, 16 Jun 2023 00:53:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:4d9959b212abdc29a099893ec5eeb0a1e80508f22581d6b7e8d7ac257769bee7`  
		Last Modified: Fri, 16 Jun 2023 01:00:47 GMT  
		Size: 25.3 MB (25271336 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85a3ceae76fca68286fb64b3323157a721f2f88a43cd21f69b7a567704523771`  
		Last Modified: Fri, 16 Jun 2023 01:00:46 GMT  
		Size: 12.7 MB (12669447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:mantic-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:c39c8df9209fb057d42e507d33a397c4eeb66a6ffe70ed74d22535da5298a1cc
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.4 MB (40412045 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1d8696c8456822956dd26c435b59c4fc910da5ba981ca88a905b29ea4e957fa4`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 07 Jun 2023 04:42:14 GMT
ARG RELEASE
# Wed, 07 Jun 2023 04:42:14 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 07 Jun 2023 04:42:14 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 07 Jun 2023 04:42:14 GMT
LABEL org.opencontainers.image.version=23.10
# Wed, 07 Jun 2023 04:42:16 GMT
ADD file:3f4faed988a03b7d05aefe677906592aade4d2bae1ec3f7055c1f10744a38de0 in / 
# Wed, 07 Jun 2023 04:42:16 GMT
CMD ["/bin/bash"]
# Fri, 16 Jun 2023 02:29:37 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:62f0439e6eacbe88b3b071461591f644c013d55d1bb0ecba6442ac98c987966e`  
		Last Modified: Fri, 16 Jun 2023 02:36:15 GMT  
		Size: 27.1 MB (27075677 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39a4f6ab448c591bc2009541723cb7648afc9648bd50663a7868f9adb99bbb00`  
		Last Modified: Fri, 16 Jun 2023 02:36:13 GMT  
		Size: 13.3 MB (13336368 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:mantic-curl` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:b373eaca90f55ed06bb9cea88ef1728bb9c98c994d180679d4c1dfb81d2b24bd
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.8 MB (47794832 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f7524aaf87d1261d35d46e8aeb73f884bc5209fcc7c9d78559cf1c793d5054e9`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 07 Jun 2023 04:48:25 GMT
ARG RELEASE
# Wed, 07 Jun 2023 04:48:26 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 07 Jun 2023 04:48:26 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 07 Jun 2023 04:48:26 GMT
LABEL org.opencontainers.image.version=23.10
# Wed, 07 Jun 2023 04:48:28 GMT
ADD file:6cf1bffac55b7de64803fabdb35baf75349cc0a40c0b4c68ac2690b7123edc85 in / 
# Wed, 07 Jun 2023 04:48:29 GMT
CMD ["/bin/bash"]
# Fri, 16 Jun 2023 01:18:42 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:3977e86345903c1f3d3fa576bf7d23648e574cafb925e0b8db7f0a26b5b9813d`  
		Last Modified: Fri, 16 Jun 2023 01:30:28 GMT  
		Size: 32.0 MB (31950363 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80356e871c531718f8219858742d4f265352a0709040acb54605134885fb5b5f`  
		Last Modified: Fri, 16 Jun 2023 01:30:24 GMT  
		Size: 15.8 MB (15844469 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:mantic-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:ab4328d5274768f0608716426e9ce2c956ab90efefcd7848844538af0ee711d8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.3 MB (40288440 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5e7f91374a9f3ad829228f1446965b4ef2c6bb72199c4542b8f261641a8c60f1`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 07 Jun 2023 04:42:36 GMT
ARG RELEASE
# Wed, 07 Jun 2023 04:42:36 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 07 Jun 2023 04:42:36 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 07 Jun 2023 04:42:36 GMT
LABEL org.opencontainers.image.version=23.10
# Wed, 07 Jun 2023 04:42:38 GMT
ADD file:4e8ca8820de4a27d67ad223be645ce7a7a48289dfcbc01b4e1dbe3bc74ebbc56 in / 
# Wed, 07 Jun 2023 04:42:38 GMT
CMD ["/bin/bash"]
# Sat, 17 Jun 2023 09:56:31 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:f6943591795586ce983bdf25369a45a8d58f64cd04bb9b22a9ebfbbbcaa9443a`  
		Last Modified: Sat, 17 Jun 2023 10:03:01 GMT  
		Size: 26.3 MB (26281083 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:031ae27af25073c29d7050bd7d1de8c0178d4af4c165618364aec7a707620748`  
		Last Modified: Sat, 17 Jun 2023 10:02:59 GMT  
		Size: 14.0 MB (14007357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
