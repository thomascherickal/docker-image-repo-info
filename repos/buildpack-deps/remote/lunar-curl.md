## `buildpack-deps:lunar-curl`

```console
$ docker pull buildpack-deps@sha256:a90cd559f58c147ed7e994786e84b5656fadb23d0d0d18b347d63acec373df4b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `buildpack-deps:lunar-curl` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:4dd88c849c466833bc442ca0af75b2de2b19351338b04338af3d3a44e1815531
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.4 MB (41396588 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6094e5e80f92499ace6989f78bc8339ba778b721f8d6ed7332a35c20020e92f1`
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

### `buildpack-deps:lunar-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:e0ee7bd4dff2df21914a218557f98e7d13357c691d9b96c45d34c460b7960afc
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.1 MB (38093443 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3df89c3daf175c8485f22129e691eeed43e03cbb4da48783beced9084af8a3bf`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 16 Aug 2023 04:16:11 GMT
ARG RELEASE
# Wed, 16 Aug 2023 04:16:11 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 16 Aug 2023 04:16:11 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 16 Aug 2023 04:16:11 GMT
LABEL org.opencontainers.image.version=23.04
# Wed, 16 Aug 2023 04:16:16 GMT
ADD file:1f1c9502544acdbb6a7450226ced78cfe982a6305f2aea77ab7d1f73b50fc7f0 in / 
# Wed, 16 Aug 2023 04:16:16 GMT
CMD ["/bin/bash"]
# Fri, 01 Sep 2023 23:45:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:9fce615a928dd3a3068e1de48019af925a9120537cb22174bef3b5bc6c81aa30`  
		Last Modified: Fri, 01 Sep 2023 23:55:36 GMT  
		Size: 25.4 MB (25429153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:226718c385cfaf19fd9705f67eadf089cc077b99eacfccbae1ec6906f4cdfcbc`  
		Last Modified: Fri, 01 Sep 2023 23:55:34 GMT  
		Size: 12.7 MB (12664290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:lunar-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:82a3373f4890c76cc802fd33fa70d70b96b69aef86331e3f2708b816f829b221
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.3 MB (40340014 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:347dbace0278ff9d4b8b65a1fd129a9699401e182dc43dd1334165842f6a843e`
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

### `buildpack-deps:lunar-curl` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:98d110730769e1fef236121e4a9ae53b0c37b149dba6c92336743e2112d36bc9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.9 MB (47855866 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5c74f04b9e892d08bce8686689ac9c25c8376a2d70e6dc91c625f4bdf95734b0`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 31 Jul 2023 17:18:51 GMT
ARG RELEASE
# Mon, 31 Jul 2023 17:18:51 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 31 Jul 2023 17:18:51 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 31 Jul 2023 17:18:51 GMT
LABEL org.opencontainers.image.version=23.04
# Mon, 31 Jul 2023 17:18:54 GMT
ADD file:98fe279e3c3239702ac2eef51540228e24a3e15e923342cb3e7cd7dd3684a090 in / 
# Mon, 31 Jul 2023 17:18:54 GMT
CMD ["/bin/bash"]
# Thu, 03 Aug 2023 03:31:31 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:c8f1d2c62b1aacc6f999b01ed9c6ef10bc5fd3a989af86649162cf5292934393`  
		Last Modified: Thu, 03 Aug 2023 03:51:49 GMT  
		Size: 32.0 MB (32013471 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71dd1b07037748833f21cbeb83084ac8ff4a0ca93e61d3e0ac3914daf1beac24`  
		Last Modified: Thu, 03 Aug 2023 03:51:45 GMT  
		Size: 15.8 MB (15842395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:lunar-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:3e2c1730f17419017837d5f1fc9db6ff833b9dc686ee7b21402e510119d4f4b7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.2 MB (40229678 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:32608e7b5cf27557f6091473da05b6af8a046c450931620144b6162abe38dc78`
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
