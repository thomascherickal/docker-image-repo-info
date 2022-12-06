## `buildpack-deps:bookworm-curl`

```console
$ docker pull buildpack-deps@sha256:35d58f9c3b6efa67986c5bbaf50af401c5f0d060a5b7bf99203203811f0e1e07
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
$ docker pull buildpack-deps@sha256:e8e8d02047936e3f0f5976738c11d2dd8298b995d945f4f0684163f722ebef41
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.7 MB (70687856 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4cad875972408cb17a9c8eaf7cf91c92a602b593162a152024a99d39ec1a365c`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 15 Nov 2022 04:04:23 GMT
ADD file:7d616c027c138495879d0578d333124a7a41f161d38339949eae9fc46a97bafc in / 
# Tue, 15 Nov 2022 04:04:23 GMT
CMD ["bash"]
# Tue, 15 Nov 2022 10:21:03 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 10:21:13 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:6e44dba964a0f1646d06ab7f617603ef51c645dd641b4ce74411770449b003f3`  
		Last Modified: Tue, 15 Nov 2022 04:07:53 GMT  
		Size: 50.3 MB (50297005 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65df78b7eb3f0a3cb19c3e7e1eee5c5f93e45ff73ff9fa0a57ea8d5bbf289837`  
		Last Modified: Tue, 15 Nov 2022 10:30:32 GMT  
		Size: 9.0 MB (9017903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df801fdaea384702a5d171a41a11d9e52f28f2ef21d2c34c289602d6933bfc14`  
		Last Modified: Tue, 15 Nov 2022 10:30:32 GMT  
		Size: 11.4 MB (11372948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm-curl` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:425efa0c6e88e4b9b33f158ae8d1e6b2f01c472bf26a22e3d7efc668f3b1ced0
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.8 MB (68763017 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2f99a41e9121b4cf98a9d22083053ab22eb76f5e92dc879d86a5571519d38580`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 15 Nov 2022 01:48:32 GMT
ADD file:f5954c36a3601d3dcf67f8701fe7691c7a94bc36e88827c06ff7338a52d56c5f in / 
# Tue, 15 Nov 2022 01:48:34 GMT
CMD ["bash"]
# Tue, 15 Nov 2022 05:38:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 05:39:01 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:34757784ba8ccecfd4a2f549aff99cd98b7b291a61176def51827463bc77aa00`  
		Last Modified: Tue, 15 Nov 2022 01:53:14 GMT  
		Size: 49.3 MB (49265841 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf55f2cf20315f11c0568b2c8e64fa08c08d44cd3c2ed5e281caebe13320c93c`  
		Last Modified: Tue, 15 Nov 2022 05:47:05 GMT  
		Size: 8.5 MB (8471441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9889ed4552e2f48445b3ae801a3f6bf662eac23614471014335840669c23ecf4`  
		Last Modified: Tue, 15 Nov 2022 05:47:06 GMT  
		Size: 11.0 MB (11025735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:ae032576b7bca0d4dbcd2d1afa615eae72b2d41ff4ea6fef32fe41879df59f12
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **65.9 MB (65858234 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:57bef20d1ea1ff3116cceecdced5c9614640844295d6d28df7fb462fc99bf73b`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 15 Nov 2022 03:42:37 GMT
ADD file:7196c14a33cd1774b746a830598de6b6368174bf15faa83c36c244a6e27938fc in / 
# Tue, 15 Nov 2022 03:42:38 GMT
CMD ["bash"]
# Tue, 15 Nov 2022 12:15:30 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 12:15:38 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:192a2a7ee5b2cd81557e51320bddd5cf2b318283cd7f7c0c0998525448fcf94a`  
		Last Modified: Tue, 15 Nov 2022 03:49:02 GMT  
		Size: 47.1 MB (47088370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbf2f82dd6bc5c9f45ea459022b7744bc671cdbbf0e4a75b81f8f7806c95bec9`  
		Last Modified: Tue, 15 Nov 2022 12:27:19 GMT  
		Size: 8.1 MB (8119764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a83154b6af543fb7c117afa8a800dcc4616a91acfe5de9000b91948e1dbd258`  
		Last Modified: Tue, 15 Nov 2022 12:27:19 GMT  
		Size: 10.7 MB (10650100 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:0013fff71d6010807d1e884d6a397805a6345216ce0e1bd47aa0324d952a5118
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.5 MB (70484312 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4515c15470d800fc5987489fbcee049119e3a6fa45ff44d87ad8c7ebffb86ed8`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 06 Dec 2022 01:39:50 GMT
ADD file:de3ed89259c63b45a553c11db2206a6ca4201bfd264f04890af2c672736c15b4 in / 
# Tue, 06 Dec 2022 01:39:50 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 02:02:45 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 06 Dec 2022 02:02:52 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:6d78ccc24e38e1c539440b7f90d65e136bba8366864c2b4a45e3956272709049`  
		Last Modified: Tue, 06 Dec 2022 01:43:02 GMT  
		Size: 50.3 MB (50307715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bb26845d7157ae0fdc105d1666dd413b3f1236876c9e38fe497d4b566c5b8a0`  
		Last Modified: Tue, 06 Dec 2022 02:10:56 GMT  
		Size: 8.9 MB (8851114 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aee48d89e1a98c15d782346793fdaba61be0e798358172b68670681463bdd69f`  
		Last Modified: Tue, 06 Dec 2022 02:10:56 GMT  
		Size: 11.3 MB (11325483 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm-curl` - linux; 386

```console
$ docker pull buildpack-deps@sha256:8d5fa6d85d1f5df8f8c7d8253ed9c8296d352e48e9d780cec70d454fc70f12df
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.1 MB (72058952 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f2b86fdcd6d324de17f304a77d442a0882677f97eefad5d51a8affd980858972`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 06 Dec 2022 01:38:43 GMT
ADD file:6064ead20e3d5415784fcb74157c3ba1b90982f542deb132e9dabb2a1712e396 in / 
# Tue, 06 Dec 2022 01:38:44 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 02:05:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 06 Dec 2022 02:05:30 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:45070d389a5ecd4dae6cdcb3e06567c8481416cfb2efb085e318fb5e2d11393b`  
		Last Modified: Tue, 06 Dec 2022 01:44:36 GMT  
		Size: 51.3 MB (51301574 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efe8313be6a60f2abeebcfad5a2e4539e7d4b28618e0b019908926dd39c9c1bd`  
		Last Modified: Tue, 06 Dec 2022 02:14:11 GMT  
		Size: 9.2 MB (9196657 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7aa4a90125b538cbb0d87c8c0d37737cdc01ed561a27c8ecfae4cc4f708aecc3`  
		Last Modified: Tue, 06 Dec 2022 02:14:11 GMT  
		Size: 11.6 MB (11560721 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm-curl` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:723920e9fe8b53aeebd05a15aace50f1dc7a20f4858a75b515a93d799833e59a
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.8 MB (69830488 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d698d505b85e9c0e232b0ea7109aa41798a4c0e38ded5b435a7abe4429d340c5`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 15 Nov 2022 04:11:59 GMT
ADD file:0d439a2fdede63b0646f17fe0578b4ebab24012a35c93e6e63e5c511ccce8fe7 in / 
# Tue, 15 Nov 2022 04:12:04 GMT
CMD ["bash"]
# Wed, 16 Nov 2022 02:02:29 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 16 Nov 2022 02:03:12 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:52449a481885eb7aca2b2fbb088c8d233a6249a8aaaf65e32f8c268ad8340850`  
		Last Modified: Tue, 15 Nov 2022 04:19:19 GMT  
		Size: 50.3 MB (50314192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72d29bbc0f4e1684560d462982ab292feb495140fdd75d13e6826460b19d90c0`  
		Last Modified: Wed, 16 Nov 2022 02:27:31 GMT  
		Size: 8.4 MB (8383819 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:232356f6f3990a119f67b1a72642482a16966341b02a7f077b08d38e1d12852a`  
		Last Modified: Wed, 16 Nov 2022 02:27:31 GMT  
		Size: 11.1 MB (11132477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm-curl` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:88a2d219394341b68d4f5921259c07905cbd095262c5ad9a83ac787ea172d4b1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.1 MB (76086639 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2c73cd50f13a80ab70e487962fc0beaff1aadb0dd9b7a085a13e0acc64db4882`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 15 Nov 2022 05:17:43 GMT
ADD file:b13da8e7ee4f9b71f42de64cf2dfe92a09d9d6be3537a8b151db32013e632fb4 in / 
# Tue, 15 Nov 2022 05:17:45 GMT
CMD ["bash"]
# Tue, 15 Nov 2022 11:51:37 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 11:51:59 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:24f3e6cef4f753f77f6e0b5b4e73cf7a7fdbfa85b11f29916d1d4fe28bee544c`  
		Last Modified: Tue, 15 Nov 2022 05:22:58 GMT  
		Size: 54.4 MB (54360800 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e462c1bdfc268a97c6033242cd34635559a926155991efd84c30d93ce39ce6ee`  
		Last Modified: Tue, 15 Nov 2022 12:06:33 GMT  
		Size: 9.6 MB (9596802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:970a93fcc7e991ae16e04be69f70dc91326e712c64e700b5ee5a6a3f14bb797f`  
		Last Modified: Tue, 15 Nov 2022 12:06:34 GMT  
		Size: 12.1 MB (12129037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:036132d70a14cbfa3a43131ccfc091d033c3f8cb8988e2773a64162221998275
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.5 MB (68544375 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7290f812fc20133b9d55535b8cd6775dcd6a1dfb5213570652e779f20bea521e`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 06 Dec 2022 01:41:45 GMT
ADD file:45186e2067a128e8dbf3558a97cd5853548faaf7c2bb93ef1544ed66907fcf19 in / 
# Tue, 06 Dec 2022 01:41:55 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 02:06:39 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 06 Dec 2022 02:06:48 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:effa21bde36181862f20d53853fc03e36421f6a13d6aad41051d593fe9c7c097`  
		Last Modified: Tue, 06 Dec 2022 01:47:58 GMT  
		Size: 48.7 MB (48664905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67f5dcd56007991a3866c8b0bf2ee7220f18a57fb48ff74112e6c810f63c8b96`  
		Last Modified: Tue, 06 Dec 2022 02:18:52 GMT  
		Size: 8.7 MB (8652754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1216521a137ae490612192a50d936077fcb94da6292a8ef16485599b92a5ace`  
		Last Modified: Tue, 06 Dec 2022 02:18:51 GMT  
		Size: 11.2 MB (11226716 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
