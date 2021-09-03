## `debian:bullseye-backports`

```console
$ docker pull debian@sha256:c0d655c70bba5f99d9dd0c2f8cd54692537df9a6ad6f746032d41cea9cd91041
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
$ docker pull debian@sha256:291352de18a215e3cb46fcebc11ade6adbf383956b5454a545025f3e1d9dbfbc
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **54.9 MB (54927099 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ec4f03747c2745c8677ef5c89c4415736335bc7a579a41dfdfbfbb703c4d3ccf`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 03 Sep 2021 01:21:07 GMT
ADD file:1fedf68870782f1b44cd50691444aab4061cc0c70f24e5fabe9c562cc46eb9af in / 
# Fri, 03 Sep 2021 01:21:08 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 01:21:12 GMT
RUN echo 'deb http://deb.debian.org/debian bullseye-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:955615a668ce169f8a1443fc6b6e6215f43fe0babfb4790712a2d3171f34d366`  
		Last Modified: Fri, 03 Sep 2021 01:26:55 GMT  
		Size: 54.9 MB (54926871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a27274c8f3a5b765b521997d9103831059dd152e9612644b8e39005a95a6eea9`  
		Last Modified: Fri, 03 Sep 2021 01:27:13 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:bullseye-backports` - linux; arm variant v5

```console
$ docker pull debian@sha256:0dad1a478a358b41f36bc63e0994d5c36d6eee7c8ca08f286f9339a9b5a1054d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.5 MB (52461725 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8ee906ea20ddd142228103a379ba397ef5e67cd9f7f5459957159d16b8b978b9`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 03 Sep 2021 00:49:54 GMT
ADD file:1e667a7a6266f0b2af7a4c7638575e79c77fb7cdbe2034cc4673d83fe7251899 in / 
# Fri, 03 Sep 2021 00:49:56 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 00:50:11 GMT
RUN echo 'deb http://deb.debian.org/debian bullseye-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:f6dc2bdd42eeff7d4a88d4ace72cf9281d77232183d6919b4c3162051e654910`  
		Last Modified: Fri, 03 Sep 2021 01:04:48 GMT  
		Size: 52.5 MB (52461500 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bed7c7c9c25eb41b33c2ec31d16fe83e01ec1ec1937ca84f8018f4aeb9bb432f`  
		Last Modified: Fri, 03 Sep 2021 01:05:12 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:bullseye-backports` - linux; arm variant v7

```console
$ docker pull debian@sha256:9c15269da08360fa0d9db36bdd025942cc0a114c26ba22a4d88fd73f3c6ba7ca
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.1 MB (50127484 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5b4c14fd93ecb5b0c3f8484fc8286230956d4307bde4cb8d5a72dcd818323247`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 03 Sep 2021 00:59:03 GMT
ADD file:a885b024f19da3fff424486fd5495eaae458dea6a1038715198e0449b6b00518 in / 
# Fri, 03 Sep 2021 00:59:04 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 00:59:20 GMT
RUN echo 'deb http://deb.debian.org/debian bullseye-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:ff8c004d0dc8a6ef263acdc2f23760be64e46bb9a75384a950f29b2c5d8b5c98`  
		Last Modified: Fri, 03 Sep 2021 01:14:05 GMT  
		Size: 50.1 MB (50127257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f14679cf1b24c68ed091445cf858d97b62f9779f9cd1918f95eae6755163b85`  
		Last Modified: Fri, 03 Sep 2021 01:14:30 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:bullseye-backports` - linux; arm64 variant v8

```console
$ docker pull debian@sha256:daf1f24b70a8b3c5292b072627cf34cba0889c8a960a30f2c0429f4bcbffdd0b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.6 MB (53613282 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:98949ffbaadfc21dbe5d64548b93d639c896b295fd1e04b543df1a07973ccdad`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 03 Sep 2021 00:40:18 GMT
ADD file:0b1ff9dcb90d6b787179d2e43ca534c39e0372227a3af198bab158a89fb2c966 in / 
# Fri, 03 Sep 2021 00:40:19 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 00:40:26 GMT
RUN echo 'deb http://deb.debian.org/debian bullseye-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:ffacddc51d82196acb1d49f2e3c13601fc16c61c995a860b450d23b000353ca1`  
		Last Modified: Fri, 03 Sep 2021 00:48:17 GMT  
		Size: 53.6 MB (53613054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fa7825321dc3c5909bf00ec88f7243212e489355341781b16d9e96ccfd83ea3`  
		Last Modified: Fri, 03 Sep 2021 00:48:38 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:bullseye-backports` - linux; 386

```console
$ docker pull debian@sha256:932007f1bf0e0c6b41ee2fd154e440050ad8050546b602a03e5834a8ea874654
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **55.9 MB (55931161 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:970b31c6e4065566b93feef034740e3b81334f8009b8343d14ad53124256e79a`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 03 Sep 2021 00:39:34 GMT
ADD file:fcade9a23463d6b59cfafb811fd21f2143d482e21ea836e9c2e4796136459599 in / 
# Fri, 03 Sep 2021 00:39:35 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 00:39:42 GMT
RUN echo 'deb http://deb.debian.org/debian bullseye-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:a62297bd75cc0ee79a641136889da30fb39e2d05074874bd1d73ebe2edb6f8d7`  
		Last Modified: Fri, 03 Sep 2021 00:47:28 GMT  
		Size: 55.9 MB (55930933 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5eacc3f7c100760eddd7ddb9f00e2318cd2a7c00bf128e5cf36d299aeb5b27a`  
		Last Modified: Fri, 03 Sep 2021 00:47:50 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:bullseye-backports` - linux; mips64le

```console
$ docker pull debian@sha256:26d53dbd2adf124e644ae90a6148923f71bee0188f7758850f28ce721ea4ec28
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.2 MB (53177456 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:78d4f20931546949eb99f8b2092b9ac1f9f3752ff9d33bf7d76b2cd59cff5be8`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 03 Sep 2021 01:09:38 GMT
ADD file:aaed6c610924ac8eb3eb6be97263abde763b266a7057c9a6b5bbf8c481ddb348 in / 
# Fri, 03 Sep 2021 01:09:39 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 01:09:44 GMT
RUN echo 'deb http://deb.debian.org/debian bullseye-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:47d27042240b42cf414701e6bb0ab3bbf22fdf98f796e21e982bdc39dfcbfff4`  
		Last Modified: Fri, 03 Sep 2021 01:17:39 GMT  
		Size: 53.2 MB (53177233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02985f1587045e3df8d66dc6b3eb75e5da3598b25f055d04581453add12661e8`  
		Last Modified: Fri, 03 Sep 2021 01:17:57 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:bullseye-backports` - linux; ppc64le

```console
$ docker pull debian@sha256:fb866c97f9f9a14deb4f9ce33d0d2d2412a954041ae99339f8d4afb797024b86
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **58.8 MB (58819661 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:97cb20e3a8b193c742dc4fd6ee7531f3254be626f3fc4bd973aac52842ff9c12`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 03 Sep 2021 01:22:22 GMT
ADD file:3d1033153ba97e1c4e4f513c14db9d9f913ee4c4ce2eeb554bcaf6c5c9665c80 in / 
# Fri, 03 Sep 2021 01:22:35 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 01:22:56 GMT
RUN echo 'deb http://deb.debian.org/debian bullseye-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:5180655d8cc68420b0aa96b7c8db9131c02ad0ca93c166dffc9a3a49b22005c2`  
		Last Modified: Fri, 03 Sep 2021 01:35:56 GMT  
		Size: 58.8 MB (58819434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bb86e4144f884b8beaa24436c2083e1476457877dc8cd08b6cea44470ae0d0c`  
		Last Modified: Fri, 03 Sep 2021 01:36:18 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:bullseye-backports` - linux; s390x

```console
$ docker pull debian@sha256:18dff9ca2c7d0e437b15aa146bd71db766c3d3491ac9f5683f933a3ca14891a7
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.2 MB (53201381 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d4de8497e6d100a6b1e2635d32baa525567cc99633b0dbf513e32adc6d7430e4`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 03 Sep 2021 00:43:14 GMT
ADD file:fe20239b717a5727a4629774155356432b5a2535dc21ce2df2ee00314b48132f in / 
# Fri, 03 Sep 2021 00:43:22 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 00:43:33 GMT
RUN echo 'deb http://deb.debian.org/debian bullseye-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:440698b773ccf4480ce07124f15edd8dc6e88ddec22635fb3aa782759f4696b8`  
		Last Modified: Fri, 03 Sep 2021 00:52:28 GMT  
		Size: 53.2 MB (53201154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f59267f2144200229c707edaf6e438fb181c4e8ab4c7ee147cd14acbd977361d`  
		Last Modified: Fri, 03 Sep 2021 00:52:48 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
