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
$ docker pull ubuntu@sha256:454eb772508cebb744a4561dd25d3ba52e110513e9d7916ab5c89224810a0d7f
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
$ docker pull ubuntu@sha256:8c38f4ea0b178a98e4f9f831b29b7966d6654414c1dc008591c6ec77de3bf2c9
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.5 MB (27505622 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:14be0685b7682b182af5b862c9638cb1cb4ca1a70bd5aa90deed96e9cca881e7`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 28 Jun 2023 09:59:08 GMT
ARG RELEASE
# Wed, 28 Jun 2023 09:59:08 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 09:59:08 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 09:59:08 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 28 Jun 2023 09:59:10 GMT
ADD file:12f97b7b044d0d1166dd59408c67f5610a764127aa8a01bc57db23bee48911af in / 
# Wed, 28 Jun 2023 09:59:10 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:01085d60b3a624c06a7132ff0749efc6e6565d9f2531d7685ff559fb5d0f669f`  
		Last Modified: Wed, 28 Jun 2023 10:13:37 GMT  
		Size: 27.5 MB (27505622 bytes)  
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
$ docker pull ubuntu@sha256:7fa3e1a7f357f2ee21918f3ad5eeab7a0d02a7452acdaecc47f585ed6e52d76a
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.4 MB (26350273 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:10bdc248f7d72bc0aa775d61bceae878a8443d11d651d172a28fa56644492df9`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 28 Jun 2023 10:01:13 GMT
ARG RELEASE
# Wed, 28 Jun 2023 10:01:13 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 10:01:13 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 10:01:14 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 28 Jun 2023 10:01:15 GMT
ADD file:777fd71e798b91bf768b21e1ca4403f388db9936ef55ef68b4b019cb167fa707 in / 
# Wed, 28 Jun 2023 10:01:15 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:0ebf1bc80a393479c293dfa52056fa26e7e3699214a6559bd7004f7c2d3c2832`  
		Last Modified: Wed, 28 Jun 2023 10:14:02 GMT  
		Size: 26.4 MB (26350273 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

## `ubuntu:22.04`

```console
$ docker pull ubuntu@sha256:1a8c20aeeed491d5aa4ab85946adefeecb90ec10bfd7a316fe3b632e3a917674
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
$ docker pull ubuntu@sha256:b060fffe8e1561c9c3e6dea6db487b900100fc26830b9ea2ec966c151ab4c020
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.5 MB (29533422 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5a81c4b8502e4979e75bd8f91343b95b0d695ab67f241dbed0d1530a35bde1eb`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 28 Jun 2023 08:37:40 GMT
ARG RELEASE
# Wed, 28 Jun 2023 08:37:40 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 08:37:40 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 08:37:40 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 28 Jun 2023 08:37:42 GMT
ADD file:140fb5108b4a2861b5718ad03b4a5174bba03589ea8d4c053e6a0b282f439ff3 in / 
# Wed, 28 Jun 2023 08:37:42 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:3153aa388d026c26a2235e1ed0163e350e451f41a8a313e1804d7e1afb857ab4`  
		Last Modified: Wed, 28 Jun 2023 08:58:40 GMT  
		Size: 29.5 MB (29533422 bytes)  
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
$ docker pull ubuntu@sha256:107cc410d683e41f2765125ec3b3aba514025348590539fcc079fa02d54f5708
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.0 MB (28016094 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ab733017eab481028e4f46a149cba2e422b2bc0c15a07c9bd29e7d431b568546`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 28 Jun 2023 08:53:20 GMT
ARG RELEASE
# Wed, 28 Jun 2023 08:53:20 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 08:53:20 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 08:53:20 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 28 Jun 2023 08:53:22 GMT
ADD file:fa0aef35be7808c8fd6751a52bdec4dd81057e2fcaa075c547a1db53640dae9a in / 
# Wed, 28 Jun 2023 08:53:22 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:ccff9014dcde158442f3978d42c5311f5833a9a4200b72f93a87ca7f7542c39a`  
		Last Modified: Wed, 28 Jun 2023 08:59:07 GMT  
		Size: 28.0 MB (28016094 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

## `ubuntu:22.10`

```console
$ docker pull ubuntu@sha256:534d1acc4da51c47b477ec1a764bc5ed3c007bec93ee08d832538077cd0bdeaa
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
$ docker pull ubuntu@sha256:d36481db487c935436420cc4b705db8c81eec3872085ebd27963b775695fbe24
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.7 MB (26704806 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:692eb4a905c074054e0a35d647671f0e32ed150d15b23fd7bc745cfb2fdeddbd`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 28 Jun 2023 08:23:07 GMT
ARG RELEASE
# Wed, 28 Jun 2023 08:23:07 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 08:23:07 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 08:23:07 GMT
LABEL org.opencontainers.image.version=22.10
# Wed, 28 Jun 2023 08:23:09 GMT
ADD file:50094673f74cf3945ac21e23bb84d41d3516bc1ac90ebf7f17379288c33c17b2 in / 
# Wed, 28 Jun 2023 08:23:09 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:3ad6ea492c35ef48892b4587449510d372516d5969073eeaa6601a380e861c57`  
		Last Modified: Wed, 28 Jun 2023 09:32:54 GMT  
		Size: 26.7 MB (26704806 bytes)  
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
$ docker pull ubuntu@sha256:0e44a443176bc6ca4e93ac2e465db208c43934238f410f378dc3c998eee696b5
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.5 MB (25490150 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:94aa2bec78551a9bd8a92d09f4fe0504cbd6f72a3ebaf9820bbcb93897b2aed1`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 28 Jun 2023 08:31:17 GMT
ARG RELEASE
# Wed, 28 Jun 2023 08:31:17 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 08:31:17 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 08:31:17 GMT
LABEL org.opencontainers.image.version=22.10
# Wed, 28 Jun 2023 08:31:19 GMT
ADD file:e6e44f70accdecf50c8942a8e70c4d2c1d419d1d61696730d8aeda653da7216b in / 
# Wed, 28 Jun 2023 08:31:20 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:7dfef942861c66b1cea3ce2cc82694e398544893132321d00bace936daa2c360`  
		Last Modified: Wed, 28 Jun 2023 09:33:20 GMT  
		Size: 25.5 MB (25490150 bytes)  
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
$ docker pull ubuntu@sha256:8c654938f08f63f36b4a04a16d299808ec14a7120048e3b23caab6cff4325378
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
$ docker pull ubuntu@sha256:266cbca633bcb1356b9be281efe251782d30830cee0c0cf6a3c952a3a655f040
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.9 MB (26945285 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3732473f881aa819c8754dc83b3bc7afc00361ea6090c135c72ccd38c9fd3637`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 28 Jun 2023 08:23:22 GMT
ARG RELEASE
# Wed, 28 Jun 2023 08:23:22 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 08:23:22 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 08:23:22 GMT
LABEL org.opencontainers.image.version=23.10
# Wed, 28 Jun 2023 08:23:24 GMT
ADD file:ce14b5aa15734922ec61b739c654f0d2843757c5f260778d4ecd9aa097cfacaf in / 
# Wed, 28 Jun 2023 08:23:24 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:4221febb096369c46cecc96ff4b3504b9ee19e25c6524e5da970ef0b30ee1b20`  
		Last Modified: Wed, 28 Jun 2023 09:26:34 GMT  
		Size: 26.9 MB (26945285 bytes)  
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
$ docker pull ubuntu@sha256:64ed81ed8782fb3323ae81aa60141d480787cd68b56fcd1a40be02b3be47d303
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.8 MB (25757906 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9ee8ecbb7ea7af1d7ed8af19d1e5b2614c0f5591cb25be48369e53b2122d5f76`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 28 Jun 2023 08:24:14 GMT
ARG RELEASE
# Wed, 28 Jun 2023 08:24:14 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 08:24:14 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 08:24:14 GMT
LABEL org.opencontainers.image.version=23.10
# Wed, 28 Jun 2023 08:24:16 GMT
ADD file:6046e0887f51e3cd521761c62077e42ceb11c3a32d6ecd6b0b32f7d9fbb83dec in / 
# Wed, 28 Jun 2023 08:24:16 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:da055310d6b309c0380a1d16ab6cd974a850123c5014f1e57d02df5852288ef5`  
		Last Modified: Wed, 28 Jun 2023 09:27:02 GMT  
		Size: 25.8 MB (25757906 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

## `ubuntu:devel`

```console
$ docker pull ubuntu@sha256:8c654938f08f63f36b4a04a16d299808ec14a7120048e3b23caab6cff4325378
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
$ docker pull ubuntu@sha256:266cbca633bcb1356b9be281efe251782d30830cee0c0cf6a3c952a3a655f040
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.9 MB (26945285 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3732473f881aa819c8754dc83b3bc7afc00361ea6090c135c72ccd38c9fd3637`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 28 Jun 2023 08:23:22 GMT
ARG RELEASE
# Wed, 28 Jun 2023 08:23:22 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 08:23:22 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 08:23:22 GMT
LABEL org.opencontainers.image.version=23.10
# Wed, 28 Jun 2023 08:23:24 GMT
ADD file:ce14b5aa15734922ec61b739c654f0d2843757c5f260778d4ecd9aa097cfacaf in / 
# Wed, 28 Jun 2023 08:23:24 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:4221febb096369c46cecc96ff4b3504b9ee19e25c6524e5da970ef0b30ee1b20`  
		Last Modified: Wed, 28 Jun 2023 09:26:34 GMT  
		Size: 26.9 MB (26945285 bytes)  
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
$ docker pull ubuntu@sha256:64ed81ed8782fb3323ae81aa60141d480787cd68b56fcd1a40be02b3be47d303
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.8 MB (25757906 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9ee8ecbb7ea7af1d7ed8af19d1e5b2614c0f5591cb25be48369e53b2122d5f76`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 28 Jun 2023 08:24:14 GMT
ARG RELEASE
# Wed, 28 Jun 2023 08:24:14 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 08:24:14 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 08:24:14 GMT
LABEL org.opencontainers.image.version=23.10
# Wed, 28 Jun 2023 08:24:16 GMT
ADD file:6046e0887f51e3cd521761c62077e42ceb11c3a32d6ecd6b0b32f7d9fbb83dec in / 
# Wed, 28 Jun 2023 08:24:16 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:da055310d6b309c0380a1d16ab6cd974a850123c5014f1e57d02df5852288ef5`  
		Last Modified: Wed, 28 Jun 2023 09:27:02 GMT  
		Size: 25.8 MB (25757906 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

## `ubuntu:focal`

```console
$ docker pull ubuntu@sha256:454eb772508cebb744a4561dd25d3ba52e110513e9d7916ab5c89224810a0d7f
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
$ docker pull ubuntu@sha256:8c38f4ea0b178a98e4f9f831b29b7966d6654414c1dc008591c6ec77de3bf2c9
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.5 MB (27505622 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:14be0685b7682b182af5b862c9638cb1cb4ca1a70bd5aa90deed96e9cca881e7`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 28 Jun 2023 09:59:08 GMT
ARG RELEASE
# Wed, 28 Jun 2023 09:59:08 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 09:59:08 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 09:59:08 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 28 Jun 2023 09:59:10 GMT
ADD file:12f97b7b044d0d1166dd59408c67f5610a764127aa8a01bc57db23bee48911af in / 
# Wed, 28 Jun 2023 09:59:10 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:01085d60b3a624c06a7132ff0749efc6e6565d9f2531d7685ff559fb5d0f669f`  
		Last Modified: Wed, 28 Jun 2023 10:13:37 GMT  
		Size: 27.5 MB (27505622 bytes)  
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
$ docker pull ubuntu@sha256:7fa3e1a7f357f2ee21918f3ad5eeab7a0d02a7452acdaecc47f585ed6e52d76a
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.4 MB (26350273 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:10bdc248f7d72bc0aa775d61bceae878a8443d11d651d172a28fa56644492df9`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 28 Jun 2023 10:01:13 GMT
ARG RELEASE
# Wed, 28 Jun 2023 10:01:13 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 10:01:13 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 10:01:14 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 28 Jun 2023 10:01:15 GMT
ADD file:777fd71e798b91bf768b21e1ca4403f388db9936ef55ef68b4b019cb167fa707 in / 
# Wed, 28 Jun 2023 10:01:15 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:0ebf1bc80a393479c293dfa52056fa26e7e3699214a6559bd7004f7c2d3c2832`  
		Last Modified: Wed, 28 Jun 2023 10:14:02 GMT  
		Size: 26.4 MB (26350273 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

## `ubuntu:focal-20230624`

```console
$ docker pull ubuntu@sha256:f412b626785f743d3de93f7bc9ed681d4e2bceb737c25cb466f27b5e096c97b6
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; s390x

### `ubuntu:focal-20230624` - linux; amd64

```console
$ docker pull ubuntu@sha256:8c38f4ea0b178a98e4f9f831b29b7966d6654414c1dc008591c6ec77de3bf2c9
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.5 MB (27505622 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:14be0685b7682b182af5b862c9638cb1cb4ca1a70bd5aa90deed96e9cca881e7`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 28 Jun 2023 09:59:08 GMT
ARG RELEASE
# Wed, 28 Jun 2023 09:59:08 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 09:59:08 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 09:59:08 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 28 Jun 2023 09:59:10 GMT
ADD file:12f97b7b044d0d1166dd59408c67f5610a764127aa8a01bc57db23bee48911af in / 
# Wed, 28 Jun 2023 09:59:10 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:01085d60b3a624c06a7132ff0749efc6e6565d9f2531d7685ff559fb5d0f669f`  
		Last Modified: Wed, 28 Jun 2023 10:13:37 GMT  
		Size: 27.5 MB (27505622 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:focal-20230624` - linux; s390x

```console
$ docker pull ubuntu@sha256:7fa3e1a7f357f2ee21918f3ad5eeab7a0d02a7452acdaecc47f585ed6e52d76a
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.4 MB (26350273 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:10bdc248f7d72bc0aa775d61bceae878a8443d11d651d172a28fa56644492df9`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 28 Jun 2023 10:01:13 GMT
ARG RELEASE
# Wed, 28 Jun 2023 10:01:13 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 10:01:13 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 10:01:14 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 28 Jun 2023 10:01:15 GMT
ADD file:777fd71e798b91bf768b21e1ca4403f388db9936ef55ef68b4b019cb167fa707 in / 
# Wed, 28 Jun 2023 10:01:15 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:0ebf1bc80a393479c293dfa52056fa26e7e3699214a6559bd7004f7c2d3c2832`  
		Last Modified: Wed, 28 Jun 2023 10:14:02 GMT  
		Size: 26.4 MB (26350273 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

## `ubuntu:jammy`

```console
$ docker pull ubuntu@sha256:1a8c20aeeed491d5aa4ab85946adefeecb90ec10bfd7a316fe3b632e3a917674
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
$ docker pull ubuntu@sha256:b060fffe8e1561c9c3e6dea6db487b900100fc26830b9ea2ec966c151ab4c020
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.5 MB (29533422 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5a81c4b8502e4979e75bd8f91343b95b0d695ab67f241dbed0d1530a35bde1eb`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 28 Jun 2023 08:37:40 GMT
ARG RELEASE
# Wed, 28 Jun 2023 08:37:40 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 08:37:40 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 08:37:40 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 28 Jun 2023 08:37:42 GMT
ADD file:140fb5108b4a2861b5718ad03b4a5174bba03589ea8d4c053e6a0b282f439ff3 in / 
# Wed, 28 Jun 2023 08:37:42 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:3153aa388d026c26a2235e1ed0163e350e451f41a8a313e1804d7e1afb857ab4`  
		Last Modified: Wed, 28 Jun 2023 08:58:40 GMT  
		Size: 29.5 MB (29533422 bytes)  
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
$ docker pull ubuntu@sha256:107cc410d683e41f2765125ec3b3aba514025348590539fcc079fa02d54f5708
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.0 MB (28016094 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ab733017eab481028e4f46a149cba2e422b2bc0c15a07c9bd29e7d431b568546`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 28 Jun 2023 08:53:20 GMT
ARG RELEASE
# Wed, 28 Jun 2023 08:53:20 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 08:53:20 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 08:53:20 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 28 Jun 2023 08:53:22 GMT
ADD file:fa0aef35be7808c8fd6751a52bdec4dd81057e2fcaa075c547a1db53640dae9a in / 
# Wed, 28 Jun 2023 08:53:22 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:ccff9014dcde158442f3978d42c5311f5833a9a4200b72f93a87ca7f7542c39a`  
		Last Modified: Wed, 28 Jun 2023 08:59:07 GMT  
		Size: 28.0 MB (28016094 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

## `ubuntu:jammy-20230624`

```console
$ docker pull ubuntu@sha256:c8f0570d33074ad254b02d0ca80eb28c7787881f96526c1feb35a8b81bdcdd90
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; s390x

### `ubuntu:jammy-20230624` - linux; amd64

```console
$ docker pull ubuntu@sha256:b060fffe8e1561c9c3e6dea6db487b900100fc26830b9ea2ec966c151ab4c020
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.5 MB (29533422 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5a81c4b8502e4979e75bd8f91343b95b0d695ab67f241dbed0d1530a35bde1eb`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 28 Jun 2023 08:37:40 GMT
ARG RELEASE
# Wed, 28 Jun 2023 08:37:40 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 08:37:40 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 08:37:40 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 28 Jun 2023 08:37:42 GMT
ADD file:140fb5108b4a2861b5718ad03b4a5174bba03589ea8d4c053e6a0b282f439ff3 in / 
# Wed, 28 Jun 2023 08:37:42 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:3153aa388d026c26a2235e1ed0163e350e451f41a8a313e1804d7e1afb857ab4`  
		Last Modified: Wed, 28 Jun 2023 08:58:40 GMT  
		Size: 29.5 MB (29533422 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:jammy-20230624` - linux; s390x

```console
$ docker pull ubuntu@sha256:107cc410d683e41f2765125ec3b3aba514025348590539fcc079fa02d54f5708
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.0 MB (28016094 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ab733017eab481028e4f46a149cba2e422b2bc0c15a07c9bd29e7d431b568546`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 28 Jun 2023 08:53:20 GMT
ARG RELEASE
# Wed, 28 Jun 2023 08:53:20 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 08:53:20 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 08:53:20 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 28 Jun 2023 08:53:22 GMT
ADD file:fa0aef35be7808c8fd6751a52bdec4dd81057e2fcaa075c547a1db53640dae9a in / 
# Wed, 28 Jun 2023 08:53:22 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:ccff9014dcde158442f3978d42c5311f5833a9a4200b72f93a87ca7f7542c39a`  
		Last Modified: Wed, 28 Jun 2023 08:59:07 GMT  
		Size: 28.0 MB (28016094 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

## `ubuntu:kinetic`

```console
$ docker pull ubuntu@sha256:534d1acc4da51c47b477ec1a764bc5ed3c007bec93ee08d832538077cd0bdeaa
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
$ docker pull ubuntu@sha256:d36481db487c935436420cc4b705db8c81eec3872085ebd27963b775695fbe24
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.7 MB (26704806 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:692eb4a905c074054e0a35d647671f0e32ed150d15b23fd7bc745cfb2fdeddbd`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 28 Jun 2023 08:23:07 GMT
ARG RELEASE
# Wed, 28 Jun 2023 08:23:07 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 08:23:07 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 08:23:07 GMT
LABEL org.opencontainers.image.version=22.10
# Wed, 28 Jun 2023 08:23:09 GMT
ADD file:50094673f74cf3945ac21e23bb84d41d3516bc1ac90ebf7f17379288c33c17b2 in / 
# Wed, 28 Jun 2023 08:23:09 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:3ad6ea492c35ef48892b4587449510d372516d5969073eeaa6601a380e861c57`  
		Last Modified: Wed, 28 Jun 2023 09:32:54 GMT  
		Size: 26.7 MB (26704806 bytes)  
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
$ docker pull ubuntu@sha256:0e44a443176bc6ca4e93ac2e465db208c43934238f410f378dc3c998eee696b5
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.5 MB (25490150 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:94aa2bec78551a9bd8a92d09f4fe0504cbd6f72a3ebaf9820bbcb93897b2aed1`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 28 Jun 2023 08:31:17 GMT
ARG RELEASE
# Wed, 28 Jun 2023 08:31:17 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 08:31:17 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 08:31:17 GMT
LABEL org.opencontainers.image.version=22.10
# Wed, 28 Jun 2023 08:31:19 GMT
ADD file:e6e44f70accdecf50c8942a8e70c4d2c1d419d1d61696730d8aeda653da7216b in / 
# Wed, 28 Jun 2023 08:31:20 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:7dfef942861c66b1cea3ce2cc82694e398544893132321d00bace936daa2c360`  
		Last Modified: Wed, 28 Jun 2023 09:33:20 GMT  
		Size: 25.5 MB (25490150 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

## `ubuntu:kinetic-20230624`

```console
$ docker pull ubuntu@sha256:9b2fc620193db3ae5c7a214cc12f031f22359d2690597c5c371fd5d64382b859
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; s390x

### `ubuntu:kinetic-20230624` - linux; amd64

```console
$ docker pull ubuntu@sha256:d36481db487c935436420cc4b705db8c81eec3872085ebd27963b775695fbe24
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.7 MB (26704806 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:692eb4a905c074054e0a35d647671f0e32ed150d15b23fd7bc745cfb2fdeddbd`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 28 Jun 2023 08:23:07 GMT
ARG RELEASE
# Wed, 28 Jun 2023 08:23:07 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 08:23:07 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 08:23:07 GMT
LABEL org.opencontainers.image.version=22.10
# Wed, 28 Jun 2023 08:23:09 GMT
ADD file:50094673f74cf3945ac21e23bb84d41d3516bc1ac90ebf7f17379288c33c17b2 in / 
# Wed, 28 Jun 2023 08:23:09 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:3ad6ea492c35ef48892b4587449510d372516d5969073eeaa6601a380e861c57`  
		Last Modified: Wed, 28 Jun 2023 09:32:54 GMT  
		Size: 26.7 MB (26704806 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:kinetic-20230624` - linux; s390x

```console
$ docker pull ubuntu@sha256:0e44a443176bc6ca4e93ac2e465db208c43934238f410f378dc3c998eee696b5
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.5 MB (25490150 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:94aa2bec78551a9bd8a92d09f4fe0504cbd6f72a3ebaf9820bbcb93897b2aed1`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 28 Jun 2023 08:31:17 GMT
ARG RELEASE
# Wed, 28 Jun 2023 08:31:17 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 08:31:17 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 08:31:17 GMT
LABEL org.opencontainers.image.version=22.10
# Wed, 28 Jun 2023 08:31:19 GMT
ADD file:e6e44f70accdecf50c8942a8e70c4d2c1d419d1d61696730d8aeda653da7216b in / 
# Wed, 28 Jun 2023 08:31:20 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:7dfef942861c66b1cea3ce2cc82694e398544893132321d00bace936daa2c360`  
		Last Modified: Wed, 28 Jun 2023 09:33:20 GMT  
		Size: 25.5 MB (25490150 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

## `ubuntu:latest`

```console
$ docker pull ubuntu@sha256:1a8c20aeeed491d5aa4ab85946adefeecb90ec10bfd7a316fe3b632e3a917674
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
$ docker pull ubuntu@sha256:b060fffe8e1561c9c3e6dea6db487b900100fc26830b9ea2ec966c151ab4c020
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.5 MB (29533422 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5a81c4b8502e4979e75bd8f91343b95b0d695ab67f241dbed0d1530a35bde1eb`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 28 Jun 2023 08:37:40 GMT
ARG RELEASE
# Wed, 28 Jun 2023 08:37:40 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 08:37:40 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 08:37:40 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 28 Jun 2023 08:37:42 GMT
ADD file:140fb5108b4a2861b5718ad03b4a5174bba03589ea8d4c053e6a0b282f439ff3 in / 
# Wed, 28 Jun 2023 08:37:42 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:3153aa388d026c26a2235e1ed0163e350e451f41a8a313e1804d7e1afb857ab4`  
		Last Modified: Wed, 28 Jun 2023 08:58:40 GMT  
		Size: 29.5 MB (29533422 bytes)  
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
$ docker pull ubuntu@sha256:107cc410d683e41f2765125ec3b3aba514025348590539fcc079fa02d54f5708
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.0 MB (28016094 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ab733017eab481028e4f46a149cba2e422b2bc0c15a07c9bd29e7d431b568546`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 28 Jun 2023 08:53:20 GMT
ARG RELEASE
# Wed, 28 Jun 2023 08:53:20 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 08:53:20 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 08:53:20 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 28 Jun 2023 08:53:22 GMT
ADD file:fa0aef35be7808c8fd6751a52bdec4dd81057e2fcaa075c547a1db53640dae9a in / 
# Wed, 28 Jun 2023 08:53:22 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:ccff9014dcde158442f3978d42c5311f5833a9a4200b72f93a87ca7f7542c39a`  
		Last Modified: Wed, 28 Jun 2023 08:59:07 GMT  
		Size: 28.0 MB (28016094 bytes)  
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
$ docker pull ubuntu@sha256:8c654938f08f63f36b4a04a16d299808ec14a7120048e3b23caab6cff4325378
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
$ docker pull ubuntu@sha256:266cbca633bcb1356b9be281efe251782d30830cee0c0cf6a3c952a3a655f040
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.9 MB (26945285 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3732473f881aa819c8754dc83b3bc7afc00361ea6090c135c72ccd38c9fd3637`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 28 Jun 2023 08:23:22 GMT
ARG RELEASE
# Wed, 28 Jun 2023 08:23:22 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 08:23:22 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 08:23:22 GMT
LABEL org.opencontainers.image.version=23.10
# Wed, 28 Jun 2023 08:23:24 GMT
ADD file:ce14b5aa15734922ec61b739c654f0d2843757c5f260778d4ecd9aa097cfacaf in / 
# Wed, 28 Jun 2023 08:23:24 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:4221febb096369c46cecc96ff4b3504b9ee19e25c6524e5da970ef0b30ee1b20`  
		Last Modified: Wed, 28 Jun 2023 09:26:34 GMT  
		Size: 26.9 MB (26945285 bytes)  
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
$ docker pull ubuntu@sha256:64ed81ed8782fb3323ae81aa60141d480787cd68b56fcd1a40be02b3be47d303
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.8 MB (25757906 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9ee8ecbb7ea7af1d7ed8af19d1e5b2614c0f5591cb25be48369e53b2122d5f76`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 28 Jun 2023 08:24:14 GMT
ARG RELEASE
# Wed, 28 Jun 2023 08:24:14 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 08:24:14 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 08:24:14 GMT
LABEL org.opencontainers.image.version=23.10
# Wed, 28 Jun 2023 08:24:16 GMT
ADD file:6046e0887f51e3cd521761c62077e42ceb11c3a32d6ecd6b0b32f7d9fbb83dec in / 
# Wed, 28 Jun 2023 08:24:16 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:da055310d6b309c0380a1d16ab6cd974a850123c5014f1e57d02df5852288ef5`  
		Last Modified: Wed, 28 Jun 2023 09:27:02 GMT  
		Size: 25.8 MB (25757906 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

## `ubuntu:mantic-20230624`

```console
$ docker pull ubuntu@sha256:bfa292484f53a1a4ec390f95367da38e79ebd5f6058439b1e9ff4f5dec59d4ea
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; s390x

### `ubuntu:mantic-20230624` - linux; amd64

```console
$ docker pull ubuntu@sha256:266cbca633bcb1356b9be281efe251782d30830cee0c0cf6a3c952a3a655f040
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.9 MB (26945285 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3732473f881aa819c8754dc83b3bc7afc00361ea6090c135c72ccd38c9fd3637`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 28 Jun 2023 08:23:22 GMT
ARG RELEASE
# Wed, 28 Jun 2023 08:23:22 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 08:23:22 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 08:23:22 GMT
LABEL org.opencontainers.image.version=23.10
# Wed, 28 Jun 2023 08:23:24 GMT
ADD file:ce14b5aa15734922ec61b739c654f0d2843757c5f260778d4ecd9aa097cfacaf in / 
# Wed, 28 Jun 2023 08:23:24 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:4221febb096369c46cecc96ff4b3504b9ee19e25c6524e5da970ef0b30ee1b20`  
		Last Modified: Wed, 28 Jun 2023 09:26:34 GMT  
		Size: 26.9 MB (26945285 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `ubuntu:mantic-20230624` - linux; s390x

```console
$ docker pull ubuntu@sha256:64ed81ed8782fb3323ae81aa60141d480787cd68b56fcd1a40be02b3be47d303
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.8 MB (25757906 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9ee8ecbb7ea7af1d7ed8af19d1e5b2614c0f5591cb25be48369e53b2122d5f76`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 28 Jun 2023 08:24:14 GMT
ARG RELEASE
# Wed, 28 Jun 2023 08:24:14 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 08:24:14 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 08:24:14 GMT
LABEL org.opencontainers.image.version=23.10
# Wed, 28 Jun 2023 08:24:16 GMT
ADD file:6046e0887f51e3cd521761c62077e42ceb11c3a32d6ecd6b0b32f7d9fbb83dec in / 
# Wed, 28 Jun 2023 08:24:16 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:da055310d6b309c0380a1d16ab6cd974a850123c5014f1e57d02df5852288ef5`  
		Last Modified: Wed, 28 Jun 2023 09:27:02 GMT  
		Size: 25.8 MB (25757906 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

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
