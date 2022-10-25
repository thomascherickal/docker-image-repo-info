## `debian:bookworm-backports`

```console
$ docker pull debian@sha256:1fd971ca3c2e2ac7715c88ea53ab6da6cffa3d5323a58b26e8d87a7fc61f8067
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

### `debian:bookworm-backports` - linux; amd64

```console
$ docker pull debian@sha256:f3ac43095dc15e59d7f57b201b66ef2c496386bb1e4ceed8bb86bb05aee17d01
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.3 MB (51262007 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:53da2ee1ffaec303e7fb884f50d27bbd585c234aad69c57d34e28c8a3f3c39eb`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 01:43:22 GMT
ADD file:3b158c11a921c91aa3cebf5651e59c21fe59da295d3edc56147fefaa760329ff in / 
# Tue, 25 Oct 2022 01:43:23 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 01:43:26 GMT
RUN echo 'deb http://deb.debian.org/debian bookworm-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:3721e3e259583b8b78cfdeb51a553c189938925b902bceaa1f4f92e837fb9a23`  
		Last Modified: Tue, 25 Oct 2022 01:46:52 GMT  
		Size: 51.3 MB (51261783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85aa58c44af92ec3fdeaafb16bc38ebd1b2b94a81f22e0176d091f9d4692a1d4`  
		Last Modified: Tue, 25 Oct 2022 01:47:01 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:bookworm-backports` - linux; arm variant v5

```console
$ docker pull debian@sha256:440fe41ea218b42edf5616f33785d97407c110c756601d4f024f078c20e543bd
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.8 MB (51838883 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:49d884e26c94a763862576f54af80a346ddd8227db008ba743046395afaa159e`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:48:31 GMT
ADD file:2f3df348b6a9200fcbcfe13a10334cef72dca5f19d7ed73055f7a03ff08122f7 in / 
# Tue, 04 Oct 2022 23:48:31 GMT
CMD ["bash"]
# Tue, 04 Oct 2022 23:48:37 GMT
RUN echo 'deb http://deb.debian.org/debian bookworm-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:2843f1fd91937d710e0d158046e9c23fe034f11c8c934a478f443b561be758dc`  
		Last Modified: Tue, 04 Oct 2022 23:52:36 GMT  
		Size: 51.8 MB (51838659 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d8811c053a8622e7f4865655d44802aada27fdce3432a59123a6371ade0510d`  
		Last Modified: Tue, 04 Oct 2022 23:52:47 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:bookworm-backports` - linux; arm variant v7

```console
$ docker pull debian@sha256:692ad8641e8b5043bb613e0e59d02a4c787f0b0218e37ef940ff5bc4a629d552
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.7 MB (49692834 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:455416a3fa0912d05403f102ccd266be86ab862fdeed4c259000a815764c974d`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:57:54 GMT
ADD file:9f3a74b8856c0affe36dd4e0700a8a2686a9d2275934fd9af95135f13731d10e in / 
# Tue, 04 Oct 2022 23:57:54 GMT
CMD ["bash"]
# Tue, 04 Oct 2022 23:58:02 GMT
RUN echo 'deb http://deb.debian.org/debian bookworm-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:b2ee1685df1bf13149eece9e0085c6befe355f21deeea69484a3ab1fab51e40c`  
		Last Modified: Wed, 05 Oct 2022 00:03:53 GMT  
		Size: 49.7 MB (49692608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79f6bf3438e5c933dd7c682b2c006fdf41767a4cd9f81ce697265171f8f02038`  
		Last Modified: Wed, 05 Oct 2022 00:04:05 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:bookworm-backports` - linux; arm64 variant v8

```console
$ docker pull debian@sha256:de7edda3869da606bef00abf3e698b8b7c74b963910ec8cd4382b44514b66eb0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.0 MB (52980614 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bd5e0a2e6106379cee018cd6be71b75d67d9ed1c1d623c96262fb30e004f4a0a`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:44:00 GMT
ADD file:269c8bec4871d84b9133706a2f391209619d53c0bfa56121c740757cf5798fcb in / 
# Tue, 04 Oct 2022 23:44:02 GMT
CMD ["bash"]
# Tue, 04 Oct 2022 23:44:08 GMT
RUN echo 'deb http://deb.debian.org/debian bookworm-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:2debf9e7f23054c81a936da9b01c5db9f72a55d4810f7bf0e5641bd1748d90b7`  
		Last Modified: Tue, 04 Oct 2022 23:49:11 GMT  
		Size: 53.0 MB (52980389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a707182dfba1c22a9f7523d22112a259d318c0b9d2153746676c30d25446001a`  
		Last Modified: Tue, 04 Oct 2022 23:49:21 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:bookworm-backports` - linux; 386

```console
$ docker pull debian@sha256:89e7ff0044cc1d2cd3ab3972a297c1f0498926143eee31691b6f670f576f6e4c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.9 MB (53933056 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6cebac71e96f66089c5bf7ec99f01e3c9136c824f303469e0ca2c05aad5e269f`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:38:57 GMT
ADD file:2a0c743e373aeed6462c2f3ae8a138fb0e240e935ad7ca5bf008aa3efd3673a0 in / 
# Tue, 04 Oct 2022 23:38:58 GMT
CMD ["bash"]
# Tue, 04 Oct 2022 23:39:03 GMT
RUN echo 'deb http://deb.debian.org/debian bookworm-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:c68776dad61a299b8e65d1a6a02e376b8ed2e9b241bd753bf6c35d497055ecdf`  
		Last Modified: Tue, 04 Oct 2022 23:44:23 GMT  
		Size: 53.9 MB (53932827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5dc077cefcd731a5201ab62c2cf0fb92a680fcaa05be88acc276a9898b4768cd`  
		Last Modified: Tue, 04 Oct 2022 23:44:34 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:bookworm-backports` - linux; mips64le

```console
$ docker pull debian@sha256:fbfad4f28c4ea1940fdb6b5b092ebf526b8655b54e547068889f2a9319a3d775
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.0 MB (52967207 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3beac4f6dca37fa9443f60e038675677814e36dc06f9152680c45498e1ad25c6`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 05 Oct 2022 00:08:36 GMT
ADD file:f17f2d6b2018174ed9b628a69ee630ae6e011a3022bb5a0f3196ef9009d39270 in / 
# Wed, 05 Oct 2022 00:08:41 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 00:08:51 GMT
RUN echo 'deb http://deb.debian.org/debian bookworm-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:17006ab86ecbcadb62dabb0d565c7783b28660c51cccb5d7b46f01518a3753a3`  
		Last Modified: Wed, 05 Oct 2022 00:16:34 GMT  
		Size: 53.0 MB (52966979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:954c8e9a9d89fe2b5fa8e5f96010ed0e1a95fefb2abd3c73942e8587f3d78c9d`  
		Last Modified: Wed, 05 Oct 2022 00:16:44 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:bookworm-backports` - linux; ppc64le

```console
$ docker pull debian@sha256:f84642da24d9d5055b3b872828bfe4e25c01ab447781c243fd6a9532d1132e9c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **57.1 MB (57111791 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8f607bd18a190160cf3b9cb1cf8c8db6a41f686d95825cbcea37e4236825417c`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:16:56 GMT
ADD file:22dddefde9f3e8eff6049751a459a3c4fdade46622016ce6269b630157170962 in / 
# Tue, 04 Oct 2022 23:16:59 GMT
CMD ["bash"]
# Tue, 04 Oct 2022 23:17:06 GMT
RUN echo 'deb http://deb.debian.org/debian bookworm-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:8fd653dd210d0ff49ceb9b32e662a564ab01445265e165edd4f963c3953f5b33`  
		Last Modified: Tue, 04 Oct 2022 23:22:42 GMT  
		Size: 57.1 MB (57111564 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13c8ea4263e850fb3bea5dbd2615e11bbd7a1bfc883506e18a41e169a15deab3`  
		Last Modified: Tue, 04 Oct 2022 23:22:53 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:bookworm-backports` - linux; s390x

```console
$ docker pull debian@sha256:46f681f24aec1a69ea11dd21ef7e0c45d84809ae3a593ee67a51069f9ba7c57a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.6 MB (49578725 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:39feb8386d979253006a1b6d4e549b75b5ea104752015308b5edadd309713bf4`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 01:13:56 GMT
ADD file:92a462945d4b32c30f41478992b9ab30d452ac37b0ecef64e2325e4e99296ea8 in / 
# Tue, 25 Oct 2022 01:13:58 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 01:14:05 GMT
RUN echo 'deb http://deb.debian.org/debian bookworm-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:e544dc28605cf962b36f5ba4703f824c022460d64f8973e49764cd76163df5ff`  
		Last Modified: Tue, 25 Oct 2022 01:18:08 GMT  
		Size: 49.6 MB (49578501 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2496bacf19fbe6379edbe13aeda89ecfc123f3050d0c3650cf9458cb456b1293`  
		Last Modified: Tue, 25 Oct 2022 01:18:15 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
