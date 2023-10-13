## `buildpack-deps:lunar-scm`

```console
$ docker pull buildpack-deps@sha256:05b7c9f239aca6d22dc6f8b040499abf381dc1af08a0ab822dad31de4717c4ff
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `buildpack-deps:lunar-scm` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:9b185118417e72749592483b3491a6aa3b8c8e42179976319923257057ff1d72
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **85.8 MB (85782942 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8d2703be409206d1ee821eedf8f00c38df5d9e8c9dee6618340c11dc584c48d8`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 16 Aug 2023 04:28:31 GMT
ARG RELEASE
# Wed, 16 Aug 2023 04:28:31 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 16 Aug 2023 04:28:31 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 16 Aug 2023 04:28:31 GMT
LABEL org.opencontainers.image.version=23.04
# Wed, 16 Aug 2023 04:28:32 GMT
ADD file:7392bed4dbab9fb7c9ad5bde6f3bfcde3bcbf1885c336af9c231af6defaa31e1 in / 
# Wed, 16 Aug 2023 04:28:33 GMT
CMD ["/bin/bash"]
# Sat, 02 Sep 2023 00:03:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 02 Sep 2023 00:04:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:05cdbc478740a42a5ebb092eefd6fc221933f796ee343c49cb920ee60025bab8`  
		Last Modified: Sat, 02 Sep 2023 00:12:48 GMT  
		Size: 27.7 MB (27651898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ea73fe152c7c1b43c8962bdf8054f83c720b0d6251821ccf461eef843531c42`  
		Last Modified: Sat, 02 Sep 2023 00:12:47 GMT  
		Size: 13.7 MB (13744690 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10e8d218b3d1561b5d122cd9db4c10b2fa28d00a9d62a5fa468005767a3c57ad`  
		Last Modified: Sat, 02 Sep 2023 00:13:03 GMT  
		Size: 44.4 MB (44386354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:lunar-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:bc6d4248879ec4a711aa75eade706ef957385237fc45fb1249be243bd0a209b6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **86.8 MB (86772867 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c4f5915541d7721f2aa036c93064ae10075f1523f13ff507a800b5d8096b1b82`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 04 Oct 2023 12:25:21 GMT
ARG RELEASE
# Wed, 04 Oct 2023 12:25:21 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 04 Oct 2023 12:25:21 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 04 Oct 2023 12:25:22 GMT
LABEL org.opencontainers.image.version=23.04
# Wed, 04 Oct 2023 12:25:24 GMT
ADD file:b92305119eab5dd3dfb00f4d83cd84e00c8ae57143739329da5a19aeda55be4e in / 
# Wed, 04 Oct 2023 12:25:24 GMT
CMD ["/bin/bash"]
# Fri, 13 Oct 2023 01:05:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 13 Oct 2023 01:06:45 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:0055151e5ef44f81f2355e8073f34f53cc16494749dbc5ba14445ce5edf3d3b6`  
		Last Modified: Fri, 13 Oct 2023 01:13:54 GMT  
		Size: 25.4 MB (25432981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e866c11041f7a46cb12551f8e93dea44f566d63d4fe5e9771fba148287d761c3`  
		Last Modified: Fri, 13 Oct 2023 01:13:51 GMT  
		Size: 12.7 MB (12665364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f378438bc51fcd6e34f3bded8ebdf10b2f56f47951e89908cd028fb60f9d763`  
		Last Modified: Fri, 13 Oct 2023 01:14:13 GMT  
		Size: 48.7 MB (48674522 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:lunar-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:d10b349a3cd51e0997f5a3b878cdb01995d2e0e16627eb7cd0ee6af648b7aa64
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **84.6 MB (84575674 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b19b4d079e4b736392aef707eecc9b7ab65cba785fffcc6c1f3c5e8717406ff7`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 16 Aug 2023 04:15:57 GMT
ARG RELEASE
# Wed, 16 Aug 2023 04:15:57 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 16 Aug 2023 04:15:57 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 16 Aug 2023 04:15:57 GMT
LABEL org.opencontainers.image.version=23.04
# Wed, 16 Aug 2023 04:16:01 GMT
ADD file:adea2962926b29b76eb8da76ae9e830c5ad7050ae9b19f5427191b338c8a2c56 in / 
# Wed, 16 Aug 2023 04:16:02 GMT
CMD ["/bin/bash"]
# Fri, 01 Sep 2023 23:17:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 01 Sep 2023 23:17:51 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:8b3bb2adde9f4704b6cbca4cd0cd3d0035b2dbab8b3cc6fe17ec006b386e1ebd`  
		Last Modified: Fri, 01 Sep 2023 23:26:49 GMT  
		Size: 27.0 MB (27006213 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1cd1935e47d8915d0f0ab87a4d0c823b0c698145c21215e144b766365ffd8c3`  
		Last Modified: Fri, 01 Sep 2023 23:26:48 GMT  
		Size: 13.3 MB (13333801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c2c77b1d5d537e25307eba90cccef89858a69e1a468e51d157eab0cce01dc9f`  
		Last Modified: Fri, 01 Sep 2023 23:27:02 GMT  
		Size: 44.2 MB (44235660 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:lunar-scm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:083620b403fe6ce077d9bfadd4d4bc03af171dfb33728ad6bdaea55f1c90301d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **96.8 MB (96815700 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d32634bfda619c6320def492ca58e0daf3fd968f91bedab97030f96d20316356`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 16 Aug 2023 04:16:31 GMT
ARG RELEASE
# Wed, 16 Aug 2023 04:16:31 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 16 Aug 2023 04:16:31 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 16 Aug 2023 04:16:31 GMT
LABEL org.opencontainers.image.version=23.04
# Wed, 16 Aug 2023 04:16:34 GMT
ADD file:a9d35b320d969ee1ae8a7bc83aba49da30d93724befb5948c680066ad4f1acdf in / 
# Wed, 16 Aug 2023 04:16:35 GMT
CMD ["/bin/bash"]
# Sat, 02 Sep 2023 00:52:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 02 Sep 2023 00:54:09 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:7726bd9db2470633f663befac95b40c8e232237cc11c665bf1475ea520873afa`  
		Last Modified: Sat, 02 Sep 2023 01:14:06 GMT  
		Size: 31.9 MB (31887072 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb47e875735b54909bb26c51f415b01486b244104962761fb0b086e0ba7adc81`  
		Last Modified: Sat, 02 Sep 2023 01:14:03 GMT  
		Size: 15.8 MB (15842384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29e0eb0d3a3bb8011cff8a14f8ab7ca63d45cafb31bcca77da48df64a6de6930`  
		Last Modified: Sat, 02 Sep 2023 01:14:31 GMT  
		Size: 49.1 MB (49086244 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:lunar-scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:b2f2a0881286b29de742d50d48259b750a115827b358237c1669ced83f74796e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **84.5 MB (84505154 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7decbe5c1b3961eed7d080573346ae9c054116dc044e81c734abe9ee131cc04d`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 16 Aug 2023 04:29:27 GMT
ARG RELEASE
# Wed, 16 Aug 2023 04:29:28 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 16 Aug 2023 04:29:28 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 16 Aug 2023 04:29:28 GMT
LABEL org.opencontainers.image.version=23.04
# Wed, 16 Aug 2023 04:29:29 GMT
ADD file:14fcf0756fb29b609af54412c31e2ff9acbf4634984ce95bf204c67668706cb5 in / 
# Wed, 16 Aug 2023 04:29:30 GMT
CMD ["/bin/bash"]
# Fri, 01 Sep 2023 23:16:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 01 Sep 2023 23:16:49 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e9a6157a42893e6f99bd42ba05c70c5313add95c69f61f12e51517c0100470b8`  
		Last Modified: Fri, 01 Sep 2023 23:24:13 GMT  
		Size: 26.2 MB (26223925 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04f88ef015543162519d8e086a0bb86351d03f27b98218ff39b27f3b8b7bc2cd`  
		Last Modified: Fri, 01 Sep 2023 23:24:12 GMT  
		Size: 14.0 MB (14005753 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ad80a5cffb7414f3bd06d5dafc212e2f5a767d3312bead7347e2ba8fae5be35`  
		Last Modified: Fri, 01 Sep 2023 23:24:25 GMT  
		Size: 44.3 MB (44275476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
