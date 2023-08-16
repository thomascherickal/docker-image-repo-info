## `buildpack-deps:mantic-scm`

```console
$ docker pull buildpack-deps@sha256:54b98186614665cf884a24378777278a3601ca97609bd24fd164b42d662a056f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `buildpack-deps:mantic-scm` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:917c5ae7b60b328a63cecd4eb385e1f713f23098c90670f2293a967b9633093c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **86.4 MB (86426210 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:be5269e6bd4eb9dae1d4063ff31665600eef31956a07caf3e1813f1d2c08a755`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 01 Aug 2023 05:32:47 GMT
ARG RELEASE
# Tue, 01 Aug 2023 05:32:47 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 01 Aug 2023 05:32:47 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 01 Aug 2023 05:32:47 GMT
LABEL org.opencontainers.image.version=23.10
# Tue, 01 Aug 2023 05:32:49 GMT
ADD file:7d5373d4ccc5f70f68afa885a495329e33f2bf9f97a437251cfc79e7b85a1a88 in / 
# Tue, 01 Aug 2023 05:32:49 GMT
CMD ["/bin/bash"]
# Thu, 03 Aug 2023 03:33:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 03 Aug 2023 03:34:03 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:316675922a661ce4c35389bdeea6e9ec8d4708e41f08671b586c7aaea469b2c1`  
		Last Modified: Thu, 03 Aug 2023 03:40:24 GMT  
		Size: 27.9 MB (27857084 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07a7def12313ae9d69537ed1d4ea003f137f16c5789329735bfd447f8c86cfca`  
		Last Modified: Thu, 03 Aug 2023 03:40:22 GMT  
		Size: 13.8 MB (13783649 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:476103e20eaed817175054747eac1aeb5b843e57c0d9a11994cdf770c7fba77d`  
		Last Modified: Thu, 03 Aug 2023 03:40:39 GMT  
		Size: 44.8 MB (44785477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:mantic-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:b032b3221baceedc2a1e8e4454f2955d27c547a28abe95a3668336b99ada9a3a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **87.1 MB (87087351 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1b33abfeb555801fa1a398068626db7d9739c33c31dfd97ed7a8eb5e18c59702`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 07 Aug 2023 16:43:12 GMT
ARG RELEASE
# Mon, 07 Aug 2023 16:43:12 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 07 Aug 2023 16:43:12 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 07 Aug 2023 16:43:12 GMT
LABEL org.opencontainers.image.version=23.10
# Mon, 07 Aug 2023 16:43:20 GMT
ADD file:443a623a513d24fb17f92fecba92ab4b48c5cd58f4c71a4d1017f68cb28ed803 in / 
# Mon, 07 Aug 2023 16:43:20 GMT
CMD ["/bin/bash"]
# Wed, 16 Aug 2023 05:42:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 05:43:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:9a882830b71793138cc20048eb0866464a2a925cea19f5d96e75bef586f07b01`  
		Last Modified: Wed, 16 Aug 2023 05:52:57 GMT  
		Size: 25.5 MB (25451971 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c69c48a8564dd51e9033d498988912470fd0761ce0f5546103b27b81cf550ee6`  
		Last Modified: Wed, 16 Aug 2023 05:52:54 GMT  
		Size: 12.7 MB (12696492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59849160634729b9bd9592e9a03ab989ba30317f88c213629a7f24a45111cf44`  
		Last Modified: Wed, 16 Aug 2023 05:53:13 GMT  
		Size: 48.9 MB (48938888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:mantic-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:2c41c51b6ab982df780eae8161be6d38a64dcfa31eb5e1da76d36ac1df2f6bb2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **85.3 MB (85267114 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ac5e0c1c9ff336e4af720d7c08a9d1426f9825eb87fe1790baa88644d9a773da`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 07 Aug 2023 16:59:38 GMT
ARG RELEASE
# Mon, 07 Aug 2023 16:59:38 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 07 Aug 2023 16:59:39 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 07 Aug 2023 16:59:39 GMT
LABEL org.opencontainers.image.version=23.10
# Mon, 07 Aug 2023 16:59:47 GMT
ADD file:a621d5a90b1c5e05eb41dfa44616425f9e9c474acc76e148c36a525e99ff2bac in / 
# Mon, 07 Aug 2023 16:59:48 GMT
CMD ["/bin/bash"]
# Wed, 16 Aug 2023 01:33:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 01:34:17 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:4b4647be7125cb643de6d0a75158905d697da4afc1e9edcd35dbb27a43edf604`  
		Last Modified: Wed, 16 Aug 2023 01:42:51 GMT  
		Size: 27.3 MB (27266349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14f74bc0fb029a079dcd558844cc26c5973e7ec9efc2db4555c60ab536a1a11f`  
		Last Modified: Wed, 16 Aug 2023 01:42:49 GMT  
		Size: 13.4 MB (13369802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7156641b60d58d063ba957dec8ada8f9f2a4052eae760ec0c791b84480868de1`  
		Last Modified: Wed, 16 Aug 2023 01:43:05 GMT  
		Size: 44.6 MB (44630963 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:mantic-scm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:fd0eae220e0953f1e8f6db015f3819e7a0a745b01bb1d8e0c6cc7cc06b878fa7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **97.7 MB (97670522 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6f6f57f844a17257f7bc458e8bd3b32b7ee6f2093e6627869cf392d633985d30`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 07 Aug 2023 16:57:20 GMT
ARG RELEASE
# Mon, 07 Aug 2023 16:57:20 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 07 Aug 2023 16:57:20 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 07 Aug 2023 16:57:20 GMT
LABEL org.opencontainers.image.version=23.10
# Mon, 07 Aug 2023 16:57:23 GMT
ADD file:4cb180718bb451f8c264f3c3ca17e21c2f353537e1350e7285186274e7c13aa1 in / 
# Mon, 07 Aug 2023 16:57:23 GMT
CMD ["/bin/bash"]
# Wed, 16 Aug 2023 02:01:44 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 02:02:53 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:fdf3d625c5c62f16c8647b6f71fb3627aa49027d553c24dfb5bb5fe384576e06`  
		Last Modified: Wed, 16 Aug 2023 02:16:46 GMT  
		Size: 32.2 MB (32220285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4266d044f5749871179995f4d16bfab0f930c8a7fc456be89d9dde4ff53c9a04`  
		Last Modified: Wed, 16 Aug 2023 02:16:42 GMT  
		Size: 15.9 MB (15897836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a546e021bdd3317f25b6399220a698c011a5ef8050a924b3d8d5e67bdc99f46a`  
		Last Modified: Wed, 16 Aug 2023 02:17:11 GMT  
		Size: 49.6 MB (49552401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:mantic-scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:b8945d029070bc2a1c8a5d326be4e11613a9ab1f1a90a15688e4ea12ce0fef12
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **85.9 MB (85857799 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d3591f1b927603a4a8b5d31122d54e999416e2ff7d66fe57d05e051a2124c6c8`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 07 Aug 2023 16:41:40 GMT
ARG RELEASE
# Mon, 07 Aug 2023 16:41:40 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 07 Aug 2023 16:41:40 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 07 Aug 2023 16:41:40 GMT
LABEL org.opencontainers.image.version=23.10
# Mon, 07 Aug 2023 16:41:42 GMT
ADD file:7038e8b287279d65872808b33572bb449a981ceacdc4533e8e1047544044f524 in / 
# Mon, 07 Aug 2023 16:41:42 GMT
CMD ["/bin/bash"]
# Wed, 16 Aug 2023 04:32:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 04:32:39 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:6e4b480e7bad6fd35ac328034bc72b280c0019028bc95dd0dbf78d168750430e`  
		Last Modified: Wed, 16 Aug 2023 04:39:53 GMT  
		Size: 26.9 MB (26884397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44867c9f8a414f35f7e550468ffda8aadf82a61ad02779247fe2d748d28e5390`  
		Last Modified: Wed, 16 Aug 2023 04:39:51 GMT  
		Size: 14.2 MB (14158805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e837d29076d6daa1f70750605bd3c0d36bced4e25e6e7f34c8bc4360af79e30`  
		Last Modified: Wed, 16 Aug 2023 04:40:06 GMT  
		Size: 44.8 MB (44814597 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
