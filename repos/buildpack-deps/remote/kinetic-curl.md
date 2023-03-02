## `buildpack-deps:kinetic-curl`

```console
$ docker pull buildpack-deps@sha256:90955da3a53928299fa7a945b4072d569c0739bcce57a8472b481888082d4e99
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `buildpack-deps:kinetic-curl` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:c1bef77a747c1b0d0e2e1943063d242d97b14090c6fa5a4396872c2e5e86cd7f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.9 MB (37884733 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f070e17b881f324f200c61c5d2fbd431ae10cc95570becf16c69abab64af58b4`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 20 Feb 2023 11:43:07 GMT
ARG RELEASE
# Mon, 20 Feb 2023 11:43:07 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 20 Feb 2023 11:43:07 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 20 Feb 2023 11:43:07 GMT
LABEL org.opencontainers.image.version=22.10
# Mon, 20 Feb 2023 11:43:09 GMT
ADD file:18f562911635a03a9bf9e5fc22863fc2a78a64f7d35c7daa59f2d609b7ca055a in / 
# Mon, 20 Feb 2023 11:43:10 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 03:33:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 03:34:07 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:a10df61efde6b7f0cf3fbf848a5bed1c943a54e13566f30ef6a0cc6f259a2f33`  
		Last Modified: Thu, 02 Mar 2023 03:44:58 GMT  
		Size: 27.5 MB (27479398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6a9f9f71b0155b4b832dcb9bfbf542389507996cd93239b78300535c9421961`  
		Last Modified: Thu, 02 Mar 2023 03:44:55 GMT  
		Size: 6.8 MB (6770219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:710e0dcd6284a414a9f90e76d5555002980ba77c51b01d6a812e56d2c2d94d2e`  
		Last Modified: Thu, 02 Mar 2023 03:44:55 GMT  
		Size: 3.6 MB (3635116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:kinetic-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:b87d2b37a07f2b3373c8b775d1355e3139b302bd1713c89dcdbe11519b218229
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.6 MB (35635282 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d5d205c4c1777db2634384c44cf05affec171465def20dbcbf581b53881c97c8`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 20 Feb 2023 12:11:32 GMT
ARG RELEASE
# Mon, 20 Feb 2023 12:11:33 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 20 Feb 2023 12:11:33 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 20 Feb 2023 12:11:33 GMT
LABEL org.opencontainers.image.version=22.10
# Mon, 20 Feb 2023 12:11:42 GMT
ADD file:f77393d0d614b99f7ca8de09afc58a2e98d9d25c84c5ff69b50e94e7f191f7bb in / 
# Mon, 20 Feb 2023 12:11:43 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 11:43:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 11:43:51 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:e07337a9bc2a6220f565efbaf0abbba7718bb8478f0af5b255df655e98cacc06`  
		Last Modified: Thu, 02 Mar 2023 11:57:20 GMT  
		Size: 25.9 MB (25893079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f84854174ca4e4c0ad5221cd0bface3a62279cc1659c26e61319a54c79f28a32`  
		Last Modified: Thu, 02 Mar 2023 11:57:17 GMT  
		Size: 5.9 MB (5941095 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8dcf439bd51bffc866ae5a81a2764cc54c7f76949d34e14d2ef5666243a5c9e6`  
		Last Modified: Thu, 02 Mar 2023 11:57:17 GMT  
		Size: 3.8 MB (3801108 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:kinetic-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:3c113e07442a77b7e938f4bc9ef5b846f44b9cbbdc3cfc058ba264eb8738928d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.9 MB (36898999 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:caca0113519d729a4a7c61672a55b06acb176ea63c6920446e280ef75b4dca74`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 20 Feb 2023 11:58:05 GMT
ARG RELEASE
# Mon, 20 Feb 2023 11:58:05 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 20 Feb 2023 11:58:05 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 20 Feb 2023 11:58:05 GMT
LABEL org.opencontainers.image.version=22.10
# Mon, 20 Feb 2023 11:58:13 GMT
ADD file:7e756337f8554849df664b30203a26f6c39dc303e277292de31fd784b9ff471b in / 
# Mon, 20 Feb 2023 11:58:13 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 02:26:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 02:26:30 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:30762c7e5d854e6efb956328165eb8c43cbcf6c0be6766a45d3a13fc1e1f56d3`  
		Last Modified: Thu, 02 Mar 2023 02:38:12 GMT  
		Size: 26.7 MB (26699035 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42a3333370dc8d23b791b4a6098f7f5a10c7edf844266e90f4027f4e85981b72`  
		Last Modified: Thu, 02 Mar 2023 02:38:10 GMT  
		Size: 6.6 MB (6598072 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f663586508fee1a498937d0779dfdbae3bcdd16334d54ee9295ca50aae552925`  
		Last Modified: Thu, 02 Mar 2023 02:38:10 GMT  
		Size: 3.6 MB (3601892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:kinetic-curl` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:28895716799511a352dbc3b87633877569c448c91716b07fafceed861075e0ea
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.2 MB (44219918 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bb34ae855f68523ba0fb2c64a0473de1fc81baf2afdac185774fc659174ca56f`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 20 Feb 2023 11:56:23 GMT
ARG RELEASE
# Mon, 20 Feb 2023 11:56:23 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 20 Feb 2023 11:56:24 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 20 Feb 2023 11:56:24 GMT
LABEL org.opencontainers.image.version=22.10
# Mon, 20 Feb 2023 11:56:27 GMT
ADD file:541d2da8938972bd21842a8a4c8d2074a201f6f70eec4400110f90f1bc28f0e1 in / 
# Mon, 20 Feb 2023 11:56:27 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 03:37:28 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 03:37:56 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:afd8565abf9be19b25020425f0eef75bc6822497a915ac2ad7e299221258381b`  
		Last Modified: Thu, 02 Mar 2023 03:59:19 GMT  
		Size: 32.1 MB (32109672 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76c606979686591e3e15c259fedc8c72d14b5f5cb30789d4ac4fc1e7b2344079`  
		Last Modified: Thu, 02 Mar 2023 03:59:13 GMT  
		Size: 7.7 MB (7747700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec30e23fe35619983be2169d8e199c937a090ab1f2c783261d342664a3574b67`  
		Last Modified: Thu, 02 Mar 2023 03:59:12 GMT  
		Size: 4.4 MB (4362546 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:kinetic-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:b0150ef7049140aa70bbf29415a11063465c948a00c24d38fa2fbb671f63a581
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.1 MB (36116268 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:493a98847f6a760a3d453b6d316eb112b0f292f9513022c75fa6a97376df7fe4`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 20 Feb 2023 11:44:03 GMT
ARG RELEASE
# Mon, 20 Feb 2023 11:44:03 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 20 Feb 2023 11:44:03 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 20 Feb 2023 11:44:03 GMT
LABEL org.opencontainers.image.version=22.10
# Mon, 20 Feb 2023 11:44:05 GMT
ADD file:9d71356e3a29a835345254e233ddbd3a67941764476c2c7a5a2d0f8a61a84115 in / 
# Mon, 20 Feb 2023 11:44:05 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 02:13:22 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 02:13:32 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:8bcfec0e313701229d74107ece843bd247955551cd676760c2ab56d6fbf1b157`  
		Last Modified: Thu, 02 Mar 2023 02:24:05 GMT  
		Size: 26.0 MB (26029678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:741bf338192206d205e17575928e1ec37123b068da0fbfb2c33ff60198620f61`  
		Last Modified: Thu, 02 Mar 2023 02:23:59 GMT  
		Size: 6.5 MB (6461557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f19aa30c75a1427834711cd28f44ba117f910f7b5c4e50f923f34ea300cd0cd`  
		Last Modified: Thu, 02 Mar 2023 02:23:58 GMT  
		Size: 3.6 MB (3625033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
