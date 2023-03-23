## `debian:experimental`

```console
$ docker pull debian@sha256:c4ccf53f92a283f258e44d0401f6b33e752d55f5108ce5d78348858e604760a4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 9
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; mips64le
	-	linux; ppc64le
	-	linux; riscv64
	-	linux; s390x

### `debian:experimental` - linux; amd64

```console
$ docker pull debian@sha256:405ffbb05c843d9ee63a827e7e087d781486143853781ca5ed2c3ab7e6ac8c73
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.3 MB (49291856 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0362a5ecdf1c12b534a2fa65f409bf48830fcd26bc4439b193b01db48976980f`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Mar 2023 01:32:34 GMT
ADD file:1b3637ceb65f7a1169870ad9d3ea1fdba9ee5c010035b5ce5dcdccff245e3271 in / 
# Thu, 23 Mar 2023 01:32:34 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 01:32:47 GMT
RUN echo 'deb http://deb.debian.org/debian experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:d467901642e3ccafaa1073030f9f0e5b843eb159f3484cf34803049dd241d819`  
		Last Modified: Thu, 23 Mar 2023 01:37:26 GMT  
		Size: 49.3 MB (49291638 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73cb0295dabfda3e6054c805b74cdb7c35c24a822001285659738bb6d92fde81`  
		Last Modified: Thu, 23 Mar 2023 01:37:46 GMT  
		Size: 218.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:experimental` - linux; arm variant v5

```console
$ docker pull debian@sha256:3179a8c3a858f622fe52a61f2b2fb26388e39e0a21a0e0b5aff85221f8b05c8f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.1 MB (48107946 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2dda7d7a9ae00da59e82175de7bff20e7c7b2a46f14126d654778fb9493aa9ae`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 01:49:52 GMT
ADD file:c3e085c3dff5f8a26c459819fec4fdc2ea28a857d84f1b06ea2536ab2c11f178 in / 
# Wed, 01 Mar 2023 01:49:52 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 01:50:02 GMT
RUN echo 'deb http://deb.debian.org/debian experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:d9e0e6decf94a96d3649bc9614fd0ea25205676ea5004891847e53ead7e8b5f7`  
		Last Modified: Wed, 01 Mar 2023 01:55:14 GMT  
		Size: 48.1 MB (48107725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e529ac0697461ad7c874d3a0f17f7b81df8ad55567c76439918604add3a00d6`  
		Last Modified: Wed, 01 Mar 2023 01:55:39 GMT  
		Size: 221.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:experimental` - linux; arm variant v7

```console
$ docker pull debian@sha256:1b234c6233b7afba08e64d8fed0b498fd6d587292ebe0b5d0b1fc7137a1d3611
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.9 MB (45911410 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:27531f3094db3ee5b8ab4bf8f2034f81fe1a606315a89abda3282be6d1722cf7`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Mar 2023 01:31:37 GMT
ADD file:6285e1fe7d92d78fcb5fae1676105ce4fd1bcbaec70765b214e69c4eabbf66c0 in / 
# Thu, 23 Mar 2023 01:31:37 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 01:31:55 GMT
RUN echo 'deb http://deb.debian.org/debian experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:989cb2202895dc0cbd9bef2248c6675cbb620e0613235ac9c68edbd5e2ffeb24`  
		Last Modified: Thu, 23 Mar 2023 01:35:46 GMT  
		Size: 45.9 MB (45911190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e322471473b774638b4020dfb732a9b590ee609c4f38d65521d1178fa770cb1c`  
		Last Modified: Thu, 23 Mar 2023 01:36:07 GMT  
		Size: 220.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:experimental` - linux; arm64 variant v8

```console
$ docker pull debian@sha256:efc8c53c7e8ec804a3fdb97e5d41f1b87b6f03c1c262411cf5f14e7930fad5a4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.3 MB (49319208 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a64b496c658ef5ff8b09f4eb071f87a0192c7692fdbf8c883d0ea56c91adaeb9`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Mar 2023 00:46:25 GMT
ADD file:0affcb10430712dd73055564d3fe7c0548bcc203c6e8a0c200c4b48ba52900f8 in / 
# Thu, 23 Mar 2023 00:46:25 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 00:46:33 GMT
RUN echo 'deb http://deb.debian.org/debian experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:b400817afa0c1b0b5323fe5eb38a334172ba17ead32c49762767d869161603f4`  
		Last Modified: Thu, 23 Mar 2023 00:51:02 GMT  
		Size: 49.3 MB (49318987 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17e4cd8709e1cb452a702dbef9012d6bb8eaae94069e7e2436cb0ac527ed5856`  
		Last Modified: Thu, 23 Mar 2023 00:51:24 GMT  
		Size: 221.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:experimental` - linux; 386

```console
$ docker pull debian@sha256:715da7bbf5f20a42f1bf9e3965de1761da0a4fb3641e8d64f11006067e9f1b85
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.3 MB (50314767 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0d355426c99a7371bf868453a8ba6b543b110c4f84c4221ec52c2ed493d92e32`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Mar 2023 00:41:14 GMT
ADD file:91051a34bcb35ee9e94090f813b07bf915da58d01acb1e1a51031171a6eb0ce0 in / 
# Thu, 23 Mar 2023 00:41:15 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 00:41:27 GMT
RUN echo 'deb http://deb.debian.org/debian experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:350e50626198efaebb626c28f35f6aab6f02ce94e1bda1166f63672ca9c13303`  
		Last Modified: Thu, 23 Mar 2023 00:46:39 GMT  
		Size: 50.3 MB (50314547 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:562cf269bd2f25740bc81e36165a927c8907b0eb6d643c883ebf01dcc3adee47`  
		Last Modified: Thu, 23 Mar 2023 00:47:01 GMT  
		Size: 220.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:experimental` - linux; mips64le

```console
$ docker pull debian@sha256:fc93a8eeee50d7bf701c17102fe5cb17db6868127f799c58e304909d654f5624
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.3 MB (49270843 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c05fa24d6011f6260fbb995ca100cf36b4c6f24bdc1eff3d36882d878e3776d4`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 02:14:57 GMT
ADD file:3c9761555a5ea142351615b9c67fa1d733eb4055b0a7ce13452185d0a0569a8a in / 
# Wed, 01 Mar 2023 02:15:02 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 02:15:40 GMT
RUN echo 'deb http://deb.debian.org/debian experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:488a223217255f1854f177e926f43908918ca067d20ac1205a5c8058bacba304`  
		Last Modified: Wed, 01 Mar 2023 02:23:05 GMT  
		Size: 49.3 MB (49270620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f3335a1cbe608936e7e2ce0033bb81a3db2d76717e791d353e05fda95808900`  
		Last Modified: Wed, 01 Mar 2023 02:23:42 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:experimental` - linux; ppc64le

```console
$ docker pull debian@sha256:2ef40f30ef192cffa178120c568cff315853cfa18d08e667634c4c46b5301047
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.3 MB (53290400 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c5930622a4b98aebf8b3483fdc85757fc7305bb64213ff417997359366440be1`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Mar 2023 01:21:59 GMT
ADD file:808b8a3819489c1e18ada2afff40b9bba8a34535c43f85ef8aae58ca6d2b9823 in / 
# Thu, 23 Mar 2023 01:22:01 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 01:22:19 GMT
RUN echo 'deb http://deb.debian.org/debian experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:6baaac9eb72154b89f022853641e0f0edac59a2a458c00b652dfc45ac6f51b03`  
		Last Modified: Thu, 23 Mar 2023 01:27:02 GMT  
		Size: 53.3 MB (53290176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3771ce4e254bf1144fa7b3f88257f9a9a216320b2408814abfe8498048c62cb`  
		Last Modified: Thu, 23 Mar 2023 01:27:31 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:experimental` - linux; riscv64

```console
$ docker pull debian@sha256:c31917f1d6d85ddd1808759754ba41790aa1f40c4ca5f431571218319e639b5f
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.5 MB (45472107 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:627ec9f5662a91742bfab10555187804507360b96ced348a55a52df7167e932f`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Mar 2023 01:10:32 GMT
ADD file:8b0b9f137dae0117e3385ec198f10a572c548512aa4d1b425beffa76caab8ac9 in / 
# Thu, 23 Mar 2023 01:10:35 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 01:11:21 GMT
RUN echo 'deb http://deb.debian.org/debian-ports experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:2b1e83e0a2a836bebd540a6301be95b81bd79d6b21531518450432f6b0eddca4`  
		Last Modified: Thu, 23 Mar 2023 01:13:56 GMT  
		Size: 45.5 MB (45471881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c12c82849097c49ab31be8c272759ec2006de3fb31f194ae90913f57427c02f`  
		Last Modified: Thu, 23 Mar 2023 01:14:41 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:experimental` - linux; s390x

```console
$ docker pull debian@sha256:4946ca3720705048b10646de1f54f8721815c13b48f54535a3465ea8db6a8f5b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.6 MB (47648248 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ecb210152ae579ea153dd4c8c32cf41606fc0c7ec5d3ec25b3bdbed57caae101`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Mar 2023 00:45:40 GMT
ADD file:87a1c5a697c0ce402d70710d206bfb13b0399785b6b9120109f7099c256199a8 in / 
# Thu, 23 Mar 2023 00:45:43 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 00:45:56 GMT
RUN echo 'deb http://deb.debian.org/debian experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:bc794848966cb11ec8c207602b033a6a5b7e3c9334d0481e4d332bba4c4cd57a`  
		Last Modified: Thu, 23 Mar 2023 00:48:40 GMT  
		Size: 47.6 MB (47648028 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8efff8fb6d8c9f34679dad324583c9e11c7365702cc08af1adae4de7644503b6`  
		Last Modified: Thu, 23 Mar 2023 00:48:56 GMT  
		Size: 220.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
