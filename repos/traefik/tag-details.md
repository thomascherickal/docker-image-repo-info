<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `traefik`

-	[`traefik:1.7`](#traefik17)
-	[`traefik:1.7-alpine`](#traefik17-alpine)
-	[`traefik:1.7-windowsservercore-1809`](#traefik17-windowsservercore-1809)
-	[`traefik:1.7.30`](#traefik1730)
-	[`traefik:1.7.30-alpine`](#traefik1730-alpine)
-	[`traefik:1.7.30-windowsservercore-1809`](#traefik1730-windowsservercore-1809)
-	[`traefik:2.4`](#traefik24)
-	[`traefik:2.4-windowsservercore-1809`](#traefik24-windowsservercore-1809)
-	[`traefik:2.4.8`](#traefik248)
-	[`traefik:2.4.8-windowsservercore-1809`](#traefik248-windowsservercore-1809)
-	[`traefik:latest`](#traefiklatest)
-	[`traefik:livarot`](#traefiklivarot)
-	[`traefik:livarot-windowsservercore-1809`](#traefiklivarot-windowsservercore-1809)
-	[`traefik:maroilles`](#traefikmaroilles)
-	[`traefik:maroilles-alpine`](#traefikmaroilles-alpine)
-	[`traefik:maroilles-windowsservercore-1809`](#traefikmaroilles-windowsservercore-1809)
-	[`traefik:v1.7`](#traefikv17)
-	[`traefik:v1.7-alpine`](#traefikv17-alpine)
-	[`traefik:v1.7-windowsservercore-1809`](#traefikv17-windowsservercore-1809)
-	[`traefik:v1.7.30`](#traefikv1730)
-	[`traefik:v1.7.30-alpine`](#traefikv1730-alpine)
-	[`traefik:v1.7.30-windowsservercore-1809`](#traefikv1730-windowsservercore-1809)
-	[`traefik:v2.4`](#traefikv24)
-	[`traefik:v2.4-windowsservercore-1809`](#traefikv24-windowsservercore-1809)
-	[`traefik:v2.4.8`](#traefikv248)
-	[`traefik:v2.4.8-windowsservercore-1809`](#traefikv248-windowsservercore-1809)
-	[`traefik:windowsservercore-1809`](#traefikwindowsservercore-1809)

## `traefik:1.7`

```console
$ docker pull traefik@sha256:5e2dfb5243ae97ddb7c959addb389643a1c9787d813630f23684eff53b4775dd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:1.7` - linux; amd64

```console
$ docker pull traefik@sha256:353827cc14120a14b1eccbb2714039763d9cefc284213b53d82d14e110fadc39
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.1 MB (18124621 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2a2126389e0b0dbd13da033d79636b0f0626d73f1a6da0935ce6ce9eccae112a`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Tue, 09 Mar 2021 01:32:48 GMT
COPY file:cd6264d9a7514a8fbc3eb7b400566d36178794d2b757959812cc3abc6f13a97b in /etc/ssl/certs/ 
# Tue, 09 Mar 2021 01:32:49 GMT
COPY dir:379603788862c2a6c57432d70b0a67f561fe00310e1b958c9ecf85381b1c9cd9 in /usr/share/ 
# Thu, 08 Apr 2021 20:07:38 GMT
COPY file:bc0b1c0235bda22a75d2ef00a982989cdf1da3240f077584bca5c6b560a4c13a in / 
# Thu, 08 Apr 2021 20:07:38 GMT
EXPOSE 80
# Thu, 08 Apr 2021 20:07:39 GMT
VOLUME [/tmp]
# Thu, 08 Apr 2021 20:07:39 GMT
ENTRYPOINT ["/traefik"]
# Thu, 08 Apr 2021 20:07:40 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.30 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:53f50c15495c67f391a5750288681a589b19a39c4b78e7ebc0934606cc3d0bc3`  
		Last Modified: Tue, 09 Mar 2021 01:33:59 GMT  
		Size: 130.9 KB (130870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89c044b3636c16c5ab8fc96a04f320c9f97ea23aaffec9adb2d8f20ebaef93f3`  
		Last Modified: Tue, 09 Mar 2021 01:33:59 GMT  
		Size: 308.8 KB (308823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2eb3d26b40720e4da5cbeb15193c698565e23551a24cc4abc4acd1b7de414279`  
		Last Modified: Thu, 08 Apr 2021 20:08:34 GMT  
		Size: 17.7 MB (17684928 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:1.7` - linux; arm variant v6

```console
$ docker pull traefik@sha256:5c7347d0c834b82833b1d344eb84d8491f4afff9c180aad1e287bfb28612d5ec
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.0 MB (16956529 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:90f7d007bf10f706fa796c9f4cc9ad283fd98d0a8ae604e72748f96e43aa9565`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Thu, 17 Dec 2020 00:26:47 GMT
COPY file:cd6264d9a7514a8fbc3eb7b400566d36178794d2b757959812cc3abc6f13a97b in /etc/ssl/certs/ 
# Wed, 24 Feb 2021 23:34:19 GMT
COPY dir:379603788862c2a6c57432d70b0a67f561fe00310e1b958c9ecf85381b1c9cd9 in /usr/share/ 
# Thu, 08 Apr 2021 19:28:36 GMT
COPY file:440b6b1ebd389a2397ffb187ded4c85dcf37b7284d94c693b0b603d51247c683 in / 
# Thu, 08 Apr 2021 19:28:38 GMT
EXPOSE 80
# Thu, 08 Apr 2021 19:28:39 GMT
VOLUME [/tmp]
# Thu, 08 Apr 2021 19:28:41 GMT
ENTRYPOINT ["/traefik"]
# Thu, 08 Apr 2021 19:28:42 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.30 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:26c529e82b09c489524aa4f787754320793a95eb7aa7eaf306c517b76818ec25`  
		Last Modified: Thu, 17 Dec 2020 00:28:41 GMT  
		Size: 130.9 KB (130873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e74b8526f2bdaa522f470d66d09f7ebbe9a1f060ce049ac91c0f7aad153e1be`  
		Last Modified: Wed, 24 Feb 2021 23:36:10 GMT  
		Size: 308.9 KB (308855 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba2277a3749c5a6efdb45bc2ff1ce8c98de01e3225fb4b0df258523fe93391c5`  
		Last Modified: Thu, 08 Apr 2021 19:29:27 GMT  
		Size: 16.5 MB (16516801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:1.7` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:9d2ec3215411977686c39214b6a14e65eb82434ab9652451f8dc2ce54fe9ca0a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.5 MB (16533607 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:df27dd67357d586d32809c5642158f6bdccbce6f28664694b215bd5b2cb6ee99`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Thu, 17 Dec 2020 00:27:56 GMT
COPY file:cd6264d9a7514a8fbc3eb7b400566d36178794d2b757959812cc3abc6f13a97b in /etc/ssl/certs/ 
# Thu, 25 Feb 2021 04:23:55 GMT
COPY dir:379603788862c2a6c57432d70b0a67f561fe00310e1b958c9ecf85381b1c9cd9 in /usr/share/ 
# Thu, 08 Apr 2021 20:39:22 GMT
COPY file:6fdd60dc35db1c19a5de5ed8b57f159a6e121ba0f1ddb3e48a6e185da99f8cca in / 
# Thu, 08 Apr 2021 20:39:23 GMT
EXPOSE 80
# Thu, 08 Apr 2021 20:39:24 GMT
VOLUME [/tmp]
# Thu, 08 Apr 2021 20:39:25 GMT
ENTRYPOINT ["/traefik"]
# Thu, 08 Apr 2021 20:39:26 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.30 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:7dccf22d113d483cac839141f2028cbf6ac2e0c6aa4a1716c5e7b575b162028c`  
		Last Modified: Thu, 17 Dec 2020 00:29:55 GMT  
		Size: 130.9 KB (130873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41f74910073ee331bfbff1c3d20a2d29270f713f515ccee693e566b927d37654`  
		Last Modified: Thu, 25 Feb 2021 04:25:12 GMT  
		Size: 308.8 KB (308831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db3a97f2585cdbe5ac39667c253a77c35e2cbc755c2d788f76a1b2fd02413e51`  
		Last Modified: Thu, 08 Apr 2021 20:40:11 GMT  
		Size: 16.1 MB (16093903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:1.7-alpine`

```console
$ docker pull traefik@sha256:bb221da9b5335ecac917502708411306ad6ea0b720f9ee0c723451a83255fda1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:1.7-alpine` - linux; amd64

```console
$ docker pull traefik@sha256:5e1e280e8e56520c8ebc11425f2c9fe66c9fae4714d65833d7f15c40fde8fb80
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **21.2 MB (21175700 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:55847f6ab3e15d3f6304ec3271273146b44942dff17926a61366afbdf6736671`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:56 GMT
ADD file:282b9d56236cae29600bf8b698cb0a865ab17db7beea0be6870f9de63e7d4f80 in / 
# Wed, 14 Apr 2021 19:19:56 GMT
CMD ["/bin/sh"]
# Thu, 15 Apr 2021 03:04:42 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 15 Apr 2021 03:04:59 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/traefik/traefik/releases/download/v1.7.30/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Thu, 15 Apr 2021 03:05:00 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 15 Apr 2021 03:05:00 GMT
EXPOSE 80
# Thu, 15 Apr 2021 03:05:00 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 15 Apr 2021 03:05:01 GMT
CMD ["traefik"]
# Thu, 15 Apr 2021 03:05:01 GMT
LABEL org.opencontainers.image.vendor=traefik org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.30 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:ddad3d7c1e96adf9153f8921a7c9790f880a390163df453be1566e9ef0d546e0`  
		Last Modified: Wed, 14 Apr 2021 19:21:03 GMT  
		Size: 2.8 MB (2816246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f6722e60c2f6c55424dadebe886f88ba1b903df075b00048427439abb91b85a`  
		Last Modified: Thu, 15 Apr 2021 03:05:57 GMT  
		Size: 674.2 KB (674210 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e40cdaabf18912622322046bb5eeda16c1ac513a094389e9b12b33ff02abb2c`  
		Last Modified: Thu, 15 Apr 2021 03:06:32 GMT  
		Size: 17.7 MB (17684875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1ec9b7bad03eb2d44d70526dbd5478e8ee4043e8445168201605f71fafbb22e`  
		Last Modified: Thu, 15 Apr 2021 03:06:25 GMT  
		Size: 369.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:1.7-alpine` - linux; arm variant v6

```console
$ docker pull traefik@sha256:01eccfad104e020c243676c64ede0b15f789bdb44c72504534412a3751b595b6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **19.8 MB (19815547 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e2c542dcb63b74c456178e52089c32d41929581f8c12124065b7df092764d685`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 31 Mar 2021 17:19:20 GMT
ADD file:15a1f9d3700deb648f0b3701afebc97ff28eb30d1b55e18dc9c696a9dd5c8e36 in / 
# Wed, 31 Mar 2021 17:19:21 GMT
CMD ["/bin/sh"]
# Thu, 01 Apr 2021 03:52:35 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 08 Apr 2021 19:28:18 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/traefik/traefik/releases/download/v1.7.30/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Thu, 08 Apr 2021 19:28:19 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 08 Apr 2021 19:28:20 GMT
EXPOSE 80
# Thu, 08 Apr 2021 19:28:21 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 08 Apr 2021 19:28:22 GMT
CMD ["traefik"]
# Thu, 08 Apr 2021 19:28:23 GMT
LABEL org.opencontainers.image.vendor=traefik org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.30 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:ac95243af174972febc49043f62f7b952a0c610e59b55ac4133f442e399e8729`  
		Last Modified: Wed, 31 Mar 2021 17:20:17 GMT  
		Size: 2.6 MB (2621248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25173f2bf7681888ff03bae0a793dcd2a8124175d360f999d21081483f90f181`  
		Last Modified: Thu, 01 Apr 2021 03:54:34 GMT  
		Size: 677.0 KB (677016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59eb9988c4b9b573a94c2aef256f275f37bc80f4537429e21a07866e21c30c15`  
		Last Modified: Thu, 08 Apr 2021 19:29:12 GMT  
		Size: 16.5 MB (16516915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43e60f188a205da97f1f59c9e979da57a3f96fcdd8a7b677d798138f433a8fca`  
		Last Modified: Thu, 08 Apr 2021 19:29:06 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:1.7-alpine` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:0cf15008333d1cc2b7907ebead2b805754d3fd9a35ee0b5ef8f52d26e69d9e35
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **19.5 MB (19495771 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7f9ab0b3ea9162be9ba4e2fedca5164d4769d09ad5492d8df197d742139defbb`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 31 Mar 2021 17:22:02 GMT
ADD file:174ba1b913c5cf549fcdfc259e8e3aa8f49cea660865fd54b8aacb430602a783 in / 
# Wed, 31 Mar 2021 17:22:03 GMT
CMD ["/bin/sh"]
# Thu, 01 Apr 2021 16:15:15 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 08 Apr 2021 20:39:00 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/traefik/traefik/releases/download/v1.7.30/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Thu, 08 Apr 2021 20:39:01 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 08 Apr 2021 20:39:02 GMT
EXPOSE 80
# Thu, 08 Apr 2021 20:39:03 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 08 Apr 2021 20:39:04 GMT
CMD ["traefik"]
# Thu, 08 Apr 2021 20:39:05 GMT
LABEL org.opencontainers.image.vendor=traefik org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.30 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:a3cf95b55367cb73f51318ee9c854def347373482336709ca1882a5d4c20b7c7`  
		Last Modified: Wed, 31 Mar 2021 17:23:00 GMT  
		Size: 2.7 MB (2725871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e08c5532ded8a461bb2539065ec0daf26ce2ecfed811ad86719ad11c964ab658`  
		Last Modified: Thu, 01 Apr 2021 16:17:57 GMT  
		Size: 675.5 KB (675530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bdb060704f0ed88ad3c7606d012c734450f30bd6d4fdfe4afe65a3109473985`  
		Last Modified: Thu, 08 Apr 2021 20:39:54 GMT  
		Size: 16.1 MB (16094002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b924f9ea1253bff83db6941fc95ed9248766194e0712f66bde5fa5f8d89cfe0`  
		Last Modified: Thu, 08 Apr 2021 20:39:49 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:1.7-windowsservercore-1809`

```console
$ docker pull traefik@sha256:733a8c228d615ebf548385487b66c7b3fdd7699c1c9f7fec1cfa4c71feeb4785
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1879; amd64

### `traefik:1.7-windowsservercore-1809` - windows version 10.0.17763.1879; amd64

```console
$ docker pull traefik@sha256:e7f8b8eee97e1609e89c4a19e3f7f530a33ca76b26196d1c6bc927eca28645c3
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2492758593 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8bb83271e02abc3f1a599c84de304ca6c4f9ceab42a58cf154675cad4c8e761b`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 09 Apr 2021 20:34:41 GMT
RUN Install update 1809-amd64
# Wed, 14 Apr 2021 12:09:21 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 14 Apr 2021 21:29:52 GMT
RUN Invoke-WebRequest     -Uri "https://github.com/traefik/traefik/releases/download/v1.7.30/traefik_windows-amd64.exe"     -OutFile "/traefik.exe"
# Wed, 14 Apr 2021 21:29:54 GMT
EXPOSE 80
# Wed, 14 Apr 2021 21:29:55 GMT
ENTRYPOINT ["/traefik"]
# Wed, 14 Apr 2021 21:29:56 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.30 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:399f118dfaa9a753e98d128238b944432c7bcabea88a2998a6efbbece28ed303`  
		Size: 751.4 MB (751421005 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:106dbf3373fce4f0ba5e00ad54824c597f2894605fa7d8ef446ad7ea3b97449f`  
		Last Modified: Wed, 14 Apr 2021 12:58:04 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:203e1506701de3ad9fca12951ea83f903d0bdc8628f20a7bfb3d77a713a5ed52`  
		Last Modified: Wed, 14 Apr 2021 21:31:15 GMT  
		Size: 23.0 MB (22998990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2b11339a17c4a4101817c0f6ddc3f3453e39f1c052aedf3f0e9cdb0ffc84365`  
		Last Modified: Wed, 14 Apr 2021 21:31:08 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07482932f6ca5c824d683ca413e9ef96f6aa833fc867c4d614428803b25d6143`  
		Last Modified: Wed, 14 Apr 2021 21:31:08 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f776de6cf2f2359d3f8ccf8e44387cbe850d86e91540ddd4253809940c7afb76`  
		Last Modified: Wed, 14 Apr 2021 21:31:08 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:1.7.30`

```console
$ docker pull traefik@sha256:5e2dfb5243ae97ddb7c959addb389643a1c9787d813630f23684eff53b4775dd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:1.7.30` - linux; amd64

```console
$ docker pull traefik@sha256:353827cc14120a14b1eccbb2714039763d9cefc284213b53d82d14e110fadc39
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.1 MB (18124621 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2a2126389e0b0dbd13da033d79636b0f0626d73f1a6da0935ce6ce9eccae112a`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Tue, 09 Mar 2021 01:32:48 GMT
COPY file:cd6264d9a7514a8fbc3eb7b400566d36178794d2b757959812cc3abc6f13a97b in /etc/ssl/certs/ 
# Tue, 09 Mar 2021 01:32:49 GMT
COPY dir:379603788862c2a6c57432d70b0a67f561fe00310e1b958c9ecf85381b1c9cd9 in /usr/share/ 
# Thu, 08 Apr 2021 20:07:38 GMT
COPY file:bc0b1c0235bda22a75d2ef00a982989cdf1da3240f077584bca5c6b560a4c13a in / 
# Thu, 08 Apr 2021 20:07:38 GMT
EXPOSE 80
# Thu, 08 Apr 2021 20:07:39 GMT
VOLUME [/tmp]
# Thu, 08 Apr 2021 20:07:39 GMT
ENTRYPOINT ["/traefik"]
# Thu, 08 Apr 2021 20:07:40 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.30 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:53f50c15495c67f391a5750288681a589b19a39c4b78e7ebc0934606cc3d0bc3`  
		Last Modified: Tue, 09 Mar 2021 01:33:59 GMT  
		Size: 130.9 KB (130870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89c044b3636c16c5ab8fc96a04f320c9f97ea23aaffec9adb2d8f20ebaef93f3`  
		Last Modified: Tue, 09 Mar 2021 01:33:59 GMT  
		Size: 308.8 KB (308823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2eb3d26b40720e4da5cbeb15193c698565e23551a24cc4abc4acd1b7de414279`  
		Last Modified: Thu, 08 Apr 2021 20:08:34 GMT  
		Size: 17.7 MB (17684928 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:1.7.30` - linux; arm variant v6

```console
$ docker pull traefik@sha256:5c7347d0c834b82833b1d344eb84d8491f4afff9c180aad1e287bfb28612d5ec
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.0 MB (16956529 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:90f7d007bf10f706fa796c9f4cc9ad283fd98d0a8ae604e72748f96e43aa9565`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Thu, 17 Dec 2020 00:26:47 GMT
COPY file:cd6264d9a7514a8fbc3eb7b400566d36178794d2b757959812cc3abc6f13a97b in /etc/ssl/certs/ 
# Wed, 24 Feb 2021 23:34:19 GMT
COPY dir:379603788862c2a6c57432d70b0a67f561fe00310e1b958c9ecf85381b1c9cd9 in /usr/share/ 
# Thu, 08 Apr 2021 19:28:36 GMT
COPY file:440b6b1ebd389a2397ffb187ded4c85dcf37b7284d94c693b0b603d51247c683 in / 
# Thu, 08 Apr 2021 19:28:38 GMT
EXPOSE 80
# Thu, 08 Apr 2021 19:28:39 GMT
VOLUME [/tmp]
# Thu, 08 Apr 2021 19:28:41 GMT
ENTRYPOINT ["/traefik"]
# Thu, 08 Apr 2021 19:28:42 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.30 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:26c529e82b09c489524aa4f787754320793a95eb7aa7eaf306c517b76818ec25`  
		Last Modified: Thu, 17 Dec 2020 00:28:41 GMT  
		Size: 130.9 KB (130873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e74b8526f2bdaa522f470d66d09f7ebbe9a1f060ce049ac91c0f7aad153e1be`  
		Last Modified: Wed, 24 Feb 2021 23:36:10 GMT  
		Size: 308.9 KB (308855 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba2277a3749c5a6efdb45bc2ff1ce8c98de01e3225fb4b0df258523fe93391c5`  
		Last Modified: Thu, 08 Apr 2021 19:29:27 GMT  
		Size: 16.5 MB (16516801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:1.7.30` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:9d2ec3215411977686c39214b6a14e65eb82434ab9652451f8dc2ce54fe9ca0a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.5 MB (16533607 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:df27dd67357d586d32809c5642158f6bdccbce6f28664694b215bd5b2cb6ee99`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Thu, 17 Dec 2020 00:27:56 GMT
COPY file:cd6264d9a7514a8fbc3eb7b400566d36178794d2b757959812cc3abc6f13a97b in /etc/ssl/certs/ 
# Thu, 25 Feb 2021 04:23:55 GMT
COPY dir:379603788862c2a6c57432d70b0a67f561fe00310e1b958c9ecf85381b1c9cd9 in /usr/share/ 
# Thu, 08 Apr 2021 20:39:22 GMT
COPY file:6fdd60dc35db1c19a5de5ed8b57f159a6e121ba0f1ddb3e48a6e185da99f8cca in / 
# Thu, 08 Apr 2021 20:39:23 GMT
EXPOSE 80
# Thu, 08 Apr 2021 20:39:24 GMT
VOLUME [/tmp]
# Thu, 08 Apr 2021 20:39:25 GMT
ENTRYPOINT ["/traefik"]
# Thu, 08 Apr 2021 20:39:26 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.30 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:7dccf22d113d483cac839141f2028cbf6ac2e0c6aa4a1716c5e7b575b162028c`  
		Last Modified: Thu, 17 Dec 2020 00:29:55 GMT  
		Size: 130.9 KB (130873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41f74910073ee331bfbff1c3d20a2d29270f713f515ccee693e566b927d37654`  
		Last Modified: Thu, 25 Feb 2021 04:25:12 GMT  
		Size: 308.8 KB (308831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db3a97f2585cdbe5ac39667c253a77c35e2cbc755c2d788f76a1b2fd02413e51`  
		Last Modified: Thu, 08 Apr 2021 20:40:11 GMT  
		Size: 16.1 MB (16093903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:1.7.30-alpine`

```console
$ docker pull traefik@sha256:bb221da9b5335ecac917502708411306ad6ea0b720f9ee0c723451a83255fda1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:1.7.30-alpine` - linux; amd64

```console
$ docker pull traefik@sha256:5e1e280e8e56520c8ebc11425f2c9fe66c9fae4714d65833d7f15c40fde8fb80
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **21.2 MB (21175700 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:55847f6ab3e15d3f6304ec3271273146b44942dff17926a61366afbdf6736671`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:56 GMT
ADD file:282b9d56236cae29600bf8b698cb0a865ab17db7beea0be6870f9de63e7d4f80 in / 
# Wed, 14 Apr 2021 19:19:56 GMT
CMD ["/bin/sh"]
# Thu, 15 Apr 2021 03:04:42 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 15 Apr 2021 03:04:59 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/traefik/traefik/releases/download/v1.7.30/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Thu, 15 Apr 2021 03:05:00 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 15 Apr 2021 03:05:00 GMT
EXPOSE 80
# Thu, 15 Apr 2021 03:05:00 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 15 Apr 2021 03:05:01 GMT
CMD ["traefik"]
# Thu, 15 Apr 2021 03:05:01 GMT
LABEL org.opencontainers.image.vendor=traefik org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.30 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:ddad3d7c1e96adf9153f8921a7c9790f880a390163df453be1566e9ef0d546e0`  
		Last Modified: Wed, 14 Apr 2021 19:21:03 GMT  
		Size: 2.8 MB (2816246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f6722e60c2f6c55424dadebe886f88ba1b903df075b00048427439abb91b85a`  
		Last Modified: Thu, 15 Apr 2021 03:05:57 GMT  
		Size: 674.2 KB (674210 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e40cdaabf18912622322046bb5eeda16c1ac513a094389e9b12b33ff02abb2c`  
		Last Modified: Thu, 15 Apr 2021 03:06:32 GMT  
		Size: 17.7 MB (17684875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1ec9b7bad03eb2d44d70526dbd5478e8ee4043e8445168201605f71fafbb22e`  
		Last Modified: Thu, 15 Apr 2021 03:06:25 GMT  
		Size: 369.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:1.7.30-alpine` - linux; arm variant v6

```console
$ docker pull traefik@sha256:01eccfad104e020c243676c64ede0b15f789bdb44c72504534412a3751b595b6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **19.8 MB (19815547 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e2c542dcb63b74c456178e52089c32d41929581f8c12124065b7df092764d685`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 31 Mar 2021 17:19:20 GMT
ADD file:15a1f9d3700deb648f0b3701afebc97ff28eb30d1b55e18dc9c696a9dd5c8e36 in / 
# Wed, 31 Mar 2021 17:19:21 GMT
CMD ["/bin/sh"]
# Thu, 01 Apr 2021 03:52:35 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 08 Apr 2021 19:28:18 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/traefik/traefik/releases/download/v1.7.30/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Thu, 08 Apr 2021 19:28:19 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 08 Apr 2021 19:28:20 GMT
EXPOSE 80
# Thu, 08 Apr 2021 19:28:21 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 08 Apr 2021 19:28:22 GMT
CMD ["traefik"]
# Thu, 08 Apr 2021 19:28:23 GMT
LABEL org.opencontainers.image.vendor=traefik org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.30 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:ac95243af174972febc49043f62f7b952a0c610e59b55ac4133f442e399e8729`  
		Last Modified: Wed, 31 Mar 2021 17:20:17 GMT  
		Size: 2.6 MB (2621248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25173f2bf7681888ff03bae0a793dcd2a8124175d360f999d21081483f90f181`  
		Last Modified: Thu, 01 Apr 2021 03:54:34 GMT  
		Size: 677.0 KB (677016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59eb9988c4b9b573a94c2aef256f275f37bc80f4537429e21a07866e21c30c15`  
		Last Modified: Thu, 08 Apr 2021 19:29:12 GMT  
		Size: 16.5 MB (16516915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43e60f188a205da97f1f59c9e979da57a3f96fcdd8a7b677d798138f433a8fca`  
		Last Modified: Thu, 08 Apr 2021 19:29:06 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:1.7.30-alpine` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:0cf15008333d1cc2b7907ebead2b805754d3fd9a35ee0b5ef8f52d26e69d9e35
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **19.5 MB (19495771 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7f9ab0b3ea9162be9ba4e2fedca5164d4769d09ad5492d8df197d742139defbb`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 31 Mar 2021 17:22:02 GMT
ADD file:174ba1b913c5cf549fcdfc259e8e3aa8f49cea660865fd54b8aacb430602a783 in / 
# Wed, 31 Mar 2021 17:22:03 GMT
CMD ["/bin/sh"]
# Thu, 01 Apr 2021 16:15:15 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 08 Apr 2021 20:39:00 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/traefik/traefik/releases/download/v1.7.30/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Thu, 08 Apr 2021 20:39:01 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 08 Apr 2021 20:39:02 GMT
EXPOSE 80
# Thu, 08 Apr 2021 20:39:03 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 08 Apr 2021 20:39:04 GMT
CMD ["traefik"]
# Thu, 08 Apr 2021 20:39:05 GMT
LABEL org.opencontainers.image.vendor=traefik org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.30 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:a3cf95b55367cb73f51318ee9c854def347373482336709ca1882a5d4c20b7c7`  
		Last Modified: Wed, 31 Mar 2021 17:23:00 GMT  
		Size: 2.7 MB (2725871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e08c5532ded8a461bb2539065ec0daf26ce2ecfed811ad86719ad11c964ab658`  
		Last Modified: Thu, 01 Apr 2021 16:17:57 GMT  
		Size: 675.5 KB (675530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bdb060704f0ed88ad3c7606d012c734450f30bd6d4fdfe4afe65a3109473985`  
		Last Modified: Thu, 08 Apr 2021 20:39:54 GMT  
		Size: 16.1 MB (16094002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b924f9ea1253bff83db6941fc95ed9248766194e0712f66bde5fa5f8d89cfe0`  
		Last Modified: Thu, 08 Apr 2021 20:39:49 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:1.7.30-windowsservercore-1809`

```console
$ docker pull traefik@sha256:733a8c228d615ebf548385487b66c7b3fdd7699c1c9f7fec1cfa4c71feeb4785
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1879; amd64

### `traefik:1.7.30-windowsservercore-1809` - windows version 10.0.17763.1879; amd64

```console
$ docker pull traefik@sha256:e7f8b8eee97e1609e89c4a19e3f7f530a33ca76b26196d1c6bc927eca28645c3
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2492758593 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8bb83271e02abc3f1a599c84de304ca6c4f9ceab42a58cf154675cad4c8e761b`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 09 Apr 2021 20:34:41 GMT
RUN Install update 1809-amd64
# Wed, 14 Apr 2021 12:09:21 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 14 Apr 2021 21:29:52 GMT
RUN Invoke-WebRequest     -Uri "https://github.com/traefik/traefik/releases/download/v1.7.30/traefik_windows-amd64.exe"     -OutFile "/traefik.exe"
# Wed, 14 Apr 2021 21:29:54 GMT
EXPOSE 80
# Wed, 14 Apr 2021 21:29:55 GMT
ENTRYPOINT ["/traefik"]
# Wed, 14 Apr 2021 21:29:56 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.30 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:399f118dfaa9a753e98d128238b944432c7bcabea88a2998a6efbbece28ed303`  
		Size: 751.4 MB (751421005 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:106dbf3373fce4f0ba5e00ad54824c597f2894605fa7d8ef446ad7ea3b97449f`  
		Last Modified: Wed, 14 Apr 2021 12:58:04 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:203e1506701de3ad9fca12951ea83f903d0bdc8628f20a7bfb3d77a713a5ed52`  
		Last Modified: Wed, 14 Apr 2021 21:31:15 GMT  
		Size: 23.0 MB (22998990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2b11339a17c4a4101817c0f6ddc3f3453e39f1c052aedf3f0e9cdb0ffc84365`  
		Last Modified: Wed, 14 Apr 2021 21:31:08 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07482932f6ca5c824d683ca413e9ef96f6aa833fc867c4d614428803b25d6143`  
		Last Modified: Wed, 14 Apr 2021 21:31:08 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f776de6cf2f2359d3f8ccf8e44387cbe850d86e91540ddd4253809940c7afb76`  
		Last Modified: Wed, 14 Apr 2021 21:31:08 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:2.4`

```console
$ docker pull traefik@sha256:af1617e167e8a6554b5e75c1fd759c68887b890be715afa5f36d9ac467410d45
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:2.4` - linux; amd64

```console
$ docker pull traefik@sha256:4e2da005d39daa3823c6930cfb4ff5eb8d75be3679a2173489d8579e655be4be
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.8 MB (27828337 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:deaf4b1027ed4bce7d3a15a22a7ff5f5fab274bffde1709ae85e93f15085ad98`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:56 GMT
ADD file:282b9d56236cae29600bf8b698cb0a865ab17db7beea0be6870f9de63e7d4f80 in / 
# Wed, 14 Apr 2021 19:19:56 GMT
CMD ["/bin/sh"]
# Thu, 15 Apr 2021 03:04:42 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 15 Apr 2021 03:04:47 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.4.8/traefik_v2.4.8_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 15 Apr 2021 03:04:48 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 15 Apr 2021 03:04:48 GMT
EXPOSE 80
# Thu, 15 Apr 2021 03:04:48 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 15 Apr 2021 03:04:49 GMT
CMD ["traefik"]
# Thu, 15 Apr 2021 03:04:49 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.4.8 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:ddad3d7c1e96adf9153f8921a7c9790f880a390163df453be1566e9ef0d546e0`  
		Last Modified: Wed, 14 Apr 2021 19:21:03 GMT  
		Size: 2.8 MB (2816246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f6722e60c2f6c55424dadebe886f88ba1b903df075b00048427439abb91b85a`  
		Last Modified: Thu, 15 Apr 2021 03:05:57 GMT  
		Size: 674.2 KB (674210 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acb62688737133737535c58e692b79b70843447464a3760d37d1d65c33fa1e5c`  
		Last Modified: Thu, 15 Apr 2021 03:06:03 GMT  
		Size: 24.3 MB (24337513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebb6d79f94aac9a1ec9746826d0fd58ea98a05df8f5ed882819626db57909331`  
		Last Modified: Thu, 15 Apr 2021 03:05:57 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:2.4` - linux; arm variant v6

```console
$ docker pull traefik@sha256:445ec88018c03307101e734adfd8425f4da87e9ffd5d83b1e5fb512d280df5df
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.0 MB (26025735 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9a68d5d0d7cdf26c5ef8132873c04d3e8cc92b65cd6ad0af323361a5c222c57f`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 31 Mar 2021 17:19:20 GMT
ADD file:15a1f9d3700deb648f0b3701afebc97ff28eb30d1b55e18dc9c696a9dd5c8e36 in / 
# Wed, 31 Mar 2021 17:19:21 GMT
CMD ["/bin/sh"]
# Thu, 01 Apr 2021 03:52:35 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 01 Apr 2021 03:52:43 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.4.8/traefik_v2.4.8_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 01 Apr 2021 03:52:44 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 01 Apr 2021 03:52:45 GMT
EXPOSE 80
# Thu, 01 Apr 2021 03:52:47 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 01 Apr 2021 03:52:48 GMT
CMD ["traefik"]
# Thu, 01 Apr 2021 03:52:50 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.4.8 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:ac95243af174972febc49043f62f7b952a0c610e59b55ac4133f442e399e8729`  
		Last Modified: Wed, 31 Mar 2021 17:20:17 GMT  
		Size: 2.6 MB (2621248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25173f2bf7681888ff03bae0a793dcd2a8124175d360f999d21081483f90f181`  
		Last Modified: Thu, 01 Apr 2021 03:54:34 GMT  
		Size: 677.0 KB (677016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9546526ac0315b3d34e7f88f707fb5355cffd936afb2e80198eff85c6524a05`  
		Last Modified: Thu, 01 Apr 2021 03:54:41 GMT  
		Size: 22.7 MB (22727103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ddd0b0952f4a6439010368b09c4bee68dd82bad0c47ff2a4a3a0b8ce6a2c498`  
		Last Modified: Thu, 01 Apr 2021 03:54:33 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:2.4` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:edd78c8c05d3050cbd62e00de1575597f2a1c628fd5faefecb0d8b20c35d7ba9
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.5 MB (25475489 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:19eb3704549293128f6d623b5a417a6cf34b01a797b4e0bf36dee8ef8f255e71`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 31 Mar 2021 17:22:02 GMT
ADD file:174ba1b913c5cf549fcdfc259e8e3aa8f49cea660865fd54b8aacb430602a783 in / 
# Wed, 31 Mar 2021 17:22:03 GMT
CMD ["/bin/sh"]
# Thu, 01 Apr 2021 16:15:15 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 01 Apr 2021 16:15:20 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.4.8/traefik_v2.4.8_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 01 Apr 2021 16:15:22 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 01 Apr 2021 16:15:23 GMT
EXPOSE 80
# Thu, 01 Apr 2021 16:15:23 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 01 Apr 2021 16:15:24 GMT
CMD ["traefik"]
# Thu, 01 Apr 2021 16:15:25 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.4.8 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:a3cf95b55367cb73f51318ee9c854def347373482336709ca1882a5d4c20b7c7`  
		Last Modified: Wed, 31 Mar 2021 17:23:00 GMT  
		Size: 2.7 MB (2725871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e08c5532ded8a461bb2539065ec0daf26ce2ecfed811ad86719ad11c964ab658`  
		Last Modified: Thu, 01 Apr 2021 16:17:57 GMT  
		Size: 675.5 KB (675530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:664cdd830c93e0170df8d4ed17b45f260ee577dcfb6db4d48f6e009b108ff81d`  
		Last Modified: Thu, 01 Apr 2021 16:18:03 GMT  
		Size: 22.1 MB (22073720 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91bdc2d37fb1c66af3a73e5fff4790dcfa4572a7fd25779591f80bd086c718df`  
		Last Modified: Thu, 01 Apr 2021 16:17:57 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:2.4-windowsservercore-1809`

```console
$ docker pull traefik@sha256:a469fcdb7481c955407299e937c5b6cb5c203f6d7cc71c76932b0f41594ee652
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1879; amd64

### `traefik:2.4-windowsservercore-1809` - windows version 10.0.17763.1879; amd64

```console
$ docker pull traefik@sha256:0fda36d6a58507d81a2c34a79738e3e19ab72b1c3f63316fb0ea4505eb500b09
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2499488628 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3650b9ad832bb235bd53c735995b7542b8bf3dd3dd4cdd9a82e38c5ff8d23c44`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 09 Apr 2021 20:34:41 GMT
RUN Install update 1809-amd64
# Wed, 14 Apr 2021 12:09:21 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 14 Apr 2021 21:28:41 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/traefik/traefik/releases/download/v2.4.8/traefik_v2.4.8_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Wed, 14 Apr 2021 21:28:43 GMT
EXPOSE 80
# Wed, 14 Apr 2021 21:28:44 GMT
ENTRYPOINT ["/traefik"]
# Wed, 14 Apr 2021 21:28:45 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.4.8 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:399f118dfaa9a753e98d128238b944432c7bcabea88a2998a6efbbece28ed303`  
		Size: 751.4 MB (751421005 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:106dbf3373fce4f0ba5e00ad54824c597f2894605fa7d8ef446ad7ea3b97449f`  
		Last Modified: Wed, 14 Apr 2021 12:58:04 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a93cd244b1a7725d26281629f3d234056508569c464f5dea5b03ccbde91bb0f`  
		Last Modified: Wed, 14 Apr 2021 21:30:37 GMT  
		Size: 29.7 MB (29729029 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f7bb23c17022bf3359394806bf3c61d486089608895251ff7a5acfd7ad96a9a`  
		Last Modified: Wed, 14 Apr 2021 21:30:28 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb84fdded1774834fd927e9a9f74098955381bfeb1991c90d23188e9f2d4bf95`  
		Last Modified: Wed, 14 Apr 2021 21:30:27 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46b1c96a0690beee17c07772a87933a00a71ff757191a2e22ddb4b54488a8000`  
		Last Modified: Wed, 14 Apr 2021 21:30:27 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:2.4.8`

```console
$ docker pull traefik@sha256:af1617e167e8a6554b5e75c1fd759c68887b890be715afa5f36d9ac467410d45
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:2.4.8` - linux; amd64

```console
$ docker pull traefik@sha256:4e2da005d39daa3823c6930cfb4ff5eb8d75be3679a2173489d8579e655be4be
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.8 MB (27828337 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:deaf4b1027ed4bce7d3a15a22a7ff5f5fab274bffde1709ae85e93f15085ad98`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:56 GMT
ADD file:282b9d56236cae29600bf8b698cb0a865ab17db7beea0be6870f9de63e7d4f80 in / 
# Wed, 14 Apr 2021 19:19:56 GMT
CMD ["/bin/sh"]
# Thu, 15 Apr 2021 03:04:42 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 15 Apr 2021 03:04:47 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.4.8/traefik_v2.4.8_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 15 Apr 2021 03:04:48 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 15 Apr 2021 03:04:48 GMT
EXPOSE 80
# Thu, 15 Apr 2021 03:04:48 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 15 Apr 2021 03:04:49 GMT
CMD ["traefik"]
# Thu, 15 Apr 2021 03:04:49 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.4.8 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:ddad3d7c1e96adf9153f8921a7c9790f880a390163df453be1566e9ef0d546e0`  
		Last Modified: Wed, 14 Apr 2021 19:21:03 GMT  
		Size: 2.8 MB (2816246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f6722e60c2f6c55424dadebe886f88ba1b903df075b00048427439abb91b85a`  
		Last Modified: Thu, 15 Apr 2021 03:05:57 GMT  
		Size: 674.2 KB (674210 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acb62688737133737535c58e692b79b70843447464a3760d37d1d65c33fa1e5c`  
		Last Modified: Thu, 15 Apr 2021 03:06:03 GMT  
		Size: 24.3 MB (24337513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebb6d79f94aac9a1ec9746826d0fd58ea98a05df8f5ed882819626db57909331`  
		Last Modified: Thu, 15 Apr 2021 03:05:57 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:2.4.8` - linux; arm variant v6

```console
$ docker pull traefik@sha256:445ec88018c03307101e734adfd8425f4da87e9ffd5d83b1e5fb512d280df5df
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.0 MB (26025735 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9a68d5d0d7cdf26c5ef8132873c04d3e8cc92b65cd6ad0af323361a5c222c57f`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 31 Mar 2021 17:19:20 GMT
ADD file:15a1f9d3700deb648f0b3701afebc97ff28eb30d1b55e18dc9c696a9dd5c8e36 in / 
# Wed, 31 Mar 2021 17:19:21 GMT
CMD ["/bin/sh"]
# Thu, 01 Apr 2021 03:52:35 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 01 Apr 2021 03:52:43 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.4.8/traefik_v2.4.8_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 01 Apr 2021 03:52:44 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 01 Apr 2021 03:52:45 GMT
EXPOSE 80
# Thu, 01 Apr 2021 03:52:47 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 01 Apr 2021 03:52:48 GMT
CMD ["traefik"]
# Thu, 01 Apr 2021 03:52:50 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.4.8 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:ac95243af174972febc49043f62f7b952a0c610e59b55ac4133f442e399e8729`  
		Last Modified: Wed, 31 Mar 2021 17:20:17 GMT  
		Size: 2.6 MB (2621248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25173f2bf7681888ff03bae0a793dcd2a8124175d360f999d21081483f90f181`  
		Last Modified: Thu, 01 Apr 2021 03:54:34 GMT  
		Size: 677.0 KB (677016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9546526ac0315b3d34e7f88f707fb5355cffd936afb2e80198eff85c6524a05`  
		Last Modified: Thu, 01 Apr 2021 03:54:41 GMT  
		Size: 22.7 MB (22727103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ddd0b0952f4a6439010368b09c4bee68dd82bad0c47ff2a4a3a0b8ce6a2c498`  
		Last Modified: Thu, 01 Apr 2021 03:54:33 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:2.4.8` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:edd78c8c05d3050cbd62e00de1575597f2a1c628fd5faefecb0d8b20c35d7ba9
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.5 MB (25475489 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:19eb3704549293128f6d623b5a417a6cf34b01a797b4e0bf36dee8ef8f255e71`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 31 Mar 2021 17:22:02 GMT
ADD file:174ba1b913c5cf549fcdfc259e8e3aa8f49cea660865fd54b8aacb430602a783 in / 
# Wed, 31 Mar 2021 17:22:03 GMT
CMD ["/bin/sh"]
# Thu, 01 Apr 2021 16:15:15 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 01 Apr 2021 16:15:20 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.4.8/traefik_v2.4.8_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 01 Apr 2021 16:15:22 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 01 Apr 2021 16:15:23 GMT
EXPOSE 80
# Thu, 01 Apr 2021 16:15:23 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 01 Apr 2021 16:15:24 GMT
CMD ["traefik"]
# Thu, 01 Apr 2021 16:15:25 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.4.8 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:a3cf95b55367cb73f51318ee9c854def347373482336709ca1882a5d4c20b7c7`  
		Last Modified: Wed, 31 Mar 2021 17:23:00 GMT  
		Size: 2.7 MB (2725871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e08c5532ded8a461bb2539065ec0daf26ce2ecfed811ad86719ad11c964ab658`  
		Last Modified: Thu, 01 Apr 2021 16:17:57 GMT  
		Size: 675.5 KB (675530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:664cdd830c93e0170df8d4ed17b45f260ee577dcfb6db4d48f6e009b108ff81d`  
		Last Modified: Thu, 01 Apr 2021 16:18:03 GMT  
		Size: 22.1 MB (22073720 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91bdc2d37fb1c66af3a73e5fff4790dcfa4572a7fd25779591f80bd086c718df`  
		Last Modified: Thu, 01 Apr 2021 16:17:57 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:2.4.8-windowsservercore-1809`

```console
$ docker pull traefik@sha256:a469fcdb7481c955407299e937c5b6cb5c203f6d7cc71c76932b0f41594ee652
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1879; amd64

### `traefik:2.4.8-windowsservercore-1809` - windows version 10.0.17763.1879; amd64

```console
$ docker pull traefik@sha256:0fda36d6a58507d81a2c34a79738e3e19ab72b1c3f63316fb0ea4505eb500b09
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2499488628 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3650b9ad832bb235bd53c735995b7542b8bf3dd3dd4cdd9a82e38c5ff8d23c44`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 09 Apr 2021 20:34:41 GMT
RUN Install update 1809-amd64
# Wed, 14 Apr 2021 12:09:21 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 14 Apr 2021 21:28:41 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/traefik/traefik/releases/download/v2.4.8/traefik_v2.4.8_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Wed, 14 Apr 2021 21:28:43 GMT
EXPOSE 80
# Wed, 14 Apr 2021 21:28:44 GMT
ENTRYPOINT ["/traefik"]
# Wed, 14 Apr 2021 21:28:45 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.4.8 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:399f118dfaa9a753e98d128238b944432c7bcabea88a2998a6efbbece28ed303`  
		Size: 751.4 MB (751421005 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:106dbf3373fce4f0ba5e00ad54824c597f2894605fa7d8ef446ad7ea3b97449f`  
		Last Modified: Wed, 14 Apr 2021 12:58:04 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a93cd244b1a7725d26281629f3d234056508569c464f5dea5b03ccbde91bb0f`  
		Last Modified: Wed, 14 Apr 2021 21:30:37 GMT  
		Size: 29.7 MB (29729029 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f7bb23c17022bf3359394806bf3c61d486089608895251ff7a5acfd7ad96a9a`  
		Last Modified: Wed, 14 Apr 2021 21:30:28 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb84fdded1774834fd927e9a9f74098955381bfeb1991c90d23188e9f2d4bf95`  
		Last Modified: Wed, 14 Apr 2021 21:30:27 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46b1c96a0690beee17c07772a87933a00a71ff757191a2e22ddb4b54488a8000`  
		Last Modified: Wed, 14 Apr 2021 21:30:27 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:latest`

```console
$ docker pull traefik@sha256:af1617e167e8a6554b5e75c1fd759c68887b890be715afa5f36d9ac467410d45
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:latest` - linux; amd64

```console
$ docker pull traefik@sha256:4e2da005d39daa3823c6930cfb4ff5eb8d75be3679a2173489d8579e655be4be
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.8 MB (27828337 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:deaf4b1027ed4bce7d3a15a22a7ff5f5fab274bffde1709ae85e93f15085ad98`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:56 GMT
ADD file:282b9d56236cae29600bf8b698cb0a865ab17db7beea0be6870f9de63e7d4f80 in / 
# Wed, 14 Apr 2021 19:19:56 GMT
CMD ["/bin/sh"]
# Thu, 15 Apr 2021 03:04:42 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 15 Apr 2021 03:04:47 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.4.8/traefik_v2.4.8_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 15 Apr 2021 03:04:48 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 15 Apr 2021 03:04:48 GMT
EXPOSE 80
# Thu, 15 Apr 2021 03:04:48 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 15 Apr 2021 03:04:49 GMT
CMD ["traefik"]
# Thu, 15 Apr 2021 03:04:49 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.4.8 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:ddad3d7c1e96adf9153f8921a7c9790f880a390163df453be1566e9ef0d546e0`  
		Last Modified: Wed, 14 Apr 2021 19:21:03 GMT  
		Size: 2.8 MB (2816246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f6722e60c2f6c55424dadebe886f88ba1b903df075b00048427439abb91b85a`  
		Last Modified: Thu, 15 Apr 2021 03:05:57 GMT  
		Size: 674.2 KB (674210 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acb62688737133737535c58e692b79b70843447464a3760d37d1d65c33fa1e5c`  
		Last Modified: Thu, 15 Apr 2021 03:06:03 GMT  
		Size: 24.3 MB (24337513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebb6d79f94aac9a1ec9746826d0fd58ea98a05df8f5ed882819626db57909331`  
		Last Modified: Thu, 15 Apr 2021 03:05:57 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:latest` - linux; arm variant v6

```console
$ docker pull traefik@sha256:445ec88018c03307101e734adfd8425f4da87e9ffd5d83b1e5fb512d280df5df
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.0 MB (26025735 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9a68d5d0d7cdf26c5ef8132873c04d3e8cc92b65cd6ad0af323361a5c222c57f`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 31 Mar 2021 17:19:20 GMT
ADD file:15a1f9d3700deb648f0b3701afebc97ff28eb30d1b55e18dc9c696a9dd5c8e36 in / 
# Wed, 31 Mar 2021 17:19:21 GMT
CMD ["/bin/sh"]
# Thu, 01 Apr 2021 03:52:35 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 01 Apr 2021 03:52:43 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.4.8/traefik_v2.4.8_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 01 Apr 2021 03:52:44 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 01 Apr 2021 03:52:45 GMT
EXPOSE 80
# Thu, 01 Apr 2021 03:52:47 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 01 Apr 2021 03:52:48 GMT
CMD ["traefik"]
# Thu, 01 Apr 2021 03:52:50 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.4.8 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:ac95243af174972febc49043f62f7b952a0c610e59b55ac4133f442e399e8729`  
		Last Modified: Wed, 31 Mar 2021 17:20:17 GMT  
		Size: 2.6 MB (2621248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25173f2bf7681888ff03bae0a793dcd2a8124175d360f999d21081483f90f181`  
		Last Modified: Thu, 01 Apr 2021 03:54:34 GMT  
		Size: 677.0 KB (677016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9546526ac0315b3d34e7f88f707fb5355cffd936afb2e80198eff85c6524a05`  
		Last Modified: Thu, 01 Apr 2021 03:54:41 GMT  
		Size: 22.7 MB (22727103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ddd0b0952f4a6439010368b09c4bee68dd82bad0c47ff2a4a3a0b8ce6a2c498`  
		Last Modified: Thu, 01 Apr 2021 03:54:33 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:latest` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:edd78c8c05d3050cbd62e00de1575597f2a1c628fd5faefecb0d8b20c35d7ba9
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.5 MB (25475489 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:19eb3704549293128f6d623b5a417a6cf34b01a797b4e0bf36dee8ef8f255e71`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 31 Mar 2021 17:22:02 GMT
ADD file:174ba1b913c5cf549fcdfc259e8e3aa8f49cea660865fd54b8aacb430602a783 in / 
# Wed, 31 Mar 2021 17:22:03 GMT
CMD ["/bin/sh"]
# Thu, 01 Apr 2021 16:15:15 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 01 Apr 2021 16:15:20 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.4.8/traefik_v2.4.8_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 01 Apr 2021 16:15:22 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 01 Apr 2021 16:15:23 GMT
EXPOSE 80
# Thu, 01 Apr 2021 16:15:23 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 01 Apr 2021 16:15:24 GMT
CMD ["traefik"]
# Thu, 01 Apr 2021 16:15:25 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.4.8 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:a3cf95b55367cb73f51318ee9c854def347373482336709ca1882a5d4c20b7c7`  
		Last Modified: Wed, 31 Mar 2021 17:23:00 GMT  
		Size: 2.7 MB (2725871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e08c5532ded8a461bb2539065ec0daf26ce2ecfed811ad86719ad11c964ab658`  
		Last Modified: Thu, 01 Apr 2021 16:17:57 GMT  
		Size: 675.5 KB (675530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:664cdd830c93e0170df8d4ed17b45f260ee577dcfb6db4d48f6e009b108ff81d`  
		Last Modified: Thu, 01 Apr 2021 16:18:03 GMT  
		Size: 22.1 MB (22073720 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91bdc2d37fb1c66af3a73e5fff4790dcfa4572a7fd25779591f80bd086c718df`  
		Last Modified: Thu, 01 Apr 2021 16:17:57 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:livarot`

```console
$ docker pull traefik@sha256:af1617e167e8a6554b5e75c1fd759c68887b890be715afa5f36d9ac467410d45
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:livarot` - linux; amd64

```console
$ docker pull traefik@sha256:4e2da005d39daa3823c6930cfb4ff5eb8d75be3679a2173489d8579e655be4be
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.8 MB (27828337 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:deaf4b1027ed4bce7d3a15a22a7ff5f5fab274bffde1709ae85e93f15085ad98`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:56 GMT
ADD file:282b9d56236cae29600bf8b698cb0a865ab17db7beea0be6870f9de63e7d4f80 in / 
# Wed, 14 Apr 2021 19:19:56 GMT
CMD ["/bin/sh"]
# Thu, 15 Apr 2021 03:04:42 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 15 Apr 2021 03:04:47 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.4.8/traefik_v2.4.8_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 15 Apr 2021 03:04:48 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 15 Apr 2021 03:04:48 GMT
EXPOSE 80
# Thu, 15 Apr 2021 03:04:48 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 15 Apr 2021 03:04:49 GMT
CMD ["traefik"]
# Thu, 15 Apr 2021 03:04:49 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.4.8 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:ddad3d7c1e96adf9153f8921a7c9790f880a390163df453be1566e9ef0d546e0`  
		Last Modified: Wed, 14 Apr 2021 19:21:03 GMT  
		Size: 2.8 MB (2816246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f6722e60c2f6c55424dadebe886f88ba1b903df075b00048427439abb91b85a`  
		Last Modified: Thu, 15 Apr 2021 03:05:57 GMT  
		Size: 674.2 KB (674210 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acb62688737133737535c58e692b79b70843447464a3760d37d1d65c33fa1e5c`  
		Last Modified: Thu, 15 Apr 2021 03:06:03 GMT  
		Size: 24.3 MB (24337513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebb6d79f94aac9a1ec9746826d0fd58ea98a05df8f5ed882819626db57909331`  
		Last Modified: Thu, 15 Apr 2021 03:05:57 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:livarot` - linux; arm variant v6

```console
$ docker pull traefik@sha256:445ec88018c03307101e734adfd8425f4da87e9ffd5d83b1e5fb512d280df5df
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.0 MB (26025735 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9a68d5d0d7cdf26c5ef8132873c04d3e8cc92b65cd6ad0af323361a5c222c57f`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 31 Mar 2021 17:19:20 GMT
ADD file:15a1f9d3700deb648f0b3701afebc97ff28eb30d1b55e18dc9c696a9dd5c8e36 in / 
# Wed, 31 Mar 2021 17:19:21 GMT
CMD ["/bin/sh"]
# Thu, 01 Apr 2021 03:52:35 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 01 Apr 2021 03:52:43 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.4.8/traefik_v2.4.8_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 01 Apr 2021 03:52:44 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 01 Apr 2021 03:52:45 GMT
EXPOSE 80
# Thu, 01 Apr 2021 03:52:47 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 01 Apr 2021 03:52:48 GMT
CMD ["traefik"]
# Thu, 01 Apr 2021 03:52:50 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.4.8 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:ac95243af174972febc49043f62f7b952a0c610e59b55ac4133f442e399e8729`  
		Last Modified: Wed, 31 Mar 2021 17:20:17 GMT  
		Size: 2.6 MB (2621248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25173f2bf7681888ff03bae0a793dcd2a8124175d360f999d21081483f90f181`  
		Last Modified: Thu, 01 Apr 2021 03:54:34 GMT  
		Size: 677.0 KB (677016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9546526ac0315b3d34e7f88f707fb5355cffd936afb2e80198eff85c6524a05`  
		Last Modified: Thu, 01 Apr 2021 03:54:41 GMT  
		Size: 22.7 MB (22727103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ddd0b0952f4a6439010368b09c4bee68dd82bad0c47ff2a4a3a0b8ce6a2c498`  
		Last Modified: Thu, 01 Apr 2021 03:54:33 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:livarot` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:edd78c8c05d3050cbd62e00de1575597f2a1c628fd5faefecb0d8b20c35d7ba9
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.5 MB (25475489 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:19eb3704549293128f6d623b5a417a6cf34b01a797b4e0bf36dee8ef8f255e71`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 31 Mar 2021 17:22:02 GMT
ADD file:174ba1b913c5cf549fcdfc259e8e3aa8f49cea660865fd54b8aacb430602a783 in / 
# Wed, 31 Mar 2021 17:22:03 GMT
CMD ["/bin/sh"]
# Thu, 01 Apr 2021 16:15:15 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 01 Apr 2021 16:15:20 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.4.8/traefik_v2.4.8_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 01 Apr 2021 16:15:22 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 01 Apr 2021 16:15:23 GMT
EXPOSE 80
# Thu, 01 Apr 2021 16:15:23 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 01 Apr 2021 16:15:24 GMT
CMD ["traefik"]
# Thu, 01 Apr 2021 16:15:25 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.4.8 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:a3cf95b55367cb73f51318ee9c854def347373482336709ca1882a5d4c20b7c7`  
		Last Modified: Wed, 31 Mar 2021 17:23:00 GMT  
		Size: 2.7 MB (2725871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e08c5532ded8a461bb2539065ec0daf26ce2ecfed811ad86719ad11c964ab658`  
		Last Modified: Thu, 01 Apr 2021 16:17:57 GMT  
		Size: 675.5 KB (675530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:664cdd830c93e0170df8d4ed17b45f260ee577dcfb6db4d48f6e009b108ff81d`  
		Last Modified: Thu, 01 Apr 2021 16:18:03 GMT  
		Size: 22.1 MB (22073720 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91bdc2d37fb1c66af3a73e5fff4790dcfa4572a7fd25779591f80bd086c718df`  
		Last Modified: Thu, 01 Apr 2021 16:17:57 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:livarot-windowsservercore-1809`

```console
$ docker pull traefik@sha256:a469fcdb7481c955407299e937c5b6cb5c203f6d7cc71c76932b0f41594ee652
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1879; amd64

### `traefik:livarot-windowsservercore-1809` - windows version 10.0.17763.1879; amd64

```console
$ docker pull traefik@sha256:0fda36d6a58507d81a2c34a79738e3e19ab72b1c3f63316fb0ea4505eb500b09
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2499488628 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3650b9ad832bb235bd53c735995b7542b8bf3dd3dd4cdd9a82e38c5ff8d23c44`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 09 Apr 2021 20:34:41 GMT
RUN Install update 1809-amd64
# Wed, 14 Apr 2021 12:09:21 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 14 Apr 2021 21:28:41 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/traefik/traefik/releases/download/v2.4.8/traefik_v2.4.8_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Wed, 14 Apr 2021 21:28:43 GMT
EXPOSE 80
# Wed, 14 Apr 2021 21:28:44 GMT
ENTRYPOINT ["/traefik"]
# Wed, 14 Apr 2021 21:28:45 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.4.8 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:399f118dfaa9a753e98d128238b944432c7bcabea88a2998a6efbbece28ed303`  
		Size: 751.4 MB (751421005 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:106dbf3373fce4f0ba5e00ad54824c597f2894605fa7d8ef446ad7ea3b97449f`  
		Last Modified: Wed, 14 Apr 2021 12:58:04 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a93cd244b1a7725d26281629f3d234056508569c464f5dea5b03ccbde91bb0f`  
		Last Modified: Wed, 14 Apr 2021 21:30:37 GMT  
		Size: 29.7 MB (29729029 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f7bb23c17022bf3359394806bf3c61d486089608895251ff7a5acfd7ad96a9a`  
		Last Modified: Wed, 14 Apr 2021 21:30:28 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb84fdded1774834fd927e9a9f74098955381bfeb1991c90d23188e9f2d4bf95`  
		Last Modified: Wed, 14 Apr 2021 21:30:27 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46b1c96a0690beee17c07772a87933a00a71ff757191a2e22ddb4b54488a8000`  
		Last Modified: Wed, 14 Apr 2021 21:30:27 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:maroilles`

```console
$ docker pull traefik@sha256:5e2dfb5243ae97ddb7c959addb389643a1c9787d813630f23684eff53b4775dd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:maroilles` - linux; amd64

```console
$ docker pull traefik@sha256:353827cc14120a14b1eccbb2714039763d9cefc284213b53d82d14e110fadc39
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.1 MB (18124621 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2a2126389e0b0dbd13da033d79636b0f0626d73f1a6da0935ce6ce9eccae112a`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Tue, 09 Mar 2021 01:32:48 GMT
COPY file:cd6264d9a7514a8fbc3eb7b400566d36178794d2b757959812cc3abc6f13a97b in /etc/ssl/certs/ 
# Tue, 09 Mar 2021 01:32:49 GMT
COPY dir:379603788862c2a6c57432d70b0a67f561fe00310e1b958c9ecf85381b1c9cd9 in /usr/share/ 
# Thu, 08 Apr 2021 20:07:38 GMT
COPY file:bc0b1c0235bda22a75d2ef00a982989cdf1da3240f077584bca5c6b560a4c13a in / 
# Thu, 08 Apr 2021 20:07:38 GMT
EXPOSE 80
# Thu, 08 Apr 2021 20:07:39 GMT
VOLUME [/tmp]
# Thu, 08 Apr 2021 20:07:39 GMT
ENTRYPOINT ["/traefik"]
# Thu, 08 Apr 2021 20:07:40 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.30 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:53f50c15495c67f391a5750288681a589b19a39c4b78e7ebc0934606cc3d0bc3`  
		Last Modified: Tue, 09 Mar 2021 01:33:59 GMT  
		Size: 130.9 KB (130870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89c044b3636c16c5ab8fc96a04f320c9f97ea23aaffec9adb2d8f20ebaef93f3`  
		Last Modified: Tue, 09 Mar 2021 01:33:59 GMT  
		Size: 308.8 KB (308823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2eb3d26b40720e4da5cbeb15193c698565e23551a24cc4abc4acd1b7de414279`  
		Last Modified: Thu, 08 Apr 2021 20:08:34 GMT  
		Size: 17.7 MB (17684928 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:maroilles` - linux; arm variant v6

```console
$ docker pull traefik@sha256:5c7347d0c834b82833b1d344eb84d8491f4afff9c180aad1e287bfb28612d5ec
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.0 MB (16956529 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:90f7d007bf10f706fa796c9f4cc9ad283fd98d0a8ae604e72748f96e43aa9565`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Thu, 17 Dec 2020 00:26:47 GMT
COPY file:cd6264d9a7514a8fbc3eb7b400566d36178794d2b757959812cc3abc6f13a97b in /etc/ssl/certs/ 
# Wed, 24 Feb 2021 23:34:19 GMT
COPY dir:379603788862c2a6c57432d70b0a67f561fe00310e1b958c9ecf85381b1c9cd9 in /usr/share/ 
# Thu, 08 Apr 2021 19:28:36 GMT
COPY file:440b6b1ebd389a2397ffb187ded4c85dcf37b7284d94c693b0b603d51247c683 in / 
# Thu, 08 Apr 2021 19:28:38 GMT
EXPOSE 80
# Thu, 08 Apr 2021 19:28:39 GMT
VOLUME [/tmp]
# Thu, 08 Apr 2021 19:28:41 GMT
ENTRYPOINT ["/traefik"]
# Thu, 08 Apr 2021 19:28:42 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.30 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:26c529e82b09c489524aa4f787754320793a95eb7aa7eaf306c517b76818ec25`  
		Last Modified: Thu, 17 Dec 2020 00:28:41 GMT  
		Size: 130.9 KB (130873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e74b8526f2bdaa522f470d66d09f7ebbe9a1f060ce049ac91c0f7aad153e1be`  
		Last Modified: Wed, 24 Feb 2021 23:36:10 GMT  
		Size: 308.9 KB (308855 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba2277a3749c5a6efdb45bc2ff1ce8c98de01e3225fb4b0df258523fe93391c5`  
		Last Modified: Thu, 08 Apr 2021 19:29:27 GMT  
		Size: 16.5 MB (16516801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:maroilles` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:9d2ec3215411977686c39214b6a14e65eb82434ab9652451f8dc2ce54fe9ca0a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.5 MB (16533607 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:df27dd67357d586d32809c5642158f6bdccbce6f28664694b215bd5b2cb6ee99`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Thu, 17 Dec 2020 00:27:56 GMT
COPY file:cd6264d9a7514a8fbc3eb7b400566d36178794d2b757959812cc3abc6f13a97b in /etc/ssl/certs/ 
# Thu, 25 Feb 2021 04:23:55 GMT
COPY dir:379603788862c2a6c57432d70b0a67f561fe00310e1b958c9ecf85381b1c9cd9 in /usr/share/ 
# Thu, 08 Apr 2021 20:39:22 GMT
COPY file:6fdd60dc35db1c19a5de5ed8b57f159a6e121ba0f1ddb3e48a6e185da99f8cca in / 
# Thu, 08 Apr 2021 20:39:23 GMT
EXPOSE 80
# Thu, 08 Apr 2021 20:39:24 GMT
VOLUME [/tmp]
# Thu, 08 Apr 2021 20:39:25 GMT
ENTRYPOINT ["/traefik"]
# Thu, 08 Apr 2021 20:39:26 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.30 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:7dccf22d113d483cac839141f2028cbf6ac2e0c6aa4a1716c5e7b575b162028c`  
		Last Modified: Thu, 17 Dec 2020 00:29:55 GMT  
		Size: 130.9 KB (130873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41f74910073ee331bfbff1c3d20a2d29270f713f515ccee693e566b927d37654`  
		Last Modified: Thu, 25 Feb 2021 04:25:12 GMT  
		Size: 308.8 KB (308831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db3a97f2585cdbe5ac39667c253a77c35e2cbc755c2d788f76a1b2fd02413e51`  
		Last Modified: Thu, 08 Apr 2021 20:40:11 GMT  
		Size: 16.1 MB (16093903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:maroilles-alpine`

```console
$ docker pull traefik@sha256:bb221da9b5335ecac917502708411306ad6ea0b720f9ee0c723451a83255fda1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:maroilles-alpine` - linux; amd64

```console
$ docker pull traefik@sha256:5e1e280e8e56520c8ebc11425f2c9fe66c9fae4714d65833d7f15c40fde8fb80
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **21.2 MB (21175700 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:55847f6ab3e15d3f6304ec3271273146b44942dff17926a61366afbdf6736671`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:56 GMT
ADD file:282b9d56236cae29600bf8b698cb0a865ab17db7beea0be6870f9de63e7d4f80 in / 
# Wed, 14 Apr 2021 19:19:56 GMT
CMD ["/bin/sh"]
# Thu, 15 Apr 2021 03:04:42 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 15 Apr 2021 03:04:59 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/traefik/traefik/releases/download/v1.7.30/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Thu, 15 Apr 2021 03:05:00 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 15 Apr 2021 03:05:00 GMT
EXPOSE 80
# Thu, 15 Apr 2021 03:05:00 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 15 Apr 2021 03:05:01 GMT
CMD ["traefik"]
# Thu, 15 Apr 2021 03:05:01 GMT
LABEL org.opencontainers.image.vendor=traefik org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.30 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:ddad3d7c1e96adf9153f8921a7c9790f880a390163df453be1566e9ef0d546e0`  
		Last Modified: Wed, 14 Apr 2021 19:21:03 GMT  
		Size: 2.8 MB (2816246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f6722e60c2f6c55424dadebe886f88ba1b903df075b00048427439abb91b85a`  
		Last Modified: Thu, 15 Apr 2021 03:05:57 GMT  
		Size: 674.2 KB (674210 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e40cdaabf18912622322046bb5eeda16c1ac513a094389e9b12b33ff02abb2c`  
		Last Modified: Thu, 15 Apr 2021 03:06:32 GMT  
		Size: 17.7 MB (17684875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1ec9b7bad03eb2d44d70526dbd5478e8ee4043e8445168201605f71fafbb22e`  
		Last Modified: Thu, 15 Apr 2021 03:06:25 GMT  
		Size: 369.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:maroilles-alpine` - linux; arm variant v6

```console
$ docker pull traefik@sha256:01eccfad104e020c243676c64ede0b15f789bdb44c72504534412a3751b595b6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **19.8 MB (19815547 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e2c542dcb63b74c456178e52089c32d41929581f8c12124065b7df092764d685`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 31 Mar 2021 17:19:20 GMT
ADD file:15a1f9d3700deb648f0b3701afebc97ff28eb30d1b55e18dc9c696a9dd5c8e36 in / 
# Wed, 31 Mar 2021 17:19:21 GMT
CMD ["/bin/sh"]
# Thu, 01 Apr 2021 03:52:35 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 08 Apr 2021 19:28:18 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/traefik/traefik/releases/download/v1.7.30/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Thu, 08 Apr 2021 19:28:19 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 08 Apr 2021 19:28:20 GMT
EXPOSE 80
# Thu, 08 Apr 2021 19:28:21 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 08 Apr 2021 19:28:22 GMT
CMD ["traefik"]
# Thu, 08 Apr 2021 19:28:23 GMT
LABEL org.opencontainers.image.vendor=traefik org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.30 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:ac95243af174972febc49043f62f7b952a0c610e59b55ac4133f442e399e8729`  
		Last Modified: Wed, 31 Mar 2021 17:20:17 GMT  
		Size: 2.6 MB (2621248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25173f2bf7681888ff03bae0a793dcd2a8124175d360f999d21081483f90f181`  
		Last Modified: Thu, 01 Apr 2021 03:54:34 GMT  
		Size: 677.0 KB (677016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59eb9988c4b9b573a94c2aef256f275f37bc80f4537429e21a07866e21c30c15`  
		Last Modified: Thu, 08 Apr 2021 19:29:12 GMT  
		Size: 16.5 MB (16516915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43e60f188a205da97f1f59c9e979da57a3f96fcdd8a7b677d798138f433a8fca`  
		Last Modified: Thu, 08 Apr 2021 19:29:06 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:maroilles-alpine` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:0cf15008333d1cc2b7907ebead2b805754d3fd9a35ee0b5ef8f52d26e69d9e35
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **19.5 MB (19495771 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7f9ab0b3ea9162be9ba4e2fedca5164d4769d09ad5492d8df197d742139defbb`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 31 Mar 2021 17:22:02 GMT
ADD file:174ba1b913c5cf549fcdfc259e8e3aa8f49cea660865fd54b8aacb430602a783 in / 
# Wed, 31 Mar 2021 17:22:03 GMT
CMD ["/bin/sh"]
# Thu, 01 Apr 2021 16:15:15 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 08 Apr 2021 20:39:00 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/traefik/traefik/releases/download/v1.7.30/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Thu, 08 Apr 2021 20:39:01 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 08 Apr 2021 20:39:02 GMT
EXPOSE 80
# Thu, 08 Apr 2021 20:39:03 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 08 Apr 2021 20:39:04 GMT
CMD ["traefik"]
# Thu, 08 Apr 2021 20:39:05 GMT
LABEL org.opencontainers.image.vendor=traefik org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.30 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:a3cf95b55367cb73f51318ee9c854def347373482336709ca1882a5d4c20b7c7`  
		Last Modified: Wed, 31 Mar 2021 17:23:00 GMT  
		Size: 2.7 MB (2725871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e08c5532ded8a461bb2539065ec0daf26ce2ecfed811ad86719ad11c964ab658`  
		Last Modified: Thu, 01 Apr 2021 16:17:57 GMT  
		Size: 675.5 KB (675530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bdb060704f0ed88ad3c7606d012c734450f30bd6d4fdfe4afe65a3109473985`  
		Last Modified: Thu, 08 Apr 2021 20:39:54 GMT  
		Size: 16.1 MB (16094002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b924f9ea1253bff83db6941fc95ed9248766194e0712f66bde5fa5f8d89cfe0`  
		Last Modified: Thu, 08 Apr 2021 20:39:49 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:maroilles-windowsservercore-1809`

```console
$ docker pull traefik@sha256:733a8c228d615ebf548385487b66c7b3fdd7699c1c9f7fec1cfa4c71feeb4785
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1879; amd64

### `traefik:maroilles-windowsservercore-1809` - windows version 10.0.17763.1879; amd64

```console
$ docker pull traefik@sha256:e7f8b8eee97e1609e89c4a19e3f7f530a33ca76b26196d1c6bc927eca28645c3
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2492758593 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8bb83271e02abc3f1a599c84de304ca6c4f9ceab42a58cf154675cad4c8e761b`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 09 Apr 2021 20:34:41 GMT
RUN Install update 1809-amd64
# Wed, 14 Apr 2021 12:09:21 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 14 Apr 2021 21:29:52 GMT
RUN Invoke-WebRequest     -Uri "https://github.com/traefik/traefik/releases/download/v1.7.30/traefik_windows-amd64.exe"     -OutFile "/traefik.exe"
# Wed, 14 Apr 2021 21:29:54 GMT
EXPOSE 80
# Wed, 14 Apr 2021 21:29:55 GMT
ENTRYPOINT ["/traefik"]
# Wed, 14 Apr 2021 21:29:56 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.30 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:399f118dfaa9a753e98d128238b944432c7bcabea88a2998a6efbbece28ed303`  
		Size: 751.4 MB (751421005 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:106dbf3373fce4f0ba5e00ad54824c597f2894605fa7d8ef446ad7ea3b97449f`  
		Last Modified: Wed, 14 Apr 2021 12:58:04 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:203e1506701de3ad9fca12951ea83f903d0bdc8628f20a7bfb3d77a713a5ed52`  
		Last Modified: Wed, 14 Apr 2021 21:31:15 GMT  
		Size: 23.0 MB (22998990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2b11339a17c4a4101817c0f6ddc3f3453e39f1c052aedf3f0e9cdb0ffc84365`  
		Last Modified: Wed, 14 Apr 2021 21:31:08 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07482932f6ca5c824d683ca413e9ef96f6aa833fc867c4d614428803b25d6143`  
		Last Modified: Wed, 14 Apr 2021 21:31:08 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f776de6cf2f2359d3f8ccf8e44387cbe850d86e91540ddd4253809940c7afb76`  
		Last Modified: Wed, 14 Apr 2021 21:31:08 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v1.7`

```console
$ docker pull traefik@sha256:5e2dfb5243ae97ddb7c959addb389643a1c9787d813630f23684eff53b4775dd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:v1.7` - linux; amd64

```console
$ docker pull traefik@sha256:353827cc14120a14b1eccbb2714039763d9cefc284213b53d82d14e110fadc39
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.1 MB (18124621 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2a2126389e0b0dbd13da033d79636b0f0626d73f1a6da0935ce6ce9eccae112a`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Tue, 09 Mar 2021 01:32:48 GMT
COPY file:cd6264d9a7514a8fbc3eb7b400566d36178794d2b757959812cc3abc6f13a97b in /etc/ssl/certs/ 
# Tue, 09 Mar 2021 01:32:49 GMT
COPY dir:379603788862c2a6c57432d70b0a67f561fe00310e1b958c9ecf85381b1c9cd9 in /usr/share/ 
# Thu, 08 Apr 2021 20:07:38 GMT
COPY file:bc0b1c0235bda22a75d2ef00a982989cdf1da3240f077584bca5c6b560a4c13a in / 
# Thu, 08 Apr 2021 20:07:38 GMT
EXPOSE 80
# Thu, 08 Apr 2021 20:07:39 GMT
VOLUME [/tmp]
# Thu, 08 Apr 2021 20:07:39 GMT
ENTRYPOINT ["/traefik"]
# Thu, 08 Apr 2021 20:07:40 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.30 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:53f50c15495c67f391a5750288681a589b19a39c4b78e7ebc0934606cc3d0bc3`  
		Last Modified: Tue, 09 Mar 2021 01:33:59 GMT  
		Size: 130.9 KB (130870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89c044b3636c16c5ab8fc96a04f320c9f97ea23aaffec9adb2d8f20ebaef93f3`  
		Last Modified: Tue, 09 Mar 2021 01:33:59 GMT  
		Size: 308.8 KB (308823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2eb3d26b40720e4da5cbeb15193c698565e23551a24cc4abc4acd1b7de414279`  
		Last Modified: Thu, 08 Apr 2021 20:08:34 GMT  
		Size: 17.7 MB (17684928 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v1.7` - linux; arm variant v6

```console
$ docker pull traefik@sha256:5c7347d0c834b82833b1d344eb84d8491f4afff9c180aad1e287bfb28612d5ec
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.0 MB (16956529 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:90f7d007bf10f706fa796c9f4cc9ad283fd98d0a8ae604e72748f96e43aa9565`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Thu, 17 Dec 2020 00:26:47 GMT
COPY file:cd6264d9a7514a8fbc3eb7b400566d36178794d2b757959812cc3abc6f13a97b in /etc/ssl/certs/ 
# Wed, 24 Feb 2021 23:34:19 GMT
COPY dir:379603788862c2a6c57432d70b0a67f561fe00310e1b958c9ecf85381b1c9cd9 in /usr/share/ 
# Thu, 08 Apr 2021 19:28:36 GMT
COPY file:440b6b1ebd389a2397ffb187ded4c85dcf37b7284d94c693b0b603d51247c683 in / 
# Thu, 08 Apr 2021 19:28:38 GMT
EXPOSE 80
# Thu, 08 Apr 2021 19:28:39 GMT
VOLUME [/tmp]
# Thu, 08 Apr 2021 19:28:41 GMT
ENTRYPOINT ["/traefik"]
# Thu, 08 Apr 2021 19:28:42 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.30 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:26c529e82b09c489524aa4f787754320793a95eb7aa7eaf306c517b76818ec25`  
		Last Modified: Thu, 17 Dec 2020 00:28:41 GMT  
		Size: 130.9 KB (130873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e74b8526f2bdaa522f470d66d09f7ebbe9a1f060ce049ac91c0f7aad153e1be`  
		Last Modified: Wed, 24 Feb 2021 23:36:10 GMT  
		Size: 308.9 KB (308855 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba2277a3749c5a6efdb45bc2ff1ce8c98de01e3225fb4b0df258523fe93391c5`  
		Last Modified: Thu, 08 Apr 2021 19:29:27 GMT  
		Size: 16.5 MB (16516801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v1.7` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:9d2ec3215411977686c39214b6a14e65eb82434ab9652451f8dc2ce54fe9ca0a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.5 MB (16533607 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:df27dd67357d586d32809c5642158f6bdccbce6f28664694b215bd5b2cb6ee99`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Thu, 17 Dec 2020 00:27:56 GMT
COPY file:cd6264d9a7514a8fbc3eb7b400566d36178794d2b757959812cc3abc6f13a97b in /etc/ssl/certs/ 
# Thu, 25 Feb 2021 04:23:55 GMT
COPY dir:379603788862c2a6c57432d70b0a67f561fe00310e1b958c9ecf85381b1c9cd9 in /usr/share/ 
# Thu, 08 Apr 2021 20:39:22 GMT
COPY file:6fdd60dc35db1c19a5de5ed8b57f159a6e121ba0f1ddb3e48a6e185da99f8cca in / 
# Thu, 08 Apr 2021 20:39:23 GMT
EXPOSE 80
# Thu, 08 Apr 2021 20:39:24 GMT
VOLUME [/tmp]
# Thu, 08 Apr 2021 20:39:25 GMT
ENTRYPOINT ["/traefik"]
# Thu, 08 Apr 2021 20:39:26 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.30 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:7dccf22d113d483cac839141f2028cbf6ac2e0c6aa4a1716c5e7b575b162028c`  
		Last Modified: Thu, 17 Dec 2020 00:29:55 GMT  
		Size: 130.9 KB (130873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41f74910073ee331bfbff1c3d20a2d29270f713f515ccee693e566b927d37654`  
		Last Modified: Thu, 25 Feb 2021 04:25:12 GMT  
		Size: 308.8 KB (308831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db3a97f2585cdbe5ac39667c253a77c35e2cbc755c2d788f76a1b2fd02413e51`  
		Last Modified: Thu, 08 Apr 2021 20:40:11 GMT  
		Size: 16.1 MB (16093903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v1.7-alpine`

```console
$ docker pull traefik@sha256:bb221da9b5335ecac917502708411306ad6ea0b720f9ee0c723451a83255fda1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:v1.7-alpine` - linux; amd64

```console
$ docker pull traefik@sha256:5e1e280e8e56520c8ebc11425f2c9fe66c9fae4714d65833d7f15c40fde8fb80
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **21.2 MB (21175700 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:55847f6ab3e15d3f6304ec3271273146b44942dff17926a61366afbdf6736671`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:56 GMT
ADD file:282b9d56236cae29600bf8b698cb0a865ab17db7beea0be6870f9de63e7d4f80 in / 
# Wed, 14 Apr 2021 19:19:56 GMT
CMD ["/bin/sh"]
# Thu, 15 Apr 2021 03:04:42 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 15 Apr 2021 03:04:59 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/traefik/traefik/releases/download/v1.7.30/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Thu, 15 Apr 2021 03:05:00 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 15 Apr 2021 03:05:00 GMT
EXPOSE 80
# Thu, 15 Apr 2021 03:05:00 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 15 Apr 2021 03:05:01 GMT
CMD ["traefik"]
# Thu, 15 Apr 2021 03:05:01 GMT
LABEL org.opencontainers.image.vendor=traefik org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.30 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:ddad3d7c1e96adf9153f8921a7c9790f880a390163df453be1566e9ef0d546e0`  
		Last Modified: Wed, 14 Apr 2021 19:21:03 GMT  
		Size: 2.8 MB (2816246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f6722e60c2f6c55424dadebe886f88ba1b903df075b00048427439abb91b85a`  
		Last Modified: Thu, 15 Apr 2021 03:05:57 GMT  
		Size: 674.2 KB (674210 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e40cdaabf18912622322046bb5eeda16c1ac513a094389e9b12b33ff02abb2c`  
		Last Modified: Thu, 15 Apr 2021 03:06:32 GMT  
		Size: 17.7 MB (17684875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1ec9b7bad03eb2d44d70526dbd5478e8ee4043e8445168201605f71fafbb22e`  
		Last Modified: Thu, 15 Apr 2021 03:06:25 GMT  
		Size: 369.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v1.7-alpine` - linux; arm variant v6

```console
$ docker pull traefik@sha256:01eccfad104e020c243676c64ede0b15f789bdb44c72504534412a3751b595b6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **19.8 MB (19815547 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e2c542dcb63b74c456178e52089c32d41929581f8c12124065b7df092764d685`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 31 Mar 2021 17:19:20 GMT
ADD file:15a1f9d3700deb648f0b3701afebc97ff28eb30d1b55e18dc9c696a9dd5c8e36 in / 
# Wed, 31 Mar 2021 17:19:21 GMT
CMD ["/bin/sh"]
# Thu, 01 Apr 2021 03:52:35 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 08 Apr 2021 19:28:18 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/traefik/traefik/releases/download/v1.7.30/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Thu, 08 Apr 2021 19:28:19 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 08 Apr 2021 19:28:20 GMT
EXPOSE 80
# Thu, 08 Apr 2021 19:28:21 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 08 Apr 2021 19:28:22 GMT
CMD ["traefik"]
# Thu, 08 Apr 2021 19:28:23 GMT
LABEL org.opencontainers.image.vendor=traefik org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.30 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:ac95243af174972febc49043f62f7b952a0c610e59b55ac4133f442e399e8729`  
		Last Modified: Wed, 31 Mar 2021 17:20:17 GMT  
		Size: 2.6 MB (2621248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25173f2bf7681888ff03bae0a793dcd2a8124175d360f999d21081483f90f181`  
		Last Modified: Thu, 01 Apr 2021 03:54:34 GMT  
		Size: 677.0 KB (677016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59eb9988c4b9b573a94c2aef256f275f37bc80f4537429e21a07866e21c30c15`  
		Last Modified: Thu, 08 Apr 2021 19:29:12 GMT  
		Size: 16.5 MB (16516915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43e60f188a205da97f1f59c9e979da57a3f96fcdd8a7b677d798138f433a8fca`  
		Last Modified: Thu, 08 Apr 2021 19:29:06 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v1.7-alpine` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:0cf15008333d1cc2b7907ebead2b805754d3fd9a35ee0b5ef8f52d26e69d9e35
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **19.5 MB (19495771 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7f9ab0b3ea9162be9ba4e2fedca5164d4769d09ad5492d8df197d742139defbb`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 31 Mar 2021 17:22:02 GMT
ADD file:174ba1b913c5cf549fcdfc259e8e3aa8f49cea660865fd54b8aacb430602a783 in / 
# Wed, 31 Mar 2021 17:22:03 GMT
CMD ["/bin/sh"]
# Thu, 01 Apr 2021 16:15:15 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 08 Apr 2021 20:39:00 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/traefik/traefik/releases/download/v1.7.30/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Thu, 08 Apr 2021 20:39:01 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 08 Apr 2021 20:39:02 GMT
EXPOSE 80
# Thu, 08 Apr 2021 20:39:03 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 08 Apr 2021 20:39:04 GMT
CMD ["traefik"]
# Thu, 08 Apr 2021 20:39:05 GMT
LABEL org.opencontainers.image.vendor=traefik org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.30 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:a3cf95b55367cb73f51318ee9c854def347373482336709ca1882a5d4c20b7c7`  
		Last Modified: Wed, 31 Mar 2021 17:23:00 GMT  
		Size: 2.7 MB (2725871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e08c5532ded8a461bb2539065ec0daf26ce2ecfed811ad86719ad11c964ab658`  
		Last Modified: Thu, 01 Apr 2021 16:17:57 GMT  
		Size: 675.5 KB (675530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bdb060704f0ed88ad3c7606d012c734450f30bd6d4fdfe4afe65a3109473985`  
		Last Modified: Thu, 08 Apr 2021 20:39:54 GMT  
		Size: 16.1 MB (16094002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b924f9ea1253bff83db6941fc95ed9248766194e0712f66bde5fa5f8d89cfe0`  
		Last Modified: Thu, 08 Apr 2021 20:39:49 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v1.7-windowsservercore-1809`

```console
$ docker pull traefik@sha256:733a8c228d615ebf548385487b66c7b3fdd7699c1c9f7fec1cfa4c71feeb4785
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1879; amd64

### `traefik:v1.7-windowsservercore-1809` - windows version 10.0.17763.1879; amd64

```console
$ docker pull traefik@sha256:e7f8b8eee97e1609e89c4a19e3f7f530a33ca76b26196d1c6bc927eca28645c3
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2492758593 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8bb83271e02abc3f1a599c84de304ca6c4f9ceab42a58cf154675cad4c8e761b`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 09 Apr 2021 20:34:41 GMT
RUN Install update 1809-amd64
# Wed, 14 Apr 2021 12:09:21 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 14 Apr 2021 21:29:52 GMT
RUN Invoke-WebRequest     -Uri "https://github.com/traefik/traefik/releases/download/v1.7.30/traefik_windows-amd64.exe"     -OutFile "/traefik.exe"
# Wed, 14 Apr 2021 21:29:54 GMT
EXPOSE 80
# Wed, 14 Apr 2021 21:29:55 GMT
ENTRYPOINT ["/traefik"]
# Wed, 14 Apr 2021 21:29:56 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.30 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:399f118dfaa9a753e98d128238b944432c7bcabea88a2998a6efbbece28ed303`  
		Size: 751.4 MB (751421005 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:106dbf3373fce4f0ba5e00ad54824c597f2894605fa7d8ef446ad7ea3b97449f`  
		Last Modified: Wed, 14 Apr 2021 12:58:04 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:203e1506701de3ad9fca12951ea83f903d0bdc8628f20a7bfb3d77a713a5ed52`  
		Last Modified: Wed, 14 Apr 2021 21:31:15 GMT  
		Size: 23.0 MB (22998990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2b11339a17c4a4101817c0f6ddc3f3453e39f1c052aedf3f0e9cdb0ffc84365`  
		Last Modified: Wed, 14 Apr 2021 21:31:08 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07482932f6ca5c824d683ca413e9ef96f6aa833fc867c4d614428803b25d6143`  
		Last Modified: Wed, 14 Apr 2021 21:31:08 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f776de6cf2f2359d3f8ccf8e44387cbe850d86e91540ddd4253809940c7afb76`  
		Last Modified: Wed, 14 Apr 2021 21:31:08 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v1.7.30`

```console
$ docker pull traefik@sha256:5e2dfb5243ae97ddb7c959addb389643a1c9787d813630f23684eff53b4775dd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:v1.7.30` - linux; amd64

```console
$ docker pull traefik@sha256:353827cc14120a14b1eccbb2714039763d9cefc284213b53d82d14e110fadc39
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.1 MB (18124621 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2a2126389e0b0dbd13da033d79636b0f0626d73f1a6da0935ce6ce9eccae112a`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Tue, 09 Mar 2021 01:32:48 GMT
COPY file:cd6264d9a7514a8fbc3eb7b400566d36178794d2b757959812cc3abc6f13a97b in /etc/ssl/certs/ 
# Tue, 09 Mar 2021 01:32:49 GMT
COPY dir:379603788862c2a6c57432d70b0a67f561fe00310e1b958c9ecf85381b1c9cd9 in /usr/share/ 
# Thu, 08 Apr 2021 20:07:38 GMT
COPY file:bc0b1c0235bda22a75d2ef00a982989cdf1da3240f077584bca5c6b560a4c13a in / 
# Thu, 08 Apr 2021 20:07:38 GMT
EXPOSE 80
# Thu, 08 Apr 2021 20:07:39 GMT
VOLUME [/tmp]
# Thu, 08 Apr 2021 20:07:39 GMT
ENTRYPOINT ["/traefik"]
# Thu, 08 Apr 2021 20:07:40 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.30 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:53f50c15495c67f391a5750288681a589b19a39c4b78e7ebc0934606cc3d0bc3`  
		Last Modified: Tue, 09 Mar 2021 01:33:59 GMT  
		Size: 130.9 KB (130870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89c044b3636c16c5ab8fc96a04f320c9f97ea23aaffec9adb2d8f20ebaef93f3`  
		Last Modified: Tue, 09 Mar 2021 01:33:59 GMT  
		Size: 308.8 KB (308823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2eb3d26b40720e4da5cbeb15193c698565e23551a24cc4abc4acd1b7de414279`  
		Last Modified: Thu, 08 Apr 2021 20:08:34 GMT  
		Size: 17.7 MB (17684928 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v1.7.30` - linux; arm variant v6

```console
$ docker pull traefik@sha256:5c7347d0c834b82833b1d344eb84d8491f4afff9c180aad1e287bfb28612d5ec
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.0 MB (16956529 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:90f7d007bf10f706fa796c9f4cc9ad283fd98d0a8ae604e72748f96e43aa9565`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Thu, 17 Dec 2020 00:26:47 GMT
COPY file:cd6264d9a7514a8fbc3eb7b400566d36178794d2b757959812cc3abc6f13a97b in /etc/ssl/certs/ 
# Wed, 24 Feb 2021 23:34:19 GMT
COPY dir:379603788862c2a6c57432d70b0a67f561fe00310e1b958c9ecf85381b1c9cd9 in /usr/share/ 
# Thu, 08 Apr 2021 19:28:36 GMT
COPY file:440b6b1ebd389a2397ffb187ded4c85dcf37b7284d94c693b0b603d51247c683 in / 
# Thu, 08 Apr 2021 19:28:38 GMT
EXPOSE 80
# Thu, 08 Apr 2021 19:28:39 GMT
VOLUME [/tmp]
# Thu, 08 Apr 2021 19:28:41 GMT
ENTRYPOINT ["/traefik"]
# Thu, 08 Apr 2021 19:28:42 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.30 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:26c529e82b09c489524aa4f787754320793a95eb7aa7eaf306c517b76818ec25`  
		Last Modified: Thu, 17 Dec 2020 00:28:41 GMT  
		Size: 130.9 KB (130873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e74b8526f2bdaa522f470d66d09f7ebbe9a1f060ce049ac91c0f7aad153e1be`  
		Last Modified: Wed, 24 Feb 2021 23:36:10 GMT  
		Size: 308.9 KB (308855 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba2277a3749c5a6efdb45bc2ff1ce8c98de01e3225fb4b0df258523fe93391c5`  
		Last Modified: Thu, 08 Apr 2021 19:29:27 GMT  
		Size: 16.5 MB (16516801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v1.7.30` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:9d2ec3215411977686c39214b6a14e65eb82434ab9652451f8dc2ce54fe9ca0a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.5 MB (16533607 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:df27dd67357d586d32809c5642158f6bdccbce6f28664694b215bd5b2cb6ee99`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Thu, 17 Dec 2020 00:27:56 GMT
COPY file:cd6264d9a7514a8fbc3eb7b400566d36178794d2b757959812cc3abc6f13a97b in /etc/ssl/certs/ 
# Thu, 25 Feb 2021 04:23:55 GMT
COPY dir:379603788862c2a6c57432d70b0a67f561fe00310e1b958c9ecf85381b1c9cd9 in /usr/share/ 
# Thu, 08 Apr 2021 20:39:22 GMT
COPY file:6fdd60dc35db1c19a5de5ed8b57f159a6e121ba0f1ddb3e48a6e185da99f8cca in / 
# Thu, 08 Apr 2021 20:39:23 GMT
EXPOSE 80
# Thu, 08 Apr 2021 20:39:24 GMT
VOLUME [/tmp]
# Thu, 08 Apr 2021 20:39:25 GMT
ENTRYPOINT ["/traefik"]
# Thu, 08 Apr 2021 20:39:26 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.30 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:7dccf22d113d483cac839141f2028cbf6ac2e0c6aa4a1716c5e7b575b162028c`  
		Last Modified: Thu, 17 Dec 2020 00:29:55 GMT  
		Size: 130.9 KB (130873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41f74910073ee331bfbff1c3d20a2d29270f713f515ccee693e566b927d37654`  
		Last Modified: Thu, 25 Feb 2021 04:25:12 GMT  
		Size: 308.8 KB (308831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db3a97f2585cdbe5ac39667c253a77c35e2cbc755c2d788f76a1b2fd02413e51`  
		Last Modified: Thu, 08 Apr 2021 20:40:11 GMT  
		Size: 16.1 MB (16093903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v1.7.30-alpine`

```console
$ docker pull traefik@sha256:bb221da9b5335ecac917502708411306ad6ea0b720f9ee0c723451a83255fda1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:v1.7.30-alpine` - linux; amd64

```console
$ docker pull traefik@sha256:5e1e280e8e56520c8ebc11425f2c9fe66c9fae4714d65833d7f15c40fde8fb80
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **21.2 MB (21175700 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:55847f6ab3e15d3f6304ec3271273146b44942dff17926a61366afbdf6736671`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:56 GMT
ADD file:282b9d56236cae29600bf8b698cb0a865ab17db7beea0be6870f9de63e7d4f80 in / 
# Wed, 14 Apr 2021 19:19:56 GMT
CMD ["/bin/sh"]
# Thu, 15 Apr 2021 03:04:42 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 15 Apr 2021 03:04:59 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/traefik/traefik/releases/download/v1.7.30/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Thu, 15 Apr 2021 03:05:00 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 15 Apr 2021 03:05:00 GMT
EXPOSE 80
# Thu, 15 Apr 2021 03:05:00 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 15 Apr 2021 03:05:01 GMT
CMD ["traefik"]
# Thu, 15 Apr 2021 03:05:01 GMT
LABEL org.opencontainers.image.vendor=traefik org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.30 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:ddad3d7c1e96adf9153f8921a7c9790f880a390163df453be1566e9ef0d546e0`  
		Last Modified: Wed, 14 Apr 2021 19:21:03 GMT  
		Size: 2.8 MB (2816246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f6722e60c2f6c55424dadebe886f88ba1b903df075b00048427439abb91b85a`  
		Last Modified: Thu, 15 Apr 2021 03:05:57 GMT  
		Size: 674.2 KB (674210 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e40cdaabf18912622322046bb5eeda16c1ac513a094389e9b12b33ff02abb2c`  
		Last Modified: Thu, 15 Apr 2021 03:06:32 GMT  
		Size: 17.7 MB (17684875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1ec9b7bad03eb2d44d70526dbd5478e8ee4043e8445168201605f71fafbb22e`  
		Last Modified: Thu, 15 Apr 2021 03:06:25 GMT  
		Size: 369.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v1.7.30-alpine` - linux; arm variant v6

```console
$ docker pull traefik@sha256:01eccfad104e020c243676c64ede0b15f789bdb44c72504534412a3751b595b6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **19.8 MB (19815547 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e2c542dcb63b74c456178e52089c32d41929581f8c12124065b7df092764d685`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 31 Mar 2021 17:19:20 GMT
ADD file:15a1f9d3700deb648f0b3701afebc97ff28eb30d1b55e18dc9c696a9dd5c8e36 in / 
# Wed, 31 Mar 2021 17:19:21 GMT
CMD ["/bin/sh"]
# Thu, 01 Apr 2021 03:52:35 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 08 Apr 2021 19:28:18 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/traefik/traefik/releases/download/v1.7.30/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Thu, 08 Apr 2021 19:28:19 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 08 Apr 2021 19:28:20 GMT
EXPOSE 80
# Thu, 08 Apr 2021 19:28:21 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 08 Apr 2021 19:28:22 GMT
CMD ["traefik"]
# Thu, 08 Apr 2021 19:28:23 GMT
LABEL org.opencontainers.image.vendor=traefik org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.30 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:ac95243af174972febc49043f62f7b952a0c610e59b55ac4133f442e399e8729`  
		Last Modified: Wed, 31 Mar 2021 17:20:17 GMT  
		Size: 2.6 MB (2621248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25173f2bf7681888ff03bae0a793dcd2a8124175d360f999d21081483f90f181`  
		Last Modified: Thu, 01 Apr 2021 03:54:34 GMT  
		Size: 677.0 KB (677016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59eb9988c4b9b573a94c2aef256f275f37bc80f4537429e21a07866e21c30c15`  
		Last Modified: Thu, 08 Apr 2021 19:29:12 GMT  
		Size: 16.5 MB (16516915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43e60f188a205da97f1f59c9e979da57a3f96fcdd8a7b677d798138f433a8fca`  
		Last Modified: Thu, 08 Apr 2021 19:29:06 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v1.7.30-alpine` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:0cf15008333d1cc2b7907ebead2b805754d3fd9a35ee0b5ef8f52d26e69d9e35
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **19.5 MB (19495771 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7f9ab0b3ea9162be9ba4e2fedca5164d4769d09ad5492d8df197d742139defbb`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 31 Mar 2021 17:22:02 GMT
ADD file:174ba1b913c5cf549fcdfc259e8e3aa8f49cea660865fd54b8aacb430602a783 in / 
# Wed, 31 Mar 2021 17:22:03 GMT
CMD ["/bin/sh"]
# Thu, 01 Apr 2021 16:15:15 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 08 Apr 2021 20:39:00 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/traefik/traefik/releases/download/v1.7.30/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Thu, 08 Apr 2021 20:39:01 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 08 Apr 2021 20:39:02 GMT
EXPOSE 80
# Thu, 08 Apr 2021 20:39:03 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 08 Apr 2021 20:39:04 GMT
CMD ["traefik"]
# Thu, 08 Apr 2021 20:39:05 GMT
LABEL org.opencontainers.image.vendor=traefik org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.30 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:a3cf95b55367cb73f51318ee9c854def347373482336709ca1882a5d4c20b7c7`  
		Last Modified: Wed, 31 Mar 2021 17:23:00 GMT  
		Size: 2.7 MB (2725871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e08c5532ded8a461bb2539065ec0daf26ce2ecfed811ad86719ad11c964ab658`  
		Last Modified: Thu, 01 Apr 2021 16:17:57 GMT  
		Size: 675.5 KB (675530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bdb060704f0ed88ad3c7606d012c734450f30bd6d4fdfe4afe65a3109473985`  
		Last Modified: Thu, 08 Apr 2021 20:39:54 GMT  
		Size: 16.1 MB (16094002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b924f9ea1253bff83db6941fc95ed9248766194e0712f66bde5fa5f8d89cfe0`  
		Last Modified: Thu, 08 Apr 2021 20:39:49 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v1.7.30-windowsservercore-1809`

```console
$ docker pull traefik@sha256:733a8c228d615ebf548385487b66c7b3fdd7699c1c9f7fec1cfa4c71feeb4785
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1879; amd64

### `traefik:v1.7.30-windowsservercore-1809` - windows version 10.0.17763.1879; amd64

```console
$ docker pull traefik@sha256:e7f8b8eee97e1609e89c4a19e3f7f530a33ca76b26196d1c6bc927eca28645c3
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2492758593 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8bb83271e02abc3f1a599c84de304ca6c4f9ceab42a58cf154675cad4c8e761b`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 09 Apr 2021 20:34:41 GMT
RUN Install update 1809-amd64
# Wed, 14 Apr 2021 12:09:21 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 14 Apr 2021 21:29:52 GMT
RUN Invoke-WebRequest     -Uri "https://github.com/traefik/traefik/releases/download/v1.7.30/traefik_windows-amd64.exe"     -OutFile "/traefik.exe"
# Wed, 14 Apr 2021 21:29:54 GMT
EXPOSE 80
# Wed, 14 Apr 2021 21:29:55 GMT
ENTRYPOINT ["/traefik"]
# Wed, 14 Apr 2021 21:29:56 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.30 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:399f118dfaa9a753e98d128238b944432c7bcabea88a2998a6efbbece28ed303`  
		Size: 751.4 MB (751421005 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:106dbf3373fce4f0ba5e00ad54824c597f2894605fa7d8ef446ad7ea3b97449f`  
		Last Modified: Wed, 14 Apr 2021 12:58:04 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:203e1506701de3ad9fca12951ea83f903d0bdc8628f20a7bfb3d77a713a5ed52`  
		Last Modified: Wed, 14 Apr 2021 21:31:15 GMT  
		Size: 23.0 MB (22998990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2b11339a17c4a4101817c0f6ddc3f3453e39f1c052aedf3f0e9cdb0ffc84365`  
		Last Modified: Wed, 14 Apr 2021 21:31:08 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07482932f6ca5c824d683ca413e9ef96f6aa833fc867c4d614428803b25d6143`  
		Last Modified: Wed, 14 Apr 2021 21:31:08 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f776de6cf2f2359d3f8ccf8e44387cbe850d86e91540ddd4253809940c7afb76`  
		Last Modified: Wed, 14 Apr 2021 21:31:08 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v2.4`

```console
$ docker pull traefik@sha256:af1617e167e8a6554b5e75c1fd759c68887b890be715afa5f36d9ac467410d45
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:v2.4` - linux; amd64

```console
$ docker pull traefik@sha256:4e2da005d39daa3823c6930cfb4ff5eb8d75be3679a2173489d8579e655be4be
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.8 MB (27828337 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:deaf4b1027ed4bce7d3a15a22a7ff5f5fab274bffde1709ae85e93f15085ad98`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:56 GMT
ADD file:282b9d56236cae29600bf8b698cb0a865ab17db7beea0be6870f9de63e7d4f80 in / 
# Wed, 14 Apr 2021 19:19:56 GMT
CMD ["/bin/sh"]
# Thu, 15 Apr 2021 03:04:42 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 15 Apr 2021 03:04:47 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.4.8/traefik_v2.4.8_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 15 Apr 2021 03:04:48 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 15 Apr 2021 03:04:48 GMT
EXPOSE 80
# Thu, 15 Apr 2021 03:04:48 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 15 Apr 2021 03:04:49 GMT
CMD ["traefik"]
# Thu, 15 Apr 2021 03:04:49 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.4.8 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:ddad3d7c1e96adf9153f8921a7c9790f880a390163df453be1566e9ef0d546e0`  
		Last Modified: Wed, 14 Apr 2021 19:21:03 GMT  
		Size: 2.8 MB (2816246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f6722e60c2f6c55424dadebe886f88ba1b903df075b00048427439abb91b85a`  
		Last Modified: Thu, 15 Apr 2021 03:05:57 GMT  
		Size: 674.2 KB (674210 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acb62688737133737535c58e692b79b70843447464a3760d37d1d65c33fa1e5c`  
		Last Modified: Thu, 15 Apr 2021 03:06:03 GMT  
		Size: 24.3 MB (24337513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebb6d79f94aac9a1ec9746826d0fd58ea98a05df8f5ed882819626db57909331`  
		Last Modified: Thu, 15 Apr 2021 03:05:57 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v2.4` - linux; arm variant v6

```console
$ docker pull traefik@sha256:445ec88018c03307101e734adfd8425f4da87e9ffd5d83b1e5fb512d280df5df
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.0 MB (26025735 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9a68d5d0d7cdf26c5ef8132873c04d3e8cc92b65cd6ad0af323361a5c222c57f`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 31 Mar 2021 17:19:20 GMT
ADD file:15a1f9d3700deb648f0b3701afebc97ff28eb30d1b55e18dc9c696a9dd5c8e36 in / 
# Wed, 31 Mar 2021 17:19:21 GMT
CMD ["/bin/sh"]
# Thu, 01 Apr 2021 03:52:35 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 01 Apr 2021 03:52:43 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.4.8/traefik_v2.4.8_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 01 Apr 2021 03:52:44 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 01 Apr 2021 03:52:45 GMT
EXPOSE 80
# Thu, 01 Apr 2021 03:52:47 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 01 Apr 2021 03:52:48 GMT
CMD ["traefik"]
# Thu, 01 Apr 2021 03:52:50 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.4.8 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:ac95243af174972febc49043f62f7b952a0c610e59b55ac4133f442e399e8729`  
		Last Modified: Wed, 31 Mar 2021 17:20:17 GMT  
		Size: 2.6 MB (2621248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25173f2bf7681888ff03bae0a793dcd2a8124175d360f999d21081483f90f181`  
		Last Modified: Thu, 01 Apr 2021 03:54:34 GMT  
		Size: 677.0 KB (677016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9546526ac0315b3d34e7f88f707fb5355cffd936afb2e80198eff85c6524a05`  
		Last Modified: Thu, 01 Apr 2021 03:54:41 GMT  
		Size: 22.7 MB (22727103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ddd0b0952f4a6439010368b09c4bee68dd82bad0c47ff2a4a3a0b8ce6a2c498`  
		Last Modified: Thu, 01 Apr 2021 03:54:33 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v2.4` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:edd78c8c05d3050cbd62e00de1575597f2a1c628fd5faefecb0d8b20c35d7ba9
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.5 MB (25475489 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:19eb3704549293128f6d623b5a417a6cf34b01a797b4e0bf36dee8ef8f255e71`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 31 Mar 2021 17:22:02 GMT
ADD file:174ba1b913c5cf549fcdfc259e8e3aa8f49cea660865fd54b8aacb430602a783 in / 
# Wed, 31 Mar 2021 17:22:03 GMT
CMD ["/bin/sh"]
# Thu, 01 Apr 2021 16:15:15 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 01 Apr 2021 16:15:20 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.4.8/traefik_v2.4.8_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 01 Apr 2021 16:15:22 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 01 Apr 2021 16:15:23 GMT
EXPOSE 80
# Thu, 01 Apr 2021 16:15:23 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 01 Apr 2021 16:15:24 GMT
CMD ["traefik"]
# Thu, 01 Apr 2021 16:15:25 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.4.8 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:a3cf95b55367cb73f51318ee9c854def347373482336709ca1882a5d4c20b7c7`  
		Last Modified: Wed, 31 Mar 2021 17:23:00 GMT  
		Size: 2.7 MB (2725871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e08c5532ded8a461bb2539065ec0daf26ce2ecfed811ad86719ad11c964ab658`  
		Last Modified: Thu, 01 Apr 2021 16:17:57 GMT  
		Size: 675.5 KB (675530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:664cdd830c93e0170df8d4ed17b45f260ee577dcfb6db4d48f6e009b108ff81d`  
		Last Modified: Thu, 01 Apr 2021 16:18:03 GMT  
		Size: 22.1 MB (22073720 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91bdc2d37fb1c66af3a73e5fff4790dcfa4572a7fd25779591f80bd086c718df`  
		Last Modified: Thu, 01 Apr 2021 16:17:57 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v2.4-windowsservercore-1809`

```console
$ docker pull traefik@sha256:a469fcdb7481c955407299e937c5b6cb5c203f6d7cc71c76932b0f41594ee652
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1879; amd64

### `traefik:v2.4-windowsservercore-1809` - windows version 10.0.17763.1879; amd64

```console
$ docker pull traefik@sha256:0fda36d6a58507d81a2c34a79738e3e19ab72b1c3f63316fb0ea4505eb500b09
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2499488628 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3650b9ad832bb235bd53c735995b7542b8bf3dd3dd4cdd9a82e38c5ff8d23c44`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 09 Apr 2021 20:34:41 GMT
RUN Install update 1809-amd64
# Wed, 14 Apr 2021 12:09:21 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 14 Apr 2021 21:28:41 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/traefik/traefik/releases/download/v2.4.8/traefik_v2.4.8_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Wed, 14 Apr 2021 21:28:43 GMT
EXPOSE 80
# Wed, 14 Apr 2021 21:28:44 GMT
ENTRYPOINT ["/traefik"]
# Wed, 14 Apr 2021 21:28:45 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.4.8 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:399f118dfaa9a753e98d128238b944432c7bcabea88a2998a6efbbece28ed303`  
		Size: 751.4 MB (751421005 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:106dbf3373fce4f0ba5e00ad54824c597f2894605fa7d8ef446ad7ea3b97449f`  
		Last Modified: Wed, 14 Apr 2021 12:58:04 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a93cd244b1a7725d26281629f3d234056508569c464f5dea5b03ccbde91bb0f`  
		Last Modified: Wed, 14 Apr 2021 21:30:37 GMT  
		Size: 29.7 MB (29729029 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f7bb23c17022bf3359394806bf3c61d486089608895251ff7a5acfd7ad96a9a`  
		Last Modified: Wed, 14 Apr 2021 21:30:28 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb84fdded1774834fd927e9a9f74098955381bfeb1991c90d23188e9f2d4bf95`  
		Last Modified: Wed, 14 Apr 2021 21:30:27 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46b1c96a0690beee17c07772a87933a00a71ff757191a2e22ddb4b54488a8000`  
		Last Modified: Wed, 14 Apr 2021 21:30:27 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v2.4.8`

```console
$ docker pull traefik@sha256:af1617e167e8a6554b5e75c1fd759c68887b890be715afa5f36d9ac467410d45
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:v2.4.8` - linux; amd64

```console
$ docker pull traefik@sha256:4e2da005d39daa3823c6930cfb4ff5eb8d75be3679a2173489d8579e655be4be
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.8 MB (27828337 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:deaf4b1027ed4bce7d3a15a22a7ff5f5fab274bffde1709ae85e93f15085ad98`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:56 GMT
ADD file:282b9d56236cae29600bf8b698cb0a865ab17db7beea0be6870f9de63e7d4f80 in / 
# Wed, 14 Apr 2021 19:19:56 GMT
CMD ["/bin/sh"]
# Thu, 15 Apr 2021 03:04:42 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 15 Apr 2021 03:04:47 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.4.8/traefik_v2.4.8_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 15 Apr 2021 03:04:48 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 15 Apr 2021 03:04:48 GMT
EXPOSE 80
# Thu, 15 Apr 2021 03:04:48 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 15 Apr 2021 03:04:49 GMT
CMD ["traefik"]
# Thu, 15 Apr 2021 03:04:49 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.4.8 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:ddad3d7c1e96adf9153f8921a7c9790f880a390163df453be1566e9ef0d546e0`  
		Last Modified: Wed, 14 Apr 2021 19:21:03 GMT  
		Size: 2.8 MB (2816246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f6722e60c2f6c55424dadebe886f88ba1b903df075b00048427439abb91b85a`  
		Last Modified: Thu, 15 Apr 2021 03:05:57 GMT  
		Size: 674.2 KB (674210 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acb62688737133737535c58e692b79b70843447464a3760d37d1d65c33fa1e5c`  
		Last Modified: Thu, 15 Apr 2021 03:06:03 GMT  
		Size: 24.3 MB (24337513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebb6d79f94aac9a1ec9746826d0fd58ea98a05df8f5ed882819626db57909331`  
		Last Modified: Thu, 15 Apr 2021 03:05:57 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v2.4.8` - linux; arm variant v6

```console
$ docker pull traefik@sha256:445ec88018c03307101e734adfd8425f4da87e9ffd5d83b1e5fb512d280df5df
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.0 MB (26025735 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9a68d5d0d7cdf26c5ef8132873c04d3e8cc92b65cd6ad0af323361a5c222c57f`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 31 Mar 2021 17:19:20 GMT
ADD file:15a1f9d3700deb648f0b3701afebc97ff28eb30d1b55e18dc9c696a9dd5c8e36 in / 
# Wed, 31 Mar 2021 17:19:21 GMT
CMD ["/bin/sh"]
# Thu, 01 Apr 2021 03:52:35 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 01 Apr 2021 03:52:43 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.4.8/traefik_v2.4.8_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 01 Apr 2021 03:52:44 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 01 Apr 2021 03:52:45 GMT
EXPOSE 80
# Thu, 01 Apr 2021 03:52:47 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 01 Apr 2021 03:52:48 GMT
CMD ["traefik"]
# Thu, 01 Apr 2021 03:52:50 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.4.8 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:ac95243af174972febc49043f62f7b952a0c610e59b55ac4133f442e399e8729`  
		Last Modified: Wed, 31 Mar 2021 17:20:17 GMT  
		Size: 2.6 MB (2621248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25173f2bf7681888ff03bae0a793dcd2a8124175d360f999d21081483f90f181`  
		Last Modified: Thu, 01 Apr 2021 03:54:34 GMT  
		Size: 677.0 KB (677016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9546526ac0315b3d34e7f88f707fb5355cffd936afb2e80198eff85c6524a05`  
		Last Modified: Thu, 01 Apr 2021 03:54:41 GMT  
		Size: 22.7 MB (22727103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ddd0b0952f4a6439010368b09c4bee68dd82bad0c47ff2a4a3a0b8ce6a2c498`  
		Last Modified: Thu, 01 Apr 2021 03:54:33 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v2.4.8` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:edd78c8c05d3050cbd62e00de1575597f2a1c628fd5faefecb0d8b20c35d7ba9
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.5 MB (25475489 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:19eb3704549293128f6d623b5a417a6cf34b01a797b4e0bf36dee8ef8f255e71`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 31 Mar 2021 17:22:02 GMT
ADD file:174ba1b913c5cf549fcdfc259e8e3aa8f49cea660865fd54b8aacb430602a783 in / 
# Wed, 31 Mar 2021 17:22:03 GMT
CMD ["/bin/sh"]
# Thu, 01 Apr 2021 16:15:15 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 01 Apr 2021 16:15:20 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.4.8/traefik_v2.4.8_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 01 Apr 2021 16:15:22 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 01 Apr 2021 16:15:23 GMT
EXPOSE 80
# Thu, 01 Apr 2021 16:15:23 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 01 Apr 2021 16:15:24 GMT
CMD ["traefik"]
# Thu, 01 Apr 2021 16:15:25 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.4.8 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:a3cf95b55367cb73f51318ee9c854def347373482336709ca1882a5d4c20b7c7`  
		Last Modified: Wed, 31 Mar 2021 17:23:00 GMT  
		Size: 2.7 MB (2725871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e08c5532ded8a461bb2539065ec0daf26ce2ecfed811ad86719ad11c964ab658`  
		Last Modified: Thu, 01 Apr 2021 16:17:57 GMT  
		Size: 675.5 KB (675530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:664cdd830c93e0170df8d4ed17b45f260ee577dcfb6db4d48f6e009b108ff81d`  
		Last Modified: Thu, 01 Apr 2021 16:18:03 GMT  
		Size: 22.1 MB (22073720 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91bdc2d37fb1c66af3a73e5fff4790dcfa4572a7fd25779591f80bd086c718df`  
		Last Modified: Thu, 01 Apr 2021 16:17:57 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v2.4.8-windowsservercore-1809`

```console
$ docker pull traefik@sha256:a469fcdb7481c955407299e937c5b6cb5c203f6d7cc71c76932b0f41594ee652
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1879; amd64

### `traefik:v2.4.8-windowsservercore-1809` - windows version 10.0.17763.1879; amd64

```console
$ docker pull traefik@sha256:0fda36d6a58507d81a2c34a79738e3e19ab72b1c3f63316fb0ea4505eb500b09
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2499488628 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3650b9ad832bb235bd53c735995b7542b8bf3dd3dd4cdd9a82e38c5ff8d23c44`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 09 Apr 2021 20:34:41 GMT
RUN Install update 1809-amd64
# Wed, 14 Apr 2021 12:09:21 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 14 Apr 2021 21:28:41 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/traefik/traefik/releases/download/v2.4.8/traefik_v2.4.8_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Wed, 14 Apr 2021 21:28:43 GMT
EXPOSE 80
# Wed, 14 Apr 2021 21:28:44 GMT
ENTRYPOINT ["/traefik"]
# Wed, 14 Apr 2021 21:28:45 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.4.8 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:399f118dfaa9a753e98d128238b944432c7bcabea88a2998a6efbbece28ed303`  
		Size: 751.4 MB (751421005 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:106dbf3373fce4f0ba5e00ad54824c597f2894605fa7d8ef446ad7ea3b97449f`  
		Last Modified: Wed, 14 Apr 2021 12:58:04 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a93cd244b1a7725d26281629f3d234056508569c464f5dea5b03ccbde91bb0f`  
		Last Modified: Wed, 14 Apr 2021 21:30:37 GMT  
		Size: 29.7 MB (29729029 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f7bb23c17022bf3359394806bf3c61d486089608895251ff7a5acfd7ad96a9a`  
		Last Modified: Wed, 14 Apr 2021 21:30:28 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb84fdded1774834fd927e9a9f74098955381bfeb1991c90d23188e9f2d4bf95`  
		Last Modified: Wed, 14 Apr 2021 21:30:27 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46b1c96a0690beee17c07772a87933a00a71ff757191a2e22ddb4b54488a8000`  
		Last Modified: Wed, 14 Apr 2021 21:30:27 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:windowsservercore-1809`

```console
$ docker pull traefik@sha256:a469fcdb7481c955407299e937c5b6cb5c203f6d7cc71c76932b0f41594ee652
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1879; amd64

### `traefik:windowsservercore-1809` - windows version 10.0.17763.1879; amd64

```console
$ docker pull traefik@sha256:0fda36d6a58507d81a2c34a79738e3e19ab72b1c3f63316fb0ea4505eb500b09
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2499488628 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3650b9ad832bb235bd53c735995b7542b8bf3dd3dd4cdd9a82e38c5ff8d23c44`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 09 Apr 2021 20:34:41 GMT
RUN Install update 1809-amd64
# Wed, 14 Apr 2021 12:09:21 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 14 Apr 2021 21:28:41 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/traefik/traefik/releases/download/v2.4.8/traefik_v2.4.8_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Wed, 14 Apr 2021 21:28:43 GMT
EXPOSE 80
# Wed, 14 Apr 2021 21:28:44 GMT
ENTRYPOINT ["/traefik"]
# Wed, 14 Apr 2021 21:28:45 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.4.8 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:399f118dfaa9a753e98d128238b944432c7bcabea88a2998a6efbbece28ed303`  
		Size: 751.4 MB (751421005 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:106dbf3373fce4f0ba5e00ad54824c597f2894605fa7d8ef446ad7ea3b97449f`  
		Last Modified: Wed, 14 Apr 2021 12:58:04 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a93cd244b1a7725d26281629f3d234056508569c464f5dea5b03ccbde91bb0f`  
		Last Modified: Wed, 14 Apr 2021 21:30:37 GMT  
		Size: 29.7 MB (29729029 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f7bb23c17022bf3359394806bf3c61d486089608895251ff7a5acfd7ad96a9a`  
		Last Modified: Wed, 14 Apr 2021 21:30:28 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb84fdded1774834fd927e9a9f74098955381bfeb1991c90d23188e9f2d4bf95`  
		Last Modified: Wed, 14 Apr 2021 21:30:27 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46b1c96a0690beee17c07772a87933a00a71ff757191a2e22ddb4b54488a8000`  
		Last Modified: Wed, 14 Apr 2021 21:30:27 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
