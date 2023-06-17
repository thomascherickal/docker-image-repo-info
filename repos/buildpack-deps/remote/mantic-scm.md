## `buildpack-deps:mantic-scm`

```console
$ docker pull buildpack-deps@sha256:126a98ec90b3126c029ea65970f7a51f1090026a5f0fa839706c17db0a154499
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
$ docker pull buildpack-deps@sha256:85258892178bdb36541117c00935735c6a721657c4e5632cfa0691dd7d93cec8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **84.8 MB (84758939 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:506e112b04aad98bade14af15d4a20386438b08b1be95cbdd7db733fbd2a0908`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 07 Jun 2023 04:42:36 GMT
ARG RELEASE
# Wed, 07 Jun 2023 04:42:36 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 07 Jun 2023 04:42:36 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 07 Jun 2023 04:42:36 GMT
LABEL org.opencontainers.image.version=23.10
# Wed, 07 Jun 2023 04:42:38 GMT
ADD file:4e8ca8820de4a27d67ad223be645ce7a7a48289dfcbc01b4e1dbe3bc74ebbc56 in / 
# Wed, 07 Jun 2023 04:42:38 GMT
CMD ["/bin/bash"]
# Sat, 17 Jun 2023 09:56:31 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 17 Jun 2023 09:56:58 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:f6943591795586ce983bdf25369a45a8d58f64cd04bb9b22a9ebfbbbcaa9443a`  
		Last Modified: Sat, 17 Jun 2023 10:03:01 GMT  
		Size: 26.3 MB (26281083 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:031ae27af25073c29d7050bd7d1de8c0178d4af4c165618364aec7a707620748`  
		Last Modified: Sat, 17 Jun 2023 10:02:59 GMT  
		Size: 14.0 MB (14007357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0b5bce324197575b0db20f5609aefd088c3c53352089f34bf28f1ce1e2a69aa`  
		Last Modified: Sat, 17 Jun 2023 10:03:13 GMT  
		Size: 44.5 MB (44470499 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
