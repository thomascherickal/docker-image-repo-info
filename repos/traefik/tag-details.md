<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `traefik`

-	[`traefik:1.7`](#traefik17)
-	[`traefik:1.7.20`](#traefik1720)
-	[`traefik:1.7.20-alpine`](#traefik1720-alpine)
-	[`traefik:1.7.20-windowsservercore-1809`](#traefik1720-windowsservercore-1809)
-	[`traefik:1.7-alpine`](#traefik17-alpine)
-	[`traefik:1.7-windowsservercore-1809`](#traefik17-windowsservercore-1809)
-	[`traefik:2.1`](#traefik21)
-	[`traefik:2.1.3`](#traefik213)
-	[`traefik:2.1.3-windowsservercore-1809`](#traefik213-windowsservercore-1809)
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
-	[`traefik:v2.1.3`](#traefikv213)
-	[`traefik:v2.1.3-windowsservercore-1809`](#traefikv213-windowsservercore-1809)
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
$ docker pull traefik@sha256:5545c7138c85b3bc5ad0b8775ee168ae16c839bddbe83b4af20a1660a4dde29c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.973; amd64

### `traefik:1.7.20-windowsservercore-1809` - windows version 10.0.17763.973; amd64

```console
$ docker pull traefik@sha256:6cfb866dc049dc285053e1f6a51226552c66627ae5af596fef51d5816d0095a4
```

-	Docker Version: 18.03.1-ee-4
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.2 GB (2245517816 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8717289fcbe162ad339e623185f4cb3fde105c3346a906b3d9e45e58d582b94c`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 15 Sep 2018 09:10:26 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 11 Jan 2020 05:23:25 GMT
RUN Install update 1809-amd64
# Tue, 14 Jan 2020 23:46:02 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 15 Jan 2020 22:25:10 GMT
RUN Invoke-WebRequest     -Uri "https://github.com/containous/traefik/releases/download/v1.7.20/traefik_windows-amd64.exe"     -OutFile "/traefik.exe"
# Wed, 15 Jan 2020 22:25:14 GMT
EXPOSE 80
# Wed, 15 Jan 2020 22:25:16 GMT
ENTRYPOINT ["/traefik"]
# Wed, 15 Jan 2020 22:25:17 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.20 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:65014b3c312172f10bd6701a063f9b5aaf9a916c2d2cb843d406a6f77ded3f8d`  
		Last Modified: Tue, 13 Nov 2018 18:50:17 GMT  
		Size: 1.5 GB (1534685324 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:edbd72df76b46e904108d2f61a63c295b3e3d8092dbd5a03bbeb2fb4d34a3e55`  
		Size: 682.7 MB (682725872 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e9d323e253cb21832421dda4ec57dbd597bd4f934e62c162b9dec8b96e06e818`  
		Last Modified: Wed, 15 Jan 2020 01:45:20 GMT  
		Size: 1.2 KB (1193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa553b540bc891379b327f7ebaf07fc18540471d50ab5ee933ac25c388bbd599`  
		Last Modified: Wed, 15 Jan 2020 22:27:30 GMT  
		Size: 28.1 MB (28101873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a2a7f9ea7b7d37ae92c7d35e40837cf30a6fb9e06234933ef771963f08e1b5d`  
		Last Modified: Wed, 15 Jan 2020 22:27:23 GMT  
		Size: 1.2 KB (1184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96835f334cd72d34b10c788e7adf2692a9038c2e79e936ff84d1136d3e2ed8e5`  
		Last Modified: Wed, 15 Jan 2020 22:27:23 GMT  
		Size: 1.2 KB (1183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c384663a41950e20d89986102e168d0afd30f4b754869dbcf6a7e1a4d99a9d73`  
		Last Modified: Wed, 15 Jan 2020 22:27:23 GMT  
		Size: 1.2 KB (1187 bytes)  
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
$ docker pull traefik@sha256:5545c7138c85b3bc5ad0b8775ee168ae16c839bddbe83b4af20a1660a4dde29c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.973; amd64

### `traefik:1.7-windowsservercore-1809` - windows version 10.0.17763.973; amd64

```console
$ docker pull traefik@sha256:6cfb866dc049dc285053e1f6a51226552c66627ae5af596fef51d5816d0095a4
```

-	Docker Version: 18.03.1-ee-4
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.2 GB (2245517816 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8717289fcbe162ad339e623185f4cb3fde105c3346a906b3d9e45e58d582b94c`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 15 Sep 2018 09:10:26 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 11 Jan 2020 05:23:25 GMT
RUN Install update 1809-amd64
# Tue, 14 Jan 2020 23:46:02 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 15 Jan 2020 22:25:10 GMT
RUN Invoke-WebRequest     -Uri "https://github.com/containous/traefik/releases/download/v1.7.20/traefik_windows-amd64.exe"     -OutFile "/traefik.exe"
# Wed, 15 Jan 2020 22:25:14 GMT
EXPOSE 80
# Wed, 15 Jan 2020 22:25:16 GMT
ENTRYPOINT ["/traefik"]
# Wed, 15 Jan 2020 22:25:17 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.20 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:65014b3c312172f10bd6701a063f9b5aaf9a916c2d2cb843d406a6f77ded3f8d`  
		Last Modified: Tue, 13 Nov 2018 18:50:17 GMT  
		Size: 1.5 GB (1534685324 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:edbd72df76b46e904108d2f61a63c295b3e3d8092dbd5a03bbeb2fb4d34a3e55`  
		Size: 682.7 MB (682725872 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e9d323e253cb21832421dda4ec57dbd597bd4f934e62c162b9dec8b96e06e818`  
		Last Modified: Wed, 15 Jan 2020 01:45:20 GMT  
		Size: 1.2 KB (1193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa553b540bc891379b327f7ebaf07fc18540471d50ab5ee933ac25c388bbd599`  
		Last Modified: Wed, 15 Jan 2020 22:27:30 GMT  
		Size: 28.1 MB (28101873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a2a7f9ea7b7d37ae92c7d35e40837cf30a6fb9e06234933ef771963f08e1b5d`  
		Last Modified: Wed, 15 Jan 2020 22:27:23 GMT  
		Size: 1.2 KB (1184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96835f334cd72d34b10c788e7adf2692a9038c2e79e936ff84d1136d3e2ed8e5`  
		Last Modified: Wed, 15 Jan 2020 22:27:23 GMT  
		Size: 1.2 KB (1183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c384663a41950e20d89986102e168d0afd30f4b754869dbcf6a7e1a4d99a9d73`  
		Last Modified: Wed, 15 Jan 2020 22:27:23 GMT  
		Size: 1.2 KB (1187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:2.1`

```console
$ docker pull traefik@sha256:23f6057ef7b2ed7d8a36f64383c83d1639d3702d4dc8956f91b3dccc5ee9aad7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:2.1` - linux; amd64

```console
$ docker pull traefik@sha256:b45214fe976f562a2960b31d651937ff0b38096a5e190aa054ccd0d731c6999f
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.0 MB (22999258 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:49e31b6f8f937b27a5035b3783f83fdca1ed7461c8c95bfcc5b5bc437ade4edb`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Mon, 21 Oct 2019 17:21:42 GMT
ADD file:fe1f09249227e2da2089afb4d07e16cbf832eeb804120074acd2b8192876cd28 in / 
# Mon, 21 Oct 2019 17:21:42 GMT
CMD ["/bin/sh"]
# Mon, 21 Oct 2019 22:26:21 GMT
RUN apk --no-cache add ca-certificates tzdata
# Tue, 07 Jan 2020 23:34:39 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/containous/traefik/releases/download/v2.1.2/traefik_v2.1.2_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Tue, 07 Jan 2020 23:34:40 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Tue, 07 Jan 2020 23:34:40 GMT
EXPOSE 80
# Tue, 07 Jan 2020 23:34:40 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 07 Jan 2020 23:34:40 GMT
CMD ["traefik"]
# Tue, 07 Jan 2020 23:34:40 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.1.2 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:1cbc3b9baf4c49487508fd44bf1365ad4ebb49dab85b703c52a6fff23a478411`  
		Last Modified: Tue, 07 Jan 2020 23:35:06 GMT  
		Size: 19.5 MB (19517263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f62bc7f11c0b379c7d64a75606196ef30e8ca8ea737fa128f9a7ed7ce02d788`  
		Last Modified: Tue, 07 Jan 2020 23:35:02 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:2.1` - linux; arm variant v6

```console
$ docker pull traefik@sha256:c8f068acf02c01eceac2d851e98312a29c9f0b3fa2d45e259004e869c6e5f9e3
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **21.5 MB (21545654 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7b142df1d3f6cc564cf4ef889e8dbf1811f5a8c51d8f46ef73a1be8cc9bc8ad1`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Mon, 21 Oct 2019 16:56:02 GMT
ADD file:d3c7d938a78143f106a6a467ce23b599198e041220e661e5326ba91054c353ef in / 
# Mon, 21 Oct 2019 16:56:04 GMT
CMD ["/bin/sh"]
# Mon, 21 Oct 2019 20:27:15 GMT
RUN apk --no-cache add ca-certificates tzdata
# Tue, 07 Jan 2020 23:49:53 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/containous/traefik/releases/download/v2.1.2/traefik_v2.1.2_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Tue, 07 Jan 2020 23:49:54 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Tue, 07 Jan 2020 23:49:54 GMT
EXPOSE 80
# Tue, 07 Jan 2020 23:49:55 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 07 Jan 2020 23:49:55 GMT
CMD ["traefik"]
# Tue, 07 Jan 2020 23:49:56 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.1.2 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:a917af9418ba8cc1c6b3c2191603a36a2f1598f152835cda15e8e8f771189a2c`  
		Last Modified: Tue, 07 Jan 2020 23:51:16 GMT  
		Size: 18.3 MB (18276155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddd2532cf514fb1b82a3d6e0271ab806850c0c29b66e907f63d0d2acdedb459e`  
		Last Modified: Tue, 07 Jan 2020 23:51:09 GMT  
		Size: 369.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:2.1` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:29020ac8a9755056ea88c62295309cdaaa70c501d8a4976a9f8fc3f681013772
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **21.4 MB (21385632 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:316c3218c99d7a75e5611663f6f40751d942841d76397db294e3df7b4451f862`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Mon, 21 Oct 2019 18:07:03 GMT
ADD file:02f4d68afd9e9e303ff893f198d535d0d78c4b2554f299ab2d0955b2bef0e06a in / 
# Mon, 21 Oct 2019 18:07:09 GMT
CMD ["/bin/sh"]
# Mon, 21 Oct 2019 23:22:16 GMT
RUN apk --no-cache add ca-certificates tzdata
# Tue, 07 Jan 2020 23:40:23 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/containous/traefik/releases/download/v2.1.2/traefik_v2.1.2_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Tue, 07 Jan 2020 23:40:23 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Tue, 07 Jan 2020 23:40:24 GMT
EXPOSE 80
# Tue, 07 Jan 2020 23:40:25 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 07 Jan 2020 23:40:26 GMT
CMD ["traefik"]
# Tue, 07 Jan 2020 23:40:27 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.1.2 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:ed887cf3053eaa75acdc147a65a7dac09ad15b00761c6c934c452e2fd53da1f7`  
		Last Modified: Tue, 07 Jan 2020 23:41:05 GMT  
		Size: 18.0 MB (17969598 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27979fd681cee9441e39782cd83d3b0483c72a311d58b9f3b31e3ba717634b88`  
		Last Modified: Tue, 07 Jan 2020 23:40:59 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:2.1.3`

```console
$ docker pull traefik@sha256:a8409dff6597f2ef5f7ecd3c672671bb2af9a390073efd74f95c54aa41cba22a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:

## `traefik:2.1.3-windowsservercore-1809`

```console
$ docker pull traefik@sha256:a8409dff6597f2ef5f7ecd3c672671bb2af9a390073efd74f95c54aa41cba22a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:

## `traefik:2.1-windowsservercore-1809`

```console
$ docker pull traefik@sha256:aa59d49fa49fa83d7391fd66f1481babbbd88bd2282a10da3d0ce61046b43435
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.973; amd64

### `traefik:2.1-windowsservercore-1809` - windows version 10.0.17763.973; amd64

```console
$ docker pull traefik@sha256:24fb3a85df17b58602c1416b6453dd805f09a62e0a9c95e9f0eb0947f24ec4da
```

-	Docker Version: 18.03.1-ee-4
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.2 GB (2241472045 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:43ed286fa68808142212fdc36793359b2b0a9dca8f560a9974da6c86f1b8d1c4`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 15 Sep 2018 09:10:26 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 11 Jan 2020 05:23:25 GMT
RUN Install update 1809-amd64
# Tue, 14 Jan 2020 23:46:02 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 15 Jan 2020 22:23:59 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/containous/traefik/releases/download/v2.1.2/traefik_v2.1.2_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Wed, 15 Jan 2020 22:24:03 GMT
EXPOSE 80
# Wed, 15 Jan 2020 22:24:04 GMT
ENTRYPOINT ["/traefik"]
# Wed, 15 Jan 2020 22:24:06 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.1.2 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:65014b3c312172f10bd6701a063f9b5aaf9a916c2d2cb843d406a6f77ded3f8d`  
		Last Modified: Tue, 13 Nov 2018 18:50:17 GMT  
		Size: 1.5 GB (1534685324 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:edbd72df76b46e904108d2f61a63c295b3e3d8092dbd5a03bbeb2fb4d34a3e55`  
		Size: 682.7 MB (682725872 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e9d323e253cb21832421dda4ec57dbd597bd4f934e62c162b9dec8b96e06e818`  
		Last Modified: Wed, 15 Jan 2020 01:45:20 GMT  
		Size: 1.2 KB (1193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:925f59c295b5302641a4009f899086f273c0f7ae66604422c30b9cda5f334094`  
		Last Modified: Wed, 15 Jan 2020 22:26:25 GMT  
		Size: 24.1 MB (24056072 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5d394b8b9b33f0860352480d9867cf1d5f765ee8411e3452db10d62b595fd22`  
		Last Modified: Wed, 15 Jan 2020 22:26:00 GMT  
		Size: 1.2 KB (1208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:057e7d4d86fd9c71a4c24e4936055f48c8855639f3b5e4a09b84cb34ff07c435`  
		Last Modified: Wed, 15 Jan 2020 22:26:01 GMT  
		Size: 1.2 KB (1187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33754414b9289672384e99a88abefcbbe951b5ee9d26e7f1b6be260214e0b438`  
		Last Modified: Wed, 15 Jan 2020 22:26:00 GMT  
		Size: 1.2 KB (1189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:cantal`

```console
$ docker pull traefik@sha256:23f6057ef7b2ed7d8a36f64383c83d1639d3702d4dc8956f91b3dccc5ee9aad7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:cantal` - linux; amd64

```console
$ docker pull traefik@sha256:b45214fe976f562a2960b31d651937ff0b38096a5e190aa054ccd0d731c6999f
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.0 MB (22999258 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:49e31b6f8f937b27a5035b3783f83fdca1ed7461c8c95bfcc5b5bc437ade4edb`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Mon, 21 Oct 2019 17:21:42 GMT
ADD file:fe1f09249227e2da2089afb4d07e16cbf832eeb804120074acd2b8192876cd28 in / 
# Mon, 21 Oct 2019 17:21:42 GMT
CMD ["/bin/sh"]
# Mon, 21 Oct 2019 22:26:21 GMT
RUN apk --no-cache add ca-certificates tzdata
# Tue, 07 Jan 2020 23:34:39 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/containous/traefik/releases/download/v2.1.2/traefik_v2.1.2_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Tue, 07 Jan 2020 23:34:40 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Tue, 07 Jan 2020 23:34:40 GMT
EXPOSE 80
# Tue, 07 Jan 2020 23:34:40 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 07 Jan 2020 23:34:40 GMT
CMD ["traefik"]
# Tue, 07 Jan 2020 23:34:40 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.1.2 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:1cbc3b9baf4c49487508fd44bf1365ad4ebb49dab85b703c52a6fff23a478411`  
		Last Modified: Tue, 07 Jan 2020 23:35:06 GMT  
		Size: 19.5 MB (19517263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f62bc7f11c0b379c7d64a75606196ef30e8ca8ea737fa128f9a7ed7ce02d788`  
		Last Modified: Tue, 07 Jan 2020 23:35:02 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:cantal` - linux; arm variant v6

```console
$ docker pull traefik@sha256:c8f068acf02c01eceac2d851e98312a29c9f0b3fa2d45e259004e869c6e5f9e3
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **21.5 MB (21545654 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7b142df1d3f6cc564cf4ef889e8dbf1811f5a8c51d8f46ef73a1be8cc9bc8ad1`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Mon, 21 Oct 2019 16:56:02 GMT
ADD file:d3c7d938a78143f106a6a467ce23b599198e041220e661e5326ba91054c353ef in / 
# Mon, 21 Oct 2019 16:56:04 GMT
CMD ["/bin/sh"]
# Mon, 21 Oct 2019 20:27:15 GMT
RUN apk --no-cache add ca-certificates tzdata
# Tue, 07 Jan 2020 23:49:53 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/containous/traefik/releases/download/v2.1.2/traefik_v2.1.2_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Tue, 07 Jan 2020 23:49:54 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Tue, 07 Jan 2020 23:49:54 GMT
EXPOSE 80
# Tue, 07 Jan 2020 23:49:55 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 07 Jan 2020 23:49:55 GMT
CMD ["traefik"]
# Tue, 07 Jan 2020 23:49:56 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.1.2 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:a917af9418ba8cc1c6b3c2191603a36a2f1598f152835cda15e8e8f771189a2c`  
		Last Modified: Tue, 07 Jan 2020 23:51:16 GMT  
		Size: 18.3 MB (18276155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddd2532cf514fb1b82a3d6e0271ab806850c0c29b66e907f63d0d2acdedb459e`  
		Last Modified: Tue, 07 Jan 2020 23:51:09 GMT  
		Size: 369.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:cantal` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:29020ac8a9755056ea88c62295309cdaaa70c501d8a4976a9f8fc3f681013772
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **21.4 MB (21385632 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:316c3218c99d7a75e5611663f6f40751d942841d76397db294e3df7b4451f862`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Mon, 21 Oct 2019 18:07:03 GMT
ADD file:02f4d68afd9e9e303ff893f198d535d0d78c4b2554f299ab2d0955b2bef0e06a in / 
# Mon, 21 Oct 2019 18:07:09 GMT
CMD ["/bin/sh"]
# Mon, 21 Oct 2019 23:22:16 GMT
RUN apk --no-cache add ca-certificates tzdata
# Tue, 07 Jan 2020 23:40:23 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/containous/traefik/releases/download/v2.1.2/traefik_v2.1.2_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Tue, 07 Jan 2020 23:40:23 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Tue, 07 Jan 2020 23:40:24 GMT
EXPOSE 80
# Tue, 07 Jan 2020 23:40:25 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 07 Jan 2020 23:40:26 GMT
CMD ["traefik"]
# Tue, 07 Jan 2020 23:40:27 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.1.2 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:ed887cf3053eaa75acdc147a65a7dac09ad15b00761c6c934c452e2fd53da1f7`  
		Last Modified: Tue, 07 Jan 2020 23:41:05 GMT  
		Size: 18.0 MB (17969598 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27979fd681cee9441e39782cd83d3b0483c72a311d58b9f3b31e3ba717634b88`  
		Last Modified: Tue, 07 Jan 2020 23:40:59 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:cantal-windowsservercore-1809`

```console
$ docker pull traefik@sha256:aa59d49fa49fa83d7391fd66f1481babbbd88bd2282a10da3d0ce61046b43435
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.973; amd64

### `traefik:cantal-windowsservercore-1809` - windows version 10.0.17763.973; amd64

```console
$ docker pull traefik@sha256:24fb3a85df17b58602c1416b6453dd805f09a62e0a9c95e9f0eb0947f24ec4da
```

-	Docker Version: 18.03.1-ee-4
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.2 GB (2241472045 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:43ed286fa68808142212fdc36793359b2b0a9dca8f560a9974da6c86f1b8d1c4`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 15 Sep 2018 09:10:26 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 11 Jan 2020 05:23:25 GMT
RUN Install update 1809-amd64
# Tue, 14 Jan 2020 23:46:02 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 15 Jan 2020 22:23:59 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/containous/traefik/releases/download/v2.1.2/traefik_v2.1.2_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Wed, 15 Jan 2020 22:24:03 GMT
EXPOSE 80
# Wed, 15 Jan 2020 22:24:04 GMT
ENTRYPOINT ["/traefik"]
# Wed, 15 Jan 2020 22:24:06 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.1.2 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:65014b3c312172f10bd6701a063f9b5aaf9a916c2d2cb843d406a6f77ded3f8d`  
		Last Modified: Tue, 13 Nov 2018 18:50:17 GMT  
		Size: 1.5 GB (1534685324 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:edbd72df76b46e904108d2f61a63c295b3e3d8092dbd5a03bbeb2fb4d34a3e55`  
		Size: 682.7 MB (682725872 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e9d323e253cb21832421dda4ec57dbd597bd4f934e62c162b9dec8b96e06e818`  
		Last Modified: Wed, 15 Jan 2020 01:45:20 GMT  
		Size: 1.2 KB (1193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:925f59c295b5302641a4009f899086f273c0f7ae66604422c30b9cda5f334094`  
		Last Modified: Wed, 15 Jan 2020 22:26:25 GMT  
		Size: 24.1 MB (24056072 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5d394b8b9b33f0860352480d9867cf1d5f765ee8411e3452db10d62b595fd22`  
		Last Modified: Wed, 15 Jan 2020 22:26:00 GMT  
		Size: 1.2 KB (1208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:057e7d4d86fd9c71a4c24e4936055f48c8855639f3b5e4a09b84cb34ff07c435`  
		Last Modified: Wed, 15 Jan 2020 22:26:01 GMT  
		Size: 1.2 KB (1187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33754414b9289672384e99a88abefcbbe951b5ee9d26e7f1b6be260214e0b438`  
		Last Modified: Wed, 15 Jan 2020 22:26:00 GMT  
		Size: 1.2 KB (1189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:latest`

```console
$ docker pull traefik@sha256:23f6057ef7b2ed7d8a36f64383c83d1639d3702d4dc8956f91b3dccc5ee9aad7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:latest` - linux; amd64

```console
$ docker pull traefik@sha256:b45214fe976f562a2960b31d651937ff0b38096a5e190aa054ccd0d731c6999f
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.0 MB (22999258 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:49e31b6f8f937b27a5035b3783f83fdca1ed7461c8c95bfcc5b5bc437ade4edb`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Mon, 21 Oct 2019 17:21:42 GMT
ADD file:fe1f09249227e2da2089afb4d07e16cbf832eeb804120074acd2b8192876cd28 in / 
# Mon, 21 Oct 2019 17:21:42 GMT
CMD ["/bin/sh"]
# Mon, 21 Oct 2019 22:26:21 GMT
RUN apk --no-cache add ca-certificates tzdata
# Tue, 07 Jan 2020 23:34:39 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/containous/traefik/releases/download/v2.1.2/traefik_v2.1.2_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Tue, 07 Jan 2020 23:34:40 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Tue, 07 Jan 2020 23:34:40 GMT
EXPOSE 80
# Tue, 07 Jan 2020 23:34:40 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 07 Jan 2020 23:34:40 GMT
CMD ["traefik"]
# Tue, 07 Jan 2020 23:34:40 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.1.2 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:1cbc3b9baf4c49487508fd44bf1365ad4ebb49dab85b703c52a6fff23a478411`  
		Last Modified: Tue, 07 Jan 2020 23:35:06 GMT  
		Size: 19.5 MB (19517263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f62bc7f11c0b379c7d64a75606196ef30e8ca8ea737fa128f9a7ed7ce02d788`  
		Last Modified: Tue, 07 Jan 2020 23:35:02 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:latest` - linux; arm variant v6

```console
$ docker pull traefik@sha256:c8f068acf02c01eceac2d851e98312a29c9f0b3fa2d45e259004e869c6e5f9e3
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **21.5 MB (21545654 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7b142df1d3f6cc564cf4ef889e8dbf1811f5a8c51d8f46ef73a1be8cc9bc8ad1`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Mon, 21 Oct 2019 16:56:02 GMT
ADD file:d3c7d938a78143f106a6a467ce23b599198e041220e661e5326ba91054c353ef in / 
# Mon, 21 Oct 2019 16:56:04 GMT
CMD ["/bin/sh"]
# Mon, 21 Oct 2019 20:27:15 GMT
RUN apk --no-cache add ca-certificates tzdata
# Tue, 07 Jan 2020 23:49:53 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/containous/traefik/releases/download/v2.1.2/traefik_v2.1.2_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Tue, 07 Jan 2020 23:49:54 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Tue, 07 Jan 2020 23:49:54 GMT
EXPOSE 80
# Tue, 07 Jan 2020 23:49:55 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 07 Jan 2020 23:49:55 GMT
CMD ["traefik"]
# Tue, 07 Jan 2020 23:49:56 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.1.2 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:a917af9418ba8cc1c6b3c2191603a36a2f1598f152835cda15e8e8f771189a2c`  
		Last Modified: Tue, 07 Jan 2020 23:51:16 GMT  
		Size: 18.3 MB (18276155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddd2532cf514fb1b82a3d6e0271ab806850c0c29b66e907f63d0d2acdedb459e`  
		Last Modified: Tue, 07 Jan 2020 23:51:09 GMT  
		Size: 369.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:latest` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:29020ac8a9755056ea88c62295309cdaaa70c501d8a4976a9f8fc3f681013772
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **21.4 MB (21385632 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:316c3218c99d7a75e5611663f6f40751d942841d76397db294e3df7b4451f862`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Mon, 21 Oct 2019 18:07:03 GMT
ADD file:02f4d68afd9e9e303ff893f198d535d0d78c4b2554f299ab2d0955b2bef0e06a in / 
# Mon, 21 Oct 2019 18:07:09 GMT
CMD ["/bin/sh"]
# Mon, 21 Oct 2019 23:22:16 GMT
RUN apk --no-cache add ca-certificates tzdata
# Tue, 07 Jan 2020 23:40:23 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/containous/traefik/releases/download/v2.1.2/traefik_v2.1.2_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Tue, 07 Jan 2020 23:40:23 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Tue, 07 Jan 2020 23:40:24 GMT
EXPOSE 80
# Tue, 07 Jan 2020 23:40:25 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 07 Jan 2020 23:40:26 GMT
CMD ["traefik"]
# Tue, 07 Jan 2020 23:40:27 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.1.2 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:ed887cf3053eaa75acdc147a65a7dac09ad15b00761c6c934c452e2fd53da1f7`  
		Last Modified: Tue, 07 Jan 2020 23:41:05 GMT  
		Size: 18.0 MB (17969598 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27979fd681cee9441e39782cd83d3b0483c72a311d58b9f3b31e3ba717634b88`  
		Last Modified: Tue, 07 Jan 2020 23:40:59 GMT  
		Size: 368.0 B  
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
$ docker pull traefik@sha256:5545c7138c85b3bc5ad0b8775ee168ae16c839bddbe83b4af20a1660a4dde29c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.973; amd64

### `traefik:maroilles-windowsservercore-1809` - windows version 10.0.17763.973; amd64

```console
$ docker pull traefik@sha256:6cfb866dc049dc285053e1f6a51226552c66627ae5af596fef51d5816d0095a4
```

-	Docker Version: 18.03.1-ee-4
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.2 GB (2245517816 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8717289fcbe162ad339e623185f4cb3fde105c3346a906b3d9e45e58d582b94c`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 15 Sep 2018 09:10:26 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 11 Jan 2020 05:23:25 GMT
RUN Install update 1809-amd64
# Tue, 14 Jan 2020 23:46:02 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 15 Jan 2020 22:25:10 GMT
RUN Invoke-WebRequest     -Uri "https://github.com/containous/traefik/releases/download/v1.7.20/traefik_windows-amd64.exe"     -OutFile "/traefik.exe"
# Wed, 15 Jan 2020 22:25:14 GMT
EXPOSE 80
# Wed, 15 Jan 2020 22:25:16 GMT
ENTRYPOINT ["/traefik"]
# Wed, 15 Jan 2020 22:25:17 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.20 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:65014b3c312172f10bd6701a063f9b5aaf9a916c2d2cb843d406a6f77ded3f8d`  
		Last Modified: Tue, 13 Nov 2018 18:50:17 GMT  
		Size: 1.5 GB (1534685324 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:edbd72df76b46e904108d2f61a63c295b3e3d8092dbd5a03bbeb2fb4d34a3e55`  
		Size: 682.7 MB (682725872 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e9d323e253cb21832421dda4ec57dbd597bd4f934e62c162b9dec8b96e06e818`  
		Last Modified: Wed, 15 Jan 2020 01:45:20 GMT  
		Size: 1.2 KB (1193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa553b540bc891379b327f7ebaf07fc18540471d50ab5ee933ac25c388bbd599`  
		Last Modified: Wed, 15 Jan 2020 22:27:30 GMT  
		Size: 28.1 MB (28101873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a2a7f9ea7b7d37ae92c7d35e40837cf30a6fb9e06234933ef771963f08e1b5d`  
		Last Modified: Wed, 15 Jan 2020 22:27:23 GMT  
		Size: 1.2 KB (1184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96835f334cd72d34b10c788e7adf2692a9038c2e79e936ff84d1136d3e2ed8e5`  
		Last Modified: Wed, 15 Jan 2020 22:27:23 GMT  
		Size: 1.2 KB (1183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c384663a41950e20d89986102e168d0afd30f4b754869dbcf6a7e1a4d99a9d73`  
		Last Modified: Wed, 15 Jan 2020 22:27:23 GMT  
		Size: 1.2 KB (1187 bytes)  
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
$ docker pull traefik@sha256:5545c7138c85b3bc5ad0b8775ee168ae16c839bddbe83b4af20a1660a4dde29c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.973; amd64

### `traefik:v1.7.20-windowsservercore-1809` - windows version 10.0.17763.973; amd64

```console
$ docker pull traefik@sha256:6cfb866dc049dc285053e1f6a51226552c66627ae5af596fef51d5816d0095a4
```

-	Docker Version: 18.03.1-ee-4
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.2 GB (2245517816 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8717289fcbe162ad339e623185f4cb3fde105c3346a906b3d9e45e58d582b94c`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 15 Sep 2018 09:10:26 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 11 Jan 2020 05:23:25 GMT
RUN Install update 1809-amd64
# Tue, 14 Jan 2020 23:46:02 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 15 Jan 2020 22:25:10 GMT
RUN Invoke-WebRequest     -Uri "https://github.com/containous/traefik/releases/download/v1.7.20/traefik_windows-amd64.exe"     -OutFile "/traefik.exe"
# Wed, 15 Jan 2020 22:25:14 GMT
EXPOSE 80
# Wed, 15 Jan 2020 22:25:16 GMT
ENTRYPOINT ["/traefik"]
# Wed, 15 Jan 2020 22:25:17 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.20 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:65014b3c312172f10bd6701a063f9b5aaf9a916c2d2cb843d406a6f77ded3f8d`  
		Last Modified: Tue, 13 Nov 2018 18:50:17 GMT  
		Size: 1.5 GB (1534685324 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:edbd72df76b46e904108d2f61a63c295b3e3d8092dbd5a03bbeb2fb4d34a3e55`  
		Size: 682.7 MB (682725872 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e9d323e253cb21832421dda4ec57dbd597bd4f934e62c162b9dec8b96e06e818`  
		Last Modified: Wed, 15 Jan 2020 01:45:20 GMT  
		Size: 1.2 KB (1193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa553b540bc891379b327f7ebaf07fc18540471d50ab5ee933ac25c388bbd599`  
		Last Modified: Wed, 15 Jan 2020 22:27:30 GMT  
		Size: 28.1 MB (28101873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a2a7f9ea7b7d37ae92c7d35e40837cf30a6fb9e06234933ef771963f08e1b5d`  
		Last Modified: Wed, 15 Jan 2020 22:27:23 GMT  
		Size: 1.2 KB (1184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96835f334cd72d34b10c788e7adf2692a9038c2e79e936ff84d1136d3e2ed8e5`  
		Last Modified: Wed, 15 Jan 2020 22:27:23 GMT  
		Size: 1.2 KB (1183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c384663a41950e20d89986102e168d0afd30f4b754869dbcf6a7e1a4d99a9d73`  
		Last Modified: Wed, 15 Jan 2020 22:27:23 GMT  
		Size: 1.2 KB (1187 bytes)  
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
$ docker pull traefik@sha256:5545c7138c85b3bc5ad0b8775ee168ae16c839bddbe83b4af20a1660a4dde29c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.973; amd64

### `traefik:v1.7-windowsservercore-1809` - windows version 10.0.17763.973; amd64

```console
$ docker pull traefik@sha256:6cfb866dc049dc285053e1f6a51226552c66627ae5af596fef51d5816d0095a4
```

-	Docker Version: 18.03.1-ee-4
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.2 GB (2245517816 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8717289fcbe162ad339e623185f4cb3fde105c3346a906b3d9e45e58d582b94c`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 15 Sep 2018 09:10:26 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 11 Jan 2020 05:23:25 GMT
RUN Install update 1809-amd64
# Tue, 14 Jan 2020 23:46:02 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 15 Jan 2020 22:25:10 GMT
RUN Invoke-WebRequest     -Uri "https://github.com/containous/traefik/releases/download/v1.7.20/traefik_windows-amd64.exe"     -OutFile "/traefik.exe"
# Wed, 15 Jan 2020 22:25:14 GMT
EXPOSE 80
# Wed, 15 Jan 2020 22:25:16 GMT
ENTRYPOINT ["/traefik"]
# Wed, 15 Jan 2020 22:25:17 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.20 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:65014b3c312172f10bd6701a063f9b5aaf9a916c2d2cb843d406a6f77ded3f8d`  
		Last Modified: Tue, 13 Nov 2018 18:50:17 GMT  
		Size: 1.5 GB (1534685324 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:edbd72df76b46e904108d2f61a63c295b3e3d8092dbd5a03bbeb2fb4d34a3e55`  
		Size: 682.7 MB (682725872 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e9d323e253cb21832421dda4ec57dbd597bd4f934e62c162b9dec8b96e06e818`  
		Last Modified: Wed, 15 Jan 2020 01:45:20 GMT  
		Size: 1.2 KB (1193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa553b540bc891379b327f7ebaf07fc18540471d50ab5ee933ac25c388bbd599`  
		Last Modified: Wed, 15 Jan 2020 22:27:30 GMT  
		Size: 28.1 MB (28101873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a2a7f9ea7b7d37ae92c7d35e40837cf30a6fb9e06234933ef771963f08e1b5d`  
		Last Modified: Wed, 15 Jan 2020 22:27:23 GMT  
		Size: 1.2 KB (1184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96835f334cd72d34b10c788e7adf2692a9038c2e79e936ff84d1136d3e2ed8e5`  
		Last Modified: Wed, 15 Jan 2020 22:27:23 GMT  
		Size: 1.2 KB (1183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c384663a41950e20d89986102e168d0afd30f4b754869dbcf6a7e1a4d99a9d73`  
		Last Modified: Wed, 15 Jan 2020 22:27:23 GMT  
		Size: 1.2 KB (1187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v2.1`

```console
$ docker pull traefik@sha256:23f6057ef7b2ed7d8a36f64383c83d1639d3702d4dc8956f91b3dccc5ee9aad7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:v2.1` - linux; amd64

```console
$ docker pull traefik@sha256:b45214fe976f562a2960b31d651937ff0b38096a5e190aa054ccd0d731c6999f
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.0 MB (22999258 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:49e31b6f8f937b27a5035b3783f83fdca1ed7461c8c95bfcc5b5bc437ade4edb`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Mon, 21 Oct 2019 17:21:42 GMT
ADD file:fe1f09249227e2da2089afb4d07e16cbf832eeb804120074acd2b8192876cd28 in / 
# Mon, 21 Oct 2019 17:21:42 GMT
CMD ["/bin/sh"]
# Mon, 21 Oct 2019 22:26:21 GMT
RUN apk --no-cache add ca-certificates tzdata
# Tue, 07 Jan 2020 23:34:39 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/containous/traefik/releases/download/v2.1.2/traefik_v2.1.2_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Tue, 07 Jan 2020 23:34:40 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Tue, 07 Jan 2020 23:34:40 GMT
EXPOSE 80
# Tue, 07 Jan 2020 23:34:40 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 07 Jan 2020 23:34:40 GMT
CMD ["traefik"]
# Tue, 07 Jan 2020 23:34:40 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.1.2 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:1cbc3b9baf4c49487508fd44bf1365ad4ebb49dab85b703c52a6fff23a478411`  
		Last Modified: Tue, 07 Jan 2020 23:35:06 GMT  
		Size: 19.5 MB (19517263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f62bc7f11c0b379c7d64a75606196ef30e8ca8ea737fa128f9a7ed7ce02d788`  
		Last Modified: Tue, 07 Jan 2020 23:35:02 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v2.1` - linux; arm variant v6

```console
$ docker pull traefik@sha256:c8f068acf02c01eceac2d851e98312a29c9f0b3fa2d45e259004e869c6e5f9e3
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **21.5 MB (21545654 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7b142df1d3f6cc564cf4ef889e8dbf1811f5a8c51d8f46ef73a1be8cc9bc8ad1`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Mon, 21 Oct 2019 16:56:02 GMT
ADD file:d3c7d938a78143f106a6a467ce23b599198e041220e661e5326ba91054c353ef in / 
# Mon, 21 Oct 2019 16:56:04 GMT
CMD ["/bin/sh"]
# Mon, 21 Oct 2019 20:27:15 GMT
RUN apk --no-cache add ca-certificates tzdata
# Tue, 07 Jan 2020 23:49:53 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/containous/traefik/releases/download/v2.1.2/traefik_v2.1.2_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Tue, 07 Jan 2020 23:49:54 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Tue, 07 Jan 2020 23:49:54 GMT
EXPOSE 80
# Tue, 07 Jan 2020 23:49:55 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 07 Jan 2020 23:49:55 GMT
CMD ["traefik"]
# Tue, 07 Jan 2020 23:49:56 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.1.2 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:a917af9418ba8cc1c6b3c2191603a36a2f1598f152835cda15e8e8f771189a2c`  
		Last Modified: Tue, 07 Jan 2020 23:51:16 GMT  
		Size: 18.3 MB (18276155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddd2532cf514fb1b82a3d6e0271ab806850c0c29b66e907f63d0d2acdedb459e`  
		Last Modified: Tue, 07 Jan 2020 23:51:09 GMT  
		Size: 369.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v2.1` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:29020ac8a9755056ea88c62295309cdaaa70c501d8a4976a9f8fc3f681013772
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **21.4 MB (21385632 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:316c3218c99d7a75e5611663f6f40751d942841d76397db294e3df7b4451f862`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Mon, 21 Oct 2019 18:07:03 GMT
ADD file:02f4d68afd9e9e303ff893f198d535d0d78c4b2554f299ab2d0955b2bef0e06a in / 
# Mon, 21 Oct 2019 18:07:09 GMT
CMD ["/bin/sh"]
# Mon, 21 Oct 2019 23:22:16 GMT
RUN apk --no-cache add ca-certificates tzdata
# Tue, 07 Jan 2020 23:40:23 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/containous/traefik/releases/download/v2.1.2/traefik_v2.1.2_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Tue, 07 Jan 2020 23:40:23 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Tue, 07 Jan 2020 23:40:24 GMT
EXPOSE 80
# Tue, 07 Jan 2020 23:40:25 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 07 Jan 2020 23:40:26 GMT
CMD ["traefik"]
# Tue, 07 Jan 2020 23:40:27 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.1.2 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:ed887cf3053eaa75acdc147a65a7dac09ad15b00761c6c934c452e2fd53da1f7`  
		Last Modified: Tue, 07 Jan 2020 23:41:05 GMT  
		Size: 18.0 MB (17969598 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27979fd681cee9441e39782cd83d3b0483c72a311d58b9f3b31e3ba717634b88`  
		Last Modified: Tue, 07 Jan 2020 23:40:59 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v2.1.3`

```console
$ docker pull traefik@sha256:a8409dff6597f2ef5f7ecd3c672671bb2af9a390073efd74f95c54aa41cba22a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:

## `traefik:v2.1.3-windowsservercore-1809`

```console
$ docker pull traefik@sha256:a8409dff6597f2ef5f7ecd3c672671bb2af9a390073efd74f95c54aa41cba22a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:

## `traefik:v2.1-windowsservercore-1809`

```console
$ docker pull traefik@sha256:aa59d49fa49fa83d7391fd66f1481babbbd88bd2282a10da3d0ce61046b43435
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.973; amd64

### `traefik:v2.1-windowsservercore-1809` - windows version 10.0.17763.973; amd64

```console
$ docker pull traefik@sha256:24fb3a85df17b58602c1416b6453dd805f09a62e0a9c95e9f0eb0947f24ec4da
```

-	Docker Version: 18.03.1-ee-4
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.2 GB (2241472045 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:43ed286fa68808142212fdc36793359b2b0a9dca8f560a9974da6c86f1b8d1c4`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 15 Sep 2018 09:10:26 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 11 Jan 2020 05:23:25 GMT
RUN Install update 1809-amd64
# Tue, 14 Jan 2020 23:46:02 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 15 Jan 2020 22:23:59 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/containous/traefik/releases/download/v2.1.2/traefik_v2.1.2_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Wed, 15 Jan 2020 22:24:03 GMT
EXPOSE 80
# Wed, 15 Jan 2020 22:24:04 GMT
ENTRYPOINT ["/traefik"]
# Wed, 15 Jan 2020 22:24:06 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.1.2 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:65014b3c312172f10bd6701a063f9b5aaf9a916c2d2cb843d406a6f77ded3f8d`  
		Last Modified: Tue, 13 Nov 2018 18:50:17 GMT  
		Size: 1.5 GB (1534685324 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:edbd72df76b46e904108d2f61a63c295b3e3d8092dbd5a03bbeb2fb4d34a3e55`  
		Size: 682.7 MB (682725872 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e9d323e253cb21832421dda4ec57dbd597bd4f934e62c162b9dec8b96e06e818`  
		Last Modified: Wed, 15 Jan 2020 01:45:20 GMT  
		Size: 1.2 KB (1193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:925f59c295b5302641a4009f899086f273c0f7ae66604422c30b9cda5f334094`  
		Last Modified: Wed, 15 Jan 2020 22:26:25 GMT  
		Size: 24.1 MB (24056072 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5d394b8b9b33f0860352480d9867cf1d5f765ee8411e3452db10d62b595fd22`  
		Last Modified: Wed, 15 Jan 2020 22:26:00 GMT  
		Size: 1.2 KB (1208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:057e7d4d86fd9c71a4c24e4936055f48c8855639f3b5e4a09b84cb34ff07c435`  
		Last Modified: Wed, 15 Jan 2020 22:26:01 GMT  
		Size: 1.2 KB (1187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33754414b9289672384e99a88abefcbbe951b5ee9d26e7f1b6be260214e0b438`  
		Last Modified: Wed, 15 Jan 2020 22:26:00 GMT  
		Size: 1.2 KB (1189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:windowsservercore-1809`

```console
$ docker pull traefik@sha256:aa59d49fa49fa83d7391fd66f1481babbbd88bd2282a10da3d0ce61046b43435
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.973; amd64

### `traefik:windowsservercore-1809` - windows version 10.0.17763.973; amd64

```console
$ docker pull traefik@sha256:24fb3a85df17b58602c1416b6453dd805f09a62e0a9c95e9f0eb0947f24ec4da
```

-	Docker Version: 18.03.1-ee-4
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.2 GB (2241472045 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:43ed286fa68808142212fdc36793359b2b0a9dca8f560a9974da6c86f1b8d1c4`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 15 Sep 2018 09:10:26 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 11 Jan 2020 05:23:25 GMT
RUN Install update 1809-amd64
# Tue, 14 Jan 2020 23:46:02 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 15 Jan 2020 22:23:59 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/containous/traefik/releases/download/v2.1.2/traefik_v2.1.2_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Wed, 15 Jan 2020 22:24:03 GMT
EXPOSE 80
# Wed, 15 Jan 2020 22:24:04 GMT
ENTRYPOINT ["/traefik"]
# Wed, 15 Jan 2020 22:24:06 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.1.2 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:65014b3c312172f10bd6701a063f9b5aaf9a916c2d2cb843d406a6f77ded3f8d`  
		Last Modified: Tue, 13 Nov 2018 18:50:17 GMT  
		Size: 1.5 GB (1534685324 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:edbd72df76b46e904108d2f61a63c295b3e3d8092dbd5a03bbeb2fb4d34a3e55`  
		Size: 682.7 MB (682725872 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e9d323e253cb21832421dda4ec57dbd597bd4f934e62c162b9dec8b96e06e818`  
		Last Modified: Wed, 15 Jan 2020 01:45:20 GMT  
		Size: 1.2 KB (1193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:925f59c295b5302641a4009f899086f273c0f7ae66604422c30b9cda5f334094`  
		Last Modified: Wed, 15 Jan 2020 22:26:25 GMT  
		Size: 24.1 MB (24056072 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5d394b8b9b33f0860352480d9867cf1d5f765ee8411e3452db10d62b595fd22`  
		Last Modified: Wed, 15 Jan 2020 22:26:00 GMT  
		Size: 1.2 KB (1208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:057e7d4d86fd9c71a4c24e4936055f48c8855639f3b5e4a09b84cb34ff07c435`  
		Last Modified: Wed, 15 Jan 2020 22:26:01 GMT  
		Size: 1.2 KB (1187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33754414b9289672384e99a88abefcbbe951b5ee9d26e7f1b6be260214e0b438`  
		Last Modified: Wed, 15 Jan 2020 22:26:00 GMT  
		Size: 1.2 KB (1189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
