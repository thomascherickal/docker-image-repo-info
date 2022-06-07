## `buildpack-deps:focal-scm`

```console
$ docker pull buildpack-deps@sha256:ec0621a5545d2ec11dd0b952ca443c9eaf85acfb2d207f536ccb5254f7342d2a
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
$ docker pull buildpack-deps@sha256:6f0a40882a2e7fda131cf855b58f17748c4c2209b29b833c44a9fae9c4496b9d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **89.4 MB (89387301 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:16e939222556781f115fa3e71a72021581a12faa85c1d9deb4cd9faf135d8466`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 29 Apr 2022 22:58:46 GMT
ADD file:5f12bea85a1ebe365907ca3979b0e31e6043dccfcb9a3cdf62be46e054494147 in / 
# Fri, 29 Apr 2022 22:58:47 GMT
CMD ["bash"]
# Fri, 29 Apr 2022 23:27:28 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 29 Apr 2022 23:27:43 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 29 Apr 2022 23:28:44 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b20724a4297c7ca8b89f31d6ad53e7ead0c17c7908a4592871cdc97332193580`  
		Last Modified: Fri, 29 Apr 2022 23:03:00 GMT  
		Size: 24.1 MB (24073650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a1563a0a8b5e832769a2de291e460a7fcacd9bee37ad7a2d8a73b14a0f0ddfc`  
		Last Modified: Fri, 29 Apr 2022 23:46:30 GMT  
		Size: 6.8 MB (6762469 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:493cef317c1c6766357569ceb016cc5074fdef707c8caf5a67a543cd3f49f167`  
		Last Modified: Fri, 29 Apr 2022 23:46:27 GMT  
		Size: 3.1 MB (3104192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2aaaed45380a5a8e10619db9bee81a02afc8c18a5b05750eb6b438db9b180461`  
		Last Modified: Fri, 29 Apr 2022 23:47:21 GMT  
		Size: 55.4 MB (55446990 bytes)  
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
$ docker pull buildpack-deps@sha256:94843bd8f5164db55d341ce94f5e5f82cf2f9190dd19e59e4b4f5182ba409db3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.9 MB (115889134 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4ca0ee88877ec92b46b6741deae3f2a1192aa2418c65cdf7076d463c86e12d71`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 29 Apr 2022 23:22:28 GMT
ADD file:55691ac7d76af0fcfafc39ebd1e5a4f2d7018147d6db6f89812db33fbaffc2f9 in / 
# Fri, 29 Apr 2022 23:22:33 GMT
CMD ["bash"]
# Sat, 30 Apr 2022 00:03:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 00:03:47 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 30 Apr 2022 00:05:07 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e9c0a77cb9f0f7330e3fc62254e4c8ae89ed4bba21209fdc1088195250f950b9`  
		Last Modified: Fri, 29 Apr 2022 23:25:23 GMT  
		Size: 33.3 MB (33290661 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52152a0de6e46d74b97d1c4aa354df39f45b928545e3b3cfd5562aec916b61a2`  
		Last Modified: Sat, 30 Apr 2022 00:26:15 GMT  
		Size: 8.7 MB (8722859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d7e0fa1464e2cd697c14ed00b03cfae9577e44abba441afa9930519b611d1da`  
		Last Modified: Sat, 30 Apr 2022 00:26:13 GMT  
		Size: 4.5 MB (4456217 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af186f438c091a97a62b0923300630e559cef87a617df0381966dc2178cde764`  
		Last Modified: Sat, 30 Apr 2022 00:26:41 GMT  
		Size: 69.4 MB (69419397 bytes)  
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
