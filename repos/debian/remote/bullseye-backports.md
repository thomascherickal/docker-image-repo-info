## `debian:bullseye-backports`

```console
$ docker pull debian@sha256:6831db1e2968113d201d56b70a7f48a82679b176172603be5079b6731f244cec
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
$ docker pull debian@sha256:79d862c303a8c285472d35ef21a2dbc3ad9a72e4cc619049702bd078a5151532
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **55.1 MB (55055797 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c8fb10ce7f5a6f73c1d2fd36463783be8a97a58369608f814195a75e19259f15`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 27 Jul 2023 23:24:55 GMT
ADD file:b493776b6d91132ce50735e2d82076620774a1e0a690cf96777ddd6b85f513ef in / 
# Thu, 27 Jul 2023 23:24:55 GMT
CMD ["bash"]
# Thu, 27 Jul 2023 23:24:59 GMT
RUN echo 'deb http://deb.debian.org/debian bullseye-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:9a9e034800a1747ea288f38f6087c036acac99dd3ec5255bf7798abd8c23a304`  
		Last Modified: Thu, 27 Jul 2023 23:29:45 GMT  
		Size: 55.1 MB (55055571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:689c5e5496a993e5929515c02005f15ae4c5b8769e8f601b812db37facc84cdc`  
		Last Modified: Thu, 27 Jul 2023 23:29:57 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:bullseye-backports` - linux; arm variant v5

```console
$ docker pull debian@sha256:458d49a537bdea36b9d93e39f5176966a6d9e8f0ace107a163587db54ba91f73
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.6 MB (52558358 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c846818ea480fed11b86d179ff10a210c48b9b3f6caf71947d8fbe0c5d7116d8`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 15 Aug 2023 23:48:40 GMT
ADD file:d044e64aab907424be649252b5ff1d9f5e8c9494db5b60c0e54f5962bfb73478 in / 
# Tue, 15 Aug 2023 23:48:40 GMT
CMD ["bash"]
# Tue, 15 Aug 2023 23:48:43 GMT
RUN echo 'deb http://deb.debian.org/debian bullseye-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:0b63bbf2e6f6026dfaed9cbedf777472a04812b7d291501b1d416e49e3ce885e`  
		Last Modified: Tue, 15 Aug 2023 23:51:54 GMT  
		Size: 52.6 MB (52558130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76ed972dcf768d79ea214885479652118dde820681d8f215ff515e8bcc5e05d0`  
		Last Modified: Tue, 15 Aug 2023 23:52:06 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:bullseye-backports` - linux; arm variant v7

```console
$ docker pull debian@sha256:be6c32177750a4e5f2a6012749760fb37208eca7fa890023f51720457719f147
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.2 MB (50219722 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8ec72da80d2786898b1c2a70c78bf6e10c9666fac7334eba4d55872410644380`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 16 Aug 2023 00:17:21 GMT
ADD file:b529de8b48c1e507ad6f29320c3c5cd83d8d06fa66e8d89bb62faff62700e9f2 in / 
# Wed, 16 Aug 2023 00:17:22 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 00:17:25 GMT
RUN echo 'deb http://deb.debian.org/debian bullseye-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:c53151c23650f086e15d3652b8a931fb4623765c0112e8adc74eb8853c8c9232`  
		Last Modified: Wed, 16 Aug 2023 00:21:46 GMT  
		Size: 50.2 MB (50219496 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef85287085d5d2e9f166a9b1a21859a7de8cbb3180a7bcfc9ac312c25c8b845c`  
		Last Modified: Wed, 16 Aug 2023 00:21:59 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:bullseye-backports` - linux; arm64 variant v8

```console
$ docker pull debian@sha256:84790e7b8cce5f965a387f677b28596b12725562cfce077d86ab26b021a95531
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.7 MB (53705004 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ddd740fa6283f98531c840c46200af0ab0806a0f2ea2a33caf46b096bf76f01d`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 15 Aug 2023 23:40:03 GMT
ADD file:8973cddb2d84a543b71001635599951bea6485a3526ae4ff916443b584864c83 in / 
# Tue, 15 Aug 2023 23:40:04 GMT
CMD ["bash"]
# Tue, 15 Aug 2023 23:40:06 GMT
RUN echo 'deb http://deb.debian.org/debian bullseye-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:e837d9f05c625de5b814b851adbc03559ba02ea7078f57c81a01e18fc65bf42b`  
		Last Modified: Tue, 15 Aug 2023 23:43:37 GMT  
		Size: 53.7 MB (53704779 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0b932f4b110190e63603d08b867acb4cbe6a38388d0e005a3b015d7ebee9c3d`  
		Last Modified: Tue, 15 Aug 2023 23:43:50 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:bullseye-backports` - linux; 386

```console
$ docker pull debian@sha256:123e16c17b3c1eee93d6266eb06ba5e8f9790dee96c644b5f3cc1203425ee5e2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **56.0 MB (56040745 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:12d6ecf422f320ca7b48d77ab5b19ad64c3bd1d4f1c01ae8672321eac3fbc79b`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 15 Aug 2023 23:39:11 GMT
ADD file:efc88a19b31e68ca41f555bcc51338b0f135cbbd72b90637d8c73969d53addd2 in / 
# Tue, 15 Aug 2023 23:39:12 GMT
CMD ["bash"]
# Tue, 15 Aug 2023 23:39:16 GMT
RUN echo 'deb http://deb.debian.org/debian bullseye-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:822e033fa7b169545d5890de01438a9dd87774ff938ff440e823a3ec3f73996d`  
		Last Modified: Tue, 15 Aug 2023 23:43:47 GMT  
		Size: 56.0 MB (56040520 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fc2fe42b0e9a26ad377ea6baa5e2dfa1baddf1c93f41d376f5b1e8bec48cdd6`  
		Last Modified: Tue, 15 Aug 2023 23:44:00 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:bullseye-backports` - linux; mips64le

```console
$ docker pull debian@sha256:fc912db366d6c68c1272d7f6b25b2fc59dd87b283d144e7afa3f1e3f1fc61b3b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.3 MB (53271791 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b0cdfa4524eec2e9edb9a918bc287ebae072af48a1aa9dd05d69a033dcb07394`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 16 Aug 2023 00:09:18 GMT
ADD file:c0b984cd41325dc5f83fb228f8b95bd38027d8860098ac574a960400eaf0d976 in / 
# Wed, 16 Aug 2023 00:09:23 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 00:09:36 GMT
RUN echo 'deb http://deb.debian.org/debian bullseye-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:4a039678eb41cc8e7dbd73bbab533513108157d96943588a97c7fac7c940eaca`  
		Last Modified: Wed, 16 Aug 2023 00:20:18 GMT  
		Size: 53.3 MB (53271564 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f6857354ce38787ec4c5624de1352fde3fbce8bbd075cc668aaa7377aa284b3`  
		Last Modified: Wed, 16 Aug 2023 00:20:33 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:bullseye-backports` - linux; ppc64le

```console
$ docker pull debian@sha256:5555ff3a3e69c608c9df67081440e7fe4872b068f25c6b4bb03031e444658cba
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **58.9 MB (58927689 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:55744a08d8f1c4bf663226bbde4f0e49064f72e024dc9313f8ad30d2056007e6`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 27 Jul 2023 23:23:20 GMT
ADD file:c9c051b70d4b5c059dc4dfc25c2ce056efb99058bbea4911c346eaf8c90ea938 in / 
# Thu, 27 Jul 2023 23:23:23 GMT
CMD ["bash"]
# Thu, 27 Jul 2023 23:23:29 GMT
RUN echo 'deb http://deb.debian.org/debian bullseye-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:ba7a048f0d1295609b34eb062a51486e1f3e5831711b4569a3583b1e8ad30aff`  
		Last Modified: Thu, 27 Jul 2023 23:29:55 GMT  
		Size: 58.9 MB (58927464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0aed5c3ef5b2c2c64c715f268aa40b2a8833a63278901ab0d4fcaa497df6fcf4`  
		Last Modified: Thu, 27 Jul 2023 23:30:16 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:bullseye-backports` - linux; s390x

```console
$ docker pull debian@sha256:d6cb9084545aa4fc460e26cfe167062bb4893185529e2ec7d6fd9f65c90fb511
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.3 MB (53290868 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0b3cd499a4bc06dc62a198ccdece237bfb02f677b1a2902bee6786db4562ff5a`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 15 Aug 2023 23:42:43 GMT
ADD file:021ebd89eb6b326058b4fc3aeca5d0d93925ed29a443618fedef034618e8f2db in / 
# Tue, 15 Aug 2023 23:42:48 GMT
CMD ["bash"]
# Tue, 15 Aug 2023 23:42:54 GMT
RUN echo 'deb http://deb.debian.org/debian bullseye-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:cf9beb6f1941863d1df3b7a9c4f925894662762a3ceeba920f164d9e8c8bab57`  
		Last Modified: Tue, 15 Aug 2023 23:48:07 GMT  
		Size: 53.3 MB (53290642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f845b7fb8b3daa9998e5465d601bf060be9cc9350c28f140ae7843312c83e0d`  
		Last Modified: Tue, 15 Aug 2023 23:48:15 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
