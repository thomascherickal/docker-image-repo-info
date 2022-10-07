<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `traefik`

-	[`traefik:1.7`](#traefik17)
-	[`traefik:1.7-alpine`](#traefik17-alpine)
-	[`traefik:1.7-windowsservercore-1809`](#traefik17-windowsservercore-1809)
-	[`traefik:1.7.34`](#traefik1734)
-	[`traefik:1.7.34-alpine`](#traefik1734-alpine)
-	[`traefik:1.7.34-windowsservercore-1809`](#traefik1734-windowsservercore-1809)
-	[`traefik:2.9`](#traefik29)
-	[`traefik:2.9-windowsservercore-1809`](#traefik29-windowsservercore-1809)
-	[`traefik:2.9.1`](#traefik291)
-	[`traefik:2.9.1-windowsservercore-1809`](#traefik291-windowsservercore-1809)
-	[`traefik:banon`](#traefikbanon)
-	[`traefik:banon-windowsservercore-1809`](#traefikbanon-windowsservercore-1809)
-	[`traefik:latest`](#traefiklatest)
-	[`traefik:maroilles`](#traefikmaroilles)
-	[`traefik:maroilles-alpine`](#traefikmaroilles-alpine)
-	[`traefik:maroilles-windowsservercore-1809`](#traefikmaroilles-windowsservercore-1809)
-	[`traefik:v1.7`](#traefikv17)
-	[`traefik:v1.7-alpine`](#traefikv17-alpine)
-	[`traefik:v1.7-windowsservercore-1809`](#traefikv17-windowsservercore-1809)
-	[`traefik:v1.7.34`](#traefikv1734)
-	[`traefik:v1.7.34-alpine`](#traefikv1734-alpine)
-	[`traefik:v1.7.34-windowsservercore-1809`](#traefikv1734-windowsservercore-1809)
-	[`traefik:v2.9`](#traefikv29)
-	[`traefik:v2.9-windowsservercore-1809`](#traefikv29-windowsservercore-1809)
-	[`traefik:v2.9.1`](#traefikv291)
-	[`traefik:v2.9.1-windowsservercore-1809`](#traefikv291-windowsservercore-1809)
-	[`traefik:windowsservercore-1809`](#traefikwindowsservercore-1809)

## `traefik:1.7`

```console
$ docker pull traefik@sha256:c7ac8f4b5c47b5ee28c3ef93cb46e37e249173605629f775e8f33ffd00b52d04
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:1.7` - linux; amd64

```console
$ docker pull traefik@sha256:9248f7f17d44a02872613d652aff91856f928ebc400d037cd3439731da4cecbb
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **22.6 MB (22605595 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f2dd394242b858ec3a77eec6506ea614377091f1904f704d3412983c1be8c0cd`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Fri, 07 Oct 2022 04:21:33 GMT
COPY file:48964762d0c961c28f59ebd3ea194fb6486cf2bd9a9cf1780f6702d88bd7b7d9 in /etc/ssl/certs/ 
# Fri, 07 Oct 2022 04:21:34 GMT
COPY dir:c3f72545af4f290c8fc0a43693ea3334451b85d0dee09c519eb983a71a5a38fa in /usr/share/ 
# Fri, 07 Oct 2022 04:21:35 GMT
COPY file:36217e5a6056bef26cfff395c8af8c1010a61dbe8d62b2c7869ca221e2a6302c in / 
# Fri, 07 Oct 2022 04:21:35 GMT
EXPOSE 80
# Fri, 07 Oct 2022 04:21:35 GMT
VOLUME [/tmp]
# Fri, 07 Oct 2022 04:21:35 GMT
ENTRYPOINT ["/traefik"]
# Fri, 07 Oct 2022 04:21:35 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.34 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:39006e619508cd8a1ace2dcb57ecaa3a206fc01c9b72018e30b538ba58b0f45a`  
		Last Modified: Fri, 07 Oct 2022 04:22:39 GMT  
		Size: 123.5 KB (123540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa79c7609bd35acb6baeec95c0534de9f28c053bb3b54b53c4831b70e4a2b6e2`  
		Last Modified: Fri, 07 Oct 2022 04:22:39 GMT  
		Size: 320.1 KB (320103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19b58027c881a56cde12f5ad6ba79f399d338b083423a96ae8fdb32a53f55af9`  
		Last Modified: Fri, 07 Oct 2022 04:22:44 GMT  
		Size: 22.2 MB (22161952 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:1.7` - linux; arm variant v6

```console
$ docker pull traefik@sha256:8fccb57b1adeec9e17144aeae1399b8ac4241b11d7b914dd315902a830ba733a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **21.1 MB (21075358 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:92fdada8ccde42d699c1a63cf60e989525bc21342c1ac12e6638ee02d43a4a06`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Thu, 11 Aug 2022 01:14:36 GMT
COPY file:48964762d0c961c28f59ebd3ea194fb6486cf2bd9a9cf1780f6702d88bd7b7d9 in /etc/ssl/certs/ 
# Thu, 11 Aug 2022 01:14:37 GMT
COPY dir:a84372748b89eb90478bb1b120b7c8fff3112421d7f93e50fbeae3f53adc6788 in /usr/share/ 
# Thu, 11 Aug 2022 01:14:38 GMT
COPY file:5d1e7e81e8b77b4f8828eeaf0d30a0f135a949b51396f12ae22af376c36d3129 in / 
# Thu, 11 Aug 2022 01:14:38 GMT
EXPOSE 80
# Thu, 11 Aug 2022 01:14:39 GMT
VOLUME [/tmp]
# Thu, 11 Aug 2022 01:14:39 GMT
ENTRYPOINT ["/traefik"]
# Thu, 11 Aug 2022 01:14:39 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.34 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:75f0504c96ad5e9ea3bfc1f0fee80ae3ed4a779d16dba3bf3372c959db0857fe`  
		Last Modified: Thu, 11 Aug 2022 01:16:18 GMT  
		Size: 123.5 KB (123540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a29d285728c6dfaea768ae8c8fa72cfb8acdfb637798090ec09469d4a33b9fb4`  
		Last Modified: Thu, 11 Aug 2022 01:16:18 GMT  
		Size: 328.5 KB (328536 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73f2ae5ba0fcd216aa8ef6f62507561e6616937a868c3acfd3046fa039b7e5ce`  
		Last Modified: Thu, 11 Aug 2022 01:16:22 GMT  
		Size: 20.6 MB (20623282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:1.7` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:fa1d0bc12d9c099cef08d01b3a9eab66778aedf00fbef5b3da0d272333af80d1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **20.6 MB (20574968 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:63349a030de8627c4abdf307b26a78e32c2a18bc376815ff5cbc07ae39722178`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Fri, 07 Oct 2022 07:39:24 GMT
COPY file:48964762d0c961c28f59ebd3ea194fb6486cf2bd9a9cf1780f6702d88bd7b7d9 in /etc/ssl/certs/ 
# Fri, 07 Oct 2022 07:39:25 GMT
COPY dir:c3f72545af4f290c8fc0a43693ea3334451b85d0dee09c519eb983a71a5a38fa in /usr/share/ 
# Fri, 07 Oct 2022 07:39:26 GMT
COPY file:60330593b6644f3f519fd13ce8ee34c2c7ab9994a1420afabbc01926dd1230dd in / 
# Fri, 07 Oct 2022 07:39:26 GMT
EXPOSE 80
# Fri, 07 Oct 2022 07:39:27 GMT
VOLUME [/tmp]
# Fri, 07 Oct 2022 07:39:28 GMT
ENTRYPOINT ["/traefik"]
# Fri, 07 Oct 2022 07:39:29 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.34 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:1151fb31968944320508e292407b79b28626a76d0af23bfcb76650fd6129b93f`  
		Last Modified: Fri, 07 Oct 2022 07:40:55 GMT  
		Size: 123.5 KB (123539 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:019c3a4ad05f22d384ae4ec9a37d144b01923d7a2a5241e8a510dd4d6b6ee5f9`  
		Last Modified: Fri, 07 Oct 2022 07:40:55 GMT  
		Size: 320.1 KB (320082 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d89d15d062829fe9582b412a41e0c33f0050d927582e9f13666017c4f6992017`  
		Last Modified: Fri, 07 Oct 2022 07:40:58 GMT  
		Size: 20.1 MB (20131347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:1.7-alpine`

```console
$ docker pull traefik@sha256:5df35f40f618c30e4458d0f23591c74818cab81f889110db2de86a0640dc127f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:1.7-alpine` - linux; amd64

```console
$ docker pull traefik@sha256:26fa7cd56b81852ea9f61e45df0913aab21313dc3ceeab8a893916893b533054
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.7 MB (25662747 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:16d7c99e10d8ab1a83a9b8ae9755e9912e39a2a9e52da6ce6de8defc71809bd8`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Tue, 09 Aug 2022 17:20:07 GMT
ADD file:b9bd10cf83356cb7281baa0fbaca5186cf27491f59eda87abe57f83a5aaf5ec1 in / 
# Tue, 09 Aug 2022 17:20:08 GMT
CMD ["/bin/sh"]
# Fri, 07 Oct 2022 04:21:23 GMT
RUN apk --no-cache add ca-certificates tzdata
# Fri, 07 Oct 2022 04:21:27 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/traefik/traefik/releases/download/v1.7.34/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Fri, 07 Oct 2022 04:21:27 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Fri, 07 Oct 2022 04:21:27 GMT
EXPOSE 80
# Fri, 07 Oct 2022 04:21:27 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 07 Oct 2022 04:21:28 GMT
CMD ["traefik"]
# Fri, 07 Oct 2022 04:21:28 GMT
LABEL org.opencontainers.image.vendor=traefik org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.34 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:c7ed990a2339ee598662849de4f56e2241399f5a32340c8c4a7bbd5378a12b5f`  
		Last Modified: Tue, 09 Aug 2022 17:21:06 GMT  
		Size: 2.8 MB (2827489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02345b26a3d377d58f815ff68ead6a7dd73b699f6c32431c8d20e8f089729c37`  
		Last Modified: Fri, 07 Oct 2022 04:22:19 GMT  
		Size: 672.8 KB (672839 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fedb3d96d801ee542c140b3c61969835a610feec705ca8958b056cca584fce66`  
		Last Modified: Fri, 07 Oct 2022 04:22:23 GMT  
		Size: 22.2 MB (22162052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4889541507d1292f1cc22ab716fe900b3cf01a14362a5fe85f91fbf67a75cee`  
		Last Modified: Fri, 07 Oct 2022 04:22:19 GMT  
		Size: 367.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:1.7-alpine` - linux; arm variant v6

```console
$ docker pull traefik@sha256:aa449bd11477cfbcb2023958b4a006fe8c5c7cd93eb3dbb30a7014356686ed20
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.9 MB (23945270 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9c0445b729681b5642ccc3eae945721e8d39c71806b442cace900bca97537cc6`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Tue, 09 Aug 2022 17:49:35 GMT
ADD file:8ff80989f06f5a8ffe16c56e00538928dcb1e46faa2b58ab9c14c7227a6cd8f9 in / 
# Tue, 09 Aug 2022 17:49:35 GMT
CMD ["/bin/sh"]
# Thu, 11 Aug 2022 01:14:24 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 11 Aug 2022 01:14:28 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/traefik/traefik/releases/download/v1.7.34/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Thu, 11 Aug 2022 01:14:29 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 11 Aug 2022 01:14:29 GMT
EXPOSE 80
# Thu, 11 Aug 2022 01:14:29 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 11 Aug 2022 01:14:29 GMT
CMD ["traefik"]
# Thu, 11 Aug 2022 01:14:29 GMT
LABEL org.opencontainers.image.vendor=traefik org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.34 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:7d147289082e6aa6ef510c09d7c0ac8b5026e0b591f1bfcaf01ceada43c9ec65`  
		Last Modified: Tue, 09 Aug 2022 17:51:04 GMT  
		Size: 2.6 MB (2635498 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c46f6fc1fc29e436e3a75b410a2801637bb73995aa0e7b64b676b17443a973f9`  
		Last Modified: Thu, 11 Aug 2022 01:15:55 GMT  
		Size: 686.0 KB (685981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1fe741c4fe2d8bec0997fa1b514de659d0daa075215ec13d7259b7388c56612`  
		Last Modified: Thu, 11 Aug 2022 01:15:58 GMT  
		Size: 20.6 MB (20623422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fc60ca867112243a32bb0d4db8b9f289c30d55b72fa2c4c20dd21d2ebb4edc1`  
		Last Modified: Thu, 11 Aug 2022 01:15:55 GMT  
		Size: 369.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:1.7-alpine` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:81bc86d35c76c5a6289b2162ab33431e5e7e814c51400a1624d4726d3d5d913c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.5 MB (23527631 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:94a85707debaaa6d4e90402c73e5ec37e7965c0699c6fd71cb0b8123b62110bd`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Tue, 09 Aug 2022 17:39:59 GMT
ADD file:b312c8f512719efd09811d17c2b250bbad03cf3f90c135a00695cc8e152f4ee2 in / 
# Tue, 09 Aug 2022 17:39:59 GMT
CMD ["/bin/sh"]
# Fri, 07 Oct 2022 07:39:08 GMT
RUN apk --no-cache add ca-certificates tzdata
# Fri, 07 Oct 2022 07:39:11 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/traefik/traefik/releases/download/v1.7.34/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Fri, 07 Oct 2022 07:39:13 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Fri, 07 Oct 2022 07:39:13 GMT
EXPOSE 80
# Fri, 07 Oct 2022 07:39:14 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 07 Oct 2022 07:39:15 GMT
CMD ["traefik"]
# Fri, 07 Oct 2022 07:39:16 GMT
LABEL org.opencontainers.image.vendor=traefik org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.34 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:90cda3b7c32511829cd5ae9074240c36c34507085acb6e55b96f993740d2be93`  
		Last Modified: Tue, 09 Aug 2022 17:41:06 GMT  
		Size: 2.7 MB (2722153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43c315e6d7f9d205ba53331de71d2e455d2f6c238e3916ea0fa90c6aeb56ba18`  
		Last Modified: Fri, 07 Oct 2022 07:40:33 GMT  
		Size: 673.7 KB (673730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e0303139d79db6c9786dbdd349cfc46e7aeb686ba6a142bdc12ae48112fcbe6`  
		Last Modified: Fri, 07 Oct 2022 07:40:36 GMT  
		Size: 20.1 MB (20131379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02ee5cf74fa4c8b0e9c2567d694100f1ce2406b150d66b21b1af5880b839eaad`  
		Last Modified: Fri, 07 Oct 2022 07:40:33 GMT  
		Size: 369.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:1.7-windowsservercore-1809`

```console
$ docker pull traefik@sha256:7c233c425c02be64e4d02c6ac904f8fd586214173652667ed12a6cbe40b35251
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3406; amd64

### `traefik:1.7-windowsservercore-1809` - windows version 10.0.17763.3406; amd64

```console
$ docker pull traefik@sha256:3cfa84be7d7e57c654a1a3b8e4c41b7ba5f3c5c550cb0174b550c2db0c88be3b
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2726409092 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0fe8cd7f2792b2846bba0ec097dd8b13686688eaacc32a4e789952137e619ede`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Fri, 09 Sep 2022 22:43:02 GMT
RUN Install update 10.0.17763.3406
# Tue, 13 Sep 2022 18:21:27 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 13 Sep 2022 18:24:55 GMT
RUN Invoke-WebRequest     -Uri "https://github.com/traefik/traefik/releases/download/v1.7.34/traefik_windows-amd64.exe"     -OutFile "/traefik.exe"
# Tue, 13 Sep 2022 18:24:56 GMT
EXPOSE 80
# Tue, 13 Sep 2022 18:24:57 GMT
ENTRYPOINT ["/traefik"]
# Tue, 13 Sep 2022 18:24:57 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.34 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:b111c3320c949bea81612bf4554f1b6592c2f504920b5bf57ba340a1d4d52c93`  
		Size: 1.9 GB (1877166088 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:cee64bf279e2ca8e924884a10ecb98bfa79c7f0cc8d25e73039b9aeb940815b6`  
		Size: 826.4 MB (826398623 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:2bc395c8c47e61e593d2e905e0e051d40e7d25e4aeac7dbe08d3ec57acd0e68f`  
		Last Modified: Tue, 13 Sep 2022 18:25:24 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fef8fcae363c967cdda31871dbfcc00b3f35458cbfcba05f7a6d1552c3b9d83c`  
		Last Modified: Tue, 13 Sep 2022 18:25:55 GMT  
		Size: 22.8 MB (22838714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c14ce042369487448642ab933c5aaf18199baa6713c317cbae8067107daeaeca`  
		Last Modified: Tue, 13 Sep 2022 18:25:49 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1836085afff7fe0b9beb9748abe6f34d94003944e2981312832ee76886845d5`  
		Last Modified: Tue, 13 Sep 2022 18:25:52 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24edcfd0e075a20e436658f609f8aa0212feb2c0739e613d2cd95a333639bfe3`  
		Last Modified: Tue, 13 Sep 2022 18:25:49 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:1.7.34`

```console
$ docker pull traefik@sha256:c7ac8f4b5c47b5ee28c3ef93cb46e37e249173605629f775e8f33ffd00b52d04
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:1.7.34` - linux; amd64

```console
$ docker pull traefik@sha256:9248f7f17d44a02872613d652aff91856f928ebc400d037cd3439731da4cecbb
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **22.6 MB (22605595 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f2dd394242b858ec3a77eec6506ea614377091f1904f704d3412983c1be8c0cd`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Fri, 07 Oct 2022 04:21:33 GMT
COPY file:48964762d0c961c28f59ebd3ea194fb6486cf2bd9a9cf1780f6702d88bd7b7d9 in /etc/ssl/certs/ 
# Fri, 07 Oct 2022 04:21:34 GMT
COPY dir:c3f72545af4f290c8fc0a43693ea3334451b85d0dee09c519eb983a71a5a38fa in /usr/share/ 
# Fri, 07 Oct 2022 04:21:35 GMT
COPY file:36217e5a6056bef26cfff395c8af8c1010a61dbe8d62b2c7869ca221e2a6302c in / 
# Fri, 07 Oct 2022 04:21:35 GMT
EXPOSE 80
# Fri, 07 Oct 2022 04:21:35 GMT
VOLUME [/tmp]
# Fri, 07 Oct 2022 04:21:35 GMT
ENTRYPOINT ["/traefik"]
# Fri, 07 Oct 2022 04:21:35 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.34 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:39006e619508cd8a1ace2dcb57ecaa3a206fc01c9b72018e30b538ba58b0f45a`  
		Last Modified: Fri, 07 Oct 2022 04:22:39 GMT  
		Size: 123.5 KB (123540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa79c7609bd35acb6baeec95c0534de9f28c053bb3b54b53c4831b70e4a2b6e2`  
		Last Modified: Fri, 07 Oct 2022 04:22:39 GMT  
		Size: 320.1 KB (320103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19b58027c881a56cde12f5ad6ba79f399d338b083423a96ae8fdb32a53f55af9`  
		Last Modified: Fri, 07 Oct 2022 04:22:44 GMT  
		Size: 22.2 MB (22161952 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:1.7.34` - linux; arm variant v6

```console
$ docker pull traefik@sha256:8fccb57b1adeec9e17144aeae1399b8ac4241b11d7b914dd315902a830ba733a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **21.1 MB (21075358 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:92fdada8ccde42d699c1a63cf60e989525bc21342c1ac12e6638ee02d43a4a06`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Thu, 11 Aug 2022 01:14:36 GMT
COPY file:48964762d0c961c28f59ebd3ea194fb6486cf2bd9a9cf1780f6702d88bd7b7d9 in /etc/ssl/certs/ 
# Thu, 11 Aug 2022 01:14:37 GMT
COPY dir:a84372748b89eb90478bb1b120b7c8fff3112421d7f93e50fbeae3f53adc6788 in /usr/share/ 
# Thu, 11 Aug 2022 01:14:38 GMT
COPY file:5d1e7e81e8b77b4f8828eeaf0d30a0f135a949b51396f12ae22af376c36d3129 in / 
# Thu, 11 Aug 2022 01:14:38 GMT
EXPOSE 80
# Thu, 11 Aug 2022 01:14:39 GMT
VOLUME [/tmp]
# Thu, 11 Aug 2022 01:14:39 GMT
ENTRYPOINT ["/traefik"]
# Thu, 11 Aug 2022 01:14:39 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.34 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:75f0504c96ad5e9ea3bfc1f0fee80ae3ed4a779d16dba3bf3372c959db0857fe`  
		Last Modified: Thu, 11 Aug 2022 01:16:18 GMT  
		Size: 123.5 KB (123540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a29d285728c6dfaea768ae8c8fa72cfb8acdfb637798090ec09469d4a33b9fb4`  
		Last Modified: Thu, 11 Aug 2022 01:16:18 GMT  
		Size: 328.5 KB (328536 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73f2ae5ba0fcd216aa8ef6f62507561e6616937a868c3acfd3046fa039b7e5ce`  
		Last Modified: Thu, 11 Aug 2022 01:16:22 GMT  
		Size: 20.6 MB (20623282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:1.7.34` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:fa1d0bc12d9c099cef08d01b3a9eab66778aedf00fbef5b3da0d272333af80d1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **20.6 MB (20574968 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:63349a030de8627c4abdf307b26a78e32c2a18bc376815ff5cbc07ae39722178`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Fri, 07 Oct 2022 07:39:24 GMT
COPY file:48964762d0c961c28f59ebd3ea194fb6486cf2bd9a9cf1780f6702d88bd7b7d9 in /etc/ssl/certs/ 
# Fri, 07 Oct 2022 07:39:25 GMT
COPY dir:c3f72545af4f290c8fc0a43693ea3334451b85d0dee09c519eb983a71a5a38fa in /usr/share/ 
# Fri, 07 Oct 2022 07:39:26 GMT
COPY file:60330593b6644f3f519fd13ce8ee34c2c7ab9994a1420afabbc01926dd1230dd in / 
# Fri, 07 Oct 2022 07:39:26 GMT
EXPOSE 80
# Fri, 07 Oct 2022 07:39:27 GMT
VOLUME [/tmp]
# Fri, 07 Oct 2022 07:39:28 GMT
ENTRYPOINT ["/traefik"]
# Fri, 07 Oct 2022 07:39:29 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.34 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:1151fb31968944320508e292407b79b28626a76d0af23bfcb76650fd6129b93f`  
		Last Modified: Fri, 07 Oct 2022 07:40:55 GMT  
		Size: 123.5 KB (123539 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:019c3a4ad05f22d384ae4ec9a37d144b01923d7a2a5241e8a510dd4d6b6ee5f9`  
		Last Modified: Fri, 07 Oct 2022 07:40:55 GMT  
		Size: 320.1 KB (320082 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d89d15d062829fe9582b412a41e0c33f0050d927582e9f13666017c4f6992017`  
		Last Modified: Fri, 07 Oct 2022 07:40:58 GMT  
		Size: 20.1 MB (20131347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:1.7.34-alpine`

```console
$ docker pull traefik@sha256:5df35f40f618c30e4458d0f23591c74818cab81f889110db2de86a0640dc127f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:1.7.34-alpine` - linux; amd64

```console
$ docker pull traefik@sha256:26fa7cd56b81852ea9f61e45df0913aab21313dc3ceeab8a893916893b533054
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.7 MB (25662747 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:16d7c99e10d8ab1a83a9b8ae9755e9912e39a2a9e52da6ce6de8defc71809bd8`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Tue, 09 Aug 2022 17:20:07 GMT
ADD file:b9bd10cf83356cb7281baa0fbaca5186cf27491f59eda87abe57f83a5aaf5ec1 in / 
# Tue, 09 Aug 2022 17:20:08 GMT
CMD ["/bin/sh"]
# Fri, 07 Oct 2022 04:21:23 GMT
RUN apk --no-cache add ca-certificates tzdata
# Fri, 07 Oct 2022 04:21:27 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/traefik/traefik/releases/download/v1.7.34/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Fri, 07 Oct 2022 04:21:27 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Fri, 07 Oct 2022 04:21:27 GMT
EXPOSE 80
# Fri, 07 Oct 2022 04:21:27 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 07 Oct 2022 04:21:28 GMT
CMD ["traefik"]
# Fri, 07 Oct 2022 04:21:28 GMT
LABEL org.opencontainers.image.vendor=traefik org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.34 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:c7ed990a2339ee598662849de4f56e2241399f5a32340c8c4a7bbd5378a12b5f`  
		Last Modified: Tue, 09 Aug 2022 17:21:06 GMT  
		Size: 2.8 MB (2827489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02345b26a3d377d58f815ff68ead6a7dd73b699f6c32431c8d20e8f089729c37`  
		Last Modified: Fri, 07 Oct 2022 04:22:19 GMT  
		Size: 672.8 KB (672839 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fedb3d96d801ee542c140b3c61969835a610feec705ca8958b056cca584fce66`  
		Last Modified: Fri, 07 Oct 2022 04:22:23 GMT  
		Size: 22.2 MB (22162052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4889541507d1292f1cc22ab716fe900b3cf01a14362a5fe85f91fbf67a75cee`  
		Last Modified: Fri, 07 Oct 2022 04:22:19 GMT  
		Size: 367.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:1.7.34-alpine` - linux; arm variant v6

```console
$ docker pull traefik@sha256:aa449bd11477cfbcb2023958b4a006fe8c5c7cd93eb3dbb30a7014356686ed20
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.9 MB (23945270 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9c0445b729681b5642ccc3eae945721e8d39c71806b442cace900bca97537cc6`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Tue, 09 Aug 2022 17:49:35 GMT
ADD file:8ff80989f06f5a8ffe16c56e00538928dcb1e46faa2b58ab9c14c7227a6cd8f9 in / 
# Tue, 09 Aug 2022 17:49:35 GMT
CMD ["/bin/sh"]
# Thu, 11 Aug 2022 01:14:24 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 11 Aug 2022 01:14:28 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/traefik/traefik/releases/download/v1.7.34/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Thu, 11 Aug 2022 01:14:29 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 11 Aug 2022 01:14:29 GMT
EXPOSE 80
# Thu, 11 Aug 2022 01:14:29 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 11 Aug 2022 01:14:29 GMT
CMD ["traefik"]
# Thu, 11 Aug 2022 01:14:29 GMT
LABEL org.opencontainers.image.vendor=traefik org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.34 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:7d147289082e6aa6ef510c09d7c0ac8b5026e0b591f1bfcaf01ceada43c9ec65`  
		Last Modified: Tue, 09 Aug 2022 17:51:04 GMT  
		Size: 2.6 MB (2635498 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c46f6fc1fc29e436e3a75b410a2801637bb73995aa0e7b64b676b17443a973f9`  
		Last Modified: Thu, 11 Aug 2022 01:15:55 GMT  
		Size: 686.0 KB (685981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1fe741c4fe2d8bec0997fa1b514de659d0daa075215ec13d7259b7388c56612`  
		Last Modified: Thu, 11 Aug 2022 01:15:58 GMT  
		Size: 20.6 MB (20623422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fc60ca867112243a32bb0d4db8b9f289c30d55b72fa2c4c20dd21d2ebb4edc1`  
		Last Modified: Thu, 11 Aug 2022 01:15:55 GMT  
		Size: 369.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:1.7.34-alpine` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:81bc86d35c76c5a6289b2162ab33431e5e7e814c51400a1624d4726d3d5d913c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.5 MB (23527631 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:94a85707debaaa6d4e90402c73e5ec37e7965c0699c6fd71cb0b8123b62110bd`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Tue, 09 Aug 2022 17:39:59 GMT
ADD file:b312c8f512719efd09811d17c2b250bbad03cf3f90c135a00695cc8e152f4ee2 in / 
# Tue, 09 Aug 2022 17:39:59 GMT
CMD ["/bin/sh"]
# Fri, 07 Oct 2022 07:39:08 GMT
RUN apk --no-cache add ca-certificates tzdata
# Fri, 07 Oct 2022 07:39:11 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/traefik/traefik/releases/download/v1.7.34/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Fri, 07 Oct 2022 07:39:13 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Fri, 07 Oct 2022 07:39:13 GMT
EXPOSE 80
# Fri, 07 Oct 2022 07:39:14 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 07 Oct 2022 07:39:15 GMT
CMD ["traefik"]
# Fri, 07 Oct 2022 07:39:16 GMT
LABEL org.opencontainers.image.vendor=traefik org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.34 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:90cda3b7c32511829cd5ae9074240c36c34507085acb6e55b96f993740d2be93`  
		Last Modified: Tue, 09 Aug 2022 17:41:06 GMT  
		Size: 2.7 MB (2722153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43c315e6d7f9d205ba53331de71d2e455d2f6c238e3916ea0fa90c6aeb56ba18`  
		Last Modified: Fri, 07 Oct 2022 07:40:33 GMT  
		Size: 673.7 KB (673730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e0303139d79db6c9786dbdd349cfc46e7aeb686ba6a142bdc12ae48112fcbe6`  
		Last Modified: Fri, 07 Oct 2022 07:40:36 GMT  
		Size: 20.1 MB (20131379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02ee5cf74fa4c8b0e9c2567d694100f1ce2406b150d66b21b1af5880b839eaad`  
		Last Modified: Fri, 07 Oct 2022 07:40:33 GMT  
		Size: 369.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:1.7.34-windowsservercore-1809`

```console
$ docker pull traefik@sha256:7c233c425c02be64e4d02c6ac904f8fd586214173652667ed12a6cbe40b35251
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3406; amd64

### `traefik:1.7.34-windowsservercore-1809` - windows version 10.0.17763.3406; amd64

```console
$ docker pull traefik@sha256:3cfa84be7d7e57c654a1a3b8e4c41b7ba5f3c5c550cb0174b550c2db0c88be3b
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2726409092 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0fe8cd7f2792b2846bba0ec097dd8b13686688eaacc32a4e789952137e619ede`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Fri, 09 Sep 2022 22:43:02 GMT
RUN Install update 10.0.17763.3406
# Tue, 13 Sep 2022 18:21:27 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 13 Sep 2022 18:24:55 GMT
RUN Invoke-WebRequest     -Uri "https://github.com/traefik/traefik/releases/download/v1.7.34/traefik_windows-amd64.exe"     -OutFile "/traefik.exe"
# Tue, 13 Sep 2022 18:24:56 GMT
EXPOSE 80
# Tue, 13 Sep 2022 18:24:57 GMT
ENTRYPOINT ["/traefik"]
# Tue, 13 Sep 2022 18:24:57 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.34 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:b111c3320c949bea81612bf4554f1b6592c2f504920b5bf57ba340a1d4d52c93`  
		Size: 1.9 GB (1877166088 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:cee64bf279e2ca8e924884a10ecb98bfa79c7f0cc8d25e73039b9aeb940815b6`  
		Size: 826.4 MB (826398623 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:2bc395c8c47e61e593d2e905e0e051d40e7d25e4aeac7dbe08d3ec57acd0e68f`  
		Last Modified: Tue, 13 Sep 2022 18:25:24 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fef8fcae363c967cdda31871dbfcc00b3f35458cbfcba05f7a6d1552c3b9d83c`  
		Last Modified: Tue, 13 Sep 2022 18:25:55 GMT  
		Size: 22.8 MB (22838714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c14ce042369487448642ab933c5aaf18199baa6713c317cbae8067107daeaeca`  
		Last Modified: Tue, 13 Sep 2022 18:25:49 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1836085afff7fe0b9beb9748abe6f34d94003944e2981312832ee76886845d5`  
		Last Modified: Tue, 13 Sep 2022 18:25:52 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24edcfd0e075a20e436658f609f8aa0212feb2c0739e613d2cd95a333639bfe3`  
		Last Modified: Tue, 13 Sep 2022 18:25:49 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:2.9`

```console
$ docker pull traefik@sha256:426f5d4e1432a1d1780a0fe081715d70c667345df1e50b02be57872f3e410628
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; s390x

### `traefik:2.9` - linux; amd64

```console
$ docker pull traefik@sha256:3eaf50b7874f63567ee5d18498536928faef199302c805cb6b766e06b649302d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.4 MB (33416269 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e6de8578b2384107d9e08f90be5d6cf43472e369ba98dca46373b336b83fdbd8`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Tue, 09 Aug 2022 17:20:00 GMT
ADD file:f77e3f51f020890d22997e6c2ca98968b75b8bc8c463341a2010ff0655d4c88f in / 
# Tue, 09 Aug 2022 17:20:01 GMT
CMD ["/bin/sh"]
# Fri, 07 Oct 2022 04:21:14 GMT
RUN apk --no-cache add ca-certificates tzdata
# Fri, 07 Oct 2022 04:21:18 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.9.1/traefik_v2.9.1_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Fri, 07 Oct 2022 04:21:18 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Fri, 07 Oct 2022 04:21:18 GMT
EXPOSE 80
# Fri, 07 Oct 2022 04:21:18 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 07 Oct 2022 04:21:18 GMT
CMD ["traefik"]
# Fri, 07 Oct 2022 04:21:19 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.9.1 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:9621f1afde84053b2f9b6ff34fc7f7460712247c01cbab483c5fa7132cf782ca`  
		Last Modified: Tue, 09 Aug 2022 17:20:52 GMT  
		Size: 2.8 MB (2823512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f62b4fe8af5e2bd23c9c1a5303b1d320706bc52330058f23c4725df3dadc9cad`  
		Last Modified: Fri, 07 Oct 2022 04:21:55 GMT  
		Size: 673.4 KB (673371 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b954c2c3b6c35a716c65a53d1bb120db920d2cdc90267d260674af3965a5b68`  
		Last Modified: Fri, 07 Oct 2022 04:22:00 GMT  
		Size: 29.9 MB (29919018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:857fadab46062ec62a3b8f3183843ff14b05f3ec377ccbe51a5296f86eacce5f`  
		Last Modified: Fri, 07 Oct 2022 04:21:55 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:2.9` - linux; arm variant v6

```console
$ docker pull traefik@sha256:95960ed785badbe47cd0ec5bfc0833db6502043a7c83d1a14fa495615bd7dbd7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.5 MB (31543171 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:df1030c56c08192fde82ebb2fef3c8b57f7d8d340ac8463f7e563f4637caa60a`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Tue, 09 Aug 2022 17:49:29 GMT
ADD file:89cb25f97e17bed5c56311280efe5cfa78422d8ffbe36232195d13f94d67417e in / 
# Tue, 09 Aug 2022 17:49:29 GMT
CMD ["/bin/sh"]
# Thu, 11 Aug 2022 01:14:12 GMT
RUN apk --no-cache add ca-certificates tzdata
# Mon, 03 Oct 2022 22:49:32 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.9.1/traefik_v2.9.1_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Mon, 03 Oct 2022 22:49:33 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Mon, 03 Oct 2022 22:49:33 GMT
EXPOSE 80
# Mon, 03 Oct 2022 22:49:33 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 03 Oct 2022 22:49:33 GMT
CMD ["traefik"]
# Mon, 03 Oct 2022 22:49:33 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.9.1 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:293b708aa6fb80967f27727d5c9c53ac9ba9cac376bed2ad02c17a5cca317b35`  
		Last Modified: Tue, 09 Aug 2022 17:50:52 GMT  
		Size: 2.6 MB (2631127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:667ecdfbf7665eeb46df55d94a2322221d8d1de9cebdc0f97c05affd0aa619f0`  
		Last Modified: Thu, 11 Aug 2022 01:15:26 GMT  
		Size: 686.0 KB (686042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31d29799c16bfd82dab22b9850857fb3488e2dc721c763c4bcc4fde280c30872`  
		Last Modified: Mon, 03 Oct 2022 22:50:37 GMT  
		Size: 28.2 MB (28225634 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce6ee8605f9b04da07ee4ce0161573fc9e64faccb9a768733f7222a40ad141c2`  
		Last Modified: Mon, 03 Oct 2022 22:50:31 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:2.9` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:3e90150cae10bbf88c2c186563c6307a0a4e7d169d2f640ac04fdda6b08b9b36
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.7 MB (30704302 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3fb461c4c2d15f33277f220c17547fd45eb0d588862147433c0d11afe2bfc1c4`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Tue, 09 Aug 2022 17:39:51 GMT
ADD file:4b51a9d40f20d2beb29d0759b161d2b9403493453beb509de4e86a5d98513f16 in / 
# Tue, 09 Aug 2022 17:39:51 GMT
CMD ["/bin/sh"]
# Fri, 07 Oct 2022 07:38:51 GMT
RUN apk --no-cache add ca-certificates tzdata
# Fri, 07 Oct 2022 07:38:55 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.9.1/traefik_v2.9.1_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Fri, 07 Oct 2022 07:38:56 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Fri, 07 Oct 2022 07:38:56 GMT
EXPOSE 80
# Fri, 07 Oct 2022 07:38:57 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 07 Oct 2022 07:38:58 GMT
CMD ["traefik"]
# Fri, 07 Oct 2022 07:38:59 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.9.1 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:47517142f6ba87eca6b7bdca1e0df160b74671c81e4b9605dad38c1862a43be3`  
		Last Modified: Tue, 09 Aug 2022 17:40:55 GMT  
		Size: 2.7 MB (2718439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24e179f025e9fd053dccf5cf01e48636e8a4fa642091186bc0a736693adbc34f`  
		Last Modified: Fri, 07 Oct 2022 07:40:07 GMT  
		Size: 673.7 KB (673749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94b59dd829100bd144172d2c8d6fa0e5c7c4b18b3f5e621012734841e8b803f7`  
		Last Modified: Fri, 07 Oct 2022 07:40:11 GMT  
		Size: 27.3 MB (27311746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3d7e56d00862713d11472648e728636220fa3aab656c706e800aba3b9be7687`  
		Last Modified: Fri, 07 Oct 2022 07:40:07 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:2.9` - linux; s390x

```console
$ docker pull traefik@sha256:86ff93cc178de9b8f86436b83bc6e896c65edb55cda098b94882253afdd3eb1d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.1 MB (32112411 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cb0174719729d126f9205e2bd2f9d55bdd430ac98c573cb2f2b92d2e5c12bcf9`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Tue, 09 Aug 2022 17:41:54 GMT
ADD file:7489fa84133e97e4f40b13dd5159989b3594c9627d9147bfc4e33134944cc368 in / 
# Tue, 09 Aug 2022 17:41:54 GMT
CMD ["/bin/sh"]
# Fri, 07 Oct 2022 09:56:58 GMT
RUN apk --no-cache add ca-certificates tzdata
# Fri, 07 Oct 2022 09:57:06 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.9.1/traefik_v2.9.1_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Fri, 07 Oct 2022 09:57:10 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Fri, 07 Oct 2022 09:57:11 GMT
EXPOSE 80
# Fri, 07 Oct 2022 09:57:12 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 07 Oct 2022 09:57:12 GMT
CMD ["traefik"]
# Fri, 07 Oct 2022 09:57:13 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.9.1 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:cdf710f5b7ee39c5124c50c753228dc9b8b1c1c0a1a38f1413487548565445c3`  
		Last Modified: Tue, 09 Aug 2022 17:42:56 GMT  
		Size: 2.6 MB (2606087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a84a1ec6f28225d3ff13bc2defe049a19ceecab6d949a0e69884c44e7e28279b`  
		Last Modified: Fri, 07 Oct 2022 09:57:42 GMT  
		Size: 677.5 KB (677512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e1d229f8b015fe7609ece81d9725b607d8ca5314d0f08667adfd7c13a5d5daf`  
		Last Modified: Fri, 07 Oct 2022 09:57:46 GMT  
		Size: 28.8 MB (28828444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd924ce12d473d0268c58ca23de4965014be194f51da2ab5fa66fbb94384d8e5`  
		Last Modified: Fri, 07 Oct 2022 09:57:42 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:2.9-windowsservercore-1809`

```console
$ docker pull traefik@sha256:f30447f41aae80f422d9e54a030544c0aef686d30be9bf2552b7bb5c5e906baa
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3406; amd64

### `traefik:2.9-windowsservercore-1809` - windows version 10.0.17763.3406; amd64

```console
$ docker pull traefik@sha256:0b774d737eb46e9d8d7ef5395b7a0eb5172b3debcb450d66460ea763137a9c9a
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2733978551 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:47a82dae6c960ec5c9dc6e6e61bd935ee3edeb2bea4e223ef31ed3ac4ee1c041`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Fri, 09 Sep 2022 22:43:02 GMT
RUN Install update 10.0.17763.3406
# Tue, 13 Sep 2022 18:21:27 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Mon, 03 Oct 2022 22:22:40 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/traefik/traefik/releases/download/v2.9.1/traefik_v2.9.1_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Mon, 03 Oct 2022 22:22:41 GMT
EXPOSE 80
# Mon, 03 Oct 2022 22:22:42 GMT
ENTRYPOINT ["/traefik"]
# Mon, 03 Oct 2022 22:22:43 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.9.1 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:b111c3320c949bea81612bf4554f1b6592c2f504920b5bf57ba340a1d4d52c93`  
		Size: 1.9 GB (1877166088 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:cee64bf279e2ca8e924884a10ecb98bfa79c7f0cc8d25e73039b9aeb940815b6`  
		Size: 826.4 MB (826398623 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:2bc395c8c47e61e593d2e905e0e051d40e7d25e4aeac7dbe08d3ec57acd0e68f`  
		Last Modified: Tue, 13 Sep 2022 18:25:24 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c7765a94b2fc5ac1ba474cd067a9942ed01008e08eefadb55cc32c40dcfb695`  
		Last Modified: Mon, 03 Oct 2022 22:23:25 GMT  
		Size: 30.4 MB (30408185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51b834274d250812b031261d0107840c5a20f3f21da74e9210818321ecff1a37`  
		Last Modified: Mon, 03 Oct 2022 22:23:18 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a51c1e6b70f0a0702f1f5a84a0e10573577c14f197262205dc63ed5f75f5b3b`  
		Last Modified: Mon, 03 Oct 2022 22:23:18 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3770a98f22a4479168ce9f4fdfc7e714e1adc958f7bb8b565c500658ea8ad298`  
		Last Modified: Mon, 03 Oct 2022 22:23:18 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:2.9.1`

```console
$ docker pull traefik@sha256:426f5d4e1432a1d1780a0fe081715d70c667345df1e50b02be57872f3e410628
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; s390x

### `traefik:2.9.1` - linux; amd64

```console
$ docker pull traefik@sha256:3eaf50b7874f63567ee5d18498536928faef199302c805cb6b766e06b649302d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.4 MB (33416269 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e6de8578b2384107d9e08f90be5d6cf43472e369ba98dca46373b336b83fdbd8`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Tue, 09 Aug 2022 17:20:00 GMT
ADD file:f77e3f51f020890d22997e6c2ca98968b75b8bc8c463341a2010ff0655d4c88f in / 
# Tue, 09 Aug 2022 17:20:01 GMT
CMD ["/bin/sh"]
# Fri, 07 Oct 2022 04:21:14 GMT
RUN apk --no-cache add ca-certificates tzdata
# Fri, 07 Oct 2022 04:21:18 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.9.1/traefik_v2.9.1_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Fri, 07 Oct 2022 04:21:18 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Fri, 07 Oct 2022 04:21:18 GMT
EXPOSE 80
# Fri, 07 Oct 2022 04:21:18 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 07 Oct 2022 04:21:18 GMT
CMD ["traefik"]
# Fri, 07 Oct 2022 04:21:19 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.9.1 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:9621f1afde84053b2f9b6ff34fc7f7460712247c01cbab483c5fa7132cf782ca`  
		Last Modified: Tue, 09 Aug 2022 17:20:52 GMT  
		Size: 2.8 MB (2823512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f62b4fe8af5e2bd23c9c1a5303b1d320706bc52330058f23c4725df3dadc9cad`  
		Last Modified: Fri, 07 Oct 2022 04:21:55 GMT  
		Size: 673.4 KB (673371 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b954c2c3b6c35a716c65a53d1bb120db920d2cdc90267d260674af3965a5b68`  
		Last Modified: Fri, 07 Oct 2022 04:22:00 GMT  
		Size: 29.9 MB (29919018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:857fadab46062ec62a3b8f3183843ff14b05f3ec377ccbe51a5296f86eacce5f`  
		Last Modified: Fri, 07 Oct 2022 04:21:55 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:2.9.1` - linux; arm variant v6

```console
$ docker pull traefik@sha256:95960ed785badbe47cd0ec5bfc0833db6502043a7c83d1a14fa495615bd7dbd7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.5 MB (31543171 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:df1030c56c08192fde82ebb2fef3c8b57f7d8d340ac8463f7e563f4637caa60a`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Tue, 09 Aug 2022 17:49:29 GMT
ADD file:89cb25f97e17bed5c56311280efe5cfa78422d8ffbe36232195d13f94d67417e in / 
# Tue, 09 Aug 2022 17:49:29 GMT
CMD ["/bin/sh"]
# Thu, 11 Aug 2022 01:14:12 GMT
RUN apk --no-cache add ca-certificates tzdata
# Mon, 03 Oct 2022 22:49:32 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.9.1/traefik_v2.9.1_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Mon, 03 Oct 2022 22:49:33 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Mon, 03 Oct 2022 22:49:33 GMT
EXPOSE 80
# Mon, 03 Oct 2022 22:49:33 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 03 Oct 2022 22:49:33 GMT
CMD ["traefik"]
# Mon, 03 Oct 2022 22:49:33 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.9.1 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:293b708aa6fb80967f27727d5c9c53ac9ba9cac376bed2ad02c17a5cca317b35`  
		Last Modified: Tue, 09 Aug 2022 17:50:52 GMT  
		Size: 2.6 MB (2631127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:667ecdfbf7665eeb46df55d94a2322221d8d1de9cebdc0f97c05affd0aa619f0`  
		Last Modified: Thu, 11 Aug 2022 01:15:26 GMT  
		Size: 686.0 KB (686042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31d29799c16bfd82dab22b9850857fb3488e2dc721c763c4bcc4fde280c30872`  
		Last Modified: Mon, 03 Oct 2022 22:50:37 GMT  
		Size: 28.2 MB (28225634 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce6ee8605f9b04da07ee4ce0161573fc9e64faccb9a768733f7222a40ad141c2`  
		Last Modified: Mon, 03 Oct 2022 22:50:31 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:2.9.1` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:3e90150cae10bbf88c2c186563c6307a0a4e7d169d2f640ac04fdda6b08b9b36
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.7 MB (30704302 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3fb461c4c2d15f33277f220c17547fd45eb0d588862147433c0d11afe2bfc1c4`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Tue, 09 Aug 2022 17:39:51 GMT
ADD file:4b51a9d40f20d2beb29d0759b161d2b9403493453beb509de4e86a5d98513f16 in / 
# Tue, 09 Aug 2022 17:39:51 GMT
CMD ["/bin/sh"]
# Fri, 07 Oct 2022 07:38:51 GMT
RUN apk --no-cache add ca-certificates tzdata
# Fri, 07 Oct 2022 07:38:55 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.9.1/traefik_v2.9.1_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Fri, 07 Oct 2022 07:38:56 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Fri, 07 Oct 2022 07:38:56 GMT
EXPOSE 80
# Fri, 07 Oct 2022 07:38:57 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 07 Oct 2022 07:38:58 GMT
CMD ["traefik"]
# Fri, 07 Oct 2022 07:38:59 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.9.1 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:47517142f6ba87eca6b7bdca1e0df160b74671c81e4b9605dad38c1862a43be3`  
		Last Modified: Tue, 09 Aug 2022 17:40:55 GMT  
		Size: 2.7 MB (2718439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24e179f025e9fd053dccf5cf01e48636e8a4fa642091186bc0a736693adbc34f`  
		Last Modified: Fri, 07 Oct 2022 07:40:07 GMT  
		Size: 673.7 KB (673749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94b59dd829100bd144172d2c8d6fa0e5c7c4b18b3f5e621012734841e8b803f7`  
		Last Modified: Fri, 07 Oct 2022 07:40:11 GMT  
		Size: 27.3 MB (27311746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3d7e56d00862713d11472648e728636220fa3aab656c706e800aba3b9be7687`  
		Last Modified: Fri, 07 Oct 2022 07:40:07 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:2.9.1` - linux; s390x

```console
$ docker pull traefik@sha256:86ff93cc178de9b8f86436b83bc6e896c65edb55cda098b94882253afdd3eb1d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.1 MB (32112411 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cb0174719729d126f9205e2bd2f9d55bdd430ac98c573cb2f2b92d2e5c12bcf9`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Tue, 09 Aug 2022 17:41:54 GMT
ADD file:7489fa84133e97e4f40b13dd5159989b3594c9627d9147bfc4e33134944cc368 in / 
# Tue, 09 Aug 2022 17:41:54 GMT
CMD ["/bin/sh"]
# Fri, 07 Oct 2022 09:56:58 GMT
RUN apk --no-cache add ca-certificates tzdata
# Fri, 07 Oct 2022 09:57:06 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.9.1/traefik_v2.9.1_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Fri, 07 Oct 2022 09:57:10 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Fri, 07 Oct 2022 09:57:11 GMT
EXPOSE 80
# Fri, 07 Oct 2022 09:57:12 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 07 Oct 2022 09:57:12 GMT
CMD ["traefik"]
# Fri, 07 Oct 2022 09:57:13 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.9.1 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:cdf710f5b7ee39c5124c50c753228dc9b8b1c1c0a1a38f1413487548565445c3`  
		Last Modified: Tue, 09 Aug 2022 17:42:56 GMT  
		Size: 2.6 MB (2606087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a84a1ec6f28225d3ff13bc2defe049a19ceecab6d949a0e69884c44e7e28279b`  
		Last Modified: Fri, 07 Oct 2022 09:57:42 GMT  
		Size: 677.5 KB (677512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e1d229f8b015fe7609ece81d9725b607d8ca5314d0f08667adfd7c13a5d5daf`  
		Last Modified: Fri, 07 Oct 2022 09:57:46 GMT  
		Size: 28.8 MB (28828444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd924ce12d473d0268c58ca23de4965014be194f51da2ab5fa66fbb94384d8e5`  
		Last Modified: Fri, 07 Oct 2022 09:57:42 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:2.9.1-windowsservercore-1809`

```console
$ docker pull traefik@sha256:f30447f41aae80f422d9e54a030544c0aef686d30be9bf2552b7bb5c5e906baa
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3406; amd64

### `traefik:2.9.1-windowsservercore-1809` - windows version 10.0.17763.3406; amd64

```console
$ docker pull traefik@sha256:0b774d737eb46e9d8d7ef5395b7a0eb5172b3debcb450d66460ea763137a9c9a
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2733978551 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:47a82dae6c960ec5c9dc6e6e61bd935ee3edeb2bea4e223ef31ed3ac4ee1c041`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Fri, 09 Sep 2022 22:43:02 GMT
RUN Install update 10.0.17763.3406
# Tue, 13 Sep 2022 18:21:27 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Mon, 03 Oct 2022 22:22:40 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/traefik/traefik/releases/download/v2.9.1/traefik_v2.9.1_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Mon, 03 Oct 2022 22:22:41 GMT
EXPOSE 80
# Mon, 03 Oct 2022 22:22:42 GMT
ENTRYPOINT ["/traefik"]
# Mon, 03 Oct 2022 22:22:43 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.9.1 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:b111c3320c949bea81612bf4554f1b6592c2f504920b5bf57ba340a1d4d52c93`  
		Size: 1.9 GB (1877166088 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:cee64bf279e2ca8e924884a10ecb98bfa79c7f0cc8d25e73039b9aeb940815b6`  
		Size: 826.4 MB (826398623 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:2bc395c8c47e61e593d2e905e0e051d40e7d25e4aeac7dbe08d3ec57acd0e68f`  
		Last Modified: Tue, 13 Sep 2022 18:25:24 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c7765a94b2fc5ac1ba474cd067a9942ed01008e08eefadb55cc32c40dcfb695`  
		Last Modified: Mon, 03 Oct 2022 22:23:25 GMT  
		Size: 30.4 MB (30408185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51b834274d250812b031261d0107840c5a20f3f21da74e9210818321ecff1a37`  
		Last Modified: Mon, 03 Oct 2022 22:23:18 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a51c1e6b70f0a0702f1f5a84a0e10573577c14f197262205dc63ed5f75f5b3b`  
		Last Modified: Mon, 03 Oct 2022 22:23:18 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3770a98f22a4479168ce9f4fdfc7e714e1adc958f7bb8b565c500658ea8ad298`  
		Last Modified: Mon, 03 Oct 2022 22:23:18 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:banon`

```console
$ docker pull traefik@sha256:426f5d4e1432a1d1780a0fe081715d70c667345df1e50b02be57872f3e410628
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; s390x

### `traefik:banon` - linux; amd64

```console
$ docker pull traefik@sha256:3eaf50b7874f63567ee5d18498536928faef199302c805cb6b766e06b649302d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.4 MB (33416269 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e6de8578b2384107d9e08f90be5d6cf43472e369ba98dca46373b336b83fdbd8`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Tue, 09 Aug 2022 17:20:00 GMT
ADD file:f77e3f51f020890d22997e6c2ca98968b75b8bc8c463341a2010ff0655d4c88f in / 
# Tue, 09 Aug 2022 17:20:01 GMT
CMD ["/bin/sh"]
# Fri, 07 Oct 2022 04:21:14 GMT
RUN apk --no-cache add ca-certificates tzdata
# Fri, 07 Oct 2022 04:21:18 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.9.1/traefik_v2.9.1_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Fri, 07 Oct 2022 04:21:18 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Fri, 07 Oct 2022 04:21:18 GMT
EXPOSE 80
# Fri, 07 Oct 2022 04:21:18 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 07 Oct 2022 04:21:18 GMT
CMD ["traefik"]
# Fri, 07 Oct 2022 04:21:19 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.9.1 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:9621f1afde84053b2f9b6ff34fc7f7460712247c01cbab483c5fa7132cf782ca`  
		Last Modified: Tue, 09 Aug 2022 17:20:52 GMT  
		Size: 2.8 MB (2823512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f62b4fe8af5e2bd23c9c1a5303b1d320706bc52330058f23c4725df3dadc9cad`  
		Last Modified: Fri, 07 Oct 2022 04:21:55 GMT  
		Size: 673.4 KB (673371 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b954c2c3b6c35a716c65a53d1bb120db920d2cdc90267d260674af3965a5b68`  
		Last Modified: Fri, 07 Oct 2022 04:22:00 GMT  
		Size: 29.9 MB (29919018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:857fadab46062ec62a3b8f3183843ff14b05f3ec377ccbe51a5296f86eacce5f`  
		Last Modified: Fri, 07 Oct 2022 04:21:55 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:banon` - linux; arm variant v6

```console
$ docker pull traefik@sha256:95960ed785badbe47cd0ec5bfc0833db6502043a7c83d1a14fa495615bd7dbd7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.5 MB (31543171 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:df1030c56c08192fde82ebb2fef3c8b57f7d8d340ac8463f7e563f4637caa60a`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Tue, 09 Aug 2022 17:49:29 GMT
ADD file:89cb25f97e17bed5c56311280efe5cfa78422d8ffbe36232195d13f94d67417e in / 
# Tue, 09 Aug 2022 17:49:29 GMT
CMD ["/bin/sh"]
# Thu, 11 Aug 2022 01:14:12 GMT
RUN apk --no-cache add ca-certificates tzdata
# Mon, 03 Oct 2022 22:49:32 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.9.1/traefik_v2.9.1_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Mon, 03 Oct 2022 22:49:33 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Mon, 03 Oct 2022 22:49:33 GMT
EXPOSE 80
# Mon, 03 Oct 2022 22:49:33 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 03 Oct 2022 22:49:33 GMT
CMD ["traefik"]
# Mon, 03 Oct 2022 22:49:33 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.9.1 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:293b708aa6fb80967f27727d5c9c53ac9ba9cac376bed2ad02c17a5cca317b35`  
		Last Modified: Tue, 09 Aug 2022 17:50:52 GMT  
		Size: 2.6 MB (2631127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:667ecdfbf7665eeb46df55d94a2322221d8d1de9cebdc0f97c05affd0aa619f0`  
		Last Modified: Thu, 11 Aug 2022 01:15:26 GMT  
		Size: 686.0 KB (686042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31d29799c16bfd82dab22b9850857fb3488e2dc721c763c4bcc4fde280c30872`  
		Last Modified: Mon, 03 Oct 2022 22:50:37 GMT  
		Size: 28.2 MB (28225634 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce6ee8605f9b04da07ee4ce0161573fc9e64faccb9a768733f7222a40ad141c2`  
		Last Modified: Mon, 03 Oct 2022 22:50:31 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:banon` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:3e90150cae10bbf88c2c186563c6307a0a4e7d169d2f640ac04fdda6b08b9b36
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.7 MB (30704302 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3fb461c4c2d15f33277f220c17547fd45eb0d588862147433c0d11afe2bfc1c4`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Tue, 09 Aug 2022 17:39:51 GMT
ADD file:4b51a9d40f20d2beb29d0759b161d2b9403493453beb509de4e86a5d98513f16 in / 
# Tue, 09 Aug 2022 17:39:51 GMT
CMD ["/bin/sh"]
# Fri, 07 Oct 2022 07:38:51 GMT
RUN apk --no-cache add ca-certificates tzdata
# Fri, 07 Oct 2022 07:38:55 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.9.1/traefik_v2.9.1_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Fri, 07 Oct 2022 07:38:56 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Fri, 07 Oct 2022 07:38:56 GMT
EXPOSE 80
# Fri, 07 Oct 2022 07:38:57 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 07 Oct 2022 07:38:58 GMT
CMD ["traefik"]
# Fri, 07 Oct 2022 07:38:59 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.9.1 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:47517142f6ba87eca6b7bdca1e0df160b74671c81e4b9605dad38c1862a43be3`  
		Last Modified: Tue, 09 Aug 2022 17:40:55 GMT  
		Size: 2.7 MB (2718439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24e179f025e9fd053dccf5cf01e48636e8a4fa642091186bc0a736693adbc34f`  
		Last Modified: Fri, 07 Oct 2022 07:40:07 GMT  
		Size: 673.7 KB (673749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94b59dd829100bd144172d2c8d6fa0e5c7c4b18b3f5e621012734841e8b803f7`  
		Last Modified: Fri, 07 Oct 2022 07:40:11 GMT  
		Size: 27.3 MB (27311746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3d7e56d00862713d11472648e728636220fa3aab656c706e800aba3b9be7687`  
		Last Modified: Fri, 07 Oct 2022 07:40:07 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:banon` - linux; s390x

```console
$ docker pull traefik@sha256:86ff93cc178de9b8f86436b83bc6e896c65edb55cda098b94882253afdd3eb1d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.1 MB (32112411 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cb0174719729d126f9205e2bd2f9d55bdd430ac98c573cb2f2b92d2e5c12bcf9`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Tue, 09 Aug 2022 17:41:54 GMT
ADD file:7489fa84133e97e4f40b13dd5159989b3594c9627d9147bfc4e33134944cc368 in / 
# Tue, 09 Aug 2022 17:41:54 GMT
CMD ["/bin/sh"]
# Fri, 07 Oct 2022 09:56:58 GMT
RUN apk --no-cache add ca-certificates tzdata
# Fri, 07 Oct 2022 09:57:06 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.9.1/traefik_v2.9.1_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Fri, 07 Oct 2022 09:57:10 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Fri, 07 Oct 2022 09:57:11 GMT
EXPOSE 80
# Fri, 07 Oct 2022 09:57:12 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 07 Oct 2022 09:57:12 GMT
CMD ["traefik"]
# Fri, 07 Oct 2022 09:57:13 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.9.1 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:cdf710f5b7ee39c5124c50c753228dc9b8b1c1c0a1a38f1413487548565445c3`  
		Last Modified: Tue, 09 Aug 2022 17:42:56 GMT  
		Size: 2.6 MB (2606087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a84a1ec6f28225d3ff13bc2defe049a19ceecab6d949a0e69884c44e7e28279b`  
		Last Modified: Fri, 07 Oct 2022 09:57:42 GMT  
		Size: 677.5 KB (677512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e1d229f8b015fe7609ece81d9725b607d8ca5314d0f08667adfd7c13a5d5daf`  
		Last Modified: Fri, 07 Oct 2022 09:57:46 GMT  
		Size: 28.8 MB (28828444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd924ce12d473d0268c58ca23de4965014be194f51da2ab5fa66fbb94384d8e5`  
		Last Modified: Fri, 07 Oct 2022 09:57:42 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:banon-windowsservercore-1809`

```console
$ docker pull traefik@sha256:f30447f41aae80f422d9e54a030544c0aef686d30be9bf2552b7bb5c5e906baa
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3406; amd64

### `traefik:banon-windowsservercore-1809` - windows version 10.0.17763.3406; amd64

```console
$ docker pull traefik@sha256:0b774d737eb46e9d8d7ef5395b7a0eb5172b3debcb450d66460ea763137a9c9a
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2733978551 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:47a82dae6c960ec5c9dc6e6e61bd935ee3edeb2bea4e223ef31ed3ac4ee1c041`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Fri, 09 Sep 2022 22:43:02 GMT
RUN Install update 10.0.17763.3406
# Tue, 13 Sep 2022 18:21:27 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Mon, 03 Oct 2022 22:22:40 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/traefik/traefik/releases/download/v2.9.1/traefik_v2.9.1_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Mon, 03 Oct 2022 22:22:41 GMT
EXPOSE 80
# Mon, 03 Oct 2022 22:22:42 GMT
ENTRYPOINT ["/traefik"]
# Mon, 03 Oct 2022 22:22:43 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.9.1 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:b111c3320c949bea81612bf4554f1b6592c2f504920b5bf57ba340a1d4d52c93`  
		Size: 1.9 GB (1877166088 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:cee64bf279e2ca8e924884a10ecb98bfa79c7f0cc8d25e73039b9aeb940815b6`  
		Size: 826.4 MB (826398623 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:2bc395c8c47e61e593d2e905e0e051d40e7d25e4aeac7dbe08d3ec57acd0e68f`  
		Last Modified: Tue, 13 Sep 2022 18:25:24 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c7765a94b2fc5ac1ba474cd067a9942ed01008e08eefadb55cc32c40dcfb695`  
		Last Modified: Mon, 03 Oct 2022 22:23:25 GMT  
		Size: 30.4 MB (30408185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51b834274d250812b031261d0107840c5a20f3f21da74e9210818321ecff1a37`  
		Last Modified: Mon, 03 Oct 2022 22:23:18 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a51c1e6b70f0a0702f1f5a84a0e10573577c14f197262205dc63ed5f75f5b3b`  
		Last Modified: Mon, 03 Oct 2022 22:23:18 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3770a98f22a4479168ce9f4fdfc7e714e1adc958f7bb8b565c500658ea8ad298`  
		Last Modified: Mon, 03 Oct 2022 22:23:18 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:latest`

```console
$ docker pull traefik@sha256:426f5d4e1432a1d1780a0fe081715d70c667345df1e50b02be57872f3e410628
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; s390x

### `traefik:latest` - linux; amd64

```console
$ docker pull traefik@sha256:3eaf50b7874f63567ee5d18498536928faef199302c805cb6b766e06b649302d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.4 MB (33416269 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e6de8578b2384107d9e08f90be5d6cf43472e369ba98dca46373b336b83fdbd8`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Tue, 09 Aug 2022 17:20:00 GMT
ADD file:f77e3f51f020890d22997e6c2ca98968b75b8bc8c463341a2010ff0655d4c88f in / 
# Tue, 09 Aug 2022 17:20:01 GMT
CMD ["/bin/sh"]
# Fri, 07 Oct 2022 04:21:14 GMT
RUN apk --no-cache add ca-certificates tzdata
# Fri, 07 Oct 2022 04:21:18 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.9.1/traefik_v2.9.1_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Fri, 07 Oct 2022 04:21:18 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Fri, 07 Oct 2022 04:21:18 GMT
EXPOSE 80
# Fri, 07 Oct 2022 04:21:18 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 07 Oct 2022 04:21:18 GMT
CMD ["traefik"]
# Fri, 07 Oct 2022 04:21:19 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.9.1 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:9621f1afde84053b2f9b6ff34fc7f7460712247c01cbab483c5fa7132cf782ca`  
		Last Modified: Tue, 09 Aug 2022 17:20:52 GMT  
		Size: 2.8 MB (2823512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f62b4fe8af5e2bd23c9c1a5303b1d320706bc52330058f23c4725df3dadc9cad`  
		Last Modified: Fri, 07 Oct 2022 04:21:55 GMT  
		Size: 673.4 KB (673371 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b954c2c3b6c35a716c65a53d1bb120db920d2cdc90267d260674af3965a5b68`  
		Last Modified: Fri, 07 Oct 2022 04:22:00 GMT  
		Size: 29.9 MB (29919018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:857fadab46062ec62a3b8f3183843ff14b05f3ec377ccbe51a5296f86eacce5f`  
		Last Modified: Fri, 07 Oct 2022 04:21:55 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:latest` - linux; arm variant v6

```console
$ docker pull traefik@sha256:95960ed785badbe47cd0ec5bfc0833db6502043a7c83d1a14fa495615bd7dbd7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.5 MB (31543171 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:df1030c56c08192fde82ebb2fef3c8b57f7d8d340ac8463f7e563f4637caa60a`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Tue, 09 Aug 2022 17:49:29 GMT
ADD file:89cb25f97e17bed5c56311280efe5cfa78422d8ffbe36232195d13f94d67417e in / 
# Tue, 09 Aug 2022 17:49:29 GMT
CMD ["/bin/sh"]
# Thu, 11 Aug 2022 01:14:12 GMT
RUN apk --no-cache add ca-certificates tzdata
# Mon, 03 Oct 2022 22:49:32 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.9.1/traefik_v2.9.1_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Mon, 03 Oct 2022 22:49:33 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Mon, 03 Oct 2022 22:49:33 GMT
EXPOSE 80
# Mon, 03 Oct 2022 22:49:33 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 03 Oct 2022 22:49:33 GMT
CMD ["traefik"]
# Mon, 03 Oct 2022 22:49:33 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.9.1 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:293b708aa6fb80967f27727d5c9c53ac9ba9cac376bed2ad02c17a5cca317b35`  
		Last Modified: Tue, 09 Aug 2022 17:50:52 GMT  
		Size: 2.6 MB (2631127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:667ecdfbf7665eeb46df55d94a2322221d8d1de9cebdc0f97c05affd0aa619f0`  
		Last Modified: Thu, 11 Aug 2022 01:15:26 GMT  
		Size: 686.0 KB (686042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31d29799c16bfd82dab22b9850857fb3488e2dc721c763c4bcc4fde280c30872`  
		Last Modified: Mon, 03 Oct 2022 22:50:37 GMT  
		Size: 28.2 MB (28225634 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce6ee8605f9b04da07ee4ce0161573fc9e64faccb9a768733f7222a40ad141c2`  
		Last Modified: Mon, 03 Oct 2022 22:50:31 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:latest` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:3e90150cae10bbf88c2c186563c6307a0a4e7d169d2f640ac04fdda6b08b9b36
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.7 MB (30704302 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3fb461c4c2d15f33277f220c17547fd45eb0d588862147433c0d11afe2bfc1c4`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Tue, 09 Aug 2022 17:39:51 GMT
ADD file:4b51a9d40f20d2beb29d0759b161d2b9403493453beb509de4e86a5d98513f16 in / 
# Tue, 09 Aug 2022 17:39:51 GMT
CMD ["/bin/sh"]
# Fri, 07 Oct 2022 07:38:51 GMT
RUN apk --no-cache add ca-certificates tzdata
# Fri, 07 Oct 2022 07:38:55 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.9.1/traefik_v2.9.1_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Fri, 07 Oct 2022 07:38:56 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Fri, 07 Oct 2022 07:38:56 GMT
EXPOSE 80
# Fri, 07 Oct 2022 07:38:57 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 07 Oct 2022 07:38:58 GMT
CMD ["traefik"]
# Fri, 07 Oct 2022 07:38:59 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.9.1 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:47517142f6ba87eca6b7bdca1e0df160b74671c81e4b9605dad38c1862a43be3`  
		Last Modified: Tue, 09 Aug 2022 17:40:55 GMT  
		Size: 2.7 MB (2718439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24e179f025e9fd053dccf5cf01e48636e8a4fa642091186bc0a736693adbc34f`  
		Last Modified: Fri, 07 Oct 2022 07:40:07 GMT  
		Size: 673.7 KB (673749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94b59dd829100bd144172d2c8d6fa0e5c7c4b18b3f5e621012734841e8b803f7`  
		Last Modified: Fri, 07 Oct 2022 07:40:11 GMT  
		Size: 27.3 MB (27311746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3d7e56d00862713d11472648e728636220fa3aab656c706e800aba3b9be7687`  
		Last Modified: Fri, 07 Oct 2022 07:40:07 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:latest` - linux; s390x

```console
$ docker pull traefik@sha256:86ff93cc178de9b8f86436b83bc6e896c65edb55cda098b94882253afdd3eb1d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.1 MB (32112411 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cb0174719729d126f9205e2bd2f9d55bdd430ac98c573cb2f2b92d2e5c12bcf9`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Tue, 09 Aug 2022 17:41:54 GMT
ADD file:7489fa84133e97e4f40b13dd5159989b3594c9627d9147bfc4e33134944cc368 in / 
# Tue, 09 Aug 2022 17:41:54 GMT
CMD ["/bin/sh"]
# Fri, 07 Oct 2022 09:56:58 GMT
RUN apk --no-cache add ca-certificates tzdata
# Fri, 07 Oct 2022 09:57:06 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.9.1/traefik_v2.9.1_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Fri, 07 Oct 2022 09:57:10 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Fri, 07 Oct 2022 09:57:11 GMT
EXPOSE 80
# Fri, 07 Oct 2022 09:57:12 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 07 Oct 2022 09:57:12 GMT
CMD ["traefik"]
# Fri, 07 Oct 2022 09:57:13 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.9.1 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:cdf710f5b7ee39c5124c50c753228dc9b8b1c1c0a1a38f1413487548565445c3`  
		Last Modified: Tue, 09 Aug 2022 17:42:56 GMT  
		Size: 2.6 MB (2606087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a84a1ec6f28225d3ff13bc2defe049a19ceecab6d949a0e69884c44e7e28279b`  
		Last Modified: Fri, 07 Oct 2022 09:57:42 GMT  
		Size: 677.5 KB (677512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e1d229f8b015fe7609ece81d9725b607d8ca5314d0f08667adfd7c13a5d5daf`  
		Last Modified: Fri, 07 Oct 2022 09:57:46 GMT  
		Size: 28.8 MB (28828444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd924ce12d473d0268c58ca23de4965014be194f51da2ab5fa66fbb94384d8e5`  
		Last Modified: Fri, 07 Oct 2022 09:57:42 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:maroilles`

```console
$ docker pull traefik@sha256:c7ac8f4b5c47b5ee28c3ef93cb46e37e249173605629f775e8f33ffd00b52d04
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:maroilles` - linux; amd64

```console
$ docker pull traefik@sha256:9248f7f17d44a02872613d652aff91856f928ebc400d037cd3439731da4cecbb
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **22.6 MB (22605595 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f2dd394242b858ec3a77eec6506ea614377091f1904f704d3412983c1be8c0cd`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Fri, 07 Oct 2022 04:21:33 GMT
COPY file:48964762d0c961c28f59ebd3ea194fb6486cf2bd9a9cf1780f6702d88bd7b7d9 in /etc/ssl/certs/ 
# Fri, 07 Oct 2022 04:21:34 GMT
COPY dir:c3f72545af4f290c8fc0a43693ea3334451b85d0dee09c519eb983a71a5a38fa in /usr/share/ 
# Fri, 07 Oct 2022 04:21:35 GMT
COPY file:36217e5a6056bef26cfff395c8af8c1010a61dbe8d62b2c7869ca221e2a6302c in / 
# Fri, 07 Oct 2022 04:21:35 GMT
EXPOSE 80
# Fri, 07 Oct 2022 04:21:35 GMT
VOLUME [/tmp]
# Fri, 07 Oct 2022 04:21:35 GMT
ENTRYPOINT ["/traefik"]
# Fri, 07 Oct 2022 04:21:35 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.34 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:39006e619508cd8a1ace2dcb57ecaa3a206fc01c9b72018e30b538ba58b0f45a`  
		Last Modified: Fri, 07 Oct 2022 04:22:39 GMT  
		Size: 123.5 KB (123540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa79c7609bd35acb6baeec95c0534de9f28c053bb3b54b53c4831b70e4a2b6e2`  
		Last Modified: Fri, 07 Oct 2022 04:22:39 GMT  
		Size: 320.1 KB (320103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19b58027c881a56cde12f5ad6ba79f399d338b083423a96ae8fdb32a53f55af9`  
		Last Modified: Fri, 07 Oct 2022 04:22:44 GMT  
		Size: 22.2 MB (22161952 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:maroilles` - linux; arm variant v6

```console
$ docker pull traefik@sha256:8fccb57b1adeec9e17144aeae1399b8ac4241b11d7b914dd315902a830ba733a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **21.1 MB (21075358 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:92fdada8ccde42d699c1a63cf60e989525bc21342c1ac12e6638ee02d43a4a06`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Thu, 11 Aug 2022 01:14:36 GMT
COPY file:48964762d0c961c28f59ebd3ea194fb6486cf2bd9a9cf1780f6702d88bd7b7d9 in /etc/ssl/certs/ 
# Thu, 11 Aug 2022 01:14:37 GMT
COPY dir:a84372748b89eb90478bb1b120b7c8fff3112421d7f93e50fbeae3f53adc6788 in /usr/share/ 
# Thu, 11 Aug 2022 01:14:38 GMT
COPY file:5d1e7e81e8b77b4f8828eeaf0d30a0f135a949b51396f12ae22af376c36d3129 in / 
# Thu, 11 Aug 2022 01:14:38 GMT
EXPOSE 80
# Thu, 11 Aug 2022 01:14:39 GMT
VOLUME [/tmp]
# Thu, 11 Aug 2022 01:14:39 GMT
ENTRYPOINT ["/traefik"]
# Thu, 11 Aug 2022 01:14:39 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.34 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:75f0504c96ad5e9ea3bfc1f0fee80ae3ed4a779d16dba3bf3372c959db0857fe`  
		Last Modified: Thu, 11 Aug 2022 01:16:18 GMT  
		Size: 123.5 KB (123540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a29d285728c6dfaea768ae8c8fa72cfb8acdfb637798090ec09469d4a33b9fb4`  
		Last Modified: Thu, 11 Aug 2022 01:16:18 GMT  
		Size: 328.5 KB (328536 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73f2ae5ba0fcd216aa8ef6f62507561e6616937a868c3acfd3046fa039b7e5ce`  
		Last Modified: Thu, 11 Aug 2022 01:16:22 GMT  
		Size: 20.6 MB (20623282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:maroilles` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:fa1d0bc12d9c099cef08d01b3a9eab66778aedf00fbef5b3da0d272333af80d1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **20.6 MB (20574968 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:63349a030de8627c4abdf307b26a78e32c2a18bc376815ff5cbc07ae39722178`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Fri, 07 Oct 2022 07:39:24 GMT
COPY file:48964762d0c961c28f59ebd3ea194fb6486cf2bd9a9cf1780f6702d88bd7b7d9 in /etc/ssl/certs/ 
# Fri, 07 Oct 2022 07:39:25 GMT
COPY dir:c3f72545af4f290c8fc0a43693ea3334451b85d0dee09c519eb983a71a5a38fa in /usr/share/ 
# Fri, 07 Oct 2022 07:39:26 GMT
COPY file:60330593b6644f3f519fd13ce8ee34c2c7ab9994a1420afabbc01926dd1230dd in / 
# Fri, 07 Oct 2022 07:39:26 GMT
EXPOSE 80
# Fri, 07 Oct 2022 07:39:27 GMT
VOLUME [/tmp]
# Fri, 07 Oct 2022 07:39:28 GMT
ENTRYPOINT ["/traefik"]
# Fri, 07 Oct 2022 07:39:29 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.34 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:1151fb31968944320508e292407b79b28626a76d0af23bfcb76650fd6129b93f`  
		Last Modified: Fri, 07 Oct 2022 07:40:55 GMT  
		Size: 123.5 KB (123539 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:019c3a4ad05f22d384ae4ec9a37d144b01923d7a2a5241e8a510dd4d6b6ee5f9`  
		Last Modified: Fri, 07 Oct 2022 07:40:55 GMT  
		Size: 320.1 KB (320082 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d89d15d062829fe9582b412a41e0c33f0050d927582e9f13666017c4f6992017`  
		Last Modified: Fri, 07 Oct 2022 07:40:58 GMT  
		Size: 20.1 MB (20131347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:maroilles-alpine`

```console
$ docker pull traefik@sha256:5df35f40f618c30e4458d0f23591c74818cab81f889110db2de86a0640dc127f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:maroilles-alpine` - linux; amd64

```console
$ docker pull traefik@sha256:26fa7cd56b81852ea9f61e45df0913aab21313dc3ceeab8a893916893b533054
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.7 MB (25662747 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:16d7c99e10d8ab1a83a9b8ae9755e9912e39a2a9e52da6ce6de8defc71809bd8`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Tue, 09 Aug 2022 17:20:07 GMT
ADD file:b9bd10cf83356cb7281baa0fbaca5186cf27491f59eda87abe57f83a5aaf5ec1 in / 
# Tue, 09 Aug 2022 17:20:08 GMT
CMD ["/bin/sh"]
# Fri, 07 Oct 2022 04:21:23 GMT
RUN apk --no-cache add ca-certificates tzdata
# Fri, 07 Oct 2022 04:21:27 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/traefik/traefik/releases/download/v1.7.34/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Fri, 07 Oct 2022 04:21:27 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Fri, 07 Oct 2022 04:21:27 GMT
EXPOSE 80
# Fri, 07 Oct 2022 04:21:27 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 07 Oct 2022 04:21:28 GMT
CMD ["traefik"]
# Fri, 07 Oct 2022 04:21:28 GMT
LABEL org.opencontainers.image.vendor=traefik org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.34 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:c7ed990a2339ee598662849de4f56e2241399f5a32340c8c4a7bbd5378a12b5f`  
		Last Modified: Tue, 09 Aug 2022 17:21:06 GMT  
		Size: 2.8 MB (2827489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02345b26a3d377d58f815ff68ead6a7dd73b699f6c32431c8d20e8f089729c37`  
		Last Modified: Fri, 07 Oct 2022 04:22:19 GMT  
		Size: 672.8 KB (672839 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fedb3d96d801ee542c140b3c61969835a610feec705ca8958b056cca584fce66`  
		Last Modified: Fri, 07 Oct 2022 04:22:23 GMT  
		Size: 22.2 MB (22162052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4889541507d1292f1cc22ab716fe900b3cf01a14362a5fe85f91fbf67a75cee`  
		Last Modified: Fri, 07 Oct 2022 04:22:19 GMT  
		Size: 367.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:maroilles-alpine` - linux; arm variant v6

```console
$ docker pull traefik@sha256:aa449bd11477cfbcb2023958b4a006fe8c5c7cd93eb3dbb30a7014356686ed20
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.9 MB (23945270 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9c0445b729681b5642ccc3eae945721e8d39c71806b442cace900bca97537cc6`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Tue, 09 Aug 2022 17:49:35 GMT
ADD file:8ff80989f06f5a8ffe16c56e00538928dcb1e46faa2b58ab9c14c7227a6cd8f9 in / 
# Tue, 09 Aug 2022 17:49:35 GMT
CMD ["/bin/sh"]
# Thu, 11 Aug 2022 01:14:24 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 11 Aug 2022 01:14:28 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/traefik/traefik/releases/download/v1.7.34/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Thu, 11 Aug 2022 01:14:29 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 11 Aug 2022 01:14:29 GMT
EXPOSE 80
# Thu, 11 Aug 2022 01:14:29 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 11 Aug 2022 01:14:29 GMT
CMD ["traefik"]
# Thu, 11 Aug 2022 01:14:29 GMT
LABEL org.opencontainers.image.vendor=traefik org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.34 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:7d147289082e6aa6ef510c09d7c0ac8b5026e0b591f1bfcaf01ceada43c9ec65`  
		Last Modified: Tue, 09 Aug 2022 17:51:04 GMT  
		Size: 2.6 MB (2635498 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c46f6fc1fc29e436e3a75b410a2801637bb73995aa0e7b64b676b17443a973f9`  
		Last Modified: Thu, 11 Aug 2022 01:15:55 GMT  
		Size: 686.0 KB (685981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1fe741c4fe2d8bec0997fa1b514de659d0daa075215ec13d7259b7388c56612`  
		Last Modified: Thu, 11 Aug 2022 01:15:58 GMT  
		Size: 20.6 MB (20623422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fc60ca867112243a32bb0d4db8b9f289c30d55b72fa2c4c20dd21d2ebb4edc1`  
		Last Modified: Thu, 11 Aug 2022 01:15:55 GMT  
		Size: 369.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:maroilles-alpine` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:81bc86d35c76c5a6289b2162ab33431e5e7e814c51400a1624d4726d3d5d913c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.5 MB (23527631 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:94a85707debaaa6d4e90402c73e5ec37e7965c0699c6fd71cb0b8123b62110bd`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Tue, 09 Aug 2022 17:39:59 GMT
ADD file:b312c8f512719efd09811d17c2b250bbad03cf3f90c135a00695cc8e152f4ee2 in / 
# Tue, 09 Aug 2022 17:39:59 GMT
CMD ["/bin/sh"]
# Fri, 07 Oct 2022 07:39:08 GMT
RUN apk --no-cache add ca-certificates tzdata
# Fri, 07 Oct 2022 07:39:11 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/traefik/traefik/releases/download/v1.7.34/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Fri, 07 Oct 2022 07:39:13 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Fri, 07 Oct 2022 07:39:13 GMT
EXPOSE 80
# Fri, 07 Oct 2022 07:39:14 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 07 Oct 2022 07:39:15 GMT
CMD ["traefik"]
# Fri, 07 Oct 2022 07:39:16 GMT
LABEL org.opencontainers.image.vendor=traefik org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.34 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:90cda3b7c32511829cd5ae9074240c36c34507085acb6e55b96f993740d2be93`  
		Last Modified: Tue, 09 Aug 2022 17:41:06 GMT  
		Size: 2.7 MB (2722153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43c315e6d7f9d205ba53331de71d2e455d2f6c238e3916ea0fa90c6aeb56ba18`  
		Last Modified: Fri, 07 Oct 2022 07:40:33 GMT  
		Size: 673.7 KB (673730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e0303139d79db6c9786dbdd349cfc46e7aeb686ba6a142bdc12ae48112fcbe6`  
		Last Modified: Fri, 07 Oct 2022 07:40:36 GMT  
		Size: 20.1 MB (20131379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02ee5cf74fa4c8b0e9c2567d694100f1ce2406b150d66b21b1af5880b839eaad`  
		Last Modified: Fri, 07 Oct 2022 07:40:33 GMT  
		Size: 369.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:maroilles-windowsservercore-1809`

```console
$ docker pull traefik@sha256:7c233c425c02be64e4d02c6ac904f8fd586214173652667ed12a6cbe40b35251
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3406; amd64

### `traefik:maroilles-windowsservercore-1809` - windows version 10.0.17763.3406; amd64

```console
$ docker pull traefik@sha256:3cfa84be7d7e57c654a1a3b8e4c41b7ba5f3c5c550cb0174b550c2db0c88be3b
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2726409092 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0fe8cd7f2792b2846bba0ec097dd8b13686688eaacc32a4e789952137e619ede`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Fri, 09 Sep 2022 22:43:02 GMT
RUN Install update 10.0.17763.3406
# Tue, 13 Sep 2022 18:21:27 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 13 Sep 2022 18:24:55 GMT
RUN Invoke-WebRequest     -Uri "https://github.com/traefik/traefik/releases/download/v1.7.34/traefik_windows-amd64.exe"     -OutFile "/traefik.exe"
# Tue, 13 Sep 2022 18:24:56 GMT
EXPOSE 80
# Tue, 13 Sep 2022 18:24:57 GMT
ENTRYPOINT ["/traefik"]
# Tue, 13 Sep 2022 18:24:57 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.34 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:b111c3320c949bea81612bf4554f1b6592c2f504920b5bf57ba340a1d4d52c93`  
		Size: 1.9 GB (1877166088 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:cee64bf279e2ca8e924884a10ecb98bfa79c7f0cc8d25e73039b9aeb940815b6`  
		Size: 826.4 MB (826398623 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:2bc395c8c47e61e593d2e905e0e051d40e7d25e4aeac7dbe08d3ec57acd0e68f`  
		Last Modified: Tue, 13 Sep 2022 18:25:24 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fef8fcae363c967cdda31871dbfcc00b3f35458cbfcba05f7a6d1552c3b9d83c`  
		Last Modified: Tue, 13 Sep 2022 18:25:55 GMT  
		Size: 22.8 MB (22838714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c14ce042369487448642ab933c5aaf18199baa6713c317cbae8067107daeaeca`  
		Last Modified: Tue, 13 Sep 2022 18:25:49 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1836085afff7fe0b9beb9748abe6f34d94003944e2981312832ee76886845d5`  
		Last Modified: Tue, 13 Sep 2022 18:25:52 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24edcfd0e075a20e436658f609f8aa0212feb2c0739e613d2cd95a333639bfe3`  
		Last Modified: Tue, 13 Sep 2022 18:25:49 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v1.7`

```console
$ docker pull traefik@sha256:c7ac8f4b5c47b5ee28c3ef93cb46e37e249173605629f775e8f33ffd00b52d04
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:v1.7` - linux; amd64

```console
$ docker pull traefik@sha256:9248f7f17d44a02872613d652aff91856f928ebc400d037cd3439731da4cecbb
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **22.6 MB (22605595 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f2dd394242b858ec3a77eec6506ea614377091f1904f704d3412983c1be8c0cd`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Fri, 07 Oct 2022 04:21:33 GMT
COPY file:48964762d0c961c28f59ebd3ea194fb6486cf2bd9a9cf1780f6702d88bd7b7d9 in /etc/ssl/certs/ 
# Fri, 07 Oct 2022 04:21:34 GMT
COPY dir:c3f72545af4f290c8fc0a43693ea3334451b85d0dee09c519eb983a71a5a38fa in /usr/share/ 
# Fri, 07 Oct 2022 04:21:35 GMT
COPY file:36217e5a6056bef26cfff395c8af8c1010a61dbe8d62b2c7869ca221e2a6302c in / 
# Fri, 07 Oct 2022 04:21:35 GMT
EXPOSE 80
# Fri, 07 Oct 2022 04:21:35 GMT
VOLUME [/tmp]
# Fri, 07 Oct 2022 04:21:35 GMT
ENTRYPOINT ["/traefik"]
# Fri, 07 Oct 2022 04:21:35 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.34 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:39006e619508cd8a1ace2dcb57ecaa3a206fc01c9b72018e30b538ba58b0f45a`  
		Last Modified: Fri, 07 Oct 2022 04:22:39 GMT  
		Size: 123.5 KB (123540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa79c7609bd35acb6baeec95c0534de9f28c053bb3b54b53c4831b70e4a2b6e2`  
		Last Modified: Fri, 07 Oct 2022 04:22:39 GMT  
		Size: 320.1 KB (320103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19b58027c881a56cde12f5ad6ba79f399d338b083423a96ae8fdb32a53f55af9`  
		Last Modified: Fri, 07 Oct 2022 04:22:44 GMT  
		Size: 22.2 MB (22161952 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v1.7` - linux; arm variant v6

```console
$ docker pull traefik@sha256:8fccb57b1adeec9e17144aeae1399b8ac4241b11d7b914dd315902a830ba733a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **21.1 MB (21075358 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:92fdada8ccde42d699c1a63cf60e989525bc21342c1ac12e6638ee02d43a4a06`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Thu, 11 Aug 2022 01:14:36 GMT
COPY file:48964762d0c961c28f59ebd3ea194fb6486cf2bd9a9cf1780f6702d88bd7b7d9 in /etc/ssl/certs/ 
# Thu, 11 Aug 2022 01:14:37 GMT
COPY dir:a84372748b89eb90478bb1b120b7c8fff3112421d7f93e50fbeae3f53adc6788 in /usr/share/ 
# Thu, 11 Aug 2022 01:14:38 GMT
COPY file:5d1e7e81e8b77b4f8828eeaf0d30a0f135a949b51396f12ae22af376c36d3129 in / 
# Thu, 11 Aug 2022 01:14:38 GMT
EXPOSE 80
# Thu, 11 Aug 2022 01:14:39 GMT
VOLUME [/tmp]
# Thu, 11 Aug 2022 01:14:39 GMT
ENTRYPOINT ["/traefik"]
# Thu, 11 Aug 2022 01:14:39 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.34 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:75f0504c96ad5e9ea3bfc1f0fee80ae3ed4a779d16dba3bf3372c959db0857fe`  
		Last Modified: Thu, 11 Aug 2022 01:16:18 GMT  
		Size: 123.5 KB (123540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a29d285728c6dfaea768ae8c8fa72cfb8acdfb637798090ec09469d4a33b9fb4`  
		Last Modified: Thu, 11 Aug 2022 01:16:18 GMT  
		Size: 328.5 KB (328536 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73f2ae5ba0fcd216aa8ef6f62507561e6616937a868c3acfd3046fa039b7e5ce`  
		Last Modified: Thu, 11 Aug 2022 01:16:22 GMT  
		Size: 20.6 MB (20623282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v1.7` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:fa1d0bc12d9c099cef08d01b3a9eab66778aedf00fbef5b3da0d272333af80d1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **20.6 MB (20574968 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:63349a030de8627c4abdf307b26a78e32c2a18bc376815ff5cbc07ae39722178`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Fri, 07 Oct 2022 07:39:24 GMT
COPY file:48964762d0c961c28f59ebd3ea194fb6486cf2bd9a9cf1780f6702d88bd7b7d9 in /etc/ssl/certs/ 
# Fri, 07 Oct 2022 07:39:25 GMT
COPY dir:c3f72545af4f290c8fc0a43693ea3334451b85d0dee09c519eb983a71a5a38fa in /usr/share/ 
# Fri, 07 Oct 2022 07:39:26 GMT
COPY file:60330593b6644f3f519fd13ce8ee34c2c7ab9994a1420afabbc01926dd1230dd in / 
# Fri, 07 Oct 2022 07:39:26 GMT
EXPOSE 80
# Fri, 07 Oct 2022 07:39:27 GMT
VOLUME [/tmp]
# Fri, 07 Oct 2022 07:39:28 GMT
ENTRYPOINT ["/traefik"]
# Fri, 07 Oct 2022 07:39:29 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.34 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:1151fb31968944320508e292407b79b28626a76d0af23bfcb76650fd6129b93f`  
		Last Modified: Fri, 07 Oct 2022 07:40:55 GMT  
		Size: 123.5 KB (123539 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:019c3a4ad05f22d384ae4ec9a37d144b01923d7a2a5241e8a510dd4d6b6ee5f9`  
		Last Modified: Fri, 07 Oct 2022 07:40:55 GMT  
		Size: 320.1 KB (320082 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d89d15d062829fe9582b412a41e0c33f0050d927582e9f13666017c4f6992017`  
		Last Modified: Fri, 07 Oct 2022 07:40:58 GMT  
		Size: 20.1 MB (20131347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v1.7-alpine`

```console
$ docker pull traefik@sha256:5df35f40f618c30e4458d0f23591c74818cab81f889110db2de86a0640dc127f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:v1.7-alpine` - linux; amd64

```console
$ docker pull traefik@sha256:26fa7cd56b81852ea9f61e45df0913aab21313dc3ceeab8a893916893b533054
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.7 MB (25662747 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:16d7c99e10d8ab1a83a9b8ae9755e9912e39a2a9e52da6ce6de8defc71809bd8`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Tue, 09 Aug 2022 17:20:07 GMT
ADD file:b9bd10cf83356cb7281baa0fbaca5186cf27491f59eda87abe57f83a5aaf5ec1 in / 
# Tue, 09 Aug 2022 17:20:08 GMT
CMD ["/bin/sh"]
# Fri, 07 Oct 2022 04:21:23 GMT
RUN apk --no-cache add ca-certificates tzdata
# Fri, 07 Oct 2022 04:21:27 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/traefik/traefik/releases/download/v1.7.34/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Fri, 07 Oct 2022 04:21:27 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Fri, 07 Oct 2022 04:21:27 GMT
EXPOSE 80
# Fri, 07 Oct 2022 04:21:27 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 07 Oct 2022 04:21:28 GMT
CMD ["traefik"]
# Fri, 07 Oct 2022 04:21:28 GMT
LABEL org.opencontainers.image.vendor=traefik org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.34 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:c7ed990a2339ee598662849de4f56e2241399f5a32340c8c4a7bbd5378a12b5f`  
		Last Modified: Tue, 09 Aug 2022 17:21:06 GMT  
		Size: 2.8 MB (2827489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02345b26a3d377d58f815ff68ead6a7dd73b699f6c32431c8d20e8f089729c37`  
		Last Modified: Fri, 07 Oct 2022 04:22:19 GMT  
		Size: 672.8 KB (672839 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fedb3d96d801ee542c140b3c61969835a610feec705ca8958b056cca584fce66`  
		Last Modified: Fri, 07 Oct 2022 04:22:23 GMT  
		Size: 22.2 MB (22162052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4889541507d1292f1cc22ab716fe900b3cf01a14362a5fe85f91fbf67a75cee`  
		Last Modified: Fri, 07 Oct 2022 04:22:19 GMT  
		Size: 367.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v1.7-alpine` - linux; arm variant v6

```console
$ docker pull traefik@sha256:aa449bd11477cfbcb2023958b4a006fe8c5c7cd93eb3dbb30a7014356686ed20
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.9 MB (23945270 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9c0445b729681b5642ccc3eae945721e8d39c71806b442cace900bca97537cc6`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Tue, 09 Aug 2022 17:49:35 GMT
ADD file:8ff80989f06f5a8ffe16c56e00538928dcb1e46faa2b58ab9c14c7227a6cd8f9 in / 
# Tue, 09 Aug 2022 17:49:35 GMT
CMD ["/bin/sh"]
# Thu, 11 Aug 2022 01:14:24 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 11 Aug 2022 01:14:28 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/traefik/traefik/releases/download/v1.7.34/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Thu, 11 Aug 2022 01:14:29 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 11 Aug 2022 01:14:29 GMT
EXPOSE 80
# Thu, 11 Aug 2022 01:14:29 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 11 Aug 2022 01:14:29 GMT
CMD ["traefik"]
# Thu, 11 Aug 2022 01:14:29 GMT
LABEL org.opencontainers.image.vendor=traefik org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.34 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:7d147289082e6aa6ef510c09d7c0ac8b5026e0b591f1bfcaf01ceada43c9ec65`  
		Last Modified: Tue, 09 Aug 2022 17:51:04 GMT  
		Size: 2.6 MB (2635498 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c46f6fc1fc29e436e3a75b410a2801637bb73995aa0e7b64b676b17443a973f9`  
		Last Modified: Thu, 11 Aug 2022 01:15:55 GMT  
		Size: 686.0 KB (685981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1fe741c4fe2d8bec0997fa1b514de659d0daa075215ec13d7259b7388c56612`  
		Last Modified: Thu, 11 Aug 2022 01:15:58 GMT  
		Size: 20.6 MB (20623422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fc60ca867112243a32bb0d4db8b9f289c30d55b72fa2c4c20dd21d2ebb4edc1`  
		Last Modified: Thu, 11 Aug 2022 01:15:55 GMT  
		Size: 369.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v1.7-alpine` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:81bc86d35c76c5a6289b2162ab33431e5e7e814c51400a1624d4726d3d5d913c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.5 MB (23527631 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:94a85707debaaa6d4e90402c73e5ec37e7965c0699c6fd71cb0b8123b62110bd`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Tue, 09 Aug 2022 17:39:59 GMT
ADD file:b312c8f512719efd09811d17c2b250bbad03cf3f90c135a00695cc8e152f4ee2 in / 
# Tue, 09 Aug 2022 17:39:59 GMT
CMD ["/bin/sh"]
# Fri, 07 Oct 2022 07:39:08 GMT
RUN apk --no-cache add ca-certificates tzdata
# Fri, 07 Oct 2022 07:39:11 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/traefik/traefik/releases/download/v1.7.34/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Fri, 07 Oct 2022 07:39:13 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Fri, 07 Oct 2022 07:39:13 GMT
EXPOSE 80
# Fri, 07 Oct 2022 07:39:14 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 07 Oct 2022 07:39:15 GMT
CMD ["traefik"]
# Fri, 07 Oct 2022 07:39:16 GMT
LABEL org.opencontainers.image.vendor=traefik org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.34 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:90cda3b7c32511829cd5ae9074240c36c34507085acb6e55b96f993740d2be93`  
		Last Modified: Tue, 09 Aug 2022 17:41:06 GMT  
		Size: 2.7 MB (2722153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43c315e6d7f9d205ba53331de71d2e455d2f6c238e3916ea0fa90c6aeb56ba18`  
		Last Modified: Fri, 07 Oct 2022 07:40:33 GMT  
		Size: 673.7 KB (673730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e0303139d79db6c9786dbdd349cfc46e7aeb686ba6a142bdc12ae48112fcbe6`  
		Last Modified: Fri, 07 Oct 2022 07:40:36 GMT  
		Size: 20.1 MB (20131379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02ee5cf74fa4c8b0e9c2567d694100f1ce2406b150d66b21b1af5880b839eaad`  
		Last Modified: Fri, 07 Oct 2022 07:40:33 GMT  
		Size: 369.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v1.7-windowsservercore-1809`

```console
$ docker pull traefik@sha256:7c233c425c02be64e4d02c6ac904f8fd586214173652667ed12a6cbe40b35251
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3406; amd64

### `traefik:v1.7-windowsservercore-1809` - windows version 10.0.17763.3406; amd64

```console
$ docker pull traefik@sha256:3cfa84be7d7e57c654a1a3b8e4c41b7ba5f3c5c550cb0174b550c2db0c88be3b
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2726409092 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0fe8cd7f2792b2846bba0ec097dd8b13686688eaacc32a4e789952137e619ede`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Fri, 09 Sep 2022 22:43:02 GMT
RUN Install update 10.0.17763.3406
# Tue, 13 Sep 2022 18:21:27 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 13 Sep 2022 18:24:55 GMT
RUN Invoke-WebRequest     -Uri "https://github.com/traefik/traefik/releases/download/v1.7.34/traefik_windows-amd64.exe"     -OutFile "/traefik.exe"
# Tue, 13 Sep 2022 18:24:56 GMT
EXPOSE 80
# Tue, 13 Sep 2022 18:24:57 GMT
ENTRYPOINT ["/traefik"]
# Tue, 13 Sep 2022 18:24:57 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.34 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:b111c3320c949bea81612bf4554f1b6592c2f504920b5bf57ba340a1d4d52c93`  
		Size: 1.9 GB (1877166088 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:cee64bf279e2ca8e924884a10ecb98bfa79c7f0cc8d25e73039b9aeb940815b6`  
		Size: 826.4 MB (826398623 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:2bc395c8c47e61e593d2e905e0e051d40e7d25e4aeac7dbe08d3ec57acd0e68f`  
		Last Modified: Tue, 13 Sep 2022 18:25:24 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fef8fcae363c967cdda31871dbfcc00b3f35458cbfcba05f7a6d1552c3b9d83c`  
		Last Modified: Tue, 13 Sep 2022 18:25:55 GMT  
		Size: 22.8 MB (22838714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c14ce042369487448642ab933c5aaf18199baa6713c317cbae8067107daeaeca`  
		Last Modified: Tue, 13 Sep 2022 18:25:49 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1836085afff7fe0b9beb9748abe6f34d94003944e2981312832ee76886845d5`  
		Last Modified: Tue, 13 Sep 2022 18:25:52 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24edcfd0e075a20e436658f609f8aa0212feb2c0739e613d2cd95a333639bfe3`  
		Last Modified: Tue, 13 Sep 2022 18:25:49 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v1.7.34`

```console
$ docker pull traefik@sha256:c7ac8f4b5c47b5ee28c3ef93cb46e37e249173605629f775e8f33ffd00b52d04
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:v1.7.34` - linux; amd64

```console
$ docker pull traefik@sha256:9248f7f17d44a02872613d652aff91856f928ebc400d037cd3439731da4cecbb
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **22.6 MB (22605595 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f2dd394242b858ec3a77eec6506ea614377091f1904f704d3412983c1be8c0cd`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Fri, 07 Oct 2022 04:21:33 GMT
COPY file:48964762d0c961c28f59ebd3ea194fb6486cf2bd9a9cf1780f6702d88bd7b7d9 in /etc/ssl/certs/ 
# Fri, 07 Oct 2022 04:21:34 GMT
COPY dir:c3f72545af4f290c8fc0a43693ea3334451b85d0dee09c519eb983a71a5a38fa in /usr/share/ 
# Fri, 07 Oct 2022 04:21:35 GMT
COPY file:36217e5a6056bef26cfff395c8af8c1010a61dbe8d62b2c7869ca221e2a6302c in / 
# Fri, 07 Oct 2022 04:21:35 GMT
EXPOSE 80
# Fri, 07 Oct 2022 04:21:35 GMT
VOLUME [/tmp]
# Fri, 07 Oct 2022 04:21:35 GMT
ENTRYPOINT ["/traefik"]
# Fri, 07 Oct 2022 04:21:35 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.34 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:39006e619508cd8a1ace2dcb57ecaa3a206fc01c9b72018e30b538ba58b0f45a`  
		Last Modified: Fri, 07 Oct 2022 04:22:39 GMT  
		Size: 123.5 KB (123540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa79c7609bd35acb6baeec95c0534de9f28c053bb3b54b53c4831b70e4a2b6e2`  
		Last Modified: Fri, 07 Oct 2022 04:22:39 GMT  
		Size: 320.1 KB (320103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19b58027c881a56cde12f5ad6ba79f399d338b083423a96ae8fdb32a53f55af9`  
		Last Modified: Fri, 07 Oct 2022 04:22:44 GMT  
		Size: 22.2 MB (22161952 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v1.7.34` - linux; arm variant v6

```console
$ docker pull traefik@sha256:8fccb57b1adeec9e17144aeae1399b8ac4241b11d7b914dd315902a830ba733a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **21.1 MB (21075358 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:92fdada8ccde42d699c1a63cf60e989525bc21342c1ac12e6638ee02d43a4a06`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Thu, 11 Aug 2022 01:14:36 GMT
COPY file:48964762d0c961c28f59ebd3ea194fb6486cf2bd9a9cf1780f6702d88bd7b7d9 in /etc/ssl/certs/ 
# Thu, 11 Aug 2022 01:14:37 GMT
COPY dir:a84372748b89eb90478bb1b120b7c8fff3112421d7f93e50fbeae3f53adc6788 in /usr/share/ 
# Thu, 11 Aug 2022 01:14:38 GMT
COPY file:5d1e7e81e8b77b4f8828eeaf0d30a0f135a949b51396f12ae22af376c36d3129 in / 
# Thu, 11 Aug 2022 01:14:38 GMT
EXPOSE 80
# Thu, 11 Aug 2022 01:14:39 GMT
VOLUME [/tmp]
# Thu, 11 Aug 2022 01:14:39 GMT
ENTRYPOINT ["/traefik"]
# Thu, 11 Aug 2022 01:14:39 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.34 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:75f0504c96ad5e9ea3bfc1f0fee80ae3ed4a779d16dba3bf3372c959db0857fe`  
		Last Modified: Thu, 11 Aug 2022 01:16:18 GMT  
		Size: 123.5 KB (123540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a29d285728c6dfaea768ae8c8fa72cfb8acdfb637798090ec09469d4a33b9fb4`  
		Last Modified: Thu, 11 Aug 2022 01:16:18 GMT  
		Size: 328.5 KB (328536 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73f2ae5ba0fcd216aa8ef6f62507561e6616937a868c3acfd3046fa039b7e5ce`  
		Last Modified: Thu, 11 Aug 2022 01:16:22 GMT  
		Size: 20.6 MB (20623282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v1.7.34` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:fa1d0bc12d9c099cef08d01b3a9eab66778aedf00fbef5b3da0d272333af80d1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **20.6 MB (20574968 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:63349a030de8627c4abdf307b26a78e32c2a18bc376815ff5cbc07ae39722178`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Fri, 07 Oct 2022 07:39:24 GMT
COPY file:48964762d0c961c28f59ebd3ea194fb6486cf2bd9a9cf1780f6702d88bd7b7d9 in /etc/ssl/certs/ 
# Fri, 07 Oct 2022 07:39:25 GMT
COPY dir:c3f72545af4f290c8fc0a43693ea3334451b85d0dee09c519eb983a71a5a38fa in /usr/share/ 
# Fri, 07 Oct 2022 07:39:26 GMT
COPY file:60330593b6644f3f519fd13ce8ee34c2c7ab9994a1420afabbc01926dd1230dd in / 
# Fri, 07 Oct 2022 07:39:26 GMT
EXPOSE 80
# Fri, 07 Oct 2022 07:39:27 GMT
VOLUME [/tmp]
# Fri, 07 Oct 2022 07:39:28 GMT
ENTRYPOINT ["/traefik"]
# Fri, 07 Oct 2022 07:39:29 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.34 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:1151fb31968944320508e292407b79b28626a76d0af23bfcb76650fd6129b93f`  
		Last Modified: Fri, 07 Oct 2022 07:40:55 GMT  
		Size: 123.5 KB (123539 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:019c3a4ad05f22d384ae4ec9a37d144b01923d7a2a5241e8a510dd4d6b6ee5f9`  
		Last Modified: Fri, 07 Oct 2022 07:40:55 GMT  
		Size: 320.1 KB (320082 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d89d15d062829fe9582b412a41e0c33f0050d927582e9f13666017c4f6992017`  
		Last Modified: Fri, 07 Oct 2022 07:40:58 GMT  
		Size: 20.1 MB (20131347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v1.7.34-alpine`

```console
$ docker pull traefik@sha256:5df35f40f618c30e4458d0f23591c74818cab81f889110db2de86a0640dc127f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:v1.7.34-alpine` - linux; amd64

```console
$ docker pull traefik@sha256:26fa7cd56b81852ea9f61e45df0913aab21313dc3ceeab8a893916893b533054
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.7 MB (25662747 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:16d7c99e10d8ab1a83a9b8ae9755e9912e39a2a9e52da6ce6de8defc71809bd8`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Tue, 09 Aug 2022 17:20:07 GMT
ADD file:b9bd10cf83356cb7281baa0fbaca5186cf27491f59eda87abe57f83a5aaf5ec1 in / 
# Tue, 09 Aug 2022 17:20:08 GMT
CMD ["/bin/sh"]
# Fri, 07 Oct 2022 04:21:23 GMT
RUN apk --no-cache add ca-certificates tzdata
# Fri, 07 Oct 2022 04:21:27 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/traefik/traefik/releases/download/v1.7.34/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Fri, 07 Oct 2022 04:21:27 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Fri, 07 Oct 2022 04:21:27 GMT
EXPOSE 80
# Fri, 07 Oct 2022 04:21:27 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 07 Oct 2022 04:21:28 GMT
CMD ["traefik"]
# Fri, 07 Oct 2022 04:21:28 GMT
LABEL org.opencontainers.image.vendor=traefik org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.34 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:c7ed990a2339ee598662849de4f56e2241399f5a32340c8c4a7bbd5378a12b5f`  
		Last Modified: Tue, 09 Aug 2022 17:21:06 GMT  
		Size: 2.8 MB (2827489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02345b26a3d377d58f815ff68ead6a7dd73b699f6c32431c8d20e8f089729c37`  
		Last Modified: Fri, 07 Oct 2022 04:22:19 GMT  
		Size: 672.8 KB (672839 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fedb3d96d801ee542c140b3c61969835a610feec705ca8958b056cca584fce66`  
		Last Modified: Fri, 07 Oct 2022 04:22:23 GMT  
		Size: 22.2 MB (22162052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4889541507d1292f1cc22ab716fe900b3cf01a14362a5fe85f91fbf67a75cee`  
		Last Modified: Fri, 07 Oct 2022 04:22:19 GMT  
		Size: 367.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v1.7.34-alpine` - linux; arm variant v6

```console
$ docker pull traefik@sha256:aa449bd11477cfbcb2023958b4a006fe8c5c7cd93eb3dbb30a7014356686ed20
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.9 MB (23945270 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9c0445b729681b5642ccc3eae945721e8d39c71806b442cace900bca97537cc6`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Tue, 09 Aug 2022 17:49:35 GMT
ADD file:8ff80989f06f5a8ffe16c56e00538928dcb1e46faa2b58ab9c14c7227a6cd8f9 in / 
# Tue, 09 Aug 2022 17:49:35 GMT
CMD ["/bin/sh"]
# Thu, 11 Aug 2022 01:14:24 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 11 Aug 2022 01:14:28 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/traefik/traefik/releases/download/v1.7.34/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Thu, 11 Aug 2022 01:14:29 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 11 Aug 2022 01:14:29 GMT
EXPOSE 80
# Thu, 11 Aug 2022 01:14:29 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 11 Aug 2022 01:14:29 GMT
CMD ["traefik"]
# Thu, 11 Aug 2022 01:14:29 GMT
LABEL org.opencontainers.image.vendor=traefik org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.34 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:7d147289082e6aa6ef510c09d7c0ac8b5026e0b591f1bfcaf01ceada43c9ec65`  
		Last Modified: Tue, 09 Aug 2022 17:51:04 GMT  
		Size: 2.6 MB (2635498 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c46f6fc1fc29e436e3a75b410a2801637bb73995aa0e7b64b676b17443a973f9`  
		Last Modified: Thu, 11 Aug 2022 01:15:55 GMT  
		Size: 686.0 KB (685981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1fe741c4fe2d8bec0997fa1b514de659d0daa075215ec13d7259b7388c56612`  
		Last Modified: Thu, 11 Aug 2022 01:15:58 GMT  
		Size: 20.6 MB (20623422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fc60ca867112243a32bb0d4db8b9f289c30d55b72fa2c4c20dd21d2ebb4edc1`  
		Last Modified: Thu, 11 Aug 2022 01:15:55 GMT  
		Size: 369.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v1.7.34-alpine` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:81bc86d35c76c5a6289b2162ab33431e5e7e814c51400a1624d4726d3d5d913c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.5 MB (23527631 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:94a85707debaaa6d4e90402c73e5ec37e7965c0699c6fd71cb0b8123b62110bd`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Tue, 09 Aug 2022 17:39:59 GMT
ADD file:b312c8f512719efd09811d17c2b250bbad03cf3f90c135a00695cc8e152f4ee2 in / 
# Tue, 09 Aug 2022 17:39:59 GMT
CMD ["/bin/sh"]
# Fri, 07 Oct 2022 07:39:08 GMT
RUN apk --no-cache add ca-certificates tzdata
# Fri, 07 Oct 2022 07:39:11 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/traefik/traefik/releases/download/v1.7.34/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Fri, 07 Oct 2022 07:39:13 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Fri, 07 Oct 2022 07:39:13 GMT
EXPOSE 80
# Fri, 07 Oct 2022 07:39:14 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 07 Oct 2022 07:39:15 GMT
CMD ["traefik"]
# Fri, 07 Oct 2022 07:39:16 GMT
LABEL org.opencontainers.image.vendor=traefik org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.34 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:90cda3b7c32511829cd5ae9074240c36c34507085acb6e55b96f993740d2be93`  
		Last Modified: Tue, 09 Aug 2022 17:41:06 GMT  
		Size: 2.7 MB (2722153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43c315e6d7f9d205ba53331de71d2e455d2f6c238e3916ea0fa90c6aeb56ba18`  
		Last Modified: Fri, 07 Oct 2022 07:40:33 GMT  
		Size: 673.7 KB (673730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e0303139d79db6c9786dbdd349cfc46e7aeb686ba6a142bdc12ae48112fcbe6`  
		Last Modified: Fri, 07 Oct 2022 07:40:36 GMT  
		Size: 20.1 MB (20131379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02ee5cf74fa4c8b0e9c2567d694100f1ce2406b150d66b21b1af5880b839eaad`  
		Last Modified: Fri, 07 Oct 2022 07:40:33 GMT  
		Size: 369.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v1.7.34-windowsservercore-1809`

```console
$ docker pull traefik@sha256:7c233c425c02be64e4d02c6ac904f8fd586214173652667ed12a6cbe40b35251
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3406; amd64

### `traefik:v1.7.34-windowsservercore-1809` - windows version 10.0.17763.3406; amd64

```console
$ docker pull traefik@sha256:3cfa84be7d7e57c654a1a3b8e4c41b7ba5f3c5c550cb0174b550c2db0c88be3b
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2726409092 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0fe8cd7f2792b2846bba0ec097dd8b13686688eaacc32a4e789952137e619ede`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Fri, 09 Sep 2022 22:43:02 GMT
RUN Install update 10.0.17763.3406
# Tue, 13 Sep 2022 18:21:27 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 13 Sep 2022 18:24:55 GMT
RUN Invoke-WebRequest     -Uri "https://github.com/traefik/traefik/releases/download/v1.7.34/traefik_windows-amd64.exe"     -OutFile "/traefik.exe"
# Tue, 13 Sep 2022 18:24:56 GMT
EXPOSE 80
# Tue, 13 Sep 2022 18:24:57 GMT
ENTRYPOINT ["/traefik"]
# Tue, 13 Sep 2022 18:24:57 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.34 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:b111c3320c949bea81612bf4554f1b6592c2f504920b5bf57ba340a1d4d52c93`  
		Size: 1.9 GB (1877166088 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:cee64bf279e2ca8e924884a10ecb98bfa79c7f0cc8d25e73039b9aeb940815b6`  
		Size: 826.4 MB (826398623 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:2bc395c8c47e61e593d2e905e0e051d40e7d25e4aeac7dbe08d3ec57acd0e68f`  
		Last Modified: Tue, 13 Sep 2022 18:25:24 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fef8fcae363c967cdda31871dbfcc00b3f35458cbfcba05f7a6d1552c3b9d83c`  
		Last Modified: Tue, 13 Sep 2022 18:25:55 GMT  
		Size: 22.8 MB (22838714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c14ce042369487448642ab933c5aaf18199baa6713c317cbae8067107daeaeca`  
		Last Modified: Tue, 13 Sep 2022 18:25:49 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1836085afff7fe0b9beb9748abe6f34d94003944e2981312832ee76886845d5`  
		Last Modified: Tue, 13 Sep 2022 18:25:52 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24edcfd0e075a20e436658f609f8aa0212feb2c0739e613d2cd95a333639bfe3`  
		Last Modified: Tue, 13 Sep 2022 18:25:49 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v2.9`

```console
$ docker pull traefik@sha256:426f5d4e1432a1d1780a0fe081715d70c667345df1e50b02be57872f3e410628
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; s390x

### `traefik:v2.9` - linux; amd64

```console
$ docker pull traefik@sha256:3eaf50b7874f63567ee5d18498536928faef199302c805cb6b766e06b649302d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.4 MB (33416269 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e6de8578b2384107d9e08f90be5d6cf43472e369ba98dca46373b336b83fdbd8`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Tue, 09 Aug 2022 17:20:00 GMT
ADD file:f77e3f51f020890d22997e6c2ca98968b75b8bc8c463341a2010ff0655d4c88f in / 
# Tue, 09 Aug 2022 17:20:01 GMT
CMD ["/bin/sh"]
# Fri, 07 Oct 2022 04:21:14 GMT
RUN apk --no-cache add ca-certificates tzdata
# Fri, 07 Oct 2022 04:21:18 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.9.1/traefik_v2.9.1_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Fri, 07 Oct 2022 04:21:18 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Fri, 07 Oct 2022 04:21:18 GMT
EXPOSE 80
# Fri, 07 Oct 2022 04:21:18 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 07 Oct 2022 04:21:18 GMT
CMD ["traefik"]
# Fri, 07 Oct 2022 04:21:19 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.9.1 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:9621f1afde84053b2f9b6ff34fc7f7460712247c01cbab483c5fa7132cf782ca`  
		Last Modified: Tue, 09 Aug 2022 17:20:52 GMT  
		Size: 2.8 MB (2823512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f62b4fe8af5e2bd23c9c1a5303b1d320706bc52330058f23c4725df3dadc9cad`  
		Last Modified: Fri, 07 Oct 2022 04:21:55 GMT  
		Size: 673.4 KB (673371 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b954c2c3b6c35a716c65a53d1bb120db920d2cdc90267d260674af3965a5b68`  
		Last Modified: Fri, 07 Oct 2022 04:22:00 GMT  
		Size: 29.9 MB (29919018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:857fadab46062ec62a3b8f3183843ff14b05f3ec377ccbe51a5296f86eacce5f`  
		Last Modified: Fri, 07 Oct 2022 04:21:55 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v2.9` - linux; arm variant v6

```console
$ docker pull traefik@sha256:95960ed785badbe47cd0ec5bfc0833db6502043a7c83d1a14fa495615bd7dbd7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.5 MB (31543171 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:df1030c56c08192fde82ebb2fef3c8b57f7d8d340ac8463f7e563f4637caa60a`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Tue, 09 Aug 2022 17:49:29 GMT
ADD file:89cb25f97e17bed5c56311280efe5cfa78422d8ffbe36232195d13f94d67417e in / 
# Tue, 09 Aug 2022 17:49:29 GMT
CMD ["/bin/sh"]
# Thu, 11 Aug 2022 01:14:12 GMT
RUN apk --no-cache add ca-certificates tzdata
# Mon, 03 Oct 2022 22:49:32 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.9.1/traefik_v2.9.1_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Mon, 03 Oct 2022 22:49:33 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Mon, 03 Oct 2022 22:49:33 GMT
EXPOSE 80
# Mon, 03 Oct 2022 22:49:33 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 03 Oct 2022 22:49:33 GMT
CMD ["traefik"]
# Mon, 03 Oct 2022 22:49:33 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.9.1 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:293b708aa6fb80967f27727d5c9c53ac9ba9cac376bed2ad02c17a5cca317b35`  
		Last Modified: Tue, 09 Aug 2022 17:50:52 GMT  
		Size: 2.6 MB (2631127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:667ecdfbf7665eeb46df55d94a2322221d8d1de9cebdc0f97c05affd0aa619f0`  
		Last Modified: Thu, 11 Aug 2022 01:15:26 GMT  
		Size: 686.0 KB (686042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31d29799c16bfd82dab22b9850857fb3488e2dc721c763c4bcc4fde280c30872`  
		Last Modified: Mon, 03 Oct 2022 22:50:37 GMT  
		Size: 28.2 MB (28225634 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce6ee8605f9b04da07ee4ce0161573fc9e64faccb9a768733f7222a40ad141c2`  
		Last Modified: Mon, 03 Oct 2022 22:50:31 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v2.9` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:3e90150cae10bbf88c2c186563c6307a0a4e7d169d2f640ac04fdda6b08b9b36
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.7 MB (30704302 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3fb461c4c2d15f33277f220c17547fd45eb0d588862147433c0d11afe2bfc1c4`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Tue, 09 Aug 2022 17:39:51 GMT
ADD file:4b51a9d40f20d2beb29d0759b161d2b9403493453beb509de4e86a5d98513f16 in / 
# Tue, 09 Aug 2022 17:39:51 GMT
CMD ["/bin/sh"]
# Fri, 07 Oct 2022 07:38:51 GMT
RUN apk --no-cache add ca-certificates tzdata
# Fri, 07 Oct 2022 07:38:55 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.9.1/traefik_v2.9.1_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Fri, 07 Oct 2022 07:38:56 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Fri, 07 Oct 2022 07:38:56 GMT
EXPOSE 80
# Fri, 07 Oct 2022 07:38:57 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 07 Oct 2022 07:38:58 GMT
CMD ["traefik"]
# Fri, 07 Oct 2022 07:38:59 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.9.1 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:47517142f6ba87eca6b7bdca1e0df160b74671c81e4b9605dad38c1862a43be3`  
		Last Modified: Tue, 09 Aug 2022 17:40:55 GMT  
		Size: 2.7 MB (2718439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24e179f025e9fd053dccf5cf01e48636e8a4fa642091186bc0a736693adbc34f`  
		Last Modified: Fri, 07 Oct 2022 07:40:07 GMT  
		Size: 673.7 KB (673749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94b59dd829100bd144172d2c8d6fa0e5c7c4b18b3f5e621012734841e8b803f7`  
		Last Modified: Fri, 07 Oct 2022 07:40:11 GMT  
		Size: 27.3 MB (27311746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3d7e56d00862713d11472648e728636220fa3aab656c706e800aba3b9be7687`  
		Last Modified: Fri, 07 Oct 2022 07:40:07 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v2.9` - linux; s390x

```console
$ docker pull traefik@sha256:86ff93cc178de9b8f86436b83bc6e896c65edb55cda098b94882253afdd3eb1d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.1 MB (32112411 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cb0174719729d126f9205e2bd2f9d55bdd430ac98c573cb2f2b92d2e5c12bcf9`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Tue, 09 Aug 2022 17:41:54 GMT
ADD file:7489fa84133e97e4f40b13dd5159989b3594c9627d9147bfc4e33134944cc368 in / 
# Tue, 09 Aug 2022 17:41:54 GMT
CMD ["/bin/sh"]
# Fri, 07 Oct 2022 09:56:58 GMT
RUN apk --no-cache add ca-certificates tzdata
# Fri, 07 Oct 2022 09:57:06 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.9.1/traefik_v2.9.1_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Fri, 07 Oct 2022 09:57:10 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Fri, 07 Oct 2022 09:57:11 GMT
EXPOSE 80
# Fri, 07 Oct 2022 09:57:12 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 07 Oct 2022 09:57:12 GMT
CMD ["traefik"]
# Fri, 07 Oct 2022 09:57:13 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.9.1 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:cdf710f5b7ee39c5124c50c753228dc9b8b1c1c0a1a38f1413487548565445c3`  
		Last Modified: Tue, 09 Aug 2022 17:42:56 GMT  
		Size: 2.6 MB (2606087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a84a1ec6f28225d3ff13bc2defe049a19ceecab6d949a0e69884c44e7e28279b`  
		Last Modified: Fri, 07 Oct 2022 09:57:42 GMT  
		Size: 677.5 KB (677512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e1d229f8b015fe7609ece81d9725b607d8ca5314d0f08667adfd7c13a5d5daf`  
		Last Modified: Fri, 07 Oct 2022 09:57:46 GMT  
		Size: 28.8 MB (28828444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd924ce12d473d0268c58ca23de4965014be194f51da2ab5fa66fbb94384d8e5`  
		Last Modified: Fri, 07 Oct 2022 09:57:42 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v2.9-windowsservercore-1809`

```console
$ docker pull traefik@sha256:f30447f41aae80f422d9e54a030544c0aef686d30be9bf2552b7bb5c5e906baa
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3406; amd64

### `traefik:v2.9-windowsservercore-1809` - windows version 10.0.17763.3406; amd64

```console
$ docker pull traefik@sha256:0b774d737eb46e9d8d7ef5395b7a0eb5172b3debcb450d66460ea763137a9c9a
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2733978551 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:47a82dae6c960ec5c9dc6e6e61bd935ee3edeb2bea4e223ef31ed3ac4ee1c041`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Fri, 09 Sep 2022 22:43:02 GMT
RUN Install update 10.0.17763.3406
# Tue, 13 Sep 2022 18:21:27 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Mon, 03 Oct 2022 22:22:40 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/traefik/traefik/releases/download/v2.9.1/traefik_v2.9.1_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Mon, 03 Oct 2022 22:22:41 GMT
EXPOSE 80
# Mon, 03 Oct 2022 22:22:42 GMT
ENTRYPOINT ["/traefik"]
# Mon, 03 Oct 2022 22:22:43 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.9.1 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:b111c3320c949bea81612bf4554f1b6592c2f504920b5bf57ba340a1d4d52c93`  
		Size: 1.9 GB (1877166088 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:cee64bf279e2ca8e924884a10ecb98bfa79c7f0cc8d25e73039b9aeb940815b6`  
		Size: 826.4 MB (826398623 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:2bc395c8c47e61e593d2e905e0e051d40e7d25e4aeac7dbe08d3ec57acd0e68f`  
		Last Modified: Tue, 13 Sep 2022 18:25:24 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c7765a94b2fc5ac1ba474cd067a9942ed01008e08eefadb55cc32c40dcfb695`  
		Last Modified: Mon, 03 Oct 2022 22:23:25 GMT  
		Size: 30.4 MB (30408185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51b834274d250812b031261d0107840c5a20f3f21da74e9210818321ecff1a37`  
		Last Modified: Mon, 03 Oct 2022 22:23:18 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a51c1e6b70f0a0702f1f5a84a0e10573577c14f197262205dc63ed5f75f5b3b`  
		Last Modified: Mon, 03 Oct 2022 22:23:18 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3770a98f22a4479168ce9f4fdfc7e714e1adc958f7bb8b565c500658ea8ad298`  
		Last Modified: Mon, 03 Oct 2022 22:23:18 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v2.9.1`

```console
$ docker pull traefik@sha256:426f5d4e1432a1d1780a0fe081715d70c667345df1e50b02be57872f3e410628
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; s390x

### `traefik:v2.9.1` - linux; amd64

```console
$ docker pull traefik@sha256:3eaf50b7874f63567ee5d18498536928faef199302c805cb6b766e06b649302d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.4 MB (33416269 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e6de8578b2384107d9e08f90be5d6cf43472e369ba98dca46373b336b83fdbd8`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Tue, 09 Aug 2022 17:20:00 GMT
ADD file:f77e3f51f020890d22997e6c2ca98968b75b8bc8c463341a2010ff0655d4c88f in / 
# Tue, 09 Aug 2022 17:20:01 GMT
CMD ["/bin/sh"]
# Fri, 07 Oct 2022 04:21:14 GMT
RUN apk --no-cache add ca-certificates tzdata
# Fri, 07 Oct 2022 04:21:18 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.9.1/traefik_v2.9.1_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Fri, 07 Oct 2022 04:21:18 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Fri, 07 Oct 2022 04:21:18 GMT
EXPOSE 80
# Fri, 07 Oct 2022 04:21:18 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 07 Oct 2022 04:21:18 GMT
CMD ["traefik"]
# Fri, 07 Oct 2022 04:21:19 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.9.1 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:9621f1afde84053b2f9b6ff34fc7f7460712247c01cbab483c5fa7132cf782ca`  
		Last Modified: Tue, 09 Aug 2022 17:20:52 GMT  
		Size: 2.8 MB (2823512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f62b4fe8af5e2bd23c9c1a5303b1d320706bc52330058f23c4725df3dadc9cad`  
		Last Modified: Fri, 07 Oct 2022 04:21:55 GMT  
		Size: 673.4 KB (673371 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b954c2c3b6c35a716c65a53d1bb120db920d2cdc90267d260674af3965a5b68`  
		Last Modified: Fri, 07 Oct 2022 04:22:00 GMT  
		Size: 29.9 MB (29919018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:857fadab46062ec62a3b8f3183843ff14b05f3ec377ccbe51a5296f86eacce5f`  
		Last Modified: Fri, 07 Oct 2022 04:21:55 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v2.9.1` - linux; arm variant v6

```console
$ docker pull traefik@sha256:95960ed785badbe47cd0ec5bfc0833db6502043a7c83d1a14fa495615bd7dbd7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.5 MB (31543171 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:df1030c56c08192fde82ebb2fef3c8b57f7d8d340ac8463f7e563f4637caa60a`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Tue, 09 Aug 2022 17:49:29 GMT
ADD file:89cb25f97e17bed5c56311280efe5cfa78422d8ffbe36232195d13f94d67417e in / 
# Tue, 09 Aug 2022 17:49:29 GMT
CMD ["/bin/sh"]
# Thu, 11 Aug 2022 01:14:12 GMT
RUN apk --no-cache add ca-certificates tzdata
# Mon, 03 Oct 2022 22:49:32 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.9.1/traefik_v2.9.1_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Mon, 03 Oct 2022 22:49:33 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Mon, 03 Oct 2022 22:49:33 GMT
EXPOSE 80
# Mon, 03 Oct 2022 22:49:33 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 03 Oct 2022 22:49:33 GMT
CMD ["traefik"]
# Mon, 03 Oct 2022 22:49:33 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.9.1 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:293b708aa6fb80967f27727d5c9c53ac9ba9cac376bed2ad02c17a5cca317b35`  
		Last Modified: Tue, 09 Aug 2022 17:50:52 GMT  
		Size: 2.6 MB (2631127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:667ecdfbf7665eeb46df55d94a2322221d8d1de9cebdc0f97c05affd0aa619f0`  
		Last Modified: Thu, 11 Aug 2022 01:15:26 GMT  
		Size: 686.0 KB (686042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31d29799c16bfd82dab22b9850857fb3488e2dc721c763c4bcc4fde280c30872`  
		Last Modified: Mon, 03 Oct 2022 22:50:37 GMT  
		Size: 28.2 MB (28225634 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce6ee8605f9b04da07ee4ce0161573fc9e64faccb9a768733f7222a40ad141c2`  
		Last Modified: Mon, 03 Oct 2022 22:50:31 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v2.9.1` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:3e90150cae10bbf88c2c186563c6307a0a4e7d169d2f640ac04fdda6b08b9b36
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.7 MB (30704302 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3fb461c4c2d15f33277f220c17547fd45eb0d588862147433c0d11afe2bfc1c4`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Tue, 09 Aug 2022 17:39:51 GMT
ADD file:4b51a9d40f20d2beb29d0759b161d2b9403493453beb509de4e86a5d98513f16 in / 
# Tue, 09 Aug 2022 17:39:51 GMT
CMD ["/bin/sh"]
# Fri, 07 Oct 2022 07:38:51 GMT
RUN apk --no-cache add ca-certificates tzdata
# Fri, 07 Oct 2022 07:38:55 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.9.1/traefik_v2.9.1_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Fri, 07 Oct 2022 07:38:56 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Fri, 07 Oct 2022 07:38:56 GMT
EXPOSE 80
# Fri, 07 Oct 2022 07:38:57 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 07 Oct 2022 07:38:58 GMT
CMD ["traefik"]
# Fri, 07 Oct 2022 07:38:59 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.9.1 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:47517142f6ba87eca6b7bdca1e0df160b74671c81e4b9605dad38c1862a43be3`  
		Last Modified: Tue, 09 Aug 2022 17:40:55 GMT  
		Size: 2.7 MB (2718439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24e179f025e9fd053dccf5cf01e48636e8a4fa642091186bc0a736693adbc34f`  
		Last Modified: Fri, 07 Oct 2022 07:40:07 GMT  
		Size: 673.7 KB (673749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94b59dd829100bd144172d2c8d6fa0e5c7c4b18b3f5e621012734841e8b803f7`  
		Last Modified: Fri, 07 Oct 2022 07:40:11 GMT  
		Size: 27.3 MB (27311746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3d7e56d00862713d11472648e728636220fa3aab656c706e800aba3b9be7687`  
		Last Modified: Fri, 07 Oct 2022 07:40:07 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v2.9.1` - linux; s390x

```console
$ docker pull traefik@sha256:86ff93cc178de9b8f86436b83bc6e896c65edb55cda098b94882253afdd3eb1d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.1 MB (32112411 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cb0174719729d126f9205e2bd2f9d55bdd430ac98c573cb2f2b92d2e5c12bcf9`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Tue, 09 Aug 2022 17:41:54 GMT
ADD file:7489fa84133e97e4f40b13dd5159989b3594c9627d9147bfc4e33134944cc368 in / 
# Tue, 09 Aug 2022 17:41:54 GMT
CMD ["/bin/sh"]
# Fri, 07 Oct 2022 09:56:58 GMT
RUN apk --no-cache add ca-certificates tzdata
# Fri, 07 Oct 2022 09:57:06 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.9.1/traefik_v2.9.1_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Fri, 07 Oct 2022 09:57:10 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Fri, 07 Oct 2022 09:57:11 GMT
EXPOSE 80
# Fri, 07 Oct 2022 09:57:12 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 07 Oct 2022 09:57:12 GMT
CMD ["traefik"]
# Fri, 07 Oct 2022 09:57:13 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.9.1 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:cdf710f5b7ee39c5124c50c753228dc9b8b1c1c0a1a38f1413487548565445c3`  
		Last Modified: Tue, 09 Aug 2022 17:42:56 GMT  
		Size: 2.6 MB (2606087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a84a1ec6f28225d3ff13bc2defe049a19ceecab6d949a0e69884c44e7e28279b`  
		Last Modified: Fri, 07 Oct 2022 09:57:42 GMT  
		Size: 677.5 KB (677512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e1d229f8b015fe7609ece81d9725b607d8ca5314d0f08667adfd7c13a5d5daf`  
		Last Modified: Fri, 07 Oct 2022 09:57:46 GMT  
		Size: 28.8 MB (28828444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd924ce12d473d0268c58ca23de4965014be194f51da2ab5fa66fbb94384d8e5`  
		Last Modified: Fri, 07 Oct 2022 09:57:42 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v2.9.1-windowsservercore-1809`

```console
$ docker pull traefik@sha256:f30447f41aae80f422d9e54a030544c0aef686d30be9bf2552b7bb5c5e906baa
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3406; amd64

### `traefik:v2.9.1-windowsservercore-1809` - windows version 10.0.17763.3406; amd64

```console
$ docker pull traefik@sha256:0b774d737eb46e9d8d7ef5395b7a0eb5172b3debcb450d66460ea763137a9c9a
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2733978551 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:47a82dae6c960ec5c9dc6e6e61bd935ee3edeb2bea4e223ef31ed3ac4ee1c041`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Fri, 09 Sep 2022 22:43:02 GMT
RUN Install update 10.0.17763.3406
# Tue, 13 Sep 2022 18:21:27 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Mon, 03 Oct 2022 22:22:40 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/traefik/traefik/releases/download/v2.9.1/traefik_v2.9.1_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Mon, 03 Oct 2022 22:22:41 GMT
EXPOSE 80
# Mon, 03 Oct 2022 22:22:42 GMT
ENTRYPOINT ["/traefik"]
# Mon, 03 Oct 2022 22:22:43 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.9.1 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:b111c3320c949bea81612bf4554f1b6592c2f504920b5bf57ba340a1d4d52c93`  
		Size: 1.9 GB (1877166088 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:cee64bf279e2ca8e924884a10ecb98bfa79c7f0cc8d25e73039b9aeb940815b6`  
		Size: 826.4 MB (826398623 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:2bc395c8c47e61e593d2e905e0e051d40e7d25e4aeac7dbe08d3ec57acd0e68f`  
		Last Modified: Tue, 13 Sep 2022 18:25:24 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c7765a94b2fc5ac1ba474cd067a9942ed01008e08eefadb55cc32c40dcfb695`  
		Last Modified: Mon, 03 Oct 2022 22:23:25 GMT  
		Size: 30.4 MB (30408185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51b834274d250812b031261d0107840c5a20f3f21da74e9210818321ecff1a37`  
		Last Modified: Mon, 03 Oct 2022 22:23:18 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a51c1e6b70f0a0702f1f5a84a0e10573577c14f197262205dc63ed5f75f5b3b`  
		Last Modified: Mon, 03 Oct 2022 22:23:18 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3770a98f22a4479168ce9f4fdfc7e714e1adc958f7bb8b565c500658ea8ad298`  
		Last Modified: Mon, 03 Oct 2022 22:23:18 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:windowsservercore-1809`

```console
$ docker pull traefik@sha256:f30447f41aae80f422d9e54a030544c0aef686d30be9bf2552b7bb5c5e906baa
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3406; amd64

### `traefik:windowsservercore-1809` - windows version 10.0.17763.3406; amd64

```console
$ docker pull traefik@sha256:0b774d737eb46e9d8d7ef5395b7a0eb5172b3debcb450d66460ea763137a9c9a
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2733978551 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:47a82dae6c960ec5c9dc6e6e61bd935ee3edeb2bea4e223ef31ed3ac4ee1c041`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Fri, 09 Sep 2022 22:43:02 GMT
RUN Install update 10.0.17763.3406
# Tue, 13 Sep 2022 18:21:27 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Mon, 03 Oct 2022 22:22:40 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/traefik/traefik/releases/download/v2.9.1/traefik_v2.9.1_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Mon, 03 Oct 2022 22:22:41 GMT
EXPOSE 80
# Mon, 03 Oct 2022 22:22:42 GMT
ENTRYPOINT ["/traefik"]
# Mon, 03 Oct 2022 22:22:43 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.9.1 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:b111c3320c949bea81612bf4554f1b6592c2f504920b5bf57ba340a1d4d52c93`  
		Size: 1.9 GB (1877166088 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:cee64bf279e2ca8e924884a10ecb98bfa79c7f0cc8d25e73039b9aeb940815b6`  
		Size: 826.4 MB (826398623 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:2bc395c8c47e61e593d2e905e0e051d40e7d25e4aeac7dbe08d3ec57acd0e68f`  
		Last Modified: Tue, 13 Sep 2022 18:25:24 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c7765a94b2fc5ac1ba474cd067a9942ed01008e08eefadb55cc32c40dcfb695`  
		Last Modified: Mon, 03 Oct 2022 22:23:25 GMT  
		Size: 30.4 MB (30408185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51b834274d250812b031261d0107840c5a20f3f21da74e9210818321ecff1a37`  
		Last Modified: Mon, 03 Oct 2022 22:23:18 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a51c1e6b70f0a0702f1f5a84a0e10573577c14f197262205dc63ed5f75f5b3b`  
		Last Modified: Mon, 03 Oct 2022 22:23:18 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3770a98f22a4479168ce9f4fdfc7e714e1adc958f7bb8b565c500658ea8ad298`  
		Last Modified: Mon, 03 Oct 2022 22:23:18 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
