## `buildpack-deps:kinetic-scm`

```console
$ docker pull buildpack-deps@sha256:b0e53314b314ebf0ffb12bb21dd7d20a6a45fca68be9c9775074c8769779be87
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `buildpack-deps:kinetic-scm` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:047a981c3c4d581bea16d7a0cd289b348dfa07629f24b6cc7f6add1dcc94d1aa
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **77.6 MB (77624743 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8bc182bbb00ba8809b6ffb1c35841b67fd97eba00c6901a88c09dde29acd761f`
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
# Thu, 02 Mar 2023 03:34:49 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
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
	-	`sha256:09c20cf6be4d508b2c166988b50c5ae18cead28e74cf5a620d56202faabfe64a`  
		Last Modified: Thu, 02 Mar 2023 03:45:14 GMT  
		Size: 39.7 MB (39740010 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:kinetic-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:40dd970891c5342e622abad06cef1abb7a1028fba4ea2e2cac5ba2e86654970d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **78.2 MB (78243033 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a8b55dc8cebae19b3759058aa86d016dbd0c5b250a29ad01f961ea9507b3a27e`
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
# Thu, 02 Mar 2023 11:44:39 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
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
	-	`sha256:f989583c8ba595c2fb646ad093cc454bdb75e54ffe38ddcab4b7dc16bdb7e049`  
		Last Modified: Thu, 02 Mar 2023 11:57:37 GMT  
		Size: 42.6 MB (42607751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:kinetic-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:88e78a3e652b4b1af808021cb0b7be8e51482011249ba472e8c57ca4c852bdce
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.4 MB (76412911 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b558fd4728f4339d55d53189136d2d8d5681ab84008e295f189ebb8e86b603e1`
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
# Thu, 02 Mar 2023 02:27:15 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
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
	-	`sha256:2ce67b0569d875d7056824c4c9c02ac70786fa3b8901c3ba0c6a858c857ce0bd`  
		Last Modified: Thu, 02 Mar 2023 02:38:26 GMT  
		Size: 39.5 MB (39513912 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:kinetic-scm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:88398a25e6df8710f62c22d86345a8fa3f84e0713a6ac0c996896c2bcac959ce
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **88.4 MB (88361469 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1049a1bbcae803adb4a16ecc2adb582978810a7ddfb5ea9ec24da206f4be1ce1`
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
# Thu, 02 Mar 2023 03:39:12 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
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
	-	`sha256:738d753846623f2bf928d9c5ee5e40f7f523f14dd1df06fa8cb96528ab78ea3d`  
		Last Modified: Thu, 02 Mar 2023 03:59:42 GMT  
		Size: 44.1 MB (44141551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:kinetic-scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:fb2be6a90e849d0cee6c46ce77e713c60d83023e6b19401fffbdaf695bc333a2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.7 MB (75671361 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fecf79aedb1597b523736958d2e35a21cb919903f602fc38c3a7ac2730bd0d59`
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
# Thu, 02 Mar 2023 02:14:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
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
	-	`sha256:8810d2ec3d82d4c030df6fc52d887b2bb1e9a1c9f01e957fe9dfcdea137a33d2`  
		Last Modified: Thu, 02 Mar 2023 02:24:19 GMT  
		Size: 39.6 MB (39555093 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
