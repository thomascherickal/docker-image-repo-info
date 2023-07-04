## `debian:trixie-backports`

```console
$ docker pull debian@sha256:8287bfac87404bb35210720bd6f9b161cb2c0db53f4a9d7b55152a15def7456d
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

### `debian:trixie-backports` - linux; amd64

```console
$ docker pull debian@sha256:05981a41808de8adb43d02efef73212255962e49885ce7cdceeb302a65e3d273
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.6 MB (49552341 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e2a6ff378c84d8b1c05f71f218967224db6bf2ae365ea1029ecb31fc49781890`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 12 Jun 2023 23:23:47 GMT
ADD file:2f268935a4a1bb259a84889b28c6c360a8ef3ce8effe761060fcc1282fdd7162 in / 
# Mon, 12 Jun 2023 23:23:48 GMT
CMD ["bash"]
# Mon, 12 Jun 2023 23:23:52 GMT
RUN echo 'deb http://deb.debian.org/debian trixie-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:3ec88205db53a7e48cfcd2f1b7e3045bd6ffac54418b97bbdc66c7c72c425cc8`  
		Last Modified: Mon, 12 Jun 2023 23:30:03 GMT  
		Size: 49.6 MB (49552120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e64d46c7c5177a322e77b81f44de5b7306afac3d82cba01c12da672e7ba079f`  
		Last Modified: Mon, 12 Jun 2023 23:30:12 GMT  
		Size: 221.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:trixie-backports` - linux; arm variant v5

```console
$ docker pull debian@sha256:e81d3682081739607a458f874cdf09e6f82488329bbc3adb6658669b11e1b2da
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.4 MB (47360291 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ae32a37a97d059a474f4b4c1bfb7aed1b42298cbc7ec86161fa6fe78f69b4e75`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 00:49:59 GMT
ADD file:0ffd95af69945bc7c3ba2733bffd453f61419b678dcc1b0bf13261d9a2d147f7 in / 
# Tue, 04 Jul 2023 00:49:59 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 00:50:02 GMT
RUN echo 'deb http://deb.debian.org/debian trixie-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:059b0228783b958bcd75527dc7506c02509e9b3a009b9e7f5b944545d6d86929`  
		Last Modified: Tue, 04 Jul 2023 00:55:11 GMT  
		Size: 47.4 MB (47360068 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:800e40cbc2bdb55b4e850e1de91b839cf32b2fe10878fa6e6bfb56e2245fb5e6`  
		Last Modified: Tue, 04 Jul 2023 00:55:19 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:trixie-backports` - linux; arm variant v7

```console
$ docker pull debian@sha256:470115159880b4f4ae66a971819f3fd22f86f726a586d6732ce135e980bcedb1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.2 MB (45183044 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:10edec909c5814fbc1eec58d5f35fc76c37103c447f59b87481bce5752a709c6`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 01:00:59 GMT
ADD file:d1d870c89e7d21b3459cde2dabaf0d8fbc038324334dfb59648191201c0881a6 in / 
# Tue, 04 Jul 2023 01:00:59 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 01:01:03 GMT
RUN echo 'deb http://deb.debian.org/debian trixie-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:de599662316fbbb0e5a107c34fc84f0bd6cce1eae2febdee5f9a166bcbe6f898`  
		Last Modified: Tue, 04 Jul 2023 01:07:24 GMT  
		Size: 45.2 MB (45182820 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5670106917a9946afac9ad64e88b57f1d74426abd2e7fb9c5a1690541d0674ac`  
		Last Modified: Tue, 04 Jul 2023 01:07:33 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:trixie-backports` - linux; arm64 variant v8

```console
$ docker pull debian@sha256:456afb1d856bd56d537c5ea9ee2e744d3606ad7c3041a57a93ffbc92b8a9a558
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.6 MB (49573418 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:14d15cc08e33fc1eb9cc2a380821e8691693a9466192986686abe9384cbd1016`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 12 Jun 2023 23:42:34 GMT
ADD file:8d6fedaebaef2ab7e9fe8c253f296a84e4427aa6df2f80248ea821ad3e3c4927 in / 
# Mon, 12 Jun 2023 23:42:35 GMT
CMD ["bash"]
# Mon, 12 Jun 2023 23:42:38 GMT
RUN echo 'deb http://deb.debian.org/debian trixie-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:544d305270eb6dac2e9d07cd9771046cc45dcd62351837065488fce378d5bea5`  
		Last Modified: Mon, 12 Jun 2023 23:47:58 GMT  
		Size: 49.6 MB (49573198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11939ea8129dec9d2975e24298fa896b9e6a033b08eb4b390315d28af897b539`  
		Last Modified: Mon, 12 Jun 2023 23:48:06 GMT  
		Size: 220.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:trixie-backports` - linux; 386

```console
$ docker pull debian@sha256:3d093708da05e4c596e540552962a2f93802b04df7a998a0fec81a7eb5d50ff1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.6 MB (50562579 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cb2101d9af7630902b91c90aa82bf99e3634c52affaef915bd98993396ef4291`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 12 Jun 2023 23:44:01 GMT
ADD file:d55b975f56bfbd408aa18ccd4df1df637e021479e3630d059a33fc2853f2c058 in / 
# Mon, 12 Jun 2023 23:44:02 GMT
CMD ["bash"]
# Mon, 12 Jun 2023 23:44:07 GMT
RUN echo 'deb http://deb.debian.org/debian trixie-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:db79b9a081675971d6f4573fddf3370ce83494dff44942df3f73f2fc007711fe`  
		Last Modified: Mon, 12 Jun 2023 23:51:13 GMT  
		Size: 50.6 MB (50562356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db880ca6dfe5b98babf44d1497d8d6355a83c1084b37d10afb0457c57b3ef747`  
		Last Modified: Mon, 12 Jun 2023 23:51:21 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:trixie-backports` - linux; mips64le

```console
$ docker pull debian@sha256:67a5aff952ebc2df425a1c2b662f364a2ff55ed96c972810b1cf969c61dc31ed
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.5 MB (49541721 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:de77be5845bd30c363e2d8737a84fc0a9dacc17bc3d9adeaa93becd0b8bbc0d0`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Jun 2023 00:17:35 GMT
ADD file:59bff6e970731822677b01e286a3eadbe24927f46d0cb457ce2dfafe01c526fa in / 
# Tue, 13 Jun 2023 00:17:41 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 00:17:57 GMT
RUN echo 'deb http://deb.debian.org/debian trixie-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:ad193c6eea2eff4d154ba079c2bb27eed8305280e7a7b1a8e2a8de073ecea8b4`  
		Last Modified: Tue, 13 Jun 2023 00:29:33 GMT  
		Size: 49.5 MB (49541496 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6df38c4f37452c0e6322f3857d581455de2a53eab33a695672d309772352fdf6`  
		Last Modified: Tue, 13 Jun 2023 00:29:43 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:trixie-backports` - linux; ppc64le

```console
$ docker pull debian@sha256:2bc8f930b4bcda299bf26295caeb3d9a1965238cb1639d40ed8369a5a19c3cd1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.5 MB (53536934 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:23f553ef25e0cbd49ef2fdac191971fc28385cc539097417823402fac5db555d`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 12 Jun 2023 23:21:35 GMT
ADD file:1b07922c76a2b429657b08217944f3d121ebd5b7096011c1661544ce04c3a256 in / 
# Mon, 12 Jun 2023 23:21:38 GMT
CMD ["bash"]
# Mon, 12 Jun 2023 23:21:42 GMT
RUN echo 'deb http://deb.debian.org/debian trixie-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:5f8f7984b6dbc3cdadd73d4dfdc516e44f1fd14e24a6ff1bea8fb164e47e3dd0`  
		Last Modified: Mon, 12 Jun 2023 23:28:22 GMT  
		Size: 53.5 MB (53536713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f19bbe0f1a77c707bde592d3bc19c89b33e3a3145f3c687f7cd6a96738326d77`  
		Last Modified: Mon, 12 Jun 2023 23:28:35 GMT  
		Size: 221.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:trixie-backports` - linux; s390x

```console
$ docker pull debian@sha256:7067af30260d23b23d6a0ad61c23b73b0d776b9b88b958b61728f640b0ae9c35
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.9 MB (47921824 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:14cef483e14df9661e3be7814d0ca61f7bb25f819f5756556ffeb3e1c01f7c24`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Jun 2023 04:32:26 GMT
ADD file:d6efbf24824c41fbb2df9bb8d46fdc6e4a418edbd93f833577291fc4c298f0e9 in / 
# Tue, 13 Jun 2023 04:32:29 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 04:32:35 GMT
RUN echo 'deb http://deb.debian.org/debian trixie-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:2a1ca40b7e01ccce3abf39a53788ace9deeab9180d55a80bddac1f28a127114f`  
		Last Modified: Tue, 13 Jun 2023 04:36:32 GMT  
		Size: 47.9 MB (47921604 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31dea941f6591d2d52c77931c3a6e6057f0a470b4ab3a927bd520d05be8198b1`  
		Last Modified: Tue, 13 Jun 2023 04:36:37 GMT  
		Size: 220.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
