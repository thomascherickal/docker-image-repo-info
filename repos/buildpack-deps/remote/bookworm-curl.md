## `buildpack-deps:bookworm-curl`

```console
$ docker pull buildpack-deps@sha256:2e3eac33829d6b53d214289b54fe38fc84cf33c99b37237d5398c353d063950d
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

### `buildpack-deps:bookworm-curl` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:a313e1ca160fa76c5d9dc53ebd96e5bf59f30162a48a3489fce2e67c2532fa98
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.6 MB (73587893 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cb6cafaf6952dbc34eed9b6f6e2adb817a4b14779c23edc0da1b871b776864e8`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 27 Jul 2023 23:24:29 GMT
ADD file:cc1376ecb3d9e93e4160573c110da753ffeb2efe2223351f1fbf483d89f1a756 in / 
# Thu, 27 Jul 2023 23:24:30 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 03:00:41 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:785ef8b9b236a5f027f33cae77513051704c0538bff455ff5548105c954c3b1c`  
		Last Modified: Thu, 27 Jul 2023 23:29:02 GMT  
		Size: 49.6 MB (49557354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a6dad8f55ae6c733e986316bd08205c8b2c41640bf8d08ff6e9bbcb6884304f`  
		Last Modified: Fri, 28 Jul 2023 03:07:18 GMT  
		Size: 24.0 MB (24030539 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm-curl` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:a7592f1639d909f25dccc729a2b5aaa513a70ee28a85c4189038b9717092f588
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.1 MB (70124664 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e3a21d1f5171263c0576c940aba7c50a5812f345cc44bb53c3530243b7749caa`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 15 Aug 2023 23:48:23 GMT
ADD file:f079a473284b30bb99c4a21c61719c499c0a305c49fedaa717bbfefef021b7fe in / 
# Tue, 15 Aug 2023 23:48:24 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 00:40:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:1efc9639d902ebaa56d5e963066d5ab28cdf0e5fac5aa967c72326db76357b0e`  
		Last Modified: Tue, 15 Aug 2023 23:51:10 GMT  
		Size: 47.4 MB (47415020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e34e7b4c1a2c0700b8db12eb4cb9569ce104cda1989e5b4a480e35dd71690d33`  
		Last Modified: Wed, 16 Aug 2023 00:47:01 GMT  
		Size: 22.7 MB (22709644 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:70e09d598b5c38a406d30c717457f324114b7db7ef5693e0ae9cc939200c9f82
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.2 MB (67169862 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ee2b3159316a467ca9e01e173c57a3aaf9062379e269053863138bf9e55e1d1b`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 16 Aug 2023 00:16:59 GMT
ADD file:03964ab92340a6f07fac7e332ca5f5401b3a35aa1e4a5c0b2484a71ff345bc29 in / 
# Wed, 16 Aug 2023 00:16:59 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 05:28:17 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:22c91d9cbb3cbc0e4a05c1bfc86da0b5a439ded4f68eb2fbc055ba6b85ca1d90`  
		Last Modified: Wed, 16 Aug 2023 00:21:04 GMT  
		Size: 45.2 MB (45232937 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24238a7fc18d7c6089f4f19e3e3d866f42674716043768c48cf6cabb7c8855b0`  
		Last Modified: Wed, 16 Aug 2023 05:47:31 GMT  
		Size: 21.9 MB (21936925 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:cff052d3d1eaf4b534c62e5725852806e16aab4f90a4144c555a766ca1e1b901
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.2 MB (73161356 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2eb3957cb621c85ee2f7494fa16ccb1c65eeeff85c9b649dc3c245c2f03e78ec`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 15 Aug 2023 23:39:49 GMT
ADD file:ca43018e3d97d44b49e60fe002bb20834a74cc1163d7e95ad50d549f072de158 in / 
# Tue, 15 Aug 2023 23:39:49 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 01:21:40 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a014e5e7d08c37cf1703b97e701ccdc850e4a18d0ee679f03aa875dcd520aa85`  
		Last Modified: Tue, 15 Aug 2023 23:42:59 GMT  
		Size: 49.6 MB (49591310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:715cea74ecbb15cb82efef1e77dd60c31d90b01d1286d6f39b4562afaebe75f3`  
		Last Modified: Wed, 16 Aug 2023 01:38:30 GMT  
		Size: 23.6 MB (23570046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm-curl` - linux; 386

```console
$ docker pull buildpack-deps@sha256:a837769bd3f8a9e4f69a513a0945a56bc51b71fe083f1ded5f3b22600433eed6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.4 MB (75437808 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:32d4066bf6815648a7034016ade53e884437be1fde6892f2b3083044d74b7a86`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 15 Aug 2023 23:38:49 GMT
ADD file:3f0a4d6b18b22088d0785bc2e351d829ad1ed6f154058017035842bdbe2a8d1e in / 
# Tue, 15 Aug 2023 23:38:51 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 00:25:45 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:1dc6cc826af02d533745c4612f635e028f3471e46f50422fd20a6dc913b60574`  
		Last Modified: Tue, 15 Aug 2023 23:43:02 GMT  
		Size: 50.6 MB (50568054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ca8436c5a9dc8b9ea408612ff7210bcceebd896671ed3e31c61f398f9a00f25`  
		Last Modified: Wed, 16 Aug 2023 00:34:36 GMT  
		Size: 24.9 MB (24869754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm-curl` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:a3e2a302292d240c5ef6a911d4bfedda10227f69539ea8c2ab29f62a31e82320
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.2 MB (73154697 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:199c7f9557e825f1e7c85367c036809337980df0f60ab3bd943ec9c3ef5a701d`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 27 Jul 2023 23:10:44 GMT
ADD file:3568f288ff9791a341f5cb0e99c0a63e09a68f3816d7f7a9971127b9b98a04b8 in / 
# Thu, 27 Jul 2023 23:10:50 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 01:11:15 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e4dbd8372ba202a8b430bce8d5c5b8a4bfdbc6ef2703180665e5964d51bb0437`  
		Last Modified: Thu, 27 Jul 2023 23:21:43 GMT  
		Size: 49.5 MB (49542050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a69206dfad992d03f1e8e833ae728ffacf2c6919f78c4822d849e341473efebb`  
		Last Modified: Fri, 28 Jul 2023 01:31:27 GMT  
		Size: 23.6 MB (23612647 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm-curl` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:2850f04eb55d1c646bead20a4b56782278f56cac1945ead77243a32e21dbd376
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **79.2 MB (79224885 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:25ce09dd7847a86d1a80c72f8b63f2fbcc394fc118b4fdb8db043e5ae72e30b7`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 16 Aug 2023 01:09:14 GMT
ADD file:8397677919f9bbf5273ddf61e008bcaace9195b46bcb2c31aff4f0a88617f12e in / 
# Wed, 16 Aug 2023 01:09:17 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 01:38:39 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:c59f7b2759f74830e13fa72caeaf898f560f72787aa9d5aec28bcf8585f2f066`  
		Last Modified: Wed, 16 Aug 2023 01:15:22 GMT  
		Size: 53.5 MB (53543761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cce374dd487e4d067dd2727a6401d31bd379da6e10a83e5a902a80be18aabaf`  
		Last Modified: Wed, 16 Aug 2023 02:09:27 GMT  
		Size: 25.7 MB (25681124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:3d921b58c4f6cfc3529e474bc5c5657b69f266389dbf9ca1e01a3f993d995631
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.0 MB (71950786 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0935d347529fc2d002323338e9b1d1227981a43082eb49f42287668f6cee7c76`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 15 Aug 2023 23:42:11 GMT
ADD file:eeb165e8fcc9b8f3a9e8f10fdbd507a91bc934046a4f23f2d636ca4b1796d1e3 in / 
# Tue, 15 Aug 2023 23:42:17 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 04:20:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:2bf08d586558a71fd0c5172579e7c378968a16f427fb3af772e4aa11c6b0a7af`  
		Last Modified: Tue, 15 Aug 2023 23:47:38 GMT  
		Size: 47.9 MB (47922016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7afba98ba5dea198ec27ff40c833c54ce73ca11dccc94b59611cb506b44fa422`  
		Last Modified: Wed, 16 Aug 2023 04:36:16 GMT  
		Size: 24.0 MB (24028770 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
