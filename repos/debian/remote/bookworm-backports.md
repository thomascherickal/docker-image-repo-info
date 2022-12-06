## `debian:bookworm-backports`

```console
$ docker pull debian@sha256:2e0fbfa5f6d7b84e268759dd850d729fcd9aaa831f50a40b77666785135ead69
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

### `debian:bookworm-backports` - linux; amd64

```console
$ docker pull debian@sha256:875d73cbf7c491a75587ec5daf871f00153f6cd573f451aedc82817993197f64
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.3 MB (50260743 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e26ce6b066086a8a3c233555e901746ef4e1e14071278b098d00421194331b2a`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 06 Dec 2022 01:20:17 GMT
ADD file:bc800ccc3502eee52ab13da7e930beeea45bff7ec8e6f625f2958550a0e0c4a0 in / 
# Tue, 06 Dec 2022 01:20:17 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 01:20:20 GMT
RUN echo 'deb http://deb.debian.org/debian bookworm-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:3d5213c1b98149df5de6014f7a0822d3f7c1239b55b191918b5019861d2385bf`  
		Last Modified: Tue, 06 Dec 2022 01:24:15 GMT  
		Size: 50.3 MB (50260519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52174568cd600885e30ce9c4862c1cc3a5e424dd78eaaaf9b9499193b336ce00`  
		Last Modified: Tue, 06 Dec 2022 01:24:23 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:bookworm-backports` - linux; arm variant v5

```console
$ docker pull debian@sha256:d0d5d7c74c6438692c3a9a42332223f54ff28da57fa4abe79c59e7f72a7b4fc1
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.2 MB (49227554 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:87dd48a980742ef957828e52427095a78b4ba1dfccd7ed1484d2e91e8fbadf6c`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 06 Dec 2022 01:48:36 GMT
ADD file:6f4f61d29cd543b4aac92345f1eafd1e5d79db8feeabac7b2a9bc503e68a105b in / 
# Tue, 06 Dec 2022 01:48:38 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 01:48:45 GMT
RUN echo 'deb http://deb.debian.org/debian bookworm-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:378b1d254700c864b8aa581433afac6f6a683e7a13dcd04dea4c2a4f39262d45`  
		Last Modified: Tue, 06 Dec 2022 01:53:21 GMT  
		Size: 49.2 MB (49227330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2ba88af502b8dd5bba8c20253e3473a057bace7e72fa284830c792a4041c102`  
		Last Modified: Tue, 06 Dec 2022 01:53:32 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:bookworm-backports` - linux; arm variant v7

```console
$ docker pull debian@sha256:38c95e0c194a30248700c5745c181e556238f925f18f1320d36f8bf9b7e7a5bc
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.0 MB (47047317 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a6622b3cfc990527797ef4e2a9d994463662ef3953deec3bf514625b77ba84c9`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 06 Dec 2022 00:57:56 GMT
ADD file:82dd62a6df63f711bc714098f18b9106a7507772b5320c66a30f7ccba2ae24a0 in / 
# Tue, 06 Dec 2022 00:57:57 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 00:58:04 GMT
RUN echo 'deb http://deb.debian.org/debian bookworm-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:2e675a2bd8a737d1b09b68b33be3a9ae4bf0f69f7b1ce279fd4c63e38d294b1b`  
		Last Modified: Tue, 06 Dec 2022 01:04:50 GMT  
		Size: 47.0 MB (47047090 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44b88e857f7530a93d2fc07e7656706e14a10a1b28d141df6696152c2cb97da5`  
		Last Modified: Tue, 06 Dec 2022 01:05:02 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:bookworm-backports` - linux; arm64 variant v8

```console
$ docker pull debian@sha256:35bb9a4c5de9f1e04b1538b4082037609697d8ab69615a0cb76102619c5cc84c
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.3 MB (50307939 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0922d255ea9d49477ff1f879a387562c94637e12fc861fdb57da215abd8c6758`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 06 Dec 2022 01:39:50 GMT
ADD file:de3ed89259c63b45a553c11db2206a6ca4201bfd264f04890af2c672736c15b4 in / 
# Tue, 06 Dec 2022 01:39:50 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 01:39:53 GMT
RUN echo 'deb http://deb.debian.org/debian bookworm-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:6d78ccc24e38e1c539440b7f90d65e136bba8366864c2b4a45e3956272709049`  
		Last Modified: Tue, 06 Dec 2022 01:43:02 GMT  
		Size: 50.3 MB (50307715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48f1eb438b590327d146af267824d7e54e637dd1aaec0b623363b2d91cd7ced1`  
		Last Modified: Tue, 06 Dec 2022 01:43:11 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:bookworm-backports` - linux; 386

```console
$ docker pull debian@sha256:a6b1650a3c3c6315c591bf68d39982c419b67dcb44fa1813db01ef320ada3fcf
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.3 MB (51301802 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e620548b7107e13a1fed372e6286e16a53d5884938ca57ebda5c0b3c7baa6051`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 06 Dec 2022 01:38:43 GMT
ADD file:6064ead20e3d5415784fcb74157c3ba1b90982f542deb132e9dabb2a1712e396 in / 
# Tue, 06 Dec 2022 01:38:44 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 01:38:50 GMT
RUN echo 'deb http://deb.debian.org/debian bookworm-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:45070d389a5ecd4dae6cdcb3e06567c8481416cfb2efb085e318fb5e2d11393b`  
		Last Modified: Tue, 06 Dec 2022 01:44:36 GMT  
		Size: 51.3 MB (51301574 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:452510896f2c0f42e67ee6e519831fa837963a53d4a14533687cef9ae422cb75`  
		Last Modified: Tue, 06 Dec 2022 01:44:46 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:bookworm-backports` - linux; mips64le

```console
$ docker pull debian@sha256:25eae21dca88b81f9f14ab4653221ccc1c630a519a966aa25e5035810f3124a2
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.3 MB (50259718 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3c2b1d688b16867c0c9365e4f55e0e3a1070d338407863b9a3e582dd86b6be68`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 06 Dec 2022 01:53:35 GMT
ADD file:5f771b53cd80db61f6fcf0df30ca6b99cd2c768f57ab1ffdf53d1f646b7db7c2 in / 
# Tue, 06 Dec 2022 01:53:41 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 01:53:52 GMT
RUN echo 'deb http://deb.debian.org/debian bookworm-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:a9cc4004cb6d73c258a4d864dabb35e2beb3272eaf0de591430b0bb1af15141c`  
		Last Modified: Tue, 06 Dec 2022 02:01:46 GMT  
		Size: 50.3 MB (50259491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04b1d7a6347f47776cc310d497861bbe6c03786ece4abedb16e964b812c0a101`  
		Last Modified: Tue, 06 Dec 2022 02:01:55 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:bookworm-backports` - linux; ppc64le

```console
$ docker pull debian@sha256:42c97ceee5752649009b441a9847323cd40a06b29a932332ca24b97973dcbde7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **54.3 MB (54319516 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:df5dbde1a1375c815d3bbd9bf8bc9f725f34f52bf63c191e59cfc5363e9ebf0b`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 06 Dec 2022 01:16:54 GMT
ADD file:394004d3191138471ba2dd50891718f9142a137ec9018f4f69a653139a98abf1 in / 
# Tue, 06 Dec 2022 01:16:57 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 01:17:03 GMT
RUN echo 'deb http://deb.debian.org/debian bookworm-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:c1206773e59171c1200c3692244202cc0da97f8fc41cb86ed64f742f1e75b47f`  
		Last Modified: Tue, 06 Dec 2022 01:22:51 GMT  
		Size: 54.3 MB (54319290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffe4173c0e797dc3324051f241bd58a315afae24c4c6afb993f92636cd546495`  
		Last Modified: Tue, 06 Dec 2022 01:23:01 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:bookworm-backports` - linux; s390x

```console
$ docker pull debian@sha256:ece5562f4b23308a5ad175e6ef3d09697f16f20b1264bc85fb2ca0596d63499b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.7 MB (48665129 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2d2b254bde7577742ab6e8757091dc8f0047147aae1188d9f3ca61528c802d97`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 06 Dec 2022 01:41:45 GMT
ADD file:45186e2067a128e8dbf3558a97cd5853548faaf7c2bb93ef1544ed66907fcf19 in / 
# Tue, 06 Dec 2022 01:41:55 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 01:42:07 GMT
RUN echo 'deb http://deb.debian.org/debian bookworm-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:effa21bde36181862f20d53853fc03e36421f6a13d6aad41051d593fe9c7c097`  
		Last Modified: Tue, 06 Dec 2022 01:47:58 GMT  
		Size: 48.7 MB (48664905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22ee34dc51c64e8fdb421345c317fa7c396250377fe19348938e5b95eb8c5d1e`  
		Last Modified: Tue, 06 Dec 2022 01:48:05 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
