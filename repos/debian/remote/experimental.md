## `debian:experimental`

```console
$ docker pull debian@sha256:23f6d97fc38b5a8e9dce33219885abc23ef73d95df871a339c5bf26c47c1156c
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
$ docker pull debian@sha256:a9926b972c5282b62296a2d0179d9eb0f8a0351cf4c19acaba5b7dc42fd98ac9
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **54.9 MB (54931136 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2909206d6b9ffe5920147035c814f42dab78f18d5b50f2e03ef52a5a8e07bf8b`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Aug 2021 01:26:48 GMT
ADD file:5c6ab93e85d632a9bca0b5c303c89f467d80be62c90b71f74965e7fba4a8a2b0 in / 
# Tue, 17 Aug 2021 01:26:48 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 01:27:04 GMT
RUN echo 'deb http://deb.debian.org/debian experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:76d3fc4613014e340f469ffd4d5ae6c3582728c7b4330ffee95271b4f3ca9904`  
		Last Modified: Tue, 17 Aug 2021 01:34:27 GMT  
		Size: 54.9 MB (54930914 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a857f4b824d7fc9e87e82ebca89f9ac420bc6fc58b01353b304c3b6b806311f8`  
		Last Modified: Tue, 17 Aug 2021 01:34:51 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:experimental` - linux; arm variant v5

```console
$ docker pull debian@sha256:452a491f0cca558ccbbf9ecf578a3fee92cbc361ca68f4f0e98f2b15eaf62d6f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.4 MB (52446220 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9cfab69fa43a9c5c87f0dc74835a417e4475afa7a15368afb8d8c936b50fa29f`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 22 Jul 2021 00:54:58 GMT
ADD file:130a56cc4f62c5f99992b40717d91aee59653029881066d5d2f6aa90f3c534c2 in / 
# Thu, 22 Jul 2021 00:55:01 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 00:55:33 GMT
RUN echo 'deb http://deb.debian.org/debian experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:02fd227d65b202bd21ad9f318e3bd4c2fb7fdadef762296f692a14c87e4287eb`  
		Last Modified: Thu, 22 Jul 2021 01:09:14 GMT  
		Size: 52.4 MB (52445996 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f120935126b6f6a1ef8ef39b08cb2d4a7b9fbbc2713d6740f87e50da689417c`  
		Last Modified: Thu, 22 Jul 2021 01:09:57 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:experimental` - linux; arm variant v7

```console
$ docker pull debian@sha256:abaff37bdbcfadac2191c85bbef15b846e077a978e26863c8b9877e29bd38d32
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.1 MB (50112070 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:135d1d4fc916136756d99355250e694ad1a7192f45a31d20a8a6e94d3502c88c`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 22 Jul 2021 02:08:55 GMT
ADD file:1b3b77d60136df3dd46ae0ea23986c26640584a24bfe5dac4d8082fb81cec664 in / 
# Thu, 22 Jul 2021 02:08:56 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 02:09:29 GMT
RUN echo 'deb http://deb.debian.org/debian experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:f75829fe215f0952fcc8ef08bca0bd5050b0fcf9e8474e54e9d8fea9965d044e`  
		Last Modified: Thu, 22 Jul 2021 02:23:18 GMT  
		Size: 50.1 MB (50111847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d924350570e995b7707a22fedebf98816aef7fa43458322e39d0c51ee0d410b4`  
		Last Modified: Thu, 22 Jul 2021 02:23:57 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:experimental` - linux; arm64 variant v8

```console
$ docker pull debian@sha256:31bcdd1f1066632bedeb3ffd18006188de1b07613c968356c7bf80f6f3eb342a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.6 MB (53626199 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:43fac464b70feed4b1e3fac566a9cecffc14f72f72953612eaac9ae006db604d`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Aug 2021 01:49:09 GMT
ADD file:b9819fae5095c7caca0fdcf95465467d42b822e7124c65736a1cb2d67dee160d in / 
# Tue, 17 Aug 2021 01:49:09 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 01:49:25 GMT
RUN echo 'deb http://deb.debian.org/debian experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:cd13f173636041cac087fa5da0d6280d3521d873d67b6ca22df8aefb6e658a84`  
		Last Modified: Tue, 17 Aug 2021 01:59:07 GMT  
		Size: 53.6 MB (53625979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f06f6aa1943b0ada30f74f97d151d29735a4c55620d19ecc9bed90c6f219c3d`  
		Last Modified: Tue, 17 Aug 2021 01:59:34 GMT  
		Size: 220.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:experimental` - linux; 386

```console
$ docker pull debian@sha256:5281b28b70f2e435344623cf46f0ba055b7a817c233e7c86c343bca21e3e5eda
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **56.0 MB (55967755 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b59897d7fc843d2acc06ce8496d4a3bf309e495506e0ce416cffa8a7d2104d9b`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Aug 2021 01:44:56 GMT
ADD file:67fac40d64a5cd52b6df0358095887724aed1af79ac5417c6cd983105e4e60f1 in / 
# Tue, 17 Aug 2021 01:44:57 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 01:45:16 GMT
RUN echo 'deb http://deb.debian.org/debian experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:83d474e24cc84976cdb2a36e91c1882977193c775a79c96eb4b5fb83b731180a`  
		Last Modified: Tue, 17 Aug 2021 01:56:41 GMT  
		Size: 56.0 MB (55967536 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:491d95b2b9423a56cc799f94bf9d32b443353e5c5f2b405df209a8b0c166d5eb`  
		Last Modified: Tue, 17 Aug 2021 01:57:11 GMT  
		Size: 219.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:experimental` - linux; mips64le

```console
$ docker pull debian@sha256:025ccf60e7c0a8385ae770005761fe3fd4b39442125498bac4f846a4445cead3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.2 MB (53199152 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8b1ed7e119cd7363ac78cbede7c7a0f3a4ca3939d29130a032482d79bdc035d4`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Aug 2021 01:16:28 GMT
ADD file:48e5b05cf283544dc35f072181f4a55c3e89adb0c144d0be1cccf02096803234 in / 
# Tue, 17 Aug 2021 01:16:29 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 01:16:59 GMT
RUN echo 'deb http://deb.debian.org/debian experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:b83d70b8fe3ec57fc4141af74d540f46a12bffd87b41e68306f5fff6f9631360`  
		Last Modified: Tue, 17 Aug 2021 01:27:42 GMT  
		Size: 53.2 MB (53198928 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa3fa5f16867c7618494f95c6e9c3f36587d9d72d61af719d8d18e65b5756297`  
		Last Modified: Tue, 17 Aug 2021 01:28:23 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:experimental` - linux; ppc64le

```console
$ docker pull debian@sha256:90b5bb9eeb31762a168aa65cded2b78ad34471acd892899581c7520a5c48bf89
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **58.9 MB (58855380 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4a174002822b1b4728a09ba77692fa7253799dbc0a3bf53262174c8e2eaf3ad2`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Aug 2021 01:38:54 GMT
ADD file:630159b2a1019aaf8ce1a72a962575e0b57c315928aeaacb240af5be1fd56ed5 in / 
# Tue, 17 Aug 2021 01:39:00 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 01:39:43 GMT
RUN echo 'deb http://deb.debian.org/debian experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:ce43574b5a24506e7371089632f77595540e986c8d36b088b06be7aed6174898`  
		Last Modified: Tue, 17 Aug 2021 01:58:51 GMT  
		Size: 58.9 MB (58855156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd5f2d4e334ba162dab10cba8567c2fe1b5f186a7c9d1dbdff831a60b5d86617`  
		Last Modified: Tue, 17 Aug 2021 01:59:46 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:experimental` - linux; riscv64

```console
$ docker pull debian@sha256:3a66024822ef203ab58c9109a0abe1707b0057e550e65dc09fb1b7318fd8af36
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.4 MB (50438050 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7f44f37612bc6f45e607fa940ccf78d49fc82a1cbd262b50cb305bdd4ff3b8f6`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Aug 2021 01:49:30 GMT
ADD file:0f9b032e8c46c033b3715526a66fa72e4dec9b70dd905c4e0675d2410e718150 in / 
# Tue, 17 Aug 2021 01:49:33 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 01:52:42 GMT
RUN echo 'deb http://deb.debian.org/debian-ports experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:1a640adac6b0cc3fc00b5f7df9ce95cafe19e015f3ab67b26504aa9709489efc`  
		Last Modified: Tue, 17 Aug 2021 02:05:16 GMT  
		Size: 50.4 MB (50437823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:151888b96b892fe20132635b20ddcfde85327c25f79e69891223b9fd23726395`  
		Last Modified: Tue, 17 Aug 2021 02:07:56 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:experimental` - linux; s390x

```console
$ docker pull debian@sha256:16f77818aa6ce277cb82157ade0433e444df8ae8bf376954ffa146ddb41127a7
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.2 MB (53226754 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:60a353e8d5867d2e020c696cb25381c63d23b61aa38562231c451162e6e30bbe`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Aug 2021 01:53:30 GMT
ADD file:2abd2e51e88a6ead7bacc45543358162ebb2c7754c84616ed19f1098deac54d8 in / 
# Tue, 17 Aug 2021 01:53:39 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 01:54:09 GMT
RUN echo 'deb http://deb.debian.org/debian experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:5158dbc0f64ddcd299785cbeaca04e4bb960ce72e427721169ce2db531f41d4d`  
		Last Modified: Tue, 17 Aug 2021 02:00:36 GMT  
		Size: 53.2 MB (53226532 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8b8a1fbfe1b1b2d093c8e4595ec0f8cdc7f5b6be81ed9de4d9435ac6c59e387`  
		Last Modified: Tue, 17 Aug 2021 02:00:57 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
