## `debian:bullseye-backports`

```console
$ docker pull debian@sha256:d2f62a9b0518ddead5a1f88ce66cb6237a7cb90caae56a2525f031425f788c7d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; mips64le
	-	linux; ppc64le
	-	linux; s390x

### `debian:bullseye-backports` - linux; amd64

```console
$ docker pull debian@sha256:ad2d870e3052164597ec16b9bc8e999fc98f9fe4e58bf0f8dbf471a85414545e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **54.9 MB (54868314 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b2350fdb6de7c6e8e2dc196f5a7b521656963ba89df41fa7140922a945dff660`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 30 Mar 2021 21:48:53 GMT
ADD file:32519b03930d9f5db9010ae49e0987322ce19eab681ad5c841fe1cd6268ad2ee in / 
# Tue, 30 Mar 2021 21:48:53 GMT
CMD ["bash"]
# Tue, 30 Mar 2021 21:48:58 GMT
RUN echo 'deb http://deb.debian.org/debian bullseye-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:6abc78d8e2422868f293b265b6c0ec3ba250fc4987f862ba05e86d7eb277f297`  
		Last Modified: Tue, 30 Mar 2021 21:52:53 GMT  
		Size: 54.9 MB (54868089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a63f50eabcf69951c420da93d75581f0da2900446ee4e3e88e7fe27990d5c87d`  
		Last Modified: Tue, 30 Mar 2021 21:53:05 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:bullseye-backports` - linux; arm variant v5

```console
$ docker pull debian@sha256:60a7f72b36a2e28c723a4c6dfd6998f85c47b718bad21fee3313c6b7e45e5321
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.4 MB (52401397 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e382afecccbb464151e6387fe82534ed86b99bb21b426c41bce304d7c7a89192`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 30 Mar 2021 21:49:55 GMT
ADD file:3a982d4cdc7d9461623d85a4b6162531ca9adf2921f0d43a0b548d3710392387 in / 
# Tue, 30 Mar 2021 21:49:57 GMT
CMD ["bash"]
# Tue, 30 Mar 2021 21:50:05 GMT
RUN echo 'deb http://deb.debian.org/debian bullseye-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:645891123da6b320ad4fd8cfadf96c77b7144dd25b617222de1fe718cde77e35`  
		Last Modified: Tue, 30 Mar 2021 21:57:27 GMT  
		Size: 52.4 MB (52401170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2eb276f2c11af26f3ed2a151a0e714d73c0b97398211e2a5b3b00d2dd27c7324`  
		Last Modified: Tue, 30 Mar 2021 21:57:39 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:bullseye-backports` - linux; arm variant v7

```console
$ docker pull debian@sha256:eb385f6d88087236ff1f4a29475ce9b0414b5858a866d124f55dc2fd1102c080
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.1 MB (50069431 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8fe01b8711f1c443d473857061640151a03519ce18fe2adf15209716ed588d25`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 30 Mar 2021 23:07:05 GMT
ADD file:81d46e360628ea35bb1ec870f07ccb5c7722c2af2296557ac007f32663ef1cec in / 
# Tue, 30 Mar 2021 23:07:09 GMT
CMD ["bash"]
# Tue, 30 Mar 2021 23:07:24 GMT
RUN echo 'deb http://deb.debian.org/debian bullseye-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:c62a7336a784ff2e5eceb7d0da019a0022517c331efaef6fb92eca67135c6ac0`  
		Last Modified: Tue, 30 Mar 2021 23:15:13 GMT  
		Size: 50.1 MB (50069202 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4882f870b09df72a48457cf92eb74b2419a0e02e0afbc25ac08ca59935ba0081`  
		Last Modified: Tue, 30 Mar 2021 23:15:22 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:bullseye-backports` - linux; arm64 variant v8

```console
$ docker pull debian@sha256:c85b41ccf4b9e49c11fdbb514fb7b1b6641b6e8f6b6895f6292b74848e958475
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.6 MB (53555424 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a28bb97a52e4f5671307467a16b60cb0223e461332393d4be753aa6f07dd6854`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 30 Mar 2021 21:46:09 GMT
ADD file:d2b87aea7c45e4b0e478e3c2eabae00f1c80b5d77f8f579d2ff913c78b44b6b0 in / 
# Tue, 30 Mar 2021 21:46:12 GMT
CMD ["bash"]
# Tue, 30 Mar 2021 21:46:21 GMT
RUN echo 'deb http://deb.debian.org/debian bullseye-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:1063bcb9135253bd841aad1946f348a3277d992a7ecba4ef1ef68217c3c1b019`  
		Last Modified: Tue, 30 Mar 2021 21:53:23 GMT  
		Size: 53.6 MB (53555197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b30dbaf2556d1264fd4a37234ee0aa37061664b22e97e6a2882ae14d1b43de9`  
		Last Modified: Tue, 30 Mar 2021 21:53:31 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:bullseye-backports` - linux; 386

```console
$ docker pull debian@sha256:3f9734fadcb24977da54730f41689914c812feb4acf07aff0c5377b8ff0d6c91
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **55.9 MB (55881541 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ab83f3d384e97e7d8a9437d82c746b5e7d027ed15e00f52ddb89a042d4c60474`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 30 Mar 2021 21:38:58 GMT
ADD file:b5024008ca4ac295c015d04d146515efd534f38efa8793979ad8a6c1cc41a2b8 in / 
# Tue, 30 Mar 2021 21:38:59 GMT
CMD ["bash"]
# Tue, 30 Mar 2021 21:39:05 GMT
RUN echo 'deb http://deb.debian.org/debian bullseye-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:46dc83097f0241a9cf1128d563661cf2cacf0ca9445152008a4c686a8d125595`  
		Last Modified: Tue, 30 Mar 2021 21:45:11 GMT  
		Size: 55.9 MB (55881315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f81e15a51b68c9400faed178786854015175b8535655292e5517f381024cff3e`  
		Last Modified: Tue, 30 Mar 2021 21:45:28 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:bullseye-backports` - linux; mips64le

```console
$ docker pull debian@sha256:51dd493c5875ed0e6e9d355bd75e4669122b471994432422e140958f971b603d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.1 MB (53127413 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8efddf034c6e499a298d27827b1220b484050869b651a0cea935f71ddf113b57`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 30 Mar 2021 22:08:38 GMT
ADD file:4c1773eeb1eb8715f5ee35943b6ec536fef99670907da849b45a0a757fbba521 in / 
# Tue, 30 Mar 2021 22:08:39 GMT
CMD ["bash"]
# Tue, 30 Mar 2021 22:08:44 GMT
RUN echo 'deb http://deb.debian.org/debian bullseye-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:a1bfb759abe39ebb60de9072afdd4e8e520a2faad8d254176313a6e6015b23b2`  
		Last Modified: Tue, 30 Mar 2021 22:14:13 GMT  
		Size: 53.1 MB (53127187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2993ece578bb8207a028ee65980e435e802351957d0e261aac4f94cd976061aa`  
		Last Modified: Tue, 30 Mar 2021 22:14:24 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:bullseye-backports` - linux; ppc64le

```console
$ docker pull debian@sha256:32b8f290fa40c26088b1a98fb480a4d5e45df8c1db1e9d82389099b814c77236
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **58.8 MB (58783591 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e132d65c707343a9c2a30e280bc84da93ce9c3fb185c92336e5d9eb269e01069`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 30 Mar 2021 22:33:49 GMT
ADD file:b2e7a11ad622cae2b5772745c60f7e97c6bf288f72404afbcaf250515017a2e4 in / 
# Tue, 30 Mar 2021 22:34:07 GMT
CMD ["bash"]
# Tue, 30 Mar 2021 22:34:35 GMT
RUN echo 'deb http://deb.debian.org/debian bullseye-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:6eaed89d6188915a9c2274bc56b9635ae1ea5b1e77d1120748b46640f4765416`  
		Last Modified: Tue, 30 Mar 2021 22:41:14 GMT  
		Size: 58.8 MB (58783363 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddfb31ccc4d04b01a1826df4cec7bb416d94381f9a9d9f624a779b9d415b4c52`  
		Last Modified: Tue, 30 Mar 2021 22:41:25 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:bullseye-backports` - linux; s390x

```console
$ docker pull debian@sha256:7a8e3d1955819a927544399147899126c9d65bc19c91f5aad498a4456df9b87b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.1 MB (53148677 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5e5237c5a3bd3ac44c80948cada8662faa00a4fe1d9255b7928fc14846f237ad`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 30 Mar 2021 21:42:00 GMT
ADD file:06cd9dd574d91229d3aa7c645dda03791fcfbea17bb5964aaa1c5830d4174ab2 in / 
# Tue, 30 Mar 2021 21:42:06 GMT
CMD ["bash"]
# Tue, 30 Mar 2021 21:42:11 GMT
RUN echo 'deb http://deb.debian.org/debian bullseye-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:1babe08b94dd6b44aca97f5f46b49d3c3e8b1571a49971cc87c69f9c91056218`  
		Last Modified: Tue, 30 Mar 2021 21:45:29 GMT  
		Size: 53.1 MB (53148454 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cecfe71bc973ccb32d8f12c81032c52a08cb2bb245c555b1157c09ff60a2255`  
		Last Modified: Tue, 30 Mar 2021 21:45:39 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
