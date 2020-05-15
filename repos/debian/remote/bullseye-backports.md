## `debian:bullseye-backports`

```console
$ docker pull debian@sha256:b55a88fc2f86cd5bef7965fa6e13969d65d13dc15f10552d1abf396b7c30fc64
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

### `debian:bullseye-backports` - linux; amd64

```console
$ docker pull debian@sha256:89bd208f0be1e5b4d45b230a431970500d4dd13337b25d996b8b5a18412728dc
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.4 MB (51384897 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:39c3a2368694cd1987c948bc62aecc1478e2707e9893a27343782a971ed00700`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 13 May 2020 21:19:45 GMT
ADD file:19778292422b784c4eb17d79e7632fc1e3619b6bbbcf16a37bb6179a5c725b1b in / 
# Wed, 13 May 2020 21:19:45 GMT
CMD ["bash"]
# Wed, 13 May 2020 21:19:50 GMT
RUN echo 'deb http://deb.debian.org/debian bullseye-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:5ce4ab219a2f8bc551eb2502df5b719a1d8a32c4bbb00b3629001ebb6c5e0b94`  
		Last Modified: Wed, 13 May 2020 21:25:41 GMT  
		Size: 51.4 MB (51384672 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d7a681fe7de81db24d1c2f9d25fde2335bea22c03c3bbadd95de2ad27a56351`  
		Last Modified: Wed, 13 May 2020 21:25:46 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:bullseye-backports` - linux; arm variant v5

```console
$ docker pull debian@sha256:d49bd1b6c4171e640aca312bf2bc59ef77775734d3c6c635317d180c2c1d8d0e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.4 MB (49359681 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8e664c05825383d9ee33e76b45778d34e49cd526fcd46a23a9baba98fc79e90e`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 14 May 2020 22:36:28 GMT
ADD file:099743a0547d5c892b4a3daaa3fc0f05d8317cd4946a0e9508d130ee56db63bb in / 
# Thu, 14 May 2020 22:36:31 GMT
CMD ["bash"]
# Thu, 14 May 2020 22:36:51 GMT
RUN echo 'deb http://deb.debian.org/debian bullseye-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:0238daf30887e241cdd1334fa6bd5883d06738c7ff61cea1b32a3361de098564`  
		Last Modified: Thu, 14 May 2020 22:45:51 GMT  
		Size: 49.4 MB (49359451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8acfc86e3e47661a16a75cdcc5fe6e6d55e2aaa8e04c4e90d362db66dcb1efa8`  
		Last Modified: Thu, 14 May 2020 22:45:57 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:bullseye-backports` - linux; arm variant v7

```console
$ docker pull debian@sha256:68e45b5abca06aa7358bf2a815069a59031eeaf06c5a57ebba9d7ee7c3d5875b
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.2 MB (47161743 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9d67c6373ab1740c60397c841e977c661510e0d93d1c2e2d48ccb8ba131527fb`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 15 May 2020 00:58:28 GMT
ADD file:c0d2fe9468c0056452ba2eba677a3cfb1318edf3174c0106a65ec1c5608f130f in / 
# Fri, 15 May 2020 00:58:30 GMT
CMD ["bash"]
# Fri, 15 May 2020 00:58:44 GMT
RUN echo 'deb http://deb.debian.org/debian bullseye-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:add59fdfc3a148d6f3bc80c671fa82b62aebfbe6f2ed783df08b083fb9497d23`  
		Last Modified: Fri, 15 May 2020 01:10:22 GMT  
		Size: 47.2 MB (47161514 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ab01a664acccf5cf9c82b6805d5ae1e020807deccdc3448bf181881f845bd5c`  
		Last Modified: Fri, 15 May 2020 01:10:27 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:bullseye-backports` - linux; arm64 variant v8

```console
$ docker pull debian@sha256:e1005cde49b55bfdc9a31cad56d930fd5e340557bc3bed7bea3daf1889ba1dfd
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.3 MB (50328576 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7fbbc05dc1eca4101a4ef3e6203961862cd2850bd37ea4184c827d5f7f2fef7e`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 13 May 2020 21:41:52 GMT
ADD file:642f1f8b3928c38913b91b5770e5ef77e0467db31d0e7342848c66b97b0cefce in / 
# Wed, 13 May 2020 21:41:58 GMT
CMD ["bash"]
# Wed, 13 May 2020 21:42:09 GMT
RUN echo 'deb http://deb.debian.org/debian bullseye-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:da14fdea4bf7eaa36b82ecde9ee461379c7eb32fac279c7d1bce1452edd5bf2f`  
		Last Modified: Wed, 13 May 2020 21:52:10 GMT  
		Size: 50.3 MB (50328349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:923c69d83df3727a59d8835cc1a3a6db0025055b0ed52605a969e97b495ce517`  
		Last Modified: Wed, 13 May 2020 21:52:18 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:bullseye-backports` - linux; 386

```console
$ docker pull debian@sha256:d611eb5aa10e6d569766ea9e10cdab7f85ce23ba58a0c6587b319b0b9f96ad8f
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.5 MB (52480516 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5fd6bcf576e6431c44683413ac58b52df3e8e98c1faeb536c656c4fbf078a434`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 13 May 2020 21:38:36 GMT
ADD file:ad345e25a8b64e5d96a8875a8c7eceb747745ed11d495c0de132b2a33e48e29d in / 
# Wed, 13 May 2020 21:38:36 GMT
CMD ["bash"]
# Wed, 13 May 2020 21:38:40 GMT
RUN echo 'deb http://deb.debian.org/debian bullseye-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:424ac85ac099fddf73c8eff4a7e1e7a3ad318011cb2070285233ed10f3794d6f`  
		Last Modified: Wed, 13 May 2020 21:44:40 GMT  
		Size: 52.5 MB (52480291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72db658a9f62738c0c7202ce229cd25db9280a54bfe9155873469016d7ab7195`  
		Last Modified: Wed, 13 May 2020 21:44:45 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:bullseye-backports` - linux; mips64le

```console
$ docker pull debian@sha256:0e6de8b7a303b9c4b5692c236a91604b2f99f92983c44ef14c5a42be4b72153b
```

-	Docker Version: 19.03.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.1 MB (50132074 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a1d663aaeb925727fad69791f0e77fd40789558e9eecc0b523b5f7de77b94f85`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 15 May 2020 04:46:53 GMT
ADD file:fcf688b002e58dbfd2392e8a30b0ad1975c59c068b68c9d846430ce0f63eb390 in / 
# Fri, 15 May 2020 04:46:54 GMT
CMD ["bash"]
# Fri, 15 May 2020 04:47:02 GMT
RUN echo 'deb http://deb.debian.org/debian bullseye-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:dcbeba28f7aa4ae28ec4e38f90ddc68bb34f71bf49e3361203df2f569876774f`  
		Last Modified: Fri, 15 May 2020 04:55:03 GMT  
		Size: 50.1 MB (50131847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28446ae99ab0344521ea041cede59fec0c20dc9b5b8151d7879ee2e415dc17c4`  
		Last Modified: Fri, 15 May 2020 04:55:14 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:bullseye-backports` - linux; ppc64le

```console
$ docker pull debian@sha256:3080b899be804460da55b5bd777765dfc0a31b6221ad4568f244f5503bd8e543
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **55.1 MB (55110533 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9c53439de43895b437da4777bb06c9dff92dce145a2e7377a3ff0172f361a42f`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 13 May 2020 22:16:05 GMT
ADD file:890f814706ea242af3d8f4b729aed7d590611deabe25d4adae7468f0058d7a4c in / 
# Wed, 13 May 2020 22:16:10 GMT
CMD ["bash"]
# Wed, 13 May 2020 22:16:37 GMT
RUN echo 'deb http://deb.debian.org/debian bullseye-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:f2f9956082054d1fabd5ea1a9e08b145fa7f68b93b5601b36e05386466487664`  
		Last Modified: Wed, 13 May 2020 22:56:07 GMT  
		Size: 55.1 MB (55110307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58f77ca2a9766d1f5d88bd48a7548fcee222279fd5f8fed9730df2c099275274`  
		Last Modified: Wed, 13 May 2020 22:56:17 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:bullseye-backports` - linux; s390x

```console
$ docker pull debian@sha256:39a7026f68a3dd3fa3c88abd6c9908da53b4c351cb1470e47ed3cac83948d2d2
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.0 MB (50002845 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3129230cbbb89090a1efa80ab70827431fb291f4e2799597fb76f7510f2be891`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 14 May 2020 23:05:50 GMT
ADD file:56a2d8bf46ec4edd3d768966ad8e9b4c86561cbcd482ae49fc18cc34306d54fb in / 
# Thu, 14 May 2020 23:05:53 GMT
CMD ["bash"]
# Thu, 14 May 2020 23:05:57 GMT
RUN echo 'deb http://deb.debian.org/debian bullseye-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:f0cbd757e4d594cf3793c18e1f7d5d6f3fd983ea05bd2edeac4774c47e85b763`  
		Last Modified: Thu, 14 May 2020 23:10:41 GMT  
		Size: 50.0 MB (50002620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f52b71dff1221ed98ccb19cbc66280c35ee80db2dccb6476488285fcef3d70aa`  
		Last Modified: Thu, 14 May 2020 23:10:46 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
