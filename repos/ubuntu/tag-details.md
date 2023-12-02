<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `ubuntu`

-	[`ubuntu:20.04`](#ubuntu2004)
-	[`ubuntu:22.04`](#ubuntu2204)
-	[`ubuntu:23.04`](#ubuntu2304)
-	[`ubuntu:23.10`](#ubuntu2310)
-	[`ubuntu:24.04`](#ubuntu2404)
-	[`ubuntu:devel`](#ubuntudevel)
-	[`ubuntu:focal`](#ubuntufocal)
-	[`ubuntu:focal-20231128`](#ubuntufocal-20231128)
-	[`ubuntu:jammy`](#ubuntujammy)
-	[`ubuntu:jammy-20231128`](#ubuntujammy-20231128)
-	[`ubuntu:latest`](#ubuntulatest)
-	[`ubuntu:lunar`](#ubuntulunar)
-	[`ubuntu:lunar-20231128`](#ubuntulunar-20231128)
-	[`ubuntu:mantic`](#ubuntumantic)
-	[`ubuntu:mantic-20231128`](#ubuntumantic-20231128)
-	[`ubuntu:noble`](#ubuntunoble)
-	[`ubuntu:noble-20231126.1`](#ubuntunoble-202311261)
-	[`ubuntu:rolling`](#ubunturolling)

## `ubuntu:20.04`

```console
$ docker pull ubuntu@sha256:8517db592129015f59735a921fa1780d2775ba7dc4353e306d344a6308480154
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
$ docker pull ubuntu@sha256:fe8a36445d3d850960d6a24554f2cf4e19d82ba1e611e3e8713bd7b76989623d
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.5 MB (27512563 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:83a4bf3bb050e11e0f3bfdcfaff38eeb1dd851b7a362d930cd590dd97b3b1687`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 28 Nov 2023 05:17:39 GMT
ARG RELEASE
# Tue, 28 Nov 2023 05:17:39 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 28 Nov 2023 05:17:39 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 28 Nov 2023 05:17:39 GMT
LABEL org.opencontainers.image.version=20.04
# Tue, 28 Nov 2023 05:17:41 GMT
ADD file:9169bb1d6ef21313aed17e924538fee03d858460ae6b05e01968457dfc043bd7 in / 
# Tue, 28 Nov 2023 05:17:41 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:25ad149ed3cff49ddb57ceb4418377f63c897198de1f9de7a24506397822de3e`  
		Last Modified: Tue, 28 Nov 2023 05:37:19 GMT  
		Size: 27.5 MB (27512563 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:20.04` - linux; arm variant v7

```console
$ docker pull ubuntu@sha256:06e174da2c1a4cd683a888d933a235407a02f2d98fedb49c34601b293fc5e36e
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.6 MB (23612914 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4eba8b8e77a0ca1c3d8315507ef4e67d817fb199a4cdbc603a0e06fb1b9f78ad`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 03 Oct 2023 10:47:59 GMT
ARG RELEASE
# Tue, 03 Oct 2023 10:47:59 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 03 Oct 2023 10:47:59 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 03 Oct 2023 10:47:59 GMT
LABEL org.opencontainers.image.version=20.04
# Tue, 03 Oct 2023 10:48:06 GMT
ADD file:8dffbfada6e0bebb2858525182aef87ac2cbd88c624f32696ec2cb947e71a4f3 in / 
# Tue, 03 Oct 2023 10:48:07 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:a50255c0017d09ab86514148fe36d006a4ad9a46633b82efd4b0233a9c9082e8`  
		Last Modified: Tue, 03 Oct 2023 11:16:56 GMT  
		Size: 23.6 MB (23612914 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:20.04` - linux; arm64 variant v8

```console
$ docker pull ubuntu@sha256:a80d11b67ef30474bcccab048020ee25aee659c4caaca70794867deba5d392b6
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.0 MB (25973940 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0341906bdafc976cd73b05ea0e3df2e4884c6b6816197a2ffbd2367061c19acf`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 03 Oct 2023 11:04:09 GMT
ARG RELEASE
# Tue, 03 Oct 2023 11:04:09 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 03 Oct 2023 11:04:09 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 03 Oct 2023 11:04:10 GMT
LABEL org.opencontainers.image.version=20.04
# Tue, 03 Oct 2023 11:04:16 GMT
ADD file:f70cc2610ea8fcd25e6e9ae727eb9345d5b7198102f6a6d8e458ab8f99efefc3 in / 
# Tue, 03 Oct 2023 11:04:17 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:915eebb74587f0e5d3919cb77720c143be9a85a8d2d5cd44675d84c8c3a2b74a`  
		Last Modified: Tue, 03 Oct 2023 11:16:49 GMT  
		Size: 26.0 MB (25973940 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:20.04` - linux; ppc64le

```console
$ docker pull ubuntu@sha256:d85c88c0c9d7d331683e7f9d96db67946ecd217b57e5e477d1f4e527578ac026
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.1 MB (32070731 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:673ae00b2a1a4c999ed047c4a07731716987185e46132b80a58bb9cdb1f7305d`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 03 Oct 2023 11:03:52 GMT
ARG RELEASE
# Tue, 03 Oct 2023 11:03:53 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 03 Oct 2023 11:03:53 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 03 Oct 2023 11:03:53 GMT
LABEL org.opencontainers.image.version=20.04
# Tue, 03 Oct 2023 11:03:56 GMT
ADD file:ba2394102af0c0584d39af9ec5dd4fa13286293b4607ac7cb9e16d7a2781eef2 in / 
# Tue, 03 Oct 2023 11:03:56 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:f1c4ab65f666dae98ad8e32b78770e1c705b2a66bd87bd84de1371ecc6e45b22`  
		Last Modified: Tue, 03 Oct 2023 11:17:02 GMT  
		Size: 32.1 MB (32070731 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:20.04` - linux; s390x

```console
$ docker pull ubuntu@sha256:4bab3d12db59c8f2427dbec33d65e2e18d15562effcc0a021d624b1b7385a612
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.4 MB (26351014 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:173c65385684c3aebccf05f7e47832915c6265293dfe5aac55cee5cbacdb724d`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 03 Oct 2023 11:03:23 GMT
ARG RELEASE
# Tue, 03 Oct 2023 11:03:23 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 03 Oct 2023 11:03:23 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 03 Oct 2023 11:03:23 GMT
LABEL org.opencontainers.image.version=20.04
# Tue, 03 Oct 2023 11:03:25 GMT
ADD file:1d9be1bf43c126d53bda18c06d12757c021da97c0c9d3a9c9f56df17312095b8 in / 
# Tue, 03 Oct 2023 11:03:25 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:6a4bfe2c3513e065ca2fbf3e4a1c954b145512c0e7ae2d00b2dac3a5909bed7c`  
		Last Modified: Tue, 03 Oct 2023 11:17:08 GMT  
		Size: 26.4 MB (26351014 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

## `ubuntu:22.04`

```console
$ docker pull ubuntu@sha256:90f3997e3e5f82097fa3046152944772876ac338365954f693b9e1bd3dd3c280
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
$ docker pull ubuntu@sha256:149d67e29f765f4db62aa52161009e99e389544e25a8f43c8c89d4a445a7ca37
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.5 MB (29547417 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b6548eacb0639263e9d8abfee48f8ac8b327102a05335b67572f715c580a968e`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 01 Dec 2023 07:49:48 GMT
ARG RELEASE
# Fri, 01 Dec 2023 07:49:48 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Fri, 01 Dec 2023 07:49:48 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Fri, 01 Dec 2023 07:49:48 GMT
LABEL org.opencontainers.image.version=22.04
# Fri, 01 Dec 2023 07:49:50 GMT
ADD file:36d444e2cede3abe58191dcf28890b874c0908f5259bf7e8855338555701c4c5 in / 
# Fri, 01 Dec 2023 07:49:50 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:5e8117c0bd28aecad06f7e76d4d3b64734d59c1a0a44541d18060cd8fba30c50`  
		Last Modified: Fri, 01 Dec 2023 08:21:32 GMT  
		Size: 29.5 MB (29547417 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:22.04` - linux; arm variant v7

```console
$ docker pull ubuntu@sha256:212b9f426e7be12bf9a80b65e1a14fc39e319cff3a7857772b21c02f1eaff610
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.6 MB (26629612 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bb3f9d425ffe4e459ab4cfc7b6f32c504d3f86b0fcb2a1b58d7646ab045ca4c0`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 05 Oct 2023 07:34:56 GMT
ARG RELEASE
# Thu, 05 Oct 2023 07:34:56 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 05 Oct 2023 07:34:56 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 05 Oct 2023 07:34:56 GMT
LABEL org.opencontainers.image.version=22.04
# Thu, 05 Oct 2023 07:35:01 GMT
ADD file:4b9d52f97ed5796b14772a84c1e7213402430d32312d15ae04a2dcc9fc485a52 in / 
# Thu, 05 Oct 2023 07:35:02 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:4091a3a7d6aa711dc0e0bbacfd3546df44ca257c300de1ad00fbdc95e218f7bd`  
		Last Modified: Thu, 05 Oct 2023 07:43:39 GMT  
		Size: 26.6 MB (26629612 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:22.04` - linux; arm64 variant v8

```console
$ docker pull ubuntu@sha256:02410fbfad7f2842cce3cf7655828424f4f7f6b5105b0016e24f1676f3bd15f5
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.4 MB (27351048 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e343402cadef796b4f12c2ee20b7346978a42a8d95516619c36c6397c4b0c766`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 05 Oct 2023 07:32:20 GMT
ARG RELEASE
# Thu, 05 Oct 2023 07:32:21 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 05 Oct 2023 07:32:21 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 05 Oct 2023 07:32:21 GMT
LABEL org.opencontainers.image.version=22.04
# Thu, 05 Oct 2023 07:32:22 GMT
ADD file:f8594e26831508c318e42c8dfd9942041031087b8de1bf3fec11fd75b8b30fd4 in / 
# Thu, 05 Oct 2023 07:32:22 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:bfbe77e41a78ee38147c5761aa8bc896d9f6e1e648b23468f294065ffe03c107`  
		Last Modified: Thu, 05 Oct 2023 07:43:33 GMT  
		Size: 27.4 MB (27351048 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:22.04` - linux; ppc64le

```console
$ docker pull ubuntu@sha256:b5759015a02040b956d02fb5cd8150ae0fdc3db0fd15af76dd006f6833bc9ab4
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.6 MB (34555968 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e7a609d38c5a2e47b65cf2a2ff61e6d2d5db4be6eb7578f40c4a672efc1f0cd0`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 05 Oct 2023 07:34:18 GMT
ARG RELEASE
# Thu, 05 Oct 2023 07:34:19 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 05 Oct 2023 07:34:19 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 05 Oct 2023 07:34:19 GMT
LABEL org.opencontainers.image.version=22.04
# Thu, 05 Oct 2023 07:34:22 GMT
ADD file:595ff761b2778bdc6bb59cbe8ce51c4a247e0f279ccd59a17b5be6cdeac0b4d2 in / 
# Thu, 05 Oct 2023 07:34:22 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:90496cba4a92b0bf6a8307bab5dd30100905ac891d478aa27771408328244c33`  
		Last Modified: Thu, 05 Oct 2023 07:43:45 GMT  
		Size: 34.6 MB (34555968 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:22.04` - linux; s390x

```console
$ docker pull ubuntu@sha256:ffa841e85005182836d91f7abd24ec081f3910716096955dcc1874b8017b96c9
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.0 MB (28023918 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e27f4324041cd007fd9a3e77aafafa96b00de774f3b241442e8f39457b00b46d`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 05 Oct 2023 07:29:34 GMT
ARG RELEASE
# Thu, 05 Oct 2023 07:29:34 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 05 Oct 2023 07:29:34 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 05 Oct 2023 07:29:34 GMT
LABEL org.opencontainers.image.version=22.04
# Thu, 05 Oct 2023 07:29:36 GMT
ADD file:d165475f8f027ab758a463da57c8c29f5d302f0a87a475ac68fdfae30005c7ac in / 
# Thu, 05 Oct 2023 07:29:36 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:0ffe28a7c279dfdb86b23c0d22d37e89442a6d771fbded124aee76b24119c2c1`  
		Last Modified: Thu, 05 Oct 2023 07:43:51 GMT  
		Size: 28.0 MB (28023918 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

## `ubuntu:23.04`

```console
$ docker pull ubuntu@sha256:852d8cab9db2e8401402528f1d845d097e672fb28a09770aa0a4278a1911b70d
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
$ docker pull ubuntu@sha256:ea1285dffce8a938ef356908d1be741da594310c8dced79b870d66808cb12b0f
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.9 MB (26886018 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f4cdeba72b994748f5eb1f525a70a9cc553b66037ec37e23645fbf3f0f5c160d`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 28 Nov 2023 09:02:17 GMT
ARG RELEASE
# Tue, 28 Nov 2023 09:02:18 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 28 Nov 2023 09:02:18 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 28 Nov 2023 09:02:18 GMT
LABEL org.opencontainers.image.version=23.04
# Tue, 28 Nov 2023 09:02:19 GMT
ADD file:9627edfd854222fb9117755e0e89c54a01ba3477dffb8137693b12c586d970b8 in / 
# Tue, 28 Nov 2023 09:02:19 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:6360b371721185fefbbad6763ab745900f1b2f7714570234473232dd575fc07f`  
		Last Modified: Tue, 28 Nov 2023 09:27:24 GMT  
		Size: 26.9 MB (26886018 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:23.04` - linux; arm variant v7

```console
$ docker pull ubuntu@sha256:4dc1dd258d16171c6cd696ed5420402319d7cabe638b176b471495e94373f2a9
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **24.6 MB (24629439 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d83502f31cce9655561356390e34e8d506e888f6ce4743a8400bfa765f6eedb8`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 04 Oct 2023 12:25:21 GMT
ARG RELEASE
# Wed, 04 Oct 2023 12:25:21 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 04 Oct 2023 12:25:21 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 04 Oct 2023 12:25:22 GMT
LABEL org.opencontainers.image.version=23.04
# Wed, 04 Oct 2023 12:25:24 GMT
ADD file:b92305119eab5dd3dfb00f4d83cd84e00c8ae57143739329da5a19aeda55be4e in / 
# Wed, 04 Oct 2023 12:25:24 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:725335f54d3eb8903e713867d9f04db29fbc8835da3539fd3898faa22eaf016e`  
		Last Modified: Wed, 04 Oct 2023 12:33:24 GMT  
		Size: 24.6 MB (24629439 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:23.04` - linux; arm64 variant v8

```console
$ docker pull ubuntu@sha256:aa2be6baa498ab5862770bbc08cf00a058154cb257e41dca6ef8b7f7aebe22f8
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.1 MB (26065969 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4783be26912a96818aa1c9468ea8acb5eff2608697f62deff67048595a613145`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 04 Oct 2023 12:23:52 GMT
ARG RELEASE
# Wed, 04 Oct 2023 12:23:52 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 04 Oct 2023 12:23:52 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 04 Oct 2023 12:23:52 GMT
LABEL org.opencontainers.image.version=23.04
# Wed, 04 Oct 2023 12:23:53 GMT
ADD file:c9b1098bc90ac9b887c3bffdffbcff0c32f32e48df9a673041e3aa796296e69b in / 
# Wed, 04 Oct 2023 12:23:54 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:89e6336dd9e04a0993754adca328bf88d988540bb95cff284667037dd50f79eb`  
		Last Modified: Wed, 04 Oct 2023 12:33:17 GMT  
		Size: 26.1 MB (26065969 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:23.04` - linux; ppc64le

```console
$ docker pull ubuntu@sha256:2d697e1fc26340ae1a77a08397f53f978a6966d3c8a3cf195ee0870ca6e7dc2a
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.9 MB (30905941 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6651a10a7ea6479a915882811fa23c286c9baabb6ea68a11e48c3235246b574e`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 04 Oct 2023 12:08:54 GMT
ARG RELEASE
# Wed, 04 Oct 2023 12:08:54 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 04 Oct 2023 12:08:55 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 04 Oct 2023 12:08:55 GMT
LABEL org.opencontainers.image.version=23.04
# Wed, 04 Oct 2023 12:08:57 GMT
ADD file:24bc2f22a395e93a2ebbcfc45da8e5fc7f08e7c03cdc985c997300643d0310ec in / 
# Wed, 04 Oct 2023 12:08:58 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:fafd77e1a2b2b77f4b648372d147a2d31af161695aa89bed56883733707bd39f`  
		Last Modified: Wed, 04 Oct 2023 12:33:31 GMT  
		Size: 30.9 MB (30905941 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:23.04` - linux; s390x

```console
$ docker pull ubuntu@sha256:e54d7ce369ad0b993654f624153bbf76a3ef547ed0dc2e14ba0a60d199077b0e
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.7 MB (25692995 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ab36c0e39cab522c65337f5bfeaaf36ce62c510ca07b09d17bea00fe80bfed55`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 04 Oct 2023 12:26:55 GMT
ARG RELEASE
# Wed, 04 Oct 2023 12:26:55 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 04 Oct 2023 12:26:55 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 04 Oct 2023 12:26:55 GMT
LABEL org.opencontainers.image.version=23.04
# Wed, 04 Oct 2023 12:26:57 GMT
ADD file:553d1c48ed98fa8bd575a7a645019079304c101dd6e06e82591a25440fe1a9b8 in / 
# Wed, 04 Oct 2023 12:26:57 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:8333843c4e8c11c41362709d3852d288b9deee48dfdd0014810ce4d3ef224714`  
		Last Modified: Wed, 04 Oct 2023 12:33:37 GMT  
		Size: 25.7 MB (25692995 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

## `ubuntu:23.10`

```console
$ docker pull ubuntu@sha256:e82db07bf46c1da56547b5fb31c0200f4a41e0f0ea9cb7970b3ca3e8720d8d6c
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `ubuntu:23.10` - linux; amd64

```console
$ docker pull ubuntu@sha256:8d093e0651575a6437cc4a3d561f892a345d263aeac6156ef378fe6a4ccabd4c
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.3 MB (27273553 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:483a94112583ff9c6d0a7b67348fc3b0ee5bbf104a86a9e24585c9ad1028fd25`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 30 Nov 2023 17:54:17 GMT
ARG RELEASE
# Thu, 30 Nov 2023 17:54:17 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 30 Nov 2023 17:54:17 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 30 Nov 2023 17:54:17 GMT
LABEL org.opencontainers.image.version=23.10
# Thu, 30 Nov 2023 17:54:19 GMT
ADD file:5430e0b4ea856c760b6e2b88e8c2cd2d49704ed2f3c53ae34c10750a608d40ec in / 
# Thu, 30 Nov 2023 17:54:19 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:767829bcf202e4fa7e777f29d390307e29ac437f131685a1ff1293d44705ca23`  
		Last Modified: Thu, 30 Nov 2023 18:06:39 GMT  
		Size: 27.3 MB (27273553 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:23.10` - linux; arm variant v7

```console
$ docker pull ubuntu@sha256:2a465a4c4831c57977b6646e481f504061294f1bf1ae1b99fb5d93c67b8a471a
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.2 MB (25201383 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bc753c284b47a7a5ff3ec2e926551ba95dc6c9072415649cb13a9cdff503dc04`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 11 Oct 2023 18:02:33 GMT
ARG RELEASE
# Wed, 11 Oct 2023 18:02:33 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 11 Oct 2023 18:02:34 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 11 Oct 2023 18:02:34 GMT
LABEL org.opencontainers.image.version=23.10
# Wed, 11 Oct 2023 18:02:39 GMT
ADD file:1be1311acbd557f7769fb5c1913ef56305431e7547f96c20ac36284fdd926223 in / 
# Wed, 11 Oct 2023 18:02:39 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:8761b0d436cd2e1ff47496b7cc353cf0b49347ffc92b070c31a5cf5431041614`  
		Last Modified: Wed, 11 Oct 2023 18:18:00 GMT  
		Size: 25.2 MB (25201383 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:23.10` - linux; arm64 variant v8

```console
$ docker pull ubuntu@sha256:7708743264cbb7f6cf7fc13e915faece45a6cdda455748bc55e58e8de3d27b63
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.4 MB (26379954 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3f9cf3a31fbf871322b774402c7c25b800d0e93c222d5a44339f2d3a99dede82`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 11 Oct 2023 18:03:02 GMT
ARG RELEASE
# Wed, 11 Oct 2023 18:03:02 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 11 Oct 2023 18:03:02 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 11 Oct 2023 18:03:02 GMT
LABEL org.opencontainers.image.version=23.10
# Wed, 11 Oct 2023 18:03:10 GMT
ADD file:9e750ebbbf7e47a121d153e6699006776ea61b04b6c8e31556600483a020f617 in / 
# Wed, 11 Oct 2023 18:03:10 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:f906b88252effff97383eeb7dd4d265f3f31a54aa3833dd349cf8c4a35fbdbe9`  
		Last Modified: Wed, 11 Oct 2023 18:17:54 GMT  
		Size: 26.4 MB (26379954 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:23.10` - linux; ppc64le

```console
$ docker pull ubuntu@sha256:347a278b913b988b85442a3e187001edfe854da3ed499f45782d4a714f08632f
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.3 MB (31340704 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:96fb712785eb8f8fe4cdc47a6bb3bd8014c2b376c684dd430b32f81e786cdd5e`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 11 Oct 2023 18:06:00 GMT
ARG RELEASE
# Wed, 11 Oct 2023 18:06:00 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 11 Oct 2023 18:06:00 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 11 Oct 2023 18:06:00 GMT
LABEL org.opencontainers.image.version=23.10
# Wed, 11 Oct 2023 18:06:03 GMT
ADD file:a18be8add7eb60493b13d2aac8d624230297bd15be033756795582dc07cb04bb in / 
# Wed, 11 Oct 2023 18:06:03 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:6e4ddce09953092c8c6052d38bc7c2044237f1337f42f1f86edab6718af804ea`  
		Last Modified: Wed, 11 Oct 2023 18:18:11 GMT  
		Size: 31.3 MB (31340704 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:23.10` - linux; s390x

```console
$ docker pull ubuntu@sha256:f2e6e56781fb1122ffcdc449f44cb48f8a1279e0baf318582f274a1c44c3b64e
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.1 MB (27069339 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b6598907abce49b9b4f06fea395b2ed375f2bf7fad9b484729cc1b313b2b6109`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 11 Oct 2023 18:03:34 GMT
ARG RELEASE
# Wed, 11 Oct 2023 18:03:34 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 11 Oct 2023 18:03:34 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 11 Oct 2023 18:03:34 GMT
LABEL org.opencontainers.image.version=23.10
# Wed, 11 Oct 2023 18:03:36 GMT
ADD file:8ceb0028af8276b03b6c88b19445f30165a41791919c756e1434da6ded4387db in / 
# Wed, 11 Oct 2023 18:03:36 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:5ef15690269b5b1e6f9795320a2a15f009506ead422509007e5cc08858b1c41e`  
		Last Modified: Wed, 11 Oct 2023 18:18:18 GMT  
		Size: 27.1 MB (27069339 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

## `ubuntu:24.04`

```console
$ docker pull ubuntu@sha256:5cead7e5f0888b84ea7bef10ce29f17d582385b0f468ba6b418f8d3ba3eba6f6
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 1
	-	linux; amd64

### `ubuntu:24.04` - linux; amd64

```console
$ docker pull ubuntu@sha256:ef2b3c979842614a9537785f2dcc5e93a977fa50dc567c42a7d4f5ea6470fec0
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.2 MB (27213697 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bfaf276bdd215773746bde9489a88d063b98584b8a650272c037da7be94941a6`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 27 Nov 2023 11:09:34 GMT
ARG RELEASE
# Mon, 27 Nov 2023 11:09:34 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 27 Nov 2023 11:09:34 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 27 Nov 2023 11:09:34 GMT
LABEL org.opencontainers.image.version=24.04
# Mon, 27 Nov 2023 11:09:35 GMT
ADD file:b2f5aa693e38f0ebe3e4d26ded8f957b4eb6f75c8360340cfcdeee25bf1b1b40 in / 
# Mon, 27 Nov 2023 11:09:36 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:62a1d607dcd86fd912d7d1448a129970b9c35f5506fbc48f8fea327ec9706b14`  
		Last Modified: Mon, 27 Nov 2023 11:15:40 GMT  
		Size: 27.2 MB (27213697 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

## `ubuntu:devel`

```console
$ docker pull ubuntu@sha256:4f8406587f83a5b4f120e75b11b8a2d017961422dbd249c1e9f39315e5939b41
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
$ docker pull ubuntu@sha256:ef2b3c979842614a9537785f2dcc5e93a977fa50dc567c42a7d4f5ea6470fec0
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.2 MB (27213697 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bfaf276bdd215773746bde9489a88d063b98584b8a650272c037da7be94941a6`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 27 Nov 2023 11:09:34 GMT
ARG RELEASE
# Mon, 27 Nov 2023 11:09:34 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 27 Nov 2023 11:09:34 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 27 Nov 2023 11:09:34 GMT
LABEL org.opencontainers.image.version=24.04
# Mon, 27 Nov 2023 11:09:35 GMT
ADD file:b2f5aa693e38f0ebe3e4d26ded8f957b4eb6f75c8360340cfcdeee25bf1b1b40 in / 
# Mon, 27 Nov 2023 11:09:36 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:62a1d607dcd86fd912d7d1448a129970b9c35f5506fbc48f8fea327ec9706b14`  
		Last Modified: Mon, 27 Nov 2023 11:15:40 GMT  
		Size: 27.2 MB (27213697 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:devel` - linux; arm variant v7

```console
$ docker pull ubuntu@sha256:832381cafc44879857f084dd780d246e2afc077bb9f97cc76d02665b50a7b51b
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.2 MB (25244973 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0e05e891c9b4d59dea3e056be161095328b7b723250ac89b69e4178a45e894ad`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 26 Sep 2023 05:05:03 GMT
ARG RELEASE
# Tue, 26 Sep 2023 05:05:03 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 26 Sep 2023 05:05:04 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 26 Sep 2023 05:05:04 GMT
LABEL org.opencontainers.image.version=23.10
# Tue, 26 Sep 2023 05:05:08 GMT
ADD file:512405a66f1049a7237c67d9d5776db7f41d5991eceec535260f4d3b7f19e65d in / 
# Tue, 26 Sep 2023 05:05:09 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:956aaffe9fe2861fc716bca41f30a50ff2eb645844bc74edb8b90428a5ef3637`  
		Last Modified: Tue, 26 Sep 2023 05:34:08 GMT  
		Size: 25.2 MB (25244973 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:devel` - linux; arm64 variant v8

```console
$ docker pull ubuntu@sha256:bb9a61edbd6cd4f0b8458daa9a78bc09ff7ffe638e7da0a85dc28a5b6c26adb2
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.4 MB (26356283 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:461b48f7d9e026c91692982d4ad80e66be3245f28c14eebf5e1c2fd88c95bbe9`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 26 Sep 2023 05:06:27 GMT
ARG RELEASE
# Tue, 26 Sep 2023 05:06:27 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 26 Sep 2023 05:06:27 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 26 Sep 2023 05:06:27 GMT
LABEL org.opencontainers.image.version=23.10
# Tue, 26 Sep 2023 05:06:30 GMT
ADD file:0dbbd4de9483bc32897d525742b94aa13ebd3a6aac7f1844d94d7f4536b2bfb8 in / 
# Tue, 26 Sep 2023 05:06:30 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:afcf80ae17bcd3e5b46853b0fd5d9358fc62ae2b878d7ccb081bd357330cd0aa`  
		Last Modified: Tue, 26 Sep 2023 05:34:02 GMT  
		Size: 26.4 MB (26356283 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:devel` - linux; ppc64le

```console
$ docker pull ubuntu@sha256:7b532d2ce398e717ab17c9280bfac4f8cc34e8104313149c6891f9f1ed3648c1
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.3 MB (31341680 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3c9cdbbf45d488137b78c5d4e544935a5a2dd90921911c5c2ebc35b3453cf223`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 26 Sep 2023 04:52:53 GMT
ARG RELEASE
# Tue, 26 Sep 2023 04:52:53 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 26 Sep 2023 04:52:53 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 26 Sep 2023 04:52:54 GMT
LABEL org.opencontainers.image.version=23.10
# Tue, 26 Sep 2023 04:52:56 GMT
ADD file:cbeb7f814c9eebdbdc6b8e10fb87ba8334b3f6203ceb166c48f6d7492ab07c4e in / 
# Tue, 26 Sep 2023 04:52:57 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:3261179759b520c84edfab6a5842534e3552b99a5f71b1e44ccbd6017eab30b5`  
		Last Modified: Tue, 26 Sep 2023 05:34:15 GMT  
		Size: 31.3 MB (31341680 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:devel` - linux; s390x

```console
$ docker pull ubuntu@sha256:a353c527eb5233fdfc2ad112c7897cce7da6ac28b24d3aaa8f441f27ddf613c9
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.1 MB (27072390 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:12eca28f81d0bd51084742dc133e32c215a83739fc5603306f1ad774311dc6ba`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 26 Sep 2023 04:58:19 GMT
ARG RELEASE
# Tue, 26 Sep 2023 04:58:19 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 26 Sep 2023 04:58:19 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 26 Sep 2023 04:58:19 GMT
LABEL org.opencontainers.image.version=23.10
# Tue, 26 Sep 2023 04:58:21 GMT
ADD file:e86e9b7546a97fa45e9c726cc317a624a7f94b0bd6dd413d89946ff778b18c77 in / 
# Tue, 26 Sep 2023 04:58:21 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:56312385d597227d0c1232049609586ed3412b04e6ec96c5f6626f5f50f438fe`  
		Last Modified: Tue, 26 Sep 2023 05:34:22 GMT  
		Size: 27.1 MB (27072390 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

## `ubuntu:focal`

```console
$ docker pull ubuntu@sha256:8517db592129015f59735a921fa1780d2775ba7dc4353e306d344a6308480154
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
$ docker pull ubuntu@sha256:fe8a36445d3d850960d6a24554f2cf4e19d82ba1e611e3e8713bd7b76989623d
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.5 MB (27512563 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:83a4bf3bb050e11e0f3bfdcfaff38eeb1dd851b7a362d930cd590dd97b3b1687`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 28 Nov 2023 05:17:39 GMT
ARG RELEASE
# Tue, 28 Nov 2023 05:17:39 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 28 Nov 2023 05:17:39 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 28 Nov 2023 05:17:39 GMT
LABEL org.opencontainers.image.version=20.04
# Tue, 28 Nov 2023 05:17:41 GMT
ADD file:9169bb1d6ef21313aed17e924538fee03d858460ae6b05e01968457dfc043bd7 in / 
# Tue, 28 Nov 2023 05:17:41 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:25ad149ed3cff49ddb57ceb4418377f63c897198de1f9de7a24506397822de3e`  
		Last Modified: Tue, 28 Nov 2023 05:37:19 GMT  
		Size: 27.5 MB (27512563 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:focal` - linux; arm variant v7

```console
$ docker pull ubuntu@sha256:06e174da2c1a4cd683a888d933a235407a02f2d98fedb49c34601b293fc5e36e
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.6 MB (23612914 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4eba8b8e77a0ca1c3d8315507ef4e67d817fb199a4cdbc603a0e06fb1b9f78ad`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 03 Oct 2023 10:47:59 GMT
ARG RELEASE
# Tue, 03 Oct 2023 10:47:59 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 03 Oct 2023 10:47:59 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 03 Oct 2023 10:47:59 GMT
LABEL org.opencontainers.image.version=20.04
# Tue, 03 Oct 2023 10:48:06 GMT
ADD file:8dffbfada6e0bebb2858525182aef87ac2cbd88c624f32696ec2cb947e71a4f3 in / 
# Tue, 03 Oct 2023 10:48:07 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:a50255c0017d09ab86514148fe36d006a4ad9a46633b82efd4b0233a9c9082e8`  
		Last Modified: Tue, 03 Oct 2023 11:16:56 GMT  
		Size: 23.6 MB (23612914 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:focal` - linux; arm64 variant v8

```console
$ docker pull ubuntu@sha256:a80d11b67ef30474bcccab048020ee25aee659c4caaca70794867deba5d392b6
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.0 MB (25973940 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0341906bdafc976cd73b05ea0e3df2e4884c6b6816197a2ffbd2367061c19acf`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 03 Oct 2023 11:04:09 GMT
ARG RELEASE
# Tue, 03 Oct 2023 11:04:09 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 03 Oct 2023 11:04:09 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 03 Oct 2023 11:04:10 GMT
LABEL org.opencontainers.image.version=20.04
# Tue, 03 Oct 2023 11:04:16 GMT
ADD file:f70cc2610ea8fcd25e6e9ae727eb9345d5b7198102f6a6d8e458ab8f99efefc3 in / 
# Tue, 03 Oct 2023 11:04:17 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:915eebb74587f0e5d3919cb77720c143be9a85a8d2d5cd44675d84c8c3a2b74a`  
		Last Modified: Tue, 03 Oct 2023 11:16:49 GMT  
		Size: 26.0 MB (25973940 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:focal` - linux; ppc64le

```console
$ docker pull ubuntu@sha256:d85c88c0c9d7d331683e7f9d96db67946ecd217b57e5e477d1f4e527578ac026
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.1 MB (32070731 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:673ae00b2a1a4c999ed047c4a07731716987185e46132b80a58bb9cdb1f7305d`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 03 Oct 2023 11:03:52 GMT
ARG RELEASE
# Tue, 03 Oct 2023 11:03:53 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 03 Oct 2023 11:03:53 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 03 Oct 2023 11:03:53 GMT
LABEL org.opencontainers.image.version=20.04
# Tue, 03 Oct 2023 11:03:56 GMT
ADD file:ba2394102af0c0584d39af9ec5dd4fa13286293b4607ac7cb9e16d7a2781eef2 in / 
# Tue, 03 Oct 2023 11:03:56 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:f1c4ab65f666dae98ad8e32b78770e1c705b2a66bd87bd84de1371ecc6e45b22`  
		Last Modified: Tue, 03 Oct 2023 11:17:02 GMT  
		Size: 32.1 MB (32070731 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:focal` - linux; s390x

```console
$ docker pull ubuntu@sha256:4bab3d12db59c8f2427dbec33d65e2e18d15562effcc0a021d624b1b7385a612
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.4 MB (26351014 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:173c65385684c3aebccf05f7e47832915c6265293dfe5aac55cee5cbacdb724d`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 03 Oct 2023 11:03:23 GMT
ARG RELEASE
# Tue, 03 Oct 2023 11:03:23 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 03 Oct 2023 11:03:23 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 03 Oct 2023 11:03:23 GMT
LABEL org.opencontainers.image.version=20.04
# Tue, 03 Oct 2023 11:03:25 GMT
ADD file:1d9be1bf43c126d53bda18c06d12757c021da97c0c9d3a9c9f56df17312095b8 in / 
# Tue, 03 Oct 2023 11:03:25 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:6a4bfe2c3513e065ca2fbf3e4a1c954b145512c0e7ae2d00b2dac3a5909bed7c`  
		Last Modified: Tue, 03 Oct 2023 11:17:08 GMT  
		Size: 26.4 MB (26351014 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

## `ubuntu:focal-20231128`

```console
$ docker pull ubuntu@sha256:518a26342fa9736032c076369eb13203d8ee3b21a255d0af272cd316cefa687a
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 1
	-	linux; amd64

### `ubuntu:focal-20231128` - linux; amd64

```console
$ docker pull ubuntu@sha256:fe8a36445d3d850960d6a24554f2cf4e19d82ba1e611e3e8713bd7b76989623d
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.5 MB (27512563 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:83a4bf3bb050e11e0f3bfdcfaff38eeb1dd851b7a362d930cd590dd97b3b1687`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 28 Nov 2023 05:17:39 GMT
ARG RELEASE
# Tue, 28 Nov 2023 05:17:39 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 28 Nov 2023 05:17:39 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 28 Nov 2023 05:17:39 GMT
LABEL org.opencontainers.image.version=20.04
# Tue, 28 Nov 2023 05:17:41 GMT
ADD file:9169bb1d6ef21313aed17e924538fee03d858460ae6b05e01968457dfc043bd7 in / 
# Tue, 28 Nov 2023 05:17:41 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:25ad149ed3cff49ddb57ceb4418377f63c897198de1f9de7a24506397822de3e`  
		Last Modified: Tue, 28 Nov 2023 05:37:19 GMT  
		Size: 27.5 MB (27512563 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

## `ubuntu:jammy`

```console
$ docker pull ubuntu@sha256:90f3997e3e5f82097fa3046152944772876ac338365954f693b9e1bd3dd3c280
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
$ docker pull ubuntu@sha256:149d67e29f765f4db62aa52161009e99e389544e25a8f43c8c89d4a445a7ca37
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.5 MB (29547417 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b6548eacb0639263e9d8abfee48f8ac8b327102a05335b67572f715c580a968e`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 01 Dec 2023 07:49:48 GMT
ARG RELEASE
# Fri, 01 Dec 2023 07:49:48 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Fri, 01 Dec 2023 07:49:48 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Fri, 01 Dec 2023 07:49:48 GMT
LABEL org.opencontainers.image.version=22.04
# Fri, 01 Dec 2023 07:49:50 GMT
ADD file:36d444e2cede3abe58191dcf28890b874c0908f5259bf7e8855338555701c4c5 in / 
# Fri, 01 Dec 2023 07:49:50 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:5e8117c0bd28aecad06f7e76d4d3b64734d59c1a0a44541d18060cd8fba30c50`  
		Last Modified: Fri, 01 Dec 2023 08:21:32 GMT  
		Size: 29.5 MB (29547417 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:jammy` - linux; arm variant v7

```console
$ docker pull ubuntu@sha256:212b9f426e7be12bf9a80b65e1a14fc39e319cff3a7857772b21c02f1eaff610
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.6 MB (26629612 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bb3f9d425ffe4e459ab4cfc7b6f32c504d3f86b0fcb2a1b58d7646ab045ca4c0`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 05 Oct 2023 07:34:56 GMT
ARG RELEASE
# Thu, 05 Oct 2023 07:34:56 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 05 Oct 2023 07:34:56 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 05 Oct 2023 07:34:56 GMT
LABEL org.opencontainers.image.version=22.04
# Thu, 05 Oct 2023 07:35:01 GMT
ADD file:4b9d52f97ed5796b14772a84c1e7213402430d32312d15ae04a2dcc9fc485a52 in / 
# Thu, 05 Oct 2023 07:35:02 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:4091a3a7d6aa711dc0e0bbacfd3546df44ca257c300de1ad00fbdc95e218f7bd`  
		Last Modified: Thu, 05 Oct 2023 07:43:39 GMT  
		Size: 26.6 MB (26629612 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:jammy` - linux; arm64 variant v8

```console
$ docker pull ubuntu@sha256:02410fbfad7f2842cce3cf7655828424f4f7f6b5105b0016e24f1676f3bd15f5
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.4 MB (27351048 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e343402cadef796b4f12c2ee20b7346978a42a8d95516619c36c6397c4b0c766`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 05 Oct 2023 07:32:20 GMT
ARG RELEASE
# Thu, 05 Oct 2023 07:32:21 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 05 Oct 2023 07:32:21 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 05 Oct 2023 07:32:21 GMT
LABEL org.opencontainers.image.version=22.04
# Thu, 05 Oct 2023 07:32:22 GMT
ADD file:f8594e26831508c318e42c8dfd9942041031087b8de1bf3fec11fd75b8b30fd4 in / 
# Thu, 05 Oct 2023 07:32:22 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:bfbe77e41a78ee38147c5761aa8bc896d9f6e1e648b23468f294065ffe03c107`  
		Last Modified: Thu, 05 Oct 2023 07:43:33 GMT  
		Size: 27.4 MB (27351048 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:jammy` - linux; ppc64le

```console
$ docker pull ubuntu@sha256:b5759015a02040b956d02fb5cd8150ae0fdc3db0fd15af76dd006f6833bc9ab4
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.6 MB (34555968 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e7a609d38c5a2e47b65cf2a2ff61e6d2d5db4be6eb7578f40c4a672efc1f0cd0`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 05 Oct 2023 07:34:18 GMT
ARG RELEASE
# Thu, 05 Oct 2023 07:34:19 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 05 Oct 2023 07:34:19 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 05 Oct 2023 07:34:19 GMT
LABEL org.opencontainers.image.version=22.04
# Thu, 05 Oct 2023 07:34:22 GMT
ADD file:595ff761b2778bdc6bb59cbe8ce51c4a247e0f279ccd59a17b5be6cdeac0b4d2 in / 
# Thu, 05 Oct 2023 07:34:22 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:90496cba4a92b0bf6a8307bab5dd30100905ac891d478aa27771408328244c33`  
		Last Modified: Thu, 05 Oct 2023 07:43:45 GMT  
		Size: 34.6 MB (34555968 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:jammy` - linux; s390x

```console
$ docker pull ubuntu@sha256:ffa841e85005182836d91f7abd24ec081f3910716096955dcc1874b8017b96c9
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.0 MB (28023918 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e27f4324041cd007fd9a3e77aafafa96b00de774f3b241442e8f39457b00b46d`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 05 Oct 2023 07:29:34 GMT
ARG RELEASE
# Thu, 05 Oct 2023 07:29:34 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 05 Oct 2023 07:29:34 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 05 Oct 2023 07:29:34 GMT
LABEL org.opencontainers.image.version=22.04
# Thu, 05 Oct 2023 07:29:36 GMT
ADD file:d165475f8f027ab758a463da57c8c29f5d302f0a87a475ac68fdfae30005c7ac in / 
# Thu, 05 Oct 2023 07:29:36 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:0ffe28a7c279dfdb86b23c0d22d37e89442a6d771fbded124aee76b24119c2c1`  
		Last Modified: Thu, 05 Oct 2023 07:43:51 GMT  
		Size: 28.0 MB (28023918 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

## `ubuntu:jammy-20231128`

```console
$ docker pull ubuntu@sha256:76e076103d71431c71514d1c0265ce464514f6f3d0fa5f99e8afb2e4824e9b25
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 1
	-	linux; amd64

### `ubuntu:jammy-20231128` - linux; amd64

```console
$ docker pull ubuntu@sha256:149d67e29f765f4db62aa52161009e99e389544e25a8f43c8c89d4a445a7ca37
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.5 MB (29547417 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b6548eacb0639263e9d8abfee48f8ac8b327102a05335b67572f715c580a968e`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 01 Dec 2023 07:49:48 GMT
ARG RELEASE
# Fri, 01 Dec 2023 07:49:48 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Fri, 01 Dec 2023 07:49:48 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Fri, 01 Dec 2023 07:49:48 GMT
LABEL org.opencontainers.image.version=22.04
# Fri, 01 Dec 2023 07:49:50 GMT
ADD file:36d444e2cede3abe58191dcf28890b874c0908f5259bf7e8855338555701c4c5 in / 
# Fri, 01 Dec 2023 07:49:50 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:5e8117c0bd28aecad06f7e76d4d3b64734d59c1a0a44541d18060cd8fba30c50`  
		Last Modified: Fri, 01 Dec 2023 08:21:32 GMT  
		Size: 29.5 MB (29547417 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

## `ubuntu:latest`

```console
$ docker pull ubuntu@sha256:90f3997e3e5f82097fa3046152944772876ac338365954f693b9e1bd3dd3c280
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
$ docker pull ubuntu@sha256:149d67e29f765f4db62aa52161009e99e389544e25a8f43c8c89d4a445a7ca37
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.5 MB (29547417 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b6548eacb0639263e9d8abfee48f8ac8b327102a05335b67572f715c580a968e`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 01 Dec 2023 07:49:48 GMT
ARG RELEASE
# Fri, 01 Dec 2023 07:49:48 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Fri, 01 Dec 2023 07:49:48 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Fri, 01 Dec 2023 07:49:48 GMT
LABEL org.opencontainers.image.version=22.04
# Fri, 01 Dec 2023 07:49:50 GMT
ADD file:36d444e2cede3abe58191dcf28890b874c0908f5259bf7e8855338555701c4c5 in / 
# Fri, 01 Dec 2023 07:49:50 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:5e8117c0bd28aecad06f7e76d4d3b64734d59c1a0a44541d18060cd8fba30c50`  
		Last Modified: Fri, 01 Dec 2023 08:21:32 GMT  
		Size: 29.5 MB (29547417 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:latest` - linux; arm variant v7

```console
$ docker pull ubuntu@sha256:212b9f426e7be12bf9a80b65e1a14fc39e319cff3a7857772b21c02f1eaff610
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.6 MB (26629612 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bb3f9d425ffe4e459ab4cfc7b6f32c504d3f86b0fcb2a1b58d7646ab045ca4c0`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 05 Oct 2023 07:34:56 GMT
ARG RELEASE
# Thu, 05 Oct 2023 07:34:56 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 05 Oct 2023 07:34:56 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 05 Oct 2023 07:34:56 GMT
LABEL org.opencontainers.image.version=22.04
# Thu, 05 Oct 2023 07:35:01 GMT
ADD file:4b9d52f97ed5796b14772a84c1e7213402430d32312d15ae04a2dcc9fc485a52 in / 
# Thu, 05 Oct 2023 07:35:02 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:4091a3a7d6aa711dc0e0bbacfd3546df44ca257c300de1ad00fbdc95e218f7bd`  
		Last Modified: Thu, 05 Oct 2023 07:43:39 GMT  
		Size: 26.6 MB (26629612 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:latest` - linux; arm64 variant v8

```console
$ docker pull ubuntu@sha256:02410fbfad7f2842cce3cf7655828424f4f7f6b5105b0016e24f1676f3bd15f5
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.4 MB (27351048 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e343402cadef796b4f12c2ee20b7346978a42a8d95516619c36c6397c4b0c766`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 05 Oct 2023 07:32:20 GMT
ARG RELEASE
# Thu, 05 Oct 2023 07:32:21 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 05 Oct 2023 07:32:21 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 05 Oct 2023 07:32:21 GMT
LABEL org.opencontainers.image.version=22.04
# Thu, 05 Oct 2023 07:32:22 GMT
ADD file:f8594e26831508c318e42c8dfd9942041031087b8de1bf3fec11fd75b8b30fd4 in / 
# Thu, 05 Oct 2023 07:32:22 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:bfbe77e41a78ee38147c5761aa8bc896d9f6e1e648b23468f294065ffe03c107`  
		Last Modified: Thu, 05 Oct 2023 07:43:33 GMT  
		Size: 27.4 MB (27351048 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:latest` - linux; ppc64le

```console
$ docker pull ubuntu@sha256:b5759015a02040b956d02fb5cd8150ae0fdc3db0fd15af76dd006f6833bc9ab4
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.6 MB (34555968 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e7a609d38c5a2e47b65cf2a2ff61e6d2d5db4be6eb7578f40c4a672efc1f0cd0`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 05 Oct 2023 07:34:18 GMT
ARG RELEASE
# Thu, 05 Oct 2023 07:34:19 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 05 Oct 2023 07:34:19 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 05 Oct 2023 07:34:19 GMT
LABEL org.opencontainers.image.version=22.04
# Thu, 05 Oct 2023 07:34:22 GMT
ADD file:595ff761b2778bdc6bb59cbe8ce51c4a247e0f279ccd59a17b5be6cdeac0b4d2 in / 
# Thu, 05 Oct 2023 07:34:22 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:90496cba4a92b0bf6a8307bab5dd30100905ac891d478aa27771408328244c33`  
		Last Modified: Thu, 05 Oct 2023 07:43:45 GMT  
		Size: 34.6 MB (34555968 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:latest` - linux; s390x

```console
$ docker pull ubuntu@sha256:ffa841e85005182836d91f7abd24ec081f3910716096955dcc1874b8017b96c9
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.0 MB (28023918 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e27f4324041cd007fd9a3e77aafafa96b00de774f3b241442e8f39457b00b46d`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 05 Oct 2023 07:29:34 GMT
ARG RELEASE
# Thu, 05 Oct 2023 07:29:34 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 05 Oct 2023 07:29:34 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 05 Oct 2023 07:29:34 GMT
LABEL org.opencontainers.image.version=22.04
# Thu, 05 Oct 2023 07:29:36 GMT
ADD file:d165475f8f027ab758a463da57c8c29f5d302f0a87a475ac68fdfae30005c7ac in / 
# Thu, 05 Oct 2023 07:29:36 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:0ffe28a7c279dfdb86b23c0d22d37e89442a6d771fbded124aee76b24119c2c1`  
		Last Modified: Thu, 05 Oct 2023 07:43:51 GMT  
		Size: 28.0 MB (28023918 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

## `ubuntu:lunar`

```console
$ docker pull ubuntu@sha256:852d8cab9db2e8401402528f1d845d097e672fb28a09770aa0a4278a1911b70d
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
$ docker pull ubuntu@sha256:ea1285dffce8a938ef356908d1be741da594310c8dced79b870d66808cb12b0f
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.9 MB (26886018 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f4cdeba72b994748f5eb1f525a70a9cc553b66037ec37e23645fbf3f0f5c160d`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 28 Nov 2023 09:02:17 GMT
ARG RELEASE
# Tue, 28 Nov 2023 09:02:18 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 28 Nov 2023 09:02:18 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 28 Nov 2023 09:02:18 GMT
LABEL org.opencontainers.image.version=23.04
# Tue, 28 Nov 2023 09:02:19 GMT
ADD file:9627edfd854222fb9117755e0e89c54a01ba3477dffb8137693b12c586d970b8 in / 
# Tue, 28 Nov 2023 09:02:19 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:6360b371721185fefbbad6763ab745900f1b2f7714570234473232dd575fc07f`  
		Last Modified: Tue, 28 Nov 2023 09:27:24 GMT  
		Size: 26.9 MB (26886018 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:lunar` - linux; arm variant v7

```console
$ docker pull ubuntu@sha256:4dc1dd258d16171c6cd696ed5420402319d7cabe638b176b471495e94373f2a9
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **24.6 MB (24629439 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d83502f31cce9655561356390e34e8d506e888f6ce4743a8400bfa765f6eedb8`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 04 Oct 2023 12:25:21 GMT
ARG RELEASE
# Wed, 04 Oct 2023 12:25:21 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 04 Oct 2023 12:25:21 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 04 Oct 2023 12:25:22 GMT
LABEL org.opencontainers.image.version=23.04
# Wed, 04 Oct 2023 12:25:24 GMT
ADD file:b92305119eab5dd3dfb00f4d83cd84e00c8ae57143739329da5a19aeda55be4e in / 
# Wed, 04 Oct 2023 12:25:24 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:725335f54d3eb8903e713867d9f04db29fbc8835da3539fd3898faa22eaf016e`  
		Last Modified: Wed, 04 Oct 2023 12:33:24 GMT  
		Size: 24.6 MB (24629439 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:lunar` - linux; arm64 variant v8

```console
$ docker pull ubuntu@sha256:aa2be6baa498ab5862770bbc08cf00a058154cb257e41dca6ef8b7f7aebe22f8
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.1 MB (26065969 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4783be26912a96818aa1c9468ea8acb5eff2608697f62deff67048595a613145`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 04 Oct 2023 12:23:52 GMT
ARG RELEASE
# Wed, 04 Oct 2023 12:23:52 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 04 Oct 2023 12:23:52 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 04 Oct 2023 12:23:52 GMT
LABEL org.opencontainers.image.version=23.04
# Wed, 04 Oct 2023 12:23:53 GMT
ADD file:c9b1098bc90ac9b887c3bffdffbcff0c32f32e48df9a673041e3aa796296e69b in / 
# Wed, 04 Oct 2023 12:23:54 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:89e6336dd9e04a0993754adca328bf88d988540bb95cff284667037dd50f79eb`  
		Last Modified: Wed, 04 Oct 2023 12:33:17 GMT  
		Size: 26.1 MB (26065969 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:lunar` - linux; ppc64le

```console
$ docker pull ubuntu@sha256:2d697e1fc26340ae1a77a08397f53f978a6966d3c8a3cf195ee0870ca6e7dc2a
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.9 MB (30905941 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6651a10a7ea6479a915882811fa23c286c9baabb6ea68a11e48c3235246b574e`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 04 Oct 2023 12:08:54 GMT
ARG RELEASE
# Wed, 04 Oct 2023 12:08:54 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 04 Oct 2023 12:08:55 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 04 Oct 2023 12:08:55 GMT
LABEL org.opencontainers.image.version=23.04
# Wed, 04 Oct 2023 12:08:57 GMT
ADD file:24bc2f22a395e93a2ebbcfc45da8e5fc7f08e7c03cdc985c997300643d0310ec in / 
# Wed, 04 Oct 2023 12:08:58 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:fafd77e1a2b2b77f4b648372d147a2d31af161695aa89bed56883733707bd39f`  
		Last Modified: Wed, 04 Oct 2023 12:33:31 GMT  
		Size: 30.9 MB (30905941 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:lunar` - linux; s390x

```console
$ docker pull ubuntu@sha256:e54d7ce369ad0b993654f624153bbf76a3ef547ed0dc2e14ba0a60d199077b0e
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.7 MB (25692995 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ab36c0e39cab522c65337f5bfeaaf36ce62c510ca07b09d17bea00fe80bfed55`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 04 Oct 2023 12:26:55 GMT
ARG RELEASE
# Wed, 04 Oct 2023 12:26:55 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 04 Oct 2023 12:26:55 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 04 Oct 2023 12:26:55 GMT
LABEL org.opencontainers.image.version=23.04
# Wed, 04 Oct 2023 12:26:57 GMT
ADD file:553d1c48ed98fa8bd575a7a645019079304c101dd6e06e82591a25440fe1a9b8 in / 
# Wed, 04 Oct 2023 12:26:57 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:8333843c4e8c11c41362709d3852d288b9deee48dfdd0014810ce4d3ef224714`  
		Last Modified: Wed, 04 Oct 2023 12:33:37 GMT  
		Size: 25.7 MB (25692995 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

## `ubuntu:lunar-20231128`

```console
$ docker pull ubuntu@sha256:2635f9972c94322c07b945bbc25820eace635956d8b81158c30319d7e596bd43
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 1
	-	linux; amd64

### `ubuntu:lunar-20231128` - linux; amd64

```console
$ docker pull ubuntu@sha256:ea1285dffce8a938ef356908d1be741da594310c8dced79b870d66808cb12b0f
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.9 MB (26886018 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f4cdeba72b994748f5eb1f525a70a9cc553b66037ec37e23645fbf3f0f5c160d`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 28 Nov 2023 09:02:17 GMT
ARG RELEASE
# Tue, 28 Nov 2023 09:02:18 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 28 Nov 2023 09:02:18 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 28 Nov 2023 09:02:18 GMT
LABEL org.opencontainers.image.version=23.04
# Tue, 28 Nov 2023 09:02:19 GMT
ADD file:9627edfd854222fb9117755e0e89c54a01ba3477dffb8137693b12c586d970b8 in / 
# Tue, 28 Nov 2023 09:02:19 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:6360b371721185fefbbad6763ab745900f1b2f7714570234473232dd575fc07f`  
		Last Modified: Tue, 28 Nov 2023 09:27:24 GMT  
		Size: 26.9 MB (26886018 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

## `ubuntu:mantic`

```console
$ docker pull ubuntu@sha256:e82db07bf46c1da56547b5fb31c0200f4a41e0f0ea9cb7970b3ca3e8720d8d6c
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `ubuntu:mantic` - linux; amd64

```console
$ docker pull ubuntu@sha256:8d093e0651575a6437cc4a3d561f892a345d263aeac6156ef378fe6a4ccabd4c
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.3 MB (27273553 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:483a94112583ff9c6d0a7b67348fc3b0ee5bbf104a86a9e24585c9ad1028fd25`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 30 Nov 2023 17:54:17 GMT
ARG RELEASE
# Thu, 30 Nov 2023 17:54:17 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 30 Nov 2023 17:54:17 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 30 Nov 2023 17:54:17 GMT
LABEL org.opencontainers.image.version=23.10
# Thu, 30 Nov 2023 17:54:19 GMT
ADD file:5430e0b4ea856c760b6e2b88e8c2cd2d49704ed2f3c53ae34c10750a608d40ec in / 
# Thu, 30 Nov 2023 17:54:19 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:767829bcf202e4fa7e777f29d390307e29ac437f131685a1ff1293d44705ca23`  
		Last Modified: Thu, 30 Nov 2023 18:06:39 GMT  
		Size: 27.3 MB (27273553 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:mantic` - linux; arm variant v7

```console
$ docker pull ubuntu@sha256:2a465a4c4831c57977b6646e481f504061294f1bf1ae1b99fb5d93c67b8a471a
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.2 MB (25201383 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bc753c284b47a7a5ff3ec2e926551ba95dc6c9072415649cb13a9cdff503dc04`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 11 Oct 2023 18:02:33 GMT
ARG RELEASE
# Wed, 11 Oct 2023 18:02:33 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 11 Oct 2023 18:02:34 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 11 Oct 2023 18:02:34 GMT
LABEL org.opencontainers.image.version=23.10
# Wed, 11 Oct 2023 18:02:39 GMT
ADD file:1be1311acbd557f7769fb5c1913ef56305431e7547f96c20ac36284fdd926223 in / 
# Wed, 11 Oct 2023 18:02:39 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:8761b0d436cd2e1ff47496b7cc353cf0b49347ffc92b070c31a5cf5431041614`  
		Last Modified: Wed, 11 Oct 2023 18:18:00 GMT  
		Size: 25.2 MB (25201383 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:mantic` - linux; arm64 variant v8

```console
$ docker pull ubuntu@sha256:7708743264cbb7f6cf7fc13e915faece45a6cdda455748bc55e58e8de3d27b63
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.4 MB (26379954 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3f9cf3a31fbf871322b774402c7c25b800d0e93c222d5a44339f2d3a99dede82`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 11 Oct 2023 18:03:02 GMT
ARG RELEASE
# Wed, 11 Oct 2023 18:03:02 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 11 Oct 2023 18:03:02 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 11 Oct 2023 18:03:02 GMT
LABEL org.opencontainers.image.version=23.10
# Wed, 11 Oct 2023 18:03:10 GMT
ADD file:9e750ebbbf7e47a121d153e6699006776ea61b04b6c8e31556600483a020f617 in / 
# Wed, 11 Oct 2023 18:03:10 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:f906b88252effff97383eeb7dd4d265f3f31a54aa3833dd349cf8c4a35fbdbe9`  
		Last Modified: Wed, 11 Oct 2023 18:17:54 GMT  
		Size: 26.4 MB (26379954 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:mantic` - linux; ppc64le

```console
$ docker pull ubuntu@sha256:347a278b913b988b85442a3e187001edfe854da3ed499f45782d4a714f08632f
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.3 MB (31340704 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:96fb712785eb8f8fe4cdc47a6bb3bd8014c2b376c684dd430b32f81e786cdd5e`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 11 Oct 2023 18:06:00 GMT
ARG RELEASE
# Wed, 11 Oct 2023 18:06:00 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 11 Oct 2023 18:06:00 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 11 Oct 2023 18:06:00 GMT
LABEL org.opencontainers.image.version=23.10
# Wed, 11 Oct 2023 18:06:03 GMT
ADD file:a18be8add7eb60493b13d2aac8d624230297bd15be033756795582dc07cb04bb in / 
# Wed, 11 Oct 2023 18:06:03 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:6e4ddce09953092c8c6052d38bc7c2044237f1337f42f1f86edab6718af804ea`  
		Last Modified: Wed, 11 Oct 2023 18:18:11 GMT  
		Size: 31.3 MB (31340704 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:mantic` - linux; s390x

```console
$ docker pull ubuntu@sha256:f2e6e56781fb1122ffcdc449f44cb48f8a1279e0baf318582f274a1c44c3b64e
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.1 MB (27069339 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b6598907abce49b9b4f06fea395b2ed375f2bf7fad9b484729cc1b313b2b6109`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 11 Oct 2023 18:03:34 GMT
ARG RELEASE
# Wed, 11 Oct 2023 18:03:34 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 11 Oct 2023 18:03:34 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 11 Oct 2023 18:03:34 GMT
LABEL org.opencontainers.image.version=23.10
# Wed, 11 Oct 2023 18:03:36 GMT
ADD file:8ceb0028af8276b03b6c88b19445f30165a41791919c756e1434da6ded4387db in / 
# Wed, 11 Oct 2023 18:03:36 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:5ef15690269b5b1e6f9795320a2a15f009506ead422509007e5cc08858b1c41e`  
		Last Modified: Wed, 11 Oct 2023 18:18:18 GMT  
		Size: 27.1 MB (27069339 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

## `ubuntu:mantic-20231128`

```console
$ docker pull ubuntu@sha256:35b9b3ec575b1c2058ce432662a3d658804fd4210fb31121625de84127580cc3
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 1
	-	linux; amd64

### `ubuntu:mantic-20231128` - linux; amd64

```console
$ docker pull ubuntu@sha256:8d093e0651575a6437cc4a3d561f892a345d263aeac6156ef378fe6a4ccabd4c
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.3 MB (27273553 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:483a94112583ff9c6d0a7b67348fc3b0ee5bbf104a86a9e24585c9ad1028fd25`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 30 Nov 2023 17:54:17 GMT
ARG RELEASE
# Thu, 30 Nov 2023 17:54:17 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 30 Nov 2023 17:54:17 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 30 Nov 2023 17:54:17 GMT
LABEL org.opencontainers.image.version=23.10
# Thu, 30 Nov 2023 17:54:19 GMT
ADD file:5430e0b4ea856c760b6e2b88e8c2cd2d49704ed2f3c53ae34c10750a608d40ec in / 
# Thu, 30 Nov 2023 17:54:19 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:767829bcf202e4fa7e777f29d390307e29ac437f131685a1ff1293d44705ca23`  
		Last Modified: Thu, 30 Nov 2023 18:06:39 GMT  
		Size: 27.3 MB (27273553 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

## `ubuntu:noble`

```console
$ docker pull ubuntu@sha256:5cead7e5f0888b84ea7bef10ce29f17d582385b0f468ba6b418f8d3ba3eba6f6
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 1
	-	linux; amd64

### `ubuntu:noble` - linux; amd64

```console
$ docker pull ubuntu@sha256:ef2b3c979842614a9537785f2dcc5e93a977fa50dc567c42a7d4f5ea6470fec0
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.2 MB (27213697 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bfaf276bdd215773746bde9489a88d063b98584b8a650272c037da7be94941a6`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 27 Nov 2023 11:09:34 GMT
ARG RELEASE
# Mon, 27 Nov 2023 11:09:34 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 27 Nov 2023 11:09:34 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 27 Nov 2023 11:09:34 GMT
LABEL org.opencontainers.image.version=24.04
# Mon, 27 Nov 2023 11:09:35 GMT
ADD file:b2f5aa693e38f0ebe3e4d26ded8f957b4eb6f75c8360340cfcdeee25bf1b1b40 in / 
# Mon, 27 Nov 2023 11:09:36 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:62a1d607dcd86fd912d7d1448a129970b9c35f5506fbc48f8fea327ec9706b14`  
		Last Modified: Mon, 27 Nov 2023 11:15:40 GMT  
		Size: 27.2 MB (27213697 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

## `ubuntu:noble-20231126.1`

```console
$ docker pull ubuntu@sha256:5cead7e5f0888b84ea7bef10ce29f17d582385b0f468ba6b418f8d3ba3eba6f6
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 1
	-	linux; amd64

### `ubuntu:noble-20231126.1` - linux; amd64

```console
$ docker pull ubuntu@sha256:ef2b3c979842614a9537785f2dcc5e93a977fa50dc567c42a7d4f5ea6470fec0
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.2 MB (27213697 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bfaf276bdd215773746bde9489a88d063b98584b8a650272c037da7be94941a6`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 27 Nov 2023 11:09:34 GMT
ARG RELEASE
# Mon, 27 Nov 2023 11:09:34 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 27 Nov 2023 11:09:34 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 27 Nov 2023 11:09:34 GMT
LABEL org.opencontainers.image.version=24.04
# Mon, 27 Nov 2023 11:09:35 GMT
ADD file:b2f5aa693e38f0ebe3e4d26ded8f957b4eb6f75c8360340cfcdeee25bf1b1b40 in / 
# Mon, 27 Nov 2023 11:09:36 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:62a1d607dcd86fd912d7d1448a129970b9c35f5506fbc48f8fea327ec9706b14`  
		Last Modified: Mon, 27 Nov 2023 11:15:40 GMT  
		Size: 27.2 MB (27213697 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

## `ubuntu:rolling`

```console
$ docker pull ubuntu@sha256:e82db07bf46c1da56547b5fb31c0200f4a41e0f0ea9cb7970b3ca3e8720d8d6c
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
$ docker pull ubuntu@sha256:8d093e0651575a6437cc4a3d561f892a345d263aeac6156ef378fe6a4ccabd4c
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.3 MB (27273553 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:483a94112583ff9c6d0a7b67348fc3b0ee5bbf104a86a9e24585c9ad1028fd25`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 30 Nov 2023 17:54:17 GMT
ARG RELEASE
# Thu, 30 Nov 2023 17:54:17 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 30 Nov 2023 17:54:17 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 30 Nov 2023 17:54:17 GMT
LABEL org.opencontainers.image.version=23.10
# Thu, 30 Nov 2023 17:54:19 GMT
ADD file:5430e0b4ea856c760b6e2b88e8c2cd2d49704ed2f3c53ae34c10750a608d40ec in / 
# Thu, 30 Nov 2023 17:54:19 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:767829bcf202e4fa7e777f29d390307e29ac437f131685a1ff1293d44705ca23`  
		Last Modified: Thu, 30 Nov 2023 18:06:39 GMT  
		Size: 27.3 MB (27273553 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:rolling` - linux; arm variant v7

```console
$ docker pull ubuntu@sha256:2a465a4c4831c57977b6646e481f504061294f1bf1ae1b99fb5d93c67b8a471a
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.2 MB (25201383 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bc753c284b47a7a5ff3ec2e926551ba95dc6c9072415649cb13a9cdff503dc04`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 11 Oct 2023 18:02:33 GMT
ARG RELEASE
# Wed, 11 Oct 2023 18:02:33 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 11 Oct 2023 18:02:34 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 11 Oct 2023 18:02:34 GMT
LABEL org.opencontainers.image.version=23.10
# Wed, 11 Oct 2023 18:02:39 GMT
ADD file:1be1311acbd557f7769fb5c1913ef56305431e7547f96c20ac36284fdd926223 in / 
# Wed, 11 Oct 2023 18:02:39 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:8761b0d436cd2e1ff47496b7cc353cf0b49347ffc92b070c31a5cf5431041614`  
		Last Modified: Wed, 11 Oct 2023 18:18:00 GMT  
		Size: 25.2 MB (25201383 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:rolling` - linux; arm64 variant v8

```console
$ docker pull ubuntu@sha256:7708743264cbb7f6cf7fc13e915faece45a6cdda455748bc55e58e8de3d27b63
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.4 MB (26379954 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3f9cf3a31fbf871322b774402c7c25b800d0e93c222d5a44339f2d3a99dede82`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 11 Oct 2023 18:03:02 GMT
ARG RELEASE
# Wed, 11 Oct 2023 18:03:02 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 11 Oct 2023 18:03:02 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 11 Oct 2023 18:03:02 GMT
LABEL org.opencontainers.image.version=23.10
# Wed, 11 Oct 2023 18:03:10 GMT
ADD file:9e750ebbbf7e47a121d153e6699006776ea61b04b6c8e31556600483a020f617 in / 
# Wed, 11 Oct 2023 18:03:10 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:f906b88252effff97383eeb7dd4d265f3f31a54aa3833dd349cf8c4a35fbdbe9`  
		Last Modified: Wed, 11 Oct 2023 18:17:54 GMT  
		Size: 26.4 MB (26379954 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:rolling` - linux; ppc64le

```console
$ docker pull ubuntu@sha256:347a278b913b988b85442a3e187001edfe854da3ed499f45782d4a714f08632f
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.3 MB (31340704 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:96fb712785eb8f8fe4cdc47a6bb3bd8014c2b376c684dd430b32f81e786cdd5e`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 11 Oct 2023 18:06:00 GMT
ARG RELEASE
# Wed, 11 Oct 2023 18:06:00 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 11 Oct 2023 18:06:00 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 11 Oct 2023 18:06:00 GMT
LABEL org.opencontainers.image.version=23.10
# Wed, 11 Oct 2023 18:06:03 GMT
ADD file:a18be8add7eb60493b13d2aac8d624230297bd15be033756795582dc07cb04bb in / 
# Wed, 11 Oct 2023 18:06:03 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:6e4ddce09953092c8c6052d38bc7c2044237f1337f42f1f86edab6718af804ea`  
		Last Modified: Wed, 11 Oct 2023 18:18:11 GMT  
		Size: 31.3 MB (31340704 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:rolling` - linux; s390x

```console
$ docker pull ubuntu@sha256:f2e6e56781fb1122ffcdc449f44cb48f8a1279e0baf318582f274a1c44c3b64e
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.1 MB (27069339 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b6598907abce49b9b4f06fea395b2ed375f2bf7fad9b484729cc1b313b2b6109`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 11 Oct 2023 18:03:34 GMT
ARG RELEASE
# Wed, 11 Oct 2023 18:03:34 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 11 Oct 2023 18:03:34 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 11 Oct 2023 18:03:34 GMT
LABEL org.opencontainers.image.version=23.10
# Wed, 11 Oct 2023 18:03:36 GMT
ADD file:8ceb0028af8276b03b6c88b19445f30165a41791919c756e1434da6ded4387db in / 
# Wed, 11 Oct 2023 18:03:36 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:5ef15690269b5b1e6f9795320a2a15f009506ead422509007e5cc08858b1c41e`  
		Last Modified: Wed, 11 Oct 2023 18:18:18 GMT  
		Size: 27.1 MB (27069339 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
