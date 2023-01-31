<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `ubuntu`

-	[`ubuntu:18.04`](#ubuntu1804)
-	[`ubuntu:20.04`](#ubuntu2004)
-	[`ubuntu:22.04`](#ubuntu2204)
-	[`ubuntu:22.10`](#ubuntu2210)
-	[`ubuntu:23.04`](#ubuntu2304)
-	[`ubuntu:bionic`](#ubuntubionic)
-	[`ubuntu:bionic-20230126`](#ubuntubionic-20230126)
-	[`ubuntu:devel`](#ubuntudevel)
-	[`ubuntu:focal`](#ubuntufocal)
-	[`ubuntu:focal-20230126`](#ubuntufocal-20230126)
-	[`ubuntu:jammy`](#ubuntujammy)
-	[`ubuntu:jammy-20230126`](#ubuntujammy-20230126)
-	[`ubuntu:kinetic`](#ubuntukinetic)
-	[`ubuntu:kinetic-20230126`](#ubuntukinetic-20230126)
-	[`ubuntu:latest`](#ubuntulatest)
-	[`ubuntu:lunar`](#ubuntulunar)
-	[`ubuntu:lunar-20230124.1`](#ubuntulunar-202301241)
-	[`ubuntu:rolling`](#ubunturolling)

## `ubuntu:18.04`

```console
$ docker pull ubuntu@sha256:63986ce572d0e7b2268073c863561cb001ef3cb15ef69c45c1d890f7262e1bdf
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `ubuntu:18.04` - linux; amd64

```console
$ docker pull ubuntu@sha256:0b0aab2bb85da9e3168407368464cb15f828eda8860eefb4c74a57dea2f139c7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.7 MB (25688613 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5d2df19066aca89df8e5317544a1cb599dc657830184762ff6fdefaaf708db65`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 26 Jan 2023 10:03:03 GMT
ARG RELEASE
# Thu, 26 Jan 2023 10:03:03 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 10:03:03 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 10:03:03 GMT
LABEL org.opencontainers.image.version=18.04
# Thu, 26 Jan 2023 10:03:04 GMT
ADD file:365c129e10f7ef1594e8086543b45f524313e36dd6a25b68f4da542a09491f04 in / 
# Thu, 26 Jan 2023 10:03:05 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:72d9f18d70f395ff9bfae4d193077ccea3ca583e3da3dd66f5c84520c0100727`  
		Last Modified: Thu, 26 Jan 2023 10:11:57 GMT  
		Size: 25.7 MB (25688613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:18.04` - linux; arm variant v7

```console
$ docker pull ubuntu@sha256:760efd7a591154335f9e4c22ac59ed5ac9e4030bf661f65cbe842d15ff5942c0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **21.4 MB (21395113 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d17e780dbbcb4f0f3439981b5f09c45d9de103ca383942edbb8842911f2402fc`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 26 Jan 2023 09:56:13 GMT
ARG RELEASE
# Thu, 26 Jan 2023 09:56:13 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 09:56:13 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 09:56:13 GMT
LABEL org.opencontainers.image.version=18.04
# Thu, 26 Jan 2023 09:56:18 GMT
ADD file:1cc75b54b9c4d0824203532d4bb0eea2aaeafed003e37057b21aa3713b6bb0ea in / 
# Thu, 26 Jan 2023 09:56:18 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:c138257d410403a2127c08e269ac8467b8f2001b22a102934861b65b2f49bc1a`  
		Last Modified: Thu, 26 Jan 2023 10:12:17 GMT  
		Size: 21.4 MB (21395113 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:18.04` - linux; arm64 variant v8

```console
$ docker pull ubuntu@sha256:f07df923366018f4ac9d2d5b839484e2108d8631ce2872e637049147a47c9b1d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **22.7 MB (22711894 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b2b37ee8ce31e197fba06b7de0b4b07a6fe33e5921918be8d7e1de7b8f25893b`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 26 Jan 2023 10:04:53 GMT
ARG RELEASE
# Thu, 26 Jan 2023 10:04:53 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 10:04:53 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 10:04:53 GMT
LABEL org.opencontainers.image.version=18.04
# Thu, 26 Jan 2023 10:04:56 GMT
ADD file:e7556a99ac088826f5ea581a0c5e2230c1f9a9deab7106e9cec6d1ae8594f19a in / 
# Thu, 26 Jan 2023 10:04:57 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:c2a5dda1e2b0d861ec46a9c576c4fd4d667c56aa4b1cac9cd8c16e629dd11b28`  
		Last Modified: Thu, 26 Jan 2023 10:12:11 GMT  
		Size: 22.7 MB (22711894 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:18.04` - linux; 386

```console
$ docker pull ubuntu@sha256:8bb84ffaabfe58d03cf9b72ea78d248c57db985525a67ef6f2f0e404b7c59124
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.1 MB (26096513 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:97151d96f64f3b5b7cdb0fadb1c1f8556552cedf32154f23efd48595efabb1e4`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 26 Jan 2023 10:03:01 GMT
ARG RELEASE
# Thu, 26 Jan 2023 10:03:01 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 10:03:01 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 10:03:01 GMT
LABEL org.opencontainers.image.version=18.04
# Thu, 26 Jan 2023 10:03:03 GMT
ADD file:b9b814a7d1e7611a2c531fac3419a48c733c622470d3f275ce29f9ba8764eaeb in / 
# Thu, 26 Jan 2023 10:03:04 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:57a4d5aed2cd4a1f596f693a8fe5e135bd66dbf401ec169b1848d2316bdcfb2c`  
		Last Modified: Thu, 26 Jan 2023 10:12:23 GMT  
		Size: 26.1 MB (26096513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:18.04` - linux; ppc64le

```console
$ docker pull ubuntu@sha256:721b53fe8a192c32d5077c120a5e253b2bba08b13fcc02c26d6cf63dea715f9f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.4 MB (29351018 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d4e533a2e815a6606d93392dd9f8ff6938a39080b67cfd575045cfe820ede7af`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 26 Jan 2023 09:55:44 GMT
ARG RELEASE
# Thu, 26 Jan 2023 09:55:44 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 09:55:44 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 09:55:44 GMT
LABEL org.opencontainers.image.version=18.04
# Thu, 26 Jan 2023 09:55:47 GMT
ADD file:108aadd723beb46031bfaca610c036aea506955578347dda4a01cfb0c6bdc135 in / 
# Thu, 26 Jan 2023 09:55:48 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:6c790564dfb49a61552a6e89c63c7abf84177d16d0f0fb604df022bfcdc6497b`  
		Last Modified: Thu, 26 Jan 2023 10:12:31 GMT  
		Size: 29.4 MB (29351018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:18.04` - linux; s390x

```console
$ docker pull ubuntu@sha256:0e9b40aadd1aa55e0cf7f5775b21373a3b028dc9171e729255968e6e5213758c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **24.7 MB (24744933 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5e81833e90b6b40072356a6b1256c20d690401c5130f58b3343b6e30c2eccb64`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 26 Jan 2023 09:55:41 GMT
ARG RELEASE
# Thu, 26 Jan 2023 09:55:41 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 09:55:41 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 09:55:41 GMT
LABEL org.opencontainers.image.version=18.04
# Thu, 26 Jan 2023 09:55:43 GMT
ADD file:04d4137c9183cee18560fc26a092e288ff403f3dde266237eab245bd38eb9b3a in / 
# Thu, 26 Jan 2023 09:55:43 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:9e75830a8e632695dde0b55ec0159bd7b141ab79858367e3f66bfa5f255aaec9`  
		Last Modified: Thu, 26 Jan 2023 10:12:37 GMT  
		Size: 24.7 MB (24744933 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ubuntu:20.04`

```console
$ docker pull ubuntu@sha256:b33325a00c7c27b23ae48cf17d2c654e2c30812b35e7846c006389318f6a71c2
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `ubuntu:20.04` - linux; amd64

```console
$ docker pull ubuntu@sha256:d5d4814ffb155d588f10ec8926d9e1cd09b6d41a3110d2f42959e2fc37f6d0b4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.5 MB (27503418 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f32fe8df6a4c91a6bfe1fae9ffa5a05bac157d0edd78571d34c3c784985d95f7`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 26 Jan 2023 13:19:55 GMT
ARG RELEASE
# Thu, 26 Jan 2023 13:19:55 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 13:19:55 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 13:19:55 GMT
LABEL org.opencontainers.image.version=20.04
# Thu, 26 Jan 2023 13:19:57 GMT
ADD file:8b180a9b4497de0c6e131d6b48cf5c69a885379e63033ab9639d1655991e626c in / 
# Thu, 26 Jan 2023 13:19:57 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:bdec8b63443ac80dc7fdf49c2b5bbe08191e0f5fda5f1f5d6b5f25263cfa2c47`  
		Last Modified: Thu, 26 Jan 2023 14:01:47 GMT  
		Size: 27.5 MB (27503418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:20.04` - linux; arm variant v7

```console
$ docker pull ubuntu@sha256:d5d767be339687f755e936fffaa860a965316ebb23035242994ff7e3a8e26472
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.6 MB (23608452 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e7fd2989c767b17f419f4a0fd29ff08ee906380dc2d5963e51ed44537f16bcdb`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 26 Jan 2023 13:35:44 GMT
ARG RELEASE
# Thu, 26 Jan 2023 13:35:44 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 13:35:44 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 13:35:44 GMT
LABEL org.opencontainers.image.version=20.04
# Thu, 26 Jan 2023 13:35:48 GMT
ADD file:6566d63937dd1808d3a4ea5591d4369b9083772d48fad60626fb91243a9f3f53 in / 
# Thu, 26 Jan 2023 13:35:49 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:325e20204bae7a15035068b8043b4abc0f59c014564bf465b3a99757175402ce`  
		Last Modified: Thu, 26 Jan 2023 14:02:03 GMT  
		Size: 23.6 MB (23608452 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:20.04` - linux; arm64 variant v8

```console
$ docker pull ubuntu@sha256:a840dd8130bfe149a60f0ad6ca972b7259f9c55e323b16b659f58af2eb6dabfa
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.0 MB (25972163 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e26da238ce02fc608d0410d966f12d91d42677ecaa5df68dd325efdddb8fb85e`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 26 Jan 2023 13:50:26 GMT
ARG RELEASE
# Thu, 26 Jan 2023 13:50:26 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 13:50:26 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 13:50:26 GMT
LABEL org.opencontainers.image.version=20.04
# Thu, 26 Jan 2023 13:50:33 GMT
ADD file:72ca0af0100de6591b59c44bd8856655c8441eb0fcbf7c32e427f6be5108a4a4 in / 
# Thu, 26 Jan 2023 13:50:33 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:ffe6f70103a5896ebe7878266832cd044ef7b46fa905937864c9e9be67b38351`  
		Last Modified: Thu, 26 Jan 2023 14:01:54 GMT  
		Size: 26.0 MB (25972163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:20.04` - linux; ppc64le

```console
$ docker pull ubuntu@sha256:cebffa8cceec4bea7ef66193cc86b9ad216bd45292ccd79e2ea9a6830a568e4c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.1 MB (32068234 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6a6fe6633addd2a7fd34c33cdfeebefac8d57eb53ebe773fc66f22c5ccca8998`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 26 Jan 2023 13:47:16 GMT
ARG RELEASE
# Thu, 26 Jan 2023 13:47:16 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 13:47:17 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 13:47:17 GMT
LABEL org.opencontainers.image.version=20.04
# Thu, 26 Jan 2023 13:47:20 GMT
ADD file:987b941a34ad98533c64e74a3d57b9c1b983ff16c8f36e21d29278a30a2403ee in / 
# Thu, 26 Jan 2023 13:47:20 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:78c13b83c7cdda97b53d4407c98b39430a4d2a175fa9aff8503068948e87dd9a`  
		Last Modified: Thu, 26 Jan 2023 14:02:09 GMT  
		Size: 32.1 MB (32068234 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:20.04` - linux; s390x

```console
$ docker pull ubuntu@sha256:602b58d620499c50ae12f6fc2d7f6caa0fe5e00875dd7b2d291c595199c6fb43
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.4 MB (26363789 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:61b58fa4a9492ff8aba7316c0156c6d47890115d6865b7fe9eec96611ae2ee0a`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 26 Jan 2023 13:21:27 GMT
ARG RELEASE
# Thu, 26 Jan 2023 13:21:27 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 13:21:27 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 13:21:27 GMT
LABEL org.opencontainers.image.version=20.04
# Thu, 26 Jan 2023 13:21:29 GMT
ADD file:4d5fa9b68af51e9c8cd7b25fb55ddd47256efb0b2eda9432507b72b7c1a17053 in / 
# Thu, 26 Jan 2023 13:21:30 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:870f83892b5769f235d9116edab9c19d569d14d716bcd10b90ab5314292fd908`  
		Last Modified: Thu, 26 Jan 2023 14:02:16 GMT  
		Size: 26.4 MB (26363789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ubuntu:22.04`

```console
$ docker pull ubuntu@sha256:f05532b6a1dec5f7a77a8d684af87bc9cd1f2b32eab301c109f8ad151b5565d1
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `ubuntu:22.04` - linux; amd64

```console
$ docker pull ubuntu@sha256:eecba05a9ccbc219cb0f0dd280034c6ee1aab0b00b458e680f9c4efc6ca3feda
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.5 MB (29528717 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:58db3edaf2be6e80f628796355b1bdeaf8bea1692b402f48b7e7b8d1ff100b02`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 26 Jan 2023 04:57:59 GMT
ARG RELEASE
# Thu, 26 Jan 2023 04:57:59 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 04:58:00 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 04:58:00 GMT
LABEL org.opencontainers.image.version=22.04
# Thu, 26 Jan 2023 04:58:02 GMT
ADD file:18e71f049606f6339ce7a995839623f50e6ec6474bfd0a3a7ca799db726f47f6 in / 
# Thu, 26 Jan 2023 04:58:02 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:677076032cca0a2362d25cf3660072e738d1b96fe860409a33ce901d695d7ee8`  
		Last Modified: Thu, 26 Jan 2023 05:13:54 GMT  
		Size: 29.5 MB (29528717 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:22.04` - linux; arm variant v7

```console
$ docker pull ubuntu@sha256:5c3735e92e29c51fa2ac513ea7d130e0ea61de153abdf28974afc83cf5dfa8cf
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.1 MB (26137949 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b15b861da44337925963eb70b8671950999df7d8abfe7f5a9b5f95ff9f4cca7a`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 26 Jan 2023 05:05:40 GMT
ARG RELEASE
# Thu, 26 Jan 2023 05:05:40 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 05:05:40 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 05:05:40 GMT
LABEL org.opencontainers.image.version=22.04
# Thu, 26 Jan 2023 05:05:43 GMT
ADD file:12d2a7ddc8445b8f97c960075216eb8e8cd226b84259c7343ef15c65a440b500 in / 
# Thu, 26 Jan 2023 05:05:43 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:860e874323ae800886f85ab5c346783e3a9371bd9beb72c5f25e8e20c9dd18bb`  
		Last Modified: Thu, 26 Jan 2023 05:14:09 GMT  
		Size: 26.1 MB (26137949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:22.04` - linux; arm64 variant v8

```console
$ docker pull ubuntu@sha256:13e180ab78513dbe30a4f5a9e35acc6f61d92cbccac887a4f11ea23516261cc0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.3 MB (27342387 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a6be1f66f70f66ef43503292e38ccbfc14f2d5464e7736344783a8fc7bb339a8`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 26 Jan 2023 05:05:49 GMT
ARG RELEASE
# Thu, 26 Jan 2023 05:05:49 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 05:05:49 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 05:05:50 GMT
LABEL org.opencontainers.image.version=22.04
# Thu, 26 Jan 2023 05:05:51 GMT
ADD file:55486a91f732042dd4e81ecfd8457d23e04dcd7dd80a0bb06cc7c44873fac838 in / 
# Thu, 26 Jan 2023 05:05:51 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:8b150fd943bcd54ef788cece17523d19031f745b099a798de65247900d102e18`  
		Last Modified: Thu, 26 Jan 2023 05:14:03 GMT  
		Size: 27.3 MB (27342387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:22.04` - linux; ppc64le

```console
$ docker pull ubuntu@sha256:ed40c990366092268d72da08b90fb5a0f6081ab1e00918c6453e64443d775dca
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.6 MB (34588568 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d899338973bac5fb325b647c7436507e44918374fff2a72b0da6515946c868a7`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 26 Jan 2023 04:58:24 GMT
ARG RELEASE
# Thu, 26 Jan 2023 04:58:24 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 04:58:24 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 04:58:24 GMT
LABEL org.opencontainers.image.version=22.04
# Thu, 26 Jan 2023 04:58:28 GMT
ADD file:f0400001a50847feb579e66e804ec9daaaaeb9a414b4b5cca8bb0c8e9c7fa8f9 in / 
# Thu, 26 Jan 2023 04:58:28 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:717e115780fa5a198871a9eef15e446084728bf7021e7894e6118f3cd6d26b60`  
		Last Modified: Thu, 26 Jan 2023 05:14:15 GMT  
		Size: 34.6 MB (34588568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:22.04` - linux; s390x

```console
$ docker pull ubuntu@sha256:d3df0130c5dc92778c7513686bb9f10d5e2e710b7f290d686bda24ac351d3220
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.0 MB (28009396 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6abbed079020c533dbc7ca626067d743bf7effce2e4c895f104846afd8f4943a`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 26 Jan 2023 05:08:35 GMT
ARG RELEASE
# Thu, 26 Jan 2023 05:08:35 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 05:08:36 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 05:08:36 GMT
LABEL org.opencontainers.image.version=22.04
# Thu, 26 Jan 2023 05:08:37 GMT
ADD file:a9794efc1a102ab6a7160e660a63f4b267797b8b7e0b0bfd9c04ed62846cfb36 in / 
# Thu, 26 Jan 2023 05:08:38 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:f8e318d098424cef87513f4c834987f20c608791646c6b1a3ef60ed57408ddb6`  
		Last Modified: Thu, 26 Jan 2023 05:14:22 GMT  
		Size: 28.0 MB (28009396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ubuntu:22.10`

```console
$ docker pull ubuntu@sha256:a062bfdb0c233a5a7c4758c028ef6a8f4981b78008606e23f47143ca0bfb483d
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `ubuntu:22.10` - linux; amd64

```console
$ docker pull ubuntu@sha256:ef3c777a7db8a2c49d31284cc924fc3a2f471dce44378a18d6d1fefff5a63fe5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.7 MB (26691650 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:10c2f4041af137e6b0ba5c793df3dfdf4e72a4e011ce6847f4cc0247b9bbf7f2`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 26 Jan 2023 11:51:12 GMT
ARG RELEASE
# Thu, 26 Jan 2023 11:51:12 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 11:51:12 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 11:51:13 GMT
LABEL org.opencontainers.image.version=22.10
# Thu, 26 Jan 2023 11:51:14 GMT
ADD file:e886423892b371751386c0ce7147599acb72d8fb528eaaa78092b879d9ff58ce in / 
# Thu, 26 Jan 2023 11:51:15 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:256644d5a307c3efeca6ae2854b6329a2753157868dc5548e33161b377658e6a`  
		Last Modified: Thu, 26 Jan 2023 12:14:04 GMT  
		Size: 26.7 MB (26691650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:22.10` - linux; arm variant v7

```console
$ docker pull ubuntu@sha256:a9fd5288ceabc4990263038e3ff67154088e5df217fd2eaed5ac7fce8318d84a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.1 MB (25066997 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8d643d5974c30c06b1d811877a3a8f0047c4278b1fe0801d8d812b3a17ce6c15`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 26 Jan 2023 11:52:00 GMT
ARG RELEASE
# Thu, 26 Jan 2023 11:52:00 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 11:52:00 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 11:52:00 GMT
LABEL org.opencontainers.image.version=22.10
# Thu, 26 Jan 2023 11:52:03 GMT
ADD file:d35c57b0dc2840a8b1ef40f7f6cfd826da68611f1ba37a89a382618c8612b52c in / 
# Thu, 26 Jan 2023 11:52:03 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:697d38f8dfe625e3e751c0b01ddeaaeeff6e8d6f594dd7da227aea3974a49ce1`  
		Last Modified: Thu, 26 Jan 2023 12:14:16 GMT  
		Size: 25.1 MB (25066997 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:22.10` - linux; arm64 variant v8

```console
$ docker pull ubuntu@sha256:aff210956f022245b200f8be680a99c7d93f191b2cfc8d6f770f87ef3644a080
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.8 MB (25757647 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c7096432b6a9855592152ad8009431b92d7aa40980c9c94684fcc72626bbbab9`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 26 Jan 2023 12:08:18 GMT
ARG RELEASE
# Thu, 26 Jan 2023 12:08:18 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 12:08:18 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 12:08:18 GMT
LABEL org.opencontainers.image.version=22.10
# Thu, 26 Jan 2023 12:08:20 GMT
ADD file:f61617371f6963c6be2852e2b94d04e8507feb8f77e3484c94aa8b9d0ac67f76 in / 
# Thu, 26 Jan 2023 12:08:20 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:05f69cab0b799028e03233ffa93abd2d0b426412cff70959a07a29a437447ee3`  
		Last Modified: Thu, 26 Jan 2023 12:14:10 GMT  
		Size: 25.8 MB (25757647 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:22.10` - linux; ppc64le

```console
$ docker pull ubuntu@sha256:daab817634ed004a6c564aec6ca0a0d84205d49371765eb625366344ceb7d5bd
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.1 MB (31110147 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5dfbc0b60efcd8ea2a51c157e7bc286d8de7e88ae1bf756e0d8a44ff107e21c7`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 26 Jan 2023 11:57:00 GMT
ARG RELEASE
# Thu, 26 Jan 2023 11:57:00 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 11:57:00 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 11:57:00 GMT
LABEL org.opencontainers.image.version=22.10
# Thu, 26 Jan 2023 11:57:03 GMT
ADD file:3c2bc98d283cce5149d7992233f5fe644b7239417045faf3f93750b92de5f68e in / 
# Thu, 26 Jan 2023 11:57:04 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:8da618ff876e10064f550b9dc5b51b0d0ae6939f67b56ce9a0c7fa8bb77de40f`  
		Last Modified: Thu, 26 Jan 2023 12:14:22 GMT  
		Size: 31.1 MB (31110147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:22.10` - linux; s390x

```console
$ docker pull ubuntu@sha256:944066fb6be279b0de11cb4ecc57c81794b912ba6f95a544f3d462ceab3a78a6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.5 MB (25487159 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:91297aceb6d3e297e45ec91916dbea079b90ae1c7edbaf14a99c41d3f493f537`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 26 Jan 2023 12:08:47 GMT
ARG RELEASE
# Thu, 26 Jan 2023 12:08:47 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 12:08:48 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 12:08:48 GMT
LABEL org.opencontainers.image.version=22.10
# Thu, 26 Jan 2023 12:08:50 GMT
ADD file:a83afd93816f868be76d243df85b87a66b39d5ef0497c3cb8d0bba2bd4a27c40 in / 
# Thu, 26 Jan 2023 12:08:50 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:fe4914a812d394969d56f220e5ddb037a62164607a937ca866bf4ee592a8799a`  
		Last Modified: Thu, 26 Jan 2023 12:14:28 GMT  
		Size: 25.5 MB (25487159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ubuntu:23.04`

```console
$ docker pull ubuntu@sha256:e2e6dfaf4d892b0430e636f2747c3a19d47a806a1fc21810743c113ca59ab6a2
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `ubuntu:23.04` - linux; amd64

```console
$ docker pull ubuntu@sha256:76f55c747c6e3cc7a49f6bade839a8fbca72e0338fec92b54e58b8d15baf836d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.6 MB (26594295 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:096628db4ff280b69ee9eaca21f0cfc152776e1243bc6c1320b436934188d5e5`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 25 Jan 2023 14:47:05 GMT
ARG RELEASE
# Wed, 25 Jan 2023 14:47:05 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 25 Jan 2023 14:47:05 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 25 Jan 2023 14:47:05 GMT
LABEL org.opencontainers.image.version=23.04
# Wed, 25 Jan 2023 14:47:07 GMT
ADD file:5a9904395b52775ee7c10a49efc741d32b587e2cd447b8deb66811c3fb3b37a4 in / 
# Wed, 25 Jan 2023 14:47:07 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:85cec64d15ef8b1eb3ff65555dbe92d7e3ea2a21f3e1fe1206ed85e221b3593d`  
		Last Modified: Wed, 25 Jan 2023 14:56:49 GMT  
		Size: 26.6 MB (26594295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:23.04` - linux; arm variant v7

```console
$ docker pull ubuntu@sha256:1d8b24f64674c975ae2ca8b10f39a8c79cca25e278d9fe6438bddef61307e3f1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.1 MB (25095764 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9f55f15212572f043ec357086e290a82ab554094f4f7f044746ff6dec8d96428`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 25 Jan 2023 14:38:25 GMT
ARG RELEASE
# Wed, 25 Jan 2023 14:38:25 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 25 Jan 2023 14:38:26 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 25 Jan 2023 14:38:26 GMT
LABEL org.opencontainers.image.version=23.04
# Wed, 25 Jan 2023 14:38:35 GMT
ADD file:c01025be735c65553980246358cbe7c563769d7ffc886d18be817582a0d29b5c in / 
# Wed, 25 Jan 2023 14:38:36 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:f9e87c970a05364b1b6a0c18043b8cc663c1dcd5b370d87043288950fabb675a`  
		Last Modified: Wed, 25 Jan 2023 14:57:02 GMT  
		Size: 25.1 MB (25095764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:23.04` - linux; arm64 variant v8

```console
$ docker pull ubuntu@sha256:601b47b473ab776a59e725ab6bde002ed7b271b9531dc72d602c033b0c578879
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.8 MB (25777338 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:39efbc92de18d58fc90c5503a1f69c3dccce7e29830cc6560ec6857f8b6485e5`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 25 Jan 2023 14:42:22 GMT
ARG RELEASE
# Wed, 25 Jan 2023 14:42:23 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 25 Jan 2023 14:42:23 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 25 Jan 2023 14:42:23 GMT
LABEL org.opencontainers.image.version=23.04
# Wed, 25 Jan 2023 14:42:31 GMT
ADD file:6713306ff9bcc18c79430d43aafbbe519176e76b7232c563993ebda6c8caf738 in / 
# Wed, 25 Jan 2023 14:42:32 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:ce743a0a7eb81f2756829eb9afb29c85ce40ded304387cdd06f66b01793ac464`  
		Last Modified: Wed, 25 Jan 2023 14:56:55 GMT  
		Size: 25.8 MB (25777338 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:23.04` - linux; ppc64le

```console
$ docker pull ubuntu@sha256:67fe8ea65e1c908351ee7dbc6cf56660fc0d3ef49b8046aeb61e3df7fbd5172d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.0 MB (30959485 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c420642d8d83f69bc1f4eba5096256ff91343014b4d8dbdfcead8b96635f6c11`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 25 Jan 2023 14:48:03 GMT
ARG RELEASE
# Wed, 25 Jan 2023 14:48:03 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 25 Jan 2023 14:48:03 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 25 Jan 2023 14:48:04 GMT
LABEL org.opencontainers.image.version=23.04
# Wed, 25 Jan 2023 14:48:07 GMT
ADD file:5002466754dcd29080099171ab20675c9bcc55f0befbe928008127d14c027297 in / 
# Wed, 25 Jan 2023 14:48:07 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:8215a53a3d6e58238feac2e65d9c57d1f382d8ade421475347b3c522198afe4e`  
		Last Modified: Wed, 25 Jan 2023 14:57:08 GMT  
		Size: 31.0 MB (30959485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:23.04` - linux; s390x

```console
$ docker pull ubuntu@sha256:87dc7c1f1d0b9cdb25c2e1cfdcd05569ab54f7949365a8aa8677d6098f57273d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.5 MB (25455083 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2a5869fd440bbbebdfc74dcec9c949501d695f868ff73d63165a920e39d8bfca`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 25 Jan 2023 14:49:06 GMT
ARG RELEASE
# Wed, 25 Jan 2023 14:49:06 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 25 Jan 2023 14:49:06 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 25 Jan 2023 14:49:06 GMT
LABEL org.opencontainers.image.version=23.04
# Wed, 25 Jan 2023 14:49:08 GMT
ADD file:81c93bf9ec11b910a5bae8b977a82a78cb327c7bf9d0991542c9b6847cf19210 in / 
# Wed, 25 Jan 2023 14:49:12 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:f6119d8ec48acf1c2965d2233f93e21ee590564bbae9fd360b9630c3b6c694f9`  
		Last Modified: Wed, 25 Jan 2023 14:57:22 GMT  
		Size: 25.5 MB (25455083 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ubuntu:bionic`

```console
$ docker pull ubuntu@sha256:63986ce572d0e7b2268073c863561cb001ef3cb15ef69c45c1d890f7262e1bdf
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `ubuntu:bionic` - linux; amd64

```console
$ docker pull ubuntu@sha256:0b0aab2bb85da9e3168407368464cb15f828eda8860eefb4c74a57dea2f139c7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.7 MB (25688613 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5d2df19066aca89df8e5317544a1cb599dc657830184762ff6fdefaaf708db65`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 26 Jan 2023 10:03:03 GMT
ARG RELEASE
# Thu, 26 Jan 2023 10:03:03 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 10:03:03 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 10:03:03 GMT
LABEL org.opencontainers.image.version=18.04
# Thu, 26 Jan 2023 10:03:04 GMT
ADD file:365c129e10f7ef1594e8086543b45f524313e36dd6a25b68f4da542a09491f04 in / 
# Thu, 26 Jan 2023 10:03:05 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:72d9f18d70f395ff9bfae4d193077ccea3ca583e3da3dd66f5c84520c0100727`  
		Last Modified: Thu, 26 Jan 2023 10:11:57 GMT  
		Size: 25.7 MB (25688613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:bionic` - linux; arm variant v7

```console
$ docker pull ubuntu@sha256:760efd7a591154335f9e4c22ac59ed5ac9e4030bf661f65cbe842d15ff5942c0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **21.4 MB (21395113 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d17e780dbbcb4f0f3439981b5f09c45d9de103ca383942edbb8842911f2402fc`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 26 Jan 2023 09:56:13 GMT
ARG RELEASE
# Thu, 26 Jan 2023 09:56:13 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 09:56:13 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 09:56:13 GMT
LABEL org.opencontainers.image.version=18.04
# Thu, 26 Jan 2023 09:56:18 GMT
ADD file:1cc75b54b9c4d0824203532d4bb0eea2aaeafed003e37057b21aa3713b6bb0ea in / 
# Thu, 26 Jan 2023 09:56:18 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:c138257d410403a2127c08e269ac8467b8f2001b22a102934861b65b2f49bc1a`  
		Last Modified: Thu, 26 Jan 2023 10:12:17 GMT  
		Size: 21.4 MB (21395113 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:bionic` - linux; arm64 variant v8

```console
$ docker pull ubuntu@sha256:f07df923366018f4ac9d2d5b839484e2108d8631ce2872e637049147a47c9b1d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **22.7 MB (22711894 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b2b37ee8ce31e197fba06b7de0b4b07a6fe33e5921918be8d7e1de7b8f25893b`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 26 Jan 2023 10:04:53 GMT
ARG RELEASE
# Thu, 26 Jan 2023 10:04:53 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 10:04:53 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 10:04:53 GMT
LABEL org.opencontainers.image.version=18.04
# Thu, 26 Jan 2023 10:04:56 GMT
ADD file:e7556a99ac088826f5ea581a0c5e2230c1f9a9deab7106e9cec6d1ae8594f19a in / 
# Thu, 26 Jan 2023 10:04:57 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:c2a5dda1e2b0d861ec46a9c576c4fd4d667c56aa4b1cac9cd8c16e629dd11b28`  
		Last Modified: Thu, 26 Jan 2023 10:12:11 GMT  
		Size: 22.7 MB (22711894 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:bionic` - linux; 386

```console
$ docker pull ubuntu@sha256:8bb84ffaabfe58d03cf9b72ea78d248c57db985525a67ef6f2f0e404b7c59124
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.1 MB (26096513 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:97151d96f64f3b5b7cdb0fadb1c1f8556552cedf32154f23efd48595efabb1e4`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 26 Jan 2023 10:03:01 GMT
ARG RELEASE
# Thu, 26 Jan 2023 10:03:01 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 10:03:01 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 10:03:01 GMT
LABEL org.opencontainers.image.version=18.04
# Thu, 26 Jan 2023 10:03:03 GMT
ADD file:b9b814a7d1e7611a2c531fac3419a48c733c622470d3f275ce29f9ba8764eaeb in / 
# Thu, 26 Jan 2023 10:03:04 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:57a4d5aed2cd4a1f596f693a8fe5e135bd66dbf401ec169b1848d2316bdcfb2c`  
		Last Modified: Thu, 26 Jan 2023 10:12:23 GMT  
		Size: 26.1 MB (26096513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:bionic` - linux; ppc64le

```console
$ docker pull ubuntu@sha256:721b53fe8a192c32d5077c120a5e253b2bba08b13fcc02c26d6cf63dea715f9f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.4 MB (29351018 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d4e533a2e815a6606d93392dd9f8ff6938a39080b67cfd575045cfe820ede7af`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 26 Jan 2023 09:55:44 GMT
ARG RELEASE
# Thu, 26 Jan 2023 09:55:44 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 09:55:44 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 09:55:44 GMT
LABEL org.opencontainers.image.version=18.04
# Thu, 26 Jan 2023 09:55:47 GMT
ADD file:108aadd723beb46031bfaca610c036aea506955578347dda4a01cfb0c6bdc135 in / 
# Thu, 26 Jan 2023 09:55:48 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:6c790564dfb49a61552a6e89c63c7abf84177d16d0f0fb604df022bfcdc6497b`  
		Last Modified: Thu, 26 Jan 2023 10:12:31 GMT  
		Size: 29.4 MB (29351018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:bionic` - linux; s390x

```console
$ docker pull ubuntu@sha256:0e9b40aadd1aa55e0cf7f5775b21373a3b028dc9171e729255968e6e5213758c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **24.7 MB (24744933 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5e81833e90b6b40072356a6b1256c20d690401c5130f58b3343b6e30c2eccb64`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 26 Jan 2023 09:55:41 GMT
ARG RELEASE
# Thu, 26 Jan 2023 09:55:41 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 09:55:41 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 09:55:41 GMT
LABEL org.opencontainers.image.version=18.04
# Thu, 26 Jan 2023 09:55:43 GMT
ADD file:04d4137c9183cee18560fc26a092e288ff403f3dde266237eab245bd38eb9b3a in / 
# Thu, 26 Jan 2023 09:55:43 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:9e75830a8e632695dde0b55ec0159bd7b141ab79858367e3f66bfa5f255aaec9`  
		Last Modified: Thu, 26 Jan 2023 10:12:37 GMT  
		Size: 24.7 MB (24744933 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ubuntu:bionic-20230126`

```console
$ docker pull ubuntu@sha256:63986ce572d0e7b2268073c863561cb001ef3cb15ef69c45c1d890f7262e1bdf
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `ubuntu:bionic-20230126` - linux; amd64

```console
$ docker pull ubuntu@sha256:0b0aab2bb85da9e3168407368464cb15f828eda8860eefb4c74a57dea2f139c7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.7 MB (25688613 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5d2df19066aca89df8e5317544a1cb599dc657830184762ff6fdefaaf708db65`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 26 Jan 2023 10:03:03 GMT
ARG RELEASE
# Thu, 26 Jan 2023 10:03:03 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 10:03:03 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 10:03:03 GMT
LABEL org.opencontainers.image.version=18.04
# Thu, 26 Jan 2023 10:03:04 GMT
ADD file:365c129e10f7ef1594e8086543b45f524313e36dd6a25b68f4da542a09491f04 in / 
# Thu, 26 Jan 2023 10:03:05 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:72d9f18d70f395ff9bfae4d193077ccea3ca583e3da3dd66f5c84520c0100727`  
		Last Modified: Thu, 26 Jan 2023 10:11:57 GMT  
		Size: 25.7 MB (25688613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:bionic-20230126` - linux; arm variant v7

```console
$ docker pull ubuntu@sha256:760efd7a591154335f9e4c22ac59ed5ac9e4030bf661f65cbe842d15ff5942c0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **21.4 MB (21395113 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d17e780dbbcb4f0f3439981b5f09c45d9de103ca383942edbb8842911f2402fc`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 26 Jan 2023 09:56:13 GMT
ARG RELEASE
# Thu, 26 Jan 2023 09:56:13 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 09:56:13 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 09:56:13 GMT
LABEL org.opencontainers.image.version=18.04
# Thu, 26 Jan 2023 09:56:18 GMT
ADD file:1cc75b54b9c4d0824203532d4bb0eea2aaeafed003e37057b21aa3713b6bb0ea in / 
# Thu, 26 Jan 2023 09:56:18 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:c138257d410403a2127c08e269ac8467b8f2001b22a102934861b65b2f49bc1a`  
		Last Modified: Thu, 26 Jan 2023 10:12:17 GMT  
		Size: 21.4 MB (21395113 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:bionic-20230126` - linux; arm64 variant v8

```console
$ docker pull ubuntu@sha256:f07df923366018f4ac9d2d5b839484e2108d8631ce2872e637049147a47c9b1d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **22.7 MB (22711894 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b2b37ee8ce31e197fba06b7de0b4b07a6fe33e5921918be8d7e1de7b8f25893b`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 26 Jan 2023 10:04:53 GMT
ARG RELEASE
# Thu, 26 Jan 2023 10:04:53 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 10:04:53 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 10:04:53 GMT
LABEL org.opencontainers.image.version=18.04
# Thu, 26 Jan 2023 10:04:56 GMT
ADD file:e7556a99ac088826f5ea581a0c5e2230c1f9a9deab7106e9cec6d1ae8594f19a in / 
# Thu, 26 Jan 2023 10:04:57 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:c2a5dda1e2b0d861ec46a9c576c4fd4d667c56aa4b1cac9cd8c16e629dd11b28`  
		Last Modified: Thu, 26 Jan 2023 10:12:11 GMT  
		Size: 22.7 MB (22711894 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:bionic-20230126` - linux; 386

```console
$ docker pull ubuntu@sha256:8bb84ffaabfe58d03cf9b72ea78d248c57db985525a67ef6f2f0e404b7c59124
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.1 MB (26096513 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:97151d96f64f3b5b7cdb0fadb1c1f8556552cedf32154f23efd48595efabb1e4`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 26 Jan 2023 10:03:01 GMT
ARG RELEASE
# Thu, 26 Jan 2023 10:03:01 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 10:03:01 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 10:03:01 GMT
LABEL org.opencontainers.image.version=18.04
# Thu, 26 Jan 2023 10:03:03 GMT
ADD file:b9b814a7d1e7611a2c531fac3419a48c733c622470d3f275ce29f9ba8764eaeb in / 
# Thu, 26 Jan 2023 10:03:04 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:57a4d5aed2cd4a1f596f693a8fe5e135bd66dbf401ec169b1848d2316bdcfb2c`  
		Last Modified: Thu, 26 Jan 2023 10:12:23 GMT  
		Size: 26.1 MB (26096513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:bionic-20230126` - linux; ppc64le

```console
$ docker pull ubuntu@sha256:721b53fe8a192c32d5077c120a5e253b2bba08b13fcc02c26d6cf63dea715f9f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.4 MB (29351018 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d4e533a2e815a6606d93392dd9f8ff6938a39080b67cfd575045cfe820ede7af`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 26 Jan 2023 09:55:44 GMT
ARG RELEASE
# Thu, 26 Jan 2023 09:55:44 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 09:55:44 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 09:55:44 GMT
LABEL org.opencontainers.image.version=18.04
# Thu, 26 Jan 2023 09:55:47 GMT
ADD file:108aadd723beb46031bfaca610c036aea506955578347dda4a01cfb0c6bdc135 in / 
# Thu, 26 Jan 2023 09:55:48 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:6c790564dfb49a61552a6e89c63c7abf84177d16d0f0fb604df022bfcdc6497b`  
		Last Modified: Thu, 26 Jan 2023 10:12:31 GMT  
		Size: 29.4 MB (29351018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:bionic-20230126` - linux; s390x

```console
$ docker pull ubuntu@sha256:0e9b40aadd1aa55e0cf7f5775b21373a3b028dc9171e729255968e6e5213758c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **24.7 MB (24744933 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5e81833e90b6b40072356a6b1256c20d690401c5130f58b3343b6e30c2eccb64`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 26 Jan 2023 09:55:41 GMT
ARG RELEASE
# Thu, 26 Jan 2023 09:55:41 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 09:55:41 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 09:55:41 GMT
LABEL org.opencontainers.image.version=18.04
# Thu, 26 Jan 2023 09:55:43 GMT
ADD file:04d4137c9183cee18560fc26a092e288ff403f3dde266237eab245bd38eb9b3a in / 
# Thu, 26 Jan 2023 09:55:43 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:9e75830a8e632695dde0b55ec0159bd7b141ab79858367e3f66bfa5f255aaec9`  
		Last Modified: Thu, 26 Jan 2023 10:12:37 GMT  
		Size: 24.7 MB (24744933 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ubuntu:devel`

```console
$ docker pull ubuntu@sha256:e2e6dfaf4d892b0430e636f2747c3a19d47a806a1fc21810743c113ca59ab6a2
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `ubuntu:devel` - linux; amd64

```console
$ docker pull ubuntu@sha256:76f55c747c6e3cc7a49f6bade839a8fbca72e0338fec92b54e58b8d15baf836d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.6 MB (26594295 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:096628db4ff280b69ee9eaca21f0cfc152776e1243bc6c1320b436934188d5e5`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 25 Jan 2023 14:47:05 GMT
ARG RELEASE
# Wed, 25 Jan 2023 14:47:05 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 25 Jan 2023 14:47:05 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 25 Jan 2023 14:47:05 GMT
LABEL org.opencontainers.image.version=23.04
# Wed, 25 Jan 2023 14:47:07 GMT
ADD file:5a9904395b52775ee7c10a49efc741d32b587e2cd447b8deb66811c3fb3b37a4 in / 
# Wed, 25 Jan 2023 14:47:07 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:85cec64d15ef8b1eb3ff65555dbe92d7e3ea2a21f3e1fe1206ed85e221b3593d`  
		Last Modified: Wed, 25 Jan 2023 14:56:49 GMT  
		Size: 26.6 MB (26594295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:devel` - linux; arm variant v7

```console
$ docker pull ubuntu@sha256:1d8b24f64674c975ae2ca8b10f39a8c79cca25e278d9fe6438bddef61307e3f1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.1 MB (25095764 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9f55f15212572f043ec357086e290a82ab554094f4f7f044746ff6dec8d96428`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 25 Jan 2023 14:38:25 GMT
ARG RELEASE
# Wed, 25 Jan 2023 14:38:25 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 25 Jan 2023 14:38:26 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 25 Jan 2023 14:38:26 GMT
LABEL org.opencontainers.image.version=23.04
# Wed, 25 Jan 2023 14:38:35 GMT
ADD file:c01025be735c65553980246358cbe7c563769d7ffc886d18be817582a0d29b5c in / 
# Wed, 25 Jan 2023 14:38:36 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:f9e87c970a05364b1b6a0c18043b8cc663c1dcd5b370d87043288950fabb675a`  
		Last Modified: Wed, 25 Jan 2023 14:57:02 GMT  
		Size: 25.1 MB (25095764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:devel` - linux; arm64 variant v8

```console
$ docker pull ubuntu@sha256:601b47b473ab776a59e725ab6bde002ed7b271b9531dc72d602c033b0c578879
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.8 MB (25777338 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:39efbc92de18d58fc90c5503a1f69c3dccce7e29830cc6560ec6857f8b6485e5`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 25 Jan 2023 14:42:22 GMT
ARG RELEASE
# Wed, 25 Jan 2023 14:42:23 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 25 Jan 2023 14:42:23 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 25 Jan 2023 14:42:23 GMT
LABEL org.opencontainers.image.version=23.04
# Wed, 25 Jan 2023 14:42:31 GMT
ADD file:6713306ff9bcc18c79430d43aafbbe519176e76b7232c563993ebda6c8caf738 in / 
# Wed, 25 Jan 2023 14:42:32 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:ce743a0a7eb81f2756829eb9afb29c85ce40ded304387cdd06f66b01793ac464`  
		Last Modified: Wed, 25 Jan 2023 14:56:55 GMT  
		Size: 25.8 MB (25777338 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:devel` - linux; ppc64le

```console
$ docker pull ubuntu@sha256:67fe8ea65e1c908351ee7dbc6cf56660fc0d3ef49b8046aeb61e3df7fbd5172d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.0 MB (30959485 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c420642d8d83f69bc1f4eba5096256ff91343014b4d8dbdfcead8b96635f6c11`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 25 Jan 2023 14:48:03 GMT
ARG RELEASE
# Wed, 25 Jan 2023 14:48:03 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 25 Jan 2023 14:48:03 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 25 Jan 2023 14:48:04 GMT
LABEL org.opencontainers.image.version=23.04
# Wed, 25 Jan 2023 14:48:07 GMT
ADD file:5002466754dcd29080099171ab20675c9bcc55f0befbe928008127d14c027297 in / 
# Wed, 25 Jan 2023 14:48:07 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:8215a53a3d6e58238feac2e65d9c57d1f382d8ade421475347b3c522198afe4e`  
		Last Modified: Wed, 25 Jan 2023 14:57:08 GMT  
		Size: 31.0 MB (30959485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:devel` - linux; s390x

```console
$ docker pull ubuntu@sha256:87dc7c1f1d0b9cdb25c2e1cfdcd05569ab54f7949365a8aa8677d6098f57273d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.5 MB (25455083 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2a5869fd440bbbebdfc74dcec9c949501d695f868ff73d63165a920e39d8bfca`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 25 Jan 2023 14:49:06 GMT
ARG RELEASE
# Wed, 25 Jan 2023 14:49:06 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 25 Jan 2023 14:49:06 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 25 Jan 2023 14:49:06 GMT
LABEL org.opencontainers.image.version=23.04
# Wed, 25 Jan 2023 14:49:08 GMT
ADD file:81c93bf9ec11b910a5bae8b977a82a78cb327c7bf9d0991542c9b6847cf19210 in / 
# Wed, 25 Jan 2023 14:49:12 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:f6119d8ec48acf1c2965d2233f93e21ee590564bbae9fd360b9630c3b6c694f9`  
		Last Modified: Wed, 25 Jan 2023 14:57:22 GMT  
		Size: 25.5 MB (25455083 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ubuntu:focal`

```console
$ docker pull ubuntu@sha256:b33325a00c7c27b23ae48cf17d2c654e2c30812b35e7846c006389318f6a71c2
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `ubuntu:focal` - linux; amd64

```console
$ docker pull ubuntu@sha256:d5d4814ffb155d588f10ec8926d9e1cd09b6d41a3110d2f42959e2fc37f6d0b4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.5 MB (27503418 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f32fe8df6a4c91a6bfe1fae9ffa5a05bac157d0edd78571d34c3c784985d95f7`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 26 Jan 2023 13:19:55 GMT
ARG RELEASE
# Thu, 26 Jan 2023 13:19:55 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 13:19:55 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 13:19:55 GMT
LABEL org.opencontainers.image.version=20.04
# Thu, 26 Jan 2023 13:19:57 GMT
ADD file:8b180a9b4497de0c6e131d6b48cf5c69a885379e63033ab9639d1655991e626c in / 
# Thu, 26 Jan 2023 13:19:57 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:bdec8b63443ac80dc7fdf49c2b5bbe08191e0f5fda5f1f5d6b5f25263cfa2c47`  
		Last Modified: Thu, 26 Jan 2023 14:01:47 GMT  
		Size: 27.5 MB (27503418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:focal` - linux; arm variant v7

```console
$ docker pull ubuntu@sha256:d5d767be339687f755e936fffaa860a965316ebb23035242994ff7e3a8e26472
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.6 MB (23608452 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e7fd2989c767b17f419f4a0fd29ff08ee906380dc2d5963e51ed44537f16bcdb`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 26 Jan 2023 13:35:44 GMT
ARG RELEASE
# Thu, 26 Jan 2023 13:35:44 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 13:35:44 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 13:35:44 GMT
LABEL org.opencontainers.image.version=20.04
# Thu, 26 Jan 2023 13:35:48 GMT
ADD file:6566d63937dd1808d3a4ea5591d4369b9083772d48fad60626fb91243a9f3f53 in / 
# Thu, 26 Jan 2023 13:35:49 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:325e20204bae7a15035068b8043b4abc0f59c014564bf465b3a99757175402ce`  
		Last Modified: Thu, 26 Jan 2023 14:02:03 GMT  
		Size: 23.6 MB (23608452 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:focal` - linux; arm64 variant v8

```console
$ docker pull ubuntu@sha256:a840dd8130bfe149a60f0ad6ca972b7259f9c55e323b16b659f58af2eb6dabfa
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.0 MB (25972163 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e26da238ce02fc608d0410d966f12d91d42677ecaa5df68dd325efdddb8fb85e`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 26 Jan 2023 13:50:26 GMT
ARG RELEASE
# Thu, 26 Jan 2023 13:50:26 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 13:50:26 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 13:50:26 GMT
LABEL org.opencontainers.image.version=20.04
# Thu, 26 Jan 2023 13:50:33 GMT
ADD file:72ca0af0100de6591b59c44bd8856655c8441eb0fcbf7c32e427f6be5108a4a4 in / 
# Thu, 26 Jan 2023 13:50:33 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:ffe6f70103a5896ebe7878266832cd044ef7b46fa905937864c9e9be67b38351`  
		Last Modified: Thu, 26 Jan 2023 14:01:54 GMT  
		Size: 26.0 MB (25972163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:focal` - linux; ppc64le

```console
$ docker pull ubuntu@sha256:cebffa8cceec4bea7ef66193cc86b9ad216bd45292ccd79e2ea9a6830a568e4c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.1 MB (32068234 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6a6fe6633addd2a7fd34c33cdfeebefac8d57eb53ebe773fc66f22c5ccca8998`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 26 Jan 2023 13:47:16 GMT
ARG RELEASE
# Thu, 26 Jan 2023 13:47:16 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 13:47:17 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 13:47:17 GMT
LABEL org.opencontainers.image.version=20.04
# Thu, 26 Jan 2023 13:47:20 GMT
ADD file:987b941a34ad98533c64e74a3d57b9c1b983ff16c8f36e21d29278a30a2403ee in / 
# Thu, 26 Jan 2023 13:47:20 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:78c13b83c7cdda97b53d4407c98b39430a4d2a175fa9aff8503068948e87dd9a`  
		Last Modified: Thu, 26 Jan 2023 14:02:09 GMT  
		Size: 32.1 MB (32068234 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:focal` - linux; s390x

```console
$ docker pull ubuntu@sha256:602b58d620499c50ae12f6fc2d7f6caa0fe5e00875dd7b2d291c595199c6fb43
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.4 MB (26363789 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:61b58fa4a9492ff8aba7316c0156c6d47890115d6865b7fe9eec96611ae2ee0a`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 26 Jan 2023 13:21:27 GMT
ARG RELEASE
# Thu, 26 Jan 2023 13:21:27 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 13:21:27 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 13:21:27 GMT
LABEL org.opencontainers.image.version=20.04
# Thu, 26 Jan 2023 13:21:29 GMT
ADD file:4d5fa9b68af51e9c8cd7b25fb55ddd47256efb0b2eda9432507b72b7c1a17053 in / 
# Thu, 26 Jan 2023 13:21:30 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:870f83892b5769f235d9116edab9c19d569d14d716bcd10b90ab5314292fd908`  
		Last Modified: Thu, 26 Jan 2023 14:02:16 GMT  
		Size: 26.4 MB (26363789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ubuntu:focal-20230126`

```console
$ docker pull ubuntu@sha256:b33325a00c7c27b23ae48cf17d2c654e2c30812b35e7846c006389318f6a71c2
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `ubuntu:focal-20230126` - linux; amd64

```console
$ docker pull ubuntu@sha256:d5d4814ffb155d588f10ec8926d9e1cd09b6d41a3110d2f42959e2fc37f6d0b4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.5 MB (27503418 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f32fe8df6a4c91a6bfe1fae9ffa5a05bac157d0edd78571d34c3c784985d95f7`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 26 Jan 2023 13:19:55 GMT
ARG RELEASE
# Thu, 26 Jan 2023 13:19:55 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 13:19:55 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 13:19:55 GMT
LABEL org.opencontainers.image.version=20.04
# Thu, 26 Jan 2023 13:19:57 GMT
ADD file:8b180a9b4497de0c6e131d6b48cf5c69a885379e63033ab9639d1655991e626c in / 
# Thu, 26 Jan 2023 13:19:57 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:bdec8b63443ac80dc7fdf49c2b5bbe08191e0f5fda5f1f5d6b5f25263cfa2c47`  
		Last Modified: Thu, 26 Jan 2023 14:01:47 GMT  
		Size: 27.5 MB (27503418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:focal-20230126` - linux; arm variant v7

```console
$ docker pull ubuntu@sha256:d5d767be339687f755e936fffaa860a965316ebb23035242994ff7e3a8e26472
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.6 MB (23608452 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e7fd2989c767b17f419f4a0fd29ff08ee906380dc2d5963e51ed44537f16bcdb`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 26 Jan 2023 13:35:44 GMT
ARG RELEASE
# Thu, 26 Jan 2023 13:35:44 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 13:35:44 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 13:35:44 GMT
LABEL org.opencontainers.image.version=20.04
# Thu, 26 Jan 2023 13:35:48 GMT
ADD file:6566d63937dd1808d3a4ea5591d4369b9083772d48fad60626fb91243a9f3f53 in / 
# Thu, 26 Jan 2023 13:35:49 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:325e20204bae7a15035068b8043b4abc0f59c014564bf465b3a99757175402ce`  
		Last Modified: Thu, 26 Jan 2023 14:02:03 GMT  
		Size: 23.6 MB (23608452 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:focal-20230126` - linux; arm64 variant v8

```console
$ docker pull ubuntu@sha256:a840dd8130bfe149a60f0ad6ca972b7259f9c55e323b16b659f58af2eb6dabfa
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.0 MB (25972163 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e26da238ce02fc608d0410d966f12d91d42677ecaa5df68dd325efdddb8fb85e`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 26 Jan 2023 13:50:26 GMT
ARG RELEASE
# Thu, 26 Jan 2023 13:50:26 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 13:50:26 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 13:50:26 GMT
LABEL org.opencontainers.image.version=20.04
# Thu, 26 Jan 2023 13:50:33 GMT
ADD file:72ca0af0100de6591b59c44bd8856655c8441eb0fcbf7c32e427f6be5108a4a4 in / 
# Thu, 26 Jan 2023 13:50:33 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:ffe6f70103a5896ebe7878266832cd044ef7b46fa905937864c9e9be67b38351`  
		Last Modified: Thu, 26 Jan 2023 14:01:54 GMT  
		Size: 26.0 MB (25972163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:focal-20230126` - linux; ppc64le

```console
$ docker pull ubuntu@sha256:cebffa8cceec4bea7ef66193cc86b9ad216bd45292ccd79e2ea9a6830a568e4c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.1 MB (32068234 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6a6fe6633addd2a7fd34c33cdfeebefac8d57eb53ebe773fc66f22c5ccca8998`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 26 Jan 2023 13:47:16 GMT
ARG RELEASE
# Thu, 26 Jan 2023 13:47:16 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 13:47:17 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 13:47:17 GMT
LABEL org.opencontainers.image.version=20.04
# Thu, 26 Jan 2023 13:47:20 GMT
ADD file:987b941a34ad98533c64e74a3d57b9c1b983ff16c8f36e21d29278a30a2403ee in / 
# Thu, 26 Jan 2023 13:47:20 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:78c13b83c7cdda97b53d4407c98b39430a4d2a175fa9aff8503068948e87dd9a`  
		Last Modified: Thu, 26 Jan 2023 14:02:09 GMT  
		Size: 32.1 MB (32068234 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:focal-20230126` - linux; s390x

```console
$ docker pull ubuntu@sha256:602b58d620499c50ae12f6fc2d7f6caa0fe5e00875dd7b2d291c595199c6fb43
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.4 MB (26363789 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:61b58fa4a9492ff8aba7316c0156c6d47890115d6865b7fe9eec96611ae2ee0a`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 26 Jan 2023 13:21:27 GMT
ARG RELEASE
# Thu, 26 Jan 2023 13:21:27 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 13:21:27 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 13:21:27 GMT
LABEL org.opencontainers.image.version=20.04
# Thu, 26 Jan 2023 13:21:29 GMT
ADD file:4d5fa9b68af51e9c8cd7b25fb55ddd47256efb0b2eda9432507b72b7c1a17053 in / 
# Thu, 26 Jan 2023 13:21:30 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:870f83892b5769f235d9116edab9c19d569d14d716bcd10b90ab5314292fd908`  
		Last Modified: Thu, 26 Jan 2023 14:02:16 GMT  
		Size: 26.4 MB (26363789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ubuntu:jammy`

```console
$ docker pull ubuntu@sha256:f05532b6a1dec5f7a77a8d684af87bc9cd1f2b32eab301c109f8ad151b5565d1
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `ubuntu:jammy` - linux; amd64

```console
$ docker pull ubuntu@sha256:eecba05a9ccbc219cb0f0dd280034c6ee1aab0b00b458e680f9c4efc6ca3feda
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.5 MB (29528717 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:58db3edaf2be6e80f628796355b1bdeaf8bea1692b402f48b7e7b8d1ff100b02`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 26 Jan 2023 04:57:59 GMT
ARG RELEASE
# Thu, 26 Jan 2023 04:57:59 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 04:58:00 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 04:58:00 GMT
LABEL org.opencontainers.image.version=22.04
# Thu, 26 Jan 2023 04:58:02 GMT
ADD file:18e71f049606f6339ce7a995839623f50e6ec6474bfd0a3a7ca799db726f47f6 in / 
# Thu, 26 Jan 2023 04:58:02 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:677076032cca0a2362d25cf3660072e738d1b96fe860409a33ce901d695d7ee8`  
		Last Modified: Thu, 26 Jan 2023 05:13:54 GMT  
		Size: 29.5 MB (29528717 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:jammy` - linux; arm variant v7

```console
$ docker pull ubuntu@sha256:5c3735e92e29c51fa2ac513ea7d130e0ea61de153abdf28974afc83cf5dfa8cf
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.1 MB (26137949 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b15b861da44337925963eb70b8671950999df7d8abfe7f5a9b5f95ff9f4cca7a`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 26 Jan 2023 05:05:40 GMT
ARG RELEASE
# Thu, 26 Jan 2023 05:05:40 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 05:05:40 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 05:05:40 GMT
LABEL org.opencontainers.image.version=22.04
# Thu, 26 Jan 2023 05:05:43 GMT
ADD file:12d2a7ddc8445b8f97c960075216eb8e8cd226b84259c7343ef15c65a440b500 in / 
# Thu, 26 Jan 2023 05:05:43 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:860e874323ae800886f85ab5c346783e3a9371bd9beb72c5f25e8e20c9dd18bb`  
		Last Modified: Thu, 26 Jan 2023 05:14:09 GMT  
		Size: 26.1 MB (26137949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:jammy` - linux; arm64 variant v8

```console
$ docker pull ubuntu@sha256:13e180ab78513dbe30a4f5a9e35acc6f61d92cbccac887a4f11ea23516261cc0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.3 MB (27342387 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a6be1f66f70f66ef43503292e38ccbfc14f2d5464e7736344783a8fc7bb339a8`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 26 Jan 2023 05:05:49 GMT
ARG RELEASE
# Thu, 26 Jan 2023 05:05:49 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 05:05:49 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 05:05:50 GMT
LABEL org.opencontainers.image.version=22.04
# Thu, 26 Jan 2023 05:05:51 GMT
ADD file:55486a91f732042dd4e81ecfd8457d23e04dcd7dd80a0bb06cc7c44873fac838 in / 
# Thu, 26 Jan 2023 05:05:51 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:8b150fd943bcd54ef788cece17523d19031f745b099a798de65247900d102e18`  
		Last Modified: Thu, 26 Jan 2023 05:14:03 GMT  
		Size: 27.3 MB (27342387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:jammy` - linux; ppc64le

```console
$ docker pull ubuntu@sha256:ed40c990366092268d72da08b90fb5a0f6081ab1e00918c6453e64443d775dca
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.6 MB (34588568 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d899338973bac5fb325b647c7436507e44918374fff2a72b0da6515946c868a7`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 26 Jan 2023 04:58:24 GMT
ARG RELEASE
# Thu, 26 Jan 2023 04:58:24 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 04:58:24 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 04:58:24 GMT
LABEL org.opencontainers.image.version=22.04
# Thu, 26 Jan 2023 04:58:28 GMT
ADD file:f0400001a50847feb579e66e804ec9daaaaeb9a414b4b5cca8bb0c8e9c7fa8f9 in / 
# Thu, 26 Jan 2023 04:58:28 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:717e115780fa5a198871a9eef15e446084728bf7021e7894e6118f3cd6d26b60`  
		Last Modified: Thu, 26 Jan 2023 05:14:15 GMT  
		Size: 34.6 MB (34588568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:jammy` - linux; s390x

```console
$ docker pull ubuntu@sha256:d3df0130c5dc92778c7513686bb9f10d5e2e710b7f290d686bda24ac351d3220
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.0 MB (28009396 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6abbed079020c533dbc7ca626067d743bf7effce2e4c895f104846afd8f4943a`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 26 Jan 2023 05:08:35 GMT
ARG RELEASE
# Thu, 26 Jan 2023 05:08:35 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 05:08:36 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 05:08:36 GMT
LABEL org.opencontainers.image.version=22.04
# Thu, 26 Jan 2023 05:08:37 GMT
ADD file:a9794efc1a102ab6a7160e660a63f4b267797b8b7e0b0bfd9c04ed62846cfb36 in / 
# Thu, 26 Jan 2023 05:08:38 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:f8e318d098424cef87513f4c834987f20c608791646c6b1a3ef60ed57408ddb6`  
		Last Modified: Thu, 26 Jan 2023 05:14:22 GMT  
		Size: 28.0 MB (28009396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ubuntu:jammy-20230126`

```console
$ docker pull ubuntu@sha256:f05532b6a1dec5f7a77a8d684af87bc9cd1f2b32eab301c109f8ad151b5565d1
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `ubuntu:jammy-20230126` - linux; amd64

```console
$ docker pull ubuntu@sha256:eecba05a9ccbc219cb0f0dd280034c6ee1aab0b00b458e680f9c4efc6ca3feda
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.5 MB (29528717 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:58db3edaf2be6e80f628796355b1bdeaf8bea1692b402f48b7e7b8d1ff100b02`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 26 Jan 2023 04:57:59 GMT
ARG RELEASE
# Thu, 26 Jan 2023 04:57:59 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 04:58:00 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 04:58:00 GMT
LABEL org.opencontainers.image.version=22.04
# Thu, 26 Jan 2023 04:58:02 GMT
ADD file:18e71f049606f6339ce7a995839623f50e6ec6474bfd0a3a7ca799db726f47f6 in / 
# Thu, 26 Jan 2023 04:58:02 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:677076032cca0a2362d25cf3660072e738d1b96fe860409a33ce901d695d7ee8`  
		Last Modified: Thu, 26 Jan 2023 05:13:54 GMT  
		Size: 29.5 MB (29528717 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:jammy-20230126` - linux; arm variant v7

```console
$ docker pull ubuntu@sha256:5c3735e92e29c51fa2ac513ea7d130e0ea61de153abdf28974afc83cf5dfa8cf
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.1 MB (26137949 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b15b861da44337925963eb70b8671950999df7d8abfe7f5a9b5f95ff9f4cca7a`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 26 Jan 2023 05:05:40 GMT
ARG RELEASE
# Thu, 26 Jan 2023 05:05:40 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 05:05:40 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 05:05:40 GMT
LABEL org.opencontainers.image.version=22.04
# Thu, 26 Jan 2023 05:05:43 GMT
ADD file:12d2a7ddc8445b8f97c960075216eb8e8cd226b84259c7343ef15c65a440b500 in / 
# Thu, 26 Jan 2023 05:05:43 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:860e874323ae800886f85ab5c346783e3a9371bd9beb72c5f25e8e20c9dd18bb`  
		Last Modified: Thu, 26 Jan 2023 05:14:09 GMT  
		Size: 26.1 MB (26137949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:jammy-20230126` - linux; arm64 variant v8

```console
$ docker pull ubuntu@sha256:13e180ab78513dbe30a4f5a9e35acc6f61d92cbccac887a4f11ea23516261cc0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.3 MB (27342387 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a6be1f66f70f66ef43503292e38ccbfc14f2d5464e7736344783a8fc7bb339a8`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 26 Jan 2023 05:05:49 GMT
ARG RELEASE
# Thu, 26 Jan 2023 05:05:49 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 05:05:49 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 05:05:50 GMT
LABEL org.opencontainers.image.version=22.04
# Thu, 26 Jan 2023 05:05:51 GMT
ADD file:55486a91f732042dd4e81ecfd8457d23e04dcd7dd80a0bb06cc7c44873fac838 in / 
# Thu, 26 Jan 2023 05:05:51 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:8b150fd943bcd54ef788cece17523d19031f745b099a798de65247900d102e18`  
		Last Modified: Thu, 26 Jan 2023 05:14:03 GMT  
		Size: 27.3 MB (27342387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:jammy-20230126` - linux; ppc64le

```console
$ docker pull ubuntu@sha256:ed40c990366092268d72da08b90fb5a0f6081ab1e00918c6453e64443d775dca
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.6 MB (34588568 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d899338973bac5fb325b647c7436507e44918374fff2a72b0da6515946c868a7`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 26 Jan 2023 04:58:24 GMT
ARG RELEASE
# Thu, 26 Jan 2023 04:58:24 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 04:58:24 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 04:58:24 GMT
LABEL org.opencontainers.image.version=22.04
# Thu, 26 Jan 2023 04:58:28 GMT
ADD file:f0400001a50847feb579e66e804ec9daaaaeb9a414b4b5cca8bb0c8e9c7fa8f9 in / 
# Thu, 26 Jan 2023 04:58:28 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:717e115780fa5a198871a9eef15e446084728bf7021e7894e6118f3cd6d26b60`  
		Last Modified: Thu, 26 Jan 2023 05:14:15 GMT  
		Size: 34.6 MB (34588568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:jammy-20230126` - linux; s390x

```console
$ docker pull ubuntu@sha256:d3df0130c5dc92778c7513686bb9f10d5e2e710b7f290d686bda24ac351d3220
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.0 MB (28009396 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6abbed079020c533dbc7ca626067d743bf7effce2e4c895f104846afd8f4943a`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 26 Jan 2023 05:08:35 GMT
ARG RELEASE
# Thu, 26 Jan 2023 05:08:35 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 05:08:36 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 05:08:36 GMT
LABEL org.opencontainers.image.version=22.04
# Thu, 26 Jan 2023 05:08:37 GMT
ADD file:a9794efc1a102ab6a7160e660a63f4b267797b8b7e0b0bfd9c04ed62846cfb36 in / 
# Thu, 26 Jan 2023 05:08:38 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:f8e318d098424cef87513f4c834987f20c608791646c6b1a3ef60ed57408ddb6`  
		Last Modified: Thu, 26 Jan 2023 05:14:22 GMT  
		Size: 28.0 MB (28009396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ubuntu:kinetic`

```console
$ docker pull ubuntu@sha256:a062bfdb0c233a5a7c4758c028ef6a8f4981b78008606e23f47143ca0bfb483d
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `ubuntu:kinetic` - linux; amd64

```console
$ docker pull ubuntu@sha256:ef3c777a7db8a2c49d31284cc924fc3a2f471dce44378a18d6d1fefff5a63fe5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.7 MB (26691650 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:10c2f4041af137e6b0ba5c793df3dfdf4e72a4e011ce6847f4cc0247b9bbf7f2`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 26 Jan 2023 11:51:12 GMT
ARG RELEASE
# Thu, 26 Jan 2023 11:51:12 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 11:51:12 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 11:51:13 GMT
LABEL org.opencontainers.image.version=22.10
# Thu, 26 Jan 2023 11:51:14 GMT
ADD file:e886423892b371751386c0ce7147599acb72d8fb528eaaa78092b879d9ff58ce in / 
# Thu, 26 Jan 2023 11:51:15 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:256644d5a307c3efeca6ae2854b6329a2753157868dc5548e33161b377658e6a`  
		Last Modified: Thu, 26 Jan 2023 12:14:04 GMT  
		Size: 26.7 MB (26691650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:kinetic` - linux; arm variant v7

```console
$ docker pull ubuntu@sha256:a9fd5288ceabc4990263038e3ff67154088e5df217fd2eaed5ac7fce8318d84a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.1 MB (25066997 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8d643d5974c30c06b1d811877a3a8f0047c4278b1fe0801d8d812b3a17ce6c15`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 26 Jan 2023 11:52:00 GMT
ARG RELEASE
# Thu, 26 Jan 2023 11:52:00 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 11:52:00 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 11:52:00 GMT
LABEL org.opencontainers.image.version=22.10
# Thu, 26 Jan 2023 11:52:03 GMT
ADD file:d35c57b0dc2840a8b1ef40f7f6cfd826da68611f1ba37a89a382618c8612b52c in / 
# Thu, 26 Jan 2023 11:52:03 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:697d38f8dfe625e3e751c0b01ddeaaeeff6e8d6f594dd7da227aea3974a49ce1`  
		Last Modified: Thu, 26 Jan 2023 12:14:16 GMT  
		Size: 25.1 MB (25066997 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:kinetic` - linux; arm64 variant v8

```console
$ docker pull ubuntu@sha256:aff210956f022245b200f8be680a99c7d93f191b2cfc8d6f770f87ef3644a080
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.8 MB (25757647 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c7096432b6a9855592152ad8009431b92d7aa40980c9c94684fcc72626bbbab9`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 26 Jan 2023 12:08:18 GMT
ARG RELEASE
# Thu, 26 Jan 2023 12:08:18 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 12:08:18 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 12:08:18 GMT
LABEL org.opencontainers.image.version=22.10
# Thu, 26 Jan 2023 12:08:20 GMT
ADD file:f61617371f6963c6be2852e2b94d04e8507feb8f77e3484c94aa8b9d0ac67f76 in / 
# Thu, 26 Jan 2023 12:08:20 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:05f69cab0b799028e03233ffa93abd2d0b426412cff70959a07a29a437447ee3`  
		Last Modified: Thu, 26 Jan 2023 12:14:10 GMT  
		Size: 25.8 MB (25757647 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:kinetic` - linux; ppc64le

```console
$ docker pull ubuntu@sha256:daab817634ed004a6c564aec6ca0a0d84205d49371765eb625366344ceb7d5bd
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.1 MB (31110147 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5dfbc0b60efcd8ea2a51c157e7bc286d8de7e88ae1bf756e0d8a44ff107e21c7`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 26 Jan 2023 11:57:00 GMT
ARG RELEASE
# Thu, 26 Jan 2023 11:57:00 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 11:57:00 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 11:57:00 GMT
LABEL org.opencontainers.image.version=22.10
# Thu, 26 Jan 2023 11:57:03 GMT
ADD file:3c2bc98d283cce5149d7992233f5fe644b7239417045faf3f93750b92de5f68e in / 
# Thu, 26 Jan 2023 11:57:04 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:8da618ff876e10064f550b9dc5b51b0d0ae6939f67b56ce9a0c7fa8bb77de40f`  
		Last Modified: Thu, 26 Jan 2023 12:14:22 GMT  
		Size: 31.1 MB (31110147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:kinetic` - linux; s390x

```console
$ docker pull ubuntu@sha256:944066fb6be279b0de11cb4ecc57c81794b912ba6f95a544f3d462ceab3a78a6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.5 MB (25487159 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:91297aceb6d3e297e45ec91916dbea079b90ae1c7edbaf14a99c41d3f493f537`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 26 Jan 2023 12:08:47 GMT
ARG RELEASE
# Thu, 26 Jan 2023 12:08:47 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 12:08:48 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 12:08:48 GMT
LABEL org.opencontainers.image.version=22.10
# Thu, 26 Jan 2023 12:08:50 GMT
ADD file:a83afd93816f868be76d243df85b87a66b39d5ef0497c3cb8d0bba2bd4a27c40 in / 
# Thu, 26 Jan 2023 12:08:50 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:fe4914a812d394969d56f220e5ddb037a62164607a937ca866bf4ee592a8799a`  
		Last Modified: Thu, 26 Jan 2023 12:14:28 GMT  
		Size: 25.5 MB (25487159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ubuntu:kinetic-20230126`

```console
$ docker pull ubuntu@sha256:a062bfdb0c233a5a7c4758c028ef6a8f4981b78008606e23f47143ca0bfb483d
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `ubuntu:kinetic-20230126` - linux; amd64

```console
$ docker pull ubuntu@sha256:ef3c777a7db8a2c49d31284cc924fc3a2f471dce44378a18d6d1fefff5a63fe5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.7 MB (26691650 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:10c2f4041af137e6b0ba5c793df3dfdf4e72a4e011ce6847f4cc0247b9bbf7f2`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 26 Jan 2023 11:51:12 GMT
ARG RELEASE
# Thu, 26 Jan 2023 11:51:12 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 11:51:12 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 11:51:13 GMT
LABEL org.opencontainers.image.version=22.10
# Thu, 26 Jan 2023 11:51:14 GMT
ADD file:e886423892b371751386c0ce7147599acb72d8fb528eaaa78092b879d9ff58ce in / 
# Thu, 26 Jan 2023 11:51:15 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:256644d5a307c3efeca6ae2854b6329a2753157868dc5548e33161b377658e6a`  
		Last Modified: Thu, 26 Jan 2023 12:14:04 GMT  
		Size: 26.7 MB (26691650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:kinetic-20230126` - linux; arm variant v7

```console
$ docker pull ubuntu@sha256:a9fd5288ceabc4990263038e3ff67154088e5df217fd2eaed5ac7fce8318d84a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.1 MB (25066997 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8d643d5974c30c06b1d811877a3a8f0047c4278b1fe0801d8d812b3a17ce6c15`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 26 Jan 2023 11:52:00 GMT
ARG RELEASE
# Thu, 26 Jan 2023 11:52:00 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 11:52:00 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 11:52:00 GMT
LABEL org.opencontainers.image.version=22.10
# Thu, 26 Jan 2023 11:52:03 GMT
ADD file:d35c57b0dc2840a8b1ef40f7f6cfd826da68611f1ba37a89a382618c8612b52c in / 
# Thu, 26 Jan 2023 11:52:03 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:697d38f8dfe625e3e751c0b01ddeaaeeff6e8d6f594dd7da227aea3974a49ce1`  
		Last Modified: Thu, 26 Jan 2023 12:14:16 GMT  
		Size: 25.1 MB (25066997 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:kinetic-20230126` - linux; arm64 variant v8

```console
$ docker pull ubuntu@sha256:aff210956f022245b200f8be680a99c7d93f191b2cfc8d6f770f87ef3644a080
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.8 MB (25757647 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c7096432b6a9855592152ad8009431b92d7aa40980c9c94684fcc72626bbbab9`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 26 Jan 2023 12:08:18 GMT
ARG RELEASE
# Thu, 26 Jan 2023 12:08:18 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 12:08:18 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 12:08:18 GMT
LABEL org.opencontainers.image.version=22.10
# Thu, 26 Jan 2023 12:08:20 GMT
ADD file:f61617371f6963c6be2852e2b94d04e8507feb8f77e3484c94aa8b9d0ac67f76 in / 
# Thu, 26 Jan 2023 12:08:20 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:05f69cab0b799028e03233ffa93abd2d0b426412cff70959a07a29a437447ee3`  
		Last Modified: Thu, 26 Jan 2023 12:14:10 GMT  
		Size: 25.8 MB (25757647 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:kinetic-20230126` - linux; ppc64le

```console
$ docker pull ubuntu@sha256:daab817634ed004a6c564aec6ca0a0d84205d49371765eb625366344ceb7d5bd
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.1 MB (31110147 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5dfbc0b60efcd8ea2a51c157e7bc286d8de7e88ae1bf756e0d8a44ff107e21c7`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 26 Jan 2023 11:57:00 GMT
ARG RELEASE
# Thu, 26 Jan 2023 11:57:00 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 11:57:00 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 11:57:00 GMT
LABEL org.opencontainers.image.version=22.10
# Thu, 26 Jan 2023 11:57:03 GMT
ADD file:3c2bc98d283cce5149d7992233f5fe644b7239417045faf3f93750b92de5f68e in / 
# Thu, 26 Jan 2023 11:57:04 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:8da618ff876e10064f550b9dc5b51b0d0ae6939f67b56ce9a0c7fa8bb77de40f`  
		Last Modified: Thu, 26 Jan 2023 12:14:22 GMT  
		Size: 31.1 MB (31110147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:kinetic-20230126` - linux; s390x

```console
$ docker pull ubuntu@sha256:944066fb6be279b0de11cb4ecc57c81794b912ba6f95a544f3d462ceab3a78a6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.5 MB (25487159 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:91297aceb6d3e297e45ec91916dbea079b90ae1c7edbaf14a99c41d3f493f537`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 26 Jan 2023 12:08:47 GMT
ARG RELEASE
# Thu, 26 Jan 2023 12:08:47 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 12:08:48 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 12:08:48 GMT
LABEL org.opencontainers.image.version=22.10
# Thu, 26 Jan 2023 12:08:50 GMT
ADD file:a83afd93816f868be76d243df85b87a66b39d5ef0497c3cb8d0bba2bd4a27c40 in / 
# Thu, 26 Jan 2023 12:08:50 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:fe4914a812d394969d56f220e5ddb037a62164607a937ca866bf4ee592a8799a`  
		Last Modified: Thu, 26 Jan 2023 12:14:28 GMT  
		Size: 25.5 MB (25487159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ubuntu:latest`

```console
$ docker pull ubuntu@sha256:f05532b6a1dec5f7a77a8d684af87bc9cd1f2b32eab301c109f8ad151b5565d1
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `ubuntu:latest` - linux; amd64

```console
$ docker pull ubuntu@sha256:eecba05a9ccbc219cb0f0dd280034c6ee1aab0b00b458e680f9c4efc6ca3feda
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.5 MB (29528717 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:58db3edaf2be6e80f628796355b1bdeaf8bea1692b402f48b7e7b8d1ff100b02`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 26 Jan 2023 04:57:59 GMT
ARG RELEASE
# Thu, 26 Jan 2023 04:57:59 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 04:58:00 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 04:58:00 GMT
LABEL org.opencontainers.image.version=22.04
# Thu, 26 Jan 2023 04:58:02 GMT
ADD file:18e71f049606f6339ce7a995839623f50e6ec6474bfd0a3a7ca799db726f47f6 in / 
# Thu, 26 Jan 2023 04:58:02 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:677076032cca0a2362d25cf3660072e738d1b96fe860409a33ce901d695d7ee8`  
		Last Modified: Thu, 26 Jan 2023 05:13:54 GMT  
		Size: 29.5 MB (29528717 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:latest` - linux; arm variant v7

```console
$ docker pull ubuntu@sha256:5c3735e92e29c51fa2ac513ea7d130e0ea61de153abdf28974afc83cf5dfa8cf
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.1 MB (26137949 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b15b861da44337925963eb70b8671950999df7d8abfe7f5a9b5f95ff9f4cca7a`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 26 Jan 2023 05:05:40 GMT
ARG RELEASE
# Thu, 26 Jan 2023 05:05:40 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 05:05:40 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 05:05:40 GMT
LABEL org.opencontainers.image.version=22.04
# Thu, 26 Jan 2023 05:05:43 GMT
ADD file:12d2a7ddc8445b8f97c960075216eb8e8cd226b84259c7343ef15c65a440b500 in / 
# Thu, 26 Jan 2023 05:05:43 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:860e874323ae800886f85ab5c346783e3a9371bd9beb72c5f25e8e20c9dd18bb`  
		Last Modified: Thu, 26 Jan 2023 05:14:09 GMT  
		Size: 26.1 MB (26137949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:latest` - linux; arm64 variant v8

```console
$ docker pull ubuntu@sha256:13e180ab78513dbe30a4f5a9e35acc6f61d92cbccac887a4f11ea23516261cc0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.3 MB (27342387 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a6be1f66f70f66ef43503292e38ccbfc14f2d5464e7736344783a8fc7bb339a8`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 26 Jan 2023 05:05:49 GMT
ARG RELEASE
# Thu, 26 Jan 2023 05:05:49 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 05:05:49 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 05:05:50 GMT
LABEL org.opencontainers.image.version=22.04
# Thu, 26 Jan 2023 05:05:51 GMT
ADD file:55486a91f732042dd4e81ecfd8457d23e04dcd7dd80a0bb06cc7c44873fac838 in / 
# Thu, 26 Jan 2023 05:05:51 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:8b150fd943bcd54ef788cece17523d19031f745b099a798de65247900d102e18`  
		Last Modified: Thu, 26 Jan 2023 05:14:03 GMT  
		Size: 27.3 MB (27342387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:latest` - linux; ppc64le

```console
$ docker pull ubuntu@sha256:ed40c990366092268d72da08b90fb5a0f6081ab1e00918c6453e64443d775dca
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.6 MB (34588568 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d899338973bac5fb325b647c7436507e44918374fff2a72b0da6515946c868a7`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 26 Jan 2023 04:58:24 GMT
ARG RELEASE
# Thu, 26 Jan 2023 04:58:24 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 04:58:24 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 04:58:24 GMT
LABEL org.opencontainers.image.version=22.04
# Thu, 26 Jan 2023 04:58:28 GMT
ADD file:f0400001a50847feb579e66e804ec9daaaaeb9a414b4b5cca8bb0c8e9c7fa8f9 in / 
# Thu, 26 Jan 2023 04:58:28 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:717e115780fa5a198871a9eef15e446084728bf7021e7894e6118f3cd6d26b60`  
		Last Modified: Thu, 26 Jan 2023 05:14:15 GMT  
		Size: 34.6 MB (34588568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:latest` - linux; s390x

```console
$ docker pull ubuntu@sha256:d3df0130c5dc92778c7513686bb9f10d5e2e710b7f290d686bda24ac351d3220
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.0 MB (28009396 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6abbed079020c533dbc7ca626067d743bf7effce2e4c895f104846afd8f4943a`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 26 Jan 2023 05:08:35 GMT
ARG RELEASE
# Thu, 26 Jan 2023 05:08:35 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 05:08:36 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 05:08:36 GMT
LABEL org.opencontainers.image.version=22.04
# Thu, 26 Jan 2023 05:08:37 GMT
ADD file:a9794efc1a102ab6a7160e660a63f4b267797b8b7e0b0bfd9c04ed62846cfb36 in / 
# Thu, 26 Jan 2023 05:08:38 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:f8e318d098424cef87513f4c834987f20c608791646c6b1a3ef60ed57408ddb6`  
		Last Modified: Thu, 26 Jan 2023 05:14:22 GMT  
		Size: 28.0 MB (28009396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ubuntu:lunar`

```console
$ docker pull ubuntu@sha256:e2e6dfaf4d892b0430e636f2747c3a19d47a806a1fc21810743c113ca59ab6a2
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `ubuntu:lunar` - linux; amd64

```console
$ docker pull ubuntu@sha256:76f55c747c6e3cc7a49f6bade839a8fbca72e0338fec92b54e58b8d15baf836d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.6 MB (26594295 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:096628db4ff280b69ee9eaca21f0cfc152776e1243bc6c1320b436934188d5e5`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 25 Jan 2023 14:47:05 GMT
ARG RELEASE
# Wed, 25 Jan 2023 14:47:05 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 25 Jan 2023 14:47:05 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 25 Jan 2023 14:47:05 GMT
LABEL org.opencontainers.image.version=23.04
# Wed, 25 Jan 2023 14:47:07 GMT
ADD file:5a9904395b52775ee7c10a49efc741d32b587e2cd447b8deb66811c3fb3b37a4 in / 
# Wed, 25 Jan 2023 14:47:07 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:85cec64d15ef8b1eb3ff65555dbe92d7e3ea2a21f3e1fe1206ed85e221b3593d`  
		Last Modified: Wed, 25 Jan 2023 14:56:49 GMT  
		Size: 26.6 MB (26594295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:lunar` - linux; arm variant v7

```console
$ docker pull ubuntu@sha256:1d8b24f64674c975ae2ca8b10f39a8c79cca25e278d9fe6438bddef61307e3f1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.1 MB (25095764 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9f55f15212572f043ec357086e290a82ab554094f4f7f044746ff6dec8d96428`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 25 Jan 2023 14:38:25 GMT
ARG RELEASE
# Wed, 25 Jan 2023 14:38:25 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 25 Jan 2023 14:38:26 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 25 Jan 2023 14:38:26 GMT
LABEL org.opencontainers.image.version=23.04
# Wed, 25 Jan 2023 14:38:35 GMT
ADD file:c01025be735c65553980246358cbe7c563769d7ffc886d18be817582a0d29b5c in / 
# Wed, 25 Jan 2023 14:38:36 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:f9e87c970a05364b1b6a0c18043b8cc663c1dcd5b370d87043288950fabb675a`  
		Last Modified: Wed, 25 Jan 2023 14:57:02 GMT  
		Size: 25.1 MB (25095764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:lunar` - linux; arm64 variant v8

```console
$ docker pull ubuntu@sha256:601b47b473ab776a59e725ab6bde002ed7b271b9531dc72d602c033b0c578879
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.8 MB (25777338 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:39efbc92de18d58fc90c5503a1f69c3dccce7e29830cc6560ec6857f8b6485e5`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 25 Jan 2023 14:42:22 GMT
ARG RELEASE
# Wed, 25 Jan 2023 14:42:23 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 25 Jan 2023 14:42:23 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 25 Jan 2023 14:42:23 GMT
LABEL org.opencontainers.image.version=23.04
# Wed, 25 Jan 2023 14:42:31 GMT
ADD file:6713306ff9bcc18c79430d43aafbbe519176e76b7232c563993ebda6c8caf738 in / 
# Wed, 25 Jan 2023 14:42:32 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:ce743a0a7eb81f2756829eb9afb29c85ce40ded304387cdd06f66b01793ac464`  
		Last Modified: Wed, 25 Jan 2023 14:56:55 GMT  
		Size: 25.8 MB (25777338 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:lunar` - linux; ppc64le

```console
$ docker pull ubuntu@sha256:67fe8ea65e1c908351ee7dbc6cf56660fc0d3ef49b8046aeb61e3df7fbd5172d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.0 MB (30959485 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c420642d8d83f69bc1f4eba5096256ff91343014b4d8dbdfcead8b96635f6c11`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 25 Jan 2023 14:48:03 GMT
ARG RELEASE
# Wed, 25 Jan 2023 14:48:03 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 25 Jan 2023 14:48:03 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 25 Jan 2023 14:48:04 GMT
LABEL org.opencontainers.image.version=23.04
# Wed, 25 Jan 2023 14:48:07 GMT
ADD file:5002466754dcd29080099171ab20675c9bcc55f0befbe928008127d14c027297 in / 
# Wed, 25 Jan 2023 14:48:07 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:8215a53a3d6e58238feac2e65d9c57d1f382d8ade421475347b3c522198afe4e`  
		Last Modified: Wed, 25 Jan 2023 14:57:08 GMT  
		Size: 31.0 MB (30959485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:lunar` - linux; s390x

```console
$ docker pull ubuntu@sha256:87dc7c1f1d0b9cdb25c2e1cfdcd05569ab54f7949365a8aa8677d6098f57273d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.5 MB (25455083 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2a5869fd440bbbebdfc74dcec9c949501d695f868ff73d63165a920e39d8bfca`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 25 Jan 2023 14:49:06 GMT
ARG RELEASE
# Wed, 25 Jan 2023 14:49:06 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 25 Jan 2023 14:49:06 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 25 Jan 2023 14:49:06 GMT
LABEL org.opencontainers.image.version=23.04
# Wed, 25 Jan 2023 14:49:08 GMT
ADD file:81c93bf9ec11b910a5bae8b977a82a78cb327c7bf9d0991542c9b6847cf19210 in / 
# Wed, 25 Jan 2023 14:49:12 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:f6119d8ec48acf1c2965d2233f93e21ee590564bbae9fd360b9630c3b6c694f9`  
		Last Modified: Wed, 25 Jan 2023 14:57:22 GMT  
		Size: 25.5 MB (25455083 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ubuntu:lunar-20230124.1`

```console
$ docker pull ubuntu@sha256:e2e6dfaf4d892b0430e636f2747c3a19d47a806a1fc21810743c113ca59ab6a2
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `ubuntu:lunar-20230124.1` - linux; amd64

```console
$ docker pull ubuntu@sha256:76f55c747c6e3cc7a49f6bade839a8fbca72e0338fec92b54e58b8d15baf836d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.6 MB (26594295 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:096628db4ff280b69ee9eaca21f0cfc152776e1243bc6c1320b436934188d5e5`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 25 Jan 2023 14:47:05 GMT
ARG RELEASE
# Wed, 25 Jan 2023 14:47:05 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 25 Jan 2023 14:47:05 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 25 Jan 2023 14:47:05 GMT
LABEL org.opencontainers.image.version=23.04
# Wed, 25 Jan 2023 14:47:07 GMT
ADD file:5a9904395b52775ee7c10a49efc741d32b587e2cd447b8deb66811c3fb3b37a4 in / 
# Wed, 25 Jan 2023 14:47:07 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:85cec64d15ef8b1eb3ff65555dbe92d7e3ea2a21f3e1fe1206ed85e221b3593d`  
		Last Modified: Wed, 25 Jan 2023 14:56:49 GMT  
		Size: 26.6 MB (26594295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:lunar-20230124.1` - linux; arm variant v7

```console
$ docker pull ubuntu@sha256:1d8b24f64674c975ae2ca8b10f39a8c79cca25e278d9fe6438bddef61307e3f1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.1 MB (25095764 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9f55f15212572f043ec357086e290a82ab554094f4f7f044746ff6dec8d96428`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 25 Jan 2023 14:38:25 GMT
ARG RELEASE
# Wed, 25 Jan 2023 14:38:25 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 25 Jan 2023 14:38:26 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 25 Jan 2023 14:38:26 GMT
LABEL org.opencontainers.image.version=23.04
# Wed, 25 Jan 2023 14:38:35 GMT
ADD file:c01025be735c65553980246358cbe7c563769d7ffc886d18be817582a0d29b5c in / 
# Wed, 25 Jan 2023 14:38:36 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:f9e87c970a05364b1b6a0c18043b8cc663c1dcd5b370d87043288950fabb675a`  
		Last Modified: Wed, 25 Jan 2023 14:57:02 GMT  
		Size: 25.1 MB (25095764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:lunar-20230124.1` - linux; arm64 variant v8

```console
$ docker pull ubuntu@sha256:601b47b473ab776a59e725ab6bde002ed7b271b9531dc72d602c033b0c578879
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.8 MB (25777338 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:39efbc92de18d58fc90c5503a1f69c3dccce7e29830cc6560ec6857f8b6485e5`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 25 Jan 2023 14:42:22 GMT
ARG RELEASE
# Wed, 25 Jan 2023 14:42:23 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 25 Jan 2023 14:42:23 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 25 Jan 2023 14:42:23 GMT
LABEL org.opencontainers.image.version=23.04
# Wed, 25 Jan 2023 14:42:31 GMT
ADD file:6713306ff9bcc18c79430d43aafbbe519176e76b7232c563993ebda6c8caf738 in / 
# Wed, 25 Jan 2023 14:42:32 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:ce743a0a7eb81f2756829eb9afb29c85ce40ded304387cdd06f66b01793ac464`  
		Last Modified: Wed, 25 Jan 2023 14:56:55 GMT  
		Size: 25.8 MB (25777338 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:lunar-20230124.1` - linux; ppc64le

```console
$ docker pull ubuntu@sha256:67fe8ea65e1c908351ee7dbc6cf56660fc0d3ef49b8046aeb61e3df7fbd5172d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.0 MB (30959485 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c420642d8d83f69bc1f4eba5096256ff91343014b4d8dbdfcead8b96635f6c11`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 25 Jan 2023 14:48:03 GMT
ARG RELEASE
# Wed, 25 Jan 2023 14:48:03 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 25 Jan 2023 14:48:03 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 25 Jan 2023 14:48:04 GMT
LABEL org.opencontainers.image.version=23.04
# Wed, 25 Jan 2023 14:48:07 GMT
ADD file:5002466754dcd29080099171ab20675c9bcc55f0befbe928008127d14c027297 in / 
# Wed, 25 Jan 2023 14:48:07 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:8215a53a3d6e58238feac2e65d9c57d1f382d8ade421475347b3c522198afe4e`  
		Last Modified: Wed, 25 Jan 2023 14:57:08 GMT  
		Size: 31.0 MB (30959485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:lunar-20230124.1` - linux; s390x

```console
$ docker pull ubuntu@sha256:87dc7c1f1d0b9cdb25c2e1cfdcd05569ab54f7949365a8aa8677d6098f57273d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.5 MB (25455083 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2a5869fd440bbbebdfc74dcec9c949501d695f868ff73d63165a920e39d8bfca`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 25 Jan 2023 14:49:06 GMT
ARG RELEASE
# Wed, 25 Jan 2023 14:49:06 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 25 Jan 2023 14:49:06 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 25 Jan 2023 14:49:06 GMT
LABEL org.opencontainers.image.version=23.04
# Wed, 25 Jan 2023 14:49:08 GMT
ADD file:81c93bf9ec11b910a5bae8b977a82a78cb327c7bf9d0991542c9b6847cf19210 in / 
# Wed, 25 Jan 2023 14:49:12 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:f6119d8ec48acf1c2965d2233f93e21ee590564bbae9fd360b9630c3b6c694f9`  
		Last Modified: Wed, 25 Jan 2023 14:57:22 GMT  
		Size: 25.5 MB (25455083 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ubuntu:rolling`

```console
$ docker pull ubuntu@sha256:a062bfdb0c233a5a7c4758c028ef6a8f4981b78008606e23f47143ca0bfb483d
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `ubuntu:rolling` - linux; amd64

```console
$ docker pull ubuntu@sha256:ef3c777a7db8a2c49d31284cc924fc3a2f471dce44378a18d6d1fefff5a63fe5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.7 MB (26691650 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:10c2f4041af137e6b0ba5c793df3dfdf4e72a4e011ce6847f4cc0247b9bbf7f2`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 26 Jan 2023 11:51:12 GMT
ARG RELEASE
# Thu, 26 Jan 2023 11:51:12 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 11:51:12 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 11:51:13 GMT
LABEL org.opencontainers.image.version=22.10
# Thu, 26 Jan 2023 11:51:14 GMT
ADD file:e886423892b371751386c0ce7147599acb72d8fb528eaaa78092b879d9ff58ce in / 
# Thu, 26 Jan 2023 11:51:15 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:256644d5a307c3efeca6ae2854b6329a2753157868dc5548e33161b377658e6a`  
		Last Modified: Thu, 26 Jan 2023 12:14:04 GMT  
		Size: 26.7 MB (26691650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:rolling` - linux; arm variant v7

```console
$ docker pull ubuntu@sha256:a9fd5288ceabc4990263038e3ff67154088e5df217fd2eaed5ac7fce8318d84a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.1 MB (25066997 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8d643d5974c30c06b1d811877a3a8f0047c4278b1fe0801d8d812b3a17ce6c15`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 26 Jan 2023 11:52:00 GMT
ARG RELEASE
# Thu, 26 Jan 2023 11:52:00 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 11:52:00 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 11:52:00 GMT
LABEL org.opencontainers.image.version=22.10
# Thu, 26 Jan 2023 11:52:03 GMT
ADD file:d35c57b0dc2840a8b1ef40f7f6cfd826da68611f1ba37a89a382618c8612b52c in / 
# Thu, 26 Jan 2023 11:52:03 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:697d38f8dfe625e3e751c0b01ddeaaeeff6e8d6f594dd7da227aea3974a49ce1`  
		Last Modified: Thu, 26 Jan 2023 12:14:16 GMT  
		Size: 25.1 MB (25066997 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:rolling` - linux; arm64 variant v8

```console
$ docker pull ubuntu@sha256:aff210956f022245b200f8be680a99c7d93f191b2cfc8d6f770f87ef3644a080
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.8 MB (25757647 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c7096432b6a9855592152ad8009431b92d7aa40980c9c94684fcc72626bbbab9`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 26 Jan 2023 12:08:18 GMT
ARG RELEASE
# Thu, 26 Jan 2023 12:08:18 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 12:08:18 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 12:08:18 GMT
LABEL org.opencontainers.image.version=22.10
# Thu, 26 Jan 2023 12:08:20 GMT
ADD file:f61617371f6963c6be2852e2b94d04e8507feb8f77e3484c94aa8b9d0ac67f76 in / 
# Thu, 26 Jan 2023 12:08:20 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:05f69cab0b799028e03233ffa93abd2d0b426412cff70959a07a29a437447ee3`  
		Last Modified: Thu, 26 Jan 2023 12:14:10 GMT  
		Size: 25.8 MB (25757647 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:rolling` - linux; ppc64le

```console
$ docker pull ubuntu@sha256:daab817634ed004a6c564aec6ca0a0d84205d49371765eb625366344ceb7d5bd
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.1 MB (31110147 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5dfbc0b60efcd8ea2a51c157e7bc286d8de7e88ae1bf756e0d8a44ff107e21c7`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 26 Jan 2023 11:57:00 GMT
ARG RELEASE
# Thu, 26 Jan 2023 11:57:00 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 11:57:00 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 11:57:00 GMT
LABEL org.opencontainers.image.version=22.10
# Thu, 26 Jan 2023 11:57:03 GMT
ADD file:3c2bc98d283cce5149d7992233f5fe644b7239417045faf3f93750b92de5f68e in / 
# Thu, 26 Jan 2023 11:57:04 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:8da618ff876e10064f550b9dc5b51b0d0ae6939f67b56ce9a0c7fa8bb77de40f`  
		Last Modified: Thu, 26 Jan 2023 12:14:22 GMT  
		Size: 31.1 MB (31110147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ubuntu:rolling` - linux; s390x

```console
$ docker pull ubuntu@sha256:944066fb6be279b0de11cb4ecc57c81794b912ba6f95a544f3d462ceab3a78a6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.5 MB (25487159 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:91297aceb6d3e297e45ec91916dbea079b90ae1c7edbaf14a99c41d3f493f537`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 26 Jan 2023 12:08:47 GMT
ARG RELEASE
# Thu, 26 Jan 2023 12:08:47 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 12:08:48 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 12:08:48 GMT
LABEL org.opencontainers.image.version=22.10
# Thu, 26 Jan 2023 12:08:50 GMT
ADD file:a83afd93816f868be76d243df85b87a66b39d5ef0497c3cb8d0bba2bd4a27c40 in / 
# Thu, 26 Jan 2023 12:08:50 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:fe4914a812d394969d56f220e5ddb037a62164607a937ca866bf4ee592a8799a`  
		Last Modified: Thu, 26 Jan 2023 12:14:28 GMT  
		Size: 25.5 MB (25487159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
