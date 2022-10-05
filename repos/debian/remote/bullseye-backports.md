## `debian:bullseye-backports`

```console
$ docker pull debian@sha256:4411f5c899543f70c4bcb9063631fa661e7c1753b28120662e27d1487bebcce6
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
$ docker pull debian@sha256:5690fcb67e759dcf988c8b48aa27def8d677ab799c6537d008b060d4201cd3b0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **55.0 MB (55046475 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0b8401440673158dc9c4c3993fefc766a509572982bf179448fc88cd34c2d2dc`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:26:27 GMT
ADD file:d1268789456d2cdace6e50149e60404ad5a849b7c61e8fc8bc7b6e0eb6eeb7ca in / 
# Tue, 04 Oct 2022 23:26:27 GMT
CMD ["bash"]
# Tue, 04 Oct 2022 23:26:31 GMT
RUN echo 'deb http://deb.debian.org/debian bullseye-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:f606d8928ed378229f2460b94b504cca239fb906efc57acbdf9340bd298d5ddf`  
		Last Modified: Tue, 04 Oct 2022 23:30:27 GMT  
		Size: 55.0 MB (55046248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5cebba503380c9b43678ccfdc0d735ad42ef71fdcb84425e3259670accc18f6`  
		Last Modified: Tue, 04 Oct 2022 23:30:43 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:bullseye-backports` - linux; arm variant v5

```console
$ docker pull debian@sha256:2cc9fe0583e04de83a0d23ef9784d16442a259d47518d98babe0aa30a5ae3d09
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.5 MB (52547421 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b5483d59c5a23b20d84523cbb668633f9dd46e349fa077ba3fa80daf6f467e15`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:48:56 GMT
ADD file:e5a40ed79070e00490d94152874430cb225b3b00e8ca84eed2bf5fc8c0bd8155 in / 
# Tue, 04 Oct 2022 23:48:56 GMT
CMD ["bash"]
# Tue, 04 Oct 2022 23:49:03 GMT
RUN echo 'deb http://deb.debian.org/debian bullseye-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:5662b6ce27f2ffe436703124b1912c3225002537510f22d7c95f9a34c5ec19bb`  
		Last Modified: Tue, 04 Oct 2022 23:53:20 GMT  
		Size: 52.5 MB (52547199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:098fdc40de8b6cc08dda6bee291651148366ec0aecadaa8f7a8628ad2a56c4c3`  
		Last Modified: Tue, 04 Oct 2022 23:53:40 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:bullseye-backports` - linux; arm variant v7

```console
$ docker pull debian@sha256:c0c1465f0625b4b538ef7c72ca9c6168542e83df7c07899192e52cc5b8dacb9c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.2 MB (50209313 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a2406bcdf56ba61d48051546df49fc18baf80e3d93f9822dac882d2688d17074`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:58:28 GMT
ADD file:47a3f2948af18c39686ca59a88a439c25edaf286064d3a2ccc5dab47fee2fc52 in / 
# Tue, 04 Oct 2022 23:58:29 GMT
CMD ["bash"]
# Tue, 04 Oct 2022 23:58:36 GMT
RUN echo 'deb http://deb.debian.org/debian bullseye-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:e19342fb46cabf6147aec1d1c6af1f3a82736530cf3b067835fc8a09da092ce3`  
		Last Modified: Wed, 05 Oct 2022 00:04:36 GMT  
		Size: 50.2 MB (50209087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:485dbc56063010c53a5aeea3de25ee61bfc1448ce8f0a5f8e44f39a04247e4bc`  
		Last Modified: Wed, 05 Oct 2022 00:04:57 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:bullseye-backports` - linux; arm64 variant v8

```console
$ docker pull debian@sha256:421bcb39cf3597a945491b0613e3b0586830cb87d6358cc5b29fabd8597c267b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.7 MB (53700852 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b60836a486e3dedadd42c5eb6bc16cb708a106474a4cf4f4050efc797ad6e37d`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:44:26 GMT
ADD file:59bc45fad9cada77bf8e44ebdd982c7f6e575816b5ed6b7d1d8494faddd9b8b9 in / 
# Tue, 04 Oct 2022 23:44:27 GMT
CMD ["bash"]
# Tue, 04 Oct 2022 23:44:35 GMT
RUN echo 'deb http://deb.debian.org/debian bullseye-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:172730635f67c8f081f43275b390514bd8a05a4a7c3c467ae74ee42a029dce2b`  
		Last Modified: Tue, 04 Oct 2022 23:49:51 GMT  
		Size: 53.7 MB (53700625 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5cb4d1cc1c47818ba7b48d6f1654fcc01782df7c92ef4bc7522dc195036e24e`  
		Last Modified: Tue, 04 Oct 2022 23:50:10 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:bullseye-backports` - linux; 386

```console
$ docker pull debian@sha256:e345a26d0bb005531cebd9c61d8ed8d255b92717829bb75cefd94c1dfcbe458d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **56.0 MB (56024031 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:533d16b2b39f50deabc1ebf0ba61a0a619102ec31acd9bb5ec23b15cc04d5254`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:39:23 GMT
ADD file:4b457c51f15ab38743966e658d3174639e9eeae2719929bb637bb9a59a598d97 in / 
# Tue, 04 Oct 2022 23:39:24 GMT
CMD ["bash"]
# Tue, 04 Oct 2022 23:39:31 GMT
RUN echo 'deb http://deb.debian.org/debian bullseye-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:783379f2cdb66b4983dea0044fb0e139918a738a077f65fff29c85bb20119942`  
		Last Modified: Tue, 04 Oct 2022 23:45:03 GMT  
		Size: 56.0 MB (56023806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03446ab2d3a93e68fd3303d1ebad22441b967d14d3673e0a76bef1dc83ee8c94`  
		Last Modified: Tue, 04 Oct 2022 23:45:23 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:bullseye-backports` - linux; mips64le

```console
$ docker pull debian@sha256:d2767c0f822a56b642a28473fd2661cf29978271cd524530bfaf3b3ba1ae3e80
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.3 MB (53266064 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f5a2b43d1f610f244f69d1eadb4ee03af2e93fac8aaa767640b21a7622698eb0`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 05 Oct 2022 00:09:48 GMT
ADD file:ca40db2df3dbc600910b8cd139c564cf5b8bd6c1a06cc517cae2c1c05cff6dde in / 
# Wed, 05 Oct 2022 00:09:51 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 00:10:04 GMT
RUN echo 'deb http://deb.debian.org/debian bullseye-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:25bcd35faf05f859c3077f0e2e7010d24e56cdcfb77efbdeda236e47dc08e14a`  
		Last Modified: Wed, 05 Oct 2022 00:17:52 GMT  
		Size: 53.3 MB (53265834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:753a0f44f6a133163d3cffdecb076b58916b16b2bfe294b7d5a9d925b4b7e808`  
		Last Modified: Wed, 05 Oct 2022 00:18:10 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:bullseye-backports` - linux; ppc64le

```console
$ docker pull debian@sha256:a08ae989ab7e2137fdc7bc09523bb9c5145e535c2e5d3967fdddcdfae4d4ef7b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **58.9 MB (58917486 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:021e2846de4a47018b4e6d6ebfca090e0f55e3b6353017c0cd925481af943065`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:17:40 GMT
ADD file:74537fb4eedf6a0c9693fcdd0c9acb2797046cca66098b2e05d5c1a536a9aeda in / 
# Tue, 04 Oct 2022 23:17:43 GMT
CMD ["bash"]
# Tue, 04 Oct 2022 23:17:50 GMT
RUN echo 'deb http://deb.debian.org/debian bullseye-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:e05b86739fed11b3d0c5663063e627eebea0138239b30345630bc7e3f2549d5c`  
		Last Modified: Tue, 04 Oct 2022 23:23:34 GMT  
		Size: 58.9 MB (58917259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecd03a9e8c1d6b166f06d589cdf410461d1e8274acd83490e5e58b8778ec4055`  
		Last Modified: Tue, 04 Oct 2022 23:23:56 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:bullseye-backports` - linux; s390x

```console
$ docker pull debian@sha256:826fa50613129efb26746388853338d276bc4ac20425bf2810a5fc54270d0691
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.3 MB (53279960 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1276a01c37e3a1ff6e41d6024184b10164ecf8047b2b154be09626b25ec4e038`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:42:22 GMT
ADD file:fb9c2e517bc349a0e6677548de7dd78a3c392343ca80152fc08744efe4e1e38b in / 
# Tue, 04 Oct 2022 23:42:25 GMT
CMD ["bash"]
# Tue, 04 Oct 2022 23:42:33 GMT
RUN echo 'deb http://deb.debian.org/debian bullseye-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:ce03284d180c9b8801e9121eaf8daa52493209b61340c414b6b804b73ba5d1a4`  
		Last Modified: Tue, 04 Oct 2022 23:46:55 GMT  
		Size: 53.3 MB (53279735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5dfad01373d3d93d559b6cf27b53b0f11b69f6aabeef961dee68c8f2fcdbd2c`  
		Last Modified: Tue, 04 Oct 2022 23:47:08 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
