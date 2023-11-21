## `buildpack-deps:unstable-curl`

```console
$ docker pull buildpack-deps@sha256:8ef77eb2774e4fe2106cf9faa151b5e9cc8ef67d30d73a0a2365a7714575774d
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
$ docker pull buildpack-deps@sha256:55d3c9a086b1f3e2bf2efc43a3facd9259debb301bc36d744d399b9f9183baab
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.9 MB (73888718 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5ca5ff02ac501d48c546df140a835f2ebdb2306a1a564dd635fc72f385dd9659`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:22:27 GMT
ADD file:69815228666696b3cd3b2799492e3d9cdf4f513ccca5c1cc9282f6c569cc8730 in / 
# Wed, 01 Nov 2023 00:22:28 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 00:57:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:bf371b8152e5df155015cbda7e76bcf445a8be262f7017a9c2cd27a64c3bd875`  
		Last Modified: Wed, 01 Nov 2023 00:28:24 GMT  
		Size: 49.5 MB (49534303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfdee5573ddff91e45c81d11193d3d33f964fe89aa56549950a84c64303f6c2f`  
		Last Modified: Wed, 01 Nov 2023 01:05:03 GMT  
		Size: 24.4 MB (24354415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-curl` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:8fd71e79ed7adb4eabd5ab187c04681bd8d7225ad23f383b19e2983aafe7dca9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.2 MB (70208940 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2d62ceb7c735018d913dc495afa525a353cb6e5196e0df330873dac97ea2527f`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:49:10 GMT
ADD file:3dfec265d80292cf14629bdbd49822be7a5672ab8299d43e9ec734f6e032c8df in / 
# Wed, 01 Nov 2023 00:49:10 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 02:59:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:0609920749c8743a3627a0a7a377598014123518f5e0ed7f1443c78c8c9f3446`  
		Last Modified: Wed, 01 Nov 2023 00:53:10 GMT  
		Size: 47.2 MB (47192458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba3b7ab88084f4d09eb30fe75dbc159cd99b0692cea6232d2f457c292a62968c`  
		Last Modified: Wed, 01 Nov 2023 03:07:10 GMT  
		Size: 23.0 MB (23016482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:51146f13fdb6437822863cfb091ce22dd810970f7bf2062d9a989c5b98b20ad3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.2 MB (67216176 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:441627c1997be627df062cc68f9e0305629e418cd85ef184060f05d45e2ca94a`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:59:14 GMT
ADD file:a72fe3de4b178dd8b7c48a1dc98d4c14520570e5edb66049dfe2cd6bb0a5dd6c in / 
# Wed, 01 Nov 2023 00:59:15 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 02:36:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:f6e9a66eb905933433a5a2a8c16e480468f3731f107d5854bac12ef9a79bc271`  
		Last Modified: Wed, 01 Nov 2023 01:05:19 GMT  
		Size: 45.0 MB (44981409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c61548fabf75545be26d57a05800e5dbcd765a1c5c804a7671c92c59e15834d8`  
		Last Modified: Wed, 01 Nov 2023 02:44:58 GMT  
		Size: 22.2 MB (22234767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:37eb53a80fd102fcb5f14a4d0dc9bd7732ec1c734a422e4b427b175555c575a5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.5 MB (73469380 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0be9b3ee789a657aea7026023fad3bfad1ddd7a5e725b324dd61f03508c0130d`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:40:45 GMT
ADD file:1a4ef85bba464538c4f87a65a055d954fc8edc51f26efd06b43d8ae9f7e54f7a in / 
# Wed, 01 Nov 2023 00:40:46 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 02:09:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ba6956ade110f0fe56bbad19a8d10b1eb0ae1b1006ccba5fadff0026a00dbc20`  
		Last Modified: Wed, 01 Nov 2023 00:45:46 GMT  
		Size: 49.6 MB (49552835 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:516c292c0ab5612a524438779924b5cc187f530a208c71056c8b9994656ef043`  
		Last Modified: Wed, 01 Nov 2023 02:16:27 GMT  
		Size: 23.9 MB (23916545 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-curl` - linux; 386

```console
$ docker pull buildpack-deps@sha256:8988d06749683ea585cf137051dfe9710e79a4dd694e684d3de84c6bf3757d32
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.7 MB (75702236 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:830e36b2a276fddf3fa83594c87499d590059eb10e73ca22fcc5a827bbbda7c4`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:40:31 GMT
ADD file:0aa90abbd80c68d937903de7ac8fdcce0f516fdd70f080b677af1e2322c000b9 in / 
# Wed, 01 Nov 2023 00:40:32 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 13:50:40 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:96660bac4658b1bffb27e96ac8ecc86753a1844f042ede32c4f1faef702dc202`  
		Last Modified: Wed, 01 Nov 2023 00:46:42 GMT  
		Size: 50.5 MB (50516486 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7af088639fa61079db294f16f91145938a488365f2aec8cef7a85da80c4b13b`  
		Last Modified: Wed, 01 Nov 2023 13:59:54 GMT  
		Size: 25.2 MB (25185750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-curl` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:3d072782b869915c68ce21a8a78370274e3aad0379c863c87bed0513c371bf28
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.2 MB (73236978 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:48d581d8a17daaf6df47819c5605bf4a8542057b4a50efa28345f4f2918775db`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 01:12:08 GMT
ADD file:e27a157c42d1aedcb0f6cf695f1f5c31d442488e049826c940509e2288537427 in / 
# Wed, 01 Nov 2023 01:12:12 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 21:35:01 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:0eacf4d958160d2729e1bb31fbb12227afa7536ce6304928b13c2c65d297f9b9`  
		Last Modified: Wed, 01 Nov 2023 01:23:11 GMT  
		Size: 49.3 MB (49326735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76fea98d048b05ee3313ca45517a641b11637c7f8dc3ec543480fe6111a66fc0`  
		Last Modified: Wed, 01 Nov 2023 22:00:34 GMT  
		Size: 23.9 MB (23910243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-curl` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:e3fe6632a18f418e4435cc7a8063378cec3d6e7e86eda522d299f55d99caeb06
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **79.4 MB (79438926 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5f3939720778f56545dbb5f838729141ef56732c086b66a0537faf6460e0937f`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:22:46 GMT
ADD file:b4e182cbec02f1d3bb7c8ff0ef09924ac255ba6717bdd73f24d0a6114ff305d6 in / 
# Wed, 01 Nov 2023 00:22:49 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 01:31:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:46cca77d78176c861335b7b91e20d7b4cb2b3a75a124c300124de5818b724a9d`  
		Last Modified: Wed, 01 Nov 2023 00:27:59 GMT  
		Size: 53.4 MB (53438164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18c27d7acaf849316ba11ccd36c024abe28c48180ca4ed48c1d645cdbac13d42`  
		Last Modified: Wed, 01 Nov 2023 01:42:56 GMT  
		Size: 26.0 MB (26000762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-curl` - linux; riscv64

```console
$ docker pull buildpack-deps@sha256:d47d61fd7d6f36e367a86f12fb809a0caa3ca64d6514b9d4a264184bcdc171f9
```

-	Docker Version: 20.10.25
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.0 MB (74991264 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c519b4d73993379f707098d265c9b5132d01092cdf180e2bb22b72f3163cef07`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Nov 2023 04:09:02 GMT
ADD file:6edb177cc4c3fc7c02043410bba7fabbbaa23493a2e0444ac13e281f6fd7d209 in / 
# Tue, 21 Nov 2023 04:09:04 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 04:33:28 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:9197643899c29fb1e411101ee2f4e677b44704d5c2c8ce98f7567cb7f7a6cf58`  
		Last Modified: Tue, 21 Nov 2023 04:12:00 GMT  
		Size: 48.2 MB (48206696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0617cf6ad3eec888f08f7b773880b515adb1cae0586b8aa6f4b5f40076079dd`  
		Last Modified: Tue, 21 Nov 2023 04:43:06 GMT  
		Size: 26.8 MB (26784568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:c4b64ed3c6f7849da4bf232ee9b0346c8375234ae05e858fdaab19159c92be3b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.6 MB (73563925 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5fb6298a353936cc00a02214b0172e7ebcb8439494257afc18435c9ae46f6ac3`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:44:04 GMT
ADD file:e94f75ffd7aa648bb85fefcceb02afa58747273f05e89c473c1ad438c3ba2345 in / 
# Wed, 01 Nov 2023 00:44:07 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 01:59:02 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:43e2d693d4cc2a3e58c2344ef771699434d5f0e6ffb98ac8bdb822ee0e2534fa`  
		Last Modified: Wed, 01 Nov 2023 00:49:25 GMT  
		Size: 49.0 MB (48966976 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17216a40a3f2f28f99307df60faffa863e423de83464990e34dd5854b1206c45`  
		Last Modified: Wed, 01 Nov 2023 02:07:00 GMT  
		Size: 24.6 MB (24596949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
