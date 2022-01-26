## `debian:bullseye-backports`

```console
$ docker pull debian@sha256:39a600e6d77ea86b379747901d689d144dd64826174e8e8c8fee3cdedcc59841
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

### `debian:bullseye-backports` - linux; amd64

```console
$ docker pull debian@sha256:52851e377d74044076d8f835375eee817e5e0ffd14d87ede8faae5856a841cfe
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **54.9 MB (54917391 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:353cb88564769e67e9390665c2d42cdb3257b917dc1c68fa7277269443dfeade`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Jan 2022 01:40:22 GMT
ADD file:9cca7f8e4abcd8309501cad216ff33a28932386ded66461a7591c0fdf2c859d3 in / 
# Wed, 26 Jan 2022 01:40:23 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 01:40:27 GMT
RUN echo 'deb http://deb.debian.org/debian bullseye-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:0c6b8ff8c37e92eb1ca65ed8917e818927d5bf318b6f18896049b5d9afc28343`  
		Last Modified: Wed, 26 Jan 2022 01:46:07 GMT  
		Size: 54.9 MB (54917164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:452729c62016c6793fe44dbc7adb35693d4e1cbe12b4f587247fa15cc7018b21`  
		Last Modified: Wed, 26 Jan 2022 01:46:27 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:bullseye-backports` - linux; arm variant v5

```console
$ docker pull debian@sha256:50dd5700f5e7adf8ae19a1900017c18a17546b2b83e3414f191a3defe6cc4053
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.5 MB (52466826 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f50e92c64b9a4ed92f690fa877c2c6c5088a85949d5b038ef349b24c5e101b1f`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Jan 2022 01:41:21 GMT
ADD file:5c238170d9d1bd220e05ede3d517d33fadd813f341546cfd0f2a29285092ac05 in / 
# Wed, 26 Jan 2022 01:41:23 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 01:41:39 GMT
RUN echo 'deb http://deb.debian.org/debian bullseye-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:d09eefb6f859064403eeef43dadb425a65a1b745075123e6770f3131f93d2679`  
		Last Modified: Wed, 26 Jan 2022 01:56:45 GMT  
		Size: 52.5 MB (52466598 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f190fc8fba6eef5796fc7a43adf8028bd27f9040a101dafeccf97166df08d60b`  
		Last Modified: Wed, 26 Jan 2022 01:57:09 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:bullseye-backports` - linux; arm variant v7

```console
$ docker pull debian@sha256:39294d6a8bde970dced08e152e9e8f648ce4494d26cca4efff145f4268efe2be
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.1 MB (50117586 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ef3690d9d78b0f53ca6d814d06ab5166cb80a4b58c51a26aa97342559d839038`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Jan 2022 01:41:30 GMT
ADD file:19419917274a4a5aa3eceb0a6202f89e5b508368314f2bd0105897a847db4930 in / 
# Wed, 26 Jan 2022 01:41:31 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 01:41:48 GMT
RUN echo 'deb http://deb.debian.org/debian bullseye-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:046501ac4c58f014cc320324f6023bbef17f28025428833449198a62a97849c0`  
		Last Modified: Wed, 26 Jan 2022 01:57:13 GMT  
		Size: 50.1 MB (50117358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6a98239125b9743a7563922abfce6b0c2c9830a20ba2f1280d49f79c580dcc1`  
		Last Modified: Wed, 26 Jan 2022 01:57:37 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:bullseye-backports` - linux; arm64 variant v8

```console
$ docker pull debian@sha256:41ee3f99b5182e47eec9ddb49b2bbbc08b8bd9d040845c8cd9832ed58a511f70
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.6 MB (53609075 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5cbcc2b8b5c3aed7c98e1d53109cf586277547778558709555ebf1b8c83f55d0`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Jan 2022 01:42:15 GMT
ADD file:b6338a9c3c2f8d7ba1a23dcb7a1389c7d0eab75a7489ef66f21c773be56aa9ed in / 
# Wed, 26 Jan 2022 01:42:16 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 01:42:24 GMT
RUN echo 'deb http://deb.debian.org/debian bullseye-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:39ab78bc09e79a21f719ced771689354d1948f4afd57e86afed8dac6ffb47826`  
		Last Modified: Wed, 26 Jan 2022 01:48:34 GMT  
		Size: 53.6 MB (53608848 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c549354d26a4e6df7c1a697edb45cf072a3e4ee70b7fb7cacf3660e44721b8e`  
		Last Modified: Wed, 26 Jan 2022 01:48:52 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:bullseye-backports` - linux; 386

```console
$ docker pull debian@sha256:97104194839afd5297dfdf0e06f875238c06b581efd2ef6a2f6265e8697b0a3e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **55.9 MB (55939238 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9bbe61e543b09f5f3d8eea30394d5f097cace1ef359719d0ef65d75ebac702c1`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Jan 2022 01:39:35 GMT
ADD file:dfb883d877f16913b7019d7b3bb938890bfa288a712901baeac6e1c7403911e2 in / 
# Wed, 26 Jan 2022 01:39:36 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 01:39:44 GMT
RUN echo 'deb http://deb.debian.org/debian bullseye-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:12e30620442951468b6e2349dbcb6a8a35c39b59f1cf8096f7b5eaf7ba0ec5c9`  
		Last Modified: Wed, 26 Jan 2022 01:48:19 GMT  
		Size: 55.9 MB (55939009 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53a7e72362013a374c6e5107387fa3f139acf9fe8853adf0912a4744e94d2350`  
		Last Modified: Wed, 26 Jan 2022 01:48:42 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:bullseye-backports` - linux; mips64le

```console
$ docker pull debian@sha256:d664716fda1f416764d19229bfa9b10ff31b7ba9b06bcc7ee2d744f6386dafd9
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.2 MB (53180193 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4d981f0355f4fb8993eaf5af4cf19984383b558043c3046f96378312ced6ce56`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Jan 2022 01:42:19 GMT
ADD file:06fbff49d105bbaefb6199ecf549660a67db6cec16698f03c8ae0cf2bdfd6d4f in / 
# Wed, 26 Jan 2022 01:42:20 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 01:42:26 GMT
RUN echo 'deb http://deb.debian.org/debian bullseye-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:6176f4ee4b1d3ab7c5f3f93bc9036b71aa337a53c743b4aa347dffebfc8c772a`  
		Last Modified: Wed, 26 Jan 2022 01:50:39 GMT  
		Size: 53.2 MB (53179965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68a9dbda7e6c794dd9354514ad60ee78bd4cbdd93d719777ea44a9f90b4d0c7e`  
		Last Modified: Wed, 26 Jan 2022 01:50:56 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:bullseye-backports` - linux; ppc64le

```console
$ docker pull debian@sha256:1157a1a0cdc3cd022b2de68eb187ed24b5dcbe32ebe28a8ddbb50fca9d9e8400
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **58.8 MB (58833771 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b69564b9aacbed74628281b1606f6ca223676fe6e6ab4585f75dce23886e36aa`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Jan 2022 01:46:12 GMT
ADD file:2cbda28d396a0fa4e6d85b7b6157b40a40e4cd783fb7e2182bfbe03c1ba23943 in / 
# Wed, 26 Jan 2022 01:46:19 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 01:46:39 GMT
RUN echo 'deb http://deb.debian.org/debian bullseye-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:9ecf2845789585f183c7b423fece4a8a51e9f5753452de12292282be543e2500`  
		Last Modified: Wed, 26 Jan 2022 01:56:06 GMT  
		Size: 58.8 MB (58833543 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aaef3a1aeac9570359b7adc8781f9835ad6ee2293f11821016903457160edfdc`  
		Last Modified: Wed, 26 Jan 2022 01:56:27 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:bullseye-backports` - linux; s390x

```console
$ docker pull debian@sha256:75a3d65f1e367c354bfe3996d5bdc9c4ca5b616f591c26b63656e9b421c06c8a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.2 MB (53210633 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5485cab96573c18b5ad25c94b2bc01c6378b915b4b39c490ec1f28b1389ff955`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Jan 2022 01:40:54 GMT
ADD file:0ff9360660b63a458b2c33e09a38fd9413847541680cd01bd4dc78cb14dd0f92 in / 
# Wed, 26 Jan 2022 01:40:57 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 01:41:05 GMT
RUN echo 'deb http://deb.debian.org/debian bullseye-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:19a0c65e73a647e498e4b74e1ce53ad5b58d75b2e52e2c30058143495b1148d5`  
		Last Modified: Wed, 26 Jan 2022 01:46:36 GMT  
		Size: 53.2 MB (53210407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce0dfca83e93fca82fbb6d3803d4bdc2f372468c0ab9df7992e997c51377cd5c`  
		Last Modified: Wed, 26 Jan 2022 01:46:48 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
