<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `traefik`

-	[`traefik:1.7`](#traefik17)
-	[`traefik:1.7.20`](#traefik1720)
-	[`traefik:1.7.20-alpine`](#traefik1720-alpine)
-	[`traefik:1.7.20-windowsservercore-1809`](#traefik1720-windowsservercore-1809)
-	[`traefik:1.7-alpine`](#traefik17-alpine)
-	[`traefik:1.7-windowsservercore-1809`](#traefik17-windowsservercore-1809)
-	[`traefik:2.1`](#traefik21)
-	[`traefik:2.1.2`](#traefik212)
-	[`traefik:2.1.2-windowsservercore-1809`](#traefik212-windowsservercore-1809)
-	[`traefik:2.1-windowsservercore-1809`](#traefik21-windowsservercore-1809)
-	[`traefik:cantal`](#traefikcantal)
-	[`traefik:cantal-windowsservercore-1809`](#traefikcantal-windowsservercore-1809)
-	[`traefik:latest`](#traefiklatest)
-	[`traefik:maroilles`](#traefikmaroilles)
-	[`traefik:maroilles-alpine`](#traefikmaroilles-alpine)
-	[`traefik:maroilles-windowsservercore-1809`](#traefikmaroilles-windowsservercore-1809)
-	[`traefik:v1.7`](#traefikv17)
-	[`traefik:v1.7.20`](#traefikv1720)
-	[`traefik:v1.7.20-alpine`](#traefikv1720-alpine)
-	[`traefik:v1.7.20-windowsservercore-1809`](#traefikv1720-windowsservercore-1809)
-	[`traefik:v1.7-alpine`](#traefikv17-alpine)
-	[`traefik:v1.7-windowsservercore-1809`](#traefikv17-windowsservercore-1809)
-	[`traefik:v2.1`](#traefikv21)
-	[`traefik:v2.1.2`](#traefikv212)
-	[`traefik:v2.1.2-windowsservercore-1809`](#traefikv212-windowsservercore-1809)
-	[`traefik:v2.1-windowsservercore-1809`](#traefikv21-windowsservercore-1809)
-	[`traefik:windowsservercore-1809`](#traefikwindowsservercore-1809)

## `traefik:1.7`

```console
$ docker pull traefik@sha256:5ec34caf19d114f8f0ed76f9bc3dad6ba8cf6d13a1575c4294b59b77709def39
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:1.7` - linux; amd64

```console
$ docker pull traefik@sha256:3b1c4d57c57d125a5d949d463d41882fefc957ce117db226aace4e7314e82d5c
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **24.0 MB (24005352 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:96c63a7d3e502fcbbd8937a2523368c22d0edd1788b8389af095f64038318834`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Tue, 27 Aug 2019 01:00:22 GMT
COPY file:091d2a65366d205fc0db557b2f495da40adb5a33c9d656d02c3ea08bb22f6c4d in /etc/ssl/certs/ 
# Mon, 21 Oct 2019 22:26:52 GMT
COPY dir:e700a731062c6a1130194c74080171046494718874f8e586f78523a64d56715c in /usr/share/ 
# Tue, 10 Dec 2019 22:31:38 GMT
COPY file:be1ea92a6d3f63051c9ae787ca41c986b81a56ce7f8b8347b97c3ddc3b4471f5 in / 
# Tue, 10 Dec 2019 22:31:38 GMT
EXPOSE 80
# Tue, 10 Dec 2019 22:31:38 GMT
VOLUME [/tmp]
# Tue, 10 Dec 2019 22:31:38 GMT
ENTRYPOINT ["/traefik"]
# Tue, 10 Dec 2019 22:31:39 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.20 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:42e7d26ec3785f8ce0f20e327cf72404ee054ba022ce9068ad2d28c52e82db2a`  
		Last Modified: Tue, 27 Aug 2019 01:00:52 GMT  
		Size: 132.0 KB (132022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a753f02eeffef33e5e071a6feac9e12fffb36330fc7ef5441f378d0ce67c528`  
		Last Modified: Mon, 21 Oct 2019 22:27:25 GMT  
		Size: 327.3 KB (327346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab927d94d255c72862c3e7ada3f6cdb36f90926b7a8913a080062b17d73f186b`  
		Last Modified: Tue, 10 Dec 2019 22:32:27 GMT  
		Size: 23.5 MB (23545984 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:1.7` - linux; arm variant v6

```console
$ docker pull traefik@sha256:3a32e589b7d538f688f0a4d5777ab21dc2e946e22a1b08872aaad72b4192976e
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **22.5 MB (22491539 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:099411d81ac7bf28b232625f19ecc6590f39c3920418958b3056caa4f85815c4`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Mon, 26 Aug 2019 23:54:26 GMT
COPY file:091d2a65366d205fc0db557b2f495da40adb5a33c9d656d02c3ea08bb22f6c4d in /etc/ssl/certs/ 
# Mon, 21 Oct 2019 20:27:55 GMT
COPY dir:e700a731062c6a1130194c74080171046494718874f8e586f78523a64d56715c in /usr/share/ 
# Tue, 10 Dec 2019 21:57:12 GMT
COPY file:ad6d99c4dea9edfff1bf18494e1c85b8a82b1a74f77a8bf3f437bd05222fbf79 in / 
# Tue, 10 Dec 2019 21:57:14 GMT
EXPOSE 80
# Tue, 10 Dec 2019 21:57:15 GMT
VOLUME [/tmp]
# Tue, 10 Dec 2019 21:57:16 GMT
ENTRYPOINT ["/traefik"]
# Tue, 10 Dec 2019 21:57:17 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.20 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:506698346e0f5f486b919abaa7bc72252b3dc553cb28e0d1a5e2b6f3708cf4c0`  
		Last Modified: Mon, 26 Aug 2019 23:55:08 GMT  
		Size: 132.0 KB (132026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46037320e6487ea40f4dfb2c29d120090739bc20051bca67eb5e64a072973136`  
		Last Modified: Mon, 21 Oct 2019 20:28:50 GMT  
		Size: 327.4 KB (327388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d0d7ab9d9ce392bdaa622a30db2df3963e7ac8b19c846fddc788b2f7fd3f890`  
		Last Modified: Tue, 10 Dec 2019 21:58:07 GMT  
		Size: 22.0 MB (22032125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:1.7` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:3a587a9647aca9d58c237389157512cf349f00e99afc0f33959501bc5366b489
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **22.2 MB (22219190 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:843151930dcd29bc722fa2e9949bcecfcb0020d961037b85983f47017aa38a58`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Tue, 27 Aug 2019 00:16:41 GMT
COPY file:091d2a65366d205fc0db557b2f495da40adb5a33c9d656d02c3ea08bb22f6c4d in /etc/ssl/certs/ 
# Mon, 21 Oct 2019 23:22:44 GMT
COPY dir:e700a731062c6a1130194c74080171046494718874f8e586f78523a64d56715c in /usr/share/ 
# Tue, 10 Dec 2019 22:39:48 GMT
COPY file:2548a09c5388b09356e8109d52a2261b02b840df1156718406457af4ef9eedcd in / 
# Tue, 10 Dec 2019 22:39:50 GMT
EXPOSE 80
# Tue, 10 Dec 2019 22:39:50 GMT
VOLUME [/tmp]
# Tue, 10 Dec 2019 22:39:51 GMT
ENTRYPOINT ["/traefik"]
# Tue, 10 Dec 2019 22:39:51 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.20 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:f07a1cd6fb05ab2fb5b66f5326144f82e52f5580df40a42e400637f8a8f9c6d8`  
		Last Modified: Tue, 27 Aug 2019 00:17:31 GMT  
		Size: 132.0 KB (132021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af2afd881e5b94f57a79b2f6bcd9d637c2f7a6aa910f4013045b8653ebe29fdb`  
		Last Modified: Mon, 21 Oct 2019 23:23:36 GMT  
		Size: 327.4 KB (327378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b05c8936168a3f333423ce8dca6ed7e5ad1890ce50b95da487f61aa83440e26`  
		Last Modified: Tue, 10 Dec 2019 22:40:39 GMT  
		Size: 21.8 MB (21759791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:1.7.20`

```console
$ docker pull traefik@sha256:5ec34caf19d114f8f0ed76f9bc3dad6ba8cf6d13a1575c4294b59b77709def39
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:1.7.20` - linux; amd64

```console
$ docker pull traefik@sha256:3b1c4d57c57d125a5d949d463d41882fefc957ce117db226aace4e7314e82d5c
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **24.0 MB (24005352 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:96c63a7d3e502fcbbd8937a2523368c22d0edd1788b8389af095f64038318834`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Tue, 27 Aug 2019 01:00:22 GMT
COPY file:091d2a65366d205fc0db557b2f495da40adb5a33c9d656d02c3ea08bb22f6c4d in /etc/ssl/certs/ 
# Mon, 21 Oct 2019 22:26:52 GMT
COPY dir:e700a731062c6a1130194c74080171046494718874f8e586f78523a64d56715c in /usr/share/ 
# Tue, 10 Dec 2019 22:31:38 GMT
COPY file:be1ea92a6d3f63051c9ae787ca41c986b81a56ce7f8b8347b97c3ddc3b4471f5 in / 
# Tue, 10 Dec 2019 22:31:38 GMT
EXPOSE 80
# Tue, 10 Dec 2019 22:31:38 GMT
VOLUME [/tmp]
# Tue, 10 Dec 2019 22:31:38 GMT
ENTRYPOINT ["/traefik"]
# Tue, 10 Dec 2019 22:31:39 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.20 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:42e7d26ec3785f8ce0f20e327cf72404ee054ba022ce9068ad2d28c52e82db2a`  
		Last Modified: Tue, 27 Aug 2019 01:00:52 GMT  
		Size: 132.0 KB (132022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a753f02eeffef33e5e071a6feac9e12fffb36330fc7ef5441f378d0ce67c528`  
		Last Modified: Mon, 21 Oct 2019 22:27:25 GMT  
		Size: 327.3 KB (327346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab927d94d255c72862c3e7ada3f6cdb36f90926b7a8913a080062b17d73f186b`  
		Last Modified: Tue, 10 Dec 2019 22:32:27 GMT  
		Size: 23.5 MB (23545984 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:1.7.20` - linux; arm variant v6

```console
$ docker pull traefik@sha256:3a32e589b7d538f688f0a4d5777ab21dc2e946e22a1b08872aaad72b4192976e
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **22.5 MB (22491539 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:099411d81ac7bf28b232625f19ecc6590f39c3920418958b3056caa4f85815c4`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Mon, 26 Aug 2019 23:54:26 GMT
COPY file:091d2a65366d205fc0db557b2f495da40adb5a33c9d656d02c3ea08bb22f6c4d in /etc/ssl/certs/ 
# Mon, 21 Oct 2019 20:27:55 GMT
COPY dir:e700a731062c6a1130194c74080171046494718874f8e586f78523a64d56715c in /usr/share/ 
# Tue, 10 Dec 2019 21:57:12 GMT
COPY file:ad6d99c4dea9edfff1bf18494e1c85b8a82b1a74f77a8bf3f437bd05222fbf79 in / 
# Tue, 10 Dec 2019 21:57:14 GMT
EXPOSE 80
# Tue, 10 Dec 2019 21:57:15 GMT
VOLUME [/tmp]
# Tue, 10 Dec 2019 21:57:16 GMT
ENTRYPOINT ["/traefik"]
# Tue, 10 Dec 2019 21:57:17 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.20 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:506698346e0f5f486b919abaa7bc72252b3dc553cb28e0d1a5e2b6f3708cf4c0`  
		Last Modified: Mon, 26 Aug 2019 23:55:08 GMT  
		Size: 132.0 KB (132026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46037320e6487ea40f4dfb2c29d120090739bc20051bca67eb5e64a072973136`  
		Last Modified: Mon, 21 Oct 2019 20:28:50 GMT  
		Size: 327.4 KB (327388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d0d7ab9d9ce392bdaa622a30db2df3963e7ac8b19c846fddc788b2f7fd3f890`  
		Last Modified: Tue, 10 Dec 2019 21:58:07 GMT  
		Size: 22.0 MB (22032125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:1.7.20` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:3a587a9647aca9d58c237389157512cf349f00e99afc0f33959501bc5366b489
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **22.2 MB (22219190 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:843151930dcd29bc722fa2e9949bcecfcb0020d961037b85983f47017aa38a58`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Tue, 27 Aug 2019 00:16:41 GMT
COPY file:091d2a65366d205fc0db557b2f495da40adb5a33c9d656d02c3ea08bb22f6c4d in /etc/ssl/certs/ 
# Mon, 21 Oct 2019 23:22:44 GMT
COPY dir:e700a731062c6a1130194c74080171046494718874f8e586f78523a64d56715c in /usr/share/ 
# Tue, 10 Dec 2019 22:39:48 GMT
COPY file:2548a09c5388b09356e8109d52a2261b02b840df1156718406457af4ef9eedcd in / 
# Tue, 10 Dec 2019 22:39:50 GMT
EXPOSE 80
# Tue, 10 Dec 2019 22:39:50 GMT
VOLUME [/tmp]
# Tue, 10 Dec 2019 22:39:51 GMT
ENTRYPOINT ["/traefik"]
# Tue, 10 Dec 2019 22:39:51 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.20 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:f07a1cd6fb05ab2fb5b66f5326144f82e52f5580df40a42e400637f8a8f9c6d8`  
		Last Modified: Tue, 27 Aug 2019 00:17:31 GMT  
		Size: 132.0 KB (132021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af2afd881e5b94f57a79b2f6bcd9d637c2f7a6aa910f4013045b8653ebe29fdb`  
		Last Modified: Mon, 21 Oct 2019 23:23:36 GMT  
		Size: 327.4 KB (327378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b05c8936168a3f333423ce8dca6ed7e5ad1890ce50b95da487f61aa83440e26`  
		Last Modified: Tue, 10 Dec 2019 22:40:39 GMT  
		Size: 21.8 MB (21759791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:1.7.20-alpine`

```console
$ docker pull traefik@sha256:ce4f1f9ec3de9c802a1d6020928358d7301452fc5c009ea314fbaa728e69aa3d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:1.7.20-alpine` - linux; amd64

```console
$ docker pull traefik@sha256:f9f7bc3071415790c015ad52995e2997d9d1cfd5cffdde58cb403e15d71fbe4e
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.0 MB (27028274 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:439e73a064c8f244ce1fe21cb3abcc9b314309275e3b26fd6ac0276946f669c8`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Mon, 21 Oct 2019 17:21:42 GMT
ADD file:fe1f09249227e2da2089afb4d07e16cbf832eeb804120074acd2b8192876cd28 in / 
# Mon, 21 Oct 2019 17:21:42 GMT
CMD ["/bin/sh"]
# Mon, 21 Oct 2019 22:26:21 GMT
RUN apk --no-cache add ca-certificates tzdata
# Tue, 10 Dec 2019 22:31:01 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/containous/traefik/releases/download/v1.7.20/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Tue, 10 Dec 2019 22:31:02 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Tue, 10 Dec 2019 22:31:02 GMT
EXPOSE 80
# Tue, 10 Dec 2019 22:31:02 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 10 Dec 2019 22:31:02 GMT
CMD ["traefik"]
# Tue, 10 Dec 2019 22:31:03 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.20 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:89d9c30c1d48bac627e5c6cb0d1ed1eec28e7dbdfbcc04712e4c79c0f83faf17`  
		Last Modified: Mon, 21 Oct 2019 17:22:48 GMT  
		Size: 2.8 MB (2787134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:275722d2e7f6dc3397547bc96af555d5905a44fc2f88a1adb39ddfc6aa2a98b9`  
		Last Modified: Mon, 21 Oct 2019 22:27:05 GMT  
		Size: 694.5 KB (694493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:198d6da64444dd0f60f3c566038d6c9157c290fb6152ec296204e862073f365f`  
		Last Modified: Tue, 10 Dec 2019 22:32:13 GMT  
		Size: 23.5 MB (23546279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fd7a10facf04db24667668cb9792494b0e49f33e439cccf618f435ef237bfa3`  
		Last Modified: Tue, 10 Dec 2019 22:32:07 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:1.7.20-alpine` - linux; arm variant v6

```console
$ docker pull traefik@sha256:91c059509f0cd0fbf794e278e25674fe57f5d3f4185f7ed23c6915852d437f05
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.3 MB (25301854 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e0fb17b7213044c3a520701dcb0f1b21f9fa79d3f0ed57cebfef9dc91a064913`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Mon, 21 Oct 2019 16:56:02 GMT
ADD file:d3c7d938a78143f106a6a467ce23b599198e041220e661e5326ba91054c353ef in / 
# Mon, 21 Oct 2019 16:56:04 GMT
CMD ["/bin/sh"]
# Mon, 21 Oct 2019 20:27:15 GMT
RUN apk --no-cache add ca-certificates tzdata
# Tue, 10 Dec 2019 21:49:54 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/containous/traefik/releases/download/v1.7.20/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Tue, 10 Dec 2019 21:49:55 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Tue, 10 Dec 2019 21:49:56 GMT
EXPOSE 80
# Tue, 10 Dec 2019 21:49:56 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 10 Dec 2019 21:49:57 GMT
CMD ["traefik"]
# Tue, 10 Dec 2019 21:49:57 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.20 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:ecf664be551d26dcd221b7387283cdcc54f46c6789700d037fa3cd0c297f8645`  
		Last Modified: Mon, 21 Oct 2019 16:56:34 GMT  
		Size: 2.6 MB (2571309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e75226f24cf5fc4e2d56fbb31d8daf122273d120792aff22dee3a970a5419ee9`  
		Last Modified: Mon, 21 Oct 2019 20:28:17 GMT  
		Size: 697.8 KB (697821 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdd02ec506a5475103a69714675382b27257bcb6710941053abde15b07f1f473`  
		Last Modified: Tue, 10 Dec 2019 21:57:48 GMT  
		Size: 22.0 MB (22032356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27ff5f776c2bcd52a563737242a856d37745bdd6947d9989ee6aec3157f6db81`  
		Last Modified: Tue, 10 Dec 2019 21:57:39 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:1.7.20-alpine` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:69880c97f253a7dab9e3fb1e477bc209a297ceb369f259841a14ec194ac5fbe3
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.2 MB (25175702 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:630da378646ff9d16799a8f19fc83d02d28fe478003b44b8f37a8b0a4b715079`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Mon, 21 Oct 2019 18:07:03 GMT
ADD file:02f4d68afd9e9e303ff893f198d535d0d78c4b2554f299ab2d0955b2bef0e06a in / 
# Mon, 21 Oct 2019 18:07:09 GMT
CMD ["/bin/sh"]
# Mon, 21 Oct 2019 23:22:16 GMT
RUN apk --no-cache add ca-certificates tzdata
# Tue, 10 Dec 2019 22:39:26 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/containous/traefik/releases/download/v1.7.20/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Tue, 10 Dec 2019 22:39:27 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Tue, 10 Dec 2019 22:39:27 GMT
EXPOSE 80
# Tue, 10 Dec 2019 22:39:28 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 10 Dec 2019 22:39:28 GMT
CMD ["traefik"]
# Tue, 10 Dec 2019 22:39:29 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.20 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:8bfa913040406727f36faa9b69d0b96e071b13792a83ad69c19389031a9f3797`  
		Last Modified: Mon, 21 Oct 2019 18:08:36 GMT  
		Size: 2.7 MB (2717778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a21b1a0e782f54ba929f36f1f589cbf9cacb6e15d6644d901741533bec314cec`  
		Last Modified: Mon, 21 Oct 2019 23:23:04 GMT  
		Size: 697.9 KB (697888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a1ad2d17ee7cb6da8499ef5415cad503d05873da472bcfc6d2ac07e9bdbad2c`  
		Last Modified: Tue, 10 Dec 2019 22:40:19 GMT  
		Size: 21.8 MB (21759668 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9525ac7ce9940a937d298cf00954af64fd399df1a840cad75914caeb0b5cf224`  
		Last Modified: Tue, 10 Dec 2019 22:40:11 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:1.7.20-windowsservercore-1809`

```console
$ docker pull traefik@sha256:122b54d5a8a5cccc8839e7a3ce5c385c0b04a9c02ba4c741ea8a82f4a58ff6c8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.914; amd64

### `traefik:1.7.20-windowsservercore-1809` - windows version 10.0.17763.914; amd64

```console
$ docker pull traefik@sha256:0092b009fa818e0152462c069457055244a329e613e4f4e86801363bcbabfdd2
```

-	Docker Version: 18.03.1-ee-4
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.2 GB (2244435166 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:49463175a868dfe3c0a39b4693212b98b6d9da1043bf4b1b18570bef3a010859`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 15 Sep 2018 09:10:26 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 29 Nov 2019 04:34:15 GMT
RUN Install update 1809-amd64
# Tue, 10 Dec 2019 21:34:07 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 10 Dec 2019 22:06:49 GMT
RUN Invoke-WebRequest     -Uri "https://github.com/containous/traefik/releases/download/v1.7.20/traefik_windows-amd64.exe"     -OutFile "/traefik.exe"
# Tue, 10 Dec 2019 22:06:55 GMT
EXPOSE 80
# Tue, 10 Dec 2019 22:06:56 GMT
ENTRYPOINT ["/traefik"]
# Tue, 10 Dec 2019 22:06:58 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.20 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:65014b3c312172f10bd6701a063f9b5aaf9a916c2d2cb843d406a6f77ded3f8d`  
		Last Modified: Tue, 13 Nov 2018 18:50:17 GMT  
		Size: 1.5 GB (1534685324 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:faf31ee0aa3d3c60a38dd03c7554d632065cef50eab052ef1444590786249d07`  
		Size: 681.6 MB (681618026 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e147f14e0d6a9cbd5261162dea8f3aac7a34db5d9f6a587a9aac6b88722a2da4`  
		Last Modified: Tue, 10 Dec 2019 22:07:34 GMT  
		Size: 1.2 KB (1211 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59c8ec155d3968143fbceaac2d3d287e2a97d836b6dcf3ca1418e8bea4cd0062`  
		Last Modified: Tue, 10 Dec 2019 22:08:38 GMT  
		Size: 28.1 MB (28127080 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7f47f2cf9e401dfd15ca112b20632f36aa0a56f5f404643720a8a11aad1bb28`  
		Last Modified: Tue, 10 Dec 2019 22:08:32 GMT  
		Size: 1.2 KB (1180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e11ec09770c3643d749d678f579e251ceeaabb28536596e148ee6b71b93981cb`  
		Last Modified: Tue, 10 Dec 2019 22:08:30 GMT  
		Size: 1.2 KB (1183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2df6a0c73ef71f2868be658441f5856463b1de3edc2e49e66f13c86551981a3`  
		Last Modified: Tue, 10 Dec 2019 22:08:31 GMT  
		Size: 1.2 KB (1162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:1.7-alpine`

```console
$ docker pull traefik@sha256:ce4f1f9ec3de9c802a1d6020928358d7301452fc5c009ea314fbaa728e69aa3d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:1.7-alpine` - linux; amd64

```console
$ docker pull traefik@sha256:f9f7bc3071415790c015ad52995e2997d9d1cfd5cffdde58cb403e15d71fbe4e
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.0 MB (27028274 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:439e73a064c8f244ce1fe21cb3abcc9b314309275e3b26fd6ac0276946f669c8`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Mon, 21 Oct 2019 17:21:42 GMT
ADD file:fe1f09249227e2da2089afb4d07e16cbf832eeb804120074acd2b8192876cd28 in / 
# Mon, 21 Oct 2019 17:21:42 GMT
CMD ["/bin/sh"]
# Mon, 21 Oct 2019 22:26:21 GMT
RUN apk --no-cache add ca-certificates tzdata
# Tue, 10 Dec 2019 22:31:01 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/containous/traefik/releases/download/v1.7.20/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Tue, 10 Dec 2019 22:31:02 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Tue, 10 Dec 2019 22:31:02 GMT
EXPOSE 80
# Tue, 10 Dec 2019 22:31:02 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 10 Dec 2019 22:31:02 GMT
CMD ["traefik"]
# Tue, 10 Dec 2019 22:31:03 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.20 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:89d9c30c1d48bac627e5c6cb0d1ed1eec28e7dbdfbcc04712e4c79c0f83faf17`  
		Last Modified: Mon, 21 Oct 2019 17:22:48 GMT  
		Size: 2.8 MB (2787134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:275722d2e7f6dc3397547bc96af555d5905a44fc2f88a1adb39ddfc6aa2a98b9`  
		Last Modified: Mon, 21 Oct 2019 22:27:05 GMT  
		Size: 694.5 KB (694493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:198d6da64444dd0f60f3c566038d6c9157c290fb6152ec296204e862073f365f`  
		Last Modified: Tue, 10 Dec 2019 22:32:13 GMT  
		Size: 23.5 MB (23546279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fd7a10facf04db24667668cb9792494b0e49f33e439cccf618f435ef237bfa3`  
		Last Modified: Tue, 10 Dec 2019 22:32:07 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:1.7-alpine` - linux; arm variant v6

```console
$ docker pull traefik@sha256:91c059509f0cd0fbf794e278e25674fe57f5d3f4185f7ed23c6915852d437f05
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.3 MB (25301854 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e0fb17b7213044c3a520701dcb0f1b21f9fa79d3f0ed57cebfef9dc91a064913`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Mon, 21 Oct 2019 16:56:02 GMT
ADD file:d3c7d938a78143f106a6a467ce23b599198e041220e661e5326ba91054c353ef in / 
# Mon, 21 Oct 2019 16:56:04 GMT
CMD ["/bin/sh"]
# Mon, 21 Oct 2019 20:27:15 GMT
RUN apk --no-cache add ca-certificates tzdata
# Tue, 10 Dec 2019 21:49:54 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/containous/traefik/releases/download/v1.7.20/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Tue, 10 Dec 2019 21:49:55 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Tue, 10 Dec 2019 21:49:56 GMT
EXPOSE 80
# Tue, 10 Dec 2019 21:49:56 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 10 Dec 2019 21:49:57 GMT
CMD ["traefik"]
# Tue, 10 Dec 2019 21:49:57 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.20 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:ecf664be551d26dcd221b7387283cdcc54f46c6789700d037fa3cd0c297f8645`  
		Last Modified: Mon, 21 Oct 2019 16:56:34 GMT  
		Size: 2.6 MB (2571309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e75226f24cf5fc4e2d56fbb31d8daf122273d120792aff22dee3a970a5419ee9`  
		Last Modified: Mon, 21 Oct 2019 20:28:17 GMT  
		Size: 697.8 KB (697821 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdd02ec506a5475103a69714675382b27257bcb6710941053abde15b07f1f473`  
		Last Modified: Tue, 10 Dec 2019 21:57:48 GMT  
		Size: 22.0 MB (22032356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27ff5f776c2bcd52a563737242a856d37745bdd6947d9989ee6aec3157f6db81`  
		Last Modified: Tue, 10 Dec 2019 21:57:39 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:1.7-alpine` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:69880c97f253a7dab9e3fb1e477bc209a297ceb369f259841a14ec194ac5fbe3
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.2 MB (25175702 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:630da378646ff9d16799a8f19fc83d02d28fe478003b44b8f37a8b0a4b715079`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Mon, 21 Oct 2019 18:07:03 GMT
ADD file:02f4d68afd9e9e303ff893f198d535d0d78c4b2554f299ab2d0955b2bef0e06a in / 
# Mon, 21 Oct 2019 18:07:09 GMT
CMD ["/bin/sh"]
# Mon, 21 Oct 2019 23:22:16 GMT
RUN apk --no-cache add ca-certificates tzdata
# Tue, 10 Dec 2019 22:39:26 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/containous/traefik/releases/download/v1.7.20/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Tue, 10 Dec 2019 22:39:27 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Tue, 10 Dec 2019 22:39:27 GMT
EXPOSE 80
# Tue, 10 Dec 2019 22:39:28 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 10 Dec 2019 22:39:28 GMT
CMD ["traefik"]
# Tue, 10 Dec 2019 22:39:29 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.20 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:8bfa913040406727f36faa9b69d0b96e071b13792a83ad69c19389031a9f3797`  
		Last Modified: Mon, 21 Oct 2019 18:08:36 GMT  
		Size: 2.7 MB (2717778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a21b1a0e782f54ba929f36f1f589cbf9cacb6e15d6644d901741533bec314cec`  
		Last Modified: Mon, 21 Oct 2019 23:23:04 GMT  
		Size: 697.9 KB (697888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a1ad2d17ee7cb6da8499ef5415cad503d05873da472bcfc6d2ac07e9bdbad2c`  
		Last Modified: Tue, 10 Dec 2019 22:40:19 GMT  
		Size: 21.8 MB (21759668 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9525ac7ce9940a937d298cf00954af64fd399df1a840cad75914caeb0b5cf224`  
		Last Modified: Tue, 10 Dec 2019 22:40:11 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:1.7-windowsservercore-1809`

```console
$ docker pull traefik@sha256:122b54d5a8a5cccc8839e7a3ce5c385c0b04a9c02ba4c741ea8a82f4a58ff6c8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.914; amd64

### `traefik:1.7-windowsservercore-1809` - windows version 10.0.17763.914; amd64

```console
$ docker pull traefik@sha256:0092b009fa818e0152462c069457055244a329e613e4f4e86801363bcbabfdd2
```

-	Docker Version: 18.03.1-ee-4
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.2 GB (2244435166 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:49463175a868dfe3c0a39b4693212b98b6d9da1043bf4b1b18570bef3a010859`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 15 Sep 2018 09:10:26 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 29 Nov 2019 04:34:15 GMT
RUN Install update 1809-amd64
# Tue, 10 Dec 2019 21:34:07 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 10 Dec 2019 22:06:49 GMT
RUN Invoke-WebRequest     -Uri "https://github.com/containous/traefik/releases/download/v1.7.20/traefik_windows-amd64.exe"     -OutFile "/traefik.exe"
# Tue, 10 Dec 2019 22:06:55 GMT
EXPOSE 80
# Tue, 10 Dec 2019 22:06:56 GMT
ENTRYPOINT ["/traefik"]
# Tue, 10 Dec 2019 22:06:58 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.20 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:65014b3c312172f10bd6701a063f9b5aaf9a916c2d2cb843d406a6f77ded3f8d`  
		Last Modified: Tue, 13 Nov 2018 18:50:17 GMT  
		Size: 1.5 GB (1534685324 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:faf31ee0aa3d3c60a38dd03c7554d632065cef50eab052ef1444590786249d07`  
		Size: 681.6 MB (681618026 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e147f14e0d6a9cbd5261162dea8f3aac7a34db5d9f6a587a9aac6b88722a2da4`  
		Last Modified: Tue, 10 Dec 2019 22:07:34 GMT  
		Size: 1.2 KB (1211 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59c8ec155d3968143fbceaac2d3d287e2a97d836b6dcf3ca1418e8bea4cd0062`  
		Last Modified: Tue, 10 Dec 2019 22:08:38 GMT  
		Size: 28.1 MB (28127080 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7f47f2cf9e401dfd15ca112b20632f36aa0a56f5f404643720a8a11aad1bb28`  
		Last Modified: Tue, 10 Dec 2019 22:08:32 GMT  
		Size: 1.2 KB (1180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e11ec09770c3643d749d678f579e251ceeaabb28536596e148ee6b71b93981cb`  
		Last Modified: Tue, 10 Dec 2019 22:08:30 GMT  
		Size: 1.2 KB (1183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2df6a0c73ef71f2868be658441f5856463b1de3edc2e49e66f13c86551981a3`  
		Last Modified: Tue, 10 Dec 2019 22:08:31 GMT  
		Size: 1.2 KB (1162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:2.1`

```console
$ docker pull traefik@sha256:a87b61f3254d03c4fcc0b994e2cb7af89abba8178f1fbec3bce3f4bdc080f8a6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:2.1` - linux; amd64

```console
$ docker pull traefik@sha256:b1fe8eec6330ffe542f313a21860361f266375f854804ed19893933f65a62e67
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.0 MB (22972242 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7f7affdc32376c94f75ff0112832475d1c7b5c42ae438b3208039d29451972ac`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Mon, 21 Oct 2019 17:21:42 GMT
ADD file:fe1f09249227e2da2089afb4d07e16cbf832eeb804120074acd2b8192876cd28 in / 
# Mon, 21 Oct 2019 17:21:42 GMT
CMD ["/bin/sh"]
# Mon, 21 Oct 2019 22:26:21 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 12 Dec 2019 23:39:42 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/containous/traefik/releases/download/v2.1.1/traefik_v2.1.1_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 12 Dec 2019 23:39:43 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 12 Dec 2019 23:39:43 GMT
EXPOSE 80
# Thu, 12 Dec 2019 23:39:43 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 12 Dec 2019 23:39:43 GMT
CMD ["traefik"]
# Thu, 12 Dec 2019 23:39:43 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.1.1 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:89d9c30c1d48bac627e5c6cb0d1ed1eec28e7dbdfbcc04712e4c79c0f83faf17`  
		Last Modified: Mon, 21 Oct 2019 17:22:48 GMT  
		Size: 2.8 MB (2787134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:275722d2e7f6dc3397547bc96af555d5905a44fc2f88a1adb39ddfc6aa2a98b9`  
		Last Modified: Mon, 21 Oct 2019 22:27:05 GMT  
		Size: 694.5 KB (694493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88ca2a78572e6379d1dc1b5ddfa2302e84a42a0305c9d26259ff61b40abecc6b`  
		Last Modified: Thu, 12 Dec 2019 23:40:09 GMT  
		Size: 19.5 MB (19490246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bf623a84bbbfb8681af59457bfae6ae09537f9e29ceea00d7a872b49eacc48a`  
		Last Modified: Thu, 12 Dec 2019 23:40:04 GMT  
		Size: 369.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:2.1` - linux; arm variant v6

```console
$ docker pull traefik@sha256:8893289f168246069496fb44fe86cdd862b7497d58ea0b8d3d28509655ae772a
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **21.5 MB (21530113 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ce54f5d1d0d33e5388f78cd582d4a7d81c4b3f14a68d0468d4dc5d623d12ebb6`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Mon, 21 Oct 2019 16:56:02 GMT
ADD file:d3c7d938a78143f106a6a467ce23b599198e041220e661e5326ba91054c353ef in / 
# Mon, 21 Oct 2019 16:56:04 GMT
CMD ["/bin/sh"]
# Mon, 21 Oct 2019 20:27:15 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 12 Dec 2019 23:51:04 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/containous/traefik/releases/download/v2.1.1/traefik_v2.1.1_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 12 Dec 2019 23:51:05 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 12 Dec 2019 23:51:08 GMT
EXPOSE 80
# Thu, 12 Dec 2019 23:51:10 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 12 Dec 2019 23:51:13 GMT
CMD ["traefik"]
# Thu, 12 Dec 2019 23:51:18 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.1.1 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:ecf664be551d26dcd221b7387283cdcc54f46c6789700d037fa3cd0c297f8645`  
		Last Modified: Mon, 21 Oct 2019 16:56:34 GMT  
		Size: 2.6 MB (2571309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e75226f24cf5fc4e2d56fbb31d8daf122273d120792aff22dee3a970a5419ee9`  
		Last Modified: Mon, 21 Oct 2019 20:28:17 GMT  
		Size: 697.8 KB (697821 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:226040d9e7a47f0acbdced5e006aa1261f64cacbc04f3a09f837c362a5370b13`  
		Last Modified: Thu, 12 Dec 2019 23:52:09 GMT  
		Size: 18.3 MB (18260615 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb2a0bf2df3a2bb46100add59ef6b2bbaf57b5b496a159c6a1ebc5414125d152`  
		Last Modified: Thu, 12 Dec 2019 23:52:03 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:2.1` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:d95d874b2e045fb3a8a7360180d74b2ab7414105160a5607a3b97db891517763
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **21.4 MB (21364609 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:87e3030ddfe47d09d8a165d84f5f88527465dcd247906deb639563961b0e6c40`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Mon, 21 Oct 2019 18:07:03 GMT
ADD file:02f4d68afd9e9e303ff893f198d535d0d78c4b2554f299ab2d0955b2bef0e06a in / 
# Mon, 21 Oct 2019 18:07:09 GMT
CMD ["/bin/sh"]
# Mon, 21 Oct 2019 23:22:16 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 12 Dec 2019 23:51:27 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/containous/traefik/releases/download/v2.1.1/traefik_v2.1.1_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 12 Dec 2019 23:51:29 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 12 Dec 2019 23:51:33 GMT
EXPOSE 80
# Thu, 12 Dec 2019 23:51:38 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 12 Dec 2019 23:51:42 GMT
CMD ["traefik"]
# Thu, 12 Dec 2019 23:51:46 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.1.1 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:8bfa913040406727f36faa9b69d0b96e071b13792a83ad69c19389031a9f3797`  
		Last Modified: Mon, 21 Oct 2019 18:08:36 GMT  
		Size: 2.7 MB (2717778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a21b1a0e782f54ba929f36f1f589cbf9cacb6e15d6644d901741533bec314cec`  
		Last Modified: Mon, 21 Oct 2019 23:23:04 GMT  
		Size: 697.9 KB (697888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a5093f9995081d7b5b63babf2940a3ec750e2ed80b92e822266e16e25ff41e3`  
		Last Modified: Thu, 12 Dec 2019 23:52:23 GMT  
		Size: 17.9 MB (17948574 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7095cdc86392137d36c03c39e37c62da37671933425b16232d4c528cfee11581`  
		Last Modified: Thu, 12 Dec 2019 23:52:17 GMT  
		Size: 369.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:2.1.2`

**does not exist** (yet?)

## `traefik:2.1.2-windowsservercore-1809`

**does not exist** (yet?)

## `traefik:2.1-windowsservercore-1809`

```console
$ docker pull traefik@sha256:72f61926c08b2013cccbe1a249a6631946ef920eca7995fa52c693c53338aa72
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.914; amd64

### `traefik:2.1-windowsservercore-1809` - windows version 10.0.17763.914; amd64

```console
$ docker pull traefik@sha256:585f0b403374f6611b3e8d5f41460c97228dc284cbc9ce96d179a1118cdb58ab
```

-	Docker Version: 18.03.1-ee-4
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.2 GB (2240370088 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:84d0f8a51ec5aca3f2383905bb2c439c567e89ff67cd0821bd9fd4b6d38247df`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 15 Sep 2018 09:10:26 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 29 Nov 2019 04:34:15 GMT
RUN Install update 1809-amd64
# Tue, 10 Dec 2019 21:34:07 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 12 Dec 2019 23:23:21 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/containous/traefik/releases/download/v2.1.1/traefik_v2.1.1_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Thu, 12 Dec 2019 23:23:22 GMT
EXPOSE 80
# Thu, 12 Dec 2019 23:23:24 GMT
ENTRYPOINT ["/traefik"]
# Thu, 12 Dec 2019 23:23:26 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.1.1 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:65014b3c312172f10bd6701a063f9b5aaf9a916c2d2cb843d406a6f77ded3f8d`  
		Last Modified: Tue, 13 Nov 2018 18:50:17 GMT  
		Size: 1.5 GB (1534685324 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:faf31ee0aa3d3c60a38dd03c7554d632065cef50eab052ef1444590786249d07`  
		Size: 681.6 MB (681618026 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e147f14e0d6a9cbd5261162dea8f3aac7a34db5d9f6a587a9aac6b88722a2da4`  
		Last Modified: Tue, 10 Dec 2019 22:07:34 GMT  
		Size: 1.2 KB (1211 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08283c3529083d82a99e4e993d5f3b36a624cba1c0c29337b3c557881afeae2f`  
		Last Modified: Thu, 12 Dec 2019 23:24:05 GMT  
		Size: 24.1 MB (24061960 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d01b24dc42771e2aebc1ea9d6c3d1e7052eb5b5bf266ba4123a75e40c62ab076`  
		Last Modified: Thu, 12 Dec 2019 23:23:59 GMT  
		Size: 1.2 KB (1180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4bb434cba60f7b0cce45a2f1c6c00ef0e6b0bfb00a4ef097fa7797c5e074c12`  
		Last Modified: Thu, 12 Dec 2019 23:24:00 GMT  
		Size: 1.2 KB (1208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a20bcbc7f4aee693390e71290e8b6b4efb693ad5f2b2da57d1eb9add9d0bbba`  
		Last Modified: Thu, 12 Dec 2019 23:23:59 GMT  
		Size: 1.2 KB (1179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:cantal`

```console
$ docker pull traefik@sha256:a87b61f3254d03c4fcc0b994e2cb7af89abba8178f1fbec3bce3f4bdc080f8a6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:cantal` - linux; amd64

```console
$ docker pull traefik@sha256:b1fe8eec6330ffe542f313a21860361f266375f854804ed19893933f65a62e67
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.0 MB (22972242 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7f7affdc32376c94f75ff0112832475d1c7b5c42ae438b3208039d29451972ac`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Mon, 21 Oct 2019 17:21:42 GMT
ADD file:fe1f09249227e2da2089afb4d07e16cbf832eeb804120074acd2b8192876cd28 in / 
# Mon, 21 Oct 2019 17:21:42 GMT
CMD ["/bin/sh"]
# Mon, 21 Oct 2019 22:26:21 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 12 Dec 2019 23:39:42 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/containous/traefik/releases/download/v2.1.1/traefik_v2.1.1_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 12 Dec 2019 23:39:43 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 12 Dec 2019 23:39:43 GMT
EXPOSE 80
# Thu, 12 Dec 2019 23:39:43 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 12 Dec 2019 23:39:43 GMT
CMD ["traefik"]
# Thu, 12 Dec 2019 23:39:43 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.1.1 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:89d9c30c1d48bac627e5c6cb0d1ed1eec28e7dbdfbcc04712e4c79c0f83faf17`  
		Last Modified: Mon, 21 Oct 2019 17:22:48 GMT  
		Size: 2.8 MB (2787134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:275722d2e7f6dc3397547bc96af555d5905a44fc2f88a1adb39ddfc6aa2a98b9`  
		Last Modified: Mon, 21 Oct 2019 22:27:05 GMT  
		Size: 694.5 KB (694493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88ca2a78572e6379d1dc1b5ddfa2302e84a42a0305c9d26259ff61b40abecc6b`  
		Last Modified: Thu, 12 Dec 2019 23:40:09 GMT  
		Size: 19.5 MB (19490246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bf623a84bbbfb8681af59457bfae6ae09537f9e29ceea00d7a872b49eacc48a`  
		Last Modified: Thu, 12 Dec 2019 23:40:04 GMT  
		Size: 369.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:cantal` - linux; arm variant v6

```console
$ docker pull traefik@sha256:8893289f168246069496fb44fe86cdd862b7497d58ea0b8d3d28509655ae772a
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **21.5 MB (21530113 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ce54f5d1d0d33e5388f78cd582d4a7d81c4b3f14a68d0468d4dc5d623d12ebb6`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Mon, 21 Oct 2019 16:56:02 GMT
ADD file:d3c7d938a78143f106a6a467ce23b599198e041220e661e5326ba91054c353ef in / 
# Mon, 21 Oct 2019 16:56:04 GMT
CMD ["/bin/sh"]
# Mon, 21 Oct 2019 20:27:15 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 12 Dec 2019 23:51:04 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/containous/traefik/releases/download/v2.1.1/traefik_v2.1.1_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 12 Dec 2019 23:51:05 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 12 Dec 2019 23:51:08 GMT
EXPOSE 80
# Thu, 12 Dec 2019 23:51:10 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 12 Dec 2019 23:51:13 GMT
CMD ["traefik"]
# Thu, 12 Dec 2019 23:51:18 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.1.1 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:ecf664be551d26dcd221b7387283cdcc54f46c6789700d037fa3cd0c297f8645`  
		Last Modified: Mon, 21 Oct 2019 16:56:34 GMT  
		Size: 2.6 MB (2571309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e75226f24cf5fc4e2d56fbb31d8daf122273d120792aff22dee3a970a5419ee9`  
		Last Modified: Mon, 21 Oct 2019 20:28:17 GMT  
		Size: 697.8 KB (697821 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:226040d9e7a47f0acbdced5e006aa1261f64cacbc04f3a09f837c362a5370b13`  
		Last Modified: Thu, 12 Dec 2019 23:52:09 GMT  
		Size: 18.3 MB (18260615 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb2a0bf2df3a2bb46100add59ef6b2bbaf57b5b496a159c6a1ebc5414125d152`  
		Last Modified: Thu, 12 Dec 2019 23:52:03 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:cantal` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:d95d874b2e045fb3a8a7360180d74b2ab7414105160a5607a3b97db891517763
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **21.4 MB (21364609 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:87e3030ddfe47d09d8a165d84f5f88527465dcd247906deb639563961b0e6c40`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Mon, 21 Oct 2019 18:07:03 GMT
ADD file:02f4d68afd9e9e303ff893f198d535d0d78c4b2554f299ab2d0955b2bef0e06a in / 
# Mon, 21 Oct 2019 18:07:09 GMT
CMD ["/bin/sh"]
# Mon, 21 Oct 2019 23:22:16 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 12 Dec 2019 23:51:27 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/containous/traefik/releases/download/v2.1.1/traefik_v2.1.1_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 12 Dec 2019 23:51:29 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 12 Dec 2019 23:51:33 GMT
EXPOSE 80
# Thu, 12 Dec 2019 23:51:38 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 12 Dec 2019 23:51:42 GMT
CMD ["traefik"]
# Thu, 12 Dec 2019 23:51:46 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.1.1 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:8bfa913040406727f36faa9b69d0b96e071b13792a83ad69c19389031a9f3797`  
		Last Modified: Mon, 21 Oct 2019 18:08:36 GMT  
		Size: 2.7 MB (2717778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a21b1a0e782f54ba929f36f1f589cbf9cacb6e15d6644d901741533bec314cec`  
		Last Modified: Mon, 21 Oct 2019 23:23:04 GMT  
		Size: 697.9 KB (697888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a5093f9995081d7b5b63babf2940a3ec750e2ed80b92e822266e16e25ff41e3`  
		Last Modified: Thu, 12 Dec 2019 23:52:23 GMT  
		Size: 17.9 MB (17948574 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7095cdc86392137d36c03c39e37c62da37671933425b16232d4c528cfee11581`  
		Last Modified: Thu, 12 Dec 2019 23:52:17 GMT  
		Size: 369.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:cantal-windowsservercore-1809`

```console
$ docker pull traefik@sha256:72f61926c08b2013cccbe1a249a6631946ef920eca7995fa52c693c53338aa72
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.914; amd64

### `traefik:cantal-windowsservercore-1809` - windows version 10.0.17763.914; amd64

```console
$ docker pull traefik@sha256:585f0b403374f6611b3e8d5f41460c97228dc284cbc9ce96d179a1118cdb58ab
```

-	Docker Version: 18.03.1-ee-4
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.2 GB (2240370088 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:84d0f8a51ec5aca3f2383905bb2c439c567e89ff67cd0821bd9fd4b6d38247df`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 15 Sep 2018 09:10:26 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 29 Nov 2019 04:34:15 GMT
RUN Install update 1809-amd64
# Tue, 10 Dec 2019 21:34:07 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 12 Dec 2019 23:23:21 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/containous/traefik/releases/download/v2.1.1/traefik_v2.1.1_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Thu, 12 Dec 2019 23:23:22 GMT
EXPOSE 80
# Thu, 12 Dec 2019 23:23:24 GMT
ENTRYPOINT ["/traefik"]
# Thu, 12 Dec 2019 23:23:26 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.1.1 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:65014b3c312172f10bd6701a063f9b5aaf9a916c2d2cb843d406a6f77ded3f8d`  
		Last Modified: Tue, 13 Nov 2018 18:50:17 GMT  
		Size: 1.5 GB (1534685324 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:faf31ee0aa3d3c60a38dd03c7554d632065cef50eab052ef1444590786249d07`  
		Size: 681.6 MB (681618026 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e147f14e0d6a9cbd5261162dea8f3aac7a34db5d9f6a587a9aac6b88722a2da4`  
		Last Modified: Tue, 10 Dec 2019 22:07:34 GMT  
		Size: 1.2 KB (1211 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08283c3529083d82a99e4e993d5f3b36a624cba1c0c29337b3c557881afeae2f`  
		Last Modified: Thu, 12 Dec 2019 23:24:05 GMT  
		Size: 24.1 MB (24061960 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d01b24dc42771e2aebc1ea9d6c3d1e7052eb5b5bf266ba4123a75e40c62ab076`  
		Last Modified: Thu, 12 Dec 2019 23:23:59 GMT  
		Size: 1.2 KB (1180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4bb434cba60f7b0cce45a2f1c6c00ef0e6b0bfb00a4ef097fa7797c5e074c12`  
		Last Modified: Thu, 12 Dec 2019 23:24:00 GMT  
		Size: 1.2 KB (1208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a20bcbc7f4aee693390e71290e8b6b4efb693ad5f2b2da57d1eb9add9d0bbba`  
		Last Modified: Thu, 12 Dec 2019 23:23:59 GMT  
		Size: 1.2 KB (1179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:latest`

```console
$ docker pull traefik@sha256:a87b61f3254d03c4fcc0b994e2cb7af89abba8178f1fbec3bce3f4bdc080f8a6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:latest` - linux; amd64

```console
$ docker pull traefik@sha256:b1fe8eec6330ffe542f313a21860361f266375f854804ed19893933f65a62e67
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.0 MB (22972242 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7f7affdc32376c94f75ff0112832475d1c7b5c42ae438b3208039d29451972ac`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Mon, 21 Oct 2019 17:21:42 GMT
ADD file:fe1f09249227e2da2089afb4d07e16cbf832eeb804120074acd2b8192876cd28 in / 
# Mon, 21 Oct 2019 17:21:42 GMT
CMD ["/bin/sh"]
# Mon, 21 Oct 2019 22:26:21 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 12 Dec 2019 23:39:42 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/containous/traefik/releases/download/v2.1.1/traefik_v2.1.1_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 12 Dec 2019 23:39:43 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 12 Dec 2019 23:39:43 GMT
EXPOSE 80
# Thu, 12 Dec 2019 23:39:43 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 12 Dec 2019 23:39:43 GMT
CMD ["traefik"]
# Thu, 12 Dec 2019 23:39:43 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.1.1 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:89d9c30c1d48bac627e5c6cb0d1ed1eec28e7dbdfbcc04712e4c79c0f83faf17`  
		Last Modified: Mon, 21 Oct 2019 17:22:48 GMT  
		Size: 2.8 MB (2787134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:275722d2e7f6dc3397547bc96af555d5905a44fc2f88a1adb39ddfc6aa2a98b9`  
		Last Modified: Mon, 21 Oct 2019 22:27:05 GMT  
		Size: 694.5 KB (694493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88ca2a78572e6379d1dc1b5ddfa2302e84a42a0305c9d26259ff61b40abecc6b`  
		Last Modified: Thu, 12 Dec 2019 23:40:09 GMT  
		Size: 19.5 MB (19490246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bf623a84bbbfb8681af59457bfae6ae09537f9e29ceea00d7a872b49eacc48a`  
		Last Modified: Thu, 12 Dec 2019 23:40:04 GMT  
		Size: 369.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:latest` - linux; arm variant v6

```console
$ docker pull traefik@sha256:8893289f168246069496fb44fe86cdd862b7497d58ea0b8d3d28509655ae772a
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **21.5 MB (21530113 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ce54f5d1d0d33e5388f78cd582d4a7d81c4b3f14a68d0468d4dc5d623d12ebb6`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Mon, 21 Oct 2019 16:56:02 GMT
ADD file:d3c7d938a78143f106a6a467ce23b599198e041220e661e5326ba91054c353ef in / 
# Mon, 21 Oct 2019 16:56:04 GMT
CMD ["/bin/sh"]
# Mon, 21 Oct 2019 20:27:15 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 12 Dec 2019 23:51:04 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/containous/traefik/releases/download/v2.1.1/traefik_v2.1.1_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 12 Dec 2019 23:51:05 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 12 Dec 2019 23:51:08 GMT
EXPOSE 80
# Thu, 12 Dec 2019 23:51:10 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 12 Dec 2019 23:51:13 GMT
CMD ["traefik"]
# Thu, 12 Dec 2019 23:51:18 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.1.1 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:ecf664be551d26dcd221b7387283cdcc54f46c6789700d037fa3cd0c297f8645`  
		Last Modified: Mon, 21 Oct 2019 16:56:34 GMT  
		Size: 2.6 MB (2571309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e75226f24cf5fc4e2d56fbb31d8daf122273d120792aff22dee3a970a5419ee9`  
		Last Modified: Mon, 21 Oct 2019 20:28:17 GMT  
		Size: 697.8 KB (697821 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:226040d9e7a47f0acbdced5e006aa1261f64cacbc04f3a09f837c362a5370b13`  
		Last Modified: Thu, 12 Dec 2019 23:52:09 GMT  
		Size: 18.3 MB (18260615 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb2a0bf2df3a2bb46100add59ef6b2bbaf57b5b496a159c6a1ebc5414125d152`  
		Last Modified: Thu, 12 Dec 2019 23:52:03 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:latest` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:d95d874b2e045fb3a8a7360180d74b2ab7414105160a5607a3b97db891517763
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **21.4 MB (21364609 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:87e3030ddfe47d09d8a165d84f5f88527465dcd247906deb639563961b0e6c40`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Mon, 21 Oct 2019 18:07:03 GMT
ADD file:02f4d68afd9e9e303ff893f198d535d0d78c4b2554f299ab2d0955b2bef0e06a in / 
# Mon, 21 Oct 2019 18:07:09 GMT
CMD ["/bin/sh"]
# Mon, 21 Oct 2019 23:22:16 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 12 Dec 2019 23:51:27 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/containous/traefik/releases/download/v2.1.1/traefik_v2.1.1_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 12 Dec 2019 23:51:29 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 12 Dec 2019 23:51:33 GMT
EXPOSE 80
# Thu, 12 Dec 2019 23:51:38 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 12 Dec 2019 23:51:42 GMT
CMD ["traefik"]
# Thu, 12 Dec 2019 23:51:46 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.1.1 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:8bfa913040406727f36faa9b69d0b96e071b13792a83ad69c19389031a9f3797`  
		Last Modified: Mon, 21 Oct 2019 18:08:36 GMT  
		Size: 2.7 MB (2717778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a21b1a0e782f54ba929f36f1f589cbf9cacb6e15d6644d901741533bec314cec`  
		Last Modified: Mon, 21 Oct 2019 23:23:04 GMT  
		Size: 697.9 KB (697888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a5093f9995081d7b5b63babf2940a3ec750e2ed80b92e822266e16e25ff41e3`  
		Last Modified: Thu, 12 Dec 2019 23:52:23 GMT  
		Size: 17.9 MB (17948574 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7095cdc86392137d36c03c39e37c62da37671933425b16232d4c528cfee11581`  
		Last Modified: Thu, 12 Dec 2019 23:52:17 GMT  
		Size: 369.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:maroilles`

```console
$ docker pull traefik@sha256:5ec34caf19d114f8f0ed76f9bc3dad6ba8cf6d13a1575c4294b59b77709def39
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:maroilles` - linux; amd64

```console
$ docker pull traefik@sha256:3b1c4d57c57d125a5d949d463d41882fefc957ce117db226aace4e7314e82d5c
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **24.0 MB (24005352 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:96c63a7d3e502fcbbd8937a2523368c22d0edd1788b8389af095f64038318834`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Tue, 27 Aug 2019 01:00:22 GMT
COPY file:091d2a65366d205fc0db557b2f495da40adb5a33c9d656d02c3ea08bb22f6c4d in /etc/ssl/certs/ 
# Mon, 21 Oct 2019 22:26:52 GMT
COPY dir:e700a731062c6a1130194c74080171046494718874f8e586f78523a64d56715c in /usr/share/ 
# Tue, 10 Dec 2019 22:31:38 GMT
COPY file:be1ea92a6d3f63051c9ae787ca41c986b81a56ce7f8b8347b97c3ddc3b4471f5 in / 
# Tue, 10 Dec 2019 22:31:38 GMT
EXPOSE 80
# Tue, 10 Dec 2019 22:31:38 GMT
VOLUME [/tmp]
# Tue, 10 Dec 2019 22:31:38 GMT
ENTRYPOINT ["/traefik"]
# Tue, 10 Dec 2019 22:31:39 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.20 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:42e7d26ec3785f8ce0f20e327cf72404ee054ba022ce9068ad2d28c52e82db2a`  
		Last Modified: Tue, 27 Aug 2019 01:00:52 GMT  
		Size: 132.0 KB (132022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a753f02eeffef33e5e071a6feac9e12fffb36330fc7ef5441f378d0ce67c528`  
		Last Modified: Mon, 21 Oct 2019 22:27:25 GMT  
		Size: 327.3 KB (327346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab927d94d255c72862c3e7ada3f6cdb36f90926b7a8913a080062b17d73f186b`  
		Last Modified: Tue, 10 Dec 2019 22:32:27 GMT  
		Size: 23.5 MB (23545984 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:maroilles` - linux; arm variant v6

```console
$ docker pull traefik@sha256:3a32e589b7d538f688f0a4d5777ab21dc2e946e22a1b08872aaad72b4192976e
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **22.5 MB (22491539 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:099411d81ac7bf28b232625f19ecc6590f39c3920418958b3056caa4f85815c4`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Mon, 26 Aug 2019 23:54:26 GMT
COPY file:091d2a65366d205fc0db557b2f495da40adb5a33c9d656d02c3ea08bb22f6c4d in /etc/ssl/certs/ 
# Mon, 21 Oct 2019 20:27:55 GMT
COPY dir:e700a731062c6a1130194c74080171046494718874f8e586f78523a64d56715c in /usr/share/ 
# Tue, 10 Dec 2019 21:57:12 GMT
COPY file:ad6d99c4dea9edfff1bf18494e1c85b8a82b1a74f77a8bf3f437bd05222fbf79 in / 
# Tue, 10 Dec 2019 21:57:14 GMT
EXPOSE 80
# Tue, 10 Dec 2019 21:57:15 GMT
VOLUME [/tmp]
# Tue, 10 Dec 2019 21:57:16 GMT
ENTRYPOINT ["/traefik"]
# Tue, 10 Dec 2019 21:57:17 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.20 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:506698346e0f5f486b919abaa7bc72252b3dc553cb28e0d1a5e2b6f3708cf4c0`  
		Last Modified: Mon, 26 Aug 2019 23:55:08 GMT  
		Size: 132.0 KB (132026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46037320e6487ea40f4dfb2c29d120090739bc20051bca67eb5e64a072973136`  
		Last Modified: Mon, 21 Oct 2019 20:28:50 GMT  
		Size: 327.4 KB (327388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d0d7ab9d9ce392bdaa622a30db2df3963e7ac8b19c846fddc788b2f7fd3f890`  
		Last Modified: Tue, 10 Dec 2019 21:58:07 GMT  
		Size: 22.0 MB (22032125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:maroilles` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:3a587a9647aca9d58c237389157512cf349f00e99afc0f33959501bc5366b489
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **22.2 MB (22219190 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:843151930dcd29bc722fa2e9949bcecfcb0020d961037b85983f47017aa38a58`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Tue, 27 Aug 2019 00:16:41 GMT
COPY file:091d2a65366d205fc0db557b2f495da40adb5a33c9d656d02c3ea08bb22f6c4d in /etc/ssl/certs/ 
# Mon, 21 Oct 2019 23:22:44 GMT
COPY dir:e700a731062c6a1130194c74080171046494718874f8e586f78523a64d56715c in /usr/share/ 
# Tue, 10 Dec 2019 22:39:48 GMT
COPY file:2548a09c5388b09356e8109d52a2261b02b840df1156718406457af4ef9eedcd in / 
# Tue, 10 Dec 2019 22:39:50 GMT
EXPOSE 80
# Tue, 10 Dec 2019 22:39:50 GMT
VOLUME [/tmp]
# Tue, 10 Dec 2019 22:39:51 GMT
ENTRYPOINT ["/traefik"]
# Tue, 10 Dec 2019 22:39:51 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.20 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:f07a1cd6fb05ab2fb5b66f5326144f82e52f5580df40a42e400637f8a8f9c6d8`  
		Last Modified: Tue, 27 Aug 2019 00:17:31 GMT  
		Size: 132.0 KB (132021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af2afd881e5b94f57a79b2f6bcd9d637c2f7a6aa910f4013045b8653ebe29fdb`  
		Last Modified: Mon, 21 Oct 2019 23:23:36 GMT  
		Size: 327.4 KB (327378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b05c8936168a3f333423ce8dca6ed7e5ad1890ce50b95da487f61aa83440e26`  
		Last Modified: Tue, 10 Dec 2019 22:40:39 GMT  
		Size: 21.8 MB (21759791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:maroilles-alpine`

```console
$ docker pull traefik@sha256:ce4f1f9ec3de9c802a1d6020928358d7301452fc5c009ea314fbaa728e69aa3d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:maroilles-alpine` - linux; amd64

```console
$ docker pull traefik@sha256:f9f7bc3071415790c015ad52995e2997d9d1cfd5cffdde58cb403e15d71fbe4e
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.0 MB (27028274 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:439e73a064c8f244ce1fe21cb3abcc9b314309275e3b26fd6ac0276946f669c8`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Mon, 21 Oct 2019 17:21:42 GMT
ADD file:fe1f09249227e2da2089afb4d07e16cbf832eeb804120074acd2b8192876cd28 in / 
# Mon, 21 Oct 2019 17:21:42 GMT
CMD ["/bin/sh"]
# Mon, 21 Oct 2019 22:26:21 GMT
RUN apk --no-cache add ca-certificates tzdata
# Tue, 10 Dec 2019 22:31:01 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/containous/traefik/releases/download/v1.7.20/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Tue, 10 Dec 2019 22:31:02 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Tue, 10 Dec 2019 22:31:02 GMT
EXPOSE 80
# Tue, 10 Dec 2019 22:31:02 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 10 Dec 2019 22:31:02 GMT
CMD ["traefik"]
# Tue, 10 Dec 2019 22:31:03 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.20 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:89d9c30c1d48bac627e5c6cb0d1ed1eec28e7dbdfbcc04712e4c79c0f83faf17`  
		Last Modified: Mon, 21 Oct 2019 17:22:48 GMT  
		Size: 2.8 MB (2787134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:275722d2e7f6dc3397547bc96af555d5905a44fc2f88a1adb39ddfc6aa2a98b9`  
		Last Modified: Mon, 21 Oct 2019 22:27:05 GMT  
		Size: 694.5 KB (694493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:198d6da64444dd0f60f3c566038d6c9157c290fb6152ec296204e862073f365f`  
		Last Modified: Tue, 10 Dec 2019 22:32:13 GMT  
		Size: 23.5 MB (23546279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fd7a10facf04db24667668cb9792494b0e49f33e439cccf618f435ef237bfa3`  
		Last Modified: Tue, 10 Dec 2019 22:32:07 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:maroilles-alpine` - linux; arm variant v6

```console
$ docker pull traefik@sha256:91c059509f0cd0fbf794e278e25674fe57f5d3f4185f7ed23c6915852d437f05
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.3 MB (25301854 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e0fb17b7213044c3a520701dcb0f1b21f9fa79d3f0ed57cebfef9dc91a064913`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Mon, 21 Oct 2019 16:56:02 GMT
ADD file:d3c7d938a78143f106a6a467ce23b599198e041220e661e5326ba91054c353ef in / 
# Mon, 21 Oct 2019 16:56:04 GMT
CMD ["/bin/sh"]
# Mon, 21 Oct 2019 20:27:15 GMT
RUN apk --no-cache add ca-certificates tzdata
# Tue, 10 Dec 2019 21:49:54 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/containous/traefik/releases/download/v1.7.20/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Tue, 10 Dec 2019 21:49:55 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Tue, 10 Dec 2019 21:49:56 GMT
EXPOSE 80
# Tue, 10 Dec 2019 21:49:56 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 10 Dec 2019 21:49:57 GMT
CMD ["traefik"]
# Tue, 10 Dec 2019 21:49:57 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.20 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:ecf664be551d26dcd221b7387283cdcc54f46c6789700d037fa3cd0c297f8645`  
		Last Modified: Mon, 21 Oct 2019 16:56:34 GMT  
		Size: 2.6 MB (2571309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e75226f24cf5fc4e2d56fbb31d8daf122273d120792aff22dee3a970a5419ee9`  
		Last Modified: Mon, 21 Oct 2019 20:28:17 GMT  
		Size: 697.8 KB (697821 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdd02ec506a5475103a69714675382b27257bcb6710941053abde15b07f1f473`  
		Last Modified: Tue, 10 Dec 2019 21:57:48 GMT  
		Size: 22.0 MB (22032356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27ff5f776c2bcd52a563737242a856d37745bdd6947d9989ee6aec3157f6db81`  
		Last Modified: Tue, 10 Dec 2019 21:57:39 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:maroilles-alpine` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:69880c97f253a7dab9e3fb1e477bc209a297ceb369f259841a14ec194ac5fbe3
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.2 MB (25175702 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:630da378646ff9d16799a8f19fc83d02d28fe478003b44b8f37a8b0a4b715079`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Mon, 21 Oct 2019 18:07:03 GMT
ADD file:02f4d68afd9e9e303ff893f198d535d0d78c4b2554f299ab2d0955b2bef0e06a in / 
# Mon, 21 Oct 2019 18:07:09 GMT
CMD ["/bin/sh"]
# Mon, 21 Oct 2019 23:22:16 GMT
RUN apk --no-cache add ca-certificates tzdata
# Tue, 10 Dec 2019 22:39:26 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/containous/traefik/releases/download/v1.7.20/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Tue, 10 Dec 2019 22:39:27 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Tue, 10 Dec 2019 22:39:27 GMT
EXPOSE 80
# Tue, 10 Dec 2019 22:39:28 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 10 Dec 2019 22:39:28 GMT
CMD ["traefik"]
# Tue, 10 Dec 2019 22:39:29 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.20 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:8bfa913040406727f36faa9b69d0b96e071b13792a83ad69c19389031a9f3797`  
		Last Modified: Mon, 21 Oct 2019 18:08:36 GMT  
		Size: 2.7 MB (2717778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a21b1a0e782f54ba929f36f1f589cbf9cacb6e15d6644d901741533bec314cec`  
		Last Modified: Mon, 21 Oct 2019 23:23:04 GMT  
		Size: 697.9 KB (697888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a1ad2d17ee7cb6da8499ef5415cad503d05873da472bcfc6d2ac07e9bdbad2c`  
		Last Modified: Tue, 10 Dec 2019 22:40:19 GMT  
		Size: 21.8 MB (21759668 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9525ac7ce9940a937d298cf00954af64fd399df1a840cad75914caeb0b5cf224`  
		Last Modified: Tue, 10 Dec 2019 22:40:11 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:maroilles-windowsservercore-1809`

```console
$ docker pull traefik@sha256:122b54d5a8a5cccc8839e7a3ce5c385c0b04a9c02ba4c741ea8a82f4a58ff6c8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.914; amd64

### `traefik:maroilles-windowsservercore-1809` - windows version 10.0.17763.914; amd64

```console
$ docker pull traefik@sha256:0092b009fa818e0152462c069457055244a329e613e4f4e86801363bcbabfdd2
```

-	Docker Version: 18.03.1-ee-4
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.2 GB (2244435166 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:49463175a868dfe3c0a39b4693212b98b6d9da1043bf4b1b18570bef3a010859`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 15 Sep 2018 09:10:26 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 29 Nov 2019 04:34:15 GMT
RUN Install update 1809-amd64
# Tue, 10 Dec 2019 21:34:07 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 10 Dec 2019 22:06:49 GMT
RUN Invoke-WebRequest     -Uri "https://github.com/containous/traefik/releases/download/v1.7.20/traefik_windows-amd64.exe"     -OutFile "/traefik.exe"
# Tue, 10 Dec 2019 22:06:55 GMT
EXPOSE 80
# Tue, 10 Dec 2019 22:06:56 GMT
ENTRYPOINT ["/traefik"]
# Tue, 10 Dec 2019 22:06:58 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.20 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:65014b3c312172f10bd6701a063f9b5aaf9a916c2d2cb843d406a6f77ded3f8d`  
		Last Modified: Tue, 13 Nov 2018 18:50:17 GMT  
		Size: 1.5 GB (1534685324 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:faf31ee0aa3d3c60a38dd03c7554d632065cef50eab052ef1444590786249d07`  
		Size: 681.6 MB (681618026 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e147f14e0d6a9cbd5261162dea8f3aac7a34db5d9f6a587a9aac6b88722a2da4`  
		Last Modified: Tue, 10 Dec 2019 22:07:34 GMT  
		Size: 1.2 KB (1211 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59c8ec155d3968143fbceaac2d3d287e2a97d836b6dcf3ca1418e8bea4cd0062`  
		Last Modified: Tue, 10 Dec 2019 22:08:38 GMT  
		Size: 28.1 MB (28127080 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7f47f2cf9e401dfd15ca112b20632f36aa0a56f5f404643720a8a11aad1bb28`  
		Last Modified: Tue, 10 Dec 2019 22:08:32 GMT  
		Size: 1.2 KB (1180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e11ec09770c3643d749d678f579e251ceeaabb28536596e148ee6b71b93981cb`  
		Last Modified: Tue, 10 Dec 2019 22:08:30 GMT  
		Size: 1.2 KB (1183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2df6a0c73ef71f2868be658441f5856463b1de3edc2e49e66f13c86551981a3`  
		Last Modified: Tue, 10 Dec 2019 22:08:31 GMT  
		Size: 1.2 KB (1162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v1.7`

```console
$ docker pull traefik@sha256:5ec34caf19d114f8f0ed76f9bc3dad6ba8cf6d13a1575c4294b59b77709def39
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:v1.7` - linux; amd64

```console
$ docker pull traefik@sha256:3b1c4d57c57d125a5d949d463d41882fefc957ce117db226aace4e7314e82d5c
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **24.0 MB (24005352 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:96c63a7d3e502fcbbd8937a2523368c22d0edd1788b8389af095f64038318834`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Tue, 27 Aug 2019 01:00:22 GMT
COPY file:091d2a65366d205fc0db557b2f495da40adb5a33c9d656d02c3ea08bb22f6c4d in /etc/ssl/certs/ 
# Mon, 21 Oct 2019 22:26:52 GMT
COPY dir:e700a731062c6a1130194c74080171046494718874f8e586f78523a64d56715c in /usr/share/ 
# Tue, 10 Dec 2019 22:31:38 GMT
COPY file:be1ea92a6d3f63051c9ae787ca41c986b81a56ce7f8b8347b97c3ddc3b4471f5 in / 
# Tue, 10 Dec 2019 22:31:38 GMT
EXPOSE 80
# Tue, 10 Dec 2019 22:31:38 GMT
VOLUME [/tmp]
# Tue, 10 Dec 2019 22:31:38 GMT
ENTRYPOINT ["/traefik"]
# Tue, 10 Dec 2019 22:31:39 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.20 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:42e7d26ec3785f8ce0f20e327cf72404ee054ba022ce9068ad2d28c52e82db2a`  
		Last Modified: Tue, 27 Aug 2019 01:00:52 GMT  
		Size: 132.0 KB (132022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a753f02eeffef33e5e071a6feac9e12fffb36330fc7ef5441f378d0ce67c528`  
		Last Modified: Mon, 21 Oct 2019 22:27:25 GMT  
		Size: 327.3 KB (327346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab927d94d255c72862c3e7ada3f6cdb36f90926b7a8913a080062b17d73f186b`  
		Last Modified: Tue, 10 Dec 2019 22:32:27 GMT  
		Size: 23.5 MB (23545984 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v1.7` - linux; arm variant v6

```console
$ docker pull traefik@sha256:3a32e589b7d538f688f0a4d5777ab21dc2e946e22a1b08872aaad72b4192976e
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **22.5 MB (22491539 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:099411d81ac7bf28b232625f19ecc6590f39c3920418958b3056caa4f85815c4`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Mon, 26 Aug 2019 23:54:26 GMT
COPY file:091d2a65366d205fc0db557b2f495da40adb5a33c9d656d02c3ea08bb22f6c4d in /etc/ssl/certs/ 
# Mon, 21 Oct 2019 20:27:55 GMT
COPY dir:e700a731062c6a1130194c74080171046494718874f8e586f78523a64d56715c in /usr/share/ 
# Tue, 10 Dec 2019 21:57:12 GMT
COPY file:ad6d99c4dea9edfff1bf18494e1c85b8a82b1a74f77a8bf3f437bd05222fbf79 in / 
# Tue, 10 Dec 2019 21:57:14 GMT
EXPOSE 80
# Tue, 10 Dec 2019 21:57:15 GMT
VOLUME [/tmp]
# Tue, 10 Dec 2019 21:57:16 GMT
ENTRYPOINT ["/traefik"]
# Tue, 10 Dec 2019 21:57:17 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.20 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:506698346e0f5f486b919abaa7bc72252b3dc553cb28e0d1a5e2b6f3708cf4c0`  
		Last Modified: Mon, 26 Aug 2019 23:55:08 GMT  
		Size: 132.0 KB (132026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46037320e6487ea40f4dfb2c29d120090739bc20051bca67eb5e64a072973136`  
		Last Modified: Mon, 21 Oct 2019 20:28:50 GMT  
		Size: 327.4 KB (327388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d0d7ab9d9ce392bdaa622a30db2df3963e7ac8b19c846fddc788b2f7fd3f890`  
		Last Modified: Tue, 10 Dec 2019 21:58:07 GMT  
		Size: 22.0 MB (22032125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v1.7` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:3a587a9647aca9d58c237389157512cf349f00e99afc0f33959501bc5366b489
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **22.2 MB (22219190 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:843151930dcd29bc722fa2e9949bcecfcb0020d961037b85983f47017aa38a58`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Tue, 27 Aug 2019 00:16:41 GMT
COPY file:091d2a65366d205fc0db557b2f495da40adb5a33c9d656d02c3ea08bb22f6c4d in /etc/ssl/certs/ 
# Mon, 21 Oct 2019 23:22:44 GMT
COPY dir:e700a731062c6a1130194c74080171046494718874f8e586f78523a64d56715c in /usr/share/ 
# Tue, 10 Dec 2019 22:39:48 GMT
COPY file:2548a09c5388b09356e8109d52a2261b02b840df1156718406457af4ef9eedcd in / 
# Tue, 10 Dec 2019 22:39:50 GMT
EXPOSE 80
# Tue, 10 Dec 2019 22:39:50 GMT
VOLUME [/tmp]
# Tue, 10 Dec 2019 22:39:51 GMT
ENTRYPOINT ["/traefik"]
# Tue, 10 Dec 2019 22:39:51 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.20 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:f07a1cd6fb05ab2fb5b66f5326144f82e52f5580df40a42e400637f8a8f9c6d8`  
		Last Modified: Tue, 27 Aug 2019 00:17:31 GMT  
		Size: 132.0 KB (132021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af2afd881e5b94f57a79b2f6bcd9d637c2f7a6aa910f4013045b8653ebe29fdb`  
		Last Modified: Mon, 21 Oct 2019 23:23:36 GMT  
		Size: 327.4 KB (327378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b05c8936168a3f333423ce8dca6ed7e5ad1890ce50b95da487f61aa83440e26`  
		Last Modified: Tue, 10 Dec 2019 22:40:39 GMT  
		Size: 21.8 MB (21759791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v1.7.20`

```console
$ docker pull traefik@sha256:5ec34caf19d114f8f0ed76f9bc3dad6ba8cf6d13a1575c4294b59b77709def39
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:v1.7.20` - linux; amd64

```console
$ docker pull traefik@sha256:3b1c4d57c57d125a5d949d463d41882fefc957ce117db226aace4e7314e82d5c
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **24.0 MB (24005352 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:96c63a7d3e502fcbbd8937a2523368c22d0edd1788b8389af095f64038318834`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Tue, 27 Aug 2019 01:00:22 GMT
COPY file:091d2a65366d205fc0db557b2f495da40adb5a33c9d656d02c3ea08bb22f6c4d in /etc/ssl/certs/ 
# Mon, 21 Oct 2019 22:26:52 GMT
COPY dir:e700a731062c6a1130194c74080171046494718874f8e586f78523a64d56715c in /usr/share/ 
# Tue, 10 Dec 2019 22:31:38 GMT
COPY file:be1ea92a6d3f63051c9ae787ca41c986b81a56ce7f8b8347b97c3ddc3b4471f5 in / 
# Tue, 10 Dec 2019 22:31:38 GMT
EXPOSE 80
# Tue, 10 Dec 2019 22:31:38 GMT
VOLUME [/tmp]
# Tue, 10 Dec 2019 22:31:38 GMT
ENTRYPOINT ["/traefik"]
# Tue, 10 Dec 2019 22:31:39 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.20 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:42e7d26ec3785f8ce0f20e327cf72404ee054ba022ce9068ad2d28c52e82db2a`  
		Last Modified: Tue, 27 Aug 2019 01:00:52 GMT  
		Size: 132.0 KB (132022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a753f02eeffef33e5e071a6feac9e12fffb36330fc7ef5441f378d0ce67c528`  
		Last Modified: Mon, 21 Oct 2019 22:27:25 GMT  
		Size: 327.3 KB (327346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab927d94d255c72862c3e7ada3f6cdb36f90926b7a8913a080062b17d73f186b`  
		Last Modified: Tue, 10 Dec 2019 22:32:27 GMT  
		Size: 23.5 MB (23545984 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v1.7.20` - linux; arm variant v6

```console
$ docker pull traefik@sha256:3a32e589b7d538f688f0a4d5777ab21dc2e946e22a1b08872aaad72b4192976e
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **22.5 MB (22491539 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:099411d81ac7bf28b232625f19ecc6590f39c3920418958b3056caa4f85815c4`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Mon, 26 Aug 2019 23:54:26 GMT
COPY file:091d2a65366d205fc0db557b2f495da40adb5a33c9d656d02c3ea08bb22f6c4d in /etc/ssl/certs/ 
# Mon, 21 Oct 2019 20:27:55 GMT
COPY dir:e700a731062c6a1130194c74080171046494718874f8e586f78523a64d56715c in /usr/share/ 
# Tue, 10 Dec 2019 21:57:12 GMT
COPY file:ad6d99c4dea9edfff1bf18494e1c85b8a82b1a74f77a8bf3f437bd05222fbf79 in / 
# Tue, 10 Dec 2019 21:57:14 GMT
EXPOSE 80
# Tue, 10 Dec 2019 21:57:15 GMT
VOLUME [/tmp]
# Tue, 10 Dec 2019 21:57:16 GMT
ENTRYPOINT ["/traefik"]
# Tue, 10 Dec 2019 21:57:17 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.20 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:506698346e0f5f486b919abaa7bc72252b3dc553cb28e0d1a5e2b6f3708cf4c0`  
		Last Modified: Mon, 26 Aug 2019 23:55:08 GMT  
		Size: 132.0 KB (132026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46037320e6487ea40f4dfb2c29d120090739bc20051bca67eb5e64a072973136`  
		Last Modified: Mon, 21 Oct 2019 20:28:50 GMT  
		Size: 327.4 KB (327388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d0d7ab9d9ce392bdaa622a30db2df3963e7ac8b19c846fddc788b2f7fd3f890`  
		Last Modified: Tue, 10 Dec 2019 21:58:07 GMT  
		Size: 22.0 MB (22032125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v1.7.20` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:3a587a9647aca9d58c237389157512cf349f00e99afc0f33959501bc5366b489
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **22.2 MB (22219190 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:843151930dcd29bc722fa2e9949bcecfcb0020d961037b85983f47017aa38a58`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Tue, 27 Aug 2019 00:16:41 GMT
COPY file:091d2a65366d205fc0db557b2f495da40adb5a33c9d656d02c3ea08bb22f6c4d in /etc/ssl/certs/ 
# Mon, 21 Oct 2019 23:22:44 GMT
COPY dir:e700a731062c6a1130194c74080171046494718874f8e586f78523a64d56715c in /usr/share/ 
# Tue, 10 Dec 2019 22:39:48 GMT
COPY file:2548a09c5388b09356e8109d52a2261b02b840df1156718406457af4ef9eedcd in / 
# Tue, 10 Dec 2019 22:39:50 GMT
EXPOSE 80
# Tue, 10 Dec 2019 22:39:50 GMT
VOLUME [/tmp]
# Tue, 10 Dec 2019 22:39:51 GMT
ENTRYPOINT ["/traefik"]
# Tue, 10 Dec 2019 22:39:51 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.20 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:f07a1cd6fb05ab2fb5b66f5326144f82e52f5580df40a42e400637f8a8f9c6d8`  
		Last Modified: Tue, 27 Aug 2019 00:17:31 GMT  
		Size: 132.0 KB (132021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af2afd881e5b94f57a79b2f6bcd9d637c2f7a6aa910f4013045b8653ebe29fdb`  
		Last Modified: Mon, 21 Oct 2019 23:23:36 GMT  
		Size: 327.4 KB (327378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b05c8936168a3f333423ce8dca6ed7e5ad1890ce50b95da487f61aa83440e26`  
		Last Modified: Tue, 10 Dec 2019 22:40:39 GMT  
		Size: 21.8 MB (21759791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v1.7.20-alpine`

```console
$ docker pull traefik@sha256:ce4f1f9ec3de9c802a1d6020928358d7301452fc5c009ea314fbaa728e69aa3d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:v1.7.20-alpine` - linux; amd64

```console
$ docker pull traefik@sha256:f9f7bc3071415790c015ad52995e2997d9d1cfd5cffdde58cb403e15d71fbe4e
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.0 MB (27028274 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:439e73a064c8f244ce1fe21cb3abcc9b314309275e3b26fd6ac0276946f669c8`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Mon, 21 Oct 2019 17:21:42 GMT
ADD file:fe1f09249227e2da2089afb4d07e16cbf832eeb804120074acd2b8192876cd28 in / 
# Mon, 21 Oct 2019 17:21:42 GMT
CMD ["/bin/sh"]
# Mon, 21 Oct 2019 22:26:21 GMT
RUN apk --no-cache add ca-certificates tzdata
# Tue, 10 Dec 2019 22:31:01 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/containous/traefik/releases/download/v1.7.20/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Tue, 10 Dec 2019 22:31:02 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Tue, 10 Dec 2019 22:31:02 GMT
EXPOSE 80
# Tue, 10 Dec 2019 22:31:02 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 10 Dec 2019 22:31:02 GMT
CMD ["traefik"]
# Tue, 10 Dec 2019 22:31:03 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.20 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:89d9c30c1d48bac627e5c6cb0d1ed1eec28e7dbdfbcc04712e4c79c0f83faf17`  
		Last Modified: Mon, 21 Oct 2019 17:22:48 GMT  
		Size: 2.8 MB (2787134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:275722d2e7f6dc3397547bc96af555d5905a44fc2f88a1adb39ddfc6aa2a98b9`  
		Last Modified: Mon, 21 Oct 2019 22:27:05 GMT  
		Size: 694.5 KB (694493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:198d6da64444dd0f60f3c566038d6c9157c290fb6152ec296204e862073f365f`  
		Last Modified: Tue, 10 Dec 2019 22:32:13 GMT  
		Size: 23.5 MB (23546279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fd7a10facf04db24667668cb9792494b0e49f33e439cccf618f435ef237bfa3`  
		Last Modified: Tue, 10 Dec 2019 22:32:07 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v1.7.20-alpine` - linux; arm variant v6

```console
$ docker pull traefik@sha256:91c059509f0cd0fbf794e278e25674fe57f5d3f4185f7ed23c6915852d437f05
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.3 MB (25301854 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e0fb17b7213044c3a520701dcb0f1b21f9fa79d3f0ed57cebfef9dc91a064913`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Mon, 21 Oct 2019 16:56:02 GMT
ADD file:d3c7d938a78143f106a6a467ce23b599198e041220e661e5326ba91054c353ef in / 
# Mon, 21 Oct 2019 16:56:04 GMT
CMD ["/bin/sh"]
# Mon, 21 Oct 2019 20:27:15 GMT
RUN apk --no-cache add ca-certificates tzdata
# Tue, 10 Dec 2019 21:49:54 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/containous/traefik/releases/download/v1.7.20/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Tue, 10 Dec 2019 21:49:55 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Tue, 10 Dec 2019 21:49:56 GMT
EXPOSE 80
# Tue, 10 Dec 2019 21:49:56 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 10 Dec 2019 21:49:57 GMT
CMD ["traefik"]
# Tue, 10 Dec 2019 21:49:57 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.20 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:ecf664be551d26dcd221b7387283cdcc54f46c6789700d037fa3cd0c297f8645`  
		Last Modified: Mon, 21 Oct 2019 16:56:34 GMT  
		Size: 2.6 MB (2571309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e75226f24cf5fc4e2d56fbb31d8daf122273d120792aff22dee3a970a5419ee9`  
		Last Modified: Mon, 21 Oct 2019 20:28:17 GMT  
		Size: 697.8 KB (697821 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdd02ec506a5475103a69714675382b27257bcb6710941053abde15b07f1f473`  
		Last Modified: Tue, 10 Dec 2019 21:57:48 GMT  
		Size: 22.0 MB (22032356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27ff5f776c2bcd52a563737242a856d37745bdd6947d9989ee6aec3157f6db81`  
		Last Modified: Tue, 10 Dec 2019 21:57:39 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v1.7.20-alpine` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:69880c97f253a7dab9e3fb1e477bc209a297ceb369f259841a14ec194ac5fbe3
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.2 MB (25175702 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:630da378646ff9d16799a8f19fc83d02d28fe478003b44b8f37a8b0a4b715079`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Mon, 21 Oct 2019 18:07:03 GMT
ADD file:02f4d68afd9e9e303ff893f198d535d0d78c4b2554f299ab2d0955b2bef0e06a in / 
# Mon, 21 Oct 2019 18:07:09 GMT
CMD ["/bin/sh"]
# Mon, 21 Oct 2019 23:22:16 GMT
RUN apk --no-cache add ca-certificates tzdata
# Tue, 10 Dec 2019 22:39:26 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/containous/traefik/releases/download/v1.7.20/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Tue, 10 Dec 2019 22:39:27 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Tue, 10 Dec 2019 22:39:27 GMT
EXPOSE 80
# Tue, 10 Dec 2019 22:39:28 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 10 Dec 2019 22:39:28 GMT
CMD ["traefik"]
# Tue, 10 Dec 2019 22:39:29 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.20 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:8bfa913040406727f36faa9b69d0b96e071b13792a83ad69c19389031a9f3797`  
		Last Modified: Mon, 21 Oct 2019 18:08:36 GMT  
		Size: 2.7 MB (2717778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a21b1a0e782f54ba929f36f1f589cbf9cacb6e15d6644d901741533bec314cec`  
		Last Modified: Mon, 21 Oct 2019 23:23:04 GMT  
		Size: 697.9 KB (697888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a1ad2d17ee7cb6da8499ef5415cad503d05873da472bcfc6d2ac07e9bdbad2c`  
		Last Modified: Tue, 10 Dec 2019 22:40:19 GMT  
		Size: 21.8 MB (21759668 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9525ac7ce9940a937d298cf00954af64fd399df1a840cad75914caeb0b5cf224`  
		Last Modified: Tue, 10 Dec 2019 22:40:11 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v1.7.20-windowsservercore-1809`

```console
$ docker pull traefik@sha256:122b54d5a8a5cccc8839e7a3ce5c385c0b04a9c02ba4c741ea8a82f4a58ff6c8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.914; amd64

### `traefik:v1.7.20-windowsservercore-1809` - windows version 10.0.17763.914; amd64

```console
$ docker pull traefik@sha256:0092b009fa818e0152462c069457055244a329e613e4f4e86801363bcbabfdd2
```

-	Docker Version: 18.03.1-ee-4
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.2 GB (2244435166 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:49463175a868dfe3c0a39b4693212b98b6d9da1043bf4b1b18570bef3a010859`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 15 Sep 2018 09:10:26 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 29 Nov 2019 04:34:15 GMT
RUN Install update 1809-amd64
# Tue, 10 Dec 2019 21:34:07 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 10 Dec 2019 22:06:49 GMT
RUN Invoke-WebRequest     -Uri "https://github.com/containous/traefik/releases/download/v1.7.20/traefik_windows-amd64.exe"     -OutFile "/traefik.exe"
# Tue, 10 Dec 2019 22:06:55 GMT
EXPOSE 80
# Tue, 10 Dec 2019 22:06:56 GMT
ENTRYPOINT ["/traefik"]
# Tue, 10 Dec 2019 22:06:58 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.20 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:65014b3c312172f10bd6701a063f9b5aaf9a916c2d2cb843d406a6f77ded3f8d`  
		Last Modified: Tue, 13 Nov 2018 18:50:17 GMT  
		Size: 1.5 GB (1534685324 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:faf31ee0aa3d3c60a38dd03c7554d632065cef50eab052ef1444590786249d07`  
		Size: 681.6 MB (681618026 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e147f14e0d6a9cbd5261162dea8f3aac7a34db5d9f6a587a9aac6b88722a2da4`  
		Last Modified: Tue, 10 Dec 2019 22:07:34 GMT  
		Size: 1.2 KB (1211 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59c8ec155d3968143fbceaac2d3d287e2a97d836b6dcf3ca1418e8bea4cd0062`  
		Last Modified: Tue, 10 Dec 2019 22:08:38 GMT  
		Size: 28.1 MB (28127080 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7f47f2cf9e401dfd15ca112b20632f36aa0a56f5f404643720a8a11aad1bb28`  
		Last Modified: Tue, 10 Dec 2019 22:08:32 GMT  
		Size: 1.2 KB (1180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e11ec09770c3643d749d678f579e251ceeaabb28536596e148ee6b71b93981cb`  
		Last Modified: Tue, 10 Dec 2019 22:08:30 GMT  
		Size: 1.2 KB (1183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2df6a0c73ef71f2868be658441f5856463b1de3edc2e49e66f13c86551981a3`  
		Last Modified: Tue, 10 Dec 2019 22:08:31 GMT  
		Size: 1.2 KB (1162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v1.7-alpine`

```console
$ docker pull traefik@sha256:ce4f1f9ec3de9c802a1d6020928358d7301452fc5c009ea314fbaa728e69aa3d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:v1.7-alpine` - linux; amd64

```console
$ docker pull traefik@sha256:f9f7bc3071415790c015ad52995e2997d9d1cfd5cffdde58cb403e15d71fbe4e
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.0 MB (27028274 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:439e73a064c8f244ce1fe21cb3abcc9b314309275e3b26fd6ac0276946f669c8`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Mon, 21 Oct 2019 17:21:42 GMT
ADD file:fe1f09249227e2da2089afb4d07e16cbf832eeb804120074acd2b8192876cd28 in / 
# Mon, 21 Oct 2019 17:21:42 GMT
CMD ["/bin/sh"]
# Mon, 21 Oct 2019 22:26:21 GMT
RUN apk --no-cache add ca-certificates tzdata
# Tue, 10 Dec 2019 22:31:01 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/containous/traefik/releases/download/v1.7.20/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Tue, 10 Dec 2019 22:31:02 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Tue, 10 Dec 2019 22:31:02 GMT
EXPOSE 80
# Tue, 10 Dec 2019 22:31:02 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 10 Dec 2019 22:31:02 GMT
CMD ["traefik"]
# Tue, 10 Dec 2019 22:31:03 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.20 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:89d9c30c1d48bac627e5c6cb0d1ed1eec28e7dbdfbcc04712e4c79c0f83faf17`  
		Last Modified: Mon, 21 Oct 2019 17:22:48 GMT  
		Size: 2.8 MB (2787134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:275722d2e7f6dc3397547bc96af555d5905a44fc2f88a1adb39ddfc6aa2a98b9`  
		Last Modified: Mon, 21 Oct 2019 22:27:05 GMT  
		Size: 694.5 KB (694493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:198d6da64444dd0f60f3c566038d6c9157c290fb6152ec296204e862073f365f`  
		Last Modified: Tue, 10 Dec 2019 22:32:13 GMT  
		Size: 23.5 MB (23546279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fd7a10facf04db24667668cb9792494b0e49f33e439cccf618f435ef237bfa3`  
		Last Modified: Tue, 10 Dec 2019 22:32:07 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v1.7-alpine` - linux; arm variant v6

```console
$ docker pull traefik@sha256:91c059509f0cd0fbf794e278e25674fe57f5d3f4185f7ed23c6915852d437f05
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.3 MB (25301854 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e0fb17b7213044c3a520701dcb0f1b21f9fa79d3f0ed57cebfef9dc91a064913`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Mon, 21 Oct 2019 16:56:02 GMT
ADD file:d3c7d938a78143f106a6a467ce23b599198e041220e661e5326ba91054c353ef in / 
# Mon, 21 Oct 2019 16:56:04 GMT
CMD ["/bin/sh"]
# Mon, 21 Oct 2019 20:27:15 GMT
RUN apk --no-cache add ca-certificates tzdata
# Tue, 10 Dec 2019 21:49:54 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/containous/traefik/releases/download/v1.7.20/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Tue, 10 Dec 2019 21:49:55 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Tue, 10 Dec 2019 21:49:56 GMT
EXPOSE 80
# Tue, 10 Dec 2019 21:49:56 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 10 Dec 2019 21:49:57 GMT
CMD ["traefik"]
# Tue, 10 Dec 2019 21:49:57 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.20 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:ecf664be551d26dcd221b7387283cdcc54f46c6789700d037fa3cd0c297f8645`  
		Last Modified: Mon, 21 Oct 2019 16:56:34 GMT  
		Size: 2.6 MB (2571309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e75226f24cf5fc4e2d56fbb31d8daf122273d120792aff22dee3a970a5419ee9`  
		Last Modified: Mon, 21 Oct 2019 20:28:17 GMT  
		Size: 697.8 KB (697821 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdd02ec506a5475103a69714675382b27257bcb6710941053abde15b07f1f473`  
		Last Modified: Tue, 10 Dec 2019 21:57:48 GMT  
		Size: 22.0 MB (22032356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27ff5f776c2bcd52a563737242a856d37745bdd6947d9989ee6aec3157f6db81`  
		Last Modified: Tue, 10 Dec 2019 21:57:39 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v1.7-alpine` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:69880c97f253a7dab9e3fb1e477bc209a297ceb369f259841a14ec194ac5fbe3
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.2 MB (25175702 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:630da378646ff9d16799a8f19fc83d02d28fe478003b44b8f37a8b0a4b715079`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Mon, 21 Oct 2019 18:07:03 GMT
ADD file:02f4d68afd9e9e303ff893f198d535d0d78c4b2554f299ab2d0955b2bef0e06a in / 
# Mon, 21 Oct 2019 18:07:09 GMT
CMD ["/bin/sh"]
# Mon, 21 Oct 2019 23:22:16 GMT
RUN apk --no-cache add ca-certificates tzdata
# Tue, 10 Dec 2019 22:39:26 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/containous/traefik/releases/download/v1.7.20/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Tue, 10 Dec 2019 22:39:27 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Tue, 10 Dec 2019 22:39:27 GMT
EXPOSE 80
# Tue, 10 Dec 2019 22:39:28 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 10 Dec 2019 22:39:28 GMT
CMD ["traefik"]
# Tue, 10 Dec 2019 22:39:29 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.20 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:8bfa913040406727f36faa9b69d0b96e071b13792a83ad69c19389031a9f3797`  
		Last Modified: Mon, 21 Oct 2019 18:08:36 GMT  
		Size: 2.7 MB (2717778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a21b1a0e782f54ba929f36f1f589cbf9cacb6e15d6644d901741533bec314cec`  
		Last Modified: Mon, 21 Oct 2019 23:23:04 GMT  
		Size: 697.9 KB (697888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a1ad2d17ee7cb6da8499ef5415cad503d05873da472bcfc6d2ac07e9bdbad2c`  
		Last Modified: Tue, 10 Dec 2019 22:40:19 GMT  
		Size: 21.8 MB (21759668 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9525ac7ce9940a937d298cf00954af64fd399df1a840cad75914caeb0b5cf224`  
		Last Modified: Tue, 10 Dec 2019 22:40:11 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v1.7-windowsservercore-1809`

```console
$ docker pull traefik@sha256:122b54d5a8a5cccc8839e7a3ce5c385c0b04a9c02ba4c741ea8a82f4a58ff6c8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.914; amd64

### `traefik:v1.7-windowsservercore-1809` - windows version 10.0.17763.914; amd64

```console
$ docker pull traefik@sha256:0092b009fa818e0152462c069457055244a329e613e4f4e86801363bcbabfdd2
```

-	Docker Version: 18.03.1-ee-4
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.2 GB (2244435166 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:49463175a868dfe3c0a39b4693212b98b6d9da1043bf4b1b18570bef3a010859`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 15 Sep 2018 09:10:26 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 29 Nov 2019 04:34:15 GMT
RUN Install update 1809-amd64
# Tue, 10 Dec 2019 21:34:07 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 10 Dec 2019 22:06:49 GMT
RUN Invoke-WebRequest     -Uri "https://github.com/containous/traefik/releases/download/v1.7.20/traefik_windows-amd64.exe"     -OutFile "/traefik.exe"
# Tue, 10 Dec 2019 22:06:55 GMT
EXPOSE 80
# Tue, 10 Dec 2019 22:06:56 GMT
ENTRYPOINT ["/traefik"]
# Tue, 10 Dec 2019 22:06:58 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.20 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:65014b3c312172f10bd6701a063f9b5aaf9a916c2d2cb843d406a6f77ded3f8d`  
		Last Modified: Tue, 13 Nov 2018 18:50:17 GMT  
		Size: 1.5 GB (1534685324 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:faf31ee0aa3d3c60a38dd03c7554d632065cef50eab052ef1444590786249d07`  
		Size: 681.6 MB (681618026 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e147f14e0d6a9cbd5261162dea8f3aac7a34db5d9f6a587a9aac6b88722a2da4`  
		Last Modified: Tue, 10 Dec 2019 22:07:34 GMT  
		Size: 1.2 KB (1211 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59c8ec155d3968143fbceaac2d3d287e2a97d836b6dcf3ca1418e8bea4cd0062`  
		Last Modified: Tue, 10 Dec 2019 22:08:38 GMT  
		Size: 28.1 MB (28127080 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7f47f2cf9e401dfd15ca112b20632f36aa0a56f5f404643720a8a11aad1bb28`  
		Last Modified: Tue, 10 Dec 2019 22:08:32 GMT  
		Size: 1.2 KB (1180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e11ec09770c3643d749d678f579e251ceeaabb28536596e148ee6b71b93981cb`  
		Last Modified: Tue, 10 Dec 2019 22:08:30 GMT  
		Size: 1.2 KB (1183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2df6a0c73ef71f2868be658441f5856463b1de3edc2e49e66f13c86551981a3`  
		Last Modified: Tue, 10 Dec 2019 22:08:31 GMT  
		Size: 1.2 KB (1162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v2.1`

```console
$ docker pull traefik@sha256:a87b61f3254d03c4fcc0b994e2cb7af89abba8178f1fbec3bce3f4bdc080f8a6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:v2.1` - linux; amd64

```console
$ docker pull traefik@sha256:b1fe8eec6330ffe542f313a21860361f266375f854804ed19893933f65a62e67
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.0 MB (22972242 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7f7affdc32376c94f75ff0112832475d1c7b5c42ae438b3208039d29451972ac`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Mon, 21 Oct 2019 17:21:42 GMT
ADD file:fe1f09249227e2da2089afb4d07e16cbf832eeb804120074acd2b8192876cd28 in / 
# Mon, 21 Oct 2019 17:21:42 GMT
CMD ["/bin/sh"]
# Mon, 21 Oct 2019 22:26:21 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 12 Dec 2019 23:39:42 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/containous/traefik/releases/download/v2.1.1/traefik_v2.1.1_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 12 Dec 2019 23:39:43 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 12 Dec 2019 23:39:43 GMT
EXPOSE 80
# Thu, 12 Dec 2019 23:39:43 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 12 Dec 2019 23:39:43 GMT
CMD ["traefik"]
# Thu, 12 Dec 2019 23:39:43 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.1.1 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:89d9c30c1d48bac627e5c6cb0d1ed1eec28e7dbdfbcc04712e4c79c0f83faf17`  
		Last Modified: Mon, 21 Oct 2019 17:22:48 GMT  
		Size: 2.8 MB (2787134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:275722d2e7f6dc3397547bc96af555d5905a44fc2f88a1adb39ddfc6aa2a98b9`  
		Last Modified: Mon, 21 Oct 2019 22:27:05 GMT  
		Size: 694.5 KB (694493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88ca2a78572e6379d1dc1b5ddfa2302e84a42a0305c9d26259ff61b40abecc6b`  
		Last Modified: Thu, 12 Dec 2019 23:40:09 GMT  
		Size: 19.5 MB (19490246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bf623a84bbbfb8681af59457bfae6ae09537f9e29ceea00d7a872b49eacc48a`  
		Last Modified: Thu, 12 Dec 2019 23:40:04 GMT  
		Size: 369.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v2.1` - linux; arm variant v6

```console
$ docker pull traefik@sha256:8893289f168246069496fb44fe86cdd862b7497d58ea0b8d3d28509655ae772a
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **21.5 MB (21530113 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ce54f5d1d0d33e5388f78cd582d4a7d81c4b3f14a68d0468d4dc5d623d12ebb6`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Mon, 21 Oct 2019 16:56:02 GMT
ADD file:d3c7d938a78143f106a6a467ce23b599198e041220e661e5326ba91054c353ef in / 
# Mon, 21 Oct 2019 16:56:04 GMT
CMD ["/bin/sh"]
# Mon, 21 Oct 2019 20:27:15 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 12 Dec 2019 23:51:04 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/containous/traefik/releases/download/v2.1.1/traefik_v2.1.1_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 12 Dec 2019 23:51:05 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 12 Dec 2019 23:51:08 GMT
EXPOSE 80
# Thu, 12 Dec 2019 23:51:10 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 12 Dec 2019 23:51:13 GMT
CMD ["traefik"]
# Thu, 12 Dec 2019 23:51:18 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.1.1 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:ecf664be551d26dcd221b7387283cdcc54f46c6789700d037fa3cd0c297f8645`  
		Last Modified: Mon, 21 Oct 2019 16:56:34 GMT  
		Size: 2.6 MB (2571309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e75226f24cf5fc4e2d56fbb31d8daf122273d120792aff22dee3a970a5419ee9`  
		Last Modified: Mon, 21 Oct 2019 20:28:17 GMT  
		Size: 697.8 KB (697821 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:226040d9e7a47f0acbdced5e006aa1261f64cacbc04f3a09f837c362a5370b13`  
		Last Modified: Thu, 12 Dec 2019 23:52:09 GMT  
		Size: 18.3 MB (18260615 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb2a0bf2df3a2bb46100add59ef6b2bbaf57b5b496a159c6a1ebc5414125d152`  
		Last Modified: Thu, 12 Dec 2019 23:52:03 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v2.1` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:d95d874b2e045fb3a8a7360180d74b2ab7414105160a5607a3b97db891517763
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **21.4 MB (21364609 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:87e3030ddfe47d09d8a165d84f5f88527465dcd247906deb639563961b0e6c40`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Mon, 21 Oct 2019 18:07:03 GMT
ADD file:02f4d68afd9e9e303ff893f198d535d0d78c4b2554f299ab2d0955b2bef0e06a in / 
# Mon, 21 Oct 2019 18:07:09 GMT
CMD ["/bin/sh"]
# Mon, 21 Oct 2019 23:22:16 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 12 Dec 2019 23:51:27 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/containous/traefik/releases/download/v2.1.1/traefik_v2.1.1_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 12 Dec 2019 23:51:29 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 12 Dec 2019 23:51:33 GMT
EXPOSE 80
# Thu, 12 Dec 2019 23:51:38 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 12 Dec 2019 23:51:42 GMT
CMD ["traefik"]
# Thu, 12 Dec 2019 23:51:46 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.1.1 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:8bfa913040406727f36faa9b69d0b96e071b13792a83ad69c19389031a9f3797`  
		Last Modified: Mon, 21 Oct 2019 18:08:36 GMT  
		Size: 2.7 MB (2717778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a21b1a0e782f54ba929f36f1f589cbf9cacb6e15d6644d901741533bec314cec`  
		Last Modified: Mon, 21 Oct 2019 23:23:04 GMT  
		Size: 697.9 KB (697888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a5093f9995081d7b5b63babf2940a3ec750e2ed80b92e822266e16e25ff41e3`  
		Last Modified: Thu, 12 Dec 2019 23:52:23 GMT  
		Size: 17.9 MB (17948574 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7095cdc86392137d36c03c39e37c62da37671933425b16232d4c528cfee11581`  
		Last Modified: Thu, 12 Dec 2019 23:52:17 GMT  
		Size: 369.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v2.1.2`

**does not exist** (yet?)

## `traefik:v2.1.2-windowsservercore-1809`

**does not exist** (yet?)

## `traefik:v2.1-windowsservercore-1809`

```console
$ docker pull traefik@sha256:72f61926c08b2013cccbe1a249a6631946ef920eca7995fa52c693c53338aa72
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.914; amd64

### `traefik:v2.1-windowsservercore-1809` - windows version 10.0.17763.914; amd64

```console
$ docker pull traefik@sha256:585f0b403374f6611b3e8d5f41460c97228dc284cbc9ce96d179a1118cdb58ab
```

-	Docker Version: 18.03.1-ee-4
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.2 GB (2240370088 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:84d0f8a51ec5aca3f2383905bb2c439c567e89ff67cd0821bd9fd4b6d38247df`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 15 Sep 2018 09:10:26 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 29 Nov 2019 04:34:15 GMT
RUN Install update 1809-amd64
# Tue, 10 Dec 2019 21:34:07 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 12 Dec 2019 23:23:21 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/containous/traefik/releases/download/v2.1.1/traefik_v2.1.1_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Thu, 12 Dec 2019 23:23:22 GMT
EXPOSE 80
# Thu, 12 Dec 2019 23:23:24 GMT
ENTRYPOINT ["/traefik"]
# Thu, 12 Dec 2019 23:23:26 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.1.1 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:65014b3c312172f10bd6701a063f9b5aaf9a916c2d2cb843d406a6f77ded3f8d`  
		Last Modified: Tue, 13 Nov 2018 18:50:17 GMT  
		Size: 1.5 GB (1534685324 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:faf31ee0aa3d3c60a38dd03c7554d632065cef50eab052ef1444590786249d07`  
		Size: 681.6 MB (681618026 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e147f14e0d6a9cbd5261162dea8f3aac7a34db5d9f6a587a9aac6b88722a2da4`  
		Last Modified: Tue, 10 Dec 2019 22:07:34 GMT  
		Size: 1.2 KB (1211 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08283c3529083d82a99e4e993d5f3b36a624cba1c0c29337b3c557881afeae2f`  
		Last Modified: Thu, 12 Dec 2019 23:24:05 GMT  
		Size: 24.1 MB (24061960 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d01b24dc42771e2aebc1ea9d6c3d1e7052eb5b5bf266ba4123a75e40c62ab076`  
		Last Modified: Thu, 12 Dec 2019 23:23:59 GMT  
		Size: 1.2 KB (1180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4bb434cba60f7b0cce45a2f1c6c00ef0e6b0bfb00a4ef097fa7797c5e074c12`  
		Last Modified: Thu, 12 Dec 2019 23:24:00 GMT  
		Size: 1.2 KB (1208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a20bcbc7f4aee693390e71290e8b6b4efb693ad5f2b2da57d1eb9add9d0bbba`  
		Last Modified: Thu, 12 Dec 2019 23:23:59 GMT  
		Size: 1.2 KB (1179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:windowsservercore-1809`

```console
$ docker pull traefik@sha256:72f61926c08b2013cccbe1a249a6631946ef920eca7995fa52c693c53338aa72
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.914; amd64

### `traefik:windowsservercore-1809` - windows version 10.0.17763.914; amd64

```console
$ docker pull traefik@sha256:585f0b403374f6611b3e8d5f41460c97228dc284cbc9ce96d179a1118cdb58ab
```

-	Docker Version: 18.03.1-ee-4
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.2 GB (2240370088 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:84d0f8a51ec5aca3f2383905bb2c439c567e89ff67cd0821bd9fd4b6d38247df`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 15 Sep 2018 09:10:26 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 29 Nov 2019 04:34:15 GMT
RUN Install update 1809-amd64
# Tue, 10 Dec 2019 21:34:07 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 12 Dec 2019 23:23:21 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/containous/traefik/releases/download/v2.1.1/traefik_v2.1.1_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Thu, 12 Dec 2019 23:23:22 GMT
EXPOSE 80
# Thu, 12 Dec 2019 23:23:24 GMT
ENTRYPOINT ["/traefik"]
# Thu, 12 Dec 2019 23:23:26 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.1.1 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:65014b3c312172f10bd6701a063f9b5aaf9a916c2d2cb843d406a6f77ded3f8d`  
		Last Modified: Tue, 13 Nov 2018 18:50:17 GMT  
		Size: 1.5 GB (1534685324 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:faf31ee0aa3d3c60a38dd03c7554d632065cef50eab052ef1444590786249d07`  
		Size: 681.6 MB (681618026 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e147f14e0d6a9cbd5261162dea8f3aac7a34db5d9f6a587a9aac6b88722a2da4`  
		Last Modified: Tue, 10 Dec 2019 22:07:34 GMT  
		Size: 1.2 KB (1211 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08283c3529083d82a99e4e993d5f3b36a624cba1c0c29337b3c557881afeae2f`  
		Last Modified: Thu, 12 Dec 2019 23:24:05 GMT  
		Size: 24.1 MB (24061960 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d01b24dc42771e2aebc1ea9d6c3d1e7052eb5b5bf266ba4123a75e40c62ab076`  
		Last Modified: Thu, 12 Dec 2019 23:23:59 GMT  
		Size: 1.2 KB (1180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4bb434cba60f7b0cce45a2f1c6c00ef0e6b0bfb00a4ef097fa7797c5e074c12`  
		Last Modified: Thu, 12 Dec 2019 23:24:00 GMT  
		Size: 1.2 KB (1208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a20bcbc7f4aee693390e71290e8b6b4efb693ad5f2b2da57d1eb9add9d0bbba`  
		Last Modified: Thu, 12 Dec 2019 23:23:59 GMT  
		Size: 1.2 KB (1179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
