<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `ubuntu`

-	[`ubuntu:18.04`](#ubuntu1804)
-	[`ubuntu:20.04`](#ubuntu2004)
-	[`ubuntu:22.04`](#ubuntu2204)
-	[`ubuntu:22.10`](#ubuntu2210)
-	[`ubuntu:23.04`](#ubuntu2304)
-	[`ubuntu:bionic`](#ubuntubionic)
-	[`ubuntu:bionic-20230308`](#ubuntubionic-20230308)
-	[`ubuntu:devel`](#ubuntudevel)
-	[`ubuntu:focal`](#ubuntufocal)
-	[`ubuntu:focal-20230308`](#ubuntufocal-20230308)
-	[`ubuntu:jammy`](#ubuntujammy)
-	[`ubuntu:jammy-20230308`](#ubuntujammy-20230308)
-	[`ubuntu:kinetic`](#ubuntukinetic)
-	[`ubuntu:kinetic-20230308`](#ubuntukinetic-20230308)
-	[`ubuntu:latest`](#ubuntulatest)
-	[`ubuntu:lunar`](#ubuntulunar)
-	[`ubuntu:lunar-20230314`](#ubuntulunar-20230314)
-	[`ubuntu:rolling`](#ubunturolling)

## `ubuntu:18.04`

```console
$ docker pull ubuntu@sha256:8aa9c2798215f99544d1ce7439ea9c3a6dfd82de607da1cec3a8a2fae005931b
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
$ docker pull ubuntu@sha256:0779371f96205678dbcaa3ef499be2e5f262c8b09aadc11754bf3daf9f35e03e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.7 MB (25688211 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3941d3b032a8168d53508410a67baad120a563df67a7959565a30a1cb2114731`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 08 Mar 2023 03:22:42 GMT
ARG RELEASE
# Wed, 08 Mar 2023 03:22:42 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 03:22:42 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 03:22:42 GMT
LABEL org.opencontainers.image.version=18.04
# Wed, 08 Mar 2023 03:22:44 GMT
ADD file:4560926e076acae6b8396a9f1e760eee0f53e22e90ce8554dda57f1103547795 in / 
# Wed, 08 Mar 2023 03:22:44 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:0c5227665c11379f79e9da3d3e4f1724f9316b87d259ac0131628ca1b923a392`  
		Last Modified: Wed, 08 Mar 2023 03:59:25 GMT  
		Size: 25.7 MB (25688211 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:18.04` - linux; arm variant v7

```console
$ docker pull ubuntu@sha256:715ddeafc950876ef9451c460d43ac1ba3e90655f582d845c7f656ee557bd2b2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **21.4 MB (21394593 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c0feaeaa2e651a8712ecfc0727458ba88952949b4b9136d20f0e7adb6a743c1f`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 08 Mar 2023 03:27:01 GMT
ARG RELEASE
# Wed, 08 Mar 2023 03:27:01 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 03:27:01 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 03:27:01 GMT
LABEL org.opencontainers.image.version=18.04
# Wed, 08 Mar 2023 03:27:08 GMT
ADD file:21d7947367fe1aa8cc668c943d11c4841b0ead14b9103ef46fb8db8084603a75 in / 
# Wed, 08 Mar 2023 03:27:09 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:55e299352d1e9c6f1d6e7aee23f9204c8e147eec9fb877be5649ad7f1af58bca`  
		Last Modified: Wed, 08 Mar 2023 03:59:37 GMT  
		Size: 21.4 MB (21394593 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:18.04` - linux; arm64 variant v8

```console
$ docker pull ubuntu@sha256:e77e90f3a41b2c9480c68088c746065623ba9ca77f4e311070ebf404ac6ef2dd
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **22.7 MB (22710750 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c1adc1968c7b7646687f8585de8e3473681323cb9052956ed8f509529a52e61d`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 08 Mar 2023 03:25:33 GMT
ARG RELEASE
# Wed, 08 Mar 2023 03:25:33 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 03:25:34 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 03:25:34 GMT
LABEL org.opencontainers.image.version=18.04
# Wed, 08 Mar 2023 03:25:35 GMT
ADD file:5f229d85bac2e85aa7ce97b2168fc61bd401d0151e8940a12d244356f984e65f in / 
# Wed, 08 Mar 2023 03:25:35 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:13f679bb266a0be5756ce3bb145f89ccd6395d778b1a4bed5a0b0b26105bde2b`  
		Last Modified: Wed, 08 Mar 2023 03:59:31 GMT  
		Size: 22.7 MB (22710750 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:18.04` - linux; 386

```console
$ docker pull ubuntu@sha256:7cbc4fafddce3cf793a94c3b5dc6295a3f569b9222c5e4e74b38aa00a65442fb
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.1 MB (26095131 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d713953b7d565f057a079026363b57bd30e4e9fef8aeaf217f6c4c8b20d968f1`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 08 Mar 2023 03:13:19 GMT
ARG RELEASE
# Wed, 08 Mar 2023 03:13:19 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 03:13:19 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 03:13:19 GMT
LABEL org.opencontainers.image.version=18.04
# Wed, 08 Mar 2023 03:13:21 GMT
ADD file:6cf3e34995c6c44762ed692b86a0442d981e9a69fa4288960047e505d75c0223 in / 
# Wed, 08 Mar 2023 03:13:22 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:472741f7e602c0ee1b34eaf14bb55e0a9377b9f28b0b00fd7ddb5b9d07046a7d`  
		Last Modified: Wed, 08 Mar 2023 03:59:42 GMT  
		Size: 26.1 MB (26095131 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:18.04` - linux; ppc64le

```console
$ docker pull ubuntu@sha256:c955620556f7490d6c4cbd7c1d73faeaad2f635cc3207ee8278832c897d1a7e2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.4 MB (29350183 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:342b45b2835cf4d380d116f2d5e52053a8335089236b194c117adf34efac0409`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 08 Mar 2023 03:13:23 GMT
ARG RELEASE
# Wed, 08 Mar 2023 03:13:23 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 03:13:23 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 03:13:23 GMT
LABEL org.opencontainers.image.version=18.04
# Wed, 08 Mar 2023 03:13:26 GMT
ADD file:5ea8615c09f693252cb9d45458421679f82f84d315200a7611165869195b3a69 in / 
# Wed, 08 Mar 2023 03:13:26 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:293f1b6b3486ffa5f90fdcf0f22fc2091718a3e012fadf073bf57b6a8604df20`  
		Last Modified: Wed, 08 Mar 2023 03:59:48 GMT  
		Size: 29.4 MB (29350183 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:18.04` - linux; s390x

```console
$ docker pull ubuntu@sha256:1e8deff80e7d247c13e32a88efe3ca7314c2e8eb6ab5224e1a7671d7d8076428
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **24.7 MB (24743830 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4ed683baf1b6cc5ec9754e58ee88c3414d4781d2b27d33dc89e16d191249bd0f`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 08 Mar 2023 03:23:29 GMT
ARG RELEASE
# Wed, 08 Mar 2023 03:23:29 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 03:23:29 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 03:23:29 GMT
LABEL org.opencontainers.image.version=18.04
# Wed, 08 Mar 2023 03:23:31 GMT
ADD file:a6309e462d28398152cb726a11615118d79858da963b8c614772b87d87465967 in / 
# Wed, 08 Mar 2023 03:23:31 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:ff61d052565af59dfea677d587c19bf7759efb08fa5db9c11019e2b30b183d9b`  
		Last Modified: Wed, 08 Mar 2023 03:59:54 GMT  
		Size: 24.7 MB (24743830 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

## `ubuntu:20.04`

```console
$ docker pull ubuntu@sha256:24a0df437301598d1a4b62ddf59fa0ed2969150d70d748c84225e6501e9c36b9
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
$ docker pull ubuntu@sha256:b39db7fc56971aac21dee02187e898db759c4f26b9b27b1d80b6ad32ff330c76
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.5 MB (27503825 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1c5c8d0b973ab9d6d7742cf050beefa8ba2efb7779e09bfb1200d6192180766e`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 08 Mar 2023 04:41:24 GMT
ARG RELEASE
# Wed, 08 Mar 2023 04:41:24 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 04:41:24 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 04:41:24 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 08 Mar 2023 04:41:26 GMT
ADD file:20f2ff22b9a8ca9bec5178036c9ebc525a12cd4312daf5d14a9a631a30be20e1 in / 
# Wed, 08 Mar 2023 04:41:27 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:06d39c85623a79eb68b6cac39f4c4aba8834873ee5fc27be9d9d7655e6313c26`  
		Last Modified: Wed, 08 Mar 2023 05:10:29 GMT  
		Size: 27.5 MB (27503825 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:20.04` - linux; arm variant v7

```console
$ docker pull ubuntu@sha256:223d6beaf1aa0978b7a0dc4731333b59fe35ee9d3a8c48db1a8d686b1b211ea0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.6 MB (23608664 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4731390bddee2b1dc9fa35d820d20b69f95bb16381ae1434821f52eb87f9d503`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 08 Mar 2023 04:31:43 GMT
ARG RELEASE
# Wed, 08 Mar 2023 04:31:43 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 04:31:43 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 04:31:43 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 08 Mar 2023 04:31:46 GMT
ADD file:99d501af7a191308f8fe3dc3f33c63bd8b54fb749d061b1a901c423b85f8cec2 in / 
# Wed, 08 Mar 2023 04:31:46 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:3503cc1332f3fe649c8a0937dbf6f052f1d2d9b9bdb97546cf15f09ec495d7a4`  
		Last Modified: Wed, 08 Mar 2023 05:10:41 GMT  
		Size: 23.6 MB (23608664 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:20.04` - linux; arm64 variant v8

```console
$ docker pull ubuntu@sha256:f92b9de5f10b6e1fcda653f5d02bd6c816386dfb830c71cef95df52b2280cd1c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.0 MB (25973169 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:625d192afcdc5add2f097cd05a177ab19f18e69473911dbb479fc5eba56ba8fd`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 08 Mar 2023 04:34:20 GMT
ARG RELEASE
# Wed, 08 Mar 2023 04:34:20 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 04:34:20 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 04:34:20 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 08 Mar 2023 04:34:24 GMT
ADD file:e73d5d005a3ba2c2fb3d8585a1f19daf5ea9ed75af5a2f97b1cc6f7f03db0cdc in / 
# Wed, 08 Mar 2023 04:34:24 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:a774dfcdedc7c7c4f0009ddadc2f33557d60452450684534df5625f9693df81a`  
		Last Modified: Wed, 08 Mar 2023 05:10:35 GMT  
		Size: 26.0 MB (25973169 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:20.04` - linux; ppc64le

```console
$ docker pull ubuntu@sha256:36b2d0b2c6aeee6945261da06ed2a0f8be5548bc5f974e3ffd224baa77e585b2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.1 MB (32068376 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7e49f046bd37833635fbd8d90722b7b57c00811d3ccf7ed7d78e796f669fbcbf`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 08 Mar 2023 04:39:14 GMT
ARG RELEASE
# Wed, 08 Mar 2023 04:39:14 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 04:39:14 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 04:39:14 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 08 Mar 2023 04:39:17 GMT
ADD file:e8eae0af07e662df38a5b691d04648b4fc72382b6918877da22520ed4d01c3a6 in / 
# Wed, 08 Mar 2023 04:39:17 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:231de8dd1e233ca65e29bae666ffef95bfca99c9ca8decd4bb6cd73269924f31`  
		Last Modified: Wed, 08 Mar 2023 05:10:47 GMT  
		Size: 32.1 MB (32068376 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:20.04` - linux; s390x

```console
$ docker pull ubuntu@sha256:ee77c5eb098846cf57a751c5b4d28678f152ebd936ee700570f77e5181f94749
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.4 MB (26364051 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0ae7691e3a999c7848a0952ef29ffbb1c235587dfce87cba0df7e8d23a8b0be6`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 08 Mar 2023 04:41:58 GMT
ARG RELEASE
# Wed, 08 Mar 2023 04:41:58 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 04:41:58 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 04:41:58 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 08 Mar 2023 04:42:00 GMT
ADD file:4463dafd3352de8c5ff87090e2f30be9bdffc3fa9d84e27b13e2364d856f82e9 in / 
# Wed, 08 Mar 2023 04:42:00 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:68e65db8d2065c8b6d0764029cabc60b7c7bfd9dc8fb638e0effa6e544486597`  
		Last Modified: Wed, 08 Mar 2023 05:10:53 GMT  
		Size: 26.4 MB (26364051 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

## `ubuntu:22.04`

```console
$ docker pull ubuntu@sha256:67211c14fa74f070d27cc59d69a7fa9aeff8e28ea118ef3babc295a0428a6d21
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
$ docker pull ubuntu@sha256:7a57c69fe1e9d5b97c5fe649849e79f2cfc3bf11d10bbd5218b4eb61716aebe6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.5 MB (29533950 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:08d22c0ceb150ddeb2237c5fa3129c0183f3cc6f5eeb2e7aa4016da3ad02140a`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 08 Mar 2023 04:44:25 GMT
ARG RELEASE
# Wed, 08 Mar 2023 04:44:25 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 04:44:25 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 04:44:25 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 08 Mar 2023 04:44:27 GMT
ADD file:c8ef6447752cab2541ffca9e3cfa27d581f3491bc8f356f6eafd951243609341 in / 
# Wed, 08 Mar 2023 04:44:27 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:2ab09b027e7f3a0c2e8bb1944ac46de38cebab7145f0bd6effebfe5492c818b6`  
		Last Modified: Wed, 08 Mar 2023 05:10:20 GMT  
		Size: 29.5 MB (29533950 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:22.04` - linux; arm variant v7

```console
$ docker pull ubuntu@sha256:ad18cfdb19dac67bf0072dacea661a817330e5c955d081f4d09914e743ae5d4a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.1 MB (26140319 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2bf0095935ffb29018664cf219d8c1b2c890e3e3c4af89113df23e7330397187`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 08 Mar 2023 04:31:38 GMT
ARG RELEASE
# Wed, 08 Mar 2023 04:31:38 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 04:31:39 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 04:31:39 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 08 Mar 2023 04:31:41 GMT
ADD file:e9c3ac290fb81ae2e78de99052d776396ee3aff05e1a66fd2dccb01d7de9bb45 in / 
# Wed, 08 Mar 2023 04:31:42 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:aea1895b7fd03ef3bc263eef4b6f1dd219fc3286f3ff79495aadb81a88650723`  
		Last Modified: Wed, 08 Mar 2023 05:10:33 GMT  
		Size: 26.1 MB (26140319 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:22.04` - linux; arm64 variant v8

```console
$ docker pull ubuntu@sha256:537da24818633b45fcb65e5285a68c3ec1f3db25f5ae5476a7757bc8dfae92a3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.3 MB (27347481 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bab8ce5c00ca3ef91e0d3eb4c6e6d6ec7cffa9574c447fd8d54a8d96e7c1c80e`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 08 Mar 2023 04:32:38 GMT
ARG RELEASE
# Wed, 08 Mar 2023 04:32:38 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 04:32:38 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 04:32:39 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 08 Mar 2023 04:32:40 GMT
ADD file:79b36308bc382d9cae7197b4cecc21430f4e8f3e8bec3547d0f00bcff7681e60 in / 
# Wed, 08 Mar 2023 04:32:41 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:cd741b12a7eaa64357041c2d3f4590c898313a7f8f65cd1577594e6ee03a8c38`  
		Last Modified: Wed, 08 Mar 2023 05:10:27 GMT  
		Size: 27.3 MB (27347481 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:22.04` - linux; ppc64le

```console
$ docker pull ubuntu@sha256:f23b7ade9f88f91c8d5932a48b721712ed509a607d9a05cdeae4cd06de09e5f7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.6 MB (34593661 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4220c61b3ab7b82dd3ff3395f9efe2b63e730c3f24284d1519013cf3cda822f8`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 08 Mar 2023 04:39:16 GMT
ARG RELEASE
# Wed, 08 Mar 2023 04:39:16 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 04:39:16 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 04:39:16 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 08 Mar 2023 04:39:20 GMT
ADD file:d7434a52d8d8aa6288e788f6fe7e156f0e11bf9b8275efaf70aab0bfc4d919cf in / 
# Wed, 08 Mar 2023 04:39:20 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:2561b3b559ec9b25bafa07804afa433803291265f7dd847de711224b0f238237`  
		Last Modified: Wed, 08 Mar 2023 05:10:39 GMT  
		Size: 34.6 MB (34593661 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:22.04` - linux; s390x

```console
$ docker pull ubuntu@sha256:b351315d950a4da70f19d62f4da5dd7f9a445eb8c8d6851a5b6cdddbdafb13cf
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.0 MB (28015959 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:63ad39053efde0c294433cd8f9709c6d69a36e1f0af4ffbf81c3d261caffb615`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 08 Mar 2023 04:39:24 GMT
ARG RELEASE
# Wed, 08 Mar 2023 04:39:24 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 04:39:24 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 04:39:24 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 08 Mar 2023 04:39:26 GMT
ADD file:630f9865d3d4fd4294d45cac7cbaea83fb549c2e563de454348da964d19fbbba in / 
# Wed, 08 Mar 2023 04:39:26 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:15f635e04e894b7646b4ebca40424ddf244867fc663429ea8b877eca172a7cf1`  
		Last Modified: Wed, 08 Mar 2023 05:10:46 GMT  
		Size: 28.0 MB (28015959 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

## `ubuntu:22.10`

```console
$ docker pull ubuntu@sha256:a82eebb42083a134e009a6b81a7e5d2eecc37112fa8ae40642bd3c5153b7e4f0
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
$ docker pull ubuntu@sha256:8c8f22bacbfba9678edddcc3b6d1e56cce02eff9cbf27ab46116de30cb79a3d6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.7 MB (26695001 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:558d44db75c8f69c29f427cf88e6a71c39320f7607584baa6860f6e4f6121892`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 08 Mar 2023 05:58:05 GMT
ARG RELEASE
# Wed, 08 Mar 2023 05:58:05 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 05:58:05 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 05:58:05 GMT
LABEL org.opencontainers.image.version=22.10
# Wed, 08 Mar 2023 05:58:07 GMT
ADD file:3492508b382c909e968c4d8467b9acbd5f61ed6ca69c8a47241f930d90de7158 in / 
# Wed, 08 Mar 2023 05:58:07 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:5c19388d38e1ea904672812dd0aac505220c9254e2621a1684e0fe29e2dba80e`  
		Last Modified: Wed, 08 Mar 2023 06:38:37 GMT  
		Size: 26.7 MB (26695001 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:22.10` - linux; arm variant v7

```console
$ docker pull ubuntu@sha256:e37c01607a81ee7737f164af67cb5f5f8e1ecbf82c4f5cfe940675b8e8830ee1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.1 MB (25067205 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:94bcbf2021edfcf5671a4872ded2d62d36cd3a86813acc7bc2471fefce3c2ac2`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 08 Mar 2023 05:55:43 GMT
ARG RELEASE
# Wed, 08 Mar 2023 05:55:43 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 05:55:43 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 05:55:43 GMT
LABEL org.opencontainers.image.version=22.10
# Wed, 08 Mar 2023 05:55:49 GMT
ADD file:827330b6c59e67c5d2edd3ceb3492b97865b15f9246f14710f478d12e94d2048 in / 
# Wed, 08 Mar 2023 05:55:49 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:5c09adf37dd1d92aeedd2906b2635d9b7f1eca9f39f51d52f919d26d113c8d35`  
		Last Modified: Wed, 08 Mar 2023 06:38:49 GMT  
		Size: 25.1 MB (25067205 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:22.10` - linux; arm64 variant v8

```console
$ docker pull ubuntu@sha256:2a79f91eb2bb4ffc5d96c58a06fda63550bf94a1a6b2e9ef2f835e52ca8a04ee
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.8 MB (25760037 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:438c48db988d0f48de4461bb2bf49524880c28c5863b1ba5b175a9d7c284b009`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 08 Mar 2023 05:57:57 GMT
ARG RELEASE
# Wed, 08 Mar 2023 05:57:57 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 05:57:57 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 05:57:58 GMT
LABEL org.opencontainers.image.version=22.10
# Wed, 08 Mar 2023 05:57:59 GMT
ADD file:884e00dc91bf6d392fa3d117913cc2534177128322d89137bfb8b2734bc38579 in / 
# Wed, 08 Mar 2023 05:58:00 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:4f720bb411d1d3a6b6c043988c66cdaeee655f968c6eabf7f1ada7ac1529b046`  
		Last Modified: Wed, 08 Mar 2023 06:38:43 GMT  
		Size: 25.8 MB (25760037 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:22.10` - linux; ppc64le

```console
$ docker pull ubuntu@sha256:fec18179ce4b8f8215f04ea75ca752d4c7865d1a06f1d9a3d961927ed2916589
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.1 MB (31114002 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:817a0842655ee55d34c1866729026d8d7fd4de6cc4ea4fcbdaac3cbc1dc10a73`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 08 Mar 2023 05:58:03 GMT
ARG RELEASE
# Wed, 08 Mar 2023 05:58:03 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 05:58:03 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 05:58:03 GMT
LABEL org.opencontainers.image.version=22.10
# Wed, 08 Mar 2023 05:58:06 GMT
ADD file:583061e8201c03de4747860e734200b6c35b449443a1382ad8e8efc6f7e9ea13 in / 
# Wed, 08 Mar 2023 05:58:06 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:e9acd60127e6a1f919659d03fc820b762a3f49f62bae6caafbd919cdbd8e4f7b`  
		Last Modified: Wed, 08 Mar 2023 06:38:55 GMT  
		Size: 31.1 MB (31114002 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:22.10` - linux; s390x

```console
$ docker pull ubuntu@sha256:c69324f895a9152b8a80f9d310710a9d2ef987330d04bc20dbfe23e79e5183bb
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.5 MB (25488878 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4997349fe1813d9306e1ad38084ecc78950e221fe4f75cd9a85e5213139fcd80`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 08 Mar 2023 06:11:04 GMT
ARG RELEASE
# Wed, 08 Mar 2023 06:11:04 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 06:11:04 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 06:11:04 GMT
LABEL org.opencontainers.image.version=22.10
# Wed, 08 Mar 2023 06:11:06 GMT
ADD file:974d67ca1d5bcaacbc707820609d36af0d7ed3ff7179a702a4aa56dcc43f79f3 in / 
# Wed, 08 Mar 2023 06:11:06 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:e7f1a81217015da9b8db635ad002e08952988dc4100cbec474290e8524391920`  
		Last Modified: Wed, 08 Mar 2023 06:39:01 GMT  
		Size: 25.5 MB (25488878 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

## `ubuntu:23.04`

```console
$ docker pull ubuntu@sha256:008c0f6712067722f42f9685476d37b0b7b689e31d66e5787d1920c7ac230849
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
$ docker pull ubuntu@sha256:ffa4bb610fa4c137211199607a5326c5a409b189d3c673cc85a4c65f5757447b
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.8 MB (26761270 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:de432ed6bff895b418712abd3084394e7dd70656b905d6390ffba649c63c64a3`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 14 Mar 2023 18:21:45 GMT
ARG RELEASE
# Tue, 14 Mar 2023 18:21:45 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 14 Mar 2023 18:21:45 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 14 Mar 2023 18:21:45 GMT
LABEL org.opencontainers.image.version=23.04
# Tue, 14 Mar 2023 18:21:47 GMT
ADD file:108000e07d9734743bfe65381248aa7e309283bdb87d8687b7ffe0d697487109 in / 
# Tue, 14 Mar 2023 18:21:47 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:391f30eda8cdf14ab4acf7e6ce5bac054bcc1d98fe5f8789908c6bc739dee216`  
		Last Modified: Tue, 14 Mar 2023 18:47:00 GMT  
		Size: 26.8 MB (26761270 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:23.04` - linux; arm variant v7

```console
$ docker pull ubuntu@sha256:e685540e6030c9b728fa6485ca8e844d824e064c9a790bc54e6e6507974ba42e
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **24.6 MB (24559160 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:28e4ad84aaa1e06e217b7ed880b9bea183f12a02bb5b8408f57855354fbd91c9`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 14 Mar 2023 18:18:28 GMT
ARG RELEASE
# Tue, 14 Mar 2023 18:18:28 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 14 Mar 2023 18:18:28 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 14 Mar 2023 18:18:28 GMT
LABEL org.opencontainers.image.version=23.04
# Tue, 14 Mar 2023 18:18:30 GMT
ADD file:dc39df38ee577fc1ddb753815787f9a90231d34a28c65e14298d136132c8d7d5 in / 
# Tue, 14 Mar 2023 18:18:31 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:7ec8b1962079f6d8d8477e2e227966fcf2e91d26a81735eb5f0411f84cbf8740`  
		Last Modified: Tue, 14 Mar 2023 18:47:12 GMT  
		Size: 24.6 MB (24559160 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:23.04` - linux; arm64 variant v8

```console
$ docker pull ubuntu@sha256:b864a1f0e9f2686fcaa86491f78d38af1b9e8e53e965df39d991a8b685bf7c74
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.0 MB (26007489 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e399e758a4b24fbecd3eed7dbaadf0eb3aa45f2ee4b2c133561693f31008b42b`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 14 Mar 2023 17:38:32 GMT
ARG RELEASE
# Tue, 14 Mar 2023 17:38:32 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 14 Mar 2023 17:38:32 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 14 Mar 2023 17:38:32 GMT
LABEL org.opencontainers.image.version=23.04
# Tue, 14 Mar 2023 17:38:40 GMT
ADD file:2562122b72f2bcdd0678a1bd0836dcbf376a8e33078452497d85ed0cd425391f in / 
# Tue, 14 Mar 2023 17:38:41 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:ff6383e8c55f097496fc03e31f40ad77007ac50d51f9735a1d45789985087387`  
		Last Modified: Tue, 14 Mar 2023 18:47:06 GMT  
		Size: 26.0 MB (26007489 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:23.04` - linux; ppc64le

```console
$ docker pull ubuntu@sha256:8e0b2dedffe81c417dc0860a92ec8520aca6f48b6b3267b18590c1ff4c4f16ea
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.0 MB (30987169 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:26160bb786e079c716ceda59a2a70b6e813f9e43dea7866e98e9edfe8a1cb84f`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 14 Mar 2023 17:31:48 GMT
ARG RELEASE
# Tue, 14 Mar 2023 17:31:48 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 14 Mar 2023 17:31:48 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 14 Mar 2023 17:31:48 GMT
LABEL org.opencontainers.image.version=23.04
# Tue, 14 Mar 2023 17:31:51 GMT
ADD file:586ae3783043b40d20c362128778cbf64404358967d540af0c899067d82744f8 in / 
# Tue, 14 Mar 2023 17:31:52 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:59dbd023a22a72c486e06919c527e79036e5a5b41ca794aafbbd35687256dee7`  
		Last Modified: Tue, 14 Mar 2023 18:47:20 GMT  
		Size: 31.0 MB (30987169 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:23.04` - linux; s390x

```console
$ docker pull ubuntu@sha256:1840997cef13af4d355cf1b5bda18e68073cc6aefe673bd36cb93ea91f3452a2
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.6 MB (25634517 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6d6744e3a8d8d30ea66143d1d2ba080a6cb9a9e1356857de142edfd33ddefb5e`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 14 Mar 2023 17:47:18 GMT
ARG RELEASE
# Tue, 14 Mar 2023 17:47:18 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 14 Mar 2023 17:47:18 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 14 Mar 2023 17:47:18 GMT
LABEL org.opencontainers.image.version=23.04
# Tue, 14 Mar 2023 17:47:20 GMT
ADD file:1ed4a1aa279c8c4fd49f73ed214f53835caecef222778b80716ba71fe60cc7f0 in / 
# Tue, 14 Mar 2023 17:47:20 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:de8d2f62d0190fb3786c431d236f8d6178a12304755c3c13b8c1ff4d6097587f`  
		Last Modified: Tue, 14 Mar 2023 18:47:26 GMT  
		Size: 25.6 MB (25634517 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

## `ubuntu:bionic`

```console
$ docker pull ubuntu@sha256:8aa9c2798215f99544d1ce7439ea9c3a6dfd82de607da1cec3a8a2fae005931b
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
$ docker pull ubuntu@sha256:0779371f96205678dbcaa3ef499be2e5f262c8b09aadc11754bf3daf9f35e03e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.7 MB (25688211 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3941d3b032a8168d53508410a67baad120a563df67a7959565a30a1cb2114731`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 08 Mar 2023 03:22:42 GMT
ARG RELEASE
# Wed, 08 Mar 2023 03:22:42 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 03:22:42 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 03:22:42 GMT
LABEL org.opencontainers.image.version=18.04
# Wed, 08 Mar 2023 03:22:44 GMT
ADD file:4560926e076acae6b8396a9f1e760eee0f53e22e90ce8554dda57f1103547795 in / 
# Wed, 08 Mar 2023 03:22:44 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:0c5227665c11379f79e9da3d3e4f1724f9316b87d259ac0131628ca1b923a392`  
		Last Modified: Wed, 08 Mar 2023 03:59:25 GMT  
		Size: 25.7 MB (25688211 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:bionic` - linux; arm variant v7

```console
$ docker pull ubuntu@sha256:715ddeafc950876ef9451c460d43ac1ba3e90655f582d845c7f656ee557bd2b2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **21.4 MB (21394593 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c0feaeaa2e651a8712ecfc0727458ba88952949b4b9136d20f0e7adb6a743c1f`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 08 Mar 2023 03:27:01 GMT
ARG RELEASE
# Wed, 08 Mar 2023 03:27:01 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 03:27:01 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 03:27:01 GMT
LABEL org.opencontainers.image.version=18.04
# Wed, 08 Mar 2023 03:27:08 GMT
ADD file:21d7947367fe1aa8cc668c943d11c4841b0ead14b9103ef46fb8db8084603a75 in / 
# Wed, 08 Mar 2023 03:27:09 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:55e299352d1e9c6f1d6e7aee23f9204c8e147eec9fb877be5649ad7f1af58bca`  
		Last Modified: Wed, 08 Mar 2023 03:59:37 GMT  
		Size: 21.4 MB (21394593 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:bionic` - linux; arm64 variant v8

```console
$ docker pull ubuntu@sha256:e77e90f3a41b2c9480c68088c746065623ba9ca77f4e311070ebf404ac6ef2dd
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **22.7 MB (22710750 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c1adc1968c7b7646687f8585de8e3473681323cb9052956ed8f509529a52e61d`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 08 Mar 2023 03:25:33 GMT
ARG RELEASE
# Wed, 08 Mar 2023 03:25:33 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 03:25:34 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 03:25:34 GMT
LABEL org.opencontainers.image.version=18.04
# Wed, 08 Mar 2023 03:25:35 GMT
ADD file:5f229d85bac2e85aa7ce97b2168fc61bd401d0151e8940a12d244356f984e65f in / 
# Wed, 08 Mar 2023 03:25:35 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:13f679bb266a0be5756ce3bb145f89ccd6395d778b1a4bed5a0b0b26105bde2b`  
		Last Modified: Wed, 08 Mar 2023 03:59:31 GMT  
		Size: 22.7 MB (22710750 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:bionic` - linux; 386

```console
$ docker pull ubuntu@sha256:7cbc4fafddce3cf793a94c3b5dc6295a3f569b9222c5e4e74b38aa00a65442fb
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.1 MB (26095131 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d713953b7d565f057a079026363b57bd30e4e9fef8aeaf217f6c4c8b20d968f1`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 08 Mar 2023 03:13:19 GMT
ARG RELEASE
# Wed, 08 Mar 2023 03:13:19 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 03:13:19 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 03:13:19 GMT
LABEL org.opencontainers.image.version=18.04
# Wed, 08 Mar 2023 03:13:21 GMT
ADD file:6cf3e34995c6c44762ed692b86a0442d981e9a69fa4288960047e505d75c0223 in / 
# Wed, 08 Mar 2023 03:13:22 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:472741f7e602c0ee1b34eaf14bb55e0a9377b9f28b0b00fd7ddb5b9d07046a7d`  
		Last Modified: Wed, 08 Mar 2023 03:59:42 GMT  
		Size: 26.1 MB (26095131 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:bionic` - linux; ppc64le

```console
$ docker pull ubuntu@sha256:c955620556f7490d6c4cbd7c1d73faeaad2f635cc3207ee8278832c897d1a7e2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.4 MB (29350183 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:342b45b2835cf4d380d116f2d5e52053a8335089236b194c117adf34efac0409`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 08 Mar 2023 03:13:23 GMT
ARG RELEASE
# Wed, 08 Mar 2023 03:13:23 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 03:13:23 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 03:13:23 GMT
LABEL org.opencontainers.image.version=18.04
# Wed, 08 Mar 2023 03:13:26 GMT
ADD file:5ea8615c09f693252cb9d45458421679f82f84d315200a7611165869195b3a69 in / 
# Wed, 08 Mar 2023 03:13:26 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:293f1b6b3486ffa5f90fdcf0f22fc2091718a3e012fadf073bf57b6a8604df20`  
		Last Modified: Wed, 08 Mar 2023 03:59:48 GMT  
		Size: 29.4 MB (29350183 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:bionic` - linux; s390x

```console
$ docker pull ubuntu@sha256:1e8deff80e7d247c13e32a88efe3ca7314c2e8eb6ab5224e1a7671d7d8076428
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **24.7 MB (24743830 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4ed683baf1b6cc5ec9754e58ee88c3414d4781d2b27d33dc89e16d191249bd0f`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 08 Mar 2023 03:23:29 GMT
ARG RELEASE
# Wed, 08 Mar 2023 03:23:29 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 03:23:29 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 03:23:29 GMT
LABEL org.opencontainers.image.version=18.04
# Wed, 08 Mar 2023 03:23:31 GMT
ADD file:a6309e462d28398152cb726a11615118d79858da963b8c614772b87d87465967 in / 
# Wed, 08 Mar 2023 03:23:31 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:ff61d052565af59dfea677d587c19bf7759efb08fa5db9c11019e2b30b183d9b`  
		Last Modified: Wed, 08 Mar 2023 03:59:54 GMT  
		Size: 24.7 MB (24743830 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

## `ubuntu:bionic-20230308`

```console
$ docker pull ubuntu@sha256:8aa9c2798215f99544d1ce7439ea9c3a6dfd82de607da1cec3a8a2fae005931b
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `ubuntu:bionic-20230308` - linux; amd64

```console
$ docker pull ubuntu@sha256:0779371f96205678dbcaa3ef499be2e5f262c8b09aadc11754bf3daf9f35e03e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.7 MB (25688211 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3941d3b032a8168d53508410a67baad120a563df67a7959565a30a1cb2114731`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 08 Mar 2023 03:22:42 GMT
ARG RELEASE
# Wed, 08 Mar 2023 03:22:42 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 03:22:42 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 03:22:42 GMT
LABEL org.opencontainers.image.version=18.04
# Wed, 08 Mar 2023 03:22:44 GMT
ADD file:4560926e076acae6b8396a9f1e760eee0f53e22e90ce8554dda57f1103547795 in / 
# Wed, 08 Mar 2023 03:22:44 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:0c5227665c11379f79e9da3d3e4f1724f9316b87d259ac0131628ca1b923a392`  
		Last Modified: Wed, 08 Mar 2023 03:59:25 GMT  
		Size: 25.7 MB (25688211 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:bionic-20230308` - linux; arm variant v7

```console
$ docker pull ubuntu@sha256:715ddeafc950876ef9451c460d43ac1ba3e90655f582d845c7f656ee557bd2b2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **21.4 MB (21394593 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c0feaeaa2e651a8712ecfc0727458ba88952949b4b9136d20f0e7adb6a743c1f`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 08 Mar 2023 03:27:01 GMT
ARG RELEASE
# Wed, 08 Mar 2023 03:27:01 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 03:27:01 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 03:27:01 GMT
LABEL org.opencontainers.image.version=18.04
# Wed, 08 Mar 2023 03:27:08 GMT
ADD file:21d7947367fe1aa8cc668c943d11c4841b0ead14b9103ef46fb8db8084603a75 in / 
# Wed, 08 Mar 2023 03:27:09 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:55e299352d1e9c6f1d6e7aee23f9204c8e147eec9fb877be5649ad7f1af58bca`  
		Last Modified: Wed, 08 Mar 2023 03:59:37 GMT  
		Size: 21.4 MB (21394593 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:bionic-20230308` - linux; arm64 variant v8

```console
$ docker pull ubuntu@sha256:e77e90f3a41b2c9480c68088c746065623ba9ca77f4e311070ebf404ac6ef2dd
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **22.7 MB (22710750 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c1adc1968c7b7646687f8585de8e3473681323cb9052956ed8f509529a52e61d`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 08 Mar 2023 03:25:33 GMT
ARG RELEASE
# Wed, 08 Mar 2023 03:25:33 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 03:25:34 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 03:25:34 GMT
LABEL org.opencontainers.image.version=18.04
# Wed, 08 Mar 2023 03:25:35 GMT
ADD file:5f229d85bac2e85aa7ce97b2168fc61bd401d0151e8940a12d244356f984e65f in / 
# Wed, 08 Mar 2023 03:25:35 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:13f679bb266a0be5756ce3bb145f89ccd6395d778b1a4bed5a0b0b26105bde2b`  
		Last Modified: Wed, 08 Mar 2023 03:59:31 GMT  
		Size: 22.7 MB (22710750 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:bionic-20230308` - linux; 386

```console
$ docker pull ubuntu@sha256:7cbc4fafddce3cf793a94c3b5dc6295a3f569b9222c5e4e74b38aa00a65442fb
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.1 MB (26095131 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d713953b7d565f057a079026363b57bd30e4e9fef8aeaf217f6c4c8b20d968f1`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 08 Mar 2023 03:13:19 GMT
ARG RELEASE
# Wed, 08 Mar 2023 03:13:19 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 03:13:19 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 03:13:19 GMT
LABEL org.opencontainers.image.version=18.04
# Wed, 08 Mar 2023 03:13:21 GMT
ADD file:6cf3e34995c6c44762ed692b86a0442d981e9a69fa4288960047e505d75c0223 in / 
# Wed, 08 Mar 2023 03:13:22 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:472741f7e602c0ee1b34eaf14bb55e0a9377b9f28b0b00fd7ddb5b9d07046a7d`  
		Last Modified: Wed, 08 Mar 2023 03:59:42 GMT  
		Size: 26.1 MB (26095131 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:bionic-20230308` - linux; ppc64le

```console
$ docker pull ubuntu@sha256:c955620556f7490d6c4cbd7c1d73faeaad2f635cc3207ee8278832c897d1a7e2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.4 MB (29350183 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:342b45b2835cf4d380d116f2d5e52053a8335089236b194c117adf34efac0409`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 08 Mar 2023 03:13:23 GMT
ARG RELEASE
# Wed, 08 Mar 2023 03:13:23 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 03:13:23 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 03:13:23 GMT
LABEL org.opencontainers.image.version=18.04
# Wed, 08 Mar 2023 03:13:26 GMT
ADD file:5ea8615c09f693252cb9d45458421679f82f84d315200a7611165869195b3a69 in / 
# Wed, 08 Mar 2023 03:13:26 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:293f1b6b3486ffa5f90fdcf0f22fc2091718a3e012fadf073bf57b6a8604df20`  
		Last Modified: Wed, 08 Mar 2023 03:59:48 GMT  
		Size: 29.4 MB (29350183 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:bionic-20230308` - linux; s390x

```console
$ docker pull ubuntu@sha256:1e8deff80e7d247c13e32a88efe3ca7314c2e8eb6ab5224e1a7671d7d8076428
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **24.7 MB (24743830 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4ed683baf1b6cc5ec9754e58ee88c3414d4781d2b27d33dc89e16d191249bd0f`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 08 Mar 2023 03:23:29 GMT
ARG RELEASE
# Wed, 08 Mar 2023 03:23:29 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 03:23:29 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 03:23:29 GMT
LABEL org.opencontainers.image.version=18.04
# Wed, 08 Mar 2023 03:23:31 GMT
ADD file:a6309e462d28398152cb726a11615118d79858da963b8c614772b87d87465967 in / 
# Wed, 08 Mar 2023 03:23:31 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:ff61d052565af59dfea677d587c19bf7759efb08fa5db9c11019e2b30b183d9b`  
		Last Modified: Wed, 08 Mar 2023 03:59:54 GMT  
		Size: 24.7 MB (24743830 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

## `ubuntu:devel`

```console
$ docker pull ubuntu@sha256:008c0f6712067722f42f9685476d37b0b7b689e31d66e5787d1920c7ac230849
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
$ docker pull ubuntu@sha256:ffa4bb610fa4c137211199607a5326c5a409b189d3c673cc85a4c65f5757447b
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.8 MB (26761270 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:de432ed6bff895b418712abd3084394e7dd70656b905d6390ffba649c63c64a3`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 14 Mar 2023 18:21:45 GMT
ARG RELEASE
# Tue, 14 Mar 2023 18:21:45 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 14 Mar 2023 18:21:45 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 14 Mar 2023 18:21:45 GMT
LABEL org.opencontainers.image.version=23.04
# Tue, 14 Mar 2023 18:21:47 GMT
ADD file:108000e07d9734743bfe65381248aa7e309283bdb87d8687b7ffe0d697487109 in / 
# Tue, 14 Mar 2023 18:21:47 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:391f30eda8cdf14ab4acf7e6ce5bac054bcc1d98fe5f8789908c6bc739dee216`  
		Last Modified: Tue, 14 Mar 2023 18:47:00 GMT  
		Size: 26.8 MB (26761270 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:devel` - linux; arm variant v7

```console
$ docker pull ubuntu@sha256:e685540e6030c9b728fa6485ca8e844d824e064c9a790bc54e6e6507974ba42e
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **24.6 MB (24559160 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:28e4ad84aaa1e06e217b7ed880b9bea183f12a02bb5b8408f57855354fbd91c9`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 14 Mar 2023 18:18:28 GMT
ARG RELEASE
# Tue, 14 Mar 2023 18:18:28 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 14 Mar 2023 18:18:28 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 14 Mar 2023 18:18:28 GMT
LABEL org.opencontainers.image.version=23.04
# Tue, 14 Mar 2023 18:18:30 GMT
ADD file:dc39df38ee577fc1ddb753815787f9a90231d34a28c65e14298d136132c8d7d5 in / 
# Tue, 14 Mar 2023 18:18:31 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:7ec8b1962079f6d8d8477e2e227966fcf2e91d26a81735eb5f0411f84cbf8740`  
		Last Modified: Tue, 14 Mar 2023 18:47:12 GMT  
		Size: 24.6 MB (24559160 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:devel` - linux; arm64 variant v8

```console
$ docker pull ubuntu@sha256:b864a1f0e9f2686fcaa86491f78d38af1b9e8e53e965df39d991a8b685bf7c74
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.0 MB (26007489 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e399e758a4b24fbecd3eed7dbaadf0eb3aa45f2ee4b2c133561693f31008b42b`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 14 Mar 2023 17:38:32 GMT
ARG RELEASE
# Tue, 14 Mar 2023 17:38:32 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 14 Mar 2023 17:38:32 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 14 Mar 2023 17:38:32 GMT
LABEL org.opencontainers.image.version=23.04
# Tue, 14 Mar 2023 17:38:40 GMT
ADD file:2562122b72f2bcdd0678a1bd0836dcbf376a8e33078452497d85ed0cd425391f in / 
# Tue, 14 Mar 2023 17:38:41 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:ff6383e8c55f097496fc03e31f40ad77007ac50d51f9735a1d45789985087387`  
		Last Modified: Tue, 14 Mar 2023 18:47:06 GMT  
		Size: 26.0 MB (26007489 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:devel` - linux; ppc64le

```console
$ docker pull ubuntu@sha256:8e0b2dedffe81c417dc0860a92ec8520aca6f48b6b3267b18590c1ff4c4f16ea
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.0 MB (30987169 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:26160bb786e079c716ceda59a2a70b6e813f9e43dea7866e98e9edfe8a1cb84f`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 14 Mar 2023 17:31:48 GMT
ARG RELEASE
# Tue, 14 Mar 2023 17:31:48 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 14 Mar 2023 17:31:48 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 14 Mar 2023 17:31:48 GMT
LABEL org.opencontainers.image.version=23.04
# Tue, 14 Mar 2023 17:31:51 GMT
ADD file:586ae3783043b40d20c362128778cbf64404358967d540af0c899067d82744f8 in / 
# Tue, 14 Mar 2023 17:31:52 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:59dbd023a22a72c486e06919c527e79036e5a5b41ca794aafbbd35687256dee7`  
		Last Modified: Tue, 14 Mar 2023 18:47:20 GMT  
		Size: 31.0 MB (30987169 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:devel` - linux; s390x

```console
$ docker pull ubuntu@sha256:1840997cef13af4d355cf1b5bda18e68073cc6aefe673bd36cb93ea91f3452a2
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.6 MB (25634517 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6d6744e3a8d8d30ea66143d1d2ba080a6cb9a9e1356857de142edfd33ddefb5e`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 14 Mar 2023 17:47:18 GMT
ARG RELEASE
# Tue, 14 Mar 2023 17:47:18 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 14 Mar 2023 17:47:18 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 14 Mar 2023 17:47:18 GMT
LABEL org.opencontainers.image.version=23.04
# Tue, 14 Mar 2023 17:47:20 GMT
ADD file:1ed4a1aa279c8c4fd49f73ed214f53835caecef222778b80716ba71fe60cc7f0 in / 
# Tue, 14 Mar 2023 17:47:20 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:de8d2f62d0190fb3786c431d236f8d6178a12304755c3c13b8c1ff4d6097587f`  
		Last Modified: Tue, 14 Mar 2023 18:47:26 GMT  
		Size: 25.6 MB (25634517 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

## `ubuntu:focal`

```console
$ docker pull ubuntu@sha256:24a0df437301598d1a4b62ddf59fa0ed2969150d70d748c84225e6501e9c36b9
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
$ docker pull ubuntu@sha256:b39db7fc56971aac21dee02187e898db759c4f26b9b27b1d80b6ad32ff330c76
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.5 MB (27503825 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1c5c8d0b973ab9d6d7742cf050beefa8ba2efb7779e09bfb1200d6192180766e`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 08 Mar 2023 04:41:24 GMT
ARG RELEASE
# Wed, 08 Mar 2023 04:41:24 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 04:41:24 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 04:41:24 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 08 Mar 2023 04:41:26 GMT
ADD file:20f2ff22b9a8ca9bec5178036c9ebc525a12cd4312daf5d14a9a631a30be20e1 in / 
# Wed, 08 Mar 2023 04:41:27 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:06d39c85623a79eb68b6cac39f4c4aba8834873ee5fc27be9d9d7655e6313c26`  
		Last Modified: Wed, 08 Mar 2023 05:10:29 GMT  
		Size: 27.5 MB (27503825 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:focal` - linux; arm variant v7

```console
$ docker pull ubuntu@sha256:223d6beaf1aa0978b7a0dc4731333b59fe35ee9d3a8c48db1a8d686b1b211ea0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.6 MB (23608664 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4731390bddee2b1dc9fa35d820d20b69f95bb16381ae1434821f52eb87f9d503`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 08 Mar 2023 04:31:43 GMT
ARG RELEASE
# Wed, 08 Mar 2023 04:31:43 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 04:31:43 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 04:31:43 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 08 Mar 2023 04:31:46 GMT
ADD file:99d501af7a191308f8fe3dc3f33c63bd8b54fb749d061b1a901c423b85f8cec2 in / 
# Wed, 08 Mar 2023 04:31:46 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:3503cc1332f3fe649c8a0937dbf6f052f1d2d9b9bdb97546cf15f09ec495d7a4`  
		Last Modified: Wed, 08 Mar 2023 05:10:41 GMT  
		Size: 23.6 MB (23608664 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:focal` - linux; arm64 variant v8

```console
$ docker pull ubuntu@sha256:f92b9de5f10b6e1fcda653f5d02bd6c816386dfb830c71cef95df52b2280cd1c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.0 MB (25973169 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:625d192afcdc5add2f097cd05a177ab19f18e69473911dbb479fc5eba56ba8fd`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 08 Mar 2023 04:34:20 GMT
ARG RELEASE
# Wed, 08 Mar 2023 04:34:20 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 04:34:20 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 04:34:20 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 08 Mar 2023 04:34:24 GMT
ADD file:e73d5d005a3ba2c2fb3d8585a1f19daf5ea9ed75af5a2f97b1cc6f7f03db0cdc in / 
# Wed, 08 Mar 2023 04:34:24 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:a774dfcdedc7c7c4f0009ddadc2f33557d60452450684534df5625f9693df81a`  
		Last Modified: Wed, 08 Mar 2023 05:10:35 GMT  
		Size: 26.0 MB (25973169 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:focal` - linux; ppc64le

```console
$ docker pull ubuntu@sha256:36b2d0b2c6aeee6945261da06ed2a0f8be5548bc5f974e3ffd224baa77e585b2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.1 MB (32068376 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7e49f046bd37833635fbd8d90722b7b57c00811d3ccf7ed7d78e796f669fbcbf`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 08 Mar 2023 04:39:14 GMT
ARG RELEASE
# Wed, 08 Mar 2023 04:39:14 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 04:39:14 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 04:39:14 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 08 Mar 2023 04:39:17 GMT
ADD file:e8eae0af07e662df38a5b691d04648b4fc72382b6918877da22520ed4d01c3a6 in / 
# Wed, 08 Mar 2023 04:39:17 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:231de8dd1e233ca65e29bae666ffef95bfca99c9ca8decd4bb6cd73269924f31`  
		Last Modified: Wed, 08 Mar 2023 05:10:47 GMT  
		Size: 32.1 MB (32068376 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:focal` - linux; s390x

```console
$ docker pull ubuntu@sha256:ee77c5eb098846cf57a751c5b4d28678f152ebd936ee700570f77e5181f94749
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.4 MB (26364051 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0ae7691e3a999c7848a0952ef29ffbb1c235587dfce87cba0df7e8d23a8b0be6`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 08 Mar 2023 04:41:58 GMT
ARG RELEASE
# Wed, 08 Mar 2023 04:41:58 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 04:41:58 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 04:41:58 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 08 Mar 2023 04:42:00 GMT
ADD file:4463dafd3352de8c5ff87090e2f30be9bdffc3fa9d84e27b13e2364d856f82e9 in / 
# Wed, 08 Mar 2023 04:42:00 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:68e65db8d2065c8b6d0764029cabc60b7c7bfd9dc8fb638e0effa6e544486597`  
		Last Modified: Wed, 08 Mar 2023 05:10:53 GMT  
		Size: 26.4 MB (26364051 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

## `ubuntu:focal-20230308`

```console
$ docker pull ubuntu@sha256:24a0df437301598d1a4b62ddf59fa0ed2969150d70d748c84225e6501e9c36b9
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `ubuntu:focal-20230308` - linux; amd64

```console
$ docker pull ubuntu@sha256:b39db7fc56971aac21dee02187e898db759c4f26b9b27b1d80b6ad32ff330c76
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.5 MB (27503825 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1c5c8d0b973ab9d6d7742cf050beefa8ba2efb7779e09bfb1200d6192180766e`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 08 Mar 2023 04:41:24 GMT
ARG RELEASE
# Wed, 08 Mar 2023 04:41:24 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 04:41:24 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 04:41:24 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 08 Mar 2023 04:41:26 GMT
ADD file:20f2ff22b9a8ca9bec5178036c9ebc525a12cd4312daf5d14a9a631a30be20e1 in / 
# Wed, 08 Mar 2023 04:41:27 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:06d39c85623a79eb68b6cac39f4c4aba8834873ee5fc27be9d9d7655e6313c26`  
		Last Modified: Wed, 08 Mar 2023 05:10:29 GMT  
		Size: 27.5 MB (27503825 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:focal-20230308` - linux; arm variant v7

```console
$ docker pull ubuntu@sha256:223d6beaf1aa0978b7a0dc4731333b59fe35ee9d3a8c48db1a8d686b1b211ea0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.6 MB (23608664 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4731390bddee2b1dc9fa35d820d20b69f95bb16381ae1434821f52eb87f9d503`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 08 Mar 2023 04:31:43 GMT
ARG RELEASE
# Wed, 08 Mar 2023 04:31:43 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 04:31:43 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 04:31:43 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 08 Mar 2023 04:31:46 GMT
ADD file:99d501af7a191308f8fe3dc3f33c63bd8b54fb749d061b1a901c423b85f8cec2 in / 
# Wed, 08 Mar 2023 04:31:46 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:3503cc1332f3fe649c8a0937dbf6f052f1d2d9b9bdb97546cf15f09ec495d7a4`  
		Last Modified: Wed, 08 Mar 2023 05:10:41 GMT  
		Size: 23.6 MB (23608664 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:focal-20230308` - linux; arm64 variant v8

```console
$ docker pull ubuntu@sha256:f92b9de5f10b6e1fcda653f5d02bd6c816386dfb830c71cef95df52b2280cd1c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.0 MB (25973169 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:625d192afcdc5add2f097cd05a177ab19f18e69473911dbb479fc5eba56ba8fd`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 08 Mar 2023 04:34:20 GMT
ARG RELEASE
# Wed, 08 Mar 2023 04:34:20 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 04:34:20 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 04:34:20 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 08 Mar 2023 04:34:24 GMT
ADD file:e73d5d005a3ba2c2fb3d8585a1f19daf5ea9ed75af5a2f97b1cc6f7f03db0cdc in / 
# Wed, 08 Mar 2023 04:34:24 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:a774dfcdedc7c7c4f0009ddadc2f33557d60452450684534df5625f9693df81a`  
		Last Modified: Wed, 08 Mar 2023 05:10:35 GMT  
		Size: 26.0 MB (25973169 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:focal-20230308` - linux; ppc64le

```console
$ docker pull ubuntu@sha256:36b2d0b2c6aeee6945261da06ed2a0f8be5548bc5f974e3ffd224baa77e585b2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.1 MB (32068376 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7e49f046bd37833635fbd8d90722b7b57c00811d3ccf7ed7d78e796f669fbcbf`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 08 Mar 2023 04:39:14 GMT
ARG RELEASE
# Wed, 08 Mar 2023 04:39:14 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 04:39:14 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 04:39:14 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 08 Mar 2023 04:39:17 GMT
ADD file:e8eae0af07e662df38a5b691d04648b4fc72382b6918877da22520ed4d01c3a6 in / 
# Wed, 08 Mar 2023 04:39:17 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:231de8dd1e233ca65e29bae666ffef95bfca99c9ca8decd4bb6cd73269924f31`  
		Last Modified: Wed, 08 Mar 2023 05:10:47 GMT  
		Size: 32.1 MB (32068376 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:focal-20230308` - linux; s390x

```console
$ docker pull ubuntu@sha256:ee77c5eb098846cf57a751c5b4d28678f152ebd936ee700570f77e5181f94749
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.4 MB (26364051 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0ae7691e3a999c7848a0952ef29ffbb1c235587dfce87cba0df7e8d23a8b0be6`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 08 Mar 2023 04:41:58 GMT
ARG RELEASE
# Wed, 08 Mar 2023 04:41:58 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 04:41:58 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 04:41:58 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 08 Mar 2023 04:42:00 GMT
ADD file:4463dafd3352de8c5ff87090e2f30be9bdffc3fa9d84e27b13e2364d856f82e9 in / 
# Wed, 08 Mar 2023 04:42:00 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:68e65db8d2065c8b6d0764029cabc60b7c7bfd9dc8fb638e0effa6e544486597`  
		Last Modified: Wed, 08 Mar 2023 05:10:53 GMT  
		Size: 26.4 MB (26364051 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

## `ubuntu:jammy`

```console
$ docker pull ubuntu@sha256:67211c14fa74f070d27cc59d69a7fa9aeff8e28ea118ef3babc295a0428a6d21
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
$ docker pull ubuntu@sha256:7a57c69fe1e9d5b97c5fe649849e79f2cfc3bf11d10bbd5218b4eb61716aebe6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.5 MB (29533950 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:08d22c0ceb150ddeb2237c5fa3129c0183f3cc6f5eeb2e7aa4016da3ad02140a`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 08 Mar 2023 04:44:25 GMT
ARG RELEASE
# Wed, 08 Mar 2023 04:44:25 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 04:44:25 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 04:44:25 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 08 Mar 2023 04:44:27 GMT
ADD file:c8ef6447752cab2541ffca9e3cfa27d581f3491bc8f356f6eafd951243609341 in / 
# Wed, 08 Mar 2023 04:44:27 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:2ab09b027e7f3a0c2e8bb1944ac46de38cebab7145f0bd6effebfe5492c818b6`  
		Last Modified: Wed, 08 Mar 2023 05:10:20 GMT  
		Size: 29.5 MB (29533950 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:jammy` - linux; arm variant v7

```console
$ docker pull ubuntu@sha256:ad18cfdb19dac67bf0072dacea661a817330e5c955d081f4d09914e743ae5d4a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.1 MB (26140319 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2bf0095935ffb29018664cf219d8c1b2c890e3e3c4af89113df23e7330397187`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 08 Mar 2023 04:31:38 GMT
ARG RELEASE
# Wed, 08 Mar 2023 04:31:38 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 04:31:39 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 04:31:39 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 08 Mar 2023 04:31:41 GMT
ADD file:e9c3ac290fb81ae2e78de99052d776396ee3aff05e1a66fd2dccb01d7de9bb45 in / 
# Wed, 08 Mar 2023 04:31:42 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:aea1895b7fd03ef3bc263eef4b6f1dd219fc3286f3ff79495aadb81a88650723`  
		Last Modified: Wed, 08 Mar 2023 05:10:33 GMT  
		Size: 26.1 MB (26140319 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:jammy` - linux; arm64 variant v8

```console
$ docker pull ubuntu@sha256:537da24818633b45fcb65e5285a68c3ec1f3db25f5ae5476a7757bc8dfae92a3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.3 MB (27347481 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bab8ce5c00ca3ef91e0d3eb4c6e6d6ec7cffa9574c447fd8d54a8d96e7c1c80e`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 08 Mar 2023 04:32:38 GMT
ARG RELEASE
# Wed, 08 Mar 2023 04:32:38 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 04:32:38 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 04:32:39 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 08 Mar 2023 04:32:40 GMT
ADD file:79b36308bc382d9cae7197b4cecc21430f4e8f3e8bec3547d0f00bcff7681e60 in / 
# Wed, 08 Mar 2023 04:32:41 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:cd741b12a7eaa64357041c2d3f4590c898313a7f8f65cd1577594e6ee03a8c38`  
		Last Modified: Wed, 08 Mar 2023 05:10:27 GMT  
		Size: 27.3 MB (27347481 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:jammy` - linux; ppc64le

```console
$ docker pull ubuntu@sha256:f23b7ade9f88f91c8d5932a48b721712ed509a607d9a05cdeae4cd06de09e5f7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.6 MB (34593661 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4220c61b3ab7b82dd3ff3395f9efe2b63e730c3f24284d1519013cf3cda822f8`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 08 Mar 2023 04:39:16 GMT
ARG RELEASE
# Wed, 08 Mar 2023 04:39:16 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 04:39:16 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 04:39:16 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 08 Mar 2023 04:39:20 GMT
ADD file:d7434a52d8d8aa6288e788f6fe7e156f0e11bf9b8275efaf70aab0bfc4d919cf in / 
# Wed, 08 Mar 2023 04:39:20 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:2561b3b559ec9b25bafa07804afa433803291265f7dd847de711224b0f238237`  
		Last Modified: Wed, 08 Mar 2023 05:10:39 GMT  
		Size: 34.6 MB (34593661 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:jammy` - linux; s390x

```console
$ docker pull ubuntu@sha256:b351315d950a4da70f19d62f4da5dd7f9a445eb8c8d6851a5b6cdddbdafb13cf
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.0 MB (28015959 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:63ad39053efde0c294433cd8f9709c6d69a36e1f0af4ffbf81c3d261caffb615`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 08 Mar 2023 04:39:24 GMT
ARG RELEASE
# Wed, 08 Mar 2023 04:39:24 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 04:39:24 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 04:39:24 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 08 Mar 2023 04:39:26 GMT
ADD file:630f9865d3d4fd4294d45cac7cbaea83fb549c2e563de454348da964d19fbbba in / 
# Wed, 08 Mar 2023 04:39:26 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:15f635e04e894b7646b4ebca40424ddf244867fc663429ea8b877eca172a7cf1`  
		Last Modified: Wed, 08 Mar 2023 05:10:46 GMT  
		Size: 28.0 MB (28015959 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

## `ubuntu:jammy-20230308`

```console
$ docker pull ubuntu@sha256:67211c14fa74f070d27cc59d69a7fa9aeff8e28ea118ef3babc295a0428a6d21
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `ubuntu:jammy-20230308` - linux; amd64

```console
$ docker pull ubuntu@sha256:7a57c69fe1e9d5b97c5fe649849e79f2cfc3bf11d10bbd5218b4eb61716aebe6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.5 MB (29533950 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:08d22c0ceb150ddeb2237c5fa3129c0183f3cc6f5eeb2e7aa4016da3ad02140a`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 08 Mar 2023 04:44:25 GMT
ARG RELEASE
# Wed, 08 Mar 2023 04:44:25 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 04:44:25 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 04:44:25 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 08 Mar 2023 04:44:27 GMT
ADD file:c8ef6447752cab2541ffca9e3cfa27d581f3491bc8f356f6eafd951243609341 in / 
# Wed, 08 Mar 2023 04:44:27 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:2ab09b027e7f3a0c2e8bb1944ac46de38cebab7145f0bd6effebfe5492c818b6`  
		Last Modified: Wed, 08 Mar 2023 05:10:20 GMT  
		Size: 29.5 MB (29533950 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:jammy-20230308` - linux; arm variant v7

```console
$ docker pull ubuntu@sha256:ad18cfdb19dac67bf0072dacea661a817330e5c955d081f4d09914e743ae5d4a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.1 MB (26140319 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2bf0095935ffb29018664cf219d8c1b2c890e3e3c4af89113df23e7330397187`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 08 Mar 2023 04:31:38 GMT
ARG RELEASE
# Wed, 08 Mar 2023 04:31:38 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 04:31:39 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 04:31:39 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 08 Mar 2023 04:31:41 GMT
ADD file:e9c3ac290fb81ae2e78de99052d776396ee3aff05e1a66fd2dccb01d7de9bb45 in / 
# Wed, 08 Mar 2023 04:31:42 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:aea1895b7fd03ef3bc263eef4b6f1dd219fc3286f3ff79495aadb81a88650723`  
		Last Modified: Wed, 08 Mar 2023 05:10:33 GMT  
		Size: 26.1 MB (26140319 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:jammy-20230308` - linux; arm64 variant v8

```console
$ docker pull ubuntu@sha256:537da24818633b45fcb65e5285a68c3ec1f3db25f5ae5476a7757bc8dfae92a3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.3 MB (27347481 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bab8ce5c00ca3ef91e0d3eb4c6e6d6ec7cffa9574c447fd8d54a8d96e7c1c80e`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 08 Mar 2023 04:32:38 GMT
ARG RELEASE
# Wed, 08 Mar 2023 04:32:38 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 04:32:38 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 04:32:39 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 08 Mar 2023 04:32:40 GMT
ADD file:79b36308bc382d9cae7197b4cecc21430f4e8f3e8bec3547d0f00bcff7681e60 in / 
# Wed, 08 Mar 2023 04:32:41 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:cd741b12a7eaa64357041c2d3f4590c898313a7f8f65cd1577594e6ee03a8c38`  
		Last Modified: Wed, 08 Mar 2023 05:10:27 GMT  
		Size: 27.3 MB (27347481 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:jammy-20230308` - linux; ppc64le

```console
$ docker pull ubuntu@sha256:f23b7ade9f88f91c8d5932a48b721712ed509a607d9a05cdeae4cd06de09e5f7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.6 MB (34593661 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4220c61b3ab7b82dd3ff3395f9efe2b63e730c3f24284d1519013cf3cda822f8`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 08 Mar 2023 04:39:16 GMT
ARG RELEASE
# Wed, 08 Mar 2023 04:39:16 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 04:39:16 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 04:39:16 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 08 Mar 2023 04:39:20 GMT
ADD file:d7434a52d8d8aa6288e788f6fe7e156f0e11bf9b8275efaf70aab0bfc4d919cf in / 
# Wed, 08 Mar 2023 04:39:20 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:2561b3b559ec9b25bafa07804afa433803291265f7dd847de711224b0f238237`  
		Last Modified: Wed, 08 Mar 2023 05:10:39 GMT  
		Size: 34.6 MB (34593661 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:jammy-20230308` - linux; s390x

```console
$ docker pull ubuntu@sha256:b351315d950a4da70f19d62f4da5dd7f9a445eb8c8d6851a5b6cdddbdafb13cf
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.0 MB (28015959 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:63ad39053efde0c294433cd8f9709c6d69a36e1f0af4ffbf81c3d261caffb615`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 08 Mar 2023 04:39:24 GMT
ARG RELEASE
# Wed, 08 Mar 2023 04:39:24 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 04:39:24 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 04:39:24 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 08 Mar 2023 04:39:26 GMT
ADD file:630f9865d3d4fd4294d45cac7cbaea83fb549c2e563de454348da964d19fbbba in / 
# Wed, 08 Mar 2023 04:39:26 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:15f635e04e894b7646b4ebca40424ddf244867fc663429ea8b877eca172a7cf1`  
		Last Modified: Wed, 08 Mar 2023 05:10:46 GMT  
		Size: 28.0 MB (28015959 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

## `ubuntu:kinetic`

```console
$ docker pull ubuntu@sha256:a82eebb42083a134e009a6b81a7e5d2eecc37112fa8ae40642bd3c5153b7e4f0
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
$ docker pull ubuntu@sha256:8c8f22bacbfba9678edddcc3b6d1e56cce02eff9cbf27ab46116de30cb79a3d6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.7 MB (26695001 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:558d44db75c8f69c29f427cf88e6a71c39320f7607584baa6860f6e4f6121892`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 08 Mar 2023 05:58:05 GMT
ARG RELEASE
# Wed, 08 Mar 2023 05:58:05 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 05:58:05 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 05:58:05 GMT
LABEL org.opencontainers.image.version=22.10
# Wed, 08 Mar 2023 05:58:07 GMT
ADD file:3492508b382c909e968c4d8467b9acbd5f61ed6ca69c8a47241f930d90de7158 in / 
# Wed, 08 Mar 2023 05:58:07 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:5c19388d38e1ea904672812dd0aac505220c9254e2621a1684e0fe29e2dba80e`  
		Last Modified: Wed, 08 Mar 2023 06:38:37 GMT  
		Size: 26.7 MB (26695001 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:kinetic` - linux; arm variant v7

```console
$ docker pull ubuntu@sha256:e37c01607a81ee7737f164af67cb5f5f8e1ecbf82c4f5cfe940675b8e8830ee1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.1 MB (25067205 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:94bcbf2021edfcf5671a4872ded2d62d36cd3a86813acc7bc2471fefce3c2ac2`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 08 Mar 2023 05:55:43 GMT
ARG RELEASE
# Wed, 08 Mar 2023 05:55:43 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 05:55:43 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 05:55:43 GMT
LABEL org.opencontainers.image.version=22.10
# Wed, 08 Mar 2023 05:55:49 GMT
ADD file:827330b6c59e67c5d2edd3ceb3492b97865b15f9246f14710f478d12e94d2048 in / 
# Wed, 08 Mar 2023 05:55:49 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:5c09adf37dd1d92aeedd2906b2635d9b7f1eca9f39f51d52f919d26d113c8d35`  
		Last Modified: Wed, 08 Mar 2023 06:38:49 GMT  
		Size: 25.1 MB (25067205 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:kinetic` - linux; arm64 variant v8

```console
$ docker pull ubuntu@sha256:2a79f91eb2bb4ffc5d96c58a06fda63550bf94a1a6b2e9ef2f835e52ca8a04ee
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.8 MB (25760037 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:438c48db988d0f48de4461bb2bf49524880c28c5863b1ba5b175a9d7c284b009`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 08 Mar 2023 05:57:57 GMT
ARG RELEASE
# Wed, 08 Mar 2023 05:57:57 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 05:57:57 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 05:57:58 GMT
LABEL org.opencontainers.image.version=22.10
# Wed, 08 Mar 2023 05:57:59 GMT
ADD file:884e00dc91bf6d392fa3d117913cc2534177128322d89137bfb8b2734bc38579 in / 
# Wed, 08 Mar 2023 05:58:00 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:4f720bb411d1d3a6b6c043988c66cdaeee655f968c6eabf7f1ada7ac1529b046`  
		Last Modified: Wed, 08 Mar 2023 06:38:43 GMT  
		Size: 25.8 MB (25760037 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:kinetic` - linux; ppc64le

```console
$ docker pull ubuntu@sha256:fec18179ce4b8f8215f04ea75ca752d4c7865d1a06f1d9a3d961927ed2916589
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.1 MB (31114002 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:817a0842655ee55d34c1866729026d8d7fd4de6cc4ea4fcbdaac3cbc1dc10a73`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 08 Mar 2023 05:58:03 GMT
ARG RELEASE
# Wed, 08 Mar 2023 05:58:03 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 05:58:03 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 05:58:03 GMT
LABEL org.opencontainers.image.version=22.10
# Wed, 08 Mar 2023 05:58:06 GMT
ADD file:583061e8201c03de4747860e734200b6c35b449443a1382ad8e8efc6f7e9ea13 in / 
# Wed, 08 Mar 2023 05:58:06 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:e9acd60127e6a1f919659d03fc820b762a3f49f62bae6caafbd919cdbd8e4f7b`  
		Last Modified: Wed, 08 Mar 2023 06:38:55 GMT  
		Size: 31.1 MB (31114002 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:kinetic` - linux; s390x

```console
$ docker pull ubuntu@sha256:c69324f895a9152b8a80f9d310710a9d2ef987330d04bc20dbfe23e79e5183bb
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.5 MB (25488878 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4997349fe1813d9306e1ad38084ecc78950e221fe4f75cd9a85e5213139fcd80`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 08 Mar 2023 06:11:04 GMT
ARG RELEASE
# Wed, 08 Mar 2023 06:11:04 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 06:11:04 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 06:11:04 GMT
LABEL org.opencontainers.image.version=22.10
# Wed, 08 Mar 2023 06:11:06 GMT
ADD file:974d67ca1d5bcaacbc707820609d36af0d7ed3ff7179a702a4aa56dcc43f79f3 in / 
# Wed, 08 Mar 2023 06:11:06 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:e7f1a81217015da9b8db635ad002e08952988dc4100cbec474290e8524391920`  
		Last Modified: Wed, 08 Mar 2023 06:39:01 GMT  
		Size: 25.5 MB (25488878 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

## `ubuntu:kinetic-20230308`

```console
$ docker pull ubuntu@sha256:a82eebb42083a134e009a6b81a7e5d2eecc37112fa8ae40642bd3c5153b7e4f0
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `ubuntu:kinetic-20230308` - linux; amd64

```console
$ docker pull ubuntu@sha256:8c8f22bacbfba9678edddcc3b6d1e56cce02eff9cbf27ab46116de30cb79a3d6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.7 MB (26695001 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:558d44db75c8f69c29f427cf88e6a71c39320f7607584baa6860f6e4f6121892`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 08 Mar 2023 05:58:05 GMT
ARG RELEASE
# Wed, 08 Mar 2023 05:58:05 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 05:58:05 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 05:58:05 GMT
LABEL org.opencontainers.image.version=22.10
# Wed, 08 Mar 2023 05:58:07 GMT
ADD file:3492508b382c909e968c4d8467b9acbd5f61ed6ca69c8a47241f930d90de7158 in / 
# Wed, 08 Mar 2023 05:58:07 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:5c19388d38e1ea904672812dd0aac505220c9254e2621a1684e0fe29e2dba80e`  
		Last Modified: Wed, 08 Mar 2023 06:38:37 GMT  
		Size: 26.7 MB (26695001 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:kinetic-20230308` - linux; arm variant v7

```console
$ docker pull ubuntu@sha256:e37c01607a81ee7737f164af67cb5f5f8e1ecbf82c4f5cfe940675b8e8830ee1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.1 MB (25067205 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:94bcbf2021edfcf5671a4872ded2d62d36cd3a86813acc7bc2471fefce3c2ac2`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 08 Mar 2023 05:55:43 GMT
ARG RELEASE
# Wed, 08 Mar 2023 05:55:43 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 05:55:43 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 05:55:43 GMT
LABEL org.opencontainers.image.version=22.10
# Wed, 08 Mar 2023 05:55:49 GMT
ADD file:827330b6c59e67c5d2edd3ceb3492b97865b15f9246f14710f478d12e94d2048 in / 
# Wed, 08 Mar 2023 05:55:49 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:5c09adf37dd1d92aeedd2906b2635d9b7f1eca9f39f51d52f919d26d113c8d35`  
		Last Modified: Wed, 08 Mar 2023 06:38:49 GMT  
		Size: 25.1 MB (25067205 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:kinetic-20230308` - linux; arm64 variant v8

```console
$ docker pull ubuntu@sha256:2a79f91eb2bb4ffc5d96c58a06fda63550bf94a1a6b2e9ef2f835e52ca8a04ee
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.8 MB (25760037 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:438c48db988d0f48de4461bb2bf49524880c28c5863b1ba5b175a9d7c284b009`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 08 Mar 2023 05:57:57 GMT
ARG RELEASE
# Wed, 08 Mar 2023 05:57:57 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 05:57:57 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 05:57:58 GMT
LABEL org.opencontainers.image.version=22.10
# Wed, 08 Mar 2023 05:57:59 GMT
ADD file:884e00dc91bf6d392fa3d117913cc2534177128322d89137bfb8b2734bc38579 in / 
# Wed, 08 Mar 2023 05:58:00 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:4f720bb411d1d3a6b6c043988c66cdaeee655f968c6eabf7f1ada7ac1529b046`  
		Last Modified: Wed, 08 Mar 2023 06:38:43 GMT  
		Size: 25.8 MB (25760037 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:kinetic-20230308` - linux; ppc64le

```console
$ docker pull ubuntu@sha256:fec18179ce4b8f8215f04ea75ca752d4c7865d1a06f1d9a3d961927ed2916589
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.1 MB (31114002 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:817a0842655ee55d34c1866729026d8d7fd4de6cc4ea4fcbdaac3cbc1dc10a73`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 08 Mar 2023 05:58:03 GMT
ARG RELEASE
# Wed, 08 Mar 2023 05:58:03 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 05:58:03 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 05:58:03 GMT
LABEL org.opencontainers.image.version=22.10
# Wed, 08 Mar 2023 05:58:06 GMT
ADD file:583061e8201c03de4747860e734200b6c35b449443a1382ad8e8efc6f7e9ea13 in / 
# Wed, 08 Mar 2023 05:58:06 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:e9acd60127e6a1f919659d03fc820b762a3f49f62bae6caafbd919cdbd8e4f7b`  
		Last Modified: Wed, 08 Mar 2023 06:38:55 GMT  
		Size: 31.1 MB (31114002 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:kinetic-20230308` - linux; s390x

```console
$ docker pull ubuntu@sha256:c69324f895a9152b8a80f9d310710a9d2ef987330d04bc20dbfe23e79e5183bb
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.5 MB (25488878 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4997349fe1813d9306e1ad38084ecc78950e221fe4f75cd9a85e5213139fcd80`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 08 Mar 2023 06:11:04 GMT
ARG RELEASE
# Wed, 08 Mar 2023 06:11:04 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 06:11:04 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 06:11:04 GMT
LABEL org.opencontainers.image.version=22.10
# Wed, 08 Mar 2023 06:11:06 GMT
ADD file:974d67ca1d5bcaacbc707820609d36af0d7ed3ff7179a702a4aa56dcc43f79f3 in / 
# Wed, 08 Mar 2023 06:11:06 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:e7f1a81217015da9b8db635ad002e08952988dc4100cbec474290e8524391920`  
		Last Modified: Wed, 08 Mar 2023 06:39:01 GMT  
		Size: 25.5 MB (25488878 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

## `ubuntu:latest`

```console
$ docker pull ubuntu@sha256:67211c14fa74f070d27cc59d69a7fa9aeff8e28ea118ef3babc295a0428a6d21
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
$ docker pull ubuntu@sha256:7a57c69fe1e9d5b97c5fe649849e79f2cfc3bf11d10bbd5218b4eb61716aebe6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.5 MB (29533950 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:08d22c0ceb150ddeb2237c5fa3129c0183f3cc6f5eeb2e7aa4016da3ad02140a`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 08 Mar 2023 04:44:25 GMT
ARG RELEASE
# Wed, 08 Mar 2023 04:44:25 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 04:44:25 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 04:44:25 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 08 Mar 2023 04:44:27 GMT
ADD file:c8ef6447752cab2541ffca9e3cfa27d581f3491bc8f356f6eafd951243609341 in / 
# Wed, 08 Mar 2023 04:44:27 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:2ab09b027e7f3a0c2e8bb1944ac46de38cebab7145f0bd6effebfe5492c818b6`  
		Last Modified: Wed, 08 Mar 2023 05:10:20 GMT  
		Size: 29.5 MB (29533950 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:latest` - linux; arm variant v7

```console
$ docker pull ubuntu@sha256:ad18cfdb19dac67bf0072dacea661a817330e5c955d081f4d09914e743ae5d4a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.1 MB (26140319 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2bf0095935ffb29018664cf219d8c1b2c890e3e3c4af89113df23e7330397187`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 08 Mar 2023 04:31:38 GMT
ARG RELEASE
# Wed, 08 Mar 2023 04:31:38 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 04:31:39 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 04:31:39 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 08 Mar 2023 04:31:41 GMT
ADD file:e9c3ac290fb81ae2e78de99052d776396ee3aff05e1a66fd2dccb01d7de9bb45 in / 
# Wed, 08 Mar 2023 04:31:42 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:aea1895b7fd03ef3bc263eef4b6f1dd219fc3286f3ff79495aadb81a88650723`  
		Last Modified: Wed, 08 Mar 2023 05:10:33 GMT  
		Size: 26.1 MB (26140319 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:latest` - linux; arm64 variant v8

```console
$ docker pull ubuntu@sha256:537da24818633b45fcb65e5285a68c3ec1f3db25f5ae5476a7757bc8dfae92a3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.3 MB (27347481 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bab8ce5c00ca3ef91e0d3eb4c6e6d6ec7cffa9574c447fd8d54a8d96e7c1c80e`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 08 Mar 2023 04:32:38 GMT
ARG RELEASE
# Wed, 08 Mar 2023 04:32:38 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 04:32:38 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 04:32:39 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 08 Mar 2023 04:32:40 GMT
ADD file:79b36308bc382d9cae7197b4cecc21430f4e8f3e8bec3547d0f00bcff7681e60 in / 
# Wed, 08 Mar 2023 04:32:41 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:cd741b12a7eaa64357041c2d3f4590c898313a7f8f65cd1577594e6ee03a8c38`  
		Last Modified: Wed, 08 Mar 2023 05:10:27 GMT  
		Size: 27.3 MB (27347481 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:latest` - linux; ppc64le

```console
$ docker pull ubuntu@sha256:f23b7ade9f88f91c8d5932a48b721712ed509a607d9a05cdeae4cd06de09e5f7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.6 MB (34593661 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4220c61b3ab7b82dd3ff3395f9efe2b63e730c3f24284d1519013cf3cda822f8`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 08 Mar 2023 04:39:16 GMT
ARG RELEASE
# Wed, 08 Mar 2023 04:39:16 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 04:39:16 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 04:39:16 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 08 Mar 2023 04:39:20 GMT
ADD file:d7434a52d8d8aa6288e788f6fe7e156f0e11bf9b8275efaf70aab0bfc4d919cf in / 
# Wed, 08 Mar 2023 04:39:20 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:2561b3b559ec9b25bafa07804afa433803291265f7dd847de711224b0f238237`  
		Last Modified: Wed, 08 Mar 2023 05:10:39 GMT  
		Size: 34.6 MB (34593661 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:latest` - linux; s390x

```console
$ docker pull ubuntu@sha256:b351315d950a4da70f19d62f4da5dd7f9a445eb8c8d6851a5b6cdddbdafb13cf
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.0 MB (28015959 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:63ad39053efde0c294433cd8f9709c6d69a36e1f0af4ffbf81c3d261caffb615`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 08 Mar 2023 04:39:24 GMT
ARG RELEASE
# Wed, 08 Mar 2023 04:39:24 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 04:39:24 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 04:39:24 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 08 Mar 2023 04:39:26 GMT
ADD file:630f9865d3d4fd4294d45cac7cbaea83fb549c2e563de454348da964d19fbbba in / 
# Wed, 08 Mar 2023 04:39:26 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:15f635e04e894b7646b4ebca40424ddf244867fc663429ea8b877eca172a7cf1`  
		Last Modified: Wed, 08 Mar 2023 05:10:46 GMT  
		Size: 28.0 MB (28015959 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

## `ubuntu:lunar`

```console
$ docker pull ubuntu@sha256:008c0f6712067722f42f9685476d37b0b7b689e31d66e5787d1920c7ac230849
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
$ docker pull ubuntu@sha256:ffa4bb610fa4c137211199607a5326c5a409b189d3c673cc85a4c65f5757447b
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.8 MB (26761270 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:de432ed6bff895b418712abd3084394e7dd70656b905d6390ffba649c63c64a3`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 14 Mar 2023 18:21:45 GMT
ARG RELEASE
# Tue, 14 Mar 2023 18:21:45 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 14 Mar 2023 18:21:45 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 14 Mar 2023 18:21:45 GMT
LABEL org.opencontainers.image.version=23.04
# Tue, 14 Mar 2023 18:21:47 GMT
ADD file:108000e07d9734743bfe65381248aa7e309283bdb87d8687b7ffe0d697487109 in / 
# Tue, 14 Mar 2023 18:21:47 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:391f30eda8cdf14ab4acf7e6ce5bac054bcc1d98fe5f8789908c6bc739dee216`  
		Last Modified: Tue, 14 Mar 2023 18:47:00 GMT  
		Size: 26.8 MB (26761270 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:lunar` - linux; arm variant v7

```console
$ docker pull ubuntu@sha256:e685540e6030c9b728fa6485ca8e844d824e064c9a790bc54e6e6507974ba42e
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **24.6 MB (24559160 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:28e4ad84aaa1e06e217b7ed880b9bea183f12a02bb5b8408f57855354fbd91c9`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 14 Mar 2023 18:18:28 GMT
ARG RELEASE
# Tue, 14 Mar 2023 18:18:28 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 14 Mar 2023 18:18:28 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 14 Mar 2023 18:18:28 GMT
LABEL org.opencontainers.image.version=23.04
# Tue, 14 Mar 2023 18:18:30 GMT
ADD file:dc39df38ee577fc1ddb753815787f9a90231d34a28c65e14298d136132c8d7d5 in / 
# Tue, 14 Mar 2023 18:18:31 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:7ec8b1962079f6d8d8477e2e227966fcf2e91d26a81735eb5f0411f84cbf8740`  
		Last Modified: Tue, 14 Mar 2023 18:47:12 GMT  
		Size: 24.6 MB (24559160 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:lunar` - linux; arm64 variant v8

```console
$ docker pull ubuntu@sha256:b864a1f0e9f2686fcaa86491f78d38af1b9e8e53e965df39d991a8b685bf7c74
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.0 MB (26007489 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e399e758a4b24fbecd3eed7dbaadf0eb3aa45f2ee4b2c133561693f31008b42b`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 14 Mar 2023 17:38:32 GMT
ARG RELEASE
# Tue, 14 Mar 2023 17:38:32 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 14 Mar 2023 17:38:32 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 14 Mar 2023 17:38:32 GMT
LABEL org.opencontainers.image.version=23.04
# Tue, 14 Mar 2023 17:38:40 GMT
ADD file:2562122b72f2bcdd0678a1bd0836dcbf376a8e33078452497d85ed0cd425391f in / 
# Tue, 14 Mar 2023 17:38:41 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:ff6383e8c55f097496fc03e31f40ad77007ac50d51f9735a1d45789985087387`  
		Last Modified: Tue, 14 Mar 2023 18:47:06 GMT  
		Size: 26.0 MB (26007489 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:lunar` - linux; ppc64le

```console
$ docker pull ubuntu@sha256:8e0b2dedffe81c417dc0860a92ec8520aca6f48b6b3267b18590c1ff4c4f16ea
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.0 MB (30987169 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:26160bb786e079c716ceda59a2a70b6e813f9e43dea7866e98e9edfe8a1cb84f`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 14 Mar 2023 17:31:48 GMT
ARG RELEASE
# Tue, 14 Mar 2023 17:31:48 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 14 Mar 2023 17:31:48 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 14 Mar 2023 17:31:48 GMT
LABEL org.opencontainers.image.version=23.04
# Tue, 14 Mar 2023 17:31:51 GMT
ADD file:586ae3783043b40d20c362128778cbf64404358967d540af0c899067d82744f8 in / 
# Tue, 14 Mar 2023 17:31:52 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:59dbd023a22a72c486e06919c527e79036e5a5b41ca794aafbbd35687256dee7`  
		Last Modified: Tue, 14 Mar 2023 18:47:20 GMT  
		Size: 31.0 MB (30987169 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:lunar` - linux; s390x

```console
$ docker pull ubuntu@sha256:1840997cef13af4d355cf1b5bda18e68073cc6aefe673bd36cb93ea91f3452a2
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.6 MB (25634517 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6d6744e3a8d8d30ea66143d1d2ba080a6cb9a9e1356857de142edfd33ddefb5e`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 14 Mar 2023 17:47:18 GMT
ARG RELEASE
# Tue, 14 Mar 2023 17:47:18 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 14 Mar 2023 17:47:18 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 14 Mar 2023 17:47:18 GMT
LABEL org.opencontainers.image.version=23.04
# Tue, 14 Mar 2023 17:47:20 GMT
ADD file:1ed4a1aa279c8c4fd49f73ed214f53835caecef222778b80716ba71fe60cc7f0 in / 
# Tue, 14 Mar 2023 17:47:20 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:de8d2f62d0190fb3786c431d236f8d6178a12304755c3c13b8c1ff4d6097587f`  
		Last Modified: Tue, 14 Mar 2023 18:47:26 GMT  
		Size: 25.6 MB (25634517 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

## `ubuntu:lunar-20230314`

```console
$ docker pull ubuntu@sha256:008c0f6712067722f42f9685476d37b0b7b689e31d66e5787d1920c7ac230849
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `ubuntu:lunar-20230314` - linux; amd64

```console
$ docker pull ubuntu@sha256:ffa4bb610fa4c137211199607a5326c5a409b189d3c673cc85a4c65f5757447b
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.8 MB (26761270 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:de432ed6bff895b418712abd3084394e7dd70656b905d6390ffba649c63c64a3`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 14 Mar 2023 18:21:45 GMT
ARG RELEASE
# Tue, 14 Mar 2023 18:21:45 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 14 Mar 2023 18:21:45 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 14 Mar 2023 18:21:45 GMT
LABEL org.opencontainers.image.version=23.04
# Tue, 14 Mar 2023 18:21:47 GMT
ADD file:108000e07d9734743bfe65381248aa7e309283bdb87d8687b7ffe0d697487109 in / 
# Tue, 14 Mar 2023 18:21:47 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:391f30eda8cdf14ab4acf7e6ce5bac054bcc1d98fe5f8789908c6bc739dee216`  
		Last Modified: Tue, 14 Mar 2023 18:47:00 GMT  
		Size: 26.8 MB (26761270 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:lunar-20230314` - linux; arm variant v7

```console
$ docker pull ubuntu@sha256:e685540e6030c9b728fa6485ca8e844d824e064c9a790bc54e6e6507974ba42e
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **24.6 MB (24559160 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:28e4ad84aaa1e06e217b7ed880b9bea183f12a02bb5b8408f57855354fbd91c9`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 14 Mar 2023 18:18:28 GMT
ARG RELEASE
# Tue, 14 Mar 2023 18:18:28 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 14 Mar 2023 18:18:28 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 14 Mar 2023 18:18:28 GMT
LABEL org.opencontainers.image.version=23.04
# Tue, 14 Mar 2023 18:18:30 GMT
ADD file:dc39df38ee577fc1ddb753815787f9a90231d34a28c65e14298d136132c8d7d5 in / 
# Tue, 14 Mar 2023 18:18:31 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:7ec8b1962079f6d8d8477e2e227966fcf2e91d26a81735eb5f0411f84cbf8740`  
		Last Modified: Tue, 14 Mar 2023 18:47:12 GMT  
		Size: 24.6 MB (24559160 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:lunar-20230314` - linux; arm64 variant v8

```console
$ docker pull ubuntu@sha256:b864a1f0e9f2686fcaa86491f78d38af1b9e8e53e965df39d991a8b685bf7c74
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.0 MB (26007489 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e399e758a4b24fbecd3eed7dbaadf0eb3aa45f2ee4b2c133561693f31008b42b`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 14 Mar 2023 17:38:32 GMT
ARG RELEASE
# Tue, 14 Mar 2023 17:38:32 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 14 Mar 2023 17:38:32 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 14 Mar 2023 17:38:32 GMT
LABEL org.opencontainers.image.version=23.04
# Tue, 14 Mar 2023 17:38:40 GMT
ADD file:2562122b72f2bcdd0678a1bd0836dcbf376a8e33078452497d85ed0cd425391f in / 
# Tue, 14 Mar 2023 17:38:41 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:ff6383e8c55f097496fc03e31f40ad77007ac50d51f9735a1d45789985087387`  
		Last Modified: Tue, 14 Mar 2023 18:47:06 GMT  
		Size: 26.0 MB (26007489 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:lunar-20230314` - linux; ppc64le

```console
$ docker pull ubuntu@sha256:8e0b2dedffe81c417dc0860a92ec8520aca6f48b6b3267b18590c1ff4c4f16ea
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.0 MB (30987169 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:26160bb786e079c716ceda59a2a70b6e813f9e43dea7866e98e9edfe8a1cb84f`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 14 Mar 2023 17:31:48 GMT
ARG RELEASE
# Tue, 14 Mar 2023 17:31:48 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 14 Mar 2023 17:31:48 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 14 Mar 2023 17:31:48 GMT
LABEL org.opencontainers.image.version=23.04
# Tue, 14 Mar 2023 17:31:51 GMT
ADD file:586ae3783043b40d20c362128778cbf64404358967d540af0c899067d82744f8 in / 
# Tue, 14 Mar 2023 17:31:52 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:59dbd023a22a72c486e06919c527e79036e5a5b41ca794aafbbd35687256dee7`  
		Last Modified: Tue, 14 Mar 2023 18:47:20 GMT  
		Size: 31.0 MB (30987169 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:lunar-20230314` - linux; s390x

```console
$ docker pull ubuntu@sha256:1840997cef13af4d355cf1b5bda18e68073cc6aefe673bd36cb93ea91f3452a2
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.6 MB (25634517 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6d6744e3a8d8d30ea66143d1d2ba080a6cb9a9e1356857de142edfd33ddefb5e`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 14 Mar 2023 17:47:18 GMT
ARG RELEASE
# Tue, 14 Mar 2023 17:47:18 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 14 Mar 2023 17:47:18 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 14 Mar 2023 17:47:18 GMT
LABEL org.opencontainers.image.version=23.04
# Tue, 14 Mar 2023 17:47:20 GMT
ADD file:1ed4a1aa279c8c4fd49f73ed214f53835caecef222778b80716ba71fe60cc7f0 in / 
# Tue, 14 Mar 2023 17:47:20 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:de8d2f62d0190fb3786c431d236f8d6178a12304755c3c13b8c1ff4d6097587f`  
		Last Modified: Tue, 14 Mar 2023 18:47:26 GMT  
		Size: 25.6 MB (25634517 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

## `ubuntu:rolling`

```console
$ docker pull ubuntu@sha256:a82eebb42083a134e009a6b81a7e5d2eecc37112fa8ae40642bd3c5153b7e4f0
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
$ docker pull ubuntu@sha256:8c8f22bacbfba9678edddcc3b6d1e56cce02eff9cbf27ab46116de30cb79a3d6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.7 MB (26695001 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:558d44db75c8f69c29f427cf88e6a71c39320f7607584baa6860f6e4f6121892`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 08 Mar 2023 05:58:05 GMT
ARG RELEASE
# Wed, 08 Mar 2023 05:58:05 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 05:58:05 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 05:58:05 GMT
LABEL org.opencontainers.image.version=22.10
# Wed, 08 Mar 2023 05:58:07 GMT
ADD file:3492508b382c909e968c4d8467b9acbd5f61ed6ca69c8a47241f930d90de7158 in / 
# Wed, 08 Mar 2023 05:58:07 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:5c19388d38e1ea904672812dd0aac505220c9254e2621a1684e0fe29e2dba80e`  
		Last Modified: Wed, 08 Mar 2023 06:38:37 GMT  
		Size: 26.7 MB (26695001 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:rolling` - linux; arm variant v7

```console
$ docker pull ubuntu@sha256:e37c01607a81ee7737f164af67cb5f5f8e1ecbf82c4f5cfe940675b8e8830ee1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.1 MB (25067205 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:94bcbf2021edfcf5671a4872ded2d62d36cd3a86813acc7bc2471fefce3c2ac2`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 08 Mar 2023 05:55:43 GMT
ARG RELEASE
# Wed, 08 Mar 2023 05:55:43 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 05:55:43 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 05:55:43 GMT
LABEL org.opencontainers.image.version=22.10
# Wed, 08 Mar 2023 05:55:49 GMT
ADD file:827330b6c59e67c5d2edd3ceb3492b97865b15f9246f14710f478d12e94d2048 in / 
# Wed, 08 Mar 2023 05:55:49 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:5c09adf37dd1d92aeedd2906b2635d9b7f1eca9f39f51d52f919d26d113c8d35`  
		Last Modified: Wed, 08 Mar 2023 06:38:49 GMT  
		Size: 25.1 MB (25067205 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:rolling` - linux; arm64 variant v8

```console
$ docker pull ubuntu@sha256:2a79f91eb2bb4ffc5d96c58a06fda63550bf94a1a6b2e9ef2f835e52ca8a04ee
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.8 MB (25760037 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:438c48db988d0f48de4461bb2bf49524880c28c5863b1ba5b175a9d7c284b009`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 08 Mar 2023 05:57:57 GMT
ARG RELEASE
# Wed, 08 Mar 2023 05:57:57 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 05:57:57 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 05:57:58 GMT
LABEL org.opencontainers.image.version=22.10
# Wed, 08 Mar 2023 05:57:59 GMT
ADD file:884e00dc91bf6d392fa3d117913cc2534177128322d89137bfb8b2734bc38579 in / 
# Wed, 08 Mar 2023 05:58:00 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:4f720bb411d1d3a6b6c043988c66cdaeee655f968c6eabf7f1ada7ac1529b046`  
		Last Modified: Wed, 08 Mar 2023 06:38:43 GMT  
		Size: 25.8 MB (25760037 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:rolling` - linux; ppc64le

```console
$ docker pull ubuntu@sha256:fec18179ce4b8f8215f04ea75ca752d4c7865d1a06f1d9a3d961927ed2916589
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.1 MB (31114002 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:817a0842655ee55d34c1866729026d8d7fd4de6cc4ea4fcbdaac3cbc1dc10a73`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 08 Mar 2023 05:58:03 GMT
ARG RELEASE
# Wed, 08 Mar 2023 05:58:03 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 05:58:03 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 05:58:03 GMT
LABEL org.opencontainers.image.version=22.10
# Wed, 08 Mar 2023 05:58:06 GMT
ADD file:583061e8201c03de4747860e734200b6c35b449443a1382ad8e8efc6f7e9ea13 in / 
# Wed, 08 Mar 2023 05:58:06 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:e9acd60127e6a1f919659d03fc820b762a3f49f62bae6caafbd919cdbd8e4f7b`  
		Last Modified: Wed, 08 Mar 2023 06:38:55 GMT  
		Size: 31.1 MB (31114002 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:rolling` - linux; s390x

```console
$ docker pull ubuntu@sha256:c69324f895a9152b8a80f9d310710a9d2ef987330d04bc20dbfe23e79e5183bb
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.5 MB (25488878 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4997349fe1813d9306e1ad38084ecc78950e221fe4f75cd9a85e5213139fcd80`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 08 Mar 2023 06:11:04 GMT
ARG RELEASE
# Wed, 08 Mar 2023 06:11:04 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 06:11:04 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 06:11:04 GMT
LABEL org.opencontainers.image.version=22.10
# Wed, 08 Mar 2023 06:11:06 GMT
ADD file:974d67ca1d5bcaacbc707820609d36af0d7ed3ff7179a702a4aa56dcc43f79f3 in / 
# Wed, 08 Mar 2023 06:11:06 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:e7f1a81217015da9b8db635ad002e08952988dc4100cbec474290e8524391920`  
		Last Modified: Wed, 08 Mar 2023 06:39:01 GMT  
		Size: 25.5 MB (25488878 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
