## `debian:rc-buggy`

```console
$ docker pull debian@sha256:9da4be4ff2b9b1f2c6cf23118a570d5dcc063b14fde8537a2b730e965dde4444
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

### `debian:rc-buggy` - linux; amd64

```console
$ docker pull debian@sha256:ba560aa422c54c440912dda300abe4fe299a61ee2739ef4f632a24cab827a810
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.6 MB (50641454 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:117ea039b9c5209f2b9978e52bed53c34d34f66ace5c5af857e662fc163cd14c`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 01:44:41 GMT
ADD file:635f36e1a46e6c28b2a6ab0637cca9e47837c3547b17916d1dbb2595fbeb0821 in / 
# Tue, 25 Oct 2022 01:44:41 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 01:45:53 GMT
RUN echo 'deb http://deb.debian.org/debian rc-buggy main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:d90f8b044e56f2589b41d1fe9b249b85bde027855731c6f512f0f9401c99e68d`  
		Last Modified: Tue, 25 Oct 2022 01:49:42 GMT  
		Size: 50.6 MB (50641226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67a01cb3408bd32f8e1becd0ff9a98c693f2466f55cc745fa93ea1d980b25730`  
		Last Modified: Tue, 25 Oct 2022 01:51:59 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:rc-buggy` - linux; arm variant v5

```console
$ docker pull debian@sha256:a1b49c160c97c73a4b1e1872449b05f5d8642d4b95373f43c1e9dc10d1a8ae45
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.6 MB (51569195 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0bccd0736a85739b278cb847886a30e9c8cf5311bf05d86a5e598f479f957944`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:49:23 GMT
ADD file:5da40917ed11781002a72811aeac4336d50b3100f4e25213b5b18cb733468d31 in / 
# Tue, 04 Oct 2022 23:49:24 GMT
CMD ["bash"]
# Tue, 04 Oct 2022 23:50:52 GMT
RUN echo 'deb http://deb.debian.org/debian rc-buggy main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:f013d31fa02ab56c7186e21477e4fd559e7e9de70eb511ed30a523990b759421`  
		Last Modified: Tue, 04 Oct 2022 23:54:20 GMT  
		Size: 51.6 MB (51568969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcecf905bf4ea0e86e572177f159c12d6f5f6077df922b5ef6773dd356709eeb`  
		Last Modified: Tue, 04 Oct 2022 23:57:02 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:rc-buggy` - linux; arm variant v7

```console
$ docker pull debian@sha256:99014b01db49afcf62fcb923122a39df0447dc1134150cf523dcedf64cb33c14
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.4 MB (49437051 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9fc4625073d748ea038496eb07f7f1739fc9a730a3d86323cf96282168ba3105`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 05 Oct 2022 00:00:01 GMT
ADD file:41046e966f37a45410c2aa02920b78f877f5aacb6ee087b2c6c6642f4e7b474f in / 
# Wed, 05 Oct 2022 00:00:02 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 00:01:47 GMT
RUN echo 'deb http://deb.debian.org/debian rc-buggy main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:1316bf5b10f256f27feadcb25edef6365e912773e60cc382610ef003daf37248`  
		Last Modified: Wed, 05 Oct 2022 00:07:10 GMT  
		Size: 49.4 MB (49436823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f562fd3c57015abcfd7b4b84a8eef9268c5c328c78b0182e624804df75ebf8ff`  
		Last Modified: Wed, 05 Oct 2022 00:09:44 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:rc-buggy` - linux; arm64 variant v8

```console
$ docker pull debian@sha256:17115d693f904fe6511c16789e9cda108d5fa45a6537c846de4f07eebe1c1b15
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.7 MB (52700217 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:300126ce4428ccf8e87403a800adb75b0f14150dc9843ffc7c1b9ca92e7ce50a`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:45:47 GMT
ADD file:28797d8b43689eae5ccab5b01e88b732a5fca655590a0c9f066d6f0a4d880a95 in / 
# Tue, 04 Oct 2022 23:45:48 GMT
CMD ["bash"]
# Tue, 04 Oct 2022 23:47:23 GMT
RUN echo 'deb http://deb.debian.org/debian rc-buggy main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:6499ab100dbfb0305e0d96b62f7ad515906275ab30864ac686f0af8ff2fdd114`  
		Last Modified: Tue, 04 Oct 2022 23:52:17 GMT  
		Size: 52.7 MB (52699991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7fa1b32b89f1cb5e8dbba6c500ab3d2f8563c9e77fc4d3fd9e73489a1f1d59b`  
		Last Modified: Tue, 04 Oct 2022 23:54:46 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:rc-buggy` - linux; 386

```console
$ docker pull debian@sha256:e439ba7130b91cf47c8b5654e93bf53b12164f26a1e570d5b6c38f45d162d5e7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.6 MB (53647693 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6922430462cc2d0bd06caafaca2b0338bf56b7323bfb7a147a301b9fad1ffc63`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:40:48 GMT
ADD file:ea6d247c762f6294c87144d1a4308c30669e9e732bd8ff9ef892c71d14563165 in / 
# Tue, 04 Oct 2022 23:40:49 GMT
CMD ["bash"]
# Tue, 04 Oct 2022 23:42:26 GMT
RUN echo 'deb http://deb.debian.org/debian rc-buggy main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:8a0d07a7940ebb4ded014cd2eaedc6b9aa8767ff5afeee7b1b09fce7cbd7a31e`  
		Last Modified: Tue, 04 Oct 2022 23:47:29 GMT  
		Size: 53.6 MB (53647464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34bed5bb8d25ff41eb16dc665b799c5e40a35043aeaade4a5040594066b07b49`  
		Last Modified: Tue, 04 Oct 2022 23:49:59 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:rc-buggy` - linux; mips64le

```console
$ docker pull debian@sha256:93ef5a3ac4fe5b4333917e97f67d2d79e5a0abbd2fa5e2926725c013359c3add
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.7 MB (52670216 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:531fb0bca6ab75245f982a9c93b77c4c8f43100b136b14e2903c310ba125a6e2`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 05 Oct 2022 00:11:00 GMT
ADD file:a7d6f7226093388fbc662c6e3fa1bc8dc263ab630fe03ea088486e6b016474ff in / 
# Wed, 05 Oct 2022 00:11:04 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 00:15:23 GMT
RUN echo 'deb http://deb.debian.org/debian rc-buggy main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:3110bff10f823ecdaa06d8f7c65ce83d7c99521680207da9d264aaa8823d5209`  
		Last Modified: Wed, 05 Oct 2022 00:19:21 GMT  
		Size: 52.7 MB (52669988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0911df4892c615f0fc7d1bd0d162622a27988905786a1d268cdfd0d94926ff4e`  
		Last Modified: Wed, 05 Oct 2022 00:23:58 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:rc-buggy` - linux; ppc64le

```console
$ docker pull debian@sha256:9adc2e1d0a83137bbf54b8a02f2cd58d5fca58f6b1210ccd5526c6253fb7f22a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **56.8 MB (56786993 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5472a7ea049296464b324e2b07c6ab26d6a01eb0f6b4ca91717d38ba8e7b15cb`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:18:23 GMT
ADD file:9a1fd28de3c910076975890aa736e3f3bbff1b433c668f4121cf52af264cd06b in / 
# Tue, 04 Oct 2022 23:18:26 GMT
CMD ["bash"]
# Tue, 04 Oct 2022 23:20:57 GMT
RUN echo 'deb http://deb.debian.org/debian rc-buggy main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:a99fd400e2fbb8830bde6fd270def7df44ad1a841ec4e7cb5f33d7f5661d181a`  
		Last Modified: Tue, 04 Oct 2022 23:24:45 GMT  
		Size: 56.8 MB (56786765 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05e9166ff6954f2a2b4828fa3667f0f4b55fe356f8061afb6bbe04823037829f`  
		Last Modified: Tue, 04 Oct 2022 23:28:05 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:rc-buggy` - linux; s390x

```console
$ docker pull debian@sha256:e5820ed8d0cb96d731ae6fcaa30387956dc6a3e1dc6c0d3ab3422794874daa85
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.0 MB (49013200 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:44f1782aac87e5db1bf4bccca5a0092fdb518efd3ec8cf43bf398ee3edd0bb27`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 01:14:54 GMT
ADD file:7dba2ae439c9f5da3fe962e867cee94eafc0b12a74939e13fdf987965ef8191c in / 
# Tue, 25 Oct 2022 01:14:57 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 01:16:40 GMT
RUN echo 'deb http://deb.debian.org/debian rc-buggy main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:1430653806baea9ab2928a0d226c10ba8e7bf4b9b93398f9082ba16edfb2d4b8`  
		Last Modified: Tue, 25 Oct 2022 01:19:17 GMT  
		Size: 49.0 MB (49012977 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44c1767501079f5541e1767fe7c7ad7d6065fa06797b104712dabc65166177d6`  
		Last Modified: Tue, 25 Oct 2022 01:21:06 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
