## `buildpack-deps:unstable-curl`

```console
$ docker pull buildpack-deps@sha256:f2a2ea21e17f23805a1868853cd02dd1b64e71c71e5f612ce27c6322fd6b16cd
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

### `buildpack-deps:unstable-curl` - linux; amd64

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

### `buildpack-deps:unstable-curl` - linux; arm variant v5

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

### `buildpack-deps:unstable-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:89c74b58d25bde00550060afd884f094990be83b1aa48e86db9cc97a9168c9b2
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **64.8 MB (64815263 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fff39f618513282bc5d758d7d6367f13ecb4ef635f2b4fb0a2e407551507b5ed`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 09 Feb 2023 06:13:32 GMT
ADD file:fbab075e495bd9771e90704c5bfe9fb15c30193973e2bb5c45e75cd23af10cf3 in / 
# Thu, 09 Feb 2023 06:13:33 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 17:40:42 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 17:40:49 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:a7ea7bdbf318551bbcc5dd17e61a023405583aed3de05afb9d0d7d7c69f7d9f1`  
		Last Modified: Thu, 09 Feb 2023 06:21:13 GMT  
		Size: 46.0 MB (45986881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cae37dac679959624898f1540e289e04f11094cac8e34e5a293d7b735010ab1`  
		Last Modified: Thu, 09 Feb 2023 17:49:39 GMT  
		Size: 8.1 MB (8140778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e5340840f2ef04e80ad9c82beb3b4a9f0685e521d4da3bcd8a7a2b582fa331d`  
		Last Modified: Thu, 09 Feb 2023 17:49:39 GMT  
		Size: 10.7 MB (10687604 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-curl` - linux; arm64 variant v8

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

### `buildpack-deps:unstable-curl` - linux; 386

```console
$ docker pull buildpack-deps@sha256:7775123d52ec33d262e7aef1f0b378fd735992260d8f9ebdd587eba11d316a63
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **71.1 MB (71121205 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4c45f42882fd81e78a2ed73244b0f22e24b78df8ed55af626a8d8ca2ba7d8150`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 09 Feb 2023 05:14:01 GMT
ADD file:9ac1978405b6f0a95e33d1c34f01be82bbc11fcce2878747e4f688335279964c in / 
# Thu, 09 Feb 2023 05:14:02 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 12:21:22 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 12:21:29 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:e58ae2871ac91256d220f3da2b9736b2afb1a06906579876546cfae103647f95`  
		Last Modified: Thu, 09 Feb 2023 05:20:31 GMT  
		Size: 50.3 MB (50285434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63157a71f0b70036d0f159943883d2dec99b34dd02078c1150493e56800b5e7a`  
		Last Modified: Thu, 09 Feb 2023 12:27:34 GMT  
		Size: 9.2 MB (9228126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a7be4264e22d81f1727f1d238e725bcec2452ff92a06d1353a114921801f911`  
		Last Modified: Thu, 09 Feb 2023 12:27:34 GMT  
		Size: 11.6 MB (11607645 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-curl` - linux; mips64le

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

### `buildpack-deps:unstable-curl` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:1003e1ec986fc94d376ba90c765b99538ab72dd44fe52a8a43371446a37680f4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.0 MB (75045000 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:35b26b4bc6ad1ecbe2b5f6263dcab3a9db03b5eb97630432406fda344a175d11`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 09 Feb 2023 06:22:13 GMT
ADD file:2c626d6b2dc96ed4051ff24603784037a34ea2aca8a2555baab15ec102b1f250 in / 
# Thu, 09 Feb 2023 06:22:16 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 12:30:19 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 12:30:34 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:bbf1522fb0b9e1d36e390546f20fa29b91e1fab7c915527df75f01bbcf172b2c`  
		Last Modified: Thu, 09 Feb 2023 06:28:56 GMT  
		Size: 53.2 MB (53247040 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0635828bd5bfeb3b339b41770bdc09a23b92382a15dfbf2d52d458b6eb76ea09`  
		Last Modified: Thu, 09 Feb 2023 12:40:38 GMT  
		Size: 9.6 MB (9629627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc219ebf76efb77244a7b932cc029b1d8c0a8582447c1c83b5951dbd0300b5c9`  
		Last Modified: Thu, 09 Feb 2023 12:40:38 GMT  
		Size: 12.2 MB (12168333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-curl` - linux; s390x

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
