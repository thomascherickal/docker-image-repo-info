## `buildpack-deps:stable-curl`

```console
$ docker pull buildpack-deps@sha256:5d7c4674dc305af10397ad88412a729b25a980c277a978036c5f3806dc080d94
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; mips64le
	-	linux; ppc64le
	-	linux; s390x

### `buildpack-deps:stable-curl` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:3242617e6dcf3959f790ddfdd0850e7e2b7a1bb77c6cf676ea915a2f53356aed
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.3 MB (68263337 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7fb36daa10c51edfd8409a2ce0d0b10790a973a83c5ebd6b3abd96e9cabac2aa`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 12 May 2021 01:21:03 GMT
ADD file:1a1eae7a82c66d673971436ce2605e97d107e2934b7cdec876c64923ae6f4f85 in / 
# Wed, 12 May 2021 01:21:03 GMT
CMD ["bash"]
# Wed, 12 May 2021 01:55:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 01:55:55 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:d960726af2bec62a87ceb07182f7b94c47be03909077e23d8226658f80b47f87`  
		Last Modified: Wed, 12 May 2021 01:26:49 GMT  
		Size: 50.4 MB (50433242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8d62473a22dec9ffef056b2017968a9dc484c8f836fb6d79f46980b309e9138`  
		Last Modified: Wed, 12 May 2021 02:04:42 GMT  
		Size: 7.8 MB (7832938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8962bc0fad55b13afedfeb6ad5cb06fd065461cf3e1ae4e7aeae5eeb17b179df`  
		Last Modified: Wed, 12 May 2021 02:04:42 GMT  
		Size: 10.0 MB (9997157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stable-curl` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:01084f5c8f25210d629f58785dfe84f6a9d91b747d8067cf528eeae3ae96f1b3
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **65.2 MB (65214956 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0aeac83c00649d1dfca20d094da18ba7d4ec6f30d6716ed5d58bbaae58acb077`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 12 May 2021 00:54:57 GMT
ADD file:443be99157e29a4ccb29f5d0ffc9994ce41fb51c512815f76fec9e1fb4d5d8ba in / 
# Wed, 12 May 2021 00:55:00 GMT
CMD ["bash"]
# Wed, 12 May 2021 02:28:15 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 02:28:41 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:db69af0c9ce605b61ac30d118d6c6ab4f8579b8c80e5469335f2108afa5d2c66`  
		Last Modified: Wed, 12 May 2021 01:09:52 GMT  
		Size: 48.2 MB (48150747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b47203fcc2d787900c2b29557537f54bfb4736cf95aeb1da72a4eb38afe48002`  
		Last Modified: Wed, 12 May 2021 02:46:08 GMT  
		Size: 7.4 MB (7376669 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8503ed6a21cfbc9d6bdac105da9df47ae10adf0aca8c5a0156725d84e6802879`  
		Last Modified: Wed, 12 May 2021 02:46:08 GMT  
		Size: 9.7 MB (9687540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stable-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:ef563ad676ad388264eb569abc896f371bf8659dbe03164e5fd146611baeb6ae
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.4 MB (62384892 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:11df73c4dbf7c437d17ca046698e11c44ba78102345157e3ddc959f1e281a86d`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 12 May 2021 01:02:10 GMT
ADD file:51a0472692adf18117444dc1f35d6eb3b4d6d672f28a7f6631f9d5d269b0b85d in / 
# Wed, 12 May 2021 01:02:15 GMT
CMD ["bash"]
# Thu, 27 May 2021 00:40:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 27 May 2021 00:40:15 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:89475607b1df9fc7eec7efe2fa845738a16cee3e92c1bb864c1f5a93b8303bc6`  
		Last Modified: Wed, 12 May 2021 01:18:49 GMT  
		Size: 45.9 MB (45916922 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88447de5eb3eca4a1d96b6980b44d82ac19d121f6b77b826989f8d611fd001b0`  
		Last Modified: Thu, 27 May 2021 01:03:02 GMT  
		Size: 7.1 MB (7124249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b25b14665fd0185f2f3b90a8d1825fc8ef9f330e1aea452f60fd70cdcfe99bf4`  
		Last Modified: Thu, 27 May 2021 01:03:02 GMT  
		Size: 9.3 MB (9343721 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stable-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:1d3b6626b73cb1c01a9a016a18369f74280872c954860a3d19d1009d4e86f58b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.9 MB (66904751 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:314f5d175bbe868cef588608b3741c8dd2d8e5e2adbd0d829a623ae63ffdaa18`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 12 May 2021 00:50:48 GMT
ADD file:ff9983cd659b3fc32ddfbbdeda76a971afd7d399e6d8b98faea3a9ead0e598f6 in / 
# Wed, 12 May 2021 00:50:52 GMT
CMD ["bash"]
# Wed, 12 May 2021 01:34:08 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 01:34:20 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:c54d9402d498e45ed396b5b6fe836f55e4ccadbad745decda3e9f83d880bc677`  
		Last Modified: Wed, 12 May 2021 01:01:40 GMT  
		Size: 49.2 MB (49225351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a91bbb3592d6685d1c683c8c20e60901274c636605800608685274c194d43d25`  
		Last Modified: Wed, 12 May 2021 01:48:24 GMT  
		Size: 7.7 MB (7695057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08d8c28b9129321858810cff4cd78385949579ed18d991f98c77f912c7a754f8`  
		Last Modified: Wed, 12 May 2021 01:48:24 GMT  
		Size: 10.0 MB (9984343 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stable-curl` - linux; 386

```console
$ docker pull buildpack-deps@sha256:d23653eec3442e1b5953f25d93fa68256f0c4976e8688267322ee12eca05933d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.5 MB (69538385 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4c9f4706e929e09aed1cacf4a212f26406e7cf0c5de5861f8f93b12d34c6e258`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 12 May 2021 00:39:33 GMT
ADD file:f823eb487fd44688b29f866d2c837da27f508db7fc1f19e4dc01dde9ea7c72c4 in / 
# Wed, 12 May 2021 00:39:34 GMT
CMD ["bash"]
# Wed, 12 May 2021 01:09:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 01:09:20 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:07a4b6b1756691e1f8a89eb64afc18fb9b4a0712eb810679a4b89b1b351f8e9b`  
		Last Modified: Wed, 12 May 2021 00:46:03 GMT  
		Size: 51.2 MB (51200034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5eb2395b55871bdaf1f7143048f77c63000ab6412664b1ce49fe9a8602e496d1`  
		Last Modified: Wed, 12 May 2021 01:17:52 GMT  
		Size: 8.0 MB (7998534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:106083f164cc6c516cf3c838e5ba0c6870172a26217bd766dac43b0ecc89ca3b`  
		Last Modified: Wed, 12 May 2021 01:17:53 GMT  
		Size: 10.3 MB (10339817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stable-curl` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:886d9e8347185eb516f7ab48281973d90b050326888ef3ca5f5696f28932f3fd
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.4 MB (66350651 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:76c2916bf63a31d180528aef6e9dc5106a8c0eef17970fa71d594359e0c8cd64`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 12 May 2021 01:09:17 GMT
ADD file:2e2c1e52b19e85e4299309ed75f088e727e316902a0dd39be198c41ced817b01 in / 
# Wed, 12 May 2021 01:09:18 GMT
CMD ["bash"]
# Wed, 12 May 2021 01:58:38 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 01:58:53 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:6e18ab78f0b7ce048045ffb547791aaa698db3869d1da87f71e538a7fd19f965`  
		Last Modified: Wed, 12 May 2021 01:15:53 GMT  
		Size: 49.1 MB (49081826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03651915a251d4aae832ea26b7e72a8d93c3b7bde9b9b309c4069e8de71798fe`  
		Last Modified: Wed, 12 May 2021 02:09:54 GMT  
		Size: 7.3 MB (7252462 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fc21a03fe417b31a222d86e092660202cc0fae5556a43581e06b7d6a7ae1849`  
		Last Modified: Wed, 12 May 2021 02:09:54 GMT  
		Size: 10.0 MB (10016363 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stable-curl` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:3ff9a4e26b6f2c2f60828f6e45fc2148a89c86a66d608116950491f0552236f3
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.2 MB (73179692 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bd24b7054edea5bff2ada4eeb08e81c221ff23fbaed425615573b1c4d65e5876`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 12 May 2021 01:34:15 GMT
ADD file:b714397b44737108500b0256abc9750626cfa28cc0bb52623b9a14bb0e2345fc in / 
# Wed, 12 May 2021 01:34:24 GMT
CMD ["bash"]
# Wed, 12 May 2021 03:37:00 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 03:37:38 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:bd4ac1330adf594df6c60d33ec5060c79833a8455e6cdb9f5ef2be33cb843845`  
		Last Modified: Wed, 12 May 2021 01:43:19 GMT  
		Size: 54.2 MB (54180124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdb8ec8ba72b4c906c6a3b88324130a605cfda687a94ed75e901c7cd141492fb`  
		Last Modified: Wed, 12 May 2021 04:19:32 GMT  
		Size: 8.3 MB (8271865 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46415d7d07194b30fe4845342dd9c5927deb73698c2cfe9a55c6417b98ed3855`  
		Last Modified: Wed, 12 May 2021 04:19:32 GMT  
		Size: 10.7 MB (10727703 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stable-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:68665defdd7af4a1a74cbf1fef67772af78bc2ff06e0b6aabc60a0be025da165
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.3 MB (66284789 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:acf51040d47db01e03060d91c4fb56a5ef9ba62b7311f5ff206c021373fdda38`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 12 May 2021 00:43:13 GMT
ADD file:ffd730820ba7e4874e61b094cd8b1b19e272722efa2f96b6c2c0518882aa8010 in / 
# Wed, 12 May 2021 00:43:21 GMT
CMD ["bash"]
# Wed, 12 May 2021 02:24:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 02:24:24 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:03edb521c4b9db23cdd0bda14609ccca13d11f4c37cd9ca16173028e6d3647df`  
		Last Modified: Wed, 12 May 2021 00:47:45 GMT  
		Size: 49.0 MB (49000941 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f34f82527bf298856cf45773644d350eef4edbbc31c0abda7c268dfbe472c46e`  
		Last Modified: Wed, 12 May 2021 02:34:40 GMT  
		Size: 7.4 MB (7400573 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7314687ab69ade4e94423968ff75eb3a6f047e5e53aae12aef126aab10da1d3c`  
		Last Modified: Wed, 12 May 2021 02:34:40 GMT  
		Size: 9.9 MB (9883275 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
