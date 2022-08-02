## `debian:oldstable-backports`

```console
$ docker pull debian@sha256:981495d838bc0709f13b2d6ae3f3698308b55a03243e3c751273333b160cf622
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

### `debian:oldstable-backports` - linux; amd64

```console
$ docker pull debian@sha256:55ab92f0f1735350338cf241844fdc91ab428290dad7929d943cfae230c11249
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.4 MB (50441222 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:03052234fa732195ad46613fc0676163c53741ce816be4dea6a48b8f9bbc829c`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 Aug 2022 01:20:33 GMT
ADD file:8fd759ee86eb9935e660985c00224e524e80f1fea7f499c01fd916744976140a in / 
# Tue, 02 Aug 2022 01:20:33 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 01:20:37 GMT
RUN echo 'deb http://deb.debian.org/debian oldstable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:981a03e5262de0892c65849de7bda6cfebabff421ab858bc67caf577ae2b575a`  
		Last Modified: Tue, 02 Aug 2022 01:25:21 GMT  
		Size: 50.4 MB (50440998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0a226fc24f9b1b37a55280894cfcdad1ae17ff5630e419f0a1103e70b72ef86`  
		Last Modified: Tue, 02 Aug 2022 01:25:31 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:oldstable-backports` - linux; arm variant v5

```console
$ docker pull debian@sha256:6839afa26bea48456a37e821074405867538af8358d0fd7f43c8985be88ec9a3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.2 MB (48161139 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cd03779f946bd550ff6dd809ca571af2373fd534d1d6f4c0d983efc48507e272`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 Aug 2022 00:49:52 GMT
ADD file:371b25ef65fd230da412f50fcb06d520927632bb96a07076d77d2a82001f5480 in / 
# Tue, 02 Aug 2022 00:49:53 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 00:49:58 GMT
RUN echo 'deb http://deb.debian.org/debian oldstable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:52d72b38899d2d45fc4ce778a949bbd531070c4248dc1f9750841a7d017be79d`  
		Last Modified: Tue, 02 Aug 2022 00:57:39 GMT  
		Size: 48.2 MB (48160914 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1635ab47f99552d7ced90b9f545427eeb5456fa0f31d25afc29ebd86ab8fbca2`  
		Last Modified: Tue, 02 Aug 2022 00:57:50 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:oldstable-backports` - linux; arm variant v7

```console
$ docker pull debian@sha256:5ce49d564bde2080f30b4597aed9f4babb19a0032088ad07aa57ca425f57f2b7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.9 MB (45916054 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d040121335d12c6bc1a6d99aef448e44dd56837e2e7645099c33db9b6987ffd7`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 Aug 2022 01:00:03 GMT
ADD file:48f605475438bf0b8deab56ae6fc53da6e75a92b21d8296876fe739ae1f303ce in / 
# Tue, 02 Aug 2022 01:00:03 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 01:00:10 GMT
RUN echo 'deb http://deb.debian.org/debian oldstable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:8a918af2085b17a0ecf8fbcec83b3852f8a05e6224faa0cb548c2412994b3bed`  
		Last Modified: Tue, 02 Aug 2022 01:08:15 GMT  
		Size: 45.9 MB (45915828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a2e64cfdd5f8fd4bc07c96f1c8eb78b99348205c1d8d90c883e62b599d3ddc7`  
		Last Modified: Tue, 02 Aug 2022 01:08:27 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:oldstable-backports` - linux; arm64 variant v8

```console
$ docker pull debian@sha256:dac17d7c13b6b6808c7e2f83343a2c02b3b6d8b40e12624823bc252ee3327923
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.2 MB (49229271 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d5a63171844d5662d3652760d26651e965544d459b61660e4bfcbfe4cff37720`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 Aug 2022 00:41:14 GMT
ADD file:b91f60d57948d67bc2971c4580d040b317d99d49817693ce287b8693969ebd31 in / 
# Tue, 02 Aug 2022 00:41:15 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 00:41:21 GMT
RUN echo 'deb http://deb.debian.org/debian oldstable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:99a39853f3afc8d4418fee49977675d2e19b1e66220c37c26ced6d0067277b46`  
		Last Modified: Tue, 02 Aug 2022 00:47:19 GMT  
		Size: 49.2 MB (49229047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f8a1c457a33dca69b1a791f729c4726b241831b1858770b47f6032f4041e2d9`  
		Last Modified: Tue, 02 Aug 2022 00:47:30 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:oldstable-backports` - linux; 386

```console
$ docker pull debian@sha256:1e0b9619f4b647a0d15740689bc12c79b36987bfaa966f1d409098f1478040dd
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.2 MB (51204502 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1b8ebebddb915020c9a237c5b67454613797a81b609631ff1c3692b69ae4dfeb`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 Aug 2022 00:39:58 GMT
ADD file:b8e12261a22f8571c7147f6c022dce8169487d1b35567042cf1abbb763838031 in / 
# Tue, 02 Aug 2022 00:39:59 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 00:40:05 GMT
RUN echo 'deb http://deb.debian.org/debian oldstable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:36f4f30c7baac798cef0027e1ae19534a4afcf1b861196029bedd806ae22191b`  
		Last Modified: Tue, 02 Aug 2022 00:46:37 GMT  
		Size: 51.2 MB (51204276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0dd42540b88ebe8a6214a4a613dc0b59efd12af0e10594ee14e5115500b7555c`  
		Last Modified: Tue, 02 Aug 2022 00:46:48 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:oldstable-backports` - linux; mips64le

```console
$ docker pull debian@sha256:47e0bea86407a51cef26a446e9c505e728d29e4ca43cbd6a97d84f22dd2b612d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.1 MB (49073398 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:86950ae110c5289dc3e69bb968350389a8518baecff49fd87fe7d4500a8b6dad`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 Aug 2022 01:12:09 GMT
ADD file:71b63eb97aab99188c2771a47670a0a137cdf6750c2eafce78fc05f97d3a81ff in / 
# Tue, 02 Aug 2022 01:12:14 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 01:12:25 GMT
RUN echo 'deb http://deb.debian.org/debian oldstable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:5353918315f6371768d54771f05e4e173e44d23ce24e8b6fa42dc86346ddea83`  
		Last Modified: Tue, 02 Aug 2022 01:23:10 GMT  
		Size: 49.1 MB (49073171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce9c3a3f809d1fbb031cd4f07b775d97d21c0cea8d86f95d3dbdad0c67759d51`  
		Last Modified: Tue, 02 Aug 2022 01:23:20 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:oldstable-backports` - linux; ppc64le

```console
$ docker pull debian@sha256:080e80083a20095e4d5b32cc6afcdfbd4701ebf184235183727ae6f8ba8da6d1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **54.2 MB (54177501 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b1152da80e41ba3c3afb31c4700317373729825fd29b24ebed082014b239a319`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 Aug 2022 01:18:20 GMT
ADD file:3735b055a4bee159246ee1f72cf18985578603af0feb9307e3574122141ebae7 in / 
# Tue, 02 Aug 2022 01:18:22 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 01:18:28 GMT
RUN echo 'deb http://deb.debian.org/debian oldstable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:1aa0385aae35f2a4cfe43d3178a7a9b745dbc1ffa49f59d8ab4350ebdf46f1bd`  
		Last Modified: Tue, 02 Aug 2022 01:26:16 GMT  
		Size: 54.2 MB (54177275 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1be90acddb53645d5b529e6563dcdff27c55d61bf705bd8da21f0099251521e7`  
		Last Modified: Tue, 02 Aug 2022 01:26:29 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:oldstable-backports` - linux; s390x

```console
$ docker pull debian@sha256:71b8997cb396131ebf391aaf8a720376b5bcc07f1c7ce8933a5d4ba713ecd222
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.0 MB (49007515 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:180f96fdcb68553ba913e3a71b39d51b7ac1c1b5177f7927629e660915ec67f8`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 Aug 2022 00:43:08 GMT
ADD file:f1312a5e33cdcca200c1f8a80bfb9e3f50674f7c475879b46a254f46f6ce33ee in / 
# Tue, 02 Aug 2022 00:43:11 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 00:43:17 GMT
RUN echo 'deb http://deb.debian.org/debian oldstable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:22d1a970475335255aadaa454f5b87a34505c8c050d61be5e83d8f90e5c70b22`  
		Last Modified: Tue, 02 Aug 2022 00:48:51 GMT  
		Size: 49.0 MB (49007290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6dc33e533d05cd27a6099a38841d3bd33b60ae4bea83f77a6a96f7b6713d7972`  
		Last Modified: Tue, 02 Aug 2022 00:48:58 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
