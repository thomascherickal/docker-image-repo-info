## `buildpack-deps:focal-scm`

```console
$ docker pull buildpack-deps@sha256:a04958925e45587b4c31763ad5ba0d8155406fde7f9c62d6cd79fa02cfadfe59
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `buildpack-deps:focal-scm` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:b878485ec2477b01b4f030e41259bcf75dfa7565e34da98cbcbcc72664f2e3c2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **100.7 MB (100696152 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7c77f89365fbb7f1cf52c8da0201f4eac537fc52a0f2c55779869f004598c8a6`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 06 Jun 2022 22:21:11 GMT
ADD file:00dae10e79b05c4e1a3db053a1f85a4f38a39fe85cbbd88d74201a01a7dd59b5 in / 
# Mon, 06 Jun 2022 22:21:12 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 02:07:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 02:07:59 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 07 Jun 2022 02:08:48 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:d7bfe07ed8476565a440c2113cc64d7c0409dba8ef761fb3ec019d7e6b5952df`  
		Last Modified: Wed, 01 Jun 2022 21:51:10 GMT  
		Size: 28.6 MB (28572632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a0b6a9c72470ff5d8860f27875472d3ad0d4b19051144f27660ad480b70c73c`  
		Last Modified: Tue, 07 Jun 2022 02:24:50 GMT  
		Size: 7.8 MB (7768843 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d27bf6512b10b479ce26a5fccce481830b0b356e00838901ed5d1d051119e3f6`  
		Last Modified: Tue, 07 Jun 2022 02:24:50 GMT  
		Size: 3.6 MB (3624431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bc5331f186f0258321175753c071842d764a2bb5d9ebfcfd39cbfb6b96bc9bd`  
		Last Modified: Tue, 07 Jun 2022 02:25:10 GMT  
		Size: 60.7 MB (60730246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:focal-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:88c5749222ea700efe8a89eaf8483681ac29d7a9cecadaf330e6b07ce7d7647c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **89.9 MB (89905791 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9467c963b0132c1a3b3fa57aa493f89a71527d0c0a412c43b0a04eb53da7ae8f`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 07 Jun 2022 05:50:50 GMT
ADD file:c95d34737ba1f11ac8b92be0125aad2baae46448f0d8ebd85ad69076006a3254 in / 
# Tue, 07 Jun 2022 05:50:51 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 08:58:32 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 08:58:47 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 07 Jun 2022 08:59:51 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:36754881d0ec0d456ee49776d62f6f0df47d29956ac7b2231b797e05780c6744`  
		Last Modified: Tue, 07 Jun 2022 05:55:05 GMT  
		Size: 24.6 MB (24592639 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45cec56ea7be37b7fa0ad5363a16f5a0a3bb7eb152d91e69b921e2962649948a`  
		Last Modified: Tue, 07 Jun 2022 09:21:24 GMT  
		Size: 6.8 MB (6762536 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24b6330d81e9773003d97c3a23e3bc9f4f886f97fed7b0715e6555164af3f0b6`  
		Last Modified: Tue, 07 Jun 2022 09:21:21 GMT  
		Size: 3.1 MB (3103860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89f193a62eb68251be57b0cf94d1788d3e2c7b54b9129d11943bb4fa7f26e14e`  
		Last Modified: Tue, 07 Jun 2022 09:22:15 GMT  
		Size: 55.4 MB (55446756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:focal-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:85378da8815d11885584c322944a4927ec4589bd2de4ae6945e3da4c4e1f990a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **99.0 MB (98988877 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:17c274bc78f3502a5b987c654b2ffef375e6fb0ce3d04a86334f82d35ce68cde`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 07 Jun 2022 01:25:15 GMT
ADD file:8bb0809a8ac8e978274cf731cff7529372088d22c5b0233a28f01ef414aefbca in / 
# Tue, 07 Jun 2022 01:25:16 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 04:44:40 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 04:44:49 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 07 Jun 2022 04:45:15 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:11e23ac719b33170b39b7e30b8027dc09c9cbad6b503b2b6b3ebbd9d33f4adad`  
		Last Modified: Thu, 02 Jun 2022 08:33:07 GMT  
		Size: 27.2 MB (27191210 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92092befe7351e6c3e1f8a95714dd641ca43c5394a906e063e98fd9c1346a83e`  
		Last Modified: Tue, 07 Jun 2022 04:54:58 GMT  
		Size: 7.6 MB (7635147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:710f2587d5ff9abda0e607cb269a207fc675f8d8a46ca00b30d0e7bd2d98dbc6`  
		Last Modified: Tue, 07 Jun 2022 04:54:57 GMT  
		Size: 3.4 MB (3386921 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41d74b682b23f88d8facd8dc68d39211f13d9de6dd1310f793e864849822e6be`  
		Last Modified: Tue, 07 Jun 2022 04:55:18 GMT  
		Size: 60.8 MB (60775599 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:focal-scm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:15310b8219a2872d7a7e7fb3182408e0b733cffe02c4365fa03e8d47e3a3be62
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **116.3 MB (116298219 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:881fb8ec687060226d21dffcd2ca2aa4a60c6f35ca70f7849f1aa7d314d7641f`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 07 Jun 2022 05:46:02 GMT
ADD file:86506a94b834ba2b6f10dc0d1955bee539be1cf565e4ccc2c4bc074e0375f115 in / 
# Tue, 07 Jun 2022 05:46:06 GMT
CMD ["bash"]
# Tue, 26 Jul 2022 22:39:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 26 Jul 2022 22:39:31 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 26 Jul 2022 23:06:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:3f52d061d2d3fdde0d3a099bbeae64080476c9650e9f3ba05de898d5bb5f03e8`  
		Last Modified: Tue, 07 Jun 2022 05:49:10 GMT  
		Size: 33.3 MB (33294345 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18349e42cb7ce91a943fbc86a6f7e492601f8eadea7475791a50b18ed0b9ba71`  
		Last Modified: Tue, 26 Jul 2022 23:55:25 GMT  
		Size: 8.7 MB (8719317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:954ef68d2e65b1a1eb4a527b2cc3d633d76aff137ee63ecfcdbb1cc9f986f4d1`  
		Last Modified: Tue, 26 Jul 2022 23:55:24 GMT  
		Size: 4.8 MB (4754804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac0a32faa32a8b78dc3fa911895e210633b01852fd3b8a7413b89758a863455e`  
		Last Modified: Tue, 26 Jul 2022 23:55:56 GMT  
		Size: 69.5 MB (69529753 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:focal-scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:56e4c1534c23743cd798d861a28fb2ded65020e9273bc4edd92c2cab85f000e8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **98.0 MB (98028256 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f1fddb608fb9f90d157dd8abc8ebe1658d6dfca5d1a11a6ea198b10e2fed9e15`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 07 Jun 2022 04:05:02 GMT
ADD file:6250f895d7d6c591cfe1b9fc991313d21b02167d94c67991db7c5c1c6814c51e in / 
# Tue, 07 Jun 2022 04:05:06 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 05:48:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 05:49:06 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 07 Jun 2022 05:50:07 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:2f1fac119b88f55cd8329458ec27c3d6d6cb324b0fe541feacfd9a4ee621a558`  
		Last Modified: Tue, 07 Jun 2022 04:07:45 GMT  
		Size: 27.1 MB (27056020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc54ecfe2f4b61591c55a270e245d426459887e4627d95ac90469391c974ae08`  
		Last Modified: Tue, 07 Jun 2022 06:07:12 GMT  
		Size: 7.4 MB (7416643 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c42b240f9c997122413533da099b86c7dcfabc8667a44b9dbc4911cd9cd19b81`  
		Last Modified: Tue, 07 Jun 2022 06:07:11 GMT  
		Size: 3.5 MB (3542577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2254bc597c3699bb036ed9c812c6e28ab1217923c92575d8ae7be3abeb7fcbb4`  
		Last Modified: Tue, 07 Jun 2022 06:07:28 GMT  
		Size: 60.0 MB (60013016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
