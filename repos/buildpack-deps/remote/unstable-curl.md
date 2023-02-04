## `buildpack-deps:unstable-curl`

```console
$ docker pull buildpack-deps@sha256:50bb65dd2b179fa0f44e655b7fccf614bd3b3c7c962624eca793de9811a7b26a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 9
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; mips64le
	-	linux; ppc64le
	-	linux; riscv64
	-	linux; s390x

### `buildpack-deps:unstable-curl` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:04b2b47a93d279a3aae93a1502ed254adcfb420c6f9080bbe9d69e1e3cb32cd9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.4 MB (69427121 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ea8c34a3d19e3c3c359dde146d1f0954a2af77729ee5bf3dddcbeb35c2e62d56`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 04 Feb 2023 06:52:42 GMT
ADD file:a2e9c6618e31202c1b929d106d9d8f2e98a0d6a45ae13b56e9149536eee01769 in / 
# Sat, 04 Feb 2023 06:52:43 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 07:25:35 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 07:25:41 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:9338402809c6c0e98dbcb30453239ee887fa0b3378ee26565d576b66c08dfdea`  
		Last Modified: Sat, 04 Feb 2023 06:57:50 GMT  
		Size: 49.0 MB (49039305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4000be28de3a086efcb096b84ff6947c42412ed2bc4e11f3ac254f7bd261ad9e`  
		Last Modified: Sat, 04 Feb 2023 07:31:34 GMT  
		Size: 9.0 MB (9033091 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e133244bdf5da6e4b9014a53c5852a95e3d23591adc288ee97761ce0ae33b538`  
		Last Modified: Sat, 04 Feb 2023 07:31:34 GMT  
		Size: 11.4 MB (11354725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-curl` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:27f0ee8f50baa5eba0819ca08c1b0081d16ec92bbdc723d28fb22224d67b9d30
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.5 MB (67479793 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1f1318d0656aaa51c62c215d480ee14f7b9a0dc2fc03585bff427122a04662b1`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 04 Feb 2023 02:46:53 GMT
ADD file:12eddccc39577b9f5e10835b6a2c5edd0b1a49ad547e20f5e2640f434b8d2a42 in / 
# Sat, 04 Feb 2023 02:46:54 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 03:18:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 03:19:05 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:9756a18a5cc1d83f45eef500c448fdd88a17d9e9c99f86f02056851b6b5ac543`  
		Last Modified: Sat, 04 Feb 2023 02:52:12 GMT  
		Size: 48.0 MB (47996437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:395fe962304c3c3ba0027d920911fc9ab41a7242d7642f72fee189ed95174159`  
		Last Modified: Sat, 04 Feb 2023 03:24:35 GMT  
		Size: 8.5 MB (8481338 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29a388c264e9b4ce6fddf6a155cc927db77f824e38f9f65a6e0faa5dfb07c3e5`  
		Last Modified: Sat, 04 Feb 2023 03:24:35 GMT  
		Size: 11.0 MB (11002018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:5abe15b673aa7b6ddb566b304274cfe9a425bfc13d5fa505ca060452cbacdbae
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **64.6 MB (64556639 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d827ece5087518ab4be95a0c7becb30e443b07833a7f8e54f7a5e714a15ef14a`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 04 Feb 2023 10:00:50 GMT
ADD file:3ef0e7784a31367bd6b8f62d72fd921e841a63c5f468870ca51cb13d32a10c98 in / 
# Sat, 04 Feb 2023 10:00:51 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 10:52:40 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 10:52:47 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:4ade7fb7e5df21b5001435afddae5270817c5e2a665e698f2b89244410fe9cf7`  
		Last Modified: Sat, 04 Feb 2023 10:08:21 GMT  
		Size: 45.8 MB (45796020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24bceada3f9ea60690de207a1e9c70a03da888ace132ddf883dae8d5fca62d92`  
		Last Modified: Sat, 04 Feb 2023 11:01:34 GMT  
		Size: 8.1 MB (8124737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50080361018a99fea8d092caa292a14416ca537e3bd79c9f67230d9a7c08a73d`  
		Last Modified: Sat, 04 Feb 2023 11:01:34 GMT  
		Size: 10.6 MB (10635882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:b269e30259b222669c46eeddd51445cf25fbd9feb6e0ae8ccb1136d68452816e
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.3 MB (69250336 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9f6e5471417fed5abba8dafdf2406a316ac445437da016ce6713040692185f39`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 04 Feb 2023 06:18:18 GMT
ADD file:e0f39d8fee93f482160beca25b949b1de50ecc55ac86b1c276bed0b5c9955393 in / 
# Sat, 04 Feb 2023 06:18:19 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 06:48:31 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 06:48:36 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:541de84dec560e0a7dc13f9e5246f1a165b0955a6aefdc92d0bc46a50138a249`  
		Last Modified: Sat, 04 Feb 2023 06:22:53 GMT  
		Size: 49.1 MB (49064951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6930bf2e2eda29b99cfe171c0422db365474b36931b359c0da6fff3dad52f8f6`  
		Last Modified: Sat, 04 Feb 2023 06:53:51 GMT  
		Size: 8.9 MB (8865606 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d13ff72c8703f7d53521adcfd3a671f43824fbccadf8fa55bb396a67218577f`  
		Last Modified: Sat, 04 Feb 2023 06:53:52 GMT  
		Size: 11.3 MB (11319779 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-curl` - linux; 386

```console
$ docker pull buildpack-deps@sha256:1fc0b31ca75d522079c5b49b3a418c807651dd9f0ed09523fdc5597f31983b65
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.9 MB (70864438 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0fee61b6d0e9991f13fdf2d2626f616be48de2547af9c65e4183e7a02ae169b1`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 04 Feb 2023 07:50:25 GMT
ADD file:e52d2501a6498b9d4b4b7c45345d2dd2f2fbfa7df2849d1f794768270c0971a5 in / 
# Sat, 04 Feb 2023 07:50:26 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 08:23:03 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 08:23:10 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:dc17d0499e93f237d6be86c3138e9cea4fd1d950920edfec3d640e8d8b6e6230`  
		Last Modified: Sat, 04 Feb 2023 07:56:51 GMT  
		Size: 50.1 MB (50095432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:710c92d5b146f60cc687aee2f6d6a8c5c0a878fe515dedd23c774c10eb2ae049`  
		Last Modified: Sat, 04 Feb 2023 08:29:19 GMT  
		Size: 9.2 MB (9211457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1259464f51bb3a359b44d45da125dab6d573ba39303370fdb924ff37d221981`  
		Last Modified: Sat, 04 Feb 2023 08:29:19 GMT  
		Size: 11.6 MB (11557549 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-curl` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:739a279836915a40fae05a884261fef806346aaef2822c9bc5c55353980ca381
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.5 MB (68547916 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:415810c304ec4743f900c43f7785c0f4388217a5cabde6e10eccca45bbad1e0d`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Jan 2023 16:35:05 GMT
ADD file:a772415cec37230670450044a3962179f53657814c9c0e8bc6ef502ab4fff614 in / 
# Wed, 11 Jan 2023 16:35:12 GMT
CMD ["bash"]
# Wed, 11 Jan 2023 17:30:54 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 Jan 2023 17:31:31 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:d8fe537e863349284188081cc926e1cbc3d1d09a758c86969580374a79f6a9a0`  
		Last Modified: Wed, 11 Jan 2023 16:44:00 GMT  
		Size: 49.0 MB (49043063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a48d22c89d2231b986e2d8e07b29039b4077a44f2ed6aac30212a0adc292871a`  
		Last Modified: Wed, 11 Jan 2023 17:46:11 GMT  
		Size: 8.4 MB (8400802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13bf98ffebf3705900ffc4ce2bc2ee4d9f6f919564fdc57406d4df67e95f4b87`  
		Last Modified: Wed, 11 Jan 2023 17:46:12 GMT  
		Size: 11.1 MB (11104051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-curl` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:e6516355d5355fca39c7b51b795bd1f6127d73e0123443df3c72bb27f6c2e1e0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.8 MB (74808691 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9aaebe271226e56519ecb2868bad2010807fefd88187277321119b2e87f9229b`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Jan 2023 03:49:50 GMT
ADD file:a8a466b916dd8b82163da9263cfb32eb757c2a0eb173228a5ac8ef05bdc55653 in / 
# Wed, 11 Jan 2023 03:49:53 GMT
CMD ["bash"]
# Wed, 11 Jan 2023 07:17:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 Jan 2023 07:18:10 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:35c8c29d2bf600cd3a311b3649ac4076a0670c35cc296f1f28d2622bb6dd54d4`  
		Last Modified: Wed, 11 Jan 2023 03:56:03 GMT  
		Size: 53.1 MB (53077709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ab0d63135d44be3ecac38d5206687b79632de571e5c05f58c0a49d13d4dd332`  
		Last Modified: Wed, 11 Jan 2023 07:27:41 GMT  
		Size: 9.6 MB (9615481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49b2df2d7c9512f9de0ee08a692413dcbdbf53d56bc49fda25fae6cba32ce022`  
		Last Modified: Wed, 11 Jan 2023 07:27:41 GMT  
		Size: 12.1 MB (12115501 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-curl` - linux; riscv64

```console
$ docker pull buildpack-deps@sha256:46df8aa307719f7e97954d0b186525e8d9bed29360c27391d85f122b798b2019
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.3 MB (66322550 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d8310571e7a0148504222ea198ace657103448b49d570daa059af1d7f427438e`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Jan 2023 16:17:03 GMT
ADD file:7633d34a8711e495e7abd3b8910b40d85f085ef637af72b73a3cf0857da28314 in / 
# Wed, 11 Jan 2023 16:17:05 GMT
CMD ["bash"]
# Wed, 11 Jan 2023 16:39:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 Jan 2023 16:40:35 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:1ea40b6f65c9b971f19699fa099a82adee884a133e7c3754e31307ee85ba8833`  
		Last Modified: Wed, 11 Jan 2023 16:20:23 GMT  
		Size: 46.5 MB (46470644 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d42baba349a5568702ac30e211e6b9f1cd7d79f2082d1926e78abe18816ac39e`  
		Last Modified: Wed, 11 Jan 2023 16:54:22 GMT  
		Size: 8.1 MB (8076481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:284421ee2357fc6da691ef109f99b7794c53da89d6702c96e6b64c9ba7e365a6`  
		Last Modified: Wed, 11 Jan 2023 16:54:23 GMT  
		Size: 11.8 MB (11775425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:8949c3ed03c47aa1b3a18f75988362ee9476ef5696675dffe53fc0761bc4f0df
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.3 MB (67292633 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:101affee787232fc5f51c487e2f81ed6362e4a1d42e68471ed1bfab0a470acb4`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 04 Feb 2023 04:06:27 GMT
ADD file:93877457106ba25112f38787099a736e27572cac3ea286b62bb0cea369e7334a in / 
# Sat, 04 Feb 2023 04:06:29 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 04:33:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 04:33:59 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:0eed18e15556323b9c6a0c2e3bb53a6d5526fb5398a405780091330bc1da9c2c`  
		Last Modified: Sat, 04 Feb 2023 04:10:42 GMT  
		Size: 47.4 MB (47408087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6536f8239e347252e1f3cdc22fe9df56c0b9215fefb3e2510b174579df58afed`  
		Last Modified: Sat, 04 Feb 2023 04:40:31 GMT  
		Size: 8.7 MB (8666333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dade48b27fe2a94e7c854679e6f337da7e24a6cd38e0413e30ce13ff2eae0232`  
		Last Modified: Sat, 04 Feb 2023 04:40:31 GMT  
		Size: 11.2 MB (11218213 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
