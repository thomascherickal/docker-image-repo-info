<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `ubuntu`

-	[`ubuntu:20.04`](#ubuntu2004)
-	[`ubuntu:22.04`](#ubuntu2204)
-	[`ubuntu:23.04`](#ubuntu2304)
-	[`ubuntu:23.10`](#ubuntu2310)
-	[`ubuntu:devel`](#ubuntudevel)
-	[`ubuntu:focal`](#ubuntufocal)
-	[`ubuntu:focal-20230801`](#ubuntufocal-20230801)
-	[`ubuntu:jammy`](#ubuntujammy)
-	[`ubuntu:jammy-20230916`](#ubuntujammy-20230916)
-	[`ubuntu:latest`](#ubuntulatest)
-	[`ubuntu:lunar`](#ubuntulunar)
-	[`ubuntu:lunar-20230816`](#ubuntulunar-20230816)
-	[`ubuntu:mantic`](#ubuntumantic)
-	[`ubuntu:mantic-20230926`](#ubuntumantic-20230926)
-	[`ubuntu:rolling`](#ubunturolling)

## `ubuntu:20.04`

```console
$ docker pull ubuntu@sha256:33a5cc25d22c45900796a1aca487ad7a7cb09f09ea00b779e3b2026b4fc2faba
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
$ docker pull ubuntu@sha256:3246518d9735254519e1b2ff35f95686e4a5011c90c85344c1f38df7bae9dd37
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.5 MB (27506442 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6df89402372646d400cf092016c28066391a26f5d46c00b1153e75003465484d`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 01 Aug 2023 06:16:43 GMT
ARG RELEASE
# Tue, 01 Aug 2023 06:16:44 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 01 Aug 2023 06:16:44 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 01 Aug 2023 06:16:44 GMT
LABEL org.opencontainers.image.version=20.04
# Tue, 01 Aug 2023 06:16:45 GMT
ADD file:233702cd816c07bc9fed02881b11fb3bdcaee41f3ce3ec1c9f0c4a060b155d5b in / 
# Tue, 01 Aug 2023 06:16:46 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:edaedc954fb53f42a7754a6e2d1b57f091bc9b11063bc445c2e325ea448f8f68`  
		Last Modified: Tue, 01 Aug 2023 06:54:06 GMT  
		Size: 27.5 MB (27506442 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:20.04` - linux; arm variant v7

```console
$ docker pull ubuntu@sha256:993dc9215facb1278d78c1ac9aacaf0b10ce01a3319245477b526fb49bb3a85b
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.6 MB (23612645 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9647c2503ec334ee47dc65a547a14f79543680a640b31669e4e417949c03857b`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 01 Aug 2023 06:16:45 GMT
ARG RELEASE
# Tue, 01 Aug 2023 06:16:45 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 01 Aug 2023 06:16:46 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 01 Aug 2023 06:16:46 GMT
LABEL org.opencontainers.image.version=20.04
# Tue, 01 Aug 2023 06:16:49 GMT
ADD file:60aa8465a6ba5538decc41365cc9b78ae86131e8c2cfc9177b4a336354ead988 in / 
# Tue, 01 Aug 2023 06:16:50 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:d2b6ba5e7ade25cef0db07ca410b7d5e09085b9c442b62904956cd4d5a81ad10`  
		Last Modified: Tue, 01 Aug 2023 06:54:18 GMT  
		Size: 23.6 MB (23612645 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:20.04` - linux; arm64 variant v8

```console
$ docker pull ubuntu@sha256:af43d52ea8f98c8ab92858a37b87be1805ce16f5300cb38b9958e63ac6b25902
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.0 MB (25974619 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:15c9d636caddd81490d58a714937f112702f9239c98950221e9fd0dd9735df9d`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 01 Aug 2023 06:20:56 GMT
ARG RELEASE
# Tue, 01 Aug 2023 06:20:56 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 01 Aug 2023 06:20:56 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 01 Aug 2023 06:20:57 GMT
LABEL org.opencontainers.image.version=20.04
# Tue, 01 Aug 2023 06:21:03 GMT
ADD file:ef6e767091d76c1461d099d5bc7a18c526ec80834cf87280803ab6480192f766 in / 
# Tue, 01 Aug 2023 06:21:03 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:82d728d38b98752cba7d2d7af8ee1cfe67ccdc5915814420650e78def5d1cebc`  
		Last Modified: Tue, 01 Aug 2023 06:54:12 GMT  
		Size: 26.0 MB (25974619 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:20.04` - linux; ppc64le

```console
$ docker pull ubuntu@sha256:a305c3951a3741555d5019870f4827c4becdcc95df539ce7ed364ab5ab2db342
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.1 MB (32070704 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a92643ae09f6e607311cb05e4f0f7679c0873b7e4c235e1b57f5e409cfc47c50`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 01 Aug 2023 06:20:36 GMT
ARG RELEASE
# Tue, 01 Aug 2023 06:20:36 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 01 Aug 2023 06:20:37 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 01 Aug 2023 06:20:37 GMT
LABEL org.opencontainers.image.version=20.04
# Tue, 01 Aug 2023 06:20:40 GMT
ADD file:822df76493d1d533c1a283ab7bb20ce81309f57279422a0eebb2ffb9fab55963 in / 
# Tue, 01 Aug 2023 06:20:40 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:fa78ce4014add322eddde3378405efe21c85e886c0195e18533d5991d5477833`  
		Last Modified: Tue, 01 Aug 2023 06:54:25 GMT  
		Size: 32.1 MB (32070704 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:20.04` - linux; s390x

```console
$ docker pull ubuntu@sha256:5ad386cefcdbd1248f73a3bbcfbf529f39864dddcf9497d9a705540afd23e6e9
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.4 MB (26351280 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5079141aa115a82eb5f952b45f4cf336075d4dc4bc3ea2cfdab4351497d2fc9e`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 01 Aug 2023 06:17:39 GMT
ARG RELEASE
# Tue, 01 Aug 2023 06:17:39 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 01 Aug 2023 06:17:39 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 01 Aug 2023 06:17:39 GMT
LABEL org.opencontainers.image.version=20.04
# Tue, 01 Aug 2023 06:17:41 GMT
ADD file:36efc3ec29bb54e0987fe91be1aa7cc849909b3cd2534af3de2d3d07a03804cf in / 
# Tue, 01 Aug 2023 06:17:41 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:773e1d05400f41114172ea2dbaa16f037c5812b7d1092cbf0df5d19e69586402`  
		Last Modified: Tue, 01 Aug 2023 06:54:31 GMT  
		Size: 26.4 MB (26351280 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

## `ubuntu:22.04`

```console
$ docker pull ubuntu@sha256:c1a4fb1fd1697920c2a422a355783a9debaf57b8eb6c92de84a75ce5be34c6cb
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
$ docker pull ubuntu@sha256:b4b521bfcec90b11d2869e00fe1f2380c21cbfcd799ee35df8bd7ac09e6f63ea
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.5 MB (29538209 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3565a89d9e81a4cb4cb2b0d947c7c11227a3f358dc216d19fc54bfd77cd5b542`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 25 Sep 2023 10:17:05 GMT
ARG RELEASE
# Mon, 25 Sep 2023 10:17:05 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 25 Sep 2023 10:17:05 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 25 Sep 2023 10:17:05 GMT
LABEL org.opencontainers.image.version=22.04
# Mon, 25 Sep 2023 10:17:07 GMT
ADD file:194c886b88876c1804cc5f80719669653c16a388b664147b7f22402105f533c4 in / 
# Mon, 25 Sep 2023 10:17:08 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:37aaf24cf781dcc5b9a4f8aa5a99a40b60ae45d64dcb4f6d5a4b9e5ab7ab0894`  
		Last Modified: Mon, 25 Sep 2023 10:30:37 GMT  
		Size: 29.5 MB (29538209 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:22.04` - linux; arm variant v7

```console
$ docker pull ubuntu@sha256:2589fe6bcf90466564741ae0d8309d1323f33b6ec8a5d401a62d0b256bcc3c37
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.1 MB (26142545 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5edd8b11048dd1910bbeeae6325888a34a64e8a0d2576b6d843063825b339cd1`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 16 Aug 2023 06:08:27 GMT
ARG RELEASE
# Wed, 16 Aug 2023 06:08:27 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 16 Aug 2023 06:08:27 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 16 Aug 2023 06:08:27 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 16 Aug 2023 06:08:32 GMT
ADD file:e61c6bbfc8728cb119b4cfd4a35d1e5aad76e84c0ac8f2ff9850a7ceec9f3dc5 in / 
# Wed, 16 Aug 2023 06:08:32 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:d79cf5fbd02b4f64ddfb1ba3ae0178a904f012bc2ff0e5603ffdb4668a8f529c`  
		Last Modified: Wed, 16 Aug 2023 06:32:59 GMT  
		Size: 26.1 MB (26142545 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:22.04` - linux; arm64 variant v8

```console
$ docker pull ubuntu@sha256:f58b48967ecc767fc238144ffdb7eb668cefcc8438de8f8a59c4cefbbf29b323
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.4 MB (27351199 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bf9e5b7213b4e0d99cddc039011cc60bfd76ed5ef63bbd837ab0b8416c305c39`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 25 Sep 2023 10:17:41 GMT
ARG RELEASE
# Mon, 25 Sep 2023 10:17:41 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 25 Sep 2023 10:17:41 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 25 Sep 2023 10:17:41 GMT
LABEL org.opencontainers.image.version=22.04
# Mon, 25 Sep 2023 10:17:44 GMT
ADD file:8540670760767f19eaf101fbce1da1881a2f24a7d65da6abdedc644b8fb00463 in / 
# Mon, 25 Sep 2023 10:17:45 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:c391327a0f1df5790bcb00ac010a1a3924c9e4387ce36b290bc16fd9f4cc5740`  
		Last Modified: Mon, 25 Sep 2023 10:30:43 GMT  
		Size: 27.4 MB (27351199 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:22.04` - linux; ppc64le

```console
$ docker pull ubuntu@sha256:de1fcbe2d7e928d0be9476e3079df8e69072dfb140be94f5d34091f09f6917dd
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.6 MB (34567229 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b67aa2427a930674989cafcaf3fa7d1d16b2c47ed37003fe712bcbf5bc07a6fc`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 16 Aug 2023 06:03:07 GMT
ARG RELEASE
# Wed, 16 Aug 2023 06:03:07 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 16 Aug 2023 06:03:08 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 16 Aug 2023 06:03:08 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 16 Aug 2023 06:03:11 GMT
ADD file:632018deeaeb9e42f0026fb331dfb08381e46bd414b2b470b18ea22ac0653bf6 in / 
# Wed, 16 Aug 2023 06:03:11 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:c76fbfef684586d44d4a79c1a2c093ecf60b0f6c5deb0742082a5152ecd9a1fa`  
		Last Modified: Wed, 16 Aug 2023 06:33:06 GMT  
		Size: 34.6 MB (34567229 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:22.04` - linux; s390x

```console
$ docker pull ubuntu@sha256:ed1a67bb47f3c35d782293229127ac1f8d64873a131186c49fe079dada0fa7e0
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.0 MB (28016004 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f34a6de6626fe032cc2ff34b644898f997ccd85378e081b63c95246ad6b11e3d`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 16 Aug 2023 06:05:03 GMT
ARG RELEASE
# Wed, 16 Aug 2023 06:05:03 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 16 Aug 2023 06:05:03 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 16 Aug 2023 06:05:03 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 16 Aug 2023 06:05:05 GMT
ADD file:58eccd685d73ff80ea235016d6e33d093e1063800d869935b67b59a1b8891344 in / 
# Wed, 16 Aug 2023 06:05:05 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:e1b6153f78cbd4f98e7250bc413a393734736138dcb57f1e41f45c3e43c5a120`  
		Last Modified: Wed, 16 Aug 2023 06:33:12 GMT  
		Size: 28.0 MB (28016004 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

## `ubuntu:23.04`

```console
$ docker pull ubuntu@sha256:f1090cfa89ab321a6d670e79652f61593502591f2fc7452fb0b7c6da575729c4
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
$ docker pull ubuntu@sha256:24898c8e1ac370d2d309d6d9df56af52bebdad86925c623b5e87e12404453518
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.9 MB (26873617 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:21098a29e034a8f6f1952d1d8a49b5732b70e532c31f0e88e1ff499c6540c57c`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 16 Aug 2023 04:28:31 GMT
ARG RELEASE
# Wed, 16 Aug 2023 04:28:31 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 16 Aug 2023 04:28:31 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 16 Aug 2023 04:28:31 GMT
LABEL org.opencontainers.image.version=23.04
# Wed, 16 Aug 2023 04:28:32 GMT
ADD file:7392bed4dbab9fb7c9ad5bde6f3bfcde3bcbf1885c336af9c231af6defaa31e1 in / 
# Wed, 16 Aug 2023 04:28:33 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:10fb01f4f619bc954ba611cebca23f2b96d255c7ead4040b449f063e530df1a4`  
		Last Modified: Wed, 16 Aug 2023 04:34:32 GMT  
		Size: 26.9 MB (26873617 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:23.04` - linux; arm variant v7

```console
$ docker pull ubuntu@sha256:1e9568cacc4bd0a59a44d8e68ae8fc5f4287c132d455492881f7a1106b722beb
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **24.6 MB (24627247 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e46f21739314ec025a0ce92c7a657ddb65785a29870d74435a08554207fb3688`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 16 Aug 2023 04:16:11 GMT
ARG RELEASE
# Wed, 16 Aug 2023 04:16:11 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 16 Aug 2023 04:16:11 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 16 Aug 2023 04:16:11 GMT
LABEL org.opencontainers.image.version=23.04
# Wed, 16 Aug 2023 04:16:16 GMT
ADD file:1f1c9502544acdbb6a7450226ced78cfe982a6305f2aea77ab7d1f73b50fc7f0 in / 
# Wed, 16 Aug 2023 04:16:16 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:e05ef4abc6c76087042349392d272a7eeb590834dc45d1247295302c212fda9d`  
		Last Modified: Wed, 16 Aug 2023 04:34:45 GMT  
		Size: 24.6 MB (24627247 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:23.04` - linux; arm64 variant v8

```console
$ docker pull ubuntu@sha256:d68d8bcae123a839bc72b91fa9df55956be3fcb2dbfc247acb7f65908eaa6c35
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.1 MB (26064545 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e1c8e9335de75964dd320b20b4290408432be2962faf7ad36d3a47d48f3131cd`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 16 Aug 2023 04:15:57 GMT
ARG RELEASE
# Wed, 16 Aug 2023 04:15:57 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 16 Aug 2023 04:15:57 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 16 Aug 2023 04:15:57 GMT
LABEL org.opencontainers.image.version=23.04
# Wed, 16 Aug 2023 04:16:01 GMT
ADD file:adea2962926b29b76eb8da76ae9e830c5ad7050ae9b19f5427191b338c8a2c56 in / 
# Wed, 16 Aug 2023 04:16:02 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:2b2d15932a31f0857b9499cc218b8777708cb1d73ae6ef680f624ca7d4342763`  
		Last Modified: Wed, 16 Aug 2023 04:34:39 GMT  
		Size: 26.1 MB (26064545 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:23.04` - linux; ppc64le

```console
$ docker pull ubuntu@sha256:1306e75f505a2305f2c46f51f33be8b8599923bd5a652c3b5dc37333db4f44ab
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.9 MB (30905042 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:91733a8763fe80d6e620ec400c2721ee45c0f80398506088d1278d6531299a90`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 16 Aug 2023 04:16:31 GMT
ARG RELEASE
# Wed, 16 Aug 2023 04:16:31 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 16 Aug 2023 04:16:31 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 16 Aug 2023 04:16:31 GMT
LABEL org.opencontainers.image.version=23.04
# Wed, 16 Aug 2023 04:16:34 GMT
ADD file:a9d35b320d969ee1ae8a7bc83aba49da30d93724befb5948c680066ad4f1acdf in / 
# Wed, 16 Aug 2023 04:16:35 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:f51cbff870f31d4c4397c2f21529046998f8d6e7748fd6f059b325a0759c7dd4`  
		Last Modified: Wed, 16 Aug 2023 04:34:51 GMT  
		Size: 30.9 MB (30905042 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:23.04` - linux; s390x

```console
$ docker pull ubuntu@sha256:ec9620bbf89d1a3b1171f961340a890166607be3423d96e740f6d56f36ccb125
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.7 MB (25691524 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1289eb3132a14bc161676d7f928d557bf63eb8561718e9d5247e16e88ebee8ff`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 16 Aug 2023 04:29:27 GMT
ARG RELEASE
# Wed, 16 Aug 2023 04:29:28 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 16 Aug 2023 04:29:28 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 16 Aug 2023 04:29:28 GMT
LABEL org.opencontainers.image.version=23.04
# Wed, 16 Aug 2023 04:29:29 GMT
ADD file:14fcf0756fb29b609af54412c31e2ff9acbf4634984ce95bf204c67668706cb5 in / 
# Wed, 16 Aug 2023 04:29:30 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:b1e434384d3d3b546e155df0cf143c8c0a92bf766c6808bf2e3e1d2f22010839`  
		Last Modified: Wed, 16 Aug 2023 04:34:57 GMT  
		Size: 25.7 MB (25691524 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

## `ubuntu:23.10`

```console
$ docker pull ubuntu@sha256:3c38c7f067cc8103c300b3ed089a0b916ad5c9852f402a95c6fb8a8cf4b69b23
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
$ docker pull ubuntu@sha256:7e44d7ed904145328785378ddac5de49ac931d3b28b72f6c9f5fb350f9b4a849
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.3 MB (27277147 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1d8801a7ecb54952ea17852be887c1d858fd7bd78dcee093afc11fee7ed53f7c`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 26 Sep 2023 05:03:43 GMT
ARG RELEASE
# Tue, 26 Sep 2023 05:03:43 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 26 Sep 2023 05:03:43 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 26 Sep 2023 05:03:43 GMT
LABEL org.opencontainers.image.version=23.10
# Tue, 26 Sep 2023 05:03:45 GMT
ADD file:5fb49f260a0c3bf404c0fe31d8f0f812e9c143bd48223c4f15a85168758eb880 in / 
# Tue, 26 Sep 2023 05:03:45 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:97e98d3adb77a3f73850e0a81cdde417afce9cd9dce78c444f99b9258caee9fa`  
		Last Modified: Tue, 26 Sep 2023 05:33:55 GMT  
		Size: 27.3 MB (27277147 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:23.10` - linux; arm variant v7

```console
$ docker pull ubuntu@sha256:d7e166e923d882bda98249bf852065c7cf27069ff5c5aeb5b8535f0e529c614f
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.2 MB (25248894 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6c7b28a5258684f51bbf3c6bc2fb3215a3965391e08182a8ce25c4ad40d87b50`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 12 Sep 2023 04:43:51 GMT
ARG RELEASE
# Tue, 12 Sep 2023 04:43:51 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 12 Sep 2023 04:43:51 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 12 Sep 2023 04:43:52 GMT
LABEL org.opencontainers.image.version=23.10
# Tue, 12 Sep 2023 04:43:57 GMT
ADD file:3b10dde790011a91258183d8ef7e8ed5e24986b2296e00417509565fdfd45e31 in / 
# Tue, 12 Sep 2023 04:43:57 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:b88dfd009c781b3ca94bb2f78164c028587fdbf1d6c56f41f12b7d8eb03bd975`  
		Last Modified: Tue, 12 Sep 2023 05:02:36 GMT  
		Size: 25.2 MB (25248894 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:23.10` - linux; arm64 variant v8

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

### `ubuntu:23.10` - linux; ppc64le

```console
$ docker pull ubuntu@sha256:b8cd2a5eae36321f5747cc2df64abbaa05e1c14c770fc744d6774067fa89a998
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.4 MB (31370401 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9de077450c3dc8887a07aff9caf353b1d070608a3f884085cddd389662992462`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 12 Sep 2023 04:43:47 GMT
ARG RELEASE
# Tue, 12 Sep 2023 04:43:47 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 12 Sep 2023 04:43:47 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 12 Sep 2023 04:43:47 GMT
LABEL org.opencontainers.image.version=23.10
# Tue, 12 Sep 2023 04:43:50 GMT
ADD file:56d58cbb4273b81f0c1a0b6eaede82f6a7e5d79c78d54525361f0537566dc9ec in / 
# Tue, 12 Sep 2023 04:43:50 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:0b3c414ea1cf4bfd1e808fd228f0b9096a8def2e1f9df113dcfa135d2422b27b`  
		Last Modified: Tue, 12 Sep 2023 05:02:43 GMT  
		Size: 31.4 MB (31370401 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:23.10` - linux; s390x

```console
$ docker pull ubuntu@sha256:f6ba7caa089441d7433604f4371a79fec8d58950cda10bd6d29be8ed899fa3ec
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.9 MB (26908064 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bf7ded0e47b6d77072838e6f9f2b41db1bdf20834e54d02cb325c1880a43cf89`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 12 Sep 2023 04:45:06 GMT
ARG RELEASE
# Tue, 12 Sep 2023 04:45:06 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 12 Sep 2023 04:45:06 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 12 Sep 2023 04:45:06 GMT
LABEL org.opencontainers.image.version=23.10
# Tue, 12 Sep 2023 04:45:08 GMT
ADD file:6724cd2c23f7ec57f0524a81125b059327cf367ea1f3387b48c3f642bddc82b9 in / 
# Tue, 12 Sep 2023 04:45:09 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:2fc3f13b6a87a63eead8aeff863bc67a0870656493725efa7e3cb1cd945c9134`  
		Last Modified: Tue, 12 Sep 2023 05:02:49 GMT  
		Size: 26.9 MB (26908064 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

## `ubuntu:devel`

```console
$ docker pull ubuntu@sha256:3c38c7f067cc8103c300b3ed089a0b916ad5c9852f402a95c6fb8a8cf4b69b23
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
$ docker pull ubuntu@sha256:7e44d7ed904145328785378ddac5de49ac931d3b28b72f6c9f5fb350f9b4a849
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.3 MB (27277147 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1d8801a7ecb54952ea17852be887c1d858fd7bd78dcee093afc11fee7ed53f7c`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 26 Sep 2023 05:03:43 GMT
ARG RELEASE
# Tue, 26 Sep 2023 05:03:43 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 26 Sep 2023 05:03:43 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 26 Sep 2023 05:03:43 GMT
LABEL org.opencontainers.image.version=23.10
# Tue, 26 Sep 2023 05:03:45 GMT
ADD file:5fb49f260a0c3bf404c0fe31d8f0f812e9c143bd48223c4f15a85168758eb880 in / 
# Tue, 26 Sep 2023 05:03:45 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:97e98d3adb77a3f73850e0a81cdde417afce9cd9dce78c444f99b9258caee9fa`  
		Last Modified: Tue, 26 Sep 2023 05:33:55 GMT  
		Size: 27.3 MB (27277147 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:devel` - linux; arm variant v7

```console
$ docker pull ubuntu@sha256:d7e166e923d882bda98249bf852065c7cf27069ff5c5aeb5b8535f0e529c614f
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.2 MB (25248894 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6c7b28a5258684f51bbf3c6bc2fb3215a3965391e08182a8ce25c4ad40d87b50`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 12 Sep 2023 04:43:51 GMT
ARG RELEASE
# Tue, 12 Sep 2023 04:43:51 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 12 Sep 2023 04:43:51 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 12 Sep 2023 04:43:52 GMT
LABEL org.opencontainers.image.version=23.10
# Tue, 12 Sep 2023 04:43:57 GMT
ADD file:3b10dde790011a91258183d8ef7e8ed5e24986b2296e00417509565fdfd45e31 in / 
# Tue, 12 Sep 2023 04:43:57 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:b88dfd009c781b3ca94bb2f78164c028587fdbf1d6c56f41f12b7d8eb03bd975`  
		Last Modified: Tue, 12 Sep 2023 05:02:36 GMT  
		Size: 25.2 MB (25248894 bytes)  
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
$ docker pull ubuntu@sha256:b8cd2a5eae36321f5747cc2df64abbaa05e1c14c770fc744d6774067fa89a998
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.4 MB (31370401 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9de077450c3dc8887a07aff9caf353b1d070608a3f884085cddd389662992462`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 12 Sep 2023 04:43:47 GMT
ARG RELEASE
# Tue, 12 Sep 2023 04:43:47 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 12 Sep 2023 04:43:47 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 12 Sep 2023 04:43:47 GMT
LABEL org.opencontainers.image.version=23.10
# Tue, 12 Sep 2023 04:43:50 GMT
ADD file:56d58cbb4273b81f0c1a0b6eaede82f6a7e5d79c78d54525361f0537566dc9ec in / 
# Tue, 12 Sep 2023 04:43:50 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:0b3c414ea1cf4bfd1e808fd228f0b9096a8def2e1f9df113dcfa135d2422b27b`  
		Last Modified: Tue, 12 Sep 2023 05:02:43 GMT  
		Size: 31.4 MB (31370401 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:devel` - linux; s390x

```console
$ docker pull ubuntu@sha256:f6ba7caa089441d7433604f4371a79fec8d58950cda10bd6d29be8ed899fa3ec
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.9 MB (26908064 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bf7ded0e47b6d77072838e6f9f2b41db1bdf20834e54d02cb325c1880a43cf89`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 12 Sep 2023 04:45:06 GMT
ARG RELEASE
# Tue, 12 Sep 2023 04:45:06 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 12 Sep 2023 04:45:06 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 12 Sep 2023 04:45:06 GMT
LABEL org.opencontainers.image.version=23.10
# Tue, 12 Sep 2023 04:45:08 GMT
ADD file:6724cd2c23f7ec57f0524a81125b059327cf367ea1f3387b48c3f642bddc82b9 in / 
# Tue, 12 Sep 2023 04:45:09 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:2fc3f13b6a87a63eead8aeff863bc67a0870656493725efa7e3cb1cd945c9134`  
		Last Modified: Tue, 12 Sep 2023 05:02:49 GMT  
		Size: 26.9 MB (26908064 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

## `ubuntu:focal`

```console
$ docker pull ubuntu@sha256:33a5cc25d22c45900796a1aca487ad7a7cb09f09ea00b779e3b2026b4fc2faba
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
$ docker pull ubuntu@sha256:3246518d9735254519e1b2ff35f95686e4a5011c90c85344c1f38df7bae9dd37
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.5 MB (27506442 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6df89402372646d400cf092016c28066391a26f5d46c00b1153e75003465484d`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 01 Aug 2023 06:16:43 GMT
ARG RELEASE
# Tue, 01 Aug 2023 06:16:44 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 01 Aug 2023 06:16:44 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 01 Aug 2023 06:16:44 GMT
LABEL org.opencontainers.image.version=20.04
# Tue, 01 Aug 2023 06:16:45 GMT
ADD file:233702cd816c07bc9fed02881b11fb3bdcaee41f3ce3ec1c9f0c4a060b155d5b in / 
# Tue, 01 Aug 2023 06:16:46 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:edaedc954fb53f42a7754a6e2d1b57f091bc9b11063bc445c2e325ea448f8f68`  
		Last Modified: Tue, 01 Aug 2023 06:54:06 GMT  
		Size: 27.5 MB (27506442 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:focal` - linux; arm variant v7

```console
$ docker pull ubuntu@sha256:993dc9215facb1278d78c1ac9aacaf0b10ce01a3319245477b526fb49bb3a85b
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.6 MB (23612645 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9647c2503ec334ee47dc65a547a14f79543680a640b31669e4e417949c03857b`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 01 Aug 2023 06:16:45 GMT
ARG RELEASE
# Tue, 01 Aug 2023 06:16:45 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 01 Aug 2023 06:16:46 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 01 Aug 2023 06:16:46 GMT
LABEL org.opencontainers.image.version=20.04
# Tue, 01 Aug 2023 06:16:49 GMT
ADD file:60aa8465a6ba5538decc41365cc9b78ae86131e8c2cfc9177b4a336354ead988 in / 
# Tue, 01 Aug 2023 06:16:50 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:d2b6ba5e7ade25cef0db07ca410b7d5e09085b9c442b62904956cd4d5a81ad10`  
		Last Modified: Tue, 01 Aug 2023 06:54:18 GMT  
		Size: 23.6 MB (23612645 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:focal` - linux; arm64 variant v8

```console
$ docker pull ubuntu@sha256:af43d52ea8f98c8ab92858a37b87be1805ce16f5300cb38b9958e63ac6b25902
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.0 MB (25974619 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:15c9d636caddd81490d58a714937f112702f9239c98950221e9fd0dd9735df9d`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 01 Aug 2023 06:20:56 GMT
ARG RELEASE
# Tue, 01 Aug 2023 06:20:56 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 01 Aug 2023 06:20:56 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 01 Aug 2023 06:20:57 GMT
LABEL org.opencontainers.image.version=20.04
# Tue, 01 Aug 2023 06:21:03 GMT
ADD file:ef6e767091d76c1461d099d5bc7a18c526ec80834cf87280803ab6480192f766 in / 
# Tue, 01 Aug 2023 06:21:03 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:82d728d38b98752cba7d2d7af8ee1cfe67ccdc5915814420650e78def5d1cebc`  
		Last Modified: Tue, 01 Aug 2023 06:54:12 GMT  
		Size: 26.0 MB (25974619 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:focal` - linux; ppc64le

```console
$ docker pull ubuntu@sha256:a305c3951a3741555d5019870f4827c4becdcc95df539ce7ed364ab5ab2db342
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.1 MB (32070704 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a92643ae09f6e607311cb05e4f0f7679c0873b7e4c235e1b57f5e409cfc47c50`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 01 Aug 2023 06:20:36 GMT
ARG RELEASE
# Tue, 01 Aug 2023 06:20:36 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 01 Aug 2023 06:20:37 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 01 Aug 2023 06:20:37 GMT
LABEL org.opencontainers.image.version=20.04
# Tue, 01 Aug 2023 06:20:40 GMT
ADD file:822df76493d1d533c1a283ab7bb20ce81309f57279422a0eebb2ffb9fab55963 in / 
# Tue, 01 Aug 2023 06:20:40 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:fa78ce4014add322eddde3378405efe21c85e886c0195e18533d5991d5477833`  
		Last Modified: Tue, 01 Aug 2023 06:54:25 GMT  
		Size: 32.1 MB (32070704 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:focal` - linux; s390x

```console
$ docker pull ubuntu@sha256:5ad386cefcdbd1248f73a3bbcfbf529f39864dddcf9497d9a705540afd23e6e9
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.4 MB (26351280 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5079141aa115a82eb5f952b45f4cf336075d4dc4bc3ea2cfdab4351497d2fc9e`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 01 Aug 2023 06:17:39 GMT
ARG RELEASE
# Tue, 01 Aug 2023 06:17:39 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 01 Aug 2023 06:17:39 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 01 Aug 2023 06:17:39 GMT
LABEL org.opencontainers.image.version=20.04
# Tue, 01 Aug 2023 06:17:41 GMT
ADD file:36efc3ec29bb54e0987fe91be1aa7cc849909b3cd2534af3de2d3d07a03804cf in / 
# Tue, 01 Aug 2023 06:17:41 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:773e1d05400f41114172ea2dbaa16f037c5812b7d1092cbf0df5d19e69586402`  
		Last Modified: Tue, 01 Aug 2023 06:54:31 GMT  
		Size: 26.4 MB (26351280 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

## `ubuntu:focal-20230801`

```console
$ docker pull ubuntu@sha256:33a5cc25d22c45900796a1aca487ad7a7cb09f09ea00b779e3b2026b4fc2faba
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `ubuntu:focal-20230801` - linux; amd64

```console
$ docker pull ubuntu@sha256:3246518d9735254519e1b2ff35f95686e4a5011c90c85344c1f38df7bae9dd37
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.5 MB (27506442 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6df89402372646d400cf092016c28066391a26f5d46c00b1153e75003465484d`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 01 Aug 2023 06:16:43 GMT
ARG RELEASE
# Tue, 01 Aug 2023 06:16:44 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 01 Aug 2023 06:16:44 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 01 Aug 2023 06:16:44 GMT
LABEL org.opencontainers.image.version=20.04
# Tue, 01 Aug 2023 06:16:45 GMT
ADD file:233702cd816c07bc9fed02881b11fb3bdcaee41f3ce3ec1c9f0c4a060b155d5b in / 
# Tue, 01 Aug 2023 06:16:46 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:edaedc954fb53f42a7754a6e2d1b57f091bc9b11063bc445c2e325ea448f8f68`  
		Last Modified: Tue, 01 Aug 2023 06:54:06 GMT  
		Size: 27.5 MB (27506442 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:focal-20230801` - linux; arm variant v7

```console
$ docker pull ubuntu@sha256:993dc9215facb1278d78c1ac9aacaf0b10ce01a3319245477b526fb49bb3a85b
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.6 MB (23612645 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9647c2503ec334ee47dc65a547a14f79543680a640b31669e4e417949c03857b`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 01 Aug 2023 06:16:45 GMT
ARG RELEASE
# Tue, 01 Aug 2023 06:16:45 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 01 Aug 2023 06:16:46 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 01 Aug 2023 06:16:46 GMT
LABEL org.opencontainers.image.version=20.04
# Tue, 01 Aug 2023 06:16:49 GMT
ADD file:60aa8465a6ba5538decc41365cc9b78ae86131e8c2cfc9177b4a336354ead988 in / 
# Tue, 01 Aug 2023 06:16:50 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:d2b6ba5e7ade25cef0db07ca410b7d5e09085b9c442b62904956cd4d5a81ad10`  
		Last Modified: Tue, 01 Aug 2023 06:54:18 GMT  
		Size: 23.6 MB (23612645 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:focal-20230801` - linux; arm64 variant v8

```console
$ docker pull ubuntu@sha256:af43d52ea8f98c8ab92858a37b87be1805ce16f5300cb38b9958e63ac6b25902
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.0 MB (25974619 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:15c9d636caddd81490d58a714937f112702f9239c98950221e9fd0dd9735df9d`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 01 Aug 2023 06:20:56 GMT
ARG RELEASE
# Tue, 01 Aug 2023 06:20:56 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 01 Aug 2023 06:20:56 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 01 Aug 2023 06:20:57 GMT
LABEL org.opencontainers.image.version=20.04
# Tue, 01 Aug 2023 06:21:03 GMT
ADD file:ef6e767091d76c1461d099d5bc7a18c526ec80834cf87280803ab6480192f766 in / 
# Tue, 01 Aug 2023 06:21:03 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:82d728d38b98752cba7d2d7af8ee1cfe67ccdc5915814420650e78def5d1cebc`  
		Last Modified: Tue, 01 Aug 2023 06:54:12 GMT  
		Size: 26.0 MB (25974619 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:focal-20230801` - linux; ppc64le

```console
$ docker pull ubuntu@sha256:a305c3951a3741555d5019870f4827c4becdcc95df539ce7ed364ab5ab2db342
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.1 MB (32070704 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a92643ae09f6e607311cb05e4f0f7679c0873b7e4c235e1b57f5e409cfc47c50`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 01 Aug 2023 06:20:36 GMT
ARG RELEASE
# Tue, 01 Aug 2023 06:20:36 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 01 Aug 2023 06:20:37 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 01 Aug 2023 06:20:37 GMT
LABEL org.opencontainers.image.version=20.04
# Tue, 01 Aug 2023 06:20:40 GMT
ADD file:822df76493d1d533c1a283ab7bb20ce81309f57279422a0eebb2ffb9fab55963 in / 
# Tue, 01 Aug 2023 06:20:40 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:fa78ce4014add322eddde3378405efe21c85e886c0195e18533d5991d5477833`  
		Last Modified: Tue, 01 Aug 2023 06:54:25 GMT  
		Size: 32.1 MB (32070704 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:focal-20230801` - linux; s390x

```console
$ docker pull ubuntu@sha256:5ad386cefcdbd1248f73a3bbcfbf529f39864dddcf9497d9a705540afd23e6e9
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.4 MB (26351280 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5079141aa115a82eb5f952b45f4cf336075d4dc4bc3ea2cfdab4351497d2fc9e`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 01 Aug 2023 06:17:39 GMT
ARG RELEASE
# Tue, 01 Aug 2023 06:17:39 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 01 Aug 2023 06:17:39 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 01 Aug 2023 06:17:39 GMT
LABEL org.opencontainers.image.version=20.04
# Tue, 01 Aug 2023 06:17:41 GMT
ADD file:36efc3ec29bb54e0987fe91be1aa7cc849909b3cd2534af3de2d3d07a03804cf in / 
# Tue, 01 Aug 2023 06:17:41 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:773e1d05400f41114172ea2dbaa16f037c5812b7d1092cbf0df5d19e69586402`  
		Last Modified: Tue, 01 Aug 2023 06:54:31 GMT  
		Size: 26.4 MB (26351280 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

## `ubuntu:jammy`

```console
$ docker pull ubuntu@sha256:c1a4fb1fd1697920c2a422a355783a9debaf57b8eb6c92de84a75ce5be34c6cb
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
$ docker pull ubuntu@sha256:b4b521bfcec90b11d2869e00fe1f2380c21cbfcd799ee35df8bd7ac09e6f63ea
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.5 MB (29538209 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3565a89d9e81a4cb4cb2b0d947c7c11227a3f358dc216d19fc54bfd77cd5b542`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 25 Sep 2023 10:17:05 GMT
ARG RELEASE
# Mon, 25 Sep 2023 10:17:05 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 25 Sep 2023 10:17:05 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 25 Sep 2023 10:17:05 GMT
LABEL org.opencontainers.image.version=22.04
# Mon, 25 Sep 2023 10:17:07 GMT
ADD file:194c886b88876c1804cc5f80719669653c16a388b664147b7f22402105f533c4 in / 
# Mon, 25 Sep 2023 10:17:08 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:37aaf24cf781dcc5b9a4f8aa5a99a40b60ae45d64dcb4f6d5a4b9e5ab7ab0894`  
		Last Modified: Mon, 25 Sep 2023 10:30:37 GMT  
		Size: 29.5 MB (29538209 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:jammy` - linux; arm variant v7

```console
$ docker pull ubuntu@sha256:2589fe6bcf90466564741ae0d8309d1323f33b6ec8a5d401a62d0b256bcc3c37
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.1 MB (26142545 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5edd8b11048dd1910bbeeae6325888a34a64e8a0d2576b6d843063825b339cd1`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 16 Aug 2023 06:08:27 GMT
ARG RELEASE
# Wed, 16 Aug 2023 06:08:27 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 16 Aug 2023 06:08:27 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 16 Aug 2023 06:08:27 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 16 Aug 2023 06:08:32 GMT
ADD file:e61c6bbfc8728cb119b4cfd4a35d1e5aad76e84c0ac8f2ff9850a7ceec9f3dc5 in / 
# Wed, 16 Aug 2023 06:08:32 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:d79cf5fbd02b4f64ddfb1ba3ae0178a904f012bc2ff0e5603ffdb4668a8f529c`  
		Last Modified: Wed, 16 Aug 2023 06:32:59 GMT  
		Size: 26.1 MB (26142545 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:jammy` - linux; arm64 variant v8

```console
$ docker pull ubuntu@sha256:f58b48967ecc767fc238144ffdb7eb668cefcc8438de8f8a59c4cefbbf29b323
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.4 MB (27351199 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bf9e5b7213b4e0d99cddc039011cc60bfd76ed5ef63bbd837ab0b8416c305c39`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 25 Sep 2023 10:17:41 GMT
ARG RELEASE
# Mon, 25 Sep 2023 10:17:41 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 25 Sep 2023 10:17:41 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 25 Sep 2023 10:17:41 GMT
LABEL org.opencontainers.image.version=22.04
# Mon, 25 Sep 2023 10:17:44 GMT
ADD file:8540670760767f19eaf101fbce1da1881a2f24a7d65da6abdedc644b8fb00463 in / 
# Mon, 25 Sep 2023 10:17:45 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:c391327a0f1df5790bcb00ac010a1a3924c9e4387ce36b290bc16fd9f4cc5740`  
		Last Modified: Mon, 25 Sep 2023 10:30:43 GMT  
		Size: 27.4 MB (27351199 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:jammy` - linux; ppc64le

```console
$ docker pull ubuntu@sha256:de1fcbe2d7e928d0be9476e3079df8e69072dfb140be94f5d34091f09f6917dd
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.6 MB (34567229 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b67aa2427a930674989cafcaf3fa7d1d16b2c47ed37003fe712bcbf5bc07a6fc`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 16 Aug 2023 06:03:07 GMT
ARG RELEASE
# Wed, 16 Aug 2023 06:03:07 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 16 Aug 2023 06:03:08 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 16 Aug 2023 06:03:08 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 16 Aug 2023 06:03:11 GMT
ADD file:632018deeaeb9e42f0026fb331dfb08381e46bd414b2b470b18ea22ac0653bf6 in / 
# Wed, 16 Aug 2023 06:03:11 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:c76fbfef684586d44d4a79c1a2c093ecf60b0f6c5deb0742082a5152ecd9a1fa`  
		Last Modified: Wed, 16 Aug 2023 06:33:06 GMT  
		Size: 34.6 MB (34567229 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:jammy` - linux; s390x

```console
$ docker pull ubuntu@sha256:ed1a67bb47f3c35d782293229127ac1f8d64873a131186c49fe079dada0fa7e0
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.0 MB (28016004 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f34a6de6626fe032cc2ff34b644898f997ccd85378e081b63c95246ad6b11e3d`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 16 Aug 2023 06:05:03 GMT
ARG RELEASE
# Wed, 16 Aug 2023 06:05:03 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 16 Aug 2023 06:05:03 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 16 Aug 2023 06:05:03 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 16 Aug 2023 06:05:05 GMT
ADD file:58eccd685d73ff80ea235016d6e33d093e1063800d869935b67b59a1b8891344 in / 
# Wed, 16 Aug 2023 06:05:05 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:e1b6153f78cbd4f98e7250bc413a393734736138dcb57f1e41f45c3e43c5a120`  
		Last Modified: Wed, 16 Aug 2023 06:33:12 GMT  
		Size: 28.0 MB (28016004 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

## `ubuntu:jammy-20230916`

```console
$ docker pull ubuntu@sha256:983505be8424b9f630e72530ff5b4815537e5bec4c3b717d96a82b047f0bb405
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ubuntu:jammy-20230916` - linux; amd64

```console
$ docker pull ubuntu@sha256:b4b521bfcec90b11d2869e00fe1f2380c21cbfcd799ee35df8bd7ac09e6f63ea
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.5 MB (29538209 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3565a89d9e81a4cb4cb2b0d947c7c11227a3f358dc216d19fc54bfd77cd5b542`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 25 Sep 2023 10:17:05 GMT
ARG RELEASE
# Mon, 25 Sep 2023 10:17:05 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 25 Sep 2023 10:17:05 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 25 Sep 2023 10:17:05 GMT
LABEL org.opencontainers.image.version=22.04
# Mon, 25 Sep 2023 10:17:07 GMT
ADD file:194c886b88876c1804cc5f80719669653c16a388b664147b7f22402105f533c4 in / 
# Mon, 25 Sep 2023 10:17:08 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:37aaf24cf781dcc5b9a4f8aa5a99a40b60ae45d64dcb4f6d5a4b9e5ab7ab0894`  
		Last Modified: Mon, 25 Sep 2023 10:30:37 GMT  
		Size: 29.5 MB (29538209 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:jammy-20230916` - linux; arm64 variant v8

```console
$ docker pull ubuntu@sha256:f58b48967ecc767fc238144ffdb7eb668cefcc8438de8f8a59c4cefbbf29b323
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.4 MB (27351199 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bf9e5b7213b4e0d99cddc039011cc60bfd76ed5ef63bbd837ab0b8416c305c39`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 25 Sep 2023 10:17:41 GMT
ARG RELEASE
# Mon, 25 Sep 2023 10:17:41 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 25 Sep 2023 10:17:41 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 25 Sep 2023 10:17:41 GMT
LABEL org.opencontainers.image.version=22.04
# Mon, 25 Sep 2023 10:17:44 GMT
ADD file:8540670760767f19eaf101fbce1da1881a2f24a7d65da6abdedc644b8fb00463 in / 
# Mon, 25 Sep 2023 10:17:45 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:c391327a0f1df5790bcb00ac010a1a3924c9e4387ce36b290bc16fd9f4cc5740`  
		Last Modified: Mon, 25 Sep 2023 10:30:43 GMT  
		Size: 27.4 MB (27351199 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

## `ubuntu:latest`

```console
$ docker pull ubuntu@sha256:c1a4fb1fd1697920c2a422a355783a9debaf57b8eb6c92de84a75ce5be34c6cb
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
$ docker pull ubuntu@sha256:b4b521bfcec90b11d2869e00fe1f2380c21cbfcd799ee35df8bd7ac09e6f63ea
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.5 MB (29538209 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3565a89d9e81a4cb4cb2b0d947c7c11227a3f358dc216d19fc54bfd77cd5b542`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 25 Sep 2023 10:17:05 GMT
ARG RELEASE
# Mon, 25 Sep 2023 10:17:05 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 25 Sep 2023 10:17:05 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 25 Sep 2023 10:17:05 GMT
LABEL org.opencontainers.image.version=22.04
# Mon, 25 Sep 2023 10:17:07 GMT
ADD file:194c886b88876c1804cc5f80719669653c16a388b664147b7f22402105f533c4 in / 
# Mon, 25 Sep 2023 10:17:08 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:37aaf24cf781dcc5b9a4f8aa5a99a40b60ae45d64dcb4f6d5a4b9e5ab7ab0894`  
		Last Modified: Mon, 25 Sep 2023 10:30:37 GMT  
		Size: 29.5 MB (29538209 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:latest` - linux; arm variant v7

```console
$ docker pull ubuntu@sha256:2589fe6bcf90466564741ae0d8309d1323f33b6ec8a5d401a62d0b256bcc3c37
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.1 MB (26142545 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5edd8b11048dd1910bbeeae6325888a34a64e8a0d2576b6d843063825b339cd1`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 16 Aug 2023 06:08:27 GMT
ARG RELEASE
# Wed, 16 Aug 2023 06:08:27 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 16 Aug 2023 06:08:27 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 16 Aug 2023 06:08:27 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 16 Aug 2023 06:08:32 GMT
ADD file:e61c6bbfc8728cb119b4cfd4a35d1e5aad76e84c0ac8f2ff9850a7ceec9f3dc5 in / 
# Wed, 16 Aug 2023 06:08:32 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:d79cf5fbd02b4f64ddfb1ba3ae0178a904f012bc2ff0e5603ffdb4668a8f529c`  
		Last Modified: Wed, 16 Aug 2023 06:32:59 GMT  
		Size: 26.1 MB (26142545 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:latest` - linux; arm64 variant v8

```console
$ docker pull ubuntu@sha256:f58b48967ecc767fc238144ffdb7eb668cefcc8438de8f8a59c4cefbbf29b323
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.4 MB (27351199 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bf9e5b7213b4e0d99cddc039011cc60bfd76ed5ef63bbd837ab0b8416c305c39`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 25 Sep 2023 10:17:41 GMT
ARG RELEASE
# Mon, 25 Sep 2023 10:17:41 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 25 Sep 2023 10:17:41 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 25 Sep 2023 10:17:41 GMT
LABEL org.opencontainers.image.version=22.04
# Mon, 25 Sep 2023 10:17:44 GMT
ADD file:8540670760767f19eaf101fbce1da1881a2f24a7d65da6abdedc644b8fb00463 in / 
# Mon, 25 Sep 2023 10:17:45 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:c391327a0f1df5790bcb00ac010a1a3924c9e4387ce36b290bc16fd9f4cc5740`  
		Last Modified: Mon, 25 Sep 2023 10:30:43 GMT  
		Size: 27.4 MB (27351199 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:latest` - linux; ppc64le

```console
$ docker pull ubuntu@sha256:de1fcbe2d7e928d0be9476e3079df8e69072dfb140be94f5d34091f09f6917dd
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.6 MB (34567229 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b67aa2427a930674989cafcaf3fa7d1d16b2c47ed37003fe712bcbf5bc07a6fc`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 16 Aug 2023 06:03:07 GMT
ARG RELEASE
# Wed, 16 Aug 2023 06:03:07 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 16 Aug 2023 06:03:08 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 16 Aug 2023 06:03:08 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 16 Aug 2023 06:03:11 GMT
ADD file:632018deeaeb9e42f0026fb331dfb08381e46bd414b2b470b18ea22ac0653bf6 in / 
# Wed, 16 Aug 2023 06:03:11 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:c76fbfef684586d44d4a79c1a2c093ecf60b0f6c5deb0742082a5152ecd9a1fa`  
		Last Modified: Wed, 16 Aug 2023 06:33:06 GMT  
		Size: 34.6 MB (34567229 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:latest` - linux; s390x

```console
$ docker pull ubuntu@sha256:ed1a67bb47f3c35d782293229127ac1f8d64873a131186c49fe079dada0fa7e0
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.0 MB (28016004 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f34a6de6626fe032cc2ff34b644898f997ccd85378e081b63c95246ad6b11e3d`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 16 Aug 2023 06:05:03 GMT
ARG RELEASE
# Wed, 16 Aug 2023 06:05:03 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 16 Aug 2023 06:05:03 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 16 Aug 2023 06:05:03 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 16 Aug 2023 06:05:05 GMT
ADD file:58eccd685d73ff80ea235016d6e33d093e1063800d869935b67b59a1b8891344 in / 
# Wed, 16 Aug 2023 06:05:05 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:e1b6153f78cbd4f98e7250bc413a393734736138dcb57f1e41f45c3e43c5a120`  
		Last Modified: Wed, 16 Aug 2023 06:33:12 GMT  
		Size: 28.0 MB (28016004 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

## `ubuntu:lunar`

```console
$ docker pull ubuntu@sha256:f1090cfa89ab321a6d670e79652f61593502591f2fc7452fb0b7c6da575729c4
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
$ docker pull ubuntu@sha256:24898c8e1ac370d2d309d6d9df56af52bebdad86925c623b5e87e12404453518
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.9 MB (26873617 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:21098a29e034a8f6f1952d1d8a49b5732b70e532c31f0e88e1ff499c6540c57c`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 16 Aug 2023 04:28:31 GMT
ARG RELEASE
# Wed, 16 Aug 2023 04:28:31 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 16 Aug 2023 04:28:31 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 16 Aug 2023 04:28:31 GMT
LABEL org.opencontainers.image.version=23.04
# Wed, 16 Aug 2023 04:28:32 GMT
ADD file:7392bed4dbab9fb7c9ad5bde6f3bfcde3bcbf1885c336af9c231af6defaa31e1 in / 
# Wed, 16 Aug 2023 04:28:33 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:10fb01f4f619bc954ba611cebca23f2b96d255c7ead4040b449f063e530df1a4`  
		Last Modified: Wed, 16 Aug 2023 04:34:32 GMT  
		Size: 26.9 MB (26873617 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:lunar` - linux; arm variant v7

```console
$ docker pull ubuntu@sha256:1e9568cacc4bd0a59a44d8e68ae8fc5f4287c132d455492881f7a1106b722beb
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **24.6 MB (24627247 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e46f21739314ec025a0ce92c7a657ddb65785a29870d74435a08554207fb3688`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 16 Aug 2023 04:16:11 GMT
ARG RELEASE
# Wed, 16 Aug 2023 04:16:11 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 16 Aug 2023 04:16:11 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 16 Aug 2023 04:16:11 GMT
LABEL org.opencontainers.image.version=23.04
# Wed, 16 Aug 2023 04:16:16 GMT
ADD file:1f1c9502544acdbb6a7450226ced78cfe982a6305f2aea77ab7d1f73b50fc7f0 in / 
# Wed, 16 Aug 2023 04:16:16 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:e05ef4abc6c76087042349392d272a7eeb590834dc45d1247295302c212fda9d`  
		Last Modified: Wed, 16 Aug 2023 04:34:45 GMT  
		Size: 24.6 MB (24627247 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:lunar` - linux; arm64 variant v8

```console
$ docker pull ubuntu@sha256:d68d8bcae123a839bc72b91fa9df55956be3fcb2dbfc247acb7f65908eaa6c35
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.1 MB (26064545 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e1c8e9335de75964dd320b20b4290408432be2962faf7ad36d3a47d48f3131cd`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 16 Aug 2023 04:15:57 GMT
ARG RELEASE
# Wed, 16 Aug 2023 04:15:57 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 16 Aug 2023 04:15:57 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 16 Aug 2023 04:15:57 GMT
LABEL org.opencontainers.image.version=23.04
# Wed, 16 Aug 2023 04:16:01 GMT
ADD file:adea2962926b29b76eb8da76ae9e830c5ad7050ae9b19f5427191b338c8a2c56 in / 
# Wed, 16 Aug 2023 04:16:02 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:2b2d15932a31f0857b9499cc218b8777708cb1d73ae6ef680f624ca7d4342763`  
		Last Modified: Wed, 16 Aug 2023 04:34:39 GMT  
		Size: 26.1 MB (26064545 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:lunar` - linux; ppc64le

```console
$ docker pull ubuntu@sha256:1306e75f505a2305f2c46f51f33be8b8599923bd5a652c3b5dc37333db4f44ab
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.9 MB (30905042 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:91733a8763fe80d6e620ec400c2721ee45c0f80398506088d1278d6531299a90`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 16 Aug 2023 04:16:31 GMT
ARG RELEASE
# Wed, 16 Aug 2023 04:16:31 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 16 Aug 2023 04:16:31 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 16 Aug 2023 04:16:31 GMT
LABEL org.opencontainers.image.version=23.04
# Wed, 16 Aug 2023 04:16:34 GMT
ADD file:a9d35b320d969ee1ae8a7bc83aba49da30d93724befb5948c680066ad4f1acdf in / 
# Wed, 16 Aug 2023 04:16:35 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:f51cbff870f31d4c4397c2f21529046998f8d6e7748fd6f059b325a0759c7dd4`  
		Last Modified: Wed, 16 Aug 2023 04:34:51 GMT  
		Size: 30.9 MB (30905042 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:lunar` - linux; s390x

```console
$ docker pull ubuntu@sha256:ec9620bbf89d1a3b1171f961340a890166607be3423d96e740f6d56f36ccb125
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.7 MB (25691524 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1289eb3132a14bc161676d7f928d557bf63eb8561718e9d5247e16e88ebee8ff`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 16 Aug 2023 04:29:27 GMT
ARG RELEASE
# Wed, 16 Aug 2023 04:29:28 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 16 Aug 2023 04:29:28 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 16 Aug 2023 04:29:28 GMT
LABEL org.opencontainers.image.version=23.04
# Wed, 16 Aug 2023 04:29:29 GMT
ADD file:14fcf0756fb29b609af54412c31e2ff9acbf4634984ce95bf204c67668706cb5 in / 
# Wed, 16 Aug 2023 04:29:30 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:b1e434384d3d3b546e155df0cf143c8c0a92bf766c6808bf2e3e1d2f22010839`  
		Last Modified: Wed, 16 Aug 2023 04:34:57 GMT  
		Size: 25.7 MB (25691524 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

## `ubuntu:lunar-20230816`

```console
$ docker pull ubuntu@sha256:f1090cfa89ab321a6d670e79652f61593502591f2fc7452fb0b7c6da575729c4
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `ubuntu:lunar-20230816` - linux; amd64

```console
$ docker pull ubuntu@sha256:24898c8e1ac370d2d309d6d9df56af52bebdad86925c623b5e87e12404453518
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.9 MB (26873617 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:21098a29e034a8f6f1952d1d8a49b5732b70e532c31f0e88e1ff499c6540c57c`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 16 Aug 2023 04:28:31 GMT
ARG RELEASE
# Wed, 16 Aug 2023 04:28:31 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 16 Aug 2023 04:28:31 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 16 Aug 2023 04:28:31 GMT
LABEL org.opencontainers.image.version=23.04
# Wed, 16 Aug 2023 04:28:32 GMT
ADD file:7392bed4dbab9fb7c9ad5bde6f3bfcde3bcbf1885c336af9c231af6defaa31e1 in / 
# Wed, 16 Aug 2023 04:28:33 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:10fb01f4f619bc954ba611cebca23f2b96d255c7ead4040b449f063e530df1a4`  
		Last Modified: Wed, 16 Aug 2023 04:34:32 GMT  
		Size: 26.9 MB (26873617 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:lunar-20230816` - linux; arm variant v7

```console
$ docker pull ubuntu@sha256:1e9568cacc4bd0a59a44d8e68ae8fc5f4287c132d455492881f7a1106b722beb
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **24.6 MB (24627247 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e46f21739314ec025a0ce92c7a657ddb65785a29870d74435a08554207fb3688`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 16 Aug 2023 04:16:11 GMT
ARG RELEASE
# Wed, 16 Aug 2023 04:16:11 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 16 Aug 2023 04:16:11 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 16 Aug 2023 04:16:11 GMT
LABEL org.opencontainers.image.version=23.04
# Wed, 16 Aug 2023 04:16:16 GMT
ADD file:1f1c9502544acdbb6a7450226ced78cfe982a6305f2aea77ab7d1f73b50fc7f0 in / 
# Wed, 16 Aug 2023 04:16:16 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:e05ef4abc6c76087042349392d272a7eeb590834dc45d1247295302c212fda9d`  
		Last Modified: Wed, 16 Aug 2023 04:34:45 GMT  
		Size: 24.6 MB (24627247 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:lunar-20230816` - linux; arm64 variant v8

```console
$ docker pull ubuntu@sha256:d68d8bcae123a839bc72b91fa9df55956be3fcb2dbfc247acb7f65908eaa6c35
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.1 MB (26064545 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e1c8e9335de75964dd320b20b4290408432be2962faf7ad36d3a47d48f3131cd`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 16 Aug 2023 04:15:57 GMT
ARG RELEASE
# Wed, 16 Aug 2023 04:15:57 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 16 Aug 2023 04:15:57 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 16 Aug 2023 04:15:57 GMT
LABEL org.opencontainers.image.version=23.04
# Wed, 16 Aug 2023 04:16:01 GMT
ADD file:adea2962926b29b76eb8da76ae9e830c5ad7050ae9b19f5427191b338c8a2c56 in / 
# Wed, 16 Aug 2023 04:16:02 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:2b2d15932a31f0857b9499cc218b8777708cb1d73ae6ef680f624ca7d4342763`  
		Last Modified: Wed, 16 Aug 2023 04:34:39 GMT  
		Size: 26.1 MB (26064545 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:lunar-20230816` - linux; ppc64le

```console
$ docker pull ubuntu@sha256:1306e75f505a2305f2c46f51f33be8b8599923bd5a652c3b5dc37333db4f44ab
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.9 MB (30905042 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:91733a8763fe80d6e620ec400c2721ee45c0f80398506088d1278d6531299a90`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 16 Aug 2023 04:16:31 GMT
ARG RELEASE
# Wed, 16 Aug 2023 04:16:31 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 16 Aug 2023 04:16:31 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 16 Aug 2023 04:16:31 GMT
LABEL org.opencontainers.image.version=23.04
# Wed, 16 Aug 2023 04:16:34 GMT
ADD file:a9d35b320d969ee1ae8a7bc83aba49da30d93724befb5948c680066ad4f1acdf in / 
# Wed, 16 Aug 2023 04:16:35 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:f51cbff870f31d4c4397c2f21529046998f8d6e7748fd6f059b325a0759c7dd4`  
		Last Modified: Wed, 16 Aug 2023 04:34:51 GMT  
		Size: 30.9 MB (30905042 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:lunar-20230816` - linux; s390x

```console
$ docker pull ubuntu@sha256:ec9620bbf89d1a3b1171f961340a890166607be3423d96e740f6d56f36ccb125
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.7 MB (25691524 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1289eb3132a14bc161676d7f928d557bf63eb8561718e9d5247e16e88ebee8ff`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 16 Aug 2023 04:29:27 GMT
ARG RELEASE
# Wed, 16 Aug 2023 04:29:28 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 16 Aug 2023 04:29:28 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 16 Aug 2023 04:29:28 GMT
LABEL org.opencontainers.image.version=23.04
# Wed, 16 Aug 2023 04:29:29 GMT
ADD file:14fcf0756fb29b609af54412c31e2ff9acbf4634984ce95bf204c67668706cb5 in / 
# Wed, 16 Aug 2023 04:29:30 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:b1e434384d3d3b546e155df0cf143c8c0a92bf766c6808bf2e3e1d2f22010839`  
		Last Modified: Wed, 16 Aug 2023 04:34:57 GMT  
		Size: 25.7 MB (25691524 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

## `ubuntu:mantic`

```console
$ docker pull ubuntu@sha256:3c38c7f067cc8103c300b3ed089a0b916ad5c9852f402a95c6fb8a8cf4b69b23
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
$ docker pull ubuntu@sha256:7e44d7ed904145328785378ddac5de49ac931d3b28b72f6c9f5fb350f9b4a849
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.3 MB (27277147 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1d8801a7ecb54952ea17852be887c1d858fd7bd78dcee093afc11fee7ed53f7c`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 26 Sep 2023 05:03:43 GMT
ARG RELEASE
# Tue, 26 Sep 2023 05:03:43 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 26 Sep 2023 05:03:43 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 26 Sep 2023 05:03:43 GMT
LABEL org.opencontainers.image.version=23.10
# Tue, 26 Sep 2023 05:03:45 GMT
ADD file:5fb49f260a0c3bf404c0fe31d8f0f812e9c143bd48223c4f15a85168758eb880 in / 
# Tue, 26 Sep 2023 05:03:45 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:97e98d3adb77a3f73850e0a81cdde417afce9cd9dce78c444f99b9258caee9fa`  
		Last Modified: Tue, 26 Sep 2023 05:33:55 GMT  
		Size: 27.3 MB (27277147 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:mantic` - linux; arm variant v7

```console
$ docker pull ubuntu@sha256:d7e166e923d882bda98249bf852065c7cf27069ff5c5aeb5b8535f0e529c614f
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.2 MB (25248894 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6c7b28a5258684f51bbf3c6bc2fb3215a3965391e08182a8ce25c4ad40d87b50`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 12 Sep 2023 04:43:51 GMT
ARG RELEASE
# Tue, 12 Sep 2023 04:43:51 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 12 Sep 2023 04:43:51 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 12 Sep 2023 04:43:52 GMT
LABEL org.opencontainers.image.version=23.10
# Tue, 12 Sep 2023 04:43:57 GMT
ADD file:3b10dde790011a91258183d8ef7e8ed5e24986b2296e00417509565fdfd45e31 in / 
# Tue, 12 Sep 2023 04:43:57 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:b88dfd009c781b3ca94bb2f78164c028587fdbf1d6c56f41f12b7d8eb03bd975`  
		Last Modified: Tue, 12 Sep 2023 05:02:36 GMT  
		Size: 25.2 MB (25248894 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:mantic` - linux; arm64 variant v8

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

### `ubuntu:mantic` - linux; ppc64le

```console
$ docker pull ubuntu@sha256:b8cd2a5eae36321f5747cc2df64abbaa05e1c14c770fc744d6774067fa89a998
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.4 MB (31370401 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9de077450c3dc8887a07aff9caf353b1d070608a3f884085cddd389662992462`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 12 Sep 2023 04:43:47 GMT
ARG RELEASE
# Tue, 12 Sep 2023 04:43:47 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 12 Sep 2023 04:43:47 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 12 Sep 2023 04:43:47 GMT
LABEL org.opencontainers.image.version=23.10
# Tue, 12 Sep 2023 04:43:50 GMT
ADD file:56d58cbb4273b81f0c1a0b6eaede82f6a7e5d79c78d54525361f0537566dc9ec in / 
# Tue, 12 Sep 2023 04:43:50 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:0b3c414ea1cf4bfd1e808fd228f0b9096a8def2e1f9df113dcfa135d2422b27b`  
		Last Modified: Tue, 12 Sep 2023 05:02:43 GMT  
		Size: 31.4 MB (31370401 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:mantic` - linux; s390x

```console
$ docker pull ubuntu@sha256:f6ba7caa089441d7433604f4371a79fec8d58950cda10bd6d29be8ed899fa3ec
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.9 MB (26908064 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bf7ded0e47b6d77072838e6f9f2b41db1bdf20834e54d02cb325c1880a43cf89`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 12 Sep 2023 04:45:06 GMT
ARG RELEASE
# Tue, 12 Sep 2023 04:45:06 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 12 Sep 2023 04:45:06 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 12 Sep 2023 04:45:06 GMT
LABEL org.opencontainers.image.version=23.10
# Tue, 12 Sep 2023 04:45:08 GMT
ADD file:6724cd2c23f7ec57f0524a81125b059327cf367ea1f3387b48c3f642bddc82b9 in / 
# Tue, 12 Sep 2023 04:45:09 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:2fc3f13b6a87a63eead8aeff863bc67a0870656493725efa7e3cb1cd945c9134`  
		Last Modified: Tue, 12 Sep 2023 05:02:49 GMT  
		Size: 26.9 MB (26908064 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

## `ubuntu:mantic-20230926`

```console
$ docker pull ubuntu@sha256:7624e069ad985d6065a1142a0234ee16c79fc8e1f165820a0bf1df87b68dda3e
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ubuntu:mantic-20230926` - linux; amd64

```console
$ docker pull ubuntu@sha256:7e44d7ed904145328785378ddac5de49ac931d3b28b72f6c9f5fb350f9b4a849
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.3 MB (27277147 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1d8801a7ecb54952ea17852be887c1d858fd7bd78dcee093afc11fee7ed53f7c`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 26 Sep 2023 05:03:43 GMT
ARG RELEASE
# Tue, 26 Sep 2023 05:03:43 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 26 Sep 2023 05:03:43 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 26 Sep 2023 05:03:43 GMT
LABEL org.opencontainers.image.version=23.10
# Tue, 26 Sep 2023 05:03:45 GMT
ADD file:5fb49f260a0c3bf404c0fe31d8f0f812e9c143bd48223c4f15a85168758eb880 in / 
# Tue, 26 Sep 2023 05:03:45 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:97e98d3adb77a3f73850e0a81cdde417afce9cd9dce78c444f99b9258caee9fa`  
		Last Modified: Tue, 26 Sep 2023 05:33:55 GMT  
		Size: 27.3 MB (27277147 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:mantic-20230926` - linux; arm64 variant v8

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

## `ubuntu:rolling`

```console
$ docker pull ubuntu@sha256:f1090cfa89ab321a6d670e79652f61593502591f2fc7452fb0b7c6da575729c4
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
$ docker pull ubuntu@sha256:24898c8e1ac370d2d309d6d9df56af52bebdad86925c623b5e87e12404453518
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.9 MB (26873617 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:21098a29e034a8f6f1952d1d8a49b5732b70e532c31f0e88e1ff499c6540c57c`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 16 Aug 2023 04:28:31 GMT
ARG RELEASE
# Wed, 16 Aug 2023 04:28:31 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 16 Aug 2023 04:28:31 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 16 Aug 2023 04:28:31 GMT
LABEL org.opencontainers.image.version=23.04
# Wed, 16 Aug 2023 04:28:32 GMT
ADD file:7392bed4dbab9fb7c9ad5bde6f3bfcde3bcbf1885c336af9c231af6defaa31e1 in / 
# Wed, 16 Aug 2023 04:28:33 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:10fb01f4f619bc954ba611cebca23f2b96d255c7ead4040b449f063e530df1a4`  
		Last Modified: Wed, 16 Aug 2023 04:34:32 GMT  
		Size: 26.9 MB (26873617 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:rolling` - linux; arm variant v7

```console
$ docker pull ubuntu@sha256:1e9568cacc4bd0a59a44d8e68ae8fc5f4287c132d455492881f7a1106b722beb
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **24.6 MB (24627247 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e46f21739314ec025a0ce92c7a657ddb65785a29870d74435a08554207fb3688`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 16 Aug 2023 04:16:11 GMT
ARG RELEASE
# Wed, 16 Aug 2023 04:16:11 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 16 Aug 2023 04:16:11 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 16 Aug 2023 04:16:11 GMT
LABEL org.opencontainers.image.version=23.04
# Wed, 16 Aug 2023 04:16:16 GMT
ADD file:1f1c9502544acdbb6a7450226ced78cfe982a6305f2aea77ab7d1f73b50fc7f0 in / 
# Wed, 16 Aug 2023 04:16:16 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:e05ef4abc6c76087042349392d272a7eeb590834dc45d1247295302c212fda9d`  
		Last Modified: Wed, 16 Aug 2023 04:34:45 GMT  
		Size: 24.6 MB (24627247 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:rolling` - linux; arm64 variant v8

```console
$ docker pull ubuntu@sha256:d68d8bcae123a839bc72b91fa9df55956be3fcb2dbfc247acb7f65908eaa6c35
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.1 MB (26064545 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e1c8e9335de75964dd320b20b4290408432be2962faf7ad36d3a47d48f3131cd`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 16 Aug 2023 04:15:57 GMT
ARG RELEASE
# Wed, 16 Aug 2023 04:15:57 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 16 Aug 2023 04:15:57 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 16 Aug 2023 04:15:57 GMT
LABEL org.opencontainers.image.version=23.04
# Wed, 16 Aug 2023 04:16:01 GMT
ADD file:adea2962926b29b76eb8da76ae9e830c5ad7050ae9b19f5427191b338c8a2c56 in / 
# Wed, 16 Aug 2023 04:16:02 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:2b2d15932a31f0857b9499cc218b8777708cb1d73ae6ef680f624ca7d4342763`  
		Last Modified: Wed, 16 Aug 2023 04:34:39 GMT  
		Size: 26.1 MB (26064545 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:rolling` - linux; ppc64le

```console
$ docker pull ubuntu@sha256:1306e75f505a2305f2c46f51f33be8b8599923bd5a652c3b5dc37333db4f44ab
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.9 MB (30905042 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:91733a8763fe80d6e620ec400c2721ee45c0f80398506088d1278d6531299a90`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 16 Aug 2023 04:16:31 GMT
ARG RELEASE
# Wed, 16 Aug 2023 04:16:31 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 16 Aug 2023 04:16:31 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 16 Aug 2023 04:16:31 GMT
LABEL org.opencontainers.image.version=23.04
# Wed, 16 Aug 2023 04:16:34 GMT
ADD file:a9d35b320d969ee1ae8a7bc83aba49da30d93724befb5948c680066ad4f1acdf in / 
# Wed, 16 Aug 2023 04:16:35 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:f51cbff870f31d4c4397c2f21529046998f8d6e7748fd6f059b325a0759c7dd4`  
		Last Modified: Wed, 16 Aug 2023 04:34:51 GMT  
		Size: 30.9 MB (30905042 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:rolling` - linux; s390x

```console
$ docker pull ubuntu@sha256:ec9620bbf89d1a3b1171f961340a890166607be3423d96e740f6d56f36ccb125
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.7 MB (25691524 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1289eb3132a14bc161676d7f928d557bf63eb8561718e9d5247e16e88ebee8ff`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 16 Aug 2023 04:29:27 GMT
ARG RELEASE
# Wed, 16 Aug 2023 04:29:28 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 16 Aug 2023 04:29:28 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 16 Aug 2023 04:29:28 GMT
LABEL org.opencontainers.image.version=23.04
# Wed, 16 Aug 2023 04:29:29 GMT
ADD file:14fcf0756fb29b609af54412c31e2ff9acbf4634984ce95bf204c67668706cb5 in / 
# Wed, 16 Aug 2023 04:29:30 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:b1e434384d3d3b546e155df0cf143c8c0a92bf766c6808bf2e3e1d2f22010839`  
		Last Modified: Wed, 16 Aug 2023 04:34:57 GMT  
		Size: 25.7 MB (25691524 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
