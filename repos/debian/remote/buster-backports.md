## `debian:buster-backports`

```console
$ docker pull debian@sha256:a1bcbd6b7732f877813efd3c370968034a8e258475db67bda02a3ddbf00c05fe
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

### `debian:buster-backports` - linux; amd64

```console
$ docker pull debian@sha256:439aca1b758bbd40728cc542dbc8bf0d27ef9f74b57ae6dccd984c99a10c486b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.4 MB (50438136 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0557f80eb08043b6868e849227397fdac5a69766f18c283d4ce7563bf9832620`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 29 Mar 2022 00:22:28 GMT
ADD file:8c5e9f12fd3b6e830ec0ee1800d8e9dcebf217896148f2dc72c010c8a88d9b8f in / 
# Tue, 29 Mar 2022 00:22:28 GMT
CMD ["bash"]
# Tue, 29 Mar 2022 00:22:31 GMT
RUN echo 'deb http://deb.debian.org/debian buster-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:b281ebec60d2630a225601bd58a4681375a31b7316263b64d3b149f49694c3fe`  
		Last Modified: Tue, 29 Mar 2022 00:27:37 GMT  
		Size: 50.4 MB (50437915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1415ade0b18ce345ff3b9b5aebada7d253918e01dc292fb8d35d7ce5618bdcf`  
		Last Modified: Tue, 29 Mar 2022 00:27:51 GMT  
		Size: 221.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:buster-backports` - linux; arm variant v5

```console
$ docker pull debian@sha256:16abc31ed326e496142e224df22113b00bcff7e47018b374e41e212db6f1797c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.2 MB (48158518 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:65cdb69b067780a76b9ff0faaab853198c5ab3628c5224d497023c66d217391c`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 29 Mar 2022 00:51:04 GMT
ADD file:e7d31ee8f990df96d5922feb35173a364a0832e8fce2d32fd4e703aa3b66e1b2 in / 
# Tue, 29 Mar 2022 00:51:05 GMT
CMD ["bash"]
# Tue, 29 Mar 2022 00:51:19 GMT
RUN echo 'deb http://deb.debian.org/debian buster-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:0bbc2517bf9c8d842997ba8f85b59bfd92c5bb6bba79c39047eecda859dcae27`  
		Last Modified: Tue, 29 Mar 2022 01:06:08 GMT  
		Size: 48.2 MB (48158294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8553322fe47c91c358b468dbd0a3044575f748084ac4494eb8424c9f459589a9`  
		Last Modified: Tue, 29 Mar 2022 01:06:28 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:buster-backports` - linux; arm variant v7

```console
$ docker pull debian@sha256:9d6ae33115da8255d188a4a89f13bb7f382b6a3a855658f34df195d834494d42
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.9 MB (45914755 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:74815f2d1be3573d54846109729b2f328d0e8369fcc7dd590d0f80417f1f809a`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 29 Mar 2022 02:19:04 GMT
ADD file:60a690e302d164c569e6f3fc29adb6686618bb728249405f90960835525b0599 in / 
# Tue, 29 Mar 2022 02:19:06 GMT
CMD ["bash"]
# Tue, 29 Mar 2022 02:19:21 GMT
RUN echo 'deb http://deb.debian.org/debian buster-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:0cc72482f2e040b686190f2967010d45947924353440070552a298b9f9f81b19`  
		Last Modified: Tue, 29 Mar 2022 02:34:54 GMT  
		Size: 45.9 MB (45914531 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e39defb05ffe267d0f557d4480f2cd810605f297261e0c3b3decb998d605f040`  
		Last Modified: Tue, 29 Mar 2022 02:35:12 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:buster-backports` - linux; arm64 variant v8

```console
$ docker pull debian@sha256:abf0b203b33e41a960727aeefc4fd87795f422621327ce6be02542eb6068c8f9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.2 MB (49226121 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2f1043294add2f8b6db442c0f282f830a2ab98b6c5e06304b2cce2da8fe92c87`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 29 Mar 2022 00:43:27 GMT
ADD file:7686930f8c48390948992fbe39ce798cc57ee1d8785b3da70f4a3220f6e7b024 in / 
# Tue, 29 Mar 2022 00:43:28 GMT
CMD ["bash"]
# Tue, 29 Mar 2022 00:43:35 GMT
RUN echo 'deb http://deb.debian.org/debian buster-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:c732c99090fe64466c6911ecfdd8d4d3f6dfb183aab95d7746163bc49ebe35c9`  
		Last Modified: Tue, 29 Mar 2022 00:50:29 GMT  
		Size: 49.2 MB (49225896 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d111dadf26706b53f8b0149667c890d3053eb896fc9f06b38dfc706ad3c91909`  
		Last Modified: Tue, 29 Mar 2022 00:50:46 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:buster-backports` - linux; 386

```console
$ docker pull debian@sha256:3a5ab1d258b639d2405fe8963dad466e5dd0c7f819d12d7e8493664ad02d1847
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.2 MB (51206895 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:59a7384c06446a52efdf2c2480bfd86bde7edaa9206294b19a61b0815e9e7de6`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 29 Mar 2022 00:42:12 GMT
ADD file:fb2c1bf394c39b5bf948ceaa00317518326bd846b3f6802dc39cfb7fcf404c69 in / 
# Tue, 29 Mar 2022 00:42:13 GMT
CMD ["bash"]
# Tue, 29 Mar 2022 00:42:19 GMT
RUN echo 'deb http://deb.debian.org/debian buster-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:b86fabf064e35595b9c8543deb0dba50a95e438387a9877ebfe189bbfce3c87b`  
		Last Modified: Tue, 29 Mar 2022 00:49:34 GMT  
		Size: 51.2 MB (51206670 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bfe23327dd5caba42a116df14bd4ea3760634b9a61bd595abff1f871e49f555`  
		Last Modified: Tue, 29 Mar 2022 00:49:50 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:buster-backports` - linux; mips64le

```console
$ docker pull debian@sha256:748e57613ee0a85251b495192ca0be7b8ce0b162827a3410930450dd6373b3fe
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.1 MB (49079685 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ea0b306f6331622c0276853d2f22734d15bc8b6e657f50b09e7e1ed303a8fca3`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 17 Mar 2022 08:53:34 GMT
ADD file:a0b3ac9e4bfb39c253a8a7a55fb55d0b908af833cdcc9931837698ec5f55b989 in / 
# Thu, 17 Mar 2022 08:53:39 GMT
CMD ["bash"]
# Thu, 17 Mar 2022 08:53:51 GMT
RUN echo 'deb http://deb.debian.org/debian buster-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:047b7fb675b6ff99fd7dedbd4d0b0a3242855acbf0be0e3a69b39ea19852bf7f`  
		Last Modified: Thu, 17 Mar 2022 10:44:02 GMT  
		Size: 49.1 MB (49079461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cebf4134930b5b2738775b3830de7c70e6eea012e3661559644a85f27e7fffd5`  
		Last Modified: Thu, 17 Mar 2022 10:44:16 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:buster-backports` - linux; ppc64le

```console
$ docker pull debian@sha256:5fd45bd659da9d3e5b8897d81fdf4b3a0f11017c01f392052dbd302ba6630b25
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **54.2 MB (54183324 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:54094003436e79a10f102ff59d8c6291f07ea35eac8eb781d13a2068fc69daeb`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 29 Mar 2022 00:22:25 GMT
ADD file:a600709d679cffd058d04ba0eb0765cc870766fd5de083ada0eeccfd7afc21f8 in / 
# Tue, 29 Mar 2022 00:22:30 GMT
CMD ["bash"]
# Tue, 29 Mar 2022 00:22:41 GMT
RUN echo 'deb http://deb.debian.org/debian buster-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:eb53bdc4c2c6ececbd424b1c643b9877934a5297a5d2db0eca1a175d7a21d32e`  
		Last Modified: Tue, 29 Mar 2022 00:33:53 GMT  
		Size: 54.2 MB (54183100 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37331d5f6a5c9bab113bc51c20b3552f60051400199d23f089144d899945a13a`  
		Last Modified: Tue, 29 Mar 2022 00:34:11 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:buster-backports` - linux; s390x

```console
$ docker pull debian@sha256:ffc315a2d4d6ddcf44f3745dedfeb9ba71833cd559cf0b7981239424c14fb056
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.0 MB (49007977 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:668bff84c384e478dda3ce20530a8bf0b7678cf2f1388bab7bcbec17253d4342`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 29 Mar 2022 00:52:09 GMT
ADD file:784894d175880656ac82b485076fb224bde46d379dd634720acf7acd5eee9365 in / 
# Tue, 29 Mar 2022 00:52:11 GMT
CMD ["bash"]
# Tue, 29 Mar 2022 00:52:19 GMT
RUN echo 'deb http://deb.debian.org/debian buster-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:e3cc532be5698da8ac6589c11495b960fec83fd52aa82617e3218678ff4546d1`  
		Last Modified: Tue, 29 Mar 2022 01:07:20 GMT  
		Size: 49.0 MB (49007755 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5250cfe615d62a1c3259121f77ba2c411b2c2c253d29df51feb4b5e171c02779`  
		Last Modified: Tue, 29 Mar 2022 01:09:27 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
