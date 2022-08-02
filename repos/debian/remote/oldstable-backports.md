## `debian:oldstable-backports`

```console
$ docker pull debian@sha256:caadbae6bf7c6dbef7ad53348fc9df3af20862b9b77108d974d4a14435c14e05
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
$ docker pull debian@sha256:578f70d71b4bd4949cc4c7dd99af6ff97839ba650efd8ec82cb228a84d2d08c3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.4 MB (50440794 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2df1b4b3ba4cda158dce58bd833769595a5ec4e8ec0225a9c8e0196857fefe0c`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jul 2022 01:20:43 GMT
ADD file:e67a2bb3260496f108614926097424892142a0a3a6921b69cbaed881534c0fe0 in / 
# Tue, 12 Jul 2022 01:20:44 GMT
CMD ["bash"]
# Tue, 12 Jul 2022 01:20:48 GMT
RUN echo 'deb http://deb.debian.org/debian oldstable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:d8cdb5a0c4ab6682f7cc479b884faadfd33f793e1c8afe72183d3e9da4737d45`  
		Last Modified: Tue, 12 Jul 2022 01:25:43 GMT  
		Size: 50.4 MB (50440566 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d82adcdd8dfdbea303c8d7ef274ad03aa3b4ed9816c0be30b7d61285a4666bee`  
		Last Modified: Tue, 12 Jul 2022 01:25:52 GMT  
		Size: 228.0 B  
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
$ docker pull debian@sha256:ffa1b8b7898906cef4dd332ef875fa5068563d84e677cb2095134e84678722e1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.1 MB (49073349 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:301ebb5cd0ed14e4d5556d75b90db913ac112dc8930b1d9d994f89d1c02fa2c9`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jul 2022 04:42:45 GMT
ADD file:a14ea85307b9b9e93b1b3e35a03ebe2c6cf7ec6942cbf850732803bc2d7dd24b in / 
# Tue, 12 Jul 2022 04:42:51 GMT
CMD ["bash"]
# Tue, 12 Jul 2022 04:43:04 GMT
RUN echo 'deb http://deb.debian.org/debian oldstable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:497f43dfda4cd8c3e2bf7e1343c3a7b840f348b91e660488cd9d56cd2d179543`  
		Last Modified: Tue, 12 Jul 2022 04:53:47 GMT  
		Size: 49.1 MB (49073122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bfdf92d3971c4959e9f4318001aa3871bae651687ce20482ec36249c43b0b40`  
		Last Modified: Tue, 12 Jul 2022 04:53:57 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:oldstable-backports` - linux; ppc64le

```console
$ docker pull debian@sha256:3647c9bbe574c11cc4cf8ec0a86c6682f1171bba8735d006912ceb9424d873f6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **54.2 MB (54177319 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0e4a5a3917c565539d0f71f050d4cfcb7748535570082b2d792ef6ead6c25e00`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jul 2022 01:26:41 GMT
ADD file:1b516c064cfcd9c7e7a3c10601803a8d2f767d7689a53ad90a27e588c091c826 in / 
# Tue, 12 Jul 2022 01:26:45 GMT
CMD ["bash"]
# Tue, 12 Jul 2022 01:26:58 GMT
RUN echo 'deb http://deb.debian.org/debian oldstable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:7060ba5c5f34d79ac616a9711d022d626f6c129bc55b7fe5a5566bb711d25d7d`  
		Last Modified: Tue, 12 Jul 2022 01:39:06 GMT  
		Size: 54.2 MB (54177092 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:183b292d92e8f5251844384c120a75e1452dd2dd50c621ef1f2b28142c8fbe28`  
		Last Modified: Tue, 12 Jul 2022 01:39:19 GMT  
		Size: 227.0 B  
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
