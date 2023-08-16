## `debian:bookworm-backports`

```console
$ docker pull debian@sha256:a76a6ca48adfaefb9ebf8414790837b34ee8e47e41ea3f557cad6fa3277a4319
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
$ docker pull debian@sha256:94cc0fa8f02ce441b4c65161aceebeb5a39da61382a33884e353f87e43476392
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.6 MB (49557582 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0ce1a8b46e4a61bb2021678c45e0450c7606b761653920f33c4145a3e314b864`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 27 Jul 2023 23:24:29 GMT
ADD file:cc1376ecb3d9e93e4160573c110da753ffeb2efe2223351f1fbf483d89f1a756 in / 
# Thu, 27 Jul 2023 23:24:30 GMT
CMD ["bash"]
# Thu, 27 Jul 2023 23:24:37 GMT
RUN echo 'deb http://deb.debian.org/debian bookworm-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:785ef8b9b236a5f027f33cae77513051704c0538bff455ff5548105c954c3b1c`  
		Last Modified: Thu, 27 Jul 2023 23:29:02 GMT  
		Size: 49.6 MB (49557354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eec98594c9741e8ebf7719ea4869fa51dbbc8807c197f0fdebb05a88111b8f7f`  
		Last Modified: Thu, 27 Jul 2023 23:29:17 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:bookworm-backports` - linux; arm variant v5

```console
$ docker pull debian@sha256:79c5cbe003aa55807f749a4babf85c128776e6c71cbc6ca04d6989fc06b6f79a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.4 MB (47415246 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1c2dcd9f6580363956331578bb5375d2c8d263881d472e3f8536094557d3ba33`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 15 Aug 2023 23:48:23 GMT
ADD file:f079a473284b30bb99c4a21c61719c499c0a305c49fedaa717bbfefef021b7fe in / 
# Tue, 15 Aug 2023 23:48:24 GMT
CMD ["bash"]
# Tue, 15 Aug 2023 23:48:27 GMT
RUN echo 'deb http://deb.debian.org/debian bookworm-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:1efc9639d902ebaa56d5e963066d5ab28cdf0e5fac5aa967c72326db76357b0e`  
		Last Modified: Tue, 15 Aug 2023 23:51:10 GMT  
		Size: 47.4 MB (47415020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb1f4fa3c5ffe50ef22ea0ae71f54afd804bdd19fb4fa457eef3200d478e2c37`  
		Last Modified: Tue, 15 Aug 2023 23:51:25 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:bookworm-backports` - linux; arm variant v7

```console
$ docker pull debian@sha256:baf544058bb50737e9812b0263089d7e7482b4526c265935823dbe9935fa520d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.2 MB (45233163 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3fbf24034145db9589ba3629e4e55e19b432f75e53debac0fdc01b27d2981fba`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 16 Aug 2023 00:16:59 GMT
ADD file:03964ab92340a6f07fac7e332ca5f5401b3a35aa1e4a5c0b2484a71ff345bc29 in / 
# Wed, 16 Aug 2023 00:16:59 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 00:17:05 GMT
RUN echo 'deb http://deb.debian.org/debian bookworm-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:22c91d9cbb3cbc0e4a05c1bfc86da0b5a439ded4f68eb2fbc055ba6b85ca1d90`  
		Last Modified: Wed, 16 Aug 2023 00:21:04 GMT  
		Size: 45.2 MB (45232937 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33a1dd2e35a39f9bd49b44b978e1aed2273e45be6ef96a3a15b64c5c8e8650e4`  
		Last Modified: Wed, 16 Aug 2023 00:21:18 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:bookworm-backports` - linux; arm64 variant v8

```console
$ docker pull debian@sha256:6ef941ea8073dd905672c136ace9d126a6f53b7c611e31fdfd55c4cf9463a401
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.6 MB (49591537 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2880ff9452653f040adf527af4ae05958ff678a47de6025366d30053d0407536`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 15 Aug 2023 23:39:49 GMT
ADD file:ca43018e3d97d44b49e60fe002bb20834a74cc1163d7e95ad50d549f072de158 in / 
# Tue, 15 Aug 2023 23:39:49 GMT
CMD ["bash"]
# Tue, 15 Aug 2023 23:39:52 GMT
RUN echo 'deb http://deb.debian.org/debian bookworm-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:a014e5e7d08c37cf1703b97e701ccdc850e4a18d0ee679f03aa875dcd520aa85`  
		Last Modified: Tue, 15 Aug 2023 23:42:59 GMT  
		Size: 49.6 MB (49591310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:614f5f1cb5cac26c70bd5da32eea411daa79d5505c57f9de7bbbd13d2dbc953c`  
		Last Modified: Tue, 15 Aug 2023 23:43:13 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:bookworm-backports` - linux; 386

```console
$ docker pull debian@sha256:3a28734b61d2a750621f91d00b9c2ad65ec852a3d4552d20ad1f792643286900
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.6 MB (50568280 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6cb973c83c5348d65f04c1dfb917dc7c0515c30a2a62bb1af4c28d0f992ec6f4`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 15 Aug 2023 23:38:49 GMT
ADD file:3f0a4d6b18b22088d0785bc2e351d829ad1ed6f154058017035842bdbe2a8d1e in / 
# Tue, 15 Aug 2023 23:38:51 GMT
CMD ["bash"]
# Tue, 15 Aug 2023 23:38:54 GMT
RUN echo 'deb http://deb.debian.org/debian bookworm-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:1dc6cc826af02d533745c4612f635e028f3471e46f50422fd20a6dc913b60574`  
		Last Modified: Tue, 15 Aug 2023 23:43:02 GMT  
		Size: 50.6 MB (50568054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abe57fb2b2913fedd1dce7b7a11ccc99127c25373224d0386538b58cf7e57f33`  
		Last Modified: Tue, 15 Aug 2023 23:43:15 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:bookworm-backports` - linux; mips64le

```console
$ docker pull debian@sha256:284c0afd1fb0677aa8c1e5a32ffc8b75cd2c85b4012281b37e2b8934b6fe8789
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.5 MB (49542229 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:081081b8186b54d8f12a1ced11719b91569a3490ee9f1b06f3effeb5abe3b6ef`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 16 Aug 2023 00:08:02 GMT
ADD file:359d49b8d6eb4185590cb5da2825a99e2b2d4b4d81519b9283794e64261eec2c in / 
# Wed, 16 Aug 2023 00:08:08 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 00:08:20 GMT
RUN echo 'deb http://deb.debian.org/debian bookworm-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:96b8a462ea6d525b430e77289e7ae92006277c062da33a8446fd1e664d41600b`  
		Last Modified: Wed, 16 Aug 2023 00:18:49 GMT  
		Size: 49.5 MB (49542000 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45de9043497c7f3abd004df4ba526f02295239266abcb1e0944f75d334f44022`  
		Last Modified: Wed, 16 Aug 2023 00:19:07 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:bookworm-backports` - linux; ppc64le

```console
$ docker pull debian@sha256:52b1e4a0dfc07a16303a6c2bb7fff5b99886ae83c39a87f02470370a794e2674
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.5 MB (53543571 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2c4598d6e9bd2a8e1851f636103abf1f479a74f7b327a348fff56cc386d99823`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 27 Jul 2023 23:22:41 GMT
ADD file:b20300808df8e1ce5b5ff534088c39d6b04467476af024e54545f7857f78a508 in / 
# Thu, 27 Jul 2023 23:22:43 GMT
CMD ["bash"]
# Thu, 27 Jul 2023 23:22:51 GMT
RUN echo 'deb http://deb.debian.org/debian bookworm-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:b6d31d119ff78cff1435e4eb51d8918916c2d5057cebf12b76d5352660fb90de`  
		Last Modified: Thu, 27 Jul 2023 23:28:46 GMT  
		Size: 53.5 MB (53543346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ade5f8824804f6b322a3ea1f2bb59c83960518cd29c33673ed6f7d5d3b0b637d`  
		Last Modified: Thu, 27 Jul 2023 23:29:08 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:bookworm-backports` - linux; s390x

```console
$ docker pull debian@sha256:7e45667efe0c8a831f5845f8990062b5331513894a05e997105d828b93f17445
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.9 MB (47922240 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d9a67d4f6bb43690a0b7372b86276ae8c66b1dd53e4bb5a3bbf490c50e67605c`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 15 Aug 2023 23:42:11 GMT
ADD file:eeb165e8fcc9b8f3a9e8f10fdbd507a91bc934046a4f23f2d636ca4b1796d1e3 in / 
# Tue, 15 Aug 2023 23:42:17 GMT
CMD ["bash"]
# Tue, 15 Aug 2023 23:42:22 GMT
RUN echo 'deb http://deb.debian.org/debian bookworm-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:2bf08d586558a71fd0c5172579e7c378968a16f427fb3af772e4aa11c6b0a7af`  
		Last Modified: Tue, 15 Aug 2023 23:47:38 GMT  
		Size: 47.9 MB (47922016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a931177458e0c7fada0bdafead5ac663263ab0fb69fc11df9c1a0e4b619224b3`  
		Last Modified: Tue, 15 Aug 2023 23:47:45 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
