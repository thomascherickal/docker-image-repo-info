## `buildpack-deps:sid-curl`

```console
$ docker pull buildpack-deps@sha256:9704d742b4f9708d0774d9d1db227882dadbbfc7445a8f752dfe5af6e31eb50c
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

### `buildpack-deps:sid-curl` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:6bee0e13105c7e6ecbe85f2ccbc1840e057f562aff1e6a78d3331b54fe5a814e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.7 MB (69689819 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:96c57d23dce65e05ce189de09c74e6d42f3fb1e3fbd1893d3885431d67847a0c`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 09 Feb 2023 03:21:29 GMT
ADD file:b3a4ee0f0fbf2d8fbbab0aefd91aa4d658c41b09c8a2beea1024bfce5e7d3fca in / 
# Thu, 09 Feb 2023 03:21:30 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 09:14:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 09:14:17 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:ca2c7deeb5af7aa8a0aa3358218901c07b10bb98573151782e5e7af0ab03009c`  
		Last Modified: Thu, 09 Feb 2023 03:26:46 GMT  
		Size: 49.2 MB (49234515 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3f93cb2a3ee7c65cae5b96772e26d36982fbb6f591036fc399794173b26a5be`  
		Last Modified: Thu, 09 Feb 2023 09:20:03 GMT  
		Size: 9.0 MB (9049525 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:550c07c3dce5647c4605a0f377d103211b5f499343e022eb8a7ca1fec0e6146c`  
		Last Modified: Thu, 09 Feb 2023 09:20:03 GMT  
		Size: 11.4 MB (11405779 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-curl` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:f4f86364f9dcf47a118bd903539781165f43891032d76265cbc114a1d619ead6
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.7 MB (67714904 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:136fc72c9b01c2ed142ec59d991bcb7628e0bcaf74e95c43e2f378dc7a045be5`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 09 Feb 2023 02:00:45 GMT
ADD file:dc28e6a68656b2258d74ca814eedc70f45b8b6c604f68add2cf2f5f7bca2b675 in / 
# Thu, 09 Feb 2023 02:00:46 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 02:33:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 02:33:27 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:cfc3c8b7a8637963e4e7c58d3159378d2dbbf0ac34f355b8781c04894e7b070c`  
		Last Modified: Thu, 09 Feb 2023 02:06:07 GMT  
		Size: 48.2 MB (48168655 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b0465a62c889ae7f4e147e07d5d9bf9550c4429db66328d0b271ef3a102aadd`  
		Last Modified: Thu, 09 Feb 2023 02:38:57 GMT  
		Size: 8.5 MB (8494792 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af07aa0cc01d6588de33c6d10e2165894401135ac335ab64e1eb43ae2718b707`  
		Last Modified: Thu, 09 Feb 2023 02:38:57 GMT  
		Size: 11.1 MB (11051457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-curl` - linux; arm variant v7

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

### `buildpack-deps:sid-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:26457943f046c177fe874d01571fcc0543d491869b2c5dc75bdd9688729eb9d6
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.5 MB (69525233 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ecd1582b984597c450ef66dd800d9868193d8833216e20304543fd339834a899`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 09 Feb 2023 03:59:27 GMT
ADD file:e092144c3667bd346dc4cb05da5a70ca9f7303d7160f9d5763af88fe51e02f66 in / 
# Thu, 09 Feb 2023 03:59:28 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 09:10:59 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 09:11:03 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:00f9d2ac5ed56c16a45852afb781f7257c58125a3b154fa75d18141566291f9f`  
		Last Modified: Thu, 09 Feb 2023 04:04:03 GMT  
		Size: 49.3 MB (49272262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4236d19f832b8139af289e6bc94d52514e6619bf7af68bf4e0d5486d078ab198`  
		Last Modified: Thu, 09 Feb 2023 09:16:12 GMT  
		Size: 8.9 MB (8881496 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0d593ddd7505c3c57f2e72480778f0c8b24fd4fc541502ac3315e74da1ece02`  
		Last Modified: Thu, 09 Feb 2023 09:16:12 GMT  
		Size: 11.4 MB (11371475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-curl` - linux; 386

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

### `buildpack-deps:sid-curl` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:31fbd48d97655e5743ae24d79f322184b28fe3e464b6ed9b4413ed1ffbea4648
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.7 MB (68662092 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:44c4ec537af7ac1217076c5de461da3049f4b71d1e970249041e8a4abcdf3f1e`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 09 Feb 2023 02:46:00 GMT
ADD file:e14c7d6714484cc404ef7af2c7e0fcb17120cc8c1b631e9ac731a3be75da22b8 in / 
# Thu, 09 Feb 2023 02:46:04 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 07:48:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 07:48:58 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:84e1d5547cbc284ab87d41eaa50711a7148e6080522c4ba245d27048c9d0fe70`  
		Last Modified: Thu, 09 Feb 2023 02:54:32 GMT  
		Size: 49.1 MB (49094289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16034fc732dcaff117d4120f724155ad39c461a2791c8bc488000dd93d88467c`  
		Last Modified: Thu, 09 Feb 2023 08:03:01 GMT  
		Size: 8.4 MB (8414070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95cc8b6e8bd467b0d1e27bfaf0bf0138f2e690aa8dd7eeddcc636d65c4b0ac34`  
		Last Modified: Thu, 09 Feb 2023 08:03:01 GMT  
		Size: 11.2 MB (11153733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-curl` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:b5f4ec38d05fa7dd163d0940017fef93e82e451aff93d36a5f231080570fd5cd
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.8 MB (74780613 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e0a56d4fcd381071f83c824d6b588ca6ad9b47fbd640158800384acccd9503d8`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 04 Feb 2023 12:26:15 GMT
ADD file:24ea24099063f3d78eb81b653d243295dc4b47f84833c244197869e3675e3840 in / 
# Sat, 04 Feb 2023 12:26:18 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 18:06:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 18:06:18 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:5983dd3dde0b9f046ad79781724edbc7a225d54d2fdbccc7f201d0ed78cde5ce`  
		Last Modified: Sat, 04 Feb 2023 12:32:41 GMT  
		Size: 53.1 MB (53052494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e08f2a71cbb1b4094ff1e2b2a99f6f2a5508609219ea425d8d5e97ee29bedbe`  
		Last Modified: Sat, 04 Feb 2023 18:16:35 GMT  
		Size: 9.6 MB (9613407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3fe989edce909a5b969e93271b155a155556141e287bb0104be1e17eacdb5d8`  
		Last Modified: Sat, 04 Feb 2023 18:16:35 GMT  
		Size: 12.1 MB (12114712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:192a4a069b0f4262629d5af43f6c4cef18a91797692314478ac7b405d716f268
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.6 MB (67556089 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5911cbbe8d9f1d308c7da15a06191c5ec20e63bfca5ecbd2a6ff4399c25933dd`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 09 Feb 2023 02:41:57 GMT
ADD file:2e666c175716fd02a858ff036fcece3fd5bc91959ad6e87ba5371f0e1c35eee8 in / 
# Thu, 09 Feb 2023 02:42:00 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 07:33:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 07:33:22 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:3019a6e7de2300389d30ae5349430a715e5e0de8dee24a1c55adb1f7bf5c4133`  
		Last Modified: Thu, 09 Feb 2023 02:46:21 GMT  
		Size: 47.6 MB (47605532 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe2bb0faf3ad6788e6ff9dc1a5f7979c08396fca0cc8a68674481cb53146b784`  
		Last Modified: Thu, 09 Feb 2023 07:41:24 GMT  
		Size: 8.7 MB (8681429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff6878c76211620beede9a73a2e8ac2a5aecaefaf3857d40ddecc77e798a54c9`  
		Last Modified: Thu, 09 Feb 2023 07:41:24 GMT  
		Size: 11.3 MB (11269128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
