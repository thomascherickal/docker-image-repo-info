<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `archlinux`

-	[`archlinux:base`](#archlinuxbase)
-	[`archlinux:base-20220724.0.70393`](#archlinuxbase-20220724070393)
-	[`archlinux:base-devel`](#archlinuxbase-devel)
-	[`archlinux:base-devel-20220724.0.70393`](#archlinuxbase-devel-20220724070393)
-	[`archlinux:latest`](#archlinuxlatest)

## `archlinux:base`

```console
$ docker pull archlinux@sha256:5679ee886aa411a371147a95667fa74c26819197f6d52c673201100c134e0b60
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `archlinux:base` - linux; amd64

```console
$ docker pull archlinux@sha256:c40bbb2c68ce6128f762d0cce87c80fcd5be40048c1df0cc5cf4c662300766ff
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.4 MB (127390377 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:317e584e3c26ecf862bb8b5662db75d5564bb041a55e08fe60621c11686b3dd6`
-	Default Command: `["\/usr\/bin\/bash"]`

```dockerfile
# Mon, 18 Jul 2022 18:24:20 GMT
COPY dir:11b761f1b802cdfda693c5153e66230180b5c81784ddc972fc678a956a5364ef in / 
# Mon, 18 Jul 2022 18:24:22 GMT
RUN ldconfig &&     sed -i '/BUILD_ID/a VERSION_ID=TEMPLATE_VERSION_ID' /etc/os-release
# Mon, 18 Jul 2022 18:24:22 GMT
ENV LANG=C.UTF-8
# Mon, 18 Jul 2022 18:24:22 GMT
CMD ["/usr/bin/bash"]
```

-	Layers:
	-	`sha256:8ed695e65781f424db075f6696f419bbdf8c64e86806b03b41880aa42355bf8d`  
		Last Modified: Mon, 18 Jul 2022 18:26:03 GMT  
		Size: 127.4 MB (127382826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05ecfa4e94531ad7b63b2c1cb26b9658b1e8421ca818e3089e979504eeb9a4de`  
		Last Modified: Mon, 18 Jul 2022 18:25:43 GMT  
		Size: 7.6 KB (7551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `archlinux:base-20220724.0.70393`

**does not exist** (yet?)

## `archlinux:base-devel`

```console
$ docker pull archlinux@sha256:595be001ae6ce5e4ed1e83056cf007bde6193835062bd8cb2d78113b8091298b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `archlinux:base-devel` - linux; amd64

```console
$ docker pull archlinux@sha256:bd9fd97df8c6ea0048df745bdbdc3a67a23c1ced5cbc5833ee0bfeb383d71b82
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **223.8 MB (223784491 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:872725140a4ba0f73d785675b6d62648416479a74adb7739f9a1822f17885e22`
-	Default Command: `["\/usr\/bin\/bash"]`

```dockerfile
# Mon, 18 Jul 2022 18:25:21 GMT
COPY dir:3a91d5869d166e8400cda2be2e1fb4b4f4a6e1e1d896aa69b037306a4a7e1a26 in / 
# Mon, 18 Jul 2022 18:25:24 GMT
RUN ldconfig &&     sed -i '/BUILD_ID/a VERSION_ID=TEMPLATE_VERSION_ID' /etc/os-release
# Mon, 18 Jul 2022 18:25:24 GMT
ENV LANG=C.UTF-8
# Mon, 18 Jul 2022 18:25:24 GMT
CMD ["/usr/bin/bash"]
```

-	Layers:
	-	`sha256:d5fbd488eb038da4cbb8c29dc282f92ce3145dbf078f408d9ee596195e08345a`  
		Last Modified: Mon, 18 Jul 2022 18:26:51 GMT  
		Size: 223.8 MB (223776321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a894abae66fa66e2041bf2eeb5242b381ab0602c969b218b4fbb8e4c109acedb`  
		Last Modified: Mon, 18 Jul 2022 18:26:15 GMT  
		Size: 8.2 KB (8170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `archlinux:base-devel-20220724.0.70393`

**does not exist** (yet?)

## `archlinux:latest`

```console
$ docker pull archlinux@sha256:5679ee886aa411a371147a95667fa74c26819197f6d52c673201100c134e0b60
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `archlinux:latest` - linux; amd64

```console
$ docker pull archlinux@sha256:c40bbb2c68ce6128f762d0cce87c80fcd5be40048c1df0cc5cf4c662300766ff
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.4 MB (127390377 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:317e584e3c26ecf862bb8b5662db75d5564bb041a55e08fe60621c11686b3dd6`
-	Default Command: `["\/usr\/bin\/bash"]`

```dockerfile
# Mon, 18 Jul 2022 18:24:20 GMT
COPY dir:11b761f1b802cdfda693c5153e66230180b5c81784ddc972fc678a956a5364ef in / 
# Mon, 18 Jul 2022 18:24:22 GMT
RUN ldconfig &&     sed -i '/BUILD_ID/a VERSION_ID=TEMPLATE_VERSION_ID' /etc/os-release
# Mon, 18 Jul 2022 18:24:22 GMT
ENV LANG=C.UTF-8
# Mon, 18 Jul 2022 18:24:22 GMT
CMD ["/usr/bin/bash"]
```

-	Layers:
	-	`sha256:8ed695e65781f424db075f6696f419bbdf8c64e86806b03b41880aa42355bf8d`  
		Last Modified: Mon, 18 Jul 2022 18:26:03 GMT  
		Size: 127.4 MB (127382826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05ecfa4e94531ad7b63b2c1cb26b9658b1e8421ca818e3089e979504eeb9a4de`  
		Last Modified: Mon, 18 Jul 2022 18:25:43 GMT  
		Size: 7.6 KB (7551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
