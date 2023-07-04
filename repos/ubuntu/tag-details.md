<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `ubuntu`

-	[`ubuntu:20.04`](#ubuntu2004)
-	[`ubuntu:22.04`](#ubuntu2204)
-	[`ubuntu:22.10`](#ubuntu2210)
-	[`ubuntu:23.04`](#ubuntu2304)
-	[`ubuntu:23.10`](#ubuntu2310)
-	[`ubuntu:devel`](#ubuntudevel)
-	[`ubuntu:focal`](#ubuntufocal)
-	[`ubuntu:focal-20230624`](#ubuntufocal-20230624)
-	[`ubuntu:jammy`](#ubuntujammy)
-	[`ubuntu:jammy-20230624`](#ubuntujammy-20230624)
-	[`ubuntu:kinetic`](#ubuntukinetic)
-	[`ubuntu:kinetic-20230624`](#ubuntukinetic-20230624)
-	[`ubuntu:latest`](#ubuntulatest)
-	[`ubuntu:lunar`](#ubuntulunar)
-	[`ubuntu:lunar-20230615`](#ubuntulunar-20230615)
-	[`ubuntu:mantic`](#ubuntumantic)
-	[`ubuntu:mantic-20230624`](#ubuntumantic-20230624)
-	[`ubuntu:rolling`](#ubunturolling)

## `ubuntu:20.04`

```console
$ docker pull ubuntu@sha256:f8f658407c35733471596f25fdb4ed748b80e545ab57e84efbdb1dbbb01bd70e
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
$ docker pull ubuntu@sha256:554e40b15453c788ec799badf0f1ad05c3e5c735b53f940feb8f27cf2ec570c5
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.5 MB (27506421 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:626a42b93d93241a6a48d81d921934891f73185547833a64dde06599cf3eafc2`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 05 Jun 2023 17:08:57 GMT
ARG RELEASE
# Mon, 05 Jun 2023 17:08:57 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 05 Jun 2023 17:08:57 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 05 Jun 2023 17:08:57 GMT
LABEL org.opencontainers.image.version=20.04
# Mon, 05 Jun 2023 17:08:58 GMT
ADD file:655d373cb551d0dd5d7867f88a4f98908dc3f16190986f693e88c423e6f21b8d in / 
# Mon, 05 Jun 2023 17:08:58 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:56e0351b98767487b3c411034be95479ed1710bb6be860db6df0be3a98653027`  
		Last Modified: Mon, 05 Jun 2023 17:26:33 GMT  
		Size: 27.5 MB (27506421 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:20.04` - linux; arm variant v7

```console
$ docker pull ubuntu@sha256:3831296f7467818605f4c8782b1a74a3488547102640e9cb8b41c42b44e7f526
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.6 MB (23611936 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3ef263d65a04f7a877f4868d790eef952ec3a69e4143477edc9f3cc80c4f9c43`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 05 Jun 2023 17:19:26 GMT
ARG RELEASE
# Mon, 05 Jun 2023 17:19:26 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 05 Jun 2023 17:19:26 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 05 Jun 2023 17:19:27 GMT
LABEL org.opencontainers.image.version=20.04
# Mon, 05 Jun 2023 17:19:31 GMT
ADD file:114d6f55f8c1c4ec7f7d2ba3c803116a188eece1d1b6dbb3bb40c11082194234 in / 
# Mon, 05 Jun 2023 17:19:31 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:4f6069ed163b7975b49dc9e8925a15a02473293dca6513363fb11c08764520b8`  
		Last Modified: Mon, 05 Jun 2023 17:26:46 GMT  
		Size: 23.6 MB (23611936 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:20.04` - linux; arm64 variant v8

```console
$ docker pull ubuntu@sha256:ebdb7ac21fef61242b87d8d00ca0d3f4434c5adf360e771dc1b8db0f75771759
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.0 MB (25974252 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a494d051d6a9c0e46123cfc516acb84b76884f21684764c166ecf4fe92a7fa4d`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 05 Jun 2023 17:07:59 GMT
ARG RELEASE
# Mon, 05 Jun 2023 17:07:59 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 05 Jun 2023 17:07:59 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 05 Jun 2023 17:07:59 GMT
LABEL org.opencontainers.image.version=20.04
# Mon, 05 Jun 2023 17:08:02 GMT
ADD file:6c0661b94e27ede70ca2a8842bdab5bc26b9ae4760b17870eda9d595672795ff in / 
# Mon, 05 Jun 2023 17:08:02 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:fb0a6f6b1798ce3ee565023c3a50777fff89bf6761a0985c8ff93aa903f7d0f1`  
		Last Modified: Mon, 05 Jun 2023 17:26:40 GMT  
		Size: 26.0 MB (25974252 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:20.04` - linux; ppc64le

```console
$ docker pull ubuntu@sha256:1b176384bc513bb425b497364f1d6353ac1b285d48862c22a9b7c450c431d4bf
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.1 MB (32070916 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c0cad30b7d8589358e8074d6fb495d774d8c52cfa8ab35ed10f518a2c8b7586c`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 05 Jun 2023 17:08:24 GMT
ARG RELEASE
# Mon, 05 Jun 2023 17:08:24 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 05 Jun 2023 17:08:24 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 05 Jun 2023 17:08:25 GMT
LABEL org.opencontainers.image.version=20.04
# Mon, 05 Jun 2023 17:08:28 GMT
ADD file:0a2372ac4d43f0f4ada2b55dd0a359df73a828a9aa9426bfdd05a02b9c4b2bd9 in / 
# Mon, 05 Jun 2023 17:08:28 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:a42700f678f7c62f7053fbbd2b046ac1742685ac4262717c9c6db8a8e872884d`  
		Last Modified: Mon, 05 Jun 2023 17:26:52 GMT  
		Size: 32.1 MB (32070916 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:20.04` - linux; s390x

```console
$ docker pull ubuntu@sha256:90dca1700c58ce633d6d7566ddcab50d8211e07a39d975197c43ddccc7ca84d1
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.4 MB (26351327 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:54f1d743745c70710688433dda5ce774740bacdbb8f6d824ac1a6150da5a72fe`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 05 Jun 2023 17:07:58 GMT
ARG RELEASE
# Mon, 05 Jun 2023 17:07:58 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 05 Jun 2023 17:07:58 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 05 Jun 2023 17:07:58 GMT
LABEL org.opencontainers.image.version=20.04
# Mon, 05 Jun 2023 17:08:00 GMT
ADD file:3aeae4efd27981f5d9d2894756f698b4fab4fbc6de4258ebd03baad8bf626d5c in / 
# Mon, 05 Jun 2023 17:08:00 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:83be4b9c36a879f795854cd45dc3e4f79cef2d7685ab6f26770b8a9e5c8baadd`  
		Last Modified: Mon, 05 Jun 2023 17:26:58 GMT  
		Size: 26.4 MB (26351327 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

## `ubuntu:22.04`

```console
$ docker pull ubuntu@sha256:6120be6a2b7ce665d0cbddc3ce6eae60fe94637c6a66985312d1f02f63cc0bcd
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
$ docker pull ubuntu@sha256:83f0c2a8d6f266d687d55b5cb1cb2201148eb7ac449e4202d9646b9083f1cee0
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.5 MB (29533050 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:99284ca6cea039c7784d1414608c6e846dd56830c2a13e1341be681c3ffcc8ac`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 05 Jun 2023 17:00:37 GMT
ARG RELEASE
# Mon, 05 Jun 2023 17:00:37 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 05 Jun 2023 17:00:37 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 05 Jun 2023 17:00:37 GMT
LABEL org.opencontainers.image.version=22.04
# Mon, 05 Jun 2023 17:00:39 GMT
ADD file:0ad2ee2cfb186802f49c9bf4148674d1c6fc201f83478ec01ffaa7086d491323 in / 
# Mon, 05 Jun 2023 17:00:39 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:6b851dcae6ca1461dde247915abc5048061f34332929ca8fb37d9dc18f2e2f44`  
		Last Modified: Mon, 05 Jun 2023 17:20:26 GMT  
		Size: 29.5 MB (29533050 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:22.04` - linux; arm variant v7

```console
$ docker pull ubuntu@sha256:9aa2ce874cc0d140b3344fb6125d0ef540d347bca8a13c2270ca1c7a40490be3
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.1 MB (26140710 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3681d7421d4545f9eb7b1aabcb24b041b347b37705f89a858f831b94d8e2f0bf`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 05 Jun 2023 16:59:35 GMT
ARG RELEASE
# Mon, 05 Jun 2023 16:59:35 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 05 Jun 2023 16:59:35 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 05 Jun 2023 16:59:35 GMT
LABEL org.opencontainers.image.version=22.04
# Mon, 05 Jun 2023 16:59:40 GMT
ADD file:5425962ced738173a50965fc5cd95c79d0a319323df4a34e9da3f5037a5264c3 in / 
# Mon, 05 Jun 2023 16:59:40 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:4ceecae09ee56d3fb7d5d26ff9505f3aa7e7cc5e54545fbecde69ef046b84f1c`  
		Last Modified: Mon, 05 Jun 2023 17:20:38 GMT  
		Size: 26.1 MB (26140710 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:22.04` - linux; arm64 variant v8

```console
$ docker pull ubuntu@sha256:25de8a960c338b7d38aa15c012ceee70d8e29239db97596d6ecc50a5085d8f7a
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.3 MB (27346742 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cfb01e8e31210c9bfc5412c3fc1b8b7aea849bc2a9c21f47553bd31cc8fd79f9`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 05 Jun 2023 17:11:17 GMT
ARG RELEASE
# Mon, 05 Jun 2023 17:11:17 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 05 Jun 2023 17:11:17 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 05 Jun 2023 17:11:17 GMT
LABEL org.opencontainers.image.version=22.04
# Mon, 05 Jun 2023 17:11:19 GMT
ADD file:1043594b482384e967c94378b65ec4bc7a38190649a94f0325b7fb00be0a623e in / 
# Mon, 05 Jun 2023 17:11:19 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:b2837baf7808226f588fabacb30598287e02d4dbf120eaf968c5299a6c2e9619`  
		Last Modified: Mon, 05 Jun 2023 17:20:32 GMT  
		Size: 27.3 MB (27346742 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:22.04` - linux; ppc64le

```console
$ docker pull ubuntu@sha256:eb4e647121c71cc9305e466d9c844a1207f90bab2e689310050e66e8b4f4d534
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.6 MB (34591237 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:16fc5784936f704a4bd8208deeb624554aeb2cdab87301aab60391db8f7ec590`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 05 Jun 2023 17:01:00 GMT
ARG RELEASE
# Mon, 05 Jun 2023 17:01:00 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 05 Jun 2023 17:01:00 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 05 Jun 2023 17:01:01 GMT
LABEL org.opencontainers.image.version=22.04
# Mon, 05 Jun 2023 17:01:03 GMT
ADD file:00c4f44b35b683caef54d5b8b0e0b1e68872f45eae17dd7543adaf6c54512447 in / 
# Mon, 05 Jun 2023 17:01:04 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:d3c256ab34973cfc9065065e684e5e5d1dac1eeb77974324e0de68944af26f62`  
		Last Modified: Mon, 05 Jun 2023 17:20:44 GMT  
		Size: 34.6 MB (34591237 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:22.04` - linux; s390x

```console
$ docker pull ubuntu@sha256:0b8eed006f12768a3a15fdf891f77d9a5fbf805882f15a8180c428f47d9d297e
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.0 MB (28015524 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8c7ef32086a3a754c9d2e6f68f731d3cd053c01ec070ae20c059995a33ac4afc`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 05 Jun 2023 17:01:02 GMT
ARG RELEASE
# Mon, 05 Jun 2023 17:01:02 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 05 Jun 2023 17:01:02 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 05 Jun 2023 17:01:02 GMT
LABEL org.opencontainers.image.version=22.04
# Mon, 05 Jun 2023 17:01:04 GMT
ADD file:2d2f31ec110b9e7ec21a9d4824a430acdaabf0b4e9c1cdd337438992859b57ae in / 
# Mon, 05 Jun 2023 17:01:04 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:02f8248e8d232d4898b07be78857694fe6651b4faa795e63952783f0aa44f1fe`  
		Last Modified: Mon, 05 Jun 2023 17:20:50 GMT  
		Size: 28.0 MB (28015524 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

## `ubuntu:22.10`

```console
$ docker pull ubuntu@sha256:1fa7586c0f10cc7ce7ca379ae48bf06776325b9f8e97963ce40803a8bcc07dca
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
$ docker pull ubuntu@sha256:80fb4ea0c0a384a3072a6be1879c342bb636b0d105209535ba893ba75ab38ede
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.7 MB (26704595 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e39f297e9dda29a8d8896051c30f32feb52c9dcfb68e8a561650a1dde97cc94b`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 05 Jun 2023 17:02:32 GMT
ARG RELEASE
# Mon, 05 Jun 2023 17:02:32 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 05 Jun 2023 17:02:32 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 05 Jun 2023 17:02:32 GMT
LABEL org.opencontainers.image.version=22.10
# Mon, 05 Jun 2023 17:02:34 GMT
ADD file:f8bb312bf73c62343d91c9988d58945c5d0fced3f559b95c4dd21a19183d933d in / 
# Mon, 05 Jun 2023 17:02:34 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:317e06b63fc01feacb4fa7a967d3a8c6fd35296935c83caa85ad28cd20add12b`  
		Last Modified: Mon, 05 Jun 2023 17:21:29 GMT  
		Size: 26.7 MB (26704595 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:22.10` - linux; arm variant v7

```console
$ docker pull ubuntu@sha256:5dc1502337b177771dd9904822cde9abd2b26ee4014a3c6df7e912a9ef103db3
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.1 MB (25098670 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1120758c0ceafe38a213551ecf496a3b05011b323c13e36840d566b2ee02416d`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 05 Jun 2023 17:04:06 GMT
ARG RELEASE
# Mon, 05 Jun 2023 17:04:06 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 05 Jun 2023 17:04:06 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 05 Jun 2023 17:04:07 GMT
LABEL org.opencontainers.image.version=22.10
# Mon, 05 Jun 2023 17:04:15 GMT
ADD file:615be72e62c21704af356d6cfd4e32a7df8dd4b93d0c3ee3ea2e1641127c54ea in / 
# Mon, 05 Jun 2023 17:04:16 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:7eb2ece7978deb374e0aa4623aa1a44d513c34c7a56e23251a0dfbba314ea260`  
		Last Modified: Mon, 05 Jun 2023 17:21:41 GMT  
		Size: 25.1 MB (25098670 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:22.10` - linux; arm64 variant v8

```console
$ docker pull ubuntu@sha256:dde2a31e58d07b2ed8be842eafae55b9a46b3629a0915dd6438fb3e484e46d65
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.8 MB (25770482 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:172adc9ce1cab441186106c04f9663f7b81edc9d3e8908b8dca58180df27ea16`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 05 Jun 2023 17:02:45 GMT
ARG RELEASE
# Mon, 05 Jun 2023 17:02:45 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 05 Jun 2023 17:02:45 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 05 Jun 2023 17:02:46 GMT
LABEL org.opencontainers.image.version=22.10
# Mon, 05 Jun 2023 17:02:50 GMT
ADD file:b85182b4593c262faef116755e01baa608e8090e1cb697d735485ff0bd5b353e in / 
# Mon, 05 Jun 2023 17:02:50 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:bb573a4d6d791b5d50f1118d01e4c9b2acc927522cec8740ac9957e37eeac29c`  
		Last Modified: Mon, 05 Jun 2023 17:21:35 GMT  
		Size: 25.8 MB (25770482 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:22.10` - linux; ppc64le

```console
$ docker pull ubuntu@sha256:b2a4b994153a43ab4941ab8efbc43c189d0c76b9fe4f8dee9f8449cd6ed83d93
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.1 MB (31112867 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c8a632c9634c258b38d044be3dfa48ee0aee70c82531def42c6e701c10e15989`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 05 Jun 2023 17:10:48 GMT
ARG RELEASE
# Mon, 05 Jun 2023 17:10:48 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 05 Jun 2023 17:10:48 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 05 Jun 2023 17:10:48 GMT
LABEL org.opencontainers.image.version=22.10
# Mon, 05 Jun 2023 17:10:52 GMT
ADD file:48c30fe281554302bb6533dd33a43a0877851ac5ba59dc3aff3d3d9ceae6f8a9 in / 
# Mon, 05 Jun 2023 17:10:52 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:e4485626c4310d83f6d257d7c30db7a4fc23c70b98dec3ca37108fef26207e3c`  
		Last Modified: Mon, 05 Jun 2023 17:21:47 GMT  
		Size: 31.1 MB (31112867 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:22.10` - linux; s390x

```console
$ docker pull ubuntu@sha256:1776cac9e796ccbe3048e682a977054303fc511313d8d7d43b805eec3d4669fa
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.5 MB (25489752 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d8c554a011867c58cc8ab63be78f10271da1d2a76c4498de2a5b33b7ecb26486`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 05 Jun 2023 17:10:49 GMT
ARG RELEASE
# Mon, 05 Jun 2023 17:10:49 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 05 Jun 2023 17:10:49 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 05 Jun 2023 17:10:49 GMT
LABEL org.opencontainers.image.version=22.10
# Mon, 05 Jun 2023 17:10:51 GMT
ADD file:2390e4c5ac4f862cf5fb266c70962a01f271fa692b74af886f18911482025825 in / 
# Mon, 05 Jun 2023 17:10:51 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:245e6239c00ff9b6decc18e3b64f2390bc669d50050fdfd65a8b91e45183fbe3`  
		Last Modified: Mon, 05 Jun 2023 17:21:53 GMT  
		Size: 25.5 MB (25489752 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

## `ubuntu:23.04`

```console
$ docker pull ubuntu@sha256:b5d5cddaeb8d2f150660cf8f9a1203dd450ac765e6c07630176ac6486eceaddb
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
$ docker pull ubuntu@sha256:09f035f46361d193ded647342903b413d57d05cc06acff8285f9dda9f2d269d5
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.8 MB (26836883 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1ed313b0551f6255bb9ea7fd953363f0f306d9e2e92dc9fb94cbdf70e3dafb6f`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 15 Jun 2023 08:28:38 GMT
ARG RELEASE
# Thu, 15 Jun 2023 08:28:38 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 15 Jun 2023 08:28:38 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 15 Jun 2023 08:28:38 GMT
LABEL org.opencontainers.image.version=23.04
# Thu, 15 Jun 2023 08:28:39 GMT
ADD file:708314051e878a0c6071fb2c8d4458a04ce058f47f2cfaa58c1b5a42e837ca0f in / 
# Thu, 15 Jun 2023 08:28:40 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:3a9d46cc3977f1066a9dd08f845b76f7f7d46e4ef74fdf8ed1f4db514ea5a45d`  
		Last Modified: Thu, 15 Jun 2023 09:08:28 GMT  
		Size: 26.8 MB (26836883 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:23.04` - linux; arm variant v7

```console
$ docker pull ubuntu@sha256:98e3a45616c77d754ce50a12634c507cecf9b53ccb2f48e94b20db7b4b698618
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **24.6 MB (24636364 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:678dff67c6b9c6ec4eaccccccd2ffae1ddbf85b5e5309ac56522d7442f3f8c2d`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 15 Jun 2023 08:10:50 GMT
ARG RELEASE
# Thu, 15 Jun 2023 08:10:50 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 15 Jun 2023 08:10:51 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 15 Jun 2023 08:10:51 GMT
LABEL org.opencontainers.image.version=23.04
# Thu, 15 Jun 2023 08:10:53 GMT
ADD file:8484efc06b5f22d170eef374f45df452d8e36f4cbef702f7ee4d1f130dd28093 in / 
# Thu, 15 Jun 2023 08:10:53 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:fb49e82a48f62b12a885a1a02ae80f5261ab51e3f138c0190fc8d119247fd11c`  
		Last Modified: Thu, 15 Jun 2023 09:08:40 GMT  
		Size: 24.6 MB (24636364 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:23.04` - linux; arm64 variant v8

```console
$ docker pull ubuntu@sha256:2ea9408d05cc2543752070f336452eda81593c2001f9931a0451bad3a45d3a31
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.1 MB (26088803 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f6b331a8a5e1bb537caa9a8e3d3f6308563136db02ab0501499e819e36d9f48a`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 15 Jun 2023 08:33:24 GMT
ARG RELEASE
# Thu, 15 Jun 2023 08:33:25 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 15 Jun 2023 08:33:25 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 15 Jun 2023 08:33:25 GMT
LABEL org.opencontainers.image.version=23.04
# Thu, 15 Jun 2023 08:33:58 GMT
ADD file:064ac1f238394a53372e0db107e28835aa3c39ed189a15fe85c532bbb50bfbaf in / 
# Thu, 15 Jun 2023 08:33:59 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:19e8382a46db1cf2ede3739a9337cad793e2228c0e455f8969bbbc14b4d6f28e`  
		Last Modified: Thu, 15 Jun 2023 09:08:34 GMT  
		Size: 26.1 MB (26088803 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:23.04` - linux; ppc64le

```console
$ docker pull ubuntu@sha256:cac0b3657eb2260df362c4949ec416d6377b36d5c2999e1765874dcbadeca4cd
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.0 MB (31029474 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:da0d4e75ccb4b903cf3c7d3515fdbbe2462a8043abbcf13667b6f860fc11302e`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 15 Jun 2023 08:29:14 GMT
ARG RELEASE
# Thu, 15 Jun 2023 08:29:14 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 15 Jun 2023 08:29:15 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 15 Jun 2023 08:29:15 GMT
LABEL org.opencontainers.image.version=23.04
# Thu, 15 Jun 2023 08:29:17 GMT
ADD file:5ebdf4bd4bc2b27019f20fb1964a395fa504d4f20e208c54237e363895b492d7 in / 
# Thu, 15 Jun 2023 08:29:18 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:223122c533fb03fa9f10684bc8fb23adf1f08af994530d4c9403f9086da8952b`  
		Last Modified: Thu, 15 Jun 2023 09:08:47 GMT  
		Size: 31.0 MB (31029474 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:23.04` - linux; s390x

```console
$ docker pull ubuntu@sha256:6b7f8b6a5280fe23d857ac4cd887805f2a7d014d3d88dccedd81379291a54a34
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.7 MB (25716588 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:08ed40f2186d81239c9993cac2d5749fcad7ee65da4786f87d8e3d0caea927e1`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 15 Jun 2023 08:11:16 GMT
ARG RELEASE
# Thu, 15 Jun 2023 08:11:16 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 15 Jun 2023 08:11:16 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 15 Jun 2023 08:11:16 GMT
LABEL org.opencontainers.image.version=23.04
# Thu, 15 Jun 2023 08:11:18 GMT
ADD file:3974fe053080180d99954042c25b3bd0c82e320fb4521b197cbc45f21885fc43 in / 
# Thu, 15 Jun 2023 08:11:18 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:1611e8f17f580c929b21787327a1e5133fd1c1954ec9b270101aee4380735e40`  
		Last Modified: Thu, 15 Jun 2023 09:08:53 GMT  
		Size: 25.7 MB (25716588 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

## `ubuntu:23.10`

```console
$ docker pull ubuntu@sha256:bd1e0eb3171a6e499c84211e73c4f5f5b2a585507256f772f5c4f4420a3d8591
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
$ docker pull ubuntu@sha256:07460e809a7141b84050c6d68220c1f7e2aa58b0bc124c40a1440988bfd87e6b
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.9 MB (26931867 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ce0fd6ed554b4fa85755cd2f9fefc45a1bff5e640b1090f4573997837f6c46b2`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 07 Jun 2023 04:39:09 GMT
ARG RELEASE
# Wed, 07 Jun 2023 04:39:09 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 07 Jun 2023 04:39:09 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 07 Jun 2023 04:39:09 GMT
LABEL org.opencontainers.image.version=23.10
# Wed, 07 Jun 2023 04:39:10 GMT
ADD file:d8dc8c4236b9885e64ccd27399ed8dddab7d39915d76378527cb730855aba0e1 in / 
# Wed, 07 Jun 2023 04:39:10 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:a3cc0ea50b9aef0e9b8b228c37edf92b0dfcb177d34ed50433918ae5eec172be`  
		Last Modified: Wed, 07 Jun 2023 04:57:40 GMT  
		Size: 26.9 MB (26931867 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:23.10` - linux; arm variant v7

```console
$ docker pull ubuntu@sha256:bf18ca0b049d010b72c35574c0261ef9c231fffb7588709e05a6b807c081e552
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **24.5 MB (24478190 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4eabbb20f267b27e88fe450b3d209313994eeb87c19d8cbdec2b2f8e821a1ce5`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 07 Jun 2023 04:48:07 GMT
ARG RELEASE
# Wed, 07 Jun 2023 04:48:07 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 07 Jun 2023 04:48:08 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 07 Jun 2023 04:48:08 GMT
LABEL org.opencontainers.image.version=23.10
# Wed, 07 Jun 2023 04:48:12 GMT
ADD file:65e05498800189bf1f48f5c6df21d144e18e5e069db55d0b88d45c04cc1fe4de in / 
# Wed, 07 Jun 2023 04:48:12 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:df4275b0f8f556aa5462a1fad0a0a188bc3d7b287bc6120389314f6b9bd6566e`  
		Last Modified: Wed, 07 Jun 2023 04:57:51 GMT  
		Size: 24.5 MB (24478190 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:23.10` - linux; arm64 variant v8

```console
$ docker pull ubuntu@sha256:d9c68082dd554f1adf3ed6169d08f0aae5431b4a7bddb8c19951eae6bd607097
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.1 MB (26131158 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0a27f5fa4b6e23e37d77cb2410d8f9efb5a9f5698e10bf3aef9bb503b14497d3`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 07 Jun 2023 04:42:14 GMT
ARG RELEASE
# Wed, 07 Jun 2023 04:42:14 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 07 Jun 2023 04:42:14 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 07 Jun 2023 04:42:14 GMT
LABEL org.opencontainers.image.version=23.10
# Wed, 07 Jun 2023 04:42:16 GMT
ADD file:3f4faed988a03b7d05aefe677906592aade4d2bae1ec3f7055c1f10744a38de0 in / 
# Wed, 07 Jun 2023 04:42:16 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:f698dd1f118f52521a462f35505a0bca0dc8a7e17802e11146a6c0acfbfc797d`  
		Last Modified: Wed, 07 Jun 2023 04:57:46 GMT  
		Size: 26.1 MB (26131158 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:23.10` - linux; ppc64le

```console
$ docker pull ubuntu@sha256:8d9660ab5ab6a35050e6f5ac4ff4170e85c1e6776e83d075f9331b85215b96a4
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.0 MB (30966286 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7a4004a6116d82330c1bb10006b89dcfb699827cd79a405a16dd59e3e33889d4`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 07 Jun 2023 04:48:25 GMT
ARG RELEASE
# Wed, 07 Jun 2023 04:48:26 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 07 Jun 2023 04:48:26 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 07 Jun 2023 04:48:26 GMT
LABEL org.opencontainers.image.version=23.10
# Wed, 07 Jun 2023 04:48:28 GMT
ADD file:6cf1bffac55b7de64803fabdb35baf75349cc0a40c0b4c68ac2690b7123edc85 in / 
# Wed, 07 Jun 2023 04:48:29 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:537eb27ff37d9fd24f7097996a5a0ed640152c3656390c06baff05ecd549d691`  
		Last Modified: Wed, 07 Jun 2023 04:57:57 GMT  
		Size: 31.0 MB (30966286 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:23.10` - linux; s390x

```console
$ docker pull ubuntu@sha256:441bef6aaac131b562992783cb31ac363fb5fa5592c928be1fc6ec01b45fb0e8
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.8 MB (25750156 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:deb4b1b351b9ab4eff7e955188cbe7a5b818325f441be917beee6a25cbf66783`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 07 Jun 2023 04:42:36 GMT
ARG RELEASE
# Wed, 07 Jun 2023 04:42:36 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 07 Jun 2023 04:42:36 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 07 Jun 2023 04:42:36 GMT
LABEL org.opencontainers.image.version=23.10
# Wed, 07 Jun 2023 04:42:38 GMT
ADD file:4e8ca8820de4a27d67ad223be645ce7a7a48289dfcbc01b4e1dbe3bc74ebbc56 in / 
# Wed, 07 Jun 2023 04:42:38 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:906d24b8296f0e80ba93ccd8c8a85183d978d41115e21f9aba3044ad0d38b45e`  
		Last Modified: Wed, 07 Jun 2023 04:58:03 GMT  
		Size: 25.8 MB (25750156 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

## `ubuntu:devel`

```console
$ docker pull ubuntu@sha256:bd1e0eb3171a6e499c84211e73c4f5f5b2a585507256f772f5c4f4420a3d8591
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
$ docker pull ubuntu@sha256:07460e809a7141b84050c6d68220c1f7e2aa58b0bc124c40a1440988bfd87e6b
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.9 MB (26931867 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ce0fd6ed554b4fa85755cd2f9fefc45a1bff5e640b1090f4573997837f6c46b2`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 07 Jun 2023 04:39:09 GMT
ARG RELEASE
# Wed, 07 Jun 2023 04:39:09 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 07 Jun 2023 04:39:09 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 07 Jun 2023 04:39:09 GMT
LABEL org.opencontainers.image.version=23.10
# Wed, 07 Jun 2023 04:39:10 GMT
ADD file:d8dc8c4236b9885e64ccd27399ed8dddab7d39915d76378527cb730855aba0e1 in / 
# Wed, 07 Jun 2023 04:39:10 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:a3cc0ea50b9aef0e9b8b228c37edf92b0dfcb177d34ed50433918ae5eec172be`  
		Last Modified: Wed, 07 Jun 2023 04:57:40 GMT  
		Size: 26.9 MB (26931867 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:devel` - linux; arm variant v7

```console
$ docker pull ubuntu@sha256:bf18ca0b049d010b72c35574c0261ef9c231fffb7588709e05a6b807c081e552
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **24.5 MB (24478190 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4eabbb20f267b27e88fe450b3d209313994eeb87c19d8cbdec2b2f8e821a1ce5`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 07 Jun 2023 04:48:07 GMT
ARG RELEASE
# Wed, 07 Jun 2023 04:48:07 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 07 Jun 2023 04:48:08 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 07 Jun 2023 04:48:08 GMT
LABEL org.opencontainers.image.version=23.10
# Wed, 07 Jun 2023 04:48:12 GMT
ADD file:65e05498800189bf1f48f5c6df21d144e18e5e069db55d0b88d45c04cc1fe4de in / 
# Wed, 07 Jun 2023 04:48:12 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:df4275b0f8f556aa5462a1fad0a0a188bc3d7b287bc6120389314f6b9bd6566e`  
		Last Modified: Wed, 07 Jun 2023 04:57:51 GMT  
		Size: 24.5 MB (24478190 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:devel` - linux; arm64 variant v8

```console
$ docker pull ubuntu@sha256:d9c68082dd554f1adf3ed6169d08f0aae5431b4a7bddb8c19951eae6bd607097
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.1 MB (26131158 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0a27f5fa4b6e23e37d77cb2410d8f9efb5a9f5698e10bf3aef9bb503b14497d3`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 07 Jun 2023 04:42:14 GMT
ARG RELEASE
# Wed, 07 Jun 2023 04:42:14 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 07 Jun 2023 04:42:14 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 07 Jun 2023 04:42:14 GMT
LABEL org.opencontainers.image.version=23.10
# Wed, 07 Jun 2023 04:42:16 GMT
ADD file:3f4faed988a03b7d05aefe677906592aade4d2bae1ec3f7055c1f10744a38de0 in / 
# Wed, 07 Jun 2023 04:42:16 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:f698dd1f118f52521a462f35505a0bca0dc8a7e17802e11146a6c0acfbfc797d`  
		Last Modified: Wed, 07 Jun 2023 04:57:46 GMT  
		Size: 26.1 MB (26131158 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:devel` - linux; ppc64le

```console
$ docker pull ubuntu@sha256:8d9660ab5ab6a35050e6f5ac4ff4170e85c1e6776e83d075f9331b85215b96a4
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.0 MB (30966286 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7a4004a6116d82330c1bb10006b89dcfb699827cd79a405a16dd59e3e33889d4`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 07 Jun 2023 04:48:25 GMT
ARG RELEASE
# Wed, 07 Jun 2023 04:48:26 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 07 Jun 2023 04:48:26 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 07 Jun 2023 04:48:26 GMT
LABEL org.opencontainers.image.version=23.10
# Wed, 07 Jun 2023 04:48:28 GMT
ADD file:6cf1bffac55b7de64803fabdb35baf75349cc0a40c0b4c68ac2690b7123edc85 in / 
# Wed, 07 Jun 2023 04:48:29 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:537eb27ff37d9fd24f7097996a5a0ed640152c3656390c06baff05ecd549d691`  
		Last Modified: Wed, 07 Jun 2023 04:57:57 GMT  
		Size: 31.0 MB (30966286 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:devel` - linux; s390x

```console
$ docker pull ubuntu@sha256:441bef6aaac131b562992783cb31ac363fb5fa5592c928be1fc6ec01b45fb0e8
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.8 MB (25750156 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:deb4b1b351b9ab4eff7e955188cbe7a5b818325f441be917beee6a25cbf66783`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 07 Jun 2023 04:42:36 GMT
ARG RELEASE
# Wed, 07 Jun 2023 04:42:36 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 07 Jun 2023 04:42:36 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 07 Jun 2023 04:42:36 GMT
LABEL org.opencontainers.image.version=23.10
# Wed, 07 Jun 2023 04:42:38 GMT
ADD file:4e8ca8820de4a27d67ad223be645ce7a7a48289dfcbc01b4e1dbe3bc74ebbc56 in / 
# Wed, 07 Jun 2023 04:42:38 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:906d24b8296f0e80ba93ccd8c8a85183d978d41115e21f9aba3044ad0d38b45e`  
		Last Modified: Wed, 07 Jun 2023 04:58:03 GMT  
		Size: 25.8 MB (25750156 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

## `ubuntu:focal`

```console
$ docker pull ubuntu@sha256:f8f658407c35733471596f25fdb4ed748b80e545ab57e84efbdb1dbbb01bd70e
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
$ docker pull ubuntu@sha256:554e40b15453c788ec799badf0f1ad05c3e5c735b53f940feb8f27cf2ec570c5
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.5 MB (27506421 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:626a42b93d93241a6a48d81d921934891f73185547833a64dde06599cf3eafc2`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 05 Jun 2023 17:08:57 GMT
ARG RELEASE
# Mon, 05 Jun 2023 17:08:57 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 05 Jun 2023 17:08:57 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 05 Jun 2023 17:08:57 GMT
LABEL org.opencontainers.image.version=20.04
# Mon, 05 Jun 2023 17:08:58 GMT
ADD file:655d373cb551d0dd5d7867f88a4f98908dc3f16190986f693e88c423e6f21b8d in / 
# Mon, 05 Jun 2023 17:08:58 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:56e0351b98767487b3c411034be95479ed1710bb6be860db6df0be3a98653027`  
		Last Modified: Mon, 05 Jun 2023 17:26:33 GMT  
		Size: 27.5 MB (27506421 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:focal` - linux; arm variant v7

```console
$ docker pull ubuntu@sha256:3831296f7467818605f4c8782b1a74a3488547102640e9cb8b41c42b44e7f526
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.6 MB (23611936 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3ef263d65a04f7a877f4868d790eef952ec3a69e4143477edc9f3cc80c4f9c43`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 05 Jun 2023 17:19:26 GMT
ARG RELEASE
# Mon, 05 Jun 2023 17:19:26 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 05 Jun 2023 17:19:26 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 05 Jun 2023 17:19:27 GMT
LABEL org.opencontainers.image.version=20.04
# Mon, 05 Jun 2023 17:19:31 GMT
ADD file:114d6f55f8c1c4ec7f7d2ba3c803116a188eece1d1b6dbb3bb40c11082194234 in / 
# Mon, 05 Jun 2023 17:19:31 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:4f6069ed163b7975b49dc9e8925a15a02473293dca6513363fb11c08764520b8`  
		Last Modified: Mon, 05 Jun 2023 17:26:46 GMT  
		Size: 23.6 MB (23611936 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:focal` - linux; arm64 variant v8

```console
$ docker pull ubuntu@sha256:ebdb7ac21fef61242b87d8d00ca0d3f4434c5adf360e771dc1b8db0f75771759
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.0 MB (25974252 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a494d051d6a9c0e46123cfc516acb84b76884f21684764c166ecf4fe92a7fa4d`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 05 Jun 2023 17:07:59 GMT
ARG RELEASE
# Mon, 05 Jun 2023 17:07:59 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 05 Jun 2023 17:07:59 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 05 Jun 2023 17:07:59 GMT
LABEL org.opencontainers.image.version=20.04
# Mon, 05 Jun 2023 17:08:02 GMT
ADD file:6c0661b94e27ede70ca2a8842bdab5bc26b9ae4760b17870eda9d595672795ff in / 
# Mon, 05 Jun 2023 17:08:02 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:fb0a6f6b1798ce3ee565023c3a50777fff89bf6761a0985c8ff93aa903f7d0f1`  
		Last Modified: Mon, 05 Jun 2023 17:26:40 GMT  
		Size: 26.0 MB (25974252 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:focal` - linux; ppc64le

```console
$ docker pull ubuntu@sha256:1b176384bc513bb425b497364f1d6353ac1b285d48862c22a9b7c450c431d4bf
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.1 MB (32070916 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c0cad30b7d8589358e8074d6fb495d774d8c52cfa8ab35ed10f518a2c8b7586c`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 05 Jun 2023 17:08:24 GMT
ARG RELEASE
# Mon, 05 Jun 2023 17:08:24 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 05 Jun 2023 17:08:24 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 05 Jun 2023 17:08:25 GMT
LABEL org.opencontainers.image.version=20.04
# Mon, 05 Jun 2023 17:08:28 GMT
ADD file:0a2372ac4d43f0f4ada2b55dd0a359df73a828a9aa9426bfdd05a02b9c4b2bd9 in / 
# Mon, 05 Jun 2023 17:08:28 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:a42700f678f7c62f7053fbbd2b046ac1742685ac4262717c9c6db8a8e872884d`  
		Last Modified: Mon, 05 Jun 2023 17:26:52 GMT  
		Size: 32.1 MB (32070916 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:focal` - linux; s390x

```console
$ docker pull ubuntu@sha256:90dca1700c58ce633d6d7566ddcab50d8211e07a39d975197c43ddccc7ca84d1
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.4 MB (26351327 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:54f1d743745c70710688433dda5ce774740bacdbb8f6d824ac1a6150da5a72fe`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 05 Jun 2023 17:07:58 GMT
ARG RELEASE
# Mon, 05 Jun 2023 17:07:58 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 05 Jun 2023 17:07:58 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 05 Jun 2023 17:07:58 GMT
LABEL org.opencontainers.image.version=20.04
# Mon, 05 Jun 2023 17:08:00 GMT
ADD file:3aeae4efd27981f5d9d2894756f698b4fab4fbc6de4258ebd03baad8bf626d5c in / 
# Mon, 05 Jun 2023 17:08:00 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:83be4b9c36a879f795854cd45dc3e4f79cef2d7685ab6f26770b8a9e5c8baadd`  
		Last Modified: Mon, 05 Jun 2023 17:26:58 GMT  
		Size: 26.4 MB (26351327 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

## `ubuntu:focal-20230624`

**does not exist** (yet?)

## `ubuntu:jammy`

```console
$ docker pull ubuntu@sha256:6120be6a2b7ce665d0cbddc3ce6eae60fe94637c6a66985312d1f02f63cc0bcd
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
$ docker pull ubuntu@sha256:83f0c2a8d6f266d687d55b5cb1cb2201148eb7ac449e4202d9646b9083f1cee0
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.5 MB (29533050 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:99284ca6cea039c7784d1414608c6e846dd56830c2a13e1341be681c3ffcc8ac`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 05 Jun 2023 17:00:37 GMT
ARG RELEASE
# Mon, 05 Jun 2023 17:00:37 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 05 Jun 2023 17:00:37 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 05 Jun 2023 17:00:37 GMT
LABEL org.opencontainers.image.version=22.04
# Mon, 05 Jun 2023 17:00:39 GMT
ADD file:0ad2ee2cfb186802f49c9bf4148674d1c6fc201f83478ec01ffaa7086d491323 in / 
# Mon, 05 Jun 2023 17:00:39 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:6b851dcae6ca1461dde247915abc5048061f34332929ca8fb37d9dc18f2e2f44`  
		Last Modified: Mon, 05 Jun 2023 17:20:26 GMT  
		Size: 29.5 MB (29533050 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:jammy` - linux; arm variant v7

```console
$ docker pull ubuntu@sha256:9aa2ce874cc0d140b3344fb6125d0ef540d347bca8a13c2270ca1c7a40490be3
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.1 MB (26140710 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3681d7421d4545f9eb7b1aabcb24b041b347b37705f89a858f831b94d8e2f0bf`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 05 Jun 2023 16:59:35 GMT
ARG RELEASE
# Mon, 05 Jun 2023 16:59:35 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 05 Jun 2023 16:59:35 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 05 Jun 2023 16:59:35 GMT
LABEL org.opencontainers.image.version=22.04
# Mon, 05 Jun 2023 16:59:40 GMT
ADD file:5425962ced738173a50965fc5cd95c79d0a319323df4a34e9da3f5037a5264c3 in / 
# Mon, 05 Jun 2023 16:59:40 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:4ceecae09ee56d3fb7d5d26ff9505f3aa7e7cc5e54545fbecde69ef046b84f1c`  
		Last Modified: Mon, 05 Jun 2023 17:20:38 GMT  
		Size: 26.1 MB (26140710 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:jammy` - linux; arm64 variant v8

```console
$ docker pull ubuntu@sha256:25de8a960c338b7d38aa15c012ceee70d8e29239db97596d6ecc50a5085d8f7a
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.3 MB (27346742 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cfb01e8e31210c9bfc5412c3fc1b8b7aea849bc2a9c21f47553bd31cc8fd79f9`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 05 Jun 2023 17:11:17 GMT
ARG RELEASE
# Mon, 05 Jun 2023 17:11:17 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 05 Jun 2023 17:11:17 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 05 Jun 2023 17:11:17 GMT
LABEL org.opencontainers.image.version=22.04
# Mon, 05 Jun 2023 17:11:19 GMT
ADD file:1043594b482384e967c94378b65ec4bc7a38190649a94f0325b7fb00be0a623e in / 
# Mon, 05 Jun 2023 17:11:19 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:b2837baf7808226f588fabacb30598287e02d4dbf120eaf968c5299a6c2e9619`  
		Last Modified: Mon, 05 Jun 2023 17:20:32 GMT  
		Size: 27.3 MB (27346742 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:jammy` - linux; ppc64le

```console
$ docker pull ubuntu@sha256:eb4e647121c71cc9305e466d9c844a1207f90bab2e689310050e66e8b4f4d534
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.6 MB (34591237 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:16fc5784936f704a4bd8208deeb624554aeb2cdab87301aab60391db8f7ec590`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 05 Jun 2023 17:01:00 GMT
ARG RELEASE
# Mon, 05 Jun 2023 17:01:00 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 05 Jun 2023 17:01:00 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 05 Jun 2023 17:01:01 GMT
LABEL org.opencontainers.image.version=22.04
# Mon, 05 Jun 2023 17:01:03 GMT
ADD file:00c4f44b35b683caef54d5b8b0e0b1e68872f45eae17dd7543adaf6c54512447 in / 
# Mon, 05 Jun 2023 17:01:04 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:d3c256ab34973cfc9065065e684e5e5d1dac1eeb77974324e0de68944af26f62`  
		Last Modified: Mon, 05 Jun 2023 17:20:44 GMT  
		Size: 34.6 MB (34591237 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:jammy` - linux; s390x

```console
$ docker pull ubuntu@sha256:0b8eed006f12768a3a15fdf891f77d9a5fbf805882f15a8180c428f47d9d297e
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.0 MB (28015524 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8c7ef32086a3a754c9d2e6f68f731d3cd053c01ec070ae20c059995a33ac4afc`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 05 Jun 2023 17:01:02 GMT
ARG RELEASE
# Mon, 05 Jun 2023 17:01:02 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 05 Jun 2023 17:01:02 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 05 Jun 2023 17:01:02 GMT
LABEL org.opencontainers.image.version=22.04
# Mon, 05 Jun 2023 17:01:04 GMT
ADD file:2d2f31ec110b9e7ec21a9d4824a430acdaabf0b4e9c1cdd337438992859b57ae in / 
# Mon, 05 Jun 2023 17:01:04 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:02f8248e8d232d4898b07be78857694fe6651b4faa795e63952783f0aa44f1fe`  
		Last Modified: Mon, 05 Jun 2023 17:20:50 GMT  
		Size: 28.0 MB (28015524 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

## `ubuntu:jammy-20230624`

**does not exist** (yet?)

## `ubuntu:kinetic`

```console
$ docker pull ubuntu@sha256:1fa7586c0f10cc7ce7ca379ae48bf06776325b9f8e97963ce40803a8bcc07dca
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
$ docker pull ubuntu@sha256:80fb4ea0c0a384a3072a6be1879c342bb636b0d105209535ba893ba75ab38ede
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.7 MB (26704595 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e39f297e9dda29a8d8896051c30f32feb52c9dcfb68e8a561650a1dde97cc94b`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 05 Jun 2023 17:02:32 GMT
ARG RELEASE
# Mon, 05 Jun 2023 17:02:32 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 05 Jun 2023 17:02:32 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 05 Jun 2023 17:02:32 GMT
LABEL org.opencontainers.image.version=22.10
# Mon, 05 Jun 2023 17:02:34 GMT
ADD file:f8bb312bf73c62343d91c9988d58945c5d0fced3f559b95c4dd21a19183d933d in / 
# Mon, 05 Jun 2023 17:02:34 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:317e06b63fc01feacb4fa7a967d3a8c6fd35296935c83caa85ad28cd20add12b`  
		Last Modified: Mon, 05 Jun 2023 17:21:29 GMT  
		Size: 26.7 MB (26704595 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:kinetic` - linux; arm variant v7

```console
$ docker pull ubuntu@sha256:5dc1502337b177771dd9904822cde9abd2b26ee4014a3c6df7e912a9ef103db3
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.1 MB (25098670 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1120758c0ceafe38a213551ecf496a3b05011b323c13e36840d566b2ee02416d`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 05 Jun 2023 17:04:06 GMT
ARG RELEASE
# Mon, 05 Jun 2023 17:04:06 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 05 Jun 2023 17:04:06 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 05 Jun 2023 17:04:07 GMT
LABEL org.opencontainers.image.version=22.10
# Mon, 05 Jun 2023 17:04:15 GMT
ADD file:615be72e62c21704af356d6cfd4e32a7df8dd4b93d0c3ee3ea2e1641127c54ea in / 
# Mon, 05 Jun 2023 17:04:16 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:7eb2ece7978deb374e0aa4623aa1a44d513c34c7a56e23251a0dfbba314ea260`  
		Last Modified: Mon, 05 Jun 2023 17:21:41 GMT  
		Size: 25.1 MB (25098670 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:kinetic` - linux; arm64 variant v8

```console
$ docker pull ubuntu@sha256:dde2a31e58d07b2ed8be842eafae55b9a46b3629a0915dd6438fb3e484e46d65
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.8 MB (25770482 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:172adc9ce1cab441186106c04f9663f7b81edc9d3e8908b8dca58180df27ea16`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 05 Jun 2023 17:02:45 GMT
ARG RELEASE
# Mon, 05 Jun 2023 17:02:45 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 05 Jun 2023 17:02:45 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 05 Jun 2023 17:02:46 GMT
LABEL org.opencontainers.image.version=22.10
# Mon, 05 Jun 2023 17:02:50 GMT
ADD file:b85182b4593c262faef116755e01baa608e8090e1cb697d735485ff0bd5b353e in / 
# Mon, 05 Jun 2023 17:02:50 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:bb573a4d6d791b5d50f1118d01e4c9b2acc927522cec8740ac9957e37eeac29c`  
		Last Modified: Mon, 05 Jun 2023 17:21:35 GMT  
		Size: 25.8 MB (25770482 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:kinetic` - linux; ppc64le

```console
$ docker pull ubuntu@sha256:b2a4b994153a43ab4941ab8efbc43c189d0c76b9fe4f8dee9f8449cd6ed83d93
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.1 MB (31112867 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c8a632c9634c258b38d044be3dfa48ee0aee70c82531def42c6e701c10e15989`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 05 Jun 2023 17:10:48 GMT
ARG RELEASE
# Mon, 05 Jun 2023 17:10:48 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 05 Jun 2023 17:10:48 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 05 Jun 2023 17:10:48 GMT
LABEL org.opencontainers.image.version=22.10
# Mon, 05 Jun 2023 17:10:52 GMT
ADD file:48c30fe281554302bb6533dd33a43a0877851ac5ba59dc3aff3d3d9ceae6f8a9 in / 
# Mon, 05 Jun 2023 17:10:52 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:e4485626c4310d83f6d257d7c30db7a4fc23c70b98dec3ca37108fef26207e3c`  
		Last Modified: Mon, 05 Jun 2023 17:21:47 GMT  
		Size: 31.1 MB (31112867 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:kinetic` - linux; s390x

```console
$ docker pull ubuntu@sha256:1776cac9e796ccbe3048e682a977054303fc511313d8d7d43b805eec3d4669fa
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.5 MB (25489752 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d8c554a011867c58cc8ab63be78f10271da1d2a76c4498de2a5b33b7ecb26486`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 05 Jun 2023 17:10:49 GMT
ARG RELEASE
# Mon, 05 Jun 2023 17:10:49 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 05 Jun 2023 17:10:49 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 05 Jun 2023 17:10:49 GMT
LABEL org.opencontainers.image.version=22.10
# Mon, 05 Jun 2023 17:10:51 GMT
ADD file:2390e4c5ac4f862cf5fb266c70962a01f271fa692b74af886f18911482025825 in / 
# Mon, 05 Jun 2023 17:10:51 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:245e6239c00ff9b6decc18e3b64f2390bc669d50050fdfd65a8b91e45183fbe3`  
		Last Modified: Mon, 05 Jun 2023 17:21:53 GMT  
		Size: 25.5 MB (25489752 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

## `ubuntu:kinetic-20230624`

**does not exist** (yet?)

## `ubuntu:latest`

```console
$ docker pull ubuntu@sha256:6120be6a2b7ce665d0cbddc3ce6eae60fe94637c6a66985312d1f02f63cc0bcd
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
$ docker pull ubuntu@sha256:83f0c2a8d6f266d687d55b5cb1cb2201148eb7ac449e4202d9646b9083f1cee0
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.5 MB (29533050 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:99284ca6cea039c7784d1414608c6e846dd56830c2a13e1341be681c3ffcc8ac`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 05 Jun 2023 17:00:37 GMT
ARG RELEASE
# Mon, 05 Jun 2023 17:00:37 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 05 Jun 2023 17:00:37 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 05 Jun 2023 17:00:37 GMT
LABEL org.opencontainers.image.version=22.04
# Mon, 05 Jun 2023 17:00:39 GMT
ADD file:0ad2ee2cfb186802f49c9bf4148674d1c6fc201f83478ec01ffaa7086d491323 in / 
# Mon, 05 Jun 2023 17:00:39 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:6b851dcae6ca1461dde247915abc5048061f34332929ca8fb37d9dc18f2e2f44`  
		Last Modified: Mon, 05 Jun 2023 17:20:26 GMT  
		Size: 29.5 MB (29533050 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:latest` - linux; arm variant v7

```console
$ docker pull ubuntu@sha256:9aa2ce874cc0d140b3344fb6125d0ef540d347bca8a13c2270ca1c7a40490be3
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.1 MB (26140710 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3681d7421d4545f9eb7b1aabcb24b041b347b37705f89a858f831b94d8e2f0bf`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 05 Jun 2023 16:59:35 GMT
ARG RELEASE
# Mon, 05 Jun 2023 16:59:35 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 05 Jun 2023 16:59:35 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 05 Jun 2023 16:59:35 GMT
LABEL org.opencontainers.image.version=22.04
# Mon, 05 Jun 2023 16:59:40 GMT
ADD file:5425962ced738173a50965fc5cd95c79d0a319323df4a34e9da3f5037a5264c3 in / 
# Mon, 05 Jun 2023 16:59:40 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:4ceecae09ee56d3fb7d5d26ff9505f3aa7e7cc5e54545fbecde69ef046b84f1c`  
		Last Modified: Mon, 05 Jun 2023 17:20:38 GMT  
		Size: 26.1 MB (26140710 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:latest` - linux; arm64 variant v8

```console
$ docker pull ubuntu@sha256:25de8a960c338b7d38aa15c012ceee70d8e29239db97596d6ecc50a5085d8f7a
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.3 MB (27346742 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cfb01e8e31210c9bfc5412c3fc1b8b7aea849bc2a9c21f47553bd31cc8fd79f9`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 05 Jun 2023 17:11:17 GMT
ARG RELEASE
# Mon, 05 Jun 2023 17:11:17 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 05 Jun 2023 17:11:17 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 05 Jun 2023 17:11:17 GMT
LABEL org.opencontainers.image.version=22.04
# Mon, 05 Jun 2023 17:11:19 GMT
ADD file:1043594b482384e967c94378b65ec4bc7a38190649a94f0325b7fb00be0a623e in / 
# Mon, 05 Jun 2023 17:11:19 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:b2837baf7808226f588fabacb30598287e02d4dbf120eaf968c5299a6c2e9619`  
		Last Modified: Mon, 05 Jun 2023 17:20:32 GMT  
		Size: 27.3 MB (27346742 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:latest` - linux; ppc64le

```console
$ docker pull ubuntu@sha256:eb4e647121c71cc9305e466d9c844a1207f90bab2e689310050e66e8b4f4d534
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.6 MB (34591237 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:16fc5784936f704a4bd8208deeb624554aeb2cdab87301aab60391db8f7ec590`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 05 Jun 2023 17:01:00 GMT
ARG RELEASE
# Mon, 05 Jun 2023 17:01:00 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 05 Jun 2023 17:01:00 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 05 Jun 2023 17:01:01 GMT
LABEL org.opencontainers.image.version=22.04
# Mon, 05 Jun 2023 17:01:03 GMT
ADD file:00c4f44b35b683caef54d5b8b0e0b1e68872f45eae17dd7543adaf6c54512447 in / 
# Mon, 05 Jun 2023 17:01:04 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:d3c256ab34973cfc9065065e684e5e5d1dac1eeb77974324e0de68944af26f62`  
		Last Modified: Mon, 05 Jun 2023 17:20:44 GMT  
		Size: 34.6 MB (34591237 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:latest` - linux; s390x

```console
$ docker pull ubuntu@sha256:0b8eed006f12768a3a15fdf891f77d9a5fbf805882f15a8180c428f47d9d297e
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.0 MB (28015524 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8c7ef32086a3a754c9d2e6f68f731d3cd053c01ec070ae20c059995a33ac4afc`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 05 Jun 2023 17:01:02 GMT
ARG RELEASE
# Mon, 05 Jun 2023 17:01:02 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 05 Jun 2023 17:01:02 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 05 Jun 2023 17:01:02 GMT
LABEL org.opencontainers.image.version=22.04
# Mon, 05 Jun 2023 17:01:04 GMT
ADD file:2d2f31ec110b9e7ec21a9d4824a430acdaabf0b4e9c1cdd337438992859b57ae in / 
# Mon, 05 Jun 2023 17:01:04 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:02f8248e8d232d4898b07be78857694fe6651b4faa795e63952783f0aa44f1fe`  
		Last Modified: Mon, 05 Jun 2023 17:20:50 GMT  
		Size: 28.0 MB (28015524 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

## `ubuntu:lunar`

```console
$ docker pull ubuntu@sha256:b5d5cddaeb8d2f150660cf8f9a1203dd450ac765e6c07630176ac6486eceaddb
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
$ docker pull ubuntu@sha256:09f035f46361d193ded647342903b413d57d05cc06acff8285f9dda9f2d269d5
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.8 MB (26836883 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1ed313b0551f6255bb9ea7fd953363f0f306d9e2e92dc9fb94cbdf70e3dafb6f`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 15 Jun 2023 08:28:38 GMT
ARG RELEASE
# Thu, 15 Jun 2023 08:28:38 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 15 Jun 2023 08:28:38 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 15 Jun 2023 08:28:38 GMT
LABEL org.opencontainers.image.version=23.04
# Thu, 15 Jun 2023 08:28:39 GMT
ADD file:708314051e878a0c6071fb2c8d4458a04ce058f47f2cfaa58c1b5a42e837ca0f in / 
# Thu, 15 Jun 2023 08:28:40 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:3a9d46cc3977f1066a9dd08f845b76f7f7d46e4ef74fdf8ed1f4db514ea5a45d`  
		Last Modified: Thu, 15 Jun 2023 09:08:28 GMT  
		Size: 26.8 MB (26836883 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:lunar` - linux; arm variant v7

```console
$ docker pull ubuntu@sha256:98e3a45616c77d754ce50a12634c507cecf9b53ccb2f48e94b20db7b4b698618
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **24.6 MB (24636364 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:678dff67c6b9c6ec4eaccccccd2ffae1ddbf85b5e5309ac56522d7442f3f8c2d`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 15 Jun 2023 08:10:50 GMT
ARG RELEASE
# Thu, 15 Jun 2023 08:10:50 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 15 Jun 2023 08:10:51 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 15 Jun 2023 08:10:51 GMT
LABEL org.opencontainers.image.version=23.04
# Thu, 15 Jun 2023 08:10:53 GMT
ADD file:8484efc06b5f22d170eef374f45df452d8e36f4cbef702f7ee4d1f130dd28093 in / 
# Thu, 15 Jun 2023 08:10:53 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:fb49e82a48f62b12a885a1a02ae80f5261ab51e3f138c0190fc8d119247fd11c`  
		Last Modified: Thu, 15 Jun 2023 09:08:40 GMT  
		Size: 24.6 MB (24636364 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:lunar` - linux; arm64 variant v8

```console
$ docker pull ubuntu@sha256:2ea9408d05cc2543752070f336452eda81593c2001f9931a0451bad3a45d3a31
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.1 MB (26088803 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f6b331a8a5e1bb537caa9a8e3d3f6308563136db02ab0501499e819e36d9f48a`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 15 Jun 2023 08:33:24 GMT
ARG RELEASE
# Thu, 15 Jun 2023 08:33:25 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 15 Jun 2023 08:33:25 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 15 Jun 2023 08:33:25 GMT
LABEL org.opencontainers.image.version=23.04
# Thu, 15 Jun 2023 08:33:58 GMT
ADD file:064ac1f238394a53372e0db107e28835aa3c39ed189a15fe85c532bbb50bfbaf in / 
# Thu, 15 Jun 2023 08:33:59 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:19e8382a46db1cf2ede3739a9337cad793e2228c0e455f8969bbbc14b4d6f28e`  
		Last Modified: Thu, 15 Jun 2023 09:08:34 GMT  
		Size: 26.1 MB (26088803 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:lunar` - linux; ppc64le

```console
$ docker pull ubuntu@sha256:cac0b3657eb2260df362c4949ec416d6377b36d5c2999e1765874dcbadeca4cd
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.0 MB (31029474 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:da0d4e75ccb4b903cf3c7d3515fdbbe2462a8043abbcf13667b6f860fc11302e`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 15 Jun 2023 08:29:14 GMT
ARG RELEASE
# Thu, 15 Jun 2023 08:29:14 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 15 Jun 2023 08:29:15 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 15 Jun 2023 08:29:15 GMT
LABEL org.opencontainers.image.version=23.04
# Thu, 15 Jun 2023 08:29:17 GMT
ADD file:5ebdf4bd4bc2b27019f20fb1964a395fa504d4f20e208c54237e363895b492d7 in / 
# Thu, 15 Jun 2023 08:29:18 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:223122c533fb03fa9f10684bc8fb23adf1f08af994530d4c9403f9086da8952b`  
		Last Modified: Thu, 15 Jun 2023 09:08:47 GMT  
		Size: 31.0 MB (31029474 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:lunar` - linux; s390x

```console
$ docker pull ubuntu@sha256:6b7f8b6a5280fe23d857ac4cd887805f2a7d014d3d88dccedd81379291a54a34
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.7 MB (25716588 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:08ed40f2186d81239c9993cac2d5749fcad7ee65da4786f87d8e3d0caea927e1`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 15 Jun 2023 08:11:16 GMT
ARG RELEASE
# Thu, 15 Jun 2023 08:11:16 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 15 Jun 2023 08:11:16 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 15 Jun 2023 08:11:16 GMT
LABEL org.opencontainers.image.version=23.04
# Thu, 15 Jun 2023 08:11:18 GMT
ADD file:3974fe053080180d99954042c25b3bd0c82e320fb4521b197cbc45f21885fc43 in / 
# Thu, 15 Jun 2023 08:11:18 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:1611e8f17f580c929b21787327a1e5133fd1c1954ec9b270101aee4380735e40`  
		Last Modified: Thu, 15 Jun 2023 09:08:53 GMT  
		Size: 25.7 MB (25716588 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

## `ubuntu:lunar-20230615`

```console
$ docker pull ubuntu@sha256:b5d5cddaeb8d2f150660cf8f9a1203dd450ac765e6c07630176ac6486eceaddb
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `ubuntu:lunar-20230615` - linux; amd64

```console
$ docker pull ubuntu@sha256:09f035f46361d193ded647342903b413d57d05cc06acff8285f9dda9f2d269d5
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.8 MB (26836883 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1ed313b0551f6255bb9ea7fd953363f0f306d9e2e92dc9fb94cbdf70e3dafb6f`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 15 Jun 2023 08:28:38 GMT
ARG RELEASE
# Thu, 15 Jun 2023 08:28:38 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 15 Jun 2023 08:28:38 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 15 Jun 2023 08:28:38 GMT
LABEL org.opencontainers.image.version=23.04
# Thu, 15 Jun 2023 08:28:39 GMT
ADD file:708314051e878a0c6071fb2c8d4458a04ce058f47f2cfaa58c1b5a42e837ca0f in / 
# Thu, 15 Jun 2023 08:28:40 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:3a9d46cc3977f1066a9dd08f845b76f7f7d46e4ef74fdf8ed1f4db514ea5a45d`  
		Last Modified: Thu, 15 Jun 2023 09:08:28 GMT  
		Size: 26.8 MB (26836883 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:lunar-20230615` - linux; arm variant v7

```console
$ docker pull ubuntu@sha256:98e3a45616c77d754ce50a12634c507cecf9b53ccb2f48e94b20db7b4b698618
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **24.6 MB (24636364 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:678dff67c6b9c6ec4eaccccccd2ffae1ddbf85b5e5309ac56522d7442f3f8c2d`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 15 Jun 2023 08:10:50 GMT
ARG RELEASE
# Thu, 15 Jun 2023 08:10:50 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 15 Jun 2023 08:10:51 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 15 Jun 2023 08:10:51 GMT
LABEL org.opencontainers.image.version=23.04
# Thu, 15 Jun 2023 08:10:53 GMT
ADD file:8484efc06b5f22d170eef374f45df452d8e36f4cbef702f7ee4d1f130dd28093 in / 
# Thu, 15 Jun 2023 08:10:53 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:fb49e82a48f62b12a885a1a02ae80f5261ab51e3f138c0190fc8d119247fd11c`  
		Last Modified: Thu, 15 Jun 2023 09:08:40 GMT  
		Size: 24.6 MB (24636364 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:lunar-20230615` - linux; arm64 variant v8

```console
$ docker pull ubuntu@sha256:2ea9408d05cc2543752070f336452eda81593c2001f9931a0451bad3a45d3a31
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.1 MB (26088803 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f6b331a8a5e1bb537caa9a8e3d3f6308563136db02ab0501499e819e36d9f48a`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 15 Jun 2023 08:33:24 GMT
ARG RELEASE
# Thu, 15 Jun 2023 08:33:25 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 15 Jun 2023 08:33:25 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 15 Jun 2023 08:33:25 GMT
LABEL org.opencontainers.image.version=23.04
# Thu, 15 Jun 2023 08:33:58 GMT
ADD file:064ac1f238394a53372e0db107e28835aa3c39ed189a15fe85c532bbb50bfbaf in / 
# Thu, 15 Jun 2023 08:33:59 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:19e8382a46db1cf2ede3739a9337cad793e2228c0e455f8969bbbc14b4d6f28e`  
		Last Modified: Thu, 15 Jun 2023 09:08:34 GMT  
		Size: 26.1 MB (26088803 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:lunar-20230615` - linux; ppc64le

```console
$ docker pull ubuntu@sha256:cac0b3657eb2260df362c4949ec416d6377b36d5c2999e1765874dcbadeca4cd
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.0 MB (31029474 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:da0d4e75ccb4b903cf3c7d3515fdbbe2462a8043abbcf13667b6f860fc11302e`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 15 Jun 2023 08:29:14 GMT
ARG RELEASE
# Thu, 15 Jun 2023 08:29:14 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 15 Jun 2023 08:29:15 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 15 Jun 2023 08:29:15 GMT
LABEL org.opencontainers.image.version=23.04
# Thu, 15 Jun 2023 08:29:17 GMT
ADD file:5ebdf4bd4bc2b27019f20fb1964a395fa504d4f20e208c54237e363895b492d7 in / 
# Thu, 15 Jun 2023 08:29:18 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:223122c533fb03fa9f10684bc8fb23adf1f08af994530d4c9403f9086da8952b`  
		Last Modified: Thu, 15 Jun 2023 09:08:47 GMT  
		Size: 31.0 MB (31029474 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:lunar-20230615` - linux; s390x

```console
$ docker pull ubuntu@sha256:6b7f8b6a5280fe23d857ac4cd887805f2a7d014d3d88dccedd81379291a54a34
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.7 MB (25716588 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:08ed40f2186d81239c9993cac2d5749fcad7ee65da4786f87d8e3d0caea927e1`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 15 Jun 2023 08:11:16 GMT
ARG RELEASE
# Thu, 15 Jun 2023 08:11:16 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 15 Jun 2023 08:11:16 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 15 Jun 2023 08:11:16 GMT
LABEL org.opencontainers.image.version=23.04
# Thu, 15 Jun 2023 08:11:18 GMT
ADD file:3974fe053080180d99954042c25b3bd0c82e320fb4521b197cbc45f21885fc43 in / 
# Thu, 15 Jun 2023 08:11:18 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:1611e8f17f580c929b21787327a1e5133fd1c1954ec9b270101aee4380735e40`  
		Last Modified: Thu, 15 Jun 2023 09:08:53 GMT  
		Size: 25.7 MB (25716588 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

## `ubuntu:mantic`

```console
$ docker pull ubuntu@sha256:bd1e0eb3171a6e499c84211e73c4f5f5b2a585507256f772f5c4f4420a3d8591
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
$ docker pull ubuntu@sha256:07460e809a7141b84050c6d68220c1f7e2aa58b0bc124c40a1440988bfd87e6b
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.9 MB (26931867 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ce0fd6ed554b4fa85755cd2f9fefc45a1bff5e640b1090f4573997837f6c46b2`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 07 Jun 2023 04:39:09 GMT
ARG RELEASE
# Wed, 07 Jun 2023 04:39:09 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 07 Jun 2023 04:39:09 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 07 Jun 2023 04:39:09 GMT
LABEL org.opencontainers.image.version=23.10
# Wed, 07 Jun 2023 04:39:10 GMT
ADD file:d8dc8c4236b9885e64ccd27399ed8dddab7d39915d76378527cb730855aba0e1 in / 
# Wed, 07 Jun 2023 04:39:10 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:a3cc0ea50b9aef0e9b8b228c37edf92b0dfcb177d34ed50433918ae5eec172be`  
		Last Modified: Wed, 07 Jun 2023 04:57:40 GMT  
		Size: 26.9 MB (26931867 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:mantic` - linux; arm variant v7

```console
$ docker pull ubuntu@sha256:bf18ca0b049d010b72c35574c0261ef9c231fffb7588709e05a6b807c081e552
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **24.5 MB (24478190 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4eabbb20f267b27e88fe450b3d209313994eeb87c19d8cbdec2b2f8e821a1ce5`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 07 Jun 2023 04:48:07 GMT
ARG RELEASE
# Wed, 07 Jun 2023 04:48:07 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 07 Jun 2023 04:48:08 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 07 Jun 2023 04:48:08 GMT
LABEL org.opencontainers.image.version=23.10
# Wed, 07 Jun 2023 04:48:12 GMT
ADD file:65e05498800189bf1f48f5c6df21d144e18e5e069db55d0b88d45c04cc1fe4de in / 
# Wed, 07 Jun 2023 04:48:12 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:df4275b0f8f556aa5462a1fad0a0a188bc3d7b287bc6120389314f6b9bd6566e`  
		Last Modified: Wed, 07 Jun 2023 04:57:51 GMT  
		Size: 24.5 MB (24478190 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:mantic` - linux; arm64 variant v8

```console
$ docker pull ubuntu@sha256:d9c68082dd554f1adf3ed6169d08f0aae5431b4a7bddb8c19951eae6bd607097
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.1 MB (26131158 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0a27f5fa4b6e23e37d77cb2410d8f9efb5a9f5698e10bf3aef9bb503b14497d3`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 07 Jun 2023 04:42:14 GMT
ARG RELEASE
# Wed, 07 Jun 2023 04:42:14 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 07 Jun 2023 04:42:14 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 07 Jun 2023 04:42:14 GMT
LABEL org.opencontainers.image.version=23.10
# Wed, 07 Jun 2023 04:42:16 GMT
ADD file:3f4faed988a03b7d05aefe677906592aade4d2bae1ec3f7055c1f10744a38de0 in / 
# Wed, 07 Jun 2023 04:42:16 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:f698dd1f118f52521a462f35505a0bca0dc8a7e17802e11146a6c0acfbfc797d`  
		Last Modified: Wed, 07 Jun 2023 04:57:46 GMT  
		Size: 26.1 MB (26131158 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:mantic` - linux; ppc64le

```console
$ docker pull ubuntu@sha256:8d9660ab5ab6a35050e6f5ac4ff4170e85c1e6776e83d075f9331b85215b96a4
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.0 MB (30966286 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7a4004a6116d82330c1bb10006b89dcfb699827cd79a405a16dd59e3e33889d4`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 07 Jun 2023 04:48:25 GMT
ARG RELEASE
# Wed, 07 Jun 2023 04:48:26 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 07 Jun 2023 04:48:26 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 07 Jun 2023 04:48:26 GMT
LABEL org.opencontainers.image.version=23.10
# Wed, 07 Jun 2023 04:48:28 GMT
ADD file:6cf1bffac55b7de64803fabdb35baf75349cc0a40c0b4c68ac2690b7123edc85 in / 
# Wed, 07 Jun 2023 04:48:29 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:537eb27ff37d9fd24f7097996a5a0ed640152c3656390c06baff05ecd549d691`  
		Last Modified: Wed, 07 Jun 2023 04:57:57 GMT  
		Size: 31.0 MB (30966286 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:mantic` - linux; s390x

```console
$ docker pull ubuntu@sha256:441bef6aaac131b562992783cb31ac363fb5fa5592c928be1fc6ec01b45fb0e8
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.8 MB (25750156 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:deb4b1b351b9ab4eff7e955188cbe7a5b818325f441be917beee6a25cbf66783`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 07 Jun 2023 04:42:36 GMT
ARG RELEASE
# Wed, 07 Jun 2023 04:42:36 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 07 Jun 2023 04:42:36 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 07 Jun 2023 04:42:36 GMT
LABEL org.opencontainers.image.version=23.10
# Wed, 07 Jun 2023 04:42:38 GMT
ADD file:4e8ca8820de4a27d67ad223be645ce7a7a48289dfcbc01b4e1dbe3bc74ebbc56 in / 
# Wed, 07 Jun 2023 04:42:38 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:906d24b8296f0e80ba93ccd8c8a85183d978d41115e21f9aba3044ad0d38b45e`  
		Last Modified: Wed, 07 Jun 2023 04:58:03 GMT  
		Size: 25.8 MB (25750156 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

## `ubuntu:mantic-20230624`

**does not exist** (yet?)

## `ubuntu:rolling`

```console
$ docker pull ubuntu@sha256:b5d5cddaeb8d2f150660cf8f9a1203dd450ac765e6c07630176ac6486eceaddb
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
$ docker pull ubuntu@sha256:09f035f46361d193ded647342903b413d57d05cc06acff8285f9dda9f2d269d5
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.8 MB (26836883 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1ed313b0551f6255bb9ea7fd953363f0f306d9e2e92dc9fb94cbdf70e3dafb6f`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 15 Jun 2023 08:28:38 GMT
ARG RELEASE
# Thu, 15 Jun 2023 08:28:38 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 15 Jun 2023 08:28:38 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 15 Jun 2023 08:28:38 GMT
LABEL org.opencontainers.image.version=23.04
# Thu, 15 Jun 2023 08:28:39 GMT
ADD file:708314051e878a0c6071fb2c8d4458a04ce058f47f2cfaa58c1b5a42e837ca0f in / 
# Thu, 15 Jun 2023 08:28:40 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:3a9d46cc3977f1066a9dd08f845b76f7f7d46e4ef74fdf8ed1f4db514ea5a45d`  
		Last Modified: Thu, 15 Jun 2023 09:08:28 GMT  
		Size: 26.8 MB (26836883 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:rolling` - linux; arm variant v7

```console
$ docker pull ubuntu@sha256:98e3a45616c77d754ce50a12634c507cecf9b53ccb2f48e94b20db7b4b698618
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **24.6 MB (24636364 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:678dff67c6b9c6ec4eaccccccd2ffae1ddbf85b5e5309ac56522d7442f3f8c2d`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 15 Jun 2023 08:10:50 GMT
ARG RELEASE
# Thu, 15 Jun 2023 08:10:50 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 15 Jun 2023 08:10:51 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 15 Jun 2023 08:10:51 GMT
LABEL org.opencontainers.image.version=23.04
# Thu, 15 Jun 2023 08:10:53 GMT
ADD file:8484efc06b5f22d170eef374f45df452d8e36f4cbef702f7ee4d1f130dd28093 in / 
# Thu, 15 Jun 2023 08:10:53 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:fb49e82a48f62b12a885a1a02ae80f5261ab51e3f138c0190fc8d119247fd11c`  
		Last Modified: Thu, 15 Jun 2023 09:08:40 GMT  
		Size: 24.6 MB (24636364 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:rolling` - linux; arm64 variant v8

```console
$ docker pull ubuntu@sha256:2ea9408d05cc2543752070f336452eda81593c2001f9931a0451bad3a45d3a31
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.1 MB (26088803 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f6b331a8a5e1bb537caa9a8e3d3f6308563136db02ab0501499e819e36d9f48a`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 15 Jun 2023 08:33:24 GMT
ARG RELEASE
# Thu, 15 Jun 2023 08:33:25 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 15 Jun 2023 08:33:25 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 15 Jun 2023 08:33:25 GMT
LABEL org.opencontainers.image.version=23.04
# Thu, 15 Jun 2023 08:33:58 GMT
ADD file:064ac1f238394a53372e0db107e28835aa3c39ed189a15fe85c532bbb50bfbaf in / 
# Thu, 15 Jun 2023 08:33:59 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:19e8382a46db1cf2ede3739a9337cad793e2228c0e455f8969bbbc14b4d6f28e`  
		Last Modified: Thu, 15 Jun 2023 09:08:34 GMT  
		Size: 26.1 MB (26088803 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:rolling` - linux; ppc64le

```console
$ docker pull ubuntu@sha256:cac0b3657eb2260df362c4949ec416d6377b36d5c2999e1765874dcbadeca4cd
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.0 MB (31029474 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:da0d4e75ccb4b903cf3c7d3515fdbbe2462a8043abbcf13667b6f860fc11302e`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 15 Jun 2023 08:29:14 GMT
ARG RELEASE
# Thu, 15 Jun 2023 08:29:14 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 15 Jun 2023 08:29:15 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 15 Jun 2023 08:29:15 GMT
LABEL org.opencontainers.image.version=23.04
# Thu, 15 Jun 2023 08:29:17 GMT
ADD file:5ebdf4bd4bc2b27019f20fb1964a395fa504d4f20e208c54237e363895b492d7 in / 
# Thu, 15 Jun 2023 08:29:18 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:223122c533fb03fa9f10684bc8fb23adf1f08af994530d4c9403f9086da8952b`  
		Last Modified: Thu, 15 Jun 2023 09:08:47 GMT  
		Size: 31.0 MB (31029474 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:rolling` - linux; s390x

```console
$ docker pull ubuntu@sha256:6b7f8b6a5280fe23d857ac4cd887805f2a7d014d3d88dccedd81379291a54a34
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.7 MB (25716588 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:08ed40f2186d81239c9993cac2d5749fcad7ee65da4786f87d8e3d0caea927e1`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 15 Jun 2023 08:11:16 GMT
ARG RELEASE
# Thu, 15 Jun 2023 08:11:16 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 15 Jun 2023 08:11:16 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 15 Jun 2023 08:11:16 GMT
LABEL org.opencontainers.image.version=23.04
# Thu, 15 Jun 2023 08:11:18 GMT
ADD file:3974fe053080180d99954042c25b3bd0c82e320fb4521b197cbc45f21885fc43 in / 
# Thu, 15 Jun 2023 08:11:18 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:1611e8f17f580c929b21787327a1e5133fd1c1954ec9b270101aee4380735e40`  
		Last Modified: Thu, 15 Jun 2023 09:08:53 GMT  
		Size: 25.7 MB (25716588 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
