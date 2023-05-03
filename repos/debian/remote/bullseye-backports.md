## `debian:bullseye-backports`

```console
$ docker pull debian@sha256:89a23ddc374aebb52f6245c7e50532d57a90bf4aab7bb51a4b1a1c5f6a93d9e4
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

### `debian:bullseye-backports` - linux; amd64

```console
$ docker pull debian@sha256:5320fd979eb4c96e378a017e6b3aa9e1c271c31b0feb54263d620b6ced390126
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **55.0 MB (55049294 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8f8b31fdb72a124b4741af0508d3609e89b27c47d3443a69d216510abb3f55ba`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 May 2023 23:46:50 GMT
ADD file:fc290cf8ddb984325474583faa79c5a98c5ea0ec7f606bf360251f63acecf389 in / 
# Tue, 02 May 2023 23:46:51 GMT
CMD ["bash"]
# Tue, 02 May 2023 23:46:53 GMT
RUN echo 'deb http://deb.debian.org/debian bullseye-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:918547b9432687b1e1d238e82dc1e0ea0b736aafbf3c402eea98c6db81a9cb65`  
		Last Modified: Tue, 02 May 2023 23:49:58 GMT  
		Size: 55.0 MB (55049070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c20a442c07b2d1ef8a2d6e43f8b2694fc76ec6ae356eb5530a83ef0147f7f73d`  
		Last Modified: Tue, 02 May 2023 23:50:12 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:bullseye-backports` - linux; arm variant v5

```console
$ docker pull debian@sha256:eb6d3e1e4d0e1f835be420b48a537a82f367827db57a89698f834581fae9c363
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.5 MB (52546757 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e9f13fee9ad9733a747fc6bad922bf7125275767d91b5fcbd65057e24ca7357e`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 May 2023 22:48:45 GMT
ADD file:e5816cf9c67a55e94065100a95ed3b269817a643b21e5b9c060bfde394a56889 in / 
# Tue, 02 May 2023 22:48:46 GMT
CMD ["bash"]
# Tue, 02 May 2023 22:48:48 GMT
RUN echo 'deb http://deb.debian.org/debian bullseye-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:a091ba323f94f60ffce46d1dad6471927a6d7136843d7bbc29ede769d6cafd86`  
		Last Modified: Tue, 02 May 2023 22:51:00 GMT  
		Size: 52.5 MB (52546533 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1827544a6fedf0f8c24aa3074567b30472563d25dfc99582e13dc3bfa2bfa793`  
		Last Modified: Tue, 02 May 2023 22:51:15 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:bullseye-backports` - linux; arm variant v7

```console
$ docker pull debian@sha256:0a17da44e9c2d6a340c2b28bd34b52e93c32c1d05fdcd090ecef734825bf3dc8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.2 MB (50210236 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:04dc023dbd1fe56f4a7e9e99c6b5ab2226b6e6c55675666fed1f6d425892ac4f`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 May 2023 23:47:46 GMT
ADD file:668ced72eb3825a6cfd123f77fed6c64b8ad5bf1f4aa8e78ede9512198ca65ad in / 
# Tue, 02 May 2023 23:47:47 GMT
CMD ["bash"]
# Tue, 02 May 2023 23:47:50 GMT
RUN echo 'deb http://deb.debian.org/debian bullseye-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:755944445ece6eac276e067f465680b57daac59a0ed9ce97e7c501f1cde8621d`  
		Last Modified: Tue, 02 May 2023 23:51:06 GMT  
		Size: 50.2 MB (50210011 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7b1661ce98e636a5e7da29c778e83db7ee6651f477d46a47983745be1f1c265`  
		Last Modified: Tue, 02 May 2023 23:51:20 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:bullseye-backports` - linux; arm64 variant v8

```console
$ docker pull debian@sha256:86838e91ca789545652661438246d81bb883f5bb618cd20a282240621872ff53
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.7 MB (53692931 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:45145202ca284a9bd8184bdede3347606c0c96c804cd683a66bf226674f872a3`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 03 May 2023 00:22:41 GMT
ADD file:f930fdb659332a615b0042ca415d6d7feda9ba6b2f58222e3e5bbed326db4d40 in / 
# Wed, 03 May 2023 00:22:42 GMT
CMD ["bash"]
# Wed, 03 May 2023 00:22:43 GMT
RUN echo 'deb http://deb.debian.org/debian bullseye-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:d677c78be691f8dcbe9d44ce576b97ad205b3dd78557dc62794e59eb19553ee9`  
		Last Modified: Wed, 03 May 2023 00:25:31 GMT  
		Size: 53.7 MB (53692705 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c06c003979169cb4957280fd3eca056d3b58b7ce5197d81f3c5ac20172b7ccb`  
		Last Modified: Wed, 03 May 2023 00:25:44 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:bullseye-backports` - linux; 386

```console
$ docker pull debian@sha256:33a7b0fca7e924c7bffadcb0391ef078cd91c4f7d66cfefdf0e5e41e01e57713
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **56.0 MB (56029374 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8d39be9500a9bb9311dca835c59321eeea4772cee01ee8a585b27112b39c8f43`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 03 May 2023 00:00:45 GMT
ADD file:59d53253d7691be0330c735eb4b57791a8fc5894572d3deaeb7138cce45132ad in / 
# Wed, 03 May 2023 00:00:46 GMT
CMD ["bash"]
# Wed, 03 May 2023 00:00:48 GMT
RUN echo 'deb http://deb.debian.org/debian bullseye-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:6ac0eb37fce5e6fca952bf804df5de5ebb63724d4d44bf23abc5d5736ee32afd`  
		Last Modified: Wed, 03 May 2023 00:04:44 GMT  
		Size: 56.0 MB (56029150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af74f5c4c9e145ac1d2936abeaaeb65877015685f5dd7da0d0302e8d0b7f0d4a`  
		Last Modified: Wed, 03 May 2023 00:04:59 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:bullseye-backports` - linux; mips64le

```console
$ docker pull debian@sha256:d1336044808ee2fe114bef743784c3cfed912cb4e6ecdebe626cf56d78868d87
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.3 MB (53261359 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0b100e28b75897ac0daad52057a5ab01135ad664177903b6f78053ba82eb8503`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 May 2023 23:49:00 GMT
ADD file:578ecc56a9b7fe8d8ebea195fcf6c3a8d78941e9c4b5da71f8b4b821b6db9f87 in / 
# Tue, 02 May 2023 23:49:06 GMT
CMD ["bash"]
# Tue, 02 May 2023 23:49:22 GMT
RUN echo 'deb http://deb.debian.org/debian bullseye-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:4753f7ffbf9149ce1d9cc543018c00a2946e14c08b1a2aa37a0ac347d08b0e29`  
		Last Modified: Tue, 02 May 2023 23:57:30 GMT  
		Size: 53.3 MB (53261131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1437d2fb81cba00a03595c2471d13d8481ecefeb8b403aec0cc6dc85a6bae1b`  
		Last Modified: Tue, 02 May 2023 23:57:46 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:bullseye-backports` - linux; ppc64le

```console
$ docker pull debian@sha256:edbc2c6605b0ffbf00fc77f11af79f65586b4e730bbf11eeaad076701bafb1b1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **58.9 MB (58924229 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f9bec496c7213f1bdc6334610cf6201be989acff1657a259b049ddbc9bf96b4a`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 03 May 2023 00:31:28 GMT
ADD file:39e4cb0fbb759c45690e34c0392acb89ac2b180e261843426f24ce0fe0189e84 in / 
# Wed, 03 May 2023 00:31:32 GMT
CMD ["bash"]
# Wed, 03 May 2023 00:31:35 GMT
RUN echo 'deb http://deb.debian.org/debian bullseye-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:0c356fc795c1bdfb3883bd87c64008fffdc0d8bdc8f0ecb386016a31fe5864fb`  
		Last Modified: Wed, 03 May 2023 00:36:26 GMT  
		Size: 58.9 MB (58924002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb190c4019caa63e5d3f950e96633a25a2e9ac21c04df2e566fdc5c672538b03`  
		Last Modified: Wed, 03 May 2023 00:36:41 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:bullseye-backports` - linux; s390x

```console
$ docker pull debian@sha256:0e4c0a91f063aa664e5393b1c602a2121fef4fdc1b375e6bac354961019eb77c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.3 MB (53286910 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d55d666fcb5965f2338b94392975cb40f61b7a40d568169be8f119d160f5bca9`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 12 Apr 2023 00:00:25 GMT
ADD file:ab4e28724d04724a57e0f5bbe299d3361103f05ad1978dc3bfef243c1f9d6476 in / 
# Wed, 12 Apr 2023 00:00:38 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 00:00:48 GMT
RUN echo 'deb http://deb.debian.org/debian bullseye-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:042263756d7dc47bf98a243871107aa3a2b41acda91d104d8b4e148749a43dda`  
		Last Modified: Wed, 12 Apr 2023 00:05:03 GMT  
		Size: 53.3 MB (53286682 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a5f8ea362068477a4e1f3dc8e71b20734f89fdc76fa216834c78d37b4ff337c`  
		Last Modified: Wed, 12 Apr 2023 00:05:11 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
