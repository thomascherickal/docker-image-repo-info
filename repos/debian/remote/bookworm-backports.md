## `debian:bookworm-backports`

```console
$ docker pull debian@sha256:a9bc5f26d88c56f6d9df387b7564293232caa0f07bbcd2684b8d12ce8d776b71
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
$ docker pull debian@sha256:0445b366d7ec0d457e1aa3307e6b38272e5179ed234e6693c9a3108a69bb74c6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.3 MB (50324694 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d75455b18dc011b515e8033d25ddef5a258fc537b6f2424001df0b0acb890b89`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 21 Dec 2022 01:20:01 GMT
ADD file:5498bb69da6f2fdd15556904d80120042d5bb48f73fc9f20a2d1bd5a908e0017 in / 
# Wed, 21 Dec 2022 01:20:02 GMT
CMD ["bash"]
# Wed, 21 Dec 2022 01:20:05 GMT
RUN echo 'deb http://deb.debian.org/debian bookworm-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:2eed4289b3de645a7af9bc81fe7c50d50a1c7aae044a61e100a676b9e6224267`  
		Last Modified: Wed, 21 Dec 2022 01:23:37 GMT  
		Size: 50.3 MB (50324468 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f1d3835c88afe761e9763b62614587c46628d4d902ec9e45d98591161f2367a`  
		Last Modified: Wed, 21 Dec 2022 01:23:45 GMT  
		Size: 226.0 B  
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
$ docker pull debian@sha256:f91715cf01aa1d7f1628caddaf4db50c48e0be8aea4a531c0173d30add8079d9
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.3 MB (50336974 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ed4fabd5e9d86299c96c9ac3091d77a5ecfcc7d65a65ff7fd8b29f045d5ae0b6`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 21 Dec 2022 01:08:43 GMT
ADD file:b2458569ae73892acee2eab6d63bd5fac233b8f2939355fc7605c8906c1bbd30 in / 
# Wed, 21 Dec 2022 01:08:49 GMT
CMD ["bash"]
# Wed, 21 Dec 2022 01:08:59 GMT
RUN echo 'deb http://deb.debian.org/debian bookworm-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:63a99937a40bd4c10c6b0d4be0826a18d963fdd5ca9c794853e98ca819d68691`  
		Last Modified: Wed, 21 Dec 2022 01:16:43 GMT  
		Size: 50.3 MB (50336746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d129eb990c579f00619b717b3bd5a5d11e01e6b1517e507c672a24aa6a64ab9`  
		Last Modified: Wed, 21 Dec 2022 01:16:52 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:bookworm-backports` - linux; ppc64le

```console
$ docker pull debian@sha256:2c292d3815d7c2a64edf80094603daa2127deab04d7d095aa18e8b4beb611964
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **54.4 MB (54374050 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4858a17369cb0fdc49cfa1bd57c25e43552a040eefc736ef220c084f003e6e97`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 21 Dec 2022 01:16:40 GMT
ADD file:ddf53eeecd4e99f9ac6dd446b84eed33212dae1b2a9476907b99dc988c316e5e in / 
# Wed, 21 Dec 2022 01:16:44 GMT
CMD ["bash"]
# Wed, 21 Dec 2022 01:16:52 GMT
RUN echo 'deb http://deb.debian.org/debian bookworm-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:9a50dadcc8beda7926088df1652aba274c8cf1817cd6956a9342f3b25db470e6`  
		Last Modified: Wed, 21 Dec 2022 01:21:57 GMT  
		Size: 54.4 MB (54373822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fafe0cefc253c2a47e3ab3d7dfcceee7b73c5ffb4ee1c2294eeac56c5c147ed8`  
		Last Modified: Wed, 21 Dec 2022 01:22:07 GMT  
		Size: 228.0 B  
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
