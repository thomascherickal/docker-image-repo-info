## `buildpack-deps:mantic-scm`

```console
$ docker pull buildpack-deps@sha256:7426923971a30a4ea6573636545da7d7defb315c7d9fe36cf29e092a34f8b45d
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
$ docker pull buildpack-deps@sha256:dce775894722bb7a698c8d1469b75c0aca6163089400ff4a14ea294144505507
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **86.1 MB (86089967 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3bab83a701026d74e0ae2ed322d8fa2cc126e1394fb089ba09155cfc13ebfb4a`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 07 Jun 2023 04:39:09 GMT
ARG RELEASE
# Wed, 07 Jun 2023 04:39:09 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 07 Jun 2023 04:39:09 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 07 Jun 2023 04:39:09 GMT
LABEL org.opencontainers.image.version=23.10
# Wed, 07 Jun 2023 04:39:10 GMT
ADD file:d8dc8c4236b9885e64ccd27399ed8dddab7d39915d76378527cb730855aba0e1 in / 
# Wed, 07 Jun 2023 04:39:10 GMT
CMD ["/bin/bash"]
# Fri, 16 Jun 2023 01:51:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 01:51:38 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:f4bf94e551580f94d5daff5f725b2d31607973745d1b88b4063002a615605d6e`  
		Last Modified: Fri, 16 Jun 2023 01:57:52 GMT  
		Size: 27.7 MB (27718548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5e689be570c2c956ab2de6b43f62c042013af889c34de3a06fa31c8840fd3bd`  
		Last Modified: Fri, 16 Jun 2023 01:57:50 GMT  
		Size: 13.8 MB (13750836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f0fac2598065d000cebfbe9e8556d9126e9b3a9e073e3c1f6dd0f9d3cdea45b`  
		Last Modified: Fri, 16 Jun 2023 01:58:07 GMT  
		Size: 44.6 MB (44620583 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:mantic-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:273ed9c32785683f8292147f0fc7e2fb6990a9df5e0a3957d1dd8544cdf3a9ae
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **86.7 MB (86706614 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b4aefe1528d1af75c9daad79f50cbe9e90f99f8da02c6d8e21194b22977327c1`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 07 Jun 2023 04:48:07 GMT
ARG RELEASE
# Wed, 07 Jun 2023 04:48:07 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 07 Jun 2023 04:48:08 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 07 Jun 2023 04:48:08 GMT
LABEL org.opencontainers.image.version=23.10
# Wed, 07 Jun 2023 04:48:12 GMT
ADD file:65e05498800189bf1f48f5c6df21d144e18e5e069db55d0b88d45c04cc1fe4de in / 
# Wed, 07 Jun 2023 04:48:12 GMT
CMD ["/bin/bash"]
# Fri, 16 Jun 2023 00:53:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 00:54:20 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:4d9959b212abdc29a099893ec5eeb0a1e80508f22581d6b7e8d7ac257769bee7`  
		Last Modified: Fri, 16 Jun 2023 01:00:47 GMT  
		Size: 25.3 MB (25271336 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85a3ceae76fca68286fb64b3323157a721f2f88a43cd21f69b7a567704523771`  
		Last Modified: Fri, 16 Jun 2023 01:00:46 GMT  
		Size: 12.7 MB (12669447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90993e861d0ec43708d28299de230556f24bbe5c1335ddb4543559a0ef84eebd`  
		Last Modified: Fri, 16 Jun 2023 01:01:03 GMT  
		Size: 48.8 MB (48765831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:mantic-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:4582791f2e2b3fa5be98507b81e404db0c8e0c450a7aebef8b10e0a19a0b68cb
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **84.9 MB (84867600 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a15eb0223167d9f89a1d80a31cce49cb9b87bacdcc59d85a0ee641a81a3e52ac`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 07 Jun 2023 04:42:14 GMT
ARG RELEASE
# Wed, 07 Jun 2023 04:42:14 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 07 Jun 2023 04:42:14 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 07 Jun 2023 04:42:14 GMT
LABEL org.opencontainers.image.version=23.10
# Wed, 07 Jun 2023 04:42:16 GMT
ADD file:3f4faed988a03b7d05aefe677906592aade4d2bae1ec3f7055c1f10744a38de0 in / 
# Wed, 07 Jun 2023 04:42:16 GMT
CMD ["/bin/bash"]
# Fri, 16 Jun 2023 02:29:37 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 02:30:07 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:62f0439e6eacbe88b3b071461591f644c013d55d1bb0ecba6442ac98c987966e`  
		Last Modified: Fri, 16 Jun 2023 02:36:15 GMT  
		Size: 27.1 MB (27075677 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39a4f6ab448c591bc2009541723cb7648afc9648bd50663a7868f9adb99bbb00`  
		Last Modified: Fri, 16 Jun 2023 02:36:13 GMT  
		Size: 13.3 MB (13336368 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc4cacd591b11e3cc5af36faa12d9667eb60b11aaa0e4ce07804dbadf858b1b9`  
		Last Modified: Fri, 16 Jun 2023 02:36:28 GMT  
		Size: 44.5 MB (44455555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:mantic-scm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:b31ac2547c0fb613ffdde3803dedebc5b816629a970152b92d175bd46ddcf231
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **97.1 MB (97144119 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:945e54eb4f23f94d5d07c9cd08f5390007886fa2744da72ecbf60d4f49441953`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 07 Jun 2023 04:48:25 GMT
ARG RELEASE
# Wed, 07 Jun 2023 04:48:26 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 07 Jun 2023 04:48:26 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 07 Jun 2023 04:48:26 GMT
LABEL org.opencontainers.image.version=23.10
# Wed, 07 Jun 2023 04:48:28 GMT
ADD file:6cf1bffac55b7de64803fabdb35baf75349cc0a40c0b4c68ac2690b7123edc85 in / 
# Wed, 07 Jun 2023 04:48:29 GMT
CMD ["/bin/bash"]
# Fri, 16 Jun 2023 01:18:42 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 01:19:34 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:3977e86345903c1f3d3fa576bf7d23648e574cafb925e0b8db7f0a26b5b9813d`  
		Last Modified: Fri, 16 Jun 2023 01:30:28 GMT  
		Size: 32.0 MB (31950363 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80356e871c531718f8219858742d4f265352a0709040acb54605134885fb5b5f`  
		Last Modified: Fri, 16 Jun 2023 01:30:24 GMT  
		Size: 15.8 MB (15844469 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:506380a8d2bc60216ca4cf81a6f68432f5f65a3aeb0a44fa44c0240ba5d5dd8f`  
		Last Modified: Fri, 16 Jun 2023 01:30:50 GMT  
		Size: 49.3 MB (49349287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:mantic-scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:31f672479b21e2cc2c87fe6dd466bfbf1694de7b58e11286d8d2a832a4b579d4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **84.5 MB (84503036 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:678ece2d51d0b780f97e099fda19610767c0d34f3faa336022f340fed73544af`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Sat, 20 May 2023 16:59:20 GMT
ARG RELEASE
# Sat, 20 May 2023 16:59:20 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Sat, 20 May 2023 16:59:20 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Sat, 20 May 2023 16:59:20 GMT
LABEL org.opencontainers.image.version=23.10
# Sat, 20 May 2023 16:59:22 GMT
ADD file:fb602b3f6c251d8267de1cf0525d0b38aab5966c848182d037bb2890557f0a6e in / 
# Sat, 20 May 2023 16:59:22 GMT
CMD ["/bin/bash"]
# Thu, 01 Jun 2023 23:15:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 01 Jun 2023 23:15:46 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e6197ead7faf6fa2f836b159dd66c603a28c581c4e273f6b664c86588a78ec95`  
		Last Modified: Thu, 01 Jun 2023 23:20:39 GMT  
		Size: 26.2 MB (26231487 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98abbd746ec759f3d8e8b447407b1e0248bc8e38e037360bdcebb69899e8cd07`  
		Last Modified: Thu, 01 Jun 2023 23:20:38 GMT  
		Size: 14.0 MB (14018998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fc44de0957139a61045543f4801b3145fa3f06e69b887ac90673e1c3da52f0f`  
		Last Modified: Thu, 01 Jun 2023 23:20:51 GMT  
		Size: 44.3 MB (44252551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
