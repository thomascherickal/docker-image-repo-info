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
-	[`traefik:2.9.5`](#traefik295)
-	[`traefik:2.9.5-windowsservercore-1809`](#traefik295-windowsservercore-1809)
-	[`traefik:3.0`](#traefik30)
-	[`traefik:3.0-windowsservercore-1809`](#traefik30-windowsservercore-1809)
-	[`traefik:3.0.0-beta1`](#traefik300-beta1)
-	[`traefik:3.0.0-beta1-windowsservercore-1809`](#traefik300-beta1-windowsservercore-1809)
-	[`traefik:banon`](#traefikbanon)
-	[`traefik:banon-windowsservercore-1809`](#traefikbanon-windowsservercore-1809)
-	[`traefik:beaufort`](#traefikbeaufort)
-	[`traefik:beaufort-windowsservercore-1809`](#traefikbeaufort-windowsservercore-1809)
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
-	[`traefik:v2.9.5`](#traefikv295)
-	[`traefik:v2.9.5-windowsservercore-1809`](#traefikv295-windowsservercore-1809)
-	[`traefik:v3.0`](#traefikv30)
-	[`traefik:v3.0-windowsservercore-1809`](#traefikv30-windowsservercore-1809)
-	[`traefik:v3.0.0-beta1`](#traefikv300-beta1)
-	[`traefik:v3.0.0-beta1-windowsservercore-1809`](#traefikv300-beta1-windowsservercore-1809)
-	[`traefik:windowsservercore-1809`](#traefikwindowsservercore-1809)

## `traefik:1.7`

```console
$ docker pull traefik@sha256:3a46f4e724ac467d9e3955792bba4327e17fa2e9e1fed93f13b85fd45b71816a
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
$ docker pull traefik@sha256:ed51daf51f75bf5735027eed93829bc2ddc8cab5f7d2c92661e9ae240a812647
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **21.1 MB (21055568 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:35629440895fbdc6144fd69e6ddccee4de8aa7785af39e4804683304ac4f2df1`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Fri, 28 Oct 2022 00:15:28 GMT
COPY file:48964762d0c961c28f59ebd3ea194fb6486cf2bd9a9cf1780f6702d88bd7b7d9 in /etc/ssl/certs/ 
# Fri, 11 Nov 2022 11:59:12 GMT
COPY dir:3b1b1d8650d4180b42ead5fd074947c16b0405195b425df367fbf007be68841d in /usr/share/ 
# Fri, 11 Nov 2022 11:59:13 GMT
COPY file:5d1e7e81e8b77b4f8828eeaf0d30a0f135a949b51396f12ae22af376c36d3129 in / 
# Fri, 11 Nov 2022 11:59:14 GMT
EXPOSE 80
# Fri, 11 Nov 2022 11:59:14 GMT
VOLUME [/tmp]
# Fri, 11 Nov 2022 11:59:14 GMT
ENTRYPOINT ["/traefik"]
# Fri, 11 Nov 2022 11:59:14 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.34 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:93432fb5c46fdb5c83e424ff85db4e06a08e5ac2ec96ce9e11f1c60f5a86d29b`  
		Last Modified: Fri, 28 Oct 2022 00:17:20 GMT  
		Size: 123.5 KB (123538 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0efdacb2b2ba042055ea537001460b2cff92ff305869705801b66bc44dc8565`  
		Last Modified: Fri, 11 Nov 2022 12:01:04 GMT  
		Size: 308.7 KB (308749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:849ebe6d2d943e776e37535f360e7b0f3745d625ee69f6ee5fe1eecee5487ce1`  
		Last Modified: Fri, 11 Nov 2022 12:01:08 GMT  
		Size: 20.6 MB (20623281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:1.7` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:ac5b287132e97dc27bbd96791a25701e051ddce973d6ee70eda1c87138e3c299
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **20.6 MB (20563697 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f9d5da1bea8e1a3e20b83ceca6e486a1e881451b1e304a0281d936d5e51f418d`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Thu, 27 Oct 2022 23:00:59 GMT
COPY file:48964762d0c961c28f59ebd3ea194fb6486cf2bd9a9cf1780f6702d88bd7b7d9 in /etc/ssl/certs/ 
# Fri, 11 Nov 2022 11:00:57 GMT
COPY dir:3b1b1d8650d4180b42ead5fd074947c16b0405195b425df367fbf007be68841d in /usr/share/ 
# Fri, 11 Nov 2022 11:00:58 GMT
COPY file:60330593b6644f3f519fd13ce8ee34c2c7ab9994a1420afabbc01926dd1230dd in / 
# Fri, 11 Nov 2022 11:00:58 GMT
EXPOSE 80
# Fri, 11 Nov 2022 11:00:58 GMT
VOLUME [/tmp]
# Fri, 11 Nov 2022 11:00:58 GMT
ENTRYPOINT ["/traefik"]
# Fri, 11 Nov 2022 11:00:58 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.34 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:384a668e636c3a58c260d7eacd140f07b0727673d5ba128334cbcedd184a99f2`  
		Last Modified: Thu, 27 Oct 2022 23:02:00 GMT  
		Size: 123.5 KB (123538 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a3f6a6b590d30fda524213974a86d6ca01981b3ab4154a359b9c2e3fa3262c6`  
		Last Modified: Fri, 11 Nov 2022 11:02:04 GMT  
		Size: 308.8 KB (308813 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2af8a7d805d81cf74f58f3793659f76132259201bea15bbb7a0edc6191f8edfa`  
		Last Modified: Fri, 11 Nov 2022 11:02:07 GMT  
		Size: 20.1 MB (20131346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:1.7-alpine`

```console
$ docker pull traefik@sha256:f50efd68ddcb8b1b8ad030fcf1011fa6a2b42412e1339b6fe2731e73eb1db963
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
$ docker pull traefik@sha256:0ae1b77619decee480ac73c5643f221285808044b307298c32c3d6c8bad3e184
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.9 MB (23925564 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:636cce97efeea9b6e6cae06ecc42e060b6488713c0b64e8a4754f9e7439ba766`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 10 Nov 2022 20:49:43 GMT
ADD file:8ff80989f06f5a8ffe16c56e00538928dcb1e46faa2b58ab9c14c7227a6cd8f9 in / 
# Thu, 10 Nov 2022 20:49:43 GMT
CMD ["/bin/sh"]
# Fri, 11 Nov 2022 11:58:55 GMT
RUN apk --no-cache add ca-certificates tzdata
# Fri, 11 Nov 2022 11:59:00 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/traefik/traefik/releases/download/v1.7.34/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Fri, 11 Nov 2022 11:59:01 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Fri, 11 Nov 2022 11:59:01 GMT
EXPOSE 80
# Fri, 11 Nov 2022 11:59:01 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 11 Nov 2022 11:59:01 GMT
CMD ["traefik"]
# Fri, 11 Nov 2022 11:59:01 GMT
LABEL org.opencontainers.image.vendor=traefik org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.34 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:7d147289082e6aa6ef510c09d7c0ac8b5026e0b591f1bfcaf01ceada43c9ec65`  
		Last Modified: Tue, 09 Aug 2022 17:51:04 GMT  
		Size: 2.6 MB (2635498 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33435e7e7c652bea7ffaf83b027d129ebd3d136e11e2469998ccbc32288c98fa`  
		Last Modified: Fri, 11 Nov 2022 12:00:39 GMT  
		Size: 666.3 KB (666268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d38a2c13dc82440cb92fa776a94c406c832435459441a480e7bf60df1e0baed`  
		Last Modified: Fri, 11 Nov 2022 12:00:43 GMT  
		Size: 20.6 MB (20623430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aed31ebc6a3ec75add73f53bf95dd91c31a2bbdadfbf38a7b44c7b57f8fb9f8a`  
		Last Modified: Fri, 11 Nov 2022 12:00:39 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:1.7-alpine` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:64b63c53bbf8a021857ee49412ff72501a52a4e821ffd1f3a17f213562a55dcf
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.5 MB (23517049 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7adbabdcf54e3ae316f53747af91e16d550dfdfc9afaa2e19f9d4f61a1ab2759`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 10 Nov 2022 20:39:51 GMT
ADD file:b312c8f512719efd09811d17c2b250bbad03cf3f90c135a00695cc8e152f4ee2 in / 
# Thu, 10 Nov 2022 20:39:51 GMT
CMD ["/bin/sh"]
# Fri, 11 Nov 2022 11:00:45 GMT
RUN apk --no-cache add ca-certificates tzdata
# Fri, 11 Nov 2022 11:00:51 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/traefik/traefik/releases/download/v1.7.34/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Fri, 11 Nov 2022 11:00:51 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Fri, 11 Nov 2022 11:00:51 GMT
EXPOSE 80
# Fri, 11 Nov 2022 11:00:51 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 11 Nov 2022 11:00:51 GMT
CMD ["traefik"]
# Fri, 11 Nov 2022 11:00:51 GMT
LABEL org.opencontainers.image.vendor=traefik org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.34 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:90cda3b7c32511829cd5ae9074240c36c34507085acb6e55b96f993740d2be93`  
		Last Modified: Tue, 09 Aug 2022 17:41:06 GMT  
		Size: 2.7 MB (2722153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bef289adf2cbb3f8d157193bbfd586faaa288d6dd23845f0db17b7c041df2ef`  
		Last Modified: Fri, 11 Nov 2022 11:01:45 GMT  
		Size: 663.1 KB (663148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4d7297d487dbad0e6a3001add15c558d8305d106c11a0f1d1572e3b8cb8c221`  
		Last Modified: Fri, 11 Nov 2022 11:01:47 GMT  
		Size: 20.1 MB (20131380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:238986be5500952726a82d7ee40ae56ba3acfe2c8512f680e8c1e764ba05184b`  
		Last Modified: Fri, 11 Nov 2022 11:01:44 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:1.7-windowsservercore-1809`

```console
$ docker pull traefik@sha256:ba22fa49d06eb335a538647f8ac6b53100619cef2d6dac06269da6c557709513
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3650; amd64

### `traefik:1.7-windowsservercore-1809` - windows version 10.0.17763.3650; amd64

```console
$ docker pull traefik@sha256:8c0df9f3b6b67923ad88bb8c325e64f06bfec58ede2be72f6161a12fb58b0514
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 GB (2801442412 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5ffbcd25321baf9b5e717f95aad8a5c850725ea21067094e561b04f95f5e73c5`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Sat, 05 Nov 2022 18:29:26 GMT
RUN Install update 10.0.17763.3650
# Tue, 08 Nov 2022 18:31:26 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Nov 2022 19:39:46 GMT
RUN Invoke-WebRequest     -Uri "https://github.com/traefik/traefik/releases/download/v1.7.34/traefik_windows-amd64.exe"     -OutFile "/traefik.exe"
# Wed, 09 Nov 2022 19:39:47 GMT
EXPOSE 80
# Wed, 09 Nov 2022 19:39:48 GMT
ENTRYPOINT ["/traefik"]
# Wed, 09 Nov 2022 19:39:50 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.34 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:a48a3e4ae2de839d8e99bde16eb91d113fb2cf889bba472d0c4274851b5fb402`  
		Last Modified: Tue, 21 Jun 2022 18:30:17 GMT  
		Size: 1.9 GB (1924269350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c26cc6e4f9eb1ae415a5ead6f884cac597bbd57efa6cd042c878d5b54c9d2091`  
		Last Modified: Tue, 08 Nov 2022 19:44:35 GMT  
		Size: 854.3 MB (854317461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f182832ad6ad5ea3d4b7320fd7bfea56fb9cf8413be904e52db6ed14c8d9e36f`  
		Last Modified: Tue, 08 Nov 2022 19:42:07 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:114e02070c38ac40033338b737577f7ed16181f6ce5ef3a282eb2a91b99c1967`  
		Last Modified: Wed, 09 Nov 2022 19:40:52 GMT  
		Size: 22.9 MB (22850203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:198ef1b6118e3b8dff31c6ada18f95988302cf4293219d1043eb9b810b79f9ec`  
		Last Modified: Wed, 09 Nov 2022 19:40:46 GMT  
		Size: 1.3 KB (1316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8499782a4e49b27eacd6a70cb60fb670341838fe2a3a9103ec45ff34bbe922c9`  
		Last Modified: Wed, 09 Nov 2022 19:40:46 GMT  
		Size: 1.3 KB (1331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aadd67eff429b70dc14789c1a0f220cf3c25607c2b6a8145d3756731eb5b771a`  
		Last Modified: Wed, 09 Nov 2022 19:40:46 GMT  
		Size: 1.3 KB (1311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:1.7.34`

```console
$ docker pull traefik@sha256:3a46f4e724ac467d9e3955792bba4327e17fa2e9e1fed93f13b85fd45b71816a
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
$ docker pull traefik@sha256:ed51daf51f75bf5735027eed93829bc2ddc8cab5f7d2c92661e9ae240a812647
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **21.1 MB (21055568 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:35629440895fbdc6144fd69e6ddccee4de8aa7785af39e4804683304ac4f2df1`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Fri, 28 Oct 2022 00:15:28 GMT
COPY file:48964762d0c961c28f59ebd3ea194fb6486cf2bd9a9cf1780f6702d88bd7b7d9 in /etc/ssl/certs/ 
# Fri, 11 Nov 2022 11:59:12 GMT
COPY dir:3b1b1d8650d4180b42ead5fd074947c16b0405195b425df367fbf007be68841d in /usr/share/ 
# Fri, 11 Nov 2022 11:59:13 GMT
COPY file:5d1e7e81e8b77b4f8828eeaf0d30a0f135a949b51396f12ae22af376c36d3129 in / 
# Fri, 11 Nov 2022 11:59:14 GMT
EXPOSE 80
# Fri, 11 Nov 2022 11:59:14 GMT
VOLUME [/tmp]
# Fri, 11 Nov 2022 11:59:14 GMT
ENTRYPOINT ["/traefik"]
# Fri, 11 Nov 2022 11:59:14 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.34 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:93432fb5c46fdb5c83e424ff85db4e06a08e5ac2ec96ce9e11f1c60f5a86d29b`  
		Last Modified: Fri, 28 Oct 2022 00:17:20 GMT  
		Size: 123.5 KB (123538 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0efdacb2b2ba042055ea537001460b2cff92ff305869705801b66bc44dc8565`  
		Last Modified: Fri, 11 Nov 2022 12:01:04 GMT  
		Size: 308.7 KB (308749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:849ebe6d2d943e776e37535f360e7b0f3745d625ee69f6ee5fe1eecee5487ce1`  
		Last Modified: Fri, 11 Nov 2022 12:01:08 GMT  
		Size: 20.6 MB (20623281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:1.7.34` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:ac5b287132e97dc27bbd96791a25701e051ddce973d6ee70eda1c87138e3c299
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **20.6 MB (20563697 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f9d5da1bea8e1a3e20b83ceca6e486a1e881451b1e304a0281d936d5e51f418d`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Thu, 27 Oct 2022 23:00:59 GMT
COPY file:48964762d0c961c28f59ebd3ea194fb6486cf2bd9a9cf1780f6702d88bd7b7d9 in /etc/ssl/certs/ 
# Fri, 11 Nov 2022 11:00:57 GMT
COPY dir:3b1b1d8650d4180b42ead5fd074947c16b0405195b425df367fbf007be68841d in /usr/share/ 
# Fri, 11 Nov 2022 11:00:58 GMT
COPY file:60330593b6644f3f519fd13ce8ee34c2c7ab9994a1420afabbc01926dd1230dd in / 
# Fri, 11 Nov 2022 11:00:58 GMT
EXPOSE 80
# Fri, 11 Nov 2022 11:00:58 GMT
VOLUME [/tmp]
# Fri, 11 Nov 2022 11:00:58 GMT
ENTRYPOINT ["/traefik"]
# Fri, 11 Nov 2022 11:00:58 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.34 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:384a668e636c3a58c260d7eacd140f07b0727673d5ba128334cbcedd184a99f2`  
		Last Modified: Thu, 27 Oct 2022 23:02:00 GMT  
		Size: 123.5 KB (123538 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a3f6a6b590d30fda524213974a86d6ca01981b3ab4154a359b9c2e3fa3262c6`  
		Last Modified: Fri, 11 Nov 2022 11:02:04 GMT  
		Size: 308.8 KB (308813 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2af8a7d805d81cf74f58f3793659f76132259201bea15bbb7a0edc6191f8edfa`  
		Last Modified: Fri, 11 Nov 2022 11:02:07 GMT  
		Size: 20.1 MB (20131346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:1.7.34-alpine`

```console
$ docker pull traefik@sha256:f50efd68ddcb8b1b8ad030fcf1011fa6a2b42412e1339b6fe2731e73eb1db963
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
$ docker pull traefik@sha256:0ae1b77619decee480ac73c5643f221285808044b307298c32c3d6c8bad3e184
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.9 MB (23925564 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:636cce97efeea9b6e6cae06ecc42e060b6488713c0b64e8a4754f9e7439ba766`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 10 Nov 2022 20:49:43 GMT
ADD file:8ff80989f06f5a8ffe16c56e00538928dcb1e46faa2b58ab9c14c7227a6cd8f9 in / 
# Thu, 10 Nov 2022 20:49:43 GMT
CMD ["/bin/sh"]
# Fri, 11 Nov 2022 11:58:55 GMT
RUN apk --no-cache add ca-certificates tzdata
# Fri, 11 Nov 2022 11:59:00 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/traefik/traefik/releases/download/v1.7.34/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Fri, 11 Nov 2022 11:59:01 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Fri, 11 Nov 2022 11:59:01 GMT
EXPOSE 80
# Fri, 11 Nov 2022 11:59:01 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 11 Nov 2022 11:59:01 GMT
CMD ["traefik"]
# Fri, 11 Nov 2022 11:59:01 GMT
LABEL org.opencontainers.image.vendor=traefik org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.34 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:7d147289082e6aa6ef510c09d7c0ac8b5026e0b591f1bfcaf01ceada43c9ec65`  
		Last Modified: Tue, 09 Aug 2022 17:51:04 GMT  
		Size: 2.6 MB (2635498 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33435e7e7c652bea7ffaf83b027d129ebd3d136e11e2469998ccbc32288c98fa`  
		Last Modified: Fri, 11 Nov 2022 12:00:39 GMT  
		Size: 666.3 KB (666268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d38a2c13dc82440cb92fa776a94c406c832435459441a480e7bf60df1e0baed`  
		Last Modified: Fri, 11 Nov 2022 12:00:43 GMT  
		Size: 20.6 MB (20623430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aed31ebc6a3ec75add73f53bf95dd91c31a2bbdadfbf38a7b44c7b57f8fb9f8a`  
		Last Modified: Fri, 11 Nov 2022 12:00:39 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:1.7.34-alpine` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:64b63c53bbf8a021857ee49412ff72501a52a4e821ffd1f3a17f213562a55dcf
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.5 MB (23517049 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7adbabdcf54e3ae316f53747af91e16d550dfdfc9afaa2e19f9d4f61a1ab2759`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 10 Nov 2022 20:39:51 GMT
ADD file:b312c8f512719efd09811d17c2b250bbad03cf3f90c135a00695cc8e152f4ee2 in / 
# Thu, 10 Nov 2022 20:39:51 GMT
CMD ["/bin/sh"]
# Fri, 11 Nov 2022 11:00:45 GMT
RUN apk --no-cache add ca-certificates tzdata
# Fri, 11 Nov 2022 11:00:51 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/traefik/traefik/releases/download/v1.7.34/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Fri, 11 Nov 2022 11:00:51 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Fri, 11 Nov 2022 11:00:51 GMT
EXPOSE 80
# Fri, 11 Nov 2022 11:00:51 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 11 Nov 2022 11:00:51 GMT
CMD ["traefik"]
# Fri, 11 Nov 2022 11:00:51 GMT
LABEL org.opencontainers.image.vendor=traefik org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.34 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:90cda3b7c32511829cd5ae9074240c36c34507085acb6e55b96f993740d2be93`  
		Last Modified: Tue, 09 Aug 2022 17:41:06 GMT  
		Size: 2.7 MB (2722153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bef289adf2cbb3f8d157193bbfd586faaa288d6dd23845f0db17b7c041df2ef`  
		Last Modified: Fri, 11 Nov 2022 11:01:45 GMT  
		Size: 663.1 KB (663148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4d7297d487dbad0e6a3001add15c558d8305d106c11a0f1d1572e3b8cb8c221`  
		Last Modified: Fri, 11 Nov 2022 11:01:47 GMT  
		Size: 20.1 MB (20131380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:238986be5500952726a82d7ee40ae56ba3acfe2c8512f680e8c1e764ba05184b`  
		Last Modified: Fri, 11 Nov 2022 11:01:44 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:1.7.34-windowsservercore-1809`

```console
$ docker pull traefik@sha256:ba22fa49d06eb335a538647f8ac6b53100619cef2d6dac06269da6c557709513
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3650; amd64

### `traefik:1.7.34-windowsservercore-1809` - windows version 10.0.17763.3650; amd64

```console
$ docker pull traefik@sha256:8c0df9f3b6b67923ad88bb8c325e64f06bfec58ede2be72f6161a12fb58b0514
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 GB (2801442412 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5ffbcd25321baf9b5e717f95aad8a5c850725ea21067094e561b04f95f5e73c5`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Sat, 05 Nov 2022 18:29:26 GMT
RUN Install update 10.0.17763.3650
# Tue, 08 Nov 2022 18:31:26 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Nov 2022 19:39:46 GMT
RUN Invoke-WebRequest     -Uri "https://github.com/traefik/traefik/releases/download/v1.7.34/traefik_windows-amd64.exe"     -OutFile "/traefik.exe"
# Wed, 09 Nov 2022 19:39:47 GMT
EXPOSE 80
# Wed, 09 Nov 2022 19:39:48 GMT
ENTRYPOINT ["/traefik"]
# Wed, 09 Nov 2022 19:39:50 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.34 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:a48a3e4ae2de839d8e99bde16eb91d113fb2cf889bba472d0c4274851b5fb402`  
		Last Modified: Tue, 21 Jun 2022 18:30:17 GMT  
		Size: 1.9 GB (1924269350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c26cc6e4f9eb1ae415a5ead6f884cac597bbd57efa6cd042c878d5b54c9d2091`  
		Last Modified: Tue, 08 Nov 2022 19:44:35 GMT  
		Size: 854.3 MB (854317461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f182832ad6ad5ea3d4b7320fd7bfea56fb9cf8413be904e52db6ed14c8d9e36f`  
		Last Modified: Tue, 08 Nov 2022 19:42:07 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:114e02070c38ac40033338b737577f7ed16181f6ce5ef3a282eb2a91b99c1967`  
		Last Modified: Wed, 09 Nov 2022 19:40:52 GMT  
		Size: 22.9 MB (22850203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:198ef1b6118e3b8dff31c6ada18f95988302cf4293219d1043eb9b810b79f9ec`  
		Last Modified: Wed, 09 Nov 2022 19:40:46 GMT  
		Size: 1.3 KB (1316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8499782a4e49b27eacd6a70cb60fb670341838fe2a3a9103ec45ff34bbe922c9`  
		Last Modified: Wed, 09 Nov 2022 19:40:46 GMT  
		Size: 1.3 KB (1331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aadd67eff429b70dc14789c1a0f220cf3c25607c2b6a8145d3756731eb5b771a`  
		Last Modified: Wed, 09 Nov 2022 19:40:46 GMT  
		Size: 1.3 KB (1311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:2.9`

```console
$ docker pull traefik@sha256:ac1480ce3203541705b01d6dce40ef4bf563cdb29d5b00db88cc396fa9fa9cd5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; s390x

### `traefik:2.9` - linux; amd64

```console
$ docker pull traefik@sha256:6c37f2135af79e0c2e387653ff3ab9abf95eb393439f07cfcfa5e06fd4bb10bb
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.7 MB (38661782 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d3cd2c35d32c1bfe78d93c2fda68314b39de4f405ff4f82c86eebd3420d108b3`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Tue, 09 Aug 2022 17:20:00 GMT
ADD file:f77e3f51f020890d22997e6c2ca98968b75b8bc8c463341a2010ff0655d4c88f in / 
# Tue, 09 Aug 2022 17:20:01 GMT
CMD ["/bin/sh"]
# Fri, 07 Oct 2022 04:21:14 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 17 Nov 2022 20:23:09 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.9.5/traefik_v2.9.5_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 17 Nov 2022 20:23:09 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 17 Nov 2022 20:23:09 GMT
EXPOSE 80
# Thu, 17 Nov 2022 20:23:09 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 17 Nov 2022 20:23:09 GMT
CMD ["traefik"]
# Thu, 17 Nov 2022 20:23:09 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.9.5 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:9ed08b51c99c95fb89d4d3eb43cacb1df34c40a394366b2ae5f94758f917c6f5`  
		Last Modified: Thu, 17 Nov 2022 20:23:40 GMT  
		Size: 35.2 MB (35164531 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2984145d314f0df14678294313f70e7a9112a1ac304a1550d6f55b3f36f95cbc`  
		Last Modified: Thu, 17 Nov 2022 20:23:34 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:2.9` - linux; arm variant v6

```console
$ docker pull traefik@sha256:f5bf1b659f8d381c1a13a2860015c160389af6fdfa3ab42b9c463a80150a84c3
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.5 MB (36498990 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:593023589445e011e74b841e01b331d02f3f257483cdda1d0327fdebba48c7de`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 10 Nov 2022 20:49:36 GMT
ADD file:89cb25f97e17bed5c56311280efe5cfa78422d8ffbe36232195d13f94d67417e in / 
# Thu, 10 Nov 2022 20:49:36 GMT
CMD ["/bin/sh"]
# Fri, 11 Nov 2022 11:58:35 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 17 Nov 2022 20:52:12 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.9.5/traefik_v2.9.5_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 17 Nov 2022 20:52:13 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 17 Nov 2022 20:52:13 GMT
EXPOSE 80
# Thu, 17 Nov 2022 20:52:13 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 17 Nov 2022 20:52:13 GMT
CMD ["traefik"]
# Thu, 17 Nov 2022 20:52:13 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.9.5 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:293b708aa6fb80967f27727d5c9c53ac9ba9cac376bed2ad02c17a5cca317b35`  
		Last Modified: Tue, 09 Aug 2022 17:50:52 GMT  
		Size: 2.6 MB (2631127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d346396c5843930d5c9d8e05ce83d5cc4fb94e7d986b9a31ed533e815c10e155`  
		Last Modified: Fri, 11 Nov 2022 12:00:08 GMT  
		Size: 666.4 KB (666362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cff7ec90e94457bb22f14c6a7c1c13725a823452f45c5ae834ec1592b521a30`  
		Last Modified: Thu, 17 Nov 2022 20:53:26 GMT  
		Size: 33.2 MB (33201133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b21b9991922acb29e5eb83766973440d83c5dff502201a569be8a655fa638b9`  
		Last Modified: Thu, 17 Nov 2022 20:53:19 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:2.9` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:36d7a9bb99e7509b27965b03c101efad6c435a883bc611a8da3341256be0fa53
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.6 MB (35642829 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a1252ce6bfaaa6350d40597943ba410313c43428e825ce64692e54780b617792`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 10 Nov 2022 20:39:46 GMT
ADD file:4b51a9d40f20d2beb29d0759b161d2b9403493453beb509de4e86a5d98513f16 in / 
# Thu, 10 Nov 2022 20:39:46 GMT
CMD ["/bin/sh"]
# Fri, 11 Nov 2022 11:00:35 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 17 Nov 2022 20:49:08 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.9.5/traefik_v2.9.5_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 17 Nov 2022 20:49:08 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 17 Nov 2022 20:49:08 GMT
EXPOSE 80
# Thu, 17 Nov 2022 20:49:08 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 17 Nov 2022 20:49:09 GMT
CMD ["traefik"]
# Thu, 17 Nov 2022 20:49:09 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.9.5 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:47517142f6ba87eca6b7bdca1e0df160b74671c81e4b9605dad38c1862a43be3`  
		Last Modified: Tue, 09 Aug 2022 17:40:55 GMT  
		Size: 2.7 MB (2718439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:249449b90f641a1b63eb9b2d4acd49b56306ca96cff71672364a6b3f00c4987f`  
		Last Modified: Fri, 11 Nov 2022 11:01:22 GMT  
		Size: 663.1 KB (663136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9eea6fbc7fa23ee63e1d48d0be490a165c452521ef2b0e1f7c5251ed40770ffa`  
		Last Modified: Thu, 17 Nov 2022 20:49:38 GMT  
		Size: 32.3 MB (32260887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a8bd16405d4b4acebd8694e9d0fac0e77d431a96daede1c6e0c58e791a5c39c`  
		Last Modified: Thu, 17 Nov 2022 20:49:34 GMT  
		Size: 367.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:2.9` - linux; s390x

```console
$ docker pull traefik@sha256:7e232016b20669caff6aeba8a8fb4aef9dc2386758e3a424ad978361b4a5980d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.3 MB (37322696 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4efcef68f66f91fcd9e200d6a5a68c1711d046ae85312931e3e87808fdd91f0f`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Tue, 09 Aug 2022 17:41:54 GMT
ADD file:7489fa84133e97e4f40b13dd5159989b3594c9627d9147bfc4e33134944cc368 in / 
# Tue, 09 Aug 2022 17:41:54 GMT
CMD ["/bin/sh"]
# Fri, 07 Oct 2022 09:56:58 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 17 Nov 2022 20:43:36 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.9.5/traefik_v2.9.5_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 17 Nov 2022 20:43:38 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 17 Nov 2022 20:43:38 GMT
EXPOSE 80
# Thu, 17 Nov 2022 20:43:38 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 17 Nov 2022 20:43:38 GMT
CMD ["traefik"]
# Thu, 17 Nov 2022 20:43:38 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.9.5 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:591a603f1fa785b25e5bd31eace69b3ffb910f7586c6a8baae6d50920c4755a7`  
		Last Modified: Thu, 17 Nov 2022 20:44:04 GMT  
		Size: 34.0 MB (34038728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:905be1b9269736fe6b80197be453aac0394c6d7651d0a0e7762e2c91a42ea604`  
		Last Modified: Thu, 17 Nov 2022 20:43:59 GMT  
		Size: 369.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:2.9-windowsservercore-1809`

```console
$ docker pull traefik@sha256:5523cb7aa12ec3d990b65e609c2be0f4cb343cb4efb4fa8277744807552b759a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3650; amd64

### `traefik:2.9-windowsservercore-1809` - windows version 10.0.17763.3650; amd64

```console
$ docker pull traefik@sha256:8ab499cb74de7d769293cd802f6cdc05ac5ffd6967979069c7a0abe022d83710
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 GB (2814280892 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:295756a7319650a07766dff97c4449914951d50d038b7e9dc956cd805c38ad7b`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Sat, 05 Nov 2022 18:29:26 GMT
RUN Install update 10.0.17763.3650
# Tue, 08 Nov 2022 18:31:26 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 17 Nov 2022 20:22:44 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/traefik/traefik/releases/download/v2.9.5/traefik_v2.9.5_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Thu, 17 Nov 2022 20:22:45 GMT
EXPOSE 80
# Thu, 17 Nov 2022 20:22:46 GMT
ENTRYPOINT ["/traefik"]
# Thu, 17 Nov 2022 20:22:47 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.9.5 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:a48a3e4ae2de839d8e99bde16eb91d113fb2cf889bba472d0c4274851b5fb402`  
		Last Modified: Tue, 21 Jun 2022 18:30:17 GMT  
		Size: 1.9 GB (1924269350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c26cc6e4f9eb1ae415a5ead6f884cac597bbd57efa6cd042c878d5b54c9d2091`  
		Last Modified: Tue, 08 Nov 2022 19:44:35 GMT  
		Size: 854.3 MB (854317461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f182832ad6ad5ea3d4b7320fd7bfea56fb9cf8413be904e52db6ed14c8d9e36f`  
		Last Modified: Tue, 08 Nov 2022 19:42:07 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:baaa6f55c06ab87b039a446d4c41afed1de673231c65262e7e453cd85f4911ac`  
		Last Modified: Thu, 17 Nov 2022 20:23:36 GMT  
		Size: 35.7 MB (35688341 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6880ebcecd161ca978b69ed9b0ad7576045802fd6e91f6d33c5fae68b77e3dc4`  
		Last Modified: Thu, 17 Nov 2022 20:23:27 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1af037205d33fcf851e821b2621162e4c95d77aa6736ca7ceff7f6816d52c776`  
		Last Modified: Thu, 17 Nov 2022 20:23:27 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:339867d3dc3e68861d0942f7f829addffa1f0416cb59f77c53730b2e1b9cb16f`  
		Last Modified: Thu, 17 Nov 2022 20:23:27 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:2.9.5`

```console
$ docker pull traefik@sha256:ac1480ce3203541705b01d6dce40ef4bf563cdb29d5b00db88cc396fa9fa9cd5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; s390x

### `traefik:2.9.5` - linux; amd64

```console
$ docker pull traefik@sha256:6c37f2135af79e0c2e387653ff3ab9abf95eb393439f07cfcfa5e06fd4bb10bb
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.7 MB (38661782 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d3cd2c35d32c1bfe78d93c2fda68314b39de4f405ff4f82c86eebd3420d108b3`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Tue, 09 Aug 2022 17:20:00 GMT
ADD file:f77e3f51f020890d22997e6c2ca98968b75b8bc8c463341a2010ff0655d4c88f in / 
# Tue, 09 Aug 2022 17:20:01 GMT
CMD ["/bin/sh"]
# Fri, 07 Oct 2022 04:21:14 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 17 Nov 2022 20:23:09 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.9.5/traefik_v2.9.5_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 17 Nov 2022 20:23:09 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 17 Nov 2022 20:23:09 GMT
EXPOSE 80
# Thu, 17 Nov 2022 20:23:09 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 17 Nov 2022 20:23:09 GMT
CMD ["traefik"]
# Thu, 17 Nov 2022 20:23:09 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.9.5 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:9ed08b51c99c95fb89d4d3eb43cacb1df34c40a394366b2ae5f94758f917c6f5`  
		Last Modified: Thu, 17 Nov 2022 20:23:40 GMT  
		Size: 35.2 MB (35164531 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2984145d314f0df14678294313f70e7a9112a1ac304a1550d6f55b3f36f95cbc`  
		Last Modified: Thu, 17 Nov 2022 20:23:34 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:2.9.5` - linux; arm variant v6

```console
$ docker pull traefik@sha256:f5bf1b659f8d381c1a13a2860015c160389af6fdfa3ab42b9c463a80150a84c3
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.5 MB (36498990 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:593023589445e011e74b841e01b331d02f3f257483cdda1d0327fdebba48c7de`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 10 Nov 2022 20:49:36 GMT
ADD file:89cb25f97e17bed5c56311280efe5cfa78422d8ffbe36232195d13f94d67417e in / 
# Thu, 10 Nov 2022 20:49:36 GMT
CMD ["/bin/sh"]
# Fri, 11 Nov 2022 11:58:35 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 17 Nov 2022 20:52:12 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.9.5/traefik_v2.9.5_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 17 Nov 2022 20:52:13 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 17 Nov 2022 20:52:13 GMT
EXPOSE 80
# Thu, 17 Nov 2022 20:52:13 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 17 Nov 2022 20:52:13 GMT
CMD ["traefik"]
# Thu, 17 Nov 2022 20:52:13 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.9.5 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:293b708aa6fb80967f27727d5c9c53ac9ba9cac376bed2ad02c17a5cca317b35`  
		Last Modified: Tue, 09 Aug 2022 17:50:52 GMT  
		Size: 2.6 MB (2631127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d346396c5843930d5c9d8e05ce83d5cc4fb94e7d986b9a31ed533e815c10e155`  
		Last Modified: Fri, 11 Nov 2022 12:00:08 GMT  
		Size: 666.4 KB (666362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cff7ec90e94457bb22f14c6a7c1c13725a823452f45c5ae834ec1592b521a30`  
		Last Modified: Thu, 17 Nov 2022 20:53:26 GMT  
		Size: 33.2 MB (33201133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b21b9991922acb29e5eb83766973440d83c5dff502201a569be8a655fa638b9`  
		Last Modified: Thu, 17 Nov 2022 20:53:19 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:2.9.5` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:36d7a9bb99e7509b27965b03c101efad6c435a883bc611a8da3341256be0fa53
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.6 MB (35642829 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a1252ce6bfaaa6350d40597943ba410313c43428e825ce64692e54780b617792`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 10 Nov 2022 20:39:46 GMT
ADD file:4b51a9d40f20d2beb29d0759b161d2b9403493453beb509de4e86a5d98513f16 in / 
# Thu, 10 Nov 2022 20:39:46 GMT
CMD ["/bin/sh"]
# Fri, 11 Nov 2022 11:00:35 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 17 Nov 2022 20:49:08 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.9.5/traefik_v2.9.5_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 17 Nov 2022 20:49:08 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 17 Nov 2022 20:49:08 GMT
EXPOSE 80
# Thu, 17 Nov 2022 20:49:08 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 17 Nov 2022 20:49:09 GMT
CMD ["traefik"]
# Thu, 17 Nov 2022 20:49:09 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.9.5 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:47517142f6ba87eca6b7bdca1e0df160b74671c81e4b9605dad38c1862a43be3`  
		Last Modified: Tue, 09 Aug 2022 17:40:55 GMT  
		Size: 2.7 MB (2718439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:249449b90f641a1b63eb9b2d4acd49b56306ca96cff71672364a6b3f00c4987f`  
		Last Modified: Fri, 11 Nov 2022 11:01:22 GMT  
		Size: 663.1 KB (663136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9eea6fbc7fa23ee63e1d48d0be490a165c452521ef2b0e1f7c5251ed40770ffa`  
		Last Modified: Thu, 17 Nov 2022 20:49:38 GMT  
		Size: 32.3 MB (32260887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a8bd16405d4b4acebd8694e9d0fac0e77d431a96daede1c6e0c58e791a5c39c`  
		Last Modified: Thu, 17 Nov 2022 20:49:34 GMT  
		Size: 367.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:2.9.5` - linux; s390x

```console
$ docker pull traefik@sha256:7e232016b20669caff6aeba8a8fb4aef9dc2386758e3a424ad978361b4a5980d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.3 MB (37322696 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4efcef68f66f91fcd9e200d6a5a68c1711d046ae85312931e3e87808fdd91f0f`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Tue, 09 Aug 2022 17:41:54 GMT
ADD file:7489fa84133e97e4f40b13dd5159989b3594c9627d9147bfc4e33134944cc368 in / 
# Tue, 09 Aug 2022 17:41:54 GMT
CMD ["/bin/sh"]
# Fri, 07 Oct 2022 09:56:58 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 17 Nov 2022 20:43:36 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.9.5/traefik_v2.9.5_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 17 Nov 2022 20:43:38 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 17 Nov 2022 20:43:38 GMT
EXPOSE 80
# Thu, 17 Nov 2022 20:43:38 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 17 Nov 2022 20:43:38 GMT
CMD ["traefik"]
# Thu, 17 Nov 2022 20:43:38 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.9.5 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:591a603f1fa785b25e5bd31eace69b3ffb910f7586c6a8baae6d50920c4755a7`  
		Last Modified: Thu, 17 Nov 2022 20:44:04 GMT  
		Size: 34.0 MB (34038728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:905be1b9269736fe6b80197be453aac0394c6d7651d0a0e7762e2c91a42ea604`  
		Last Modified: Thu, 17 Nov 2022 20:43:59 GMT  
		Size: 369.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:2.9.5-windowsservercore-1809`

```console
$ docker pull traefik@sha256:5523cb7aa12ec3d990b65e609c2be0f4cb343cb4efb4fa8277744807552b759a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3650; amd64

### `traefik:2.9.5-windowsservercore-1809` - windows version 10.0.17763.3650; amd64

```console
$ docker pull traefik@sha256:8ab499cb74de7d769293cd802f6cdc05ac5ffd6967979069c7a0abe022d83710
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 GB (2814280892 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:295756a7319650a07766dff97c4449914951d50d038b7e9dc956cd805c38ad7b`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Sat, 05 Nov 2022 18:29:26 GMT
RUN Install update 10.0.17763.3650
# Tue, 08 Nov 2022 18:31:26 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 17 Nov 2022 20:22:44 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/traefik/traefik/releases/download/v2.9.5/traefik_v2.9.5_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Thu, 17 Nov 2022 20:22:45 GMT
EXPOSE 80
# Thu, 17 Nov 2022 20:22:46 GMT
ENTRYPOINT ["/traefik"]
# Thu, 17 Nov 2022 20:22:47 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.9.5 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:a48a3e4ae2de839d8e99bde16eb91d113fb2cf889bba472d0c4274851b5fb402`  
		Last Modified: Tue, 21 Jun 2022 18:30:17 GMT  
		Size: 1.9 GB (1924269350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c26cc6e4f9eb1ae415a5ead6f884cac597bbd57efa6cd042c878d5b54c9d2091`  
		Last Modified: Tue, 08 Nov 2022 19:44:35 GMT  
		Size: 854.3 MB (854317461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f182832ad6ad5ea3d4b7320fd7bfea56fb9cf8413be904e52db6ed14c8d9e36f`  
		Last Modified: Tue, 08 Nov 2022 19:42:07 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:baaa6f55c06ab87b039a446d4c41afed1de673231c65262e7e453cd85f4911ac`  
		Last Modified: Thu, 17 Nov 2022 20:23:36 GMT  
		Size: 35.7 MB (35688341 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6880ebcecd161ca978b69ed9b0ad7576045802fd6e91f6d33c5fae68b77e3dc4`  
		Last Modified: Thu, 17 Nov 2022 20:23:27 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1af037205d33fcf851e821b2621162e4c95d77aa6736ca7ceff7f6816d52c776`  
		Last Modified: Thu, 17 Nov 2022 20:23:27 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:339867d3dc3e68861d0942f7f829addffa1f0416cb59f77c53730b2e1b9cb16f`  
		Last Modified: Thu, 17 Nov 2022 20:23:27 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:3.0`

```console
$ docker pull traefik@sha256:e27e08111cced4a2505f7e86c9987cdc88e841e00cc04d628c5d9e1dcd75577c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; s390x

### `traefik:3.0` - linux; amd64

```console
$ docker pull traefik@sha256:224603be70dbfe0438286ab45c22b157b70234c8ac3afbcb15751d0e8b212f8e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.6 MB (40558414 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8b876a2fdfb1f94a358fb4c23f6e9bcd2855f5ce3fd6303f00d54b069d32580a`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Tue, 09 Aug 2022 17:20:00 GMT
ADD file:f77e3f51f020890d22997e6c2ca98968b75b8bc8c463341a2010ff0655d4c88f in / 
# Tue, 09 Aug 2022 17:20:01 GMT
CMD ["/bin/sh"]
# Fri, 07 Oct 2022 04:21:14 GMT
RUN apk --no-cache add ca-certificates tzdata
# Mon, 05 Dec 2022 21:36:42 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v3.0.0-beta1/traefik_v3.0.0-beta1_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Mon, 05 Dec 2022 21:36:42 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Mon, 05 Dec 2022 21:36:42 GMT
EXPOSE 80
# Mon, 05 Dec 2022 21:36:43 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 05 Dec 2022 21:36:43 GMT
CMD ["traefik"]
# Mon, 05 Dec 2022 21:36:43 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v3.0.0-beta1 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:4e4dc523606876763876f4a13f05642485a71df1b2d01800d1ad801fdef562d8`  
		Last Modified: Mon, 05 Dec 2022 21:37:19 GMT  
		Size: 37.1 MB (37061162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d669c768802639b8ed02105961df833c99d47466f0d3f568128b38f6564a6d5`  
		Last Modified: Mon, 05 Dec 2022 21:37:13 GMT  
		Size: 369.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:3.0` - linux; arm variant v6

```console
$ docker pull traefik@sha256:1a69ddf9abf4ec0a9b001b130e3362c704a6c9a6a9214a464142dd2a4e238b51
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.3 MB (38283031 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:02951a4586be09d87dc08106378ce66df26ac6b34bee71362d85a61212081c3e`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 10 Nov 2022 20:49:36 GMT
ADD file:89cb25f97e17bed5c56311280efe5cfa78422d8ffbe36232195d13f94d67417e in / 
# Thu, 10 Nov 2022 20:49:36 GMT
CMD ["/bin/sh"]
# Fri, 11 Nov 2022 11:58:35 GMT
RUN apk --no-cache add ca-certificates tzdata
# Mon, 05 Dec 2022 21:06:01 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v3.0.0-beta1/traefik_v3.0.0-beta1_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Mon, 05 Dec 2022 21:06:02 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Mon, 05 Dec 2022 21:06:02 GMT
EXPOSE 80
# Mon, 05 Dec 2022 21:06:02 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 05 Dec 2022 21:06:02 GMT
CMD ["traefik"]
# Mon, 05 Dec 2022 21:06:02 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v3.0.0-beta1 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:293b708aa6fb80967f27727d5c9c53ac9ba9cac376bed2ad02c17a5cca317b35`  
		Last Modified: Tue, 09 Aug 2022 17:50:52 GMT  
		Size: 2.6 MB (2631127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d346396c5843930d5c9d8e05ce83d5cc4fb94e7d986b9a31ed533e815c10e155`  
		Last Modified: Fri, 11 Nov 2022 12:00:08 GMT  
		Size: 666.4 KB (666362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2de3172f44924df50c9481f232e34ad82ccb08def5bacbf80082ae32ff1a9f59`  
		Last Modified: Mon, 05 Dec 2022 21:07:35 GMT  
		Size: 35.0 MB (34985173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92d3657bce77bb11dac6a174ca320a66f72b6817e719f16a78a3e8e2460d652c`  
		Last Modified: Mon, 05 Dec 2022 21:07:27 GMT  
		Size: 369.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:3.0` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:89cd35233bb361b5da3a3892ac97c01ed73494c437447893088040a470823c84
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.4 MB (37390044 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:abbe7b1ec0b0646f7c57c8ebafeb2ed6a35a981149e7b80bbe8a8e8418dfc06c`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 10 Nov 2022 20:39:46 GMT
ADD file:4b51a9d40f20d2beb29d0759b161d2b9403493453beb509de4e86a5d98513f16 in / 
# Thu, 10 Nov 2022 20:39:46 GMT
CMD ["/bin/sh"]
# Fri, 11 Nov 2022 11:00:35 GMT
RUN apk --no-cache add ca-certificates tzdata
# Mon, 05 Dec 2022 21:32:58 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v3.0.0-beta1/traefik_v3.0.0-beta1_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Mon, 05 Dec 2022 21:32:58 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Mon, 05 Dec 2022 21:32:58 GMT
EXPOSE 80
# Mon, 05 Dec 2022 21:32:58 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 05 Dec 2022 21:32:58 GMT
CMD ["traefik"]
# Mon, 05 Dec 2022 21:32:58 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v3.0.0-beta1 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:47517142f6ba87eca6b7bdca1e0df160b74671c81e4b9605dad38c1862a43be3`  
		Last Modified: Tue, 09 Aug 2022 17:40:55 GMT  
		Size: 2.7 MB (2718439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:249449b90f641a1b63eb9b2d4acd49b56306ca96cff71672364a6b3f00c4987f`  
		Last Modified: Fri, 11 Nov 2022 11:01:22 GMT  
		Size: 663.1 KB (663136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5eb4eafd343ee373719a84e6dafb493a427f2c0c5011760065e33981fadac29e`  
		Last Modified: Mon, 05 Dec 2022 21:33:34 GMT  
		Size: 34.0 MB (34008101 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84347e8cbd45c0add87bc3449d8dab6a64e1f748a86f2266df30510267cf352b`  
		Last Modified: Mon, 05 Dec 2022 21:33:30 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:3.0` - linux; s390x

```console
$ docker pull traefik@sha256:4335bf033a523decf7404c56d5b1f5066cdf0cadd7d88b11773a4e4fe786f46c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.1 MB (39122041 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:679c37472e0f51cd5077eb893416f86bbd67f0f657e44f9a3db5c0753d295600`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Tue, 09 Aug 2022 17:41:54 GMT
ADD file:7489fa84133e97e4f40b13dd5159989b3594c9627d9147bfc4e33134944cc368 in / 
# Tue, 09 Aug 2022 17:41:54 GMT
CMD ["/bin/sh"]
# Fri, 07 Oct 2022 09:56:58 GMT
RUN apk --no-cache add ca-certificates tzdata
# Mon, 05 Dec 2022 20:58:11 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v3.0.0-beta1/traefik_v3.0.0-beta1_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Mon, 05 Dec 2022 20:58:12 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Mon, 05 Dec 2022 20:58:13 GMT
EXPOSE 80
# Mon, 05 Dec 2022 20:58:13 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 05 Dec 2022 20:58:13 GMT
CMD ["traefik"]
# Mon, 05 Dec 2022 20:58:13 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v3.0.0-beta1 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:3201ac53116b6203e861c6fb526eed5481c79f118b246a8a4c674f3e864fc4de`  
		Last Modified: Mon, 05 Dec 2022 20:58:56 GMT  
		Size: 35.8 MB (35838073 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b56600e5855f954be9975df988daaf3149e939469976015c165aad1cd531c9ca`  
		Last Modified: Mon, 05 Dec 2022 20:58:51 GMT  
		Size: 369.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:3.0-windowsservercore-1809`

```console
$ docker pull traefik@sha256:5eeae50f78f79dd84fee1bb77fe7fe7384a13dbd32ebaa5c80bc9b15d83d1d30
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3650; amd64

### `traefik:3.0-windowsservercore-1809` - windows version 10.0.17763.3650; amd64

```console
$ docker pull traefik@sha256:1caf484b3364fc839149585ff9e9df0e2f9b82a4d63d4298d0e1340ed97d82bb
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 GB (2816185547 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7adffb6e0e4ab0c0696bc04fd7838772060eef2bdc50aeb814ef49773e334801`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Sat, 05 Nov 2022 18:29:26 GMT
RUN Install update 10.0.17763.3650
# Tue, 08 Nov 2022 18:31:26 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Mon, 05 Dec 2022 21:19:02 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/traefik/traefik/releases/download/v3.0.0-beta1/traefik_v3.0.0-beta1_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Mon, 05 Dec 2022 21:19:03 GMT
EXPOSE 80
# Mon, 05 Dec 2022 21:19:04 GMT
ENTRYPOINT ["/traefik"]
# Mon, 05 Dec 2022 21:19:05 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v3.0.0-beta1 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:a48a3e4ae2de839d8e99bde16eb91d113fb2cf889bba472d0c4274851b5fb402`  
		Last Modified: Tue, 21 Jun 2022 18:30:17 GMT  
		Size: 1.9 GB (1924269350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c26cc6e4f9eb1ae415a5ead6f884cac597bbd57efa6cd042c878d5b54c9d2091`  
		Last Modified: Tue, 08 Nov 2022 19:44:35 GMT  
		Size: 854.3 MB (854317461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f182832ad6ad5ea3d4b7320fd7bfea56fb9cf8413be904e52db6ed14c8d9e36f`  
		Last Modified: Tue, 08 Nov 2022 19:42:07 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bf10c072ea1decad27162e33014b87a4a0d893a08f6259c83615886f7689580`  
		Last Modified: Mon, 05 Dec 2022 21:20:11 GMT  
		Size: 37.6 MB (37593045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b816ab54a1f9bf5eb43e0aea31c4b44fdec25fa6db44d02f58eb46cf021eb730`  
		Last Modified: Mon, 05 Dec 2022 21:19:57 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff05f49a360e835df322dccf350bd6ff8d907a67ce3ff32dad883a3e9ac66d61`  
		Last Modified: Mon, 05 Dec 2022 21:19:56 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9019e3961bc041a48bf292b9992be18498cc417cd524c779548b66686b7586c1`  
		Last Modified: Mon, 05 Dec 2022 21:19:57 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:3.0.0-beta1`

```console
$ docker pull traefik@sha256:e27e08111cced4a2505f7e86c9987cdc88e841e00cc04d628c5d9e1dcd75577c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; s390x

### `traefik:3.0.0-beta1` - linux; amd64

```console
$ docker pull traefik@sha256:224603be70dbfe0438286ab45c22b157b70234c8ac3afbcb15751d0e8b212f8e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.6 MB (40558414 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8b876a2fdfb1f94a358fb4c23f6e9bcd2855f5ce3fd6303f00d54b069d32580a`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Tue, 09 Aug 2022 17:20:00 GMT
ADD file:f77e3f51f020890d22997e6c2ca98968b75b8bc8c463341a2010ff0655d4c88f in / 
# Tue, 09 Aug 2022 17:20:01 GMT
CMD ["/bin/sh"]
# Fri, 07 Oct 2022 04:21:14 GMT
RUN apk --no-cache add ca-certificates tzdata
# Mon, 05 Dec 2022 21:36:42 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v3.0.0-beta1/traefik_v3.0.0-beta1_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Mon, 05 Dec 2022 21:36:42 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Mon, 05 Dec 2022 21:36:42 GMT
EXPOSE 80
# Mon, 05 Dec 2022 21:36:43 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 05 Dec 2022 21:36:43 GMT
CMD ["traefik"]
# Mon, 05 Dec 2022 21:36:43 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v3.0.0-beta1 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:4e4dc523606876763876f4a13f05642485a71df1b2d01800d1ad801fdef562d8`  
		Last Modified: Mon, 05 Dec 2022 21:37:19 GMT  
		Size: 37.1 MB (37061162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d669c768802639b8ed02105961df833c99d47466f0d3f568128b38f6564a6d5`  
		Last Modified: Mon, 05 Dec 2022 21:37:13 GMT  
		Size: 369.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:3.0.0-beta1` - linux; arm variant v6

```console
$ docker pull traefik@sha256:1a69ddf9abf4ec0a9b001b130e3362c704a6c9a6a9214a464142dd2a4e238b51
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.3 MB (38283031 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:02951a4586be09d87dc08106378ce66df26ac6b34bee71362d85a61212081c3e`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 10 Nov 2022 20:49:36 GMT
ADD file:89cb25f97e17bed5c56311280efe5cfa78422d8ffbe36232195d13f94d67417e in / 
# Thu, 10 Nov 2022 20:49:36 GMT
CMD ["/bin/sh"]
# Fri, 11 Nov 2022 11:58:35 GMT
RUN apk --no-cache add ca-certificates tzdata
# Mon, 05 Dec 2022 21:06:01 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v3.0.0-beta1/traefik_v3.0.0-beta1_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Mon, 05 Dec 2022 21:06:02 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Mon, 05 Dec 2022 21:06:02 GMT
EXPOSE 80
# Mon, 05 Dec 2022 21:06:02 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 05 Dec 2022 21:06:02 GMT
CMD ["traefik"]
# Mon, 05 Dec 2022 21:06:02 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v3.0.0-beta1 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:293b708aa6fb80967f27727d5c9c53ac9ba9cac376bed2ad02c17a5cca317b35`  
		Last Modified: Tue, 09 Aug 2022 17:50:52 GMT  
		Size: 2.6 MB (2631127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d346396c5843930d5c9d8e05ce83d5cc4fb94e7d986b9a31ed533e815c10e155`  
		Last Modified: Fri, 11 Nov 2022 12:00:08 GMT  
		Size: 666.4 KB (666362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2de3172f44924df50c9481f232e34ad82ccb08def5bacbf80082ae32ff1a9f59`  
		Last Modified: Mon, 05 Dec 2022 21:07:35 GMT  
		Size: 35.0 MB (34985173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92d3657bce77bb11dac6a174ca320a66f72b6817e719f16a78a3e8e2460d652c`  
		Last Modified: Mon, 05 Dec 2022 21:07:27 GMT  
		Size: 369.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:3.0.0-beta1` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:89cd35233bb361b5da3a3892ac97c01ed73494c437447893088040a470823c84
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.4 MB (37390044 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:abbe7b1ec0b0646f7c57c8ebafeb2ed6a35a981149e7b80bbe8a8e8418dfc06c`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 10 Nov 2022 20:39:46 GMT
ADD file:4b51a9d40f20d2beb29d0759b161d2b9403493453beb509de4e86a5d98513f16 in / 
# Thu, 10 Nov 2022 20:39:46 GMT
CMD ["/bin/sh"]
# Fri, 11 Nov 2022 11:00:35 GMT
RUN apk --no-cache add ca-certificates tzdata
# Mon, 05 Dec 2022 21:32:58 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v3.0.0-beta1/traefik_v3.0.0-beta1_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Mon, 05 Dec 2022 21:32:58 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Mon, 05 Dec 2022 21:32:58 GMT
EXPOSE 80
# Mon, 05 Dec 2022 21:32:58 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 05 Dec 2022 21:32:58 GMT
CMD ["traefik"]
# Mon, 05 Dec 2022 21:32:58 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v3.0.0-beta1 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:47517142f6ba87eca6b7bdca1e0df160b74671c81e4b9605dad38c1862a43be3`  
		Last Modified: Tue, 09 Aug 2022 17:40:55 GMT  
		Size: 2.7 MB (2718439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:249449b90f641a1b63eb9b2d4acd49b56306ca96cff71672364a6b3f00c4987f`  
		Last Modified: Fri, 11 Nov 2022 11:01:22 GMT  
		Size: 663.1 KB (663136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5eb4eafd343ee373719a84e6dafb493a427f2c0c5011760065e33981fadac29e`  
		Last Modified: Mon, 05 Dec 2022 21:33:34 GMT  
		Size: 34.0 MB (34008101 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84347e8cbd45c0add87bc3449d8dab6a64e1f748a86f2266df30510267cf352b`  
		Last Modified: Mon, 05 Dec 2022 21:33:30 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:3.0.0-beta1` - linux; s390x

```console
$ docker pull traefik@sha256:4335bf033a523decf7404c56d5b1f5066cdf0cadd7d88b11773a4e4fe786f46c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.1 MB (39122041 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:679c37472e0f51cd5077eb893416f86bbd67f0f657e44f9a3db5c0753d295600`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Tue, 09 Aug 2022 17:41:54 GMT
ADD file:7489fa84133e97e4f40b13dd5159989b3594c9627d9147bfc4e33134944cc368 in / 
# Tue, 09 Aug 2022 17:41:54 GMT
CMD ["/bin/sh"]
# Fri, 07 Oct 2022 09:56:58 GMT
RUN apk --no-cache add ca-certificates tzdata
# Mon, 05 Dec 2022 20:58:11 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v3.0.0-beta1/traefik_v3.0.0-beta1_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Mon, 05 Dec 2022 20:58:12 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Mon, 05 Dec 2022 20:58:13 GMT
EXPOSE 80
# Mon, 05 Dec 2022 20:58:13 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 05 Dec 2022 20:58:13 GMT
CMD ["traefik"]
# Mon, 05 Dec 2022 20:58:13 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v3.0.0-beta1 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:3201ac53116b6203e861c6fb526eed5481c79f118b246a8a4c674f3e864fc4de`  
		Last Modified: Mon, 05 Dec 2022 20:58:56 GMT  
		Size: 35.8 MB (35838073 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b56600e5855f954be9975df988daaf3149e939469976015c165aad1cd531c9ca`  
		Last Modified: Mon, 05 Dec 2022 20:58:51 GMT  
		Size: 369.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:3.0.0-beta1-windowsservercore-1809`

```console
$ docker pull traefik@sha256:5eeae50f78f79dd84fee1bb77fe7fe7384a13dbd32ebaa5c80bc9b15d83d1d30
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3650; amd64

### `traefik:3.0.0-beta1-windowsservercore-1809` - windows version 10.0.17763.3650; amd64

```console
$ docker pull traefik@sha256:1caf484b3364fc839149585ff9e9df0e2f9b82a4d63d4298d0e1340ed97d82bb
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 GB (2816185547 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7adffb6e0e4ab0c0696bc04fd7838772060eef2bdc50aeb814ef49773e334801`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Sat, 05 Nov 2022 18:29:26 GMT
RUN Install update 10.0.17763.3650
# Tue, 08 Nov 2022 18:31:26 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Mon, 05 Dec 2022 21:19:02 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/traefik/traefik/releases/download/v3.0.0-beta1/traefik_v3.0.0-beta1_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Mon, 05 Dec 2022 21:19:03 GMT
EXPOSE 80
# Mon, 05 Dec 2022 21:19:04 GMT
ENTRYPOINT ["/traefik"]
# Mon, 05 Dec 2022 21:19:05 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v3.0.0-beta1 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:a48a3e4ae2de839d8e99bde16eb91d113fb2cf889bba472d0c4274851b5fb402`  
		Last Modified: Tue, 21 Jun 2022 18:30:17 GMT  
		Size: 1.9 GB (1924269350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c26cc6e4f9eb1ae415a5ead6f884cac597bbd57efa6cd042c878d5b54c9d2091`  
		Last Modified: Tue, 08 Nov 2022 19:44:35 GMT  
		Size: 854.3 MB (854317461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f182832ad6ad5ea3d4b7320fd7bfea56fb9cf8413be904e52db6ed14c8d9e36f`  
		Last Modified: Tue, 08 Nov 2022 19:42:07 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bf10c072ea1decad27162e33014b87a4a0d893a08f6259c83615886f7689580`  
		Last Modified: Mon, 05 Dec 2022 21:20:11 GMT  
		Size: 37.6 MB (37593045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b816ab54a1f9bf5eb43e0aea31c4b44fdec25fa6db44d02f58eb46cf021eb730`  
		Last Modified: Mon, 05 Dec 2022 21:19:57 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff05f49a360e835df322dccf350bd6ff8d907a67ce3ff32dad883a3e9ac66d61`  
		Last Modified: Mon, 05 Dec 2022 21:19:56 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9019e3961bc041a48bf292b9992be18498cc417cd524c779548b66686b7586c1`  
		Last Modified: Mon, 05 Dec 2022 21:19:57 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:banon`

```console
$ docker pull traefik@sha256:ac1480ce3203541705b01d6dce40ef4bf563cdb29d5b00db88cc396fa9fa9cd5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; s390x

### `traefik:banon` - linux; amd64

```console
$ docker pull traefik@sha256:6c37f2135af79e0c2e387653ff3ab9abf95eb393439f07cfcfa5e06fd4bb10bb
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.7 MB (38661782 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d3cd2c35d32c1bfe78d93c2fda68314b39de4f405ff4f82c86eebd3420d108b3`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Tue, 09 Aug 2022 17:20:00 GMT
ADD file:f77e3f51f020890d22997e6c2ca98968b75b8bc8c463341a2010ff0655d4c88f in / 
# Tue, 09 Aug 2022 17:20:01 GMT
CMD ["/bin/sh"]
# Fri, 07 Oct 2022 04:21:14 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 17 Nov 2022 20:23:09 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.9.5/traefik_v2.9.5_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 17 Nov 2022 20:23:09 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 17 Nov 2022 20:23:09 GMT
EXPOSE 80
# Thu, 17 Nov 2022 20:23:09 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 17 Nov 2022 20:23:09 GMT
CMD ["traefik"]
# Thu, 17 Nov 2022 20:23:09 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.9.5 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:9ed08b51c99c95fb89d4d3eb43cacb1df34c40a394366b2ae5f94758f917c6f5`  
		Last Modified: Thu, 17 Nov 2022 20:23:40 GMT  
		Size: 35.2 MB (35164531 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2984145d314f0df14678294313f70e7a9112a1ac304a1550d6f55b3f36f95cbc`  
		Last Modified: Thu, 17 Nov 2022 20:23:34 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:banon` - linux; arm variant v6

```console
$ docker pull traefik@sha256:f5bf1b659f8d381c1a13a2860015c160389af6fdfa3ab42b9c463a80150a84c3
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.5 MB (36498990 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:593023589445e011e74b841e01b331d02f3f257483cdda1d0327fdebba48c7de`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 10 Nov 2022 20:49:36 GMT
ADD file:89cb25f97e17bed5c56311280efe5cfa78422d8ffbe36232195d13f94d67417e in / 
# Thu, 10 Nov 2022 20:49:36 GMT
CMD ["/bin/sh"]
# Fri, 11 Nov 2022 11:58:35 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 17 Nov 2022 20:52:12 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.9.5/traefik_v2.9.5_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 17 Nov 2022 20:52:13 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 17 Nov 2022 20:52:13 GMT
EXPOSE 80
# Thu, 17 Nov 2022 20:52:13 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 17 Nov 2022 20:52:13 GMT
CMD ["traefik"]
# Thu, 17 Nov 2022 20:52:13 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.9.5 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:293b708aa6fb80967f27727d5c9c53ac9ba9cac376bed2ad02c17a5cca317b35`  
		Last Modified: Tue, 09 Aug 2022 17:50:52 GMT  
		Size: 2.6 MB (2631127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d346396c5843930d5c9d8e05ce83d5cc4fb94e7d986b9a31ed533e815c10e155`  
		Last Modified: Fri, 11 Nov 2022 12:00:08 GMT  
		Size: 666.4 KB (666362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cff7ec90e94457bb22f14c6a7c1c13725a823452f45c5ae834ec1592b521a30`  
		Last Modified: Thu, 17 Nov 2022 20:53:26 GMT  
		Size: 33.2 MB (33201133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b21b9991922acb29e5eb83766973440d83c5dff502201a569be8a655fa638b9`  
		Last Modified: Thu, 17 Nov 2022 20:53:19 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:banon` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:36d7a9bb99e7509b27965b03c101efad6c435a883bc611a8da3341256be0fa53
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.6 MB (35642829 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a1252ce6bfaaa6350d40597943ba410313c43428e825ce64692e54780b617792`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 10 Nov 2022 20:39:46 GMT
ADD file:4b51a9d40f20d2beb29d0759b161d2b9403493453beb509de4e86a5d98513f16 in / 
# Thu, 10 Nov 2022 20:39:46 GMT
CMD ["/bin/sh"]
# Fri, 11 Nov 2022 11:00:35 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 17 Nov 2022 20:49:08 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.9.5/traefik_v2.9.5_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 17 Nov 2022 20:49:08 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 17 Nov 2022 20:49:08 GMT
EXPOSE 80
# Thu, 17 Nov 2022 20:49:08 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 17 Nov 2022 20:49:09 GMT
CMD ["traefik"]
# Thu, 17 Nov 2022 20:49:09 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.9.5 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:47517142f6ba87eca6b7bdca1e0df160b74671c81e4b9605dad38c1862a43be3`  
		Last Modified: Tue, 09 Aug 2022 17:40:55 GMT  
		Size: 2.7 MB (2718439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:249449b90f641a1b63eb9b2d4acd49b56306ca96cff71672364a6b3f00c4987f`  
		Last Modified: Fri, 11 Nov 2022 11:01:22 GMT  
		Size: 663.1 KB (663136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9eea6fbc7fa23ee63e1d48d0be490a165c452521ef2b0e1f7c5251ed40770ffa`  
		Last Modified: Thu, 17 Nov 2022 20:49:38 GMT  
		Size: 32.3 MB (32260887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a8bd16405d4b4acebd8694e9d0fac0e77d431a96daede1c6e0c58e791a5c39c`  
		Last Modified: Thu, 17 Nov 2022 20:49:34 GMT  
		Size: 367.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:banon` - linux; s390x

```console
$ docker pull traefik@sha256:7e232016b20669caff6aeba8a8fb4aef9dc2386758e3a424ad978361b4a5980d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.3 MB (37322696 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4efcef68f66f91fcd9e200d6a5a68c1711d046ae85312931e3e87808fdd91f0f`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Tue, 09 Aug 2022 17:41:54 GMT
ADD file:7489fa84133e97e4f40b13dd5159989b3594c9627d9147bfc4e33134944cc368 in / 
# Tue, 09 Aug 2022 17:41:54 GMT
CMD ["/bin/sh"]
# Fri, 07 Oct 2022 09:56:58 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 17 Nov 2022 20:43:36 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.9.5/traefik_v2.9.5_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 17 Nov 2022 20:43:38 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 17 Nov 2022 20:43:38 GMT
EXPOSE 80
# Thu, 17 Nov 2022 20:43:38 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 17 Nov 2022 20:43:38 GMT
CMD ["traefik"]
# Thu, 17 Nov 2022 20:43:38 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.9.5 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:591a603f1fa785b25e5bd31eace69b3ffb910f7586c6a8baae6d50920c4755a7`  
		Last Modified: Thu, 17 Nov 2022 20:44:04 GMT  
		Size: 34.0 MB (34038728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:905be1b9269736fe6b80197be453aac0394c6d7651d0a0e7762e2c91a42ea604`  
		Last Modified: Thu, 17 Nov 2022 20:43:59 GMT  
		Size: 369.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:banon-windowsservercore-1809`

```console
$ docker pull traefik@sha256:5523cb7aa12ec3d990b65e609c2be0f4cb343cb4efb4fa8277744807552b759a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3650; amd64

### `traefik:banon-windowsservercore-1809` - windows version 10.0.17763.3650; amd64

```console
$ docker pull traefik@sha256:8ab499cb74de7d769293cd802f6cdc05ac5ffd6967979069c7a0abe022d83710
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 GB (2814280892 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:295756a7319650a07766dff97c4449914951d50d038b7e9dc956cd805c38ad7b`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Sat, 05 Nov 2022 18:29:26 GMT
RUN Install update 10.0.17763.3650
# Tue, 08 Nov 2022 18:31:26 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 17 Nov 2022 20:22:44 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/traefik/traefik/releases/download/v2.9.5/traefik_v2.9.5_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Thu, 17 Nov 2022 20:22:45 GMT
EXPOSE 80
# Thu, 17 Nov 2022 20:22:46 GMT
ENTRYPOINT ["/traefik"]
# Thu, 17 Nov 2022 20:22:47 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.9.5 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:a48a3e4ae2de839d8e99bde16eb91d113fb2cf889bba472d0c4274851b5fb402`  
		Last Modified: Tue, 21 Jun 2022 18:30:17 GMT  
		Size: 1.9 GB (1924269350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c26cc6e4f9eb1ae415a5ead6f884cac597bbd57efa6cd042c878d5b54c9d2091`  
		Last Modified: Tue, 08 Nov 2022 19:44:35 GMT  
		Size: 854.3 MB (854317461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f182832ad6ad5ea3d4b7320fd7bfea56fb9cf8413be904e52db6ed14c8d9e36f`  
		Last Modified: Tue, 08 Nov 2022 19:42:07 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:baaa6f55c06ab87b039a446d4c41afed1de673231c65262e7e453cd85f4911ac`  
		Last Modified: Thu, 17 Nov 2022 20:23:36 GMT  
		Size: 35.7 MB (35688341 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6880ebcecd161ca978b69ed9b0ad7576045802fd6e91f6d33c5fae68b77e3dc4`  
		Last Modified: Thu, 17 Nov 2022 20:23:27 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1af037205d33fcf851e821b2621162e4c95d77aa6736ca7ceff7f6816d52c776`  
		Last Modified: Thu, 17 Nov 2022 20:23:27 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:339867d3dc3e68861d0942f7f829addffa1f0416cb59f77c53730b2e1b9cb16f`  
		Last Modified: Thu, 17 Nov 2022 20:23:27 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:beaufort`

```console
$ docker pull traefik@sha256:e27e08111cced4a2505f7e86c9987cdc88e841e00cc04d628c5d9e1dcd75577c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; s390x

### `traefik:beaufort` - linux; amd64

```console
$ docker pull traefik@sha256:224603be70dbfe0438286ab45c22b157b70234c8ac3afbcb15751d0e8b212f8e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.6 MB (40558414 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8b876a2fdfb1f94a358fb4c23f6e9bcd2855f5ce3fd6303f00d54b069d32580a`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Tue, 09 Aug 2022 17:20:00 GMT
ADD file:f77e3f51f020890d22997e6c2ca98968b75b8bc8c463341a2010ff0655d4c88f in / 
# Tue, 09 Aug 2022 17:20:01 GMT
CMD ["/bin/sh"]
# Fri, 07 Oct 2022 04:21:14 GMT
RUN apk --no-cache add ca-certificates tzdata
# Mon, 05 Dec 2022 21:36:42 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v3.0.0-beta1/traefik_v3.0.0-beta1_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Mon, 05 Dec 2022 21:36:42 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Mon, 05 Dec 2022 21:36:42 GMT
EXPOSE 80
# Mon, 05 Dec 2022 21:36:43 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 05 Dec 2022 21:36:43 GMT
CMD ["traefik"]
# Mon, 05 Dec 2022 21:36:43 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v3.0.0-beta1 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:4e4dc523606876763876f4a13f05642485a71df1b2d01800d1ad801fdef562d8`  
		Last Modified: Mon, 05 Dec 2022 21:37:19 GMT  
		Size: 37.1 MB (37061162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d669c768802639b8ed02105961df833c99d47466f0d3f568128b38f6564a6d5`  
		Last Modified: Mon, 05 Dec 2022 21:37:13 GMT  
		Size: 369.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:beaufort` - linux; arm variant v6

```console
$ docker pull traefik@sha256:1a69ddf9abf4ec0a9b001b130e3362c704a6c9a6a9214a464142dd2a4e238b51
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.3 MB (38283031 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:02951a4586be09d87dc08106378ce66df26ac6b34bee71362d85a61212081c3e`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 10 Nov 2022 20:49:36 GMT
ADD file:89cb25f97e17bed5c56311280efe5cfa78422d8ffbe36232195d13f94d67417e in / 
# Thu, 10 Nov 2022 20:49:36 GMT
CMD ["/bin/sh"]
# Fri, 11 Nov 2022 11:58:35 GMT
RUN apk --no-cache add ca-certificates tzdata
# Mon, 05 Dec 2022 21:06:01 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v3.0.0-beta1/traefik_v3.0.0-beta1_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Mon, 05 Dec 2022 21:06:02 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Mon, 05 Dec 2022 21:06:02 GMT
EXPOSE 80
# Mon, 05 Dec 2022 21:06:02 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 05 Dec 2022 21:06:02 GMT
CMD ["traefik"]
# Mon, 05 Dec 2022 21:06:02 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v3.0.0-beta1 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:293b708aa6fb80967f27727d5c9c53ac9ba9cac376bed2ad02c17a5cca317b35`  
		Last Modified: Tue, 09 Aug 2022 17:50:52 GMT  
		Size: 2.6 MB (2631127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d346396c5843930d5c9d8e05ce83d5cc4fb94e7d986b9a31ed533e815c10e155`  
		Last Modified: Fri, 11 Nov 2022 12:00:08 GMT  
		Size: 666.4 KB (666362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2de3172f44924df50c9481f232e34ad82ccb08def5bacbf80082ae32ff1a9f59`  
		Last Modified: Mon, 05 Dec 2022 21:07:35 GMT  
		Size: 35.0 MB (34985173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92d3657bce77bb11dac6a174ca320a66f72b6817e719f16a78a3e8e2460d652c`  
		Last Modified: Mon, 05 Dec 2022 21:07:27 GMT  
		Size: 369.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:beaufort` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:89cd35233bb361b5da3a3892ac97c01ed73494c437447893088040a470823c84
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.4 MB (37390044 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:abbe7b1ec0b0646f7c57c8ebafeb2ed6a35a981149e7b80bbe8a8e8418dfc06c`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 10 Nov 2022 20:39:46 GMT
ADD file:4b51a9d40f20d2beb29d0759b161d2b9403493453beb509de4e86a5d98513f16 in / 
# Thu, 10 Nov 2022 20:39:46 GMT
CMD ["/bin/sh"]
# Fri, 11 Nov 2022 11:00:35 GMT
RUN apk --no-cache add ca-certificates tzdata
# Mon, 05 Dec 2022 21:32:58 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v3.0.0-beta1/traefik_v3.0.0-beta1_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Mon, 05 Dec 2022 21:32:58 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Mon, 05 Dec 2022 21:32:58 GMT
EXPOSE 80
# Mon, 05 Dec 2022 21:32:58 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 05 Dec 2022 21:32:58 GMT
CMD ["traefik"]
# Mon, 05 Dec 2022 21:32:58 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v3.0.0-beta1 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:47517142f6ba87eca6b7bdca1e0df160b74671c81e4b9605dad38c1862a43be3`  
		Last Modified: Tue, 09 Aug 2022 17:40:55 GMT  
		Size: 2.7 MB (2718439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:249449b90f641a1b63eb9b2d4acd49b56306ca96cff71672364a6b3f00c4987f`  
		Last Modified: Fri, 11 Nov 2022 11:01:22 GMT  
		Size: 663.1 KB (663136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5eb4eafd343ee373719a84e6dafb493a427f2c0c5011760065e33981fadac29e`  
		Last Modified: Mon, 05 Dec 2022 21:33:34 GMT  
		Size: 34.0 MB (34008101 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84347e8cbd45c0add87bc3449d8dab6a64e1f748a86f2266df30510267cf352b`  
		Last Modified: Mon, 05 Dec 2022 21:33:30 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:beaufort` - linux; s390x

```console
$ docker pull traefik@sha256:4335bf033a523decf7404c56d5b1f5066cdf0cadd7d88b11773a4e4fe786f46c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.1 MB (39122041 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:679c37472e0f51cd5077eb893416f86bbd67f0f657e44f9a3db5c0753d295600`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Tue, 09 Aug 2022 17:41:54 GMT
ADD file:7489fa84133e97e4f40b13dd5159989b3594c9627d9147bfc4e33134944cc368 in / 
# Tue, 09 Aug 2022 17:41:54 GMT
CMD ["/bin/sh"]
# Fri, 07 Oct 2022 09:56:58 GMT
RUN apk --no-cache add ca-certificates tzdata
# Mon, 05 Dec 2022 20:58:11 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v3.0.0-beta1/traefik_v3.0.0-beta1_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Mon, 05 Dec 2022 20:58:12 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Mon, 05 Dec 2022 20:58:13 GMT
EXPOSE 80
# Mon, 05 Dec 2022 20:58:13 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 05 Dec 2022 20:58:13 GMT
CMD ["traefik"]
# Mon, 05 Dec 2022 20:58:13 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v3.0.0-beta1 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:3201ac53116b6203e861c6fb526eed5481c79f118b246a8a4c674f3e864fc4de`  
		Last Modified: Mon, 05 Dec 2022 20:58:56 GMT  
		Size: 35.8 MB (35838073 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b56600e5855f954be9975df988daaf3149e939469976015c165aad1cd531c9ca`  
		Last Modified: Mon, 05 Dec 2022 20:58:51 GMT  
		Size: 369.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:beaufort-windowsservercore-1809`

```console
$ docker pull traefik@sha256:5eeae50f78f79dd84fee1bb77fe7fe7384a13dbd32ebaa5c80bc9b15d83d1d30
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3650; amd64

### `traefik:beaufort-windowsservercore-1809` - windows version 10.0.17763.3650; amd64

```console
$ docker pull traefik@sha256:1caf484b3364fc839149585ff9e9df0e2f9b82a4d63d4298d0e1340ed97d82bb
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 GB (2816185547 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7adffb6e0e4ab0c0696bc04fd7838772060eef2bdc50aeb814ef49773e334801`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Sat, 05 Nov 2022 18:29:26 GMT
RUN Install update 10.0.17763.3650
# Tue, 08 Nov 2022 18:31:26 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Mon, 05 Dec 2022 21:19:02 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/traefik/traefik/releases/download/v3.0.0-beta1/traefik_v3.0.0-beta1_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Mon, 05 Dec 2022 21:19:03 GMT
EXPOSE 80
# Mon, 05 Dec 2022 21:19:04 GMT
ENTRYPOINT ["/traefik"]
# Mon, 05 Dec 2022 21:19:05 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v3.0.0-beta1 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:a48a3e4ae2de839d8e99bde16eb91d113fb2cf889bba472d0c4274851b5fb402`  
		Last Modified: Tue, 21 Jun 2022 18:30:17 GMT  
		Size: 1.9 GB (1924269350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c26cc6e4f9eb1ae415a5ead6f884cac597bbd57efa6cd042c878d5b54c9d2091`  
		Last Modified: Tue, 08 Nov 2022 19:44:35 GMT  
		Size: 854.3 MB (854317461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f182832ad6ad5ea3d4b7320fd7bfea56fb9cf8413be904e52db6ed14c8d9e36f`  
		Last Modified: Tue, 08 Nov 2022 19:42:07 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bf10c072ea1decad27162e33014b87a4a0d893a08f6259c83615886f7689580`  
		Last Modified: Mon, 05 Dec 2022 21:20:11 GMT  
		Size: 37.6 MB (37593045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b816ab54a1f9bf5eb43e0aea31c4b44fdec25fa6db44d02f58eb46cf021eb730`  
		Last Modified: Mon, 05 Dec 2022 21:19:57 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff05f49a360e835df322dccf350bd6ff8d907a67ce3ff32dad883a3e9ac66d61`  
		Last Modified: Mon, 05 Dec 2022 21:19:56 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9019e3961bc041a48bf292b9992be18498cc417cd524c779548b66686b7586c1`  
		Last Modified: Mon, 05 Dec 2022 21:19:57 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:latest`

```console
$ docker pull traefik@sha256:ac1480ce3203541705b01d6dce40ef4bf563cdb29d5b00db88cc396fa9fa9cd5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; s390x

### `traefik:latest` - linux; amd64

```console
$ docker pull traefik@sha256:6c37f2135af79e0c2e387653ff3ab9abf95eb393439f07cfcfa5e06fd4bb10bb
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.7 MB (38661782 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d3cd2c35d32c1bfe78d93c2fda68314b39de4f405ff4f82c86eebd3420d108b3`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Tue, 09 Aug 2022 17:20:00 GMT
ADD file:f77e3f51f020890d22997e6c2ca98968b75b8bc8c463341a2010ff0655d4c88f in / 
# Tue, 09 Aug 2022 17:20:01 GMT
CMD ["/bin/sh"]
# Fri, 07 Oct 2022 04:21:14 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 17 Nov 2022 20:23:09 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.9.5/traefik_v2.9.5_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 17 Nov 2022 20:23:09 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 17 Nov 2022 20:23:09 GMT
EXPOSE 80
# Thu, 17 Nov 2022 20:23:09 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 17 Nov 2022 20:23:09 GMT
CMD ["traefik"]
# Thu, 17 Nov 2022 20:23:09 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.9.5 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:9ed08b51c99c95fb89d4d3eb43cacb1df34c40a394366b2ae5f94758f917c6f5`  
		Last Modified: Thu, 17 Nov 2022 20:23:40 GMT  
		Size: 35.2 MB (35164531 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2984145d314f0df14678294313f70e7a9112a1ac304a1550d6f55b3f36f95cbc`  
		Last Modified: Thu, 17 Nov 2022 20:23:34 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:latest` - linux; arm variant v6

```console
$ docker pull traefik@sha256:f5bf1b659f8d381c1a13a2860015c160389af6fdfa3ab42b9c463a80150a84c3
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.5 MB (36498990 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:593023589445e011e74b841e01b331d02f3f257483cdda1d0327fdebba48c7de`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 10 Nov 2022 20:49:36 GMT
ADD file:89cb25f97e17bed5c56311280efe5cfa78422d8ffbe36232195d13f94d67417e in / 
# Thu, 10 Nov 2022 20:49:36 GMT
CMD ["/bin/sh"]
# Fri, 11 Nov 2022 11:58:35 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 17 Nov 2022 20:52:12 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.9.5/traefik_v2.9.5_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 17 Nov 2022 20:52:13 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 17 Nov 2022 20:52:13 GMT
EXPOSE 80
# Thu, 17 Nov 2022 20:52:13 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 17 Nov 2022 20:52:13 GMT
CMD ["traefik"]
# Thu, 17 Nov 2022 20:52:13 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.9.5 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:293b708aa6fb80967f27727d5c9c53ac9ba9cac376bed2ad02c17a5cca317b35`  
		Last Modified: Tue, 09 Aug 2022 17:50:52 GMT  
		Size: 2.6 MB (2631127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d346396c5843930d5c9d8e05ce83d5cc4fb94e7d986b9a31ed533e815c10e155`  
		Last Modified: Fri, 11 Nov 2022 12:00:08 GMT  
		Size: 666.4 KB (666362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cff7ec90e94457bb22f14c6a7c1c13725a823452f45c5ae834ec1592b521a30`  
		Last Modified: Thu, 17 Nov 2022 20:53:26 GMT  
		Size: 33.2 MB (33201133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b21b9991922acb29e5eb83766973440d83c5dff502201a569be8a655fa638b9`  
		Last Modified: Thu, 17 Nov 2022 20:53:19 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:latest` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:36d7a9bb99e7509b27965b03c101efad6c435a883bc611a8da3341256be0fa53
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.6 MB (35642829 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a1252ce6bfaaa6350d40597943ba410313c43428e825ce64692e54780b617792`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 10 Nov 2022 20:39:46 GMT
ADD file:4b51a9d40f20d2beb29d0759b161d2b9403493453beb509de4e86a5d98513f16 in / 
# Thu, 10 Nov 2022 20:39:46 GMT
CMD ["/bin/sh"]
# Fri, 11 Nov 2022 11:00:35 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 17 Nov 2022 20:49:08 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.9.5/traefik_v2.9.5_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 17 Nov 2022 20:49:08 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 17 Nov 2022 20:49:08 GMT
EXPOSE 80
# Thu, 17 Nov 2022 20:49:08 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 17 Nov 2022 20:49:09 GMT
CMD ["traefik"]
# Thu, 17 Nov 2022 20:49:09 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.9.5 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:47517142f6ba87eca6b7bdca1e0df160b74671c81e4b9605dad38c1862a43be3`  
		Last Modified: Tue, 09 Aug 2022 17:40:55 GMT  
		Size: 2.7 MB (2718439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:249449b90f641a1b63eb9b2d4acd49b56306ca96cff71672364a6b3f00c4987f`  
		Last Modified: Fri, 11 Nov 2022 11:01:22 GMT  
		Size: 663.1 KB (663136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9eea6fbc7fa23ee63e1d48d0be490a165c452521ef2b0e1f7c5251ed40770ffa`  
		Last Modified: Thu, 17 Nov 2022 20:49:38 GMT  
		Size: 32.3 MB (32260887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a8bd16405d4b4acebd8694e9d0fac0e77d431a96daede1c6e0c58e791a5c39c`  
		Last Modified: Thu, 17 Nov 2022 20:49:34 GMT  
		Size: 367.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:latest` - linux; s390x

```console
$ docker pull traefik@sha256:7e232016b20669caff6aeba8a8fb4aef9dc2386758e3a424ad978361b4a5980d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.3 MB (37322696 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4efcef68f66f91fcd9e200d6a5a68c1711d046ae85312931e3e87808fdd91f0f`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Tue, 09 Aug 2022 17:41:54 GMT
ADD file:7489fa84133e97e4f40b13dd5159989b3594c9627d9147bfc4e33134944cc368 in / 
# Tue, 09 Aug 2022 17:41:54 GMT
CMD ["/bin/sh"]
# Fri, 07 Oct 2022 09:56:58 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 17 Nov 2022 20:43:36 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.9.5/traefik_v2.9.5_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 17 Nov 2022 20:43:38 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 17 Nov 2022 20:43:38 GMT
EXPOSE 80
# Thu, 17 Nov 2022 20:43:38 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 17 Nov 2022 20:43:38 GMT
CMD ["traefik"]
# Thu, 17 Nov 2022 20:43:38 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.9.5 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:591a603f1fa785b25e5bd31eace69b3ffb910f7586c6a8baae6d50920c4755a7`  
		Last Modified: Thu, 17 Nov 2022 20:44:04 GMT  
		Size: 34.0 MB (34038728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:905be1b9269736fe6b80197be453aac0394c6d7651d0a0e7762e2c91a42ea604`  
		Last Modified: Thu, 17 Nov 2022 20:43:59 GMT  
		Size: 369.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:maroilles`

```console
$ docker pull traefik@sha256:3a46f4e724ac467d9e3955792bba4327e17fa2e9e1fed93f13b85fd45b71816a
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
$ docker pull traefik@sha256:ed51daf51f75bf5735027eed93829bc2ddc8cab5f7d2c92661e9ae240a812647
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **21.1 MB (21055568 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:35629440895fbdc6144fd69e6ddccee4de8aa7785af39e4804683304ac4f2df1`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Fri, 28 Oct 2022 00:15:28 GMT
COPY file:48964762d0c961c28f59ebd3ea194fb6486cf2bd9a9cf1780f6702d88bd7b7d9 in /etc/ssl/certs/ 
# Fri, 11 Nov 2022 11:59:12 GMT
COPY dir:3b1b1d8650d4180b42ead5fd074947c16b0405195b425df367fbf007be68841d in /usr/share/ 
# Fri, 11 Nov 2022 11:59:13 GMT
COPY file:5d1e7e81e8b77b4f8828eeaf0d30a0f135a949b51396f12ae22af376c36d3129 in / 
# Fri, 11 Nov 2022 11:59:14 GMT
EXPOSE 80
# Fri, 11 Nov 2022 11:59:14 GMT
VOLUME [/tmp]
# Fri, 11 Nov 2022 11:59:14 GMT
ENTRYPOINT ["/traefik"]
# Fri, 11 Nov 2022 11:59:14 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.34 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:93432fb5c46fdb5c83e424ff85db4e06a08e5ac2ec96ce9e11f1c60f5a86d29b`  
		Last Modified: Fri, 28 Oct 2022 00:17:20 GMT  
		Size: 123.5 KB (123538 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0efdacb2b2ba042055ea537001460b2cff92ff305869705801b66bc44dc8565`  
		Last Modified: Fri, 11 Nov 2022 12:01:04 GMT  
		Size: 308.7 KB (308749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:849ebe6d2d943e776e37535f360e7b0f3745d625ee69f6ee5fe1eecee5487ce1`  
		Last Modified: Fri, 11 Nov 2022 12:01:08 GMT  
		Size: 20.6 MB (20623281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:maroilles` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:ac5b287132e97dc27bbd96791a25701e051ddce973d6ee70eda1c87138e3c299
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **20.6 MB (20563697 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f9d5da1bea8e1a3e20b83ceca6e486a1e881451b1e304a0281d936d5e51f418d`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Thu, 27 Oct 2022 23:00:59 GMT
COPY file:48964762d0c961c28f59ebd3ea194fb6486cf2bd9a9cf1780f6702d88bd7b7d9 in /etc/ssl/certs/ 
# Fri, 11 Nov 2022 11:00:57 GMT
COPY dir:3b1b1d8650d4180b42ead5fd074947c16b0405195b425df367fbf007be68841d in /usr/share/ 
# Fri, 11 Nov 2022 11:00:58 GMT
COPY file:60330593b6644f3f519fd13ce8ee34c2c7ab9994a1420afabbc01926dd1230dd in / 
# Fri, 11 Nov 2022 11:00:58 GMT
EXPOSE 80
# Fri, 11 Nov 2022 11:00:58 GMT
VOLUME [/tmp]
# Fri, 11 Nov 2022 11:00:58 GMT
ENTRYPOINT ["/traefik"]
# Fri, 11 Nov 2022 11:00:58 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.34 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:384a668e636c3a58c260d7eacd140f07b0727673d5ba128334cbcedd184a99f2`  
		Last Modified: Thu, 27 Oct 2022 23:02:00 GMT  
		Size: 123.5 KB (123538 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a3f6a6b590d30fda524213974a86d6ca01981b3ab4154a359b9c2e3fa3262c6`  
		Last Modified: Fri, 11 Nov 2022 11:02:04 GMT  
		Size: 308.8 KB (308813 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2af8a7d805d81cf74f58f3793659f76132259201bea15bbb7a0edc6191f8edfa`  
		Last Modified: Fri, 11 Nov 2022 11:02:07 GMT  
		Size: 20.1 MB (20131346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:maroilles-alpine`

```console
$ docker pull traefik@sha256:f50efd68ddcb8b1b8ad030fcf1011fa6a2b42412e1339b6fe2731e73eb1db963
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
$ docker pull traefik@sha256:0ae1b77619decee480ac73c5643f221285808044b307298c32c3d6c8bad3e184
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.9 MB (23925564 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:636cce97efeea9b6e6cae06ecc42e060b6488713c0b64e8a4754f9e7439ba766`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 10 Nov 2022 20:49:43 GMT
ADD file:8ff80989f06f5a8ffe16c56e00538928dcb1e46faa2b58ab9c14c7227a6cd8f9 in / 
# Thu, 10 Nov 2022 20:49:43 GMT
CMD ["/bin/sh"]
# Fri, 11 Nov 2022 11:58:55 GMT
RUN apk --no-cache add ca-certificates tzdata
# Fri, 11 Nov 2022 11:59:00 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/traefik/traefik/releases/download/v1.7.34/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Fri, 11 Nov 2022 11:59:01 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Fri, 11 Nov 2022 11:59:01 GMT
EXPOSE 80
# Fri, 11 Nov 2022 11:59:01 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 11 Nov 2022 11:59:01 GMT
CMD ["traefik"]
# Fri, 11 Nov 2022 11:59:01 GMT
LABEL org.opencontainers.image.vendor=traefik org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.34 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:7d147289082e6aa6ef510c09d7c0ac8b5026e0b591f1bfcaf01ceada43c9ec65`  
		Last Modified: Tue, 09 Aug 2022 17:51:04 GMT  
		Size: 2.6 MB (2635498 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33435e7e7c652bea7ffaf83b027d129ebd3d136e11e2469998ccbc32288c98fa`  
		Last Modified: Fri, 11 Nov 2022 12:00:39 GMT  
		Size: 666.3 KB (666268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d38a2c13dc82440cb92fa776a94c406c832435459441a480e7bf60df1e0baed`  
		Last Modified: Fri, 11 Nov 2022 12:00:43 GMT  
		Size: 20.6 MB (20623430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aed31ebc6a3ec75add73f53bf95dd91c31a2bbdadfbf38a7b44c7b57f8fb9f8a`  
		Last Modified: Fri, 11 Nov 2022 12:00:39 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:maroilles-alpine` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:64b63c53bbf8a021857ee49412ff72501a52a4e821ffd1f3a17f213562a55dcf
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.5 MB (23517049 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7adbabdcf54e3ae316f53747af91e16d550dfdfc9afaa2e19f9d4f61a1ab2759`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 10 Nov 2022 20:39:51 GMT
ADD file:b312c8f512719efd09811d17c2b250bbad03cf3f90c135a00695cc8e152f4ee2 in / 
# Thu, 10 Nov 2022 20:39:51 GMT
CMD ["/bin/sh"]
# Fri, 11 Nov 2022 11:00:45 GMT
RUN apk --no-cache add ca-certificates tzdata
# Fri, 11 Nov 2022 11:00:51 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/traefik/traefik/releases/download/v1.7.34/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Fri, 11 Nov 2022 11:00:51 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Fri, 11 Nov 2022 11:00:51 GMT
EXPOSE 80
# Fri, 11 Nov 2022 11:00:51 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 11 Nov 2022 11:00:51 GMT
CMD ["traefik"]
# Fri, 11 Nov 2022 11:00:51 GMT
LABEL org.opencontainers.image.vendor=traefik org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.34 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:90cda3b7c32511829cd5ae9074240c36c34507085acb6e55b96f993740d2be93`  
		Last Modified: Tue, 09 Aug 2022 17:41:06 GMT  
		Size: 2.7 MB (2722153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bef289adf2cbb3f8d157193bbfd586faaa288d6dd23845f0db17b7c041df2ef`  
		Last Modified: Fri, 11 Nov 2022 11:01:45 GMT  
		Size: 663.1 KB (663148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4d7297d487dbad0e6a3001add15c558d8305d106c11a0f1d1572e3b8cb8c221`  
		Last Modified: Fri, 11 Nov 2022 11:01:47 GMT  
		Size: 20.1 MB (20131380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:238986be5500952726a82d7ee40ae56ba3acfe2c8512f680e8c1e764ba05184b`  
		Last Modified: Fri, 11 Nov 2022 11:01:44 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:maroilles-windowsservercore-1809`

```console
$ docker pull traefik@sha256:ba22fa49d06eb335a538647f8ac6b53100619cef2d6dac06269da6c557709513
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3650; amd64

### `traefik:maroilles-windowsservercore-1809` - windows version 10.0.17763.3650; amd64

```console
$ docker pull traefik@sha256:8c0df9f3b6b67923ad88bb8c325e64f06bfec58ede2be72f6161a12fb58b0514
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 GB (2801442412 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5ffbcd25321baf9b5e717f95aad8a5c850725ea21067094e561b04f95f5e73c5`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Sat, 05 Nov 2022 18:29:26 GMT
RUN Install update 10.0.17763.3650
# Tue, 08 Nov 2022 18:31:26 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Nov 2022 19:39:46 GMT
RUN Invoke-WebRequest     -Uri "https://github.com/traefik/traefik/releases/download/v1.7.34/traefik_windows-amd64.exe"     -OutFile "/traefik.exe"
# Wed, 09 Nov 2022 19:39:47 GMT
EXPOSE 80
# Wed, 09 Nov 2022 19:39:48 GMT
ENTRYPOINT ["/traefik"]
# Wed, 09 Nov 2022 19:39:50 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.34 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:a48a3e4ae2de839d8e99bde16eb91d113fb2cf889bba472d0c4274851b5fb402`  
		Last Modified: Tue, 21 Jun 2022 18:30:17 GMT  
		Size: 1.9 GB (1924269350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c26cc6e4f9eb1ae415a5ead6f884cac597bbd57efa6cd042c878d5b54c9d2091`  
		Last Modified: Tue, 08 Nov 2022 19:44:35 GMT  
		Size: 854.3 MB (854317461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f182832ad6ad5ea3d4b7320fd7bfea56fb9cf8413be904e52db6ed14c8d9e36f`  
		Last Modified: Tue, 08 Nov 2022 19:42:07 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:114e02070c38ac40033338b737577f7ed16181f6ce5ef3a282eb2a91b99c1967`  
		Last Modified: Wed, 09 Nov 2022 19:40:52 GMT  
		Size: 22.9 MB (22850203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:198ef1b6118e3b8dff31c6ada18f95988302cf4293219d1043eb9b810b79f9ec`  
		Last Modified: Wed, 09 Nov 2022 19:40:46 GMT  
		Size: 1.3 KB (1316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8499782a4e49b27eacd6a70cb60fb670341838fe2a3a9103ec45ff34bbe922c9`  
		Last Modified: Wed, 09 Nov 2022 19:40:46 GMT  
		Size: 1.3 KB (1331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aadd67eff429b70dc14789c1a0f220cf3c25607c2b6a8145d3756731eb5b771a`  
		Last Modified: Wed, 09 Nov 2022 19:40:46 GMT  
		Size: 1.3 KB (1311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v1.7`

```console
$ docker pull traefik@sha256:3a46f4e724ac467d9e3955792bba4327e17fa2e9e1fed93f13b85fd45b71816a
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
$ docker pull traefik@sha256:ed51daf51f75bf5735027eed93829bc2ddc8cab5f7d2c92661e9ae240a812647
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **21.1 MB (21055568 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:35629440895fbdc6144fd69e6ddccee4de8aa7785af39e4804683304ac4f2df1`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Fri, 28 Oct 2022 00:15:28 GMT
COPY file:48964762d0c961c28f59ebd3ea194fb6486cf2bd9a9cf1780f6702d88bd7b7d9 in /etc/ssl/certs/ 
# Fri, 11 Nov 2022 11:59:12 GMT
COPY dir:3b1b1d8650d4180b42ead5fd074947c16b0405195b425df367fbf007be68841d in /usr/share/ 
# Fri, 11 Nov 2022 11:59:13 GMT
COPY file:5d1e7e81e8b77b4f8828eeaf0d30a0f135a949b51396f12ae22af376c36d3129 in / 
# Fri, 11 Nov 2022 11:59:14 GMT
EXPOSE 80
# Fri, 11 Nov 2022 11:59:14 GMT
VOLUME [/tmp]
# Fri, 11 Nov 2022 11:59:14 GMT
ENTRYPOINT ["/traefik"]
# Fri, 11 Nov 2022 11:59:14 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.34 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:93432fb5c46fdb5c83e424ff85db4e06a08e5ac2ec96ce9e11f1c60f5a86d29b`  
		Last Modified: Fri, 28 Oct 2022 00:17:20 GMT  
		Size: 123.5 KB (123538 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0efdacb2b2ba042055ea537001460b2cff92ff305869705801b66bc44dc8565`  
		Last Modified: Fri, 11 Nov 2022 12:01:04 GMT  
		Size: 308.7 KB (308749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:849ebe6d2d943e776e37535f360e7b0f3745d625ee69f6ee5fe1eecee5487ce1`  
		Last Modified: Fri, 11 Nov 2022 12:01:08 GMT  
		Size: 20.6 MB (20623281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v1.7` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:ac5b287132e97dc27bbd96791a25701e051ddce973d6ee70eda1c87138e3c299
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **20.6 MB (20563697 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f9d5da1bea8e1a3e20b83ceca6e486a1e881451b1e304a0281d936d5e51f418d`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Thu, 27 Oct 2022 23:00:59 GMT
COPY file:48964762d0c961c28f59ebd3ea194fb6486cf2bd9a9cf1780f6702d88bd7b7d9 in /etc/ssl/certs/ 
# Fri, 11 Nov 2022 11:00:57 GMT
COPY dir:3b1b1d8650d4180b42ead5fd074947c16b0405195b425df367fbf007be68841d in /usr/share/ 
# Fri, 11 Nov 2022 11:00:58 GMT
COPY file:60330593b6644f3f519fd13ce8ee34c2c7ab9994a1420afabbc01926dd1230dd in / 
# Fri, 11 Nov 2022 11:00:58 GMT
EXPOSE 80
# Fri, 11 Nov 2022 11:00:58 GMT
VOLUME [/tmp]
# Fri, 11 Nov 2022 11:00:58 GMT
ENTRYPOINT ["/traefik"]
# Fri, 11 Nov 2022 11:00:58 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.34 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:384a668e636c3a58c260d7eacd140f07b0727673d5ba128334cbcedd184a99f2`  
		Last Modified: Thu, 27 Oct 2022 23:02:00 GMT  
		Size: 123.5 KB (123538 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a3f6a6b590d30fda524213974a86d6ca01981b3ab4154a359b9c2e3fa3262c6`  
		Last Modified: Fri, 11 Nov 2022 11:02:04 GMT  
		Size: 308.8 KB (308813 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2af8a7d805d81cf74f58f3793659f76132259201bea15bbb7a0edc6191f8edfa`  
		Last Modified: Fri, 11 Nov 2022 11:02:07 GMT  
		Size: 20.1 MB (20131346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v1.7-alpine`

```console
$ docker pull traefik@sha256:f50efd68ddcb8b1b8ad030fcf1011fa6a2b42412e1339b6fe2731e73eb1db963
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
$ docker pull traefik@sha256:0ae1b77619decee480ac73c5643f221285808044b307298c32c3d6c8bad3e184
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.9 MB (23925564 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:636cce97efeea9b6e6cae06ecc42e060b6488713c0b64e8a4754f9e7439ba766`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 10 Nov 2022 20:49:43 GMT
ADD file:8ff80989f06f5a8ffe16c56e00538928dcb1e46faa2b58ab9c14c7227a6cd8f9 in / 
# Thu, 10 Nov 2022 20:49:43 GMT
CMD ["/bin/sh"]
# Fri, 11 Nov 2022 11:58:55 GMT
RUN apk --no-cache add ca-certificates tzdata
# Fri, 11 Nov 2022 11:59:00 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/traefik/traefik/releases/download/v1.7.34/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Fri, 11 Nov 2022 11:59:01 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Fri, 11 Nov 2022 11:59:01 GMT
EXPOSE 80
# Fri, 11 Nov 2022 11:59:01 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 11 Nov 2022 11:59:01 GMT
CMD ["traefik"]
# Fri, 11 Nov 2022 11:59:01 GMT
LABEL org.opencontainers.image.vendor=traefik org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.34 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:7d147289082e6aa6ef510c09d7c0ac8b5026e0b591f1bfcaf01ceada43c9ec65`  
		Last Modified: Tue, 09 Aug 2022 17:51:04 GMT  
		Size: 2.6 MB (2635498 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33435e7e7c652bea7ffaf83b027d129ebd3d136e11e2469998ccbc32288c98fa`  
		Last Modified: Fri, 11 Nov 2022 12:00:39 GMT  
		Size: 666.3 KB (666268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d38a2c13dc82440cb92fa776a94c406c832435459441a480e7bf60df1e0baed`  
		Last Modified: Fri, 11 Nov 2022 12:00:43 GMT  
		Size: 20.6 MB (20623430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aed31ebc6a3ec75add73f53bf95dd91c31a2bbdadfbf38a7b44c7b57f8fb9f8a`  
		Last Modified: Fri, 11 Nov 2022 12:00:39 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v1.7-alpine` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:64b63c53bbf8a021857ee49412ff72501a52a4e821ffd1f3a17f213562a55dcf
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.5 MB (23517049 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7adbabdcf54e3ae316f53747af91e16d550dfdfc9afaa2e19f9d4f61a1ab2759`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 10 Nov 2022 20:39:51 GMT
ADD file:b312c8f512719efd09811d17c2b250bbad03cf3f90c135a00695cc8e152f4ee2 in / 
# Thu, 10 Nov 2022 20:39:51 GMT
CMD ["/bin/sh"]
# Fri, 11 Nov 2022 11:00:45 GMT
RUN apk --no-cache add ca-certificates tzdata
# Fri, 11 Nov 2022 11:00:51 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/traefik/traefik/releases/download/v1.7.34/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Fri, 11 Nov 2022 11:00:51 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Fri, 11 Nov 2022 11:00:51 GMT
EXPOSE 80
# Fri, 11 Nov 2022 11:00:51 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 11 Nov 2022 11:00:51 GMT
CMD ["traefik"]
# Fri, 11 Nov 2022 11:00:51 GMT
LABEL org.opencontainers.image.vendor=traefik org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.34 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:90cda3b7c32511829cd5ae9074240c36c34507085acb6e55b96f993740d2be93`  
		Last Modified: Tue, 09 Aug 2022 17:41:06 GMT  
		Size: 2.7 MB (2722153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bef289adf2cbb3f8d157193bbfd586faaa288d6dd23845f0db17b7c041df2ef`  
		Last Modified: Fri, 11 Nov 2022 11:01:45 GMT  
		Size: 663.1 KB (663148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4d7297d487dbad0e6a3001add15c558d8305d106c11a0f1d1572e3b8cb8c221`  
		Last Modified: Fri, 11 Nov 2022 11:01:47 GMT  
		Size: 20.1 MB (20131380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:238986be5500952726a82d7ee40ae56ba3acfe2c8512f680e8c1e764ba05184b`  
		Last Modified: Fri, 11 Nov 2022 11:01:44 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v1.7-windowsservercore-1809`

```console
$ docker pull traefik@sha256:ba22fa49d06eb335a538647f8ac6b53100619cef2d6dac06269da6c557709513
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3650; amd64

### `traefik:v1.7-windowsservercore-1809` - windows version 10.0.17763.3650; amd64

```console
$ docker pull traefik@sha256:8c0df9f3b6b67923ad88bb8c325e64f06bfec58ede2be72f6161a12fb58b0514
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 GB (2801442412 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5ffbcd25321baf9b5e717f95aad8a5c850725ea21067094e561b04f95f5e73c5`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Sat, 05 Nov 2022 18:29:26 GMT
RUN Install update 10.0.17763.3650
# Tue, 08 Nov 2022 18:31:26 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Nov 2022 19:39:46 GMT
RUN Invoke-WebRequest     -Uri "https://github.com/traefik/traefik/releases/download/v1.7.34/traefik_windows-amd64.exe"     -OutFile "/traefik.exe"
# Wed, 09 Nov 2022 19:39:47 GMT
EXPOSE 80
# Wed, 09 Nov 2022 19:39:48 GMT
ENTRYPOINT ["/traefik"]
# Wed, 09 Nov 2022 19:39:50 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.34 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:a48a3e4ae2de839d8e99bde16eb91d113fb2cf889bba472d0c4274851b5fb402`  
		Last Modified: Tue, 21 Jun 2022 18:30:17 GMT  
		Size: 1.9 GB (1924269350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c26cc6e4f9eb1ae415a5ead6f884cac597bbd57efa6cd042c878d5b54c9d2091`  
		Last Modified: Tue, 08 Nov 2022 19:44:35 GMT  
		Size: 854.3 MB (854317461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f182832ad6ad5ea3d4b7320fd7bfea56fb9cf8413be904e52db6ed14c8d9e36f`  
		Last Modified: Tue, 08 Nov 2022 19:42:07 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:114e02070c38ac40033338b737577f7ed16181f6ce5ef3a282eb2a91b99c1967`  
		Last Modified: Wed, 09 Nov 2022 19:40:52 GMT  
		Size: 22.9 MB (22850203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:198ef1b6118e3b8dff31c6ada18f95988302cf4293219d1043eb9b810b79f9ec`  
		Last Modified: Wed, 09 Nov 2022 19:40:46 GMT  
		Size: 1.3 KB (1316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8499782a4e49b27eacd6a70cb60fb670341838fe2a3a9103ec45ff34bbe922c9`  
		Last Modified: Wed, 09 Nov 2022 19:40:46 GMT  
		Size: 1.3 KB (1331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aadd67eff429b70dc14789c1a0f220cf3c25607c2b6a8145d3756731eb5b771a`  
		Last Modified: Wed, 09 Nov 2022 19:40:46 GMT  
		Size: 1.3 KB (1311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v1.7.34`

```console
$ docker pull traefik@sha256:3a46f4e724ac467d9e3955792bba4327e17fa2e9e1fed93f13b85fd45b71816a
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
$ docker pull traefik@sha256:ed51daf51f75bf5735027eed93829bc2ddc8cab5f7d2c92661e9ae240a812647
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **21.1 MB (21055568 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:35629440895fbdc6144fd69e6ddccee4de8aa7785af39e4804683304ac4f2df1`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Fri, 28 Oct 2022 00:15:28 GMT
COPY file:48964762d0c961c28f59ebd3ea194fb6486cf2bd9a9cf1780f6702d88bd7b7d9 in /etc/ssl/certs/ 
# Fri, 11 Nov 2022 11:59:12 GMT
COPY dir:3b1b1d8650d4180b42ead5fd074947c16b0405195b425df367fbf007be68841d in /usr/share/ 
# Fri, 11 Nov 2022 11:59:13 GMT
COPY file:5d1e7e81e8b77b4f8828eeaf0d30a0f135a949b51396f12ae22af376c36d3129 in / 
# Fri, 11 Nov 2022 11:59:14 GMT
EXPOSE 80
# Fri, 11 Nov 2022 11:59:14 GMT
VOLUME [/tmp]
# Fri, 11 Nov 2022 11:59:14 GMT
ENTRYPOINT ["/traefik"]
# Fri, 11 Nov 2022 11:59:14 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.34 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:93432fb5c46fdb5c83e424ff85db4e06a08e5ac2ec96ce9e11f1c60f5a86d29b`  
		Last Modified: Fri, 28 Oct 2022 00:17:20 GMT  
		Size: 123.5 KB (123538 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0efdacb2b2ba042055ea537001460b2cff92ff305869705801b66bc44dc8565`  
		Last Modified: Fri, 11 Nov 2022 12:01:04 GMT  
		Size: 308.7 KB (308749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:849ebe6d2d943e776e37535f360e7b0f3745d625ee69f6ee5fe1eecee5487ce1`  
		Last Modified: Fri, 11 Nov 2022 12:01:08 GMT  
		Size: 20.6 MB (20623281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v1.7.34` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:ac5b287132e97dc27bbd96791a25701e051ddce973d6ee70eda1c87138e3c299
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **20.6 MB (20563697 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f9d5da1bea8e1a3e20b83ceca6e486a1e881451b1e304a0281d936d5e51f418d`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Thu, 27 Oct 2022 23:00:59 GMT
COPY file:48964762d0c961c28f59ebd3ea194fb6486cf2bd9a9cf1780f6702d88bd7b7d9 in /etc/ssl/certs/ 
# Fri, 11 Nov 2022 11:00:57 GMT
COPY dir:3b1b1d8650d4180b42ead5fd074947c16b0405195b425df367fbf007be68841d in /usr/share/ 
# Fri, 11 Nov 2022 11:00:58 GMT
COPY file:60330593b6644f3f519fd13ce8ee34c2c7ab9994a1420afabbc01926dd1230dd in / 
# Fri, 11 Nov 2022 11:00:58 GMT
EXPOSE 80
# Fri, 11 Nov 2022 11:00:58 GMT
VOLUME [/tmp]
# Fri, 11 Nov 2022 11:00:58 GMT
ENTRYPOINT ["/traefik"]
# Fri, 11 Nov 2022 11:00:58 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.34 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:384a668e636c3a58c260d7eacd140f07b0727673d5ba128334cbcedd184a99f2`  
		Last Modified: Thu, 27 Oct 2022 23:02:00 GMT  
		Size: 123.5 KB (123538 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a3f6a6b590d30fda524213974a86d6ca01981b3ab4154a359b9c2e3fa3262c6`  
		Last Modified: Fri, 11 Nov 2022 11:02:04 GMT  
		Size: 308.8 KB (308813 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2af8a7d805d81cf74f58f3793659f76132259201bea15bbb7a0edc6191f8edfa`  
		Last Modified: Fri, 11 Nov 2022 11:02:07 GMT  
		Size: 20.1 MB (20131346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v1.7.34-alpine`

```console
$ docker pull traefik@sha256:f50efd68ddcb8b1b8ad030fcf1011fa6a2b42412e1339b6fe2731e73eb1db963
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
$ docker pull traefik@sha256:0ae1b77619decee480ac73c5643f221285808044b307298c32c3d6c8bad3e184
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.9 MB (23925564 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:636cce97efeea9b6e6cae06ecc42e060b6488713c0b64e8a4754f9e7439ba766`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 10 Nov 2022 20:49:43 GMT
ADD file:8ff80989f06f5a8ffe16c56e00538928dcb1e46faa2b58ab9c14c7227a6cd8f9 in / 
# Thu, 10 Nov 2022 20:49:43 GMT
CMD ["/bin/sh"]
# Fri, 11 Nov 2022 11:58:55 GMT
RUN apk --no-cache add ca-certificates tzdata
# Fri, 11 Nov 2022 11:59:00 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/traefik/traefik/releases/download/v1.7.34/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Fri, 11 Nov 2022 11:59:01 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Fri, 11 Nov 2022 11:59:01 GMT
EXPOSE 80
# Fri, 11 Nov 2022 11:59:01 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 11 Nov 2022 11:59:01 GMT
CMD ["traefik"]
# Fri, 11 Nov 2022 11:59:01 GMT
LABEL org.opencontainers.image.vendor=traefik org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.34 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:7d147289082e6aa6ef510c09d7c0ac8b5026e0b591f1bfcaf01ceada43c9ec65`  
		Last Modified: Tue, 09 Aug 2022 17:51:04 GMT  
		Size: 2.6 MB (2635498 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33435e7e7c652bea7ffaf83b027d129ebd3d136e11e2469998ccbc32288c98fa`  
		Last Modified: Fri, 11 Nov 2022 12:00:39 GMT  
		Size: 666.3 KB (666268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d38a2c13dc82440cb92fa776a94c406c832435459441a480e7bf60df1e0baed`  
		Last Modified: Fri, 11 Nov 2022 12:00:43 GMT  
		Size: 20.6 MB (20623430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aed31ebc6a3ec75add73f53bf95dd91c31a2bbdadfbf38a7b44c7b57f8fb9f8a`  
		Last Modified: Fri, 11 Nov 2022 12:00:39 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v1.7.34-alpine` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:64b63c53bbf8a021857ee49412ff72501a52a4e821ffd1f3a17f213562a55dcf
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.5 MB (23517049 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7adbabdcf54e3ae316f53747af91e16d550dfdfc9afaa2e19f9d4f61a1ab2759`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 10 Nov 2022 20:39:51 GMT
ADD file:b312c8f512719efd09811d17c2b250bbad03cf3f90c135a00695cc8e152f4ee2 in / 
# Thu, 10 Nov 2022 20:39:51 GMT
CMD ["/bin/sh"]
# Fri, 11 Nov 2022 11:00:45 GMT
RUN apk --no-cache add ca-certificates tzdata
# Fri, 11 Nov 2022 11:00:51 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/traefik/traefik/releases/download/v1.7.34/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Fri, 11 Nov 2022 11:00:51 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Fri, 11 Nov 2022 11:00:51 GMT
EXPOSE 80
# Fri, 11 Nov 2022 11:00:51 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 11 Nov 2022 11:00:51 GMT
CMD ["traefik"]
# Fri, 11 Nov 2022 11:00:51 GMT
LABEL org.opencontainers.image.vendor=traefik org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.34 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:90cda3b7c32511829cd5ae9074240c36c34507085acb6e55b96f993740d2be93`  
		Last Modified: Tue, 09 Aug 2022 17:41:06 GMT  
		Size: 2.7 MB (2722153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bef289adf2cbb3f8d157193bbfd586faaa288d6dd23845f0db17b7c041df2ef`  
		Last Modified: Fri, 11 Nov 2022 11:01:45 GMT  
		Size: 663.1 KB (663148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4d7297d487dbad0e6a3001add15c558d8305d106c11a0f1d1572e3b8cb8c221`  
		Last Modified: Fri, 11 Nov 2022 11:01:47 GMT  
		Size: 20.1 MB (20131380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:238986be5500952726a82d7ee40ae56ba3acfe2c8512f680e8c1e764ba05184b`  
		Last Modified: Fri, 11 Nov 2022 11:01:44 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v1.7.34-windowsservercore-1809`

```console
$ docker pull traefik@sha256:ba22fa49d06eb335a538647f8ac6b53100619cef2d6dac06269da6c557709513
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3650; amd64

### `traefik:v1.7.34-windowsservercore-1809` - windows version 10.0.17763.3650; amd64

```console
$ docker pull traefik@sha256:8c0df9f3b6b67923ad88bb8c325e64f06bfec58ede2be72f6161a12fb58b0514
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 GB (2801442412 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5ffbcd25321baf9b5e717f95aad8a5c850725ea21067094e561b04f95f5e73c5`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Sat, 05 Nov 2022 18:29:26 GMT
RUN Install update 10.0.17763.3650
# Tue, 08 Nov 2022 18:31:26 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Nov 2022 19:39:46 GMT
RUN Invoke-WebRequest     -Uri "https://github.com/traefik/traefik/releases/download/v1.7.34/traefik_windows-amd64.exe"     -OutFile "/traefik.exe"
# Wed, 09 Nov 2022 19:39:47 GMT
EXPOSE 80
# Wed, 09 Nov 2022 19:39:48 GMT
ENTRYPOINT ["/traefik"]
# Wed, 09 Nov 2022 19:39:50 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.34 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:a48a3e4ae2de839d8e99bde16eb91d113fb2cf889bba472d0c4274851b5fb402`  
		Last Modified: Tue, 21 Jun 2022 18:30:17 GMT  
		Size: 1.9 GB (1924269350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c26cc6e4f9eb1ae415a5ead6f884cac597bbd57efa6cd042c878d5b54c9d2091`  
		Last Modified: Tue, 08 Nov 2022 19:44:35 GMT  
		Size: 854.3 MB (854317461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f182832ad6ad5ea3d4b7320fd7bfea56fb9cf8413be904e52db6ed14c8d9e36f`  
		Last Modified: Tue, 08 Nov 2022 19:42:07 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:114e02070c38ac40033338b737577f7ed16181f6ce5ef3a282eb2a91b99c1967`  
		Last Modified: Wed, 09 Nov 2022 19:40:52 GMT  
		Size: 22.9 MB (22850203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:198ef1b6118e3b8dff31c6ada18f95988302cf4293219d1043eb9b810b79f9ec`  
		Last Modified: Wed, 09 Nov 2022 19:40:46 GMT  
		Size: 1.3 KB (1316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8499782a4e49b27eacd6a70cb60fb670341838fe2a3a9103ec45ff34bbe922c9`  
		Last Modified: Wed, 09 Nov 2022 19:40:46 GMT  
		Size: 1.3 KB (1331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aadd67eff429b70dc14789c1a0f220cf3c25607c2b6a8145d3756731eb5b771a`  
		Last Modified: Wed, 09 Nov 2022 19:40:46 GMT  
		Size: 1.3 KB (1311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v2.9`

```console
$ docker pull traefik@sha256:ac1480ce3203541705b01d6dce40ef4bf563cdb29d5b00db88cc396fa9fa9cd5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; s390x

### `traefik:v2.9` - linux; amd64

```console
$ docker pull traefik@sha256:6c37f2135af79e0c2e387653ff3ab9abf95eb393439f07cfcfa5e06fd4bb10bb
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.7 MB (38661782 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d3cd2c35d32c1bfe78d93c2fda68314b39de4f405ff4f82c86eebd3420d108b3`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Tue, 09 Aug 2022 17:20:00 GMT
ADD file:f77e3f51f020890d22997e6c2ca98968b75b8bc8c463341a2010ff0655d4c88f in / 
# Tue, 09 Aug 2022 17:20:01 GMT
CMD ["/bin/sh"]
# Fri, 07 Oct 2022 04:21:14 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 17 Nov 2022 20:23:09 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.9.5/traefik_v2.9.5_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 17 Nov 2022 20:23:09 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 17 Nov 2022 20:23:09 GMT
EXPOSE 80
# Thu, 17 Nov 2022 20:23:09 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 17 Nov 2022 20:23:09 GMT
CMD ["traefik"]
# Thu, 17 Nov 2022 20:23:09 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.9.5 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:9ed08b51c99c95fb89d4d3eb43cacb1df34c40a394366b2ae5f94758f917c6f5`  
		Last Modified: Thu, 17 Nov 2022 20:23:40 GMT  
		Size: 35.2 MB (35164531 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2984145d314f0df14678294313f70e7a9112a1ac304a1550d6f55b3f36f95cbc`  
		Last Modified: Thu, 17 Nov 2022 20:23:34 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v2.9` - linux; arm variant v6

```console
$ docker pull traefik@sha256:f5bf1b659f8d381c1a13a2860015c160389af6fdfa3ab42b9c463a80150a84c3
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.5 MB (36498990 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:593023589445e011e74b841e01b331d02f3f257483cdda1d0327fdebba48c7de`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 10 Nov 2022 20:49:36 GMT
ADD file:89cb25f97e17bed5c56311280efe5cfa78422d8ffbe36232195d13f94d67417e in / 
# Thu, 10 Nov 2022 20:49:36 GMT
CMD ["/bin/sh"]
# Fri, 11 Nov 2022 11:58:35 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 17 Nov 2022 20:52:12 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.9.5/traefik_v2.9.5_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 17 Nov 2022 20:52:13 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 17 Nov 2022 20:52:13 GMT
EXPOSE 80
# Thu, 17 Nov 2022 20:52:13 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 17 Nov 2022 20:52:13 GMT
CMD ["traefik"]
# Thu, 17 Nov 2022 20:52:13 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.9.5 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:293b708aa6fb80967f27727d5c9c53ac9ba9cac376bed2ad02c17a5cca317b35`  
		Last Modified: Tue, 09 Aug 2022 17:50:52 GMT  
		Size: 2.6 MB (2631127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d346396c5843930d5c9d8e05ce83d5cc4fb94e7d986b9a31ed533e815c10e155`  
		Last Modified: Fri, 11 Nov 2022 12:00:08 GMT  
		Size: 666.4 KB (666362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cff7ec90e94457bb22f14c6a7c1c13725a823452f45c5ae834ec1592b521a30`  
		Last Modified: Thu, 17 Nov 2022 20:53:26 GMT  
		Size: 33.2 MB (33201133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b21b9991922acb29e5eb83766973440d83c5dff502201a569be8a655fa638b9`  
		Last Modified: Thu, 17 Nov 2022 20:53:19 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v2.9` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:36d7a9bb99e7509b27965b03c101efad6c435a883bc611a8da3341256be0fa53
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.6 MB (35642829 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a1252ce6bfaaa6350d40597943ba410313c43428e825ce64692e54780b617792`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 10 Nov 2022 20:39:46 GMT
ADD file:4b51a9d40f20d2beb29d0759b161d2b9403493453beb509de4e86a5d98513f16 in / 
# Thu, 10 Nov 2022 20:39:46 GMT
CMD ["/bin/sh"]
# Fri, 11 Nov 2022 11:00:35 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 17 Nov 2022 20:49:08 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.9.5/traefik_v2.9.5_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 17 Nov 2022 20:49:08 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 17 Nov 2022 20:49:08 GMT
EXPOSE 80
# Thu, 17 Nov 2022 20:49:08 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 17 Nov 2022 20:49:09 GMT
CMD ["traefik"]
# Thu, 17 Nov 2022 20:49:09 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.9.5 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:47517142f6ba87eca6b7bdca1e0df160b74671c81e4b9605dad38c1862a43be3`  
		Last Modified: Tue, 09 Aug 2022 17:40:55 GMT  
		Size: 2.7 MB (2718439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:249449b90f641a1b63eb9b2d4acd49b56306ca96cff71672364a6b3f00c4987f`  
		Last Modified: Fri, 11 Nov 2022 11:01:22 GMT  
		Size: 663.1 KB (663136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9eea6fbc7fa23ee63e1d48d0be490a165c452521ef2b0e1f7c5251ed40770ffa`  
		Last Modified: Thu, 17 Nov 2022 20:49:38 GMT  
		Size: 32.3 MB (32260887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a8bd16405d4b4acebd8694e9d0fac0e77d431a96daede1c6e0c58e791a5c39c`  
		Last Modified: Thu, 17 Nov 2022 20:49:34 GMT  
		Size: 367.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v2.9` - linux; s390x

```console
$ docker pull traefik@sha256:7e232016b20669caff6aeba8a8fb4aef9dc2386758e3a424ad978361b4a5980d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.3 MB (37322696 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4efcef68f66f91fcd9e200d6a5a68c1711d046ae85312931e3e87808fdd91f0f`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Tue, 09 Aug 2022 17:41:54 GMT
ADD file:7489fa84133e97e4f40b13dd5159989b3594c9627d9147bfc4e33134944cc368 in / 
# Tue, 09 Aug 2022 17:41:54 GMT
CMD ["/bin/sh"]
# Fri, 07 Oct 2022 09:56:58 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 17 Nov 2022 20:43:36 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.9.5/traefik_v2.9.5_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 17 Nov 2022 20:43:38 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 17 Nov 2022 20:43:38 GMT
EXPOSE 80
# Thu, 17 Nov 2022 20:43:38 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 17 Nov 2022 20:43:38 GMT
CMD ["traefik"]
# Thu, 17 Nov 2022 20:43:38 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.9.5 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:591a603f1fa785b25e5bd31eace69b3ffb910f7586c6a8baae6d50920c4755a7`  
		Last Modified: Thu, 17 Nov 2022 20:44:04 GMT  
		Size: 34.0 MB (34038728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:905be1b9269736fe6b80197be453aac0394c6d7651d0a0e7762e2c91a42ea604`  
		Last Modified: Thu, 17 Nov 2022 20:43:59 GMT  
		Size: 369.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v2.9-windowsservercore-1809`

```console
$ docker pull traefik@sha256:5523cb7aa12ec3d990b65e609c2be0f4cb343cb4efb4fa8277744807552b759a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3650; amd64

### `traefik:v2.9-windowsservercore-1809` - windows version 10.0.17763.3650; amd64

```console
$ docker pull traefik@sha256:8ab499cb74de7d769293cd802f6cdc05ac5ffd6967979069c7a0abe022d83710
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 GB (2814280892 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:295756a7319650a07766dff97c4449914951d50d038b7e9dc956cd805c38ad7b`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Sat, 05 Nov 2022 18:29:26 GMT
RUN Install update 10.0.17763.3650
# Tue, 08 Nov 2022 18:31:26 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 17 Nov 2022 20:22:44 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/traefik/traefik/releases/download/v2.9.5/traefik_v2.9.5_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Thu, 17 Nov 2022 20:22:45 GMT
EXPOSE 80
# Thu, 17 Nov 2022 20:22:46 GMT
ENTRYPOINT ["/traefik"]
# Thu, 17 Nov 2022 20:22:47 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.9.5 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:a48a3e4ae2de839d8e99bde16eb91d113fb2cf889bba472d0c4274851b5fb402`  
		Last Modified: Tue, 21 Jun 2022 18:30:17 GMT  
		Size: 1.9 GB (1924269350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c26cc6e4f9eb1ae415a5ead6f884cac597bbd57efa6cd042c878d5b54c9d2091`  
		Last Modified: Tue, 08 Nov 2022 19:44:35 GMT  
		Size: 854.3 MB (854317461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f182832ad6ad5ea3d4b7320fd7bfea56fb9cf8413be904e52db6ed14c8d9e36f`  
		Last Modified: Tue, 08 Nov 2022 19:42:07 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:baaa6f55c06ab87b039a446d4c41afed1de673231c65262e7e453cd85f4911ac`  
		Last Modified: Thu, 17 Nov 2022 20:23:36 GMT  
		Size: 35.7 MB (35688341 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6880ebcecd161ca978b69ed9b0ad7576045802fd6e91f6d33c5fae68b77e3dc4`  
		Last Modified: Thu, 17 Nov 2022 20:23:27 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1af037205d33fcf851e821b2621162e4c95d77aa6736ca7ceff7f6816d52c776`  
		Last Modified: Thu, 17 Nov 2022 20:23:27 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:339867d3dc3e68861d0942f7f829addffa1f0416cb59f77c53730b2e1b9cb16f`  
		Last Modified: Thu, 17 Nov 2022 20:23:27 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v2.9.5`

```console
$ docker pull traefik@sha256:ac1480ce3203541705b01d6dce40ef4bf563cdb29d5b00db88cc396fa9fa9cd5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; s390x

### `traefik:v2.9.5` - linux; amd64

```console
$ docker pull traefik@sha256:6c37f2135af79e0c2e387653ff3ab9abf95eb393439f07cfcfa5e06fd4bb10bb
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.7 MB (38661782 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d3cd2c35d32c1bfe78d93c2fda68314b39de4f405ff4f82c86eebd3420d108b3`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Tue, 09 Aug 2022 17:20:00 GMT
ADD file:f77e3f51f020890d22997e6c2ca98968b75b8bc8c463341a2010ff0655d4c88f in / 
# Tue, 09 Aug 2022 17:20:01 GMT
CMD ["/bin/sh"]
# Fri, 07 Oct 2022 04:21:14 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 17 Nov 2022 20:23:09 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.9.5/traefik_v2.9.5_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 17 Nov 2022 20:23:09 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 17 Nov 2022 20:23:09 GMT
EXPOSE 80
# Thu, 17 Nov 2022 20:23:09 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 17 Nov 2022 20:23:09 GMT
CMD ["traefik"]
# Thu, 17 Nov 2022 20:23:09 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.9.5 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:9ed08b51c99c95fb89d4d3eb43cacb1df34c40a394366b2ae5f94758f917c6f5`  
		Last Modified: Thu, 17 Nov 2022 20:23:40 GMT  
		Size: 35.2 MB (35164531 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2984145d314f0df14678294313f70e7a9112a1ac304a1550d6f55b3f36f95cbc`  
		Last Modified: Thu, 17 Nov 2022 20:23:34 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v2.9.5` - linux; arm variant v6

```console
$ docker pull traefik@sha256:f5bf1b659f8d381c1a13a2860015c160389af6fdfa3ab42b9c463a80150a84c3
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.5 MB (36498990 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:593023589445e011e74b841e01b331d02f3f257483cdda1d0327fdebba48c7de`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 10 Nov 2022 20:49:36 GMT
ADD file:89cb25f97e17bed5c56311280efe5cfa78422d8ffbe36232195d13f94d67417e in / 
# Thu, 10 Nov 2022 20:49:36 GMT
CMD ["/bin/sh"]
# Fri, 11 Nov 2022 11:58:35 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 17 Nov 2022 20:52:12 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.9.5/traefik_v2.9.5_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 17 Nov 2022 20:52:13 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 17 Nov 2022 20:52:13 GMT
EXPOSE 80
# Thu, 17 Nov 2022 20:52:13 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 17 Nov 2022 20:52:13 GMT
CMD ["traefik"]
# Thu, 17 Nov 2022 20:52:13 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.9.5 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:293b708aa6fb80967f27727d5c9c53ac9ba9cac376bed2ad02c17a5cca317b35`  
		Last Modified: Tue, 09 Aug 2022 17:50:52 GMT  
		Size: 2.6 MB (2631127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d346396c5843930d5c9d8e05ce83d5cc4fb94e7d986b9a31ed533e815c10e155`  
		Last Modified: Fri, 11 Nov 2022 12:00:08 GMT  
		Size: 666.4 KB (666362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cff7ec90e94457bb22f14c6a7c1c13725a823452f45c5ae834ec1592b521a30`  
		Last Modified: Thu, 17 Nov 2022 20:53:26 GMT  
		Size: 33.2 MB (33201133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b21b9991922acb29e5eb83766973440d83c5dff502201a569be8a655fa638b9`  
		Last Modified: Thu, 17 Nov 2022 20:53:19 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v2.9.5` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:36d7a9bb99e7509b27965b03c101efad6c435a883bc611a8da3341256be0fa53
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.6 MB (35642829 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a1252ce6bfaaa6350d40597943ba410313c43428e825ce64692e54780b617792`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 10 Nov 2022 20:39:46 GMT
ADD file:4b51a9d40f20d2beb29d0759b161d2b9403493453beb509de4e86a5d98513f16 in / 
# Thu, 10 Nov 2022 20:39:46 GMT
CMD ["/bin/sh"]
# Fri, 11 Nov 2022 11:00:35 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 17 Nov 2022 20:49:08 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.9.5/traefik_v2.9.5_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 17 Nov 2022 20:49:08 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 17 Nov 2022 20:49:08 GMT
EXPOSE 80
# Thu, 17 Nov 2022 20:49:08 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 17 Nov 2022 20:49:09 GMT
CMD ["traefik"]
# Thu, 17 Nov 2022 20:49:09 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.9.5 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:47517142f6ba87eca6b7bdca1e0df160b74671c81e4b9605dad38c1862a43be3`  
		Last Modified: Tue, 09 Aug 2022 17:40:55 GMT  
		Size: 2.7 MB (2718439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:249449b90f641a1b63eb9b2d4acd49b56306ca96cff71672364a6b3f00c4987f`  
		Last Modified: Fri, 11 Nov 2022 11:01:22 GMT  
		Size: 663.1 KB (663136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9eea6fbc7fa23ee63e1d48d0be490a165c452521ef2b0e1f7c5251ed40770ffa`  
		Last Modified: Thu, 17 Nov 2022 20:49:38 GMT  
		Size: 32.3 MB (32260887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a8bd16405d4b4acebd8694e9d0fac0e77d431a96daede1c6e0c58e791a5c39c`  
		Last Modified: Thu, 17 Nov 2022 20:49:34 GMT  
		Size: 367.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v2.9.5` - linux; s390x

```console
$ docker pull traefik@sha256:7e232016b20669caff6aeba8a8fb4aef9dc2386758e3a424ad978361b4a5980d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.3 MB (37322696 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4efcef68f66f91fcd9e200d6a5a68c1711d046ae85312931e3e87808fdd91f0f`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Tue, 09 Aug 2022 17:41:54 GMT
ADD file:7489fa84133e97e4f40b13dd5159989b3594c9627d9147bfc4e33134944cc368 in / 
# Tue, 09 Aug 2022 17:41:54 GMT
CMD ["/bin/sh"]
# Fri, 07 Oct 2022 09:56:58 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 17 Nov 2022 20:43:36 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.9.5/traefik_v2.9.5_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 17 Nov 2022 20:43:38 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 17 Nov 2022 20:43:38 GMT
EXPOSE 80
# Thu, 17 Nov 2022 20:43:38 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 17 Nov 2022 20:43:38 GMT
CMD ["traefik"]
# Thu, 17 Nov 2022 20:43:38 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.9.5 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:591a603f1fa785b25e5bd31eace69b3ffb910f7586c6a8baae6d50920c4755a7`  
		Last Modified: Thu, 17 Nov 2022 20:44:04 GMT  
		Size: 34.0 MB (34038728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:905be1b9269736fe6b80197be453aac0394c6d7651d0a0e7762e2c91a42ea604`  
		Last Modified: Thu, 17 Nov 2022 20:43:59 GMT  
		Size: 369.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v2.9.5-windowsservercore-1809`

```console
$ docker pull traefik@sha256:5523cb7aa12ec3d990b65e609c2be0f4cb343cb4efb4fa8277744807552b759a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3650; amd64

### `traefik:v2.9.5-windowsservercore-1809` - windows version 10.0.17763.3650; amd64

```console
$ docker pull traefik@sha256:8ab499cb74de7d769293cd802f6cdc05ac5ffd6967979069c7a0abe022d83710
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 GB (2814280892 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:295756a7319650a07766dff97c4449914951d50d038b7e9dc956cd805c38ad7b`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Sat, 05 Nov 2022 18:29:26 GMT
RUN Install update 10.0.17763.3650
# Tue, 08 Nov 2022 18:31:26 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 17 Nov 2022 20:22:44 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/traefik/traefik/releases/download/v2.9.5/traefik_v2.9.5_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Thu, 17 Nov 2022 20:22:45 GMT
EXPOSE 80
# Thu, 17 Nov 2022 20:22:46 GMT
ENTRYPOINT ["/traefik"]
# Thu, 17 Nov 2022 20:22:47 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.9.5 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:a48a3e4ae2de839d8e99bde16eb91d113fb2cf889bba472d0c4274851b5fb402`  
		Last Modified: Tue, 21 Jun 2022 18:30:17 GMT  
		Size: 1.9 GB (1924269350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c26cc6e4f9eb1ae415a5ead6f884cac597bbd57efa6cd042c878d5b54c9d2091`  
		Last Modified: Tue, 08 Nov 2022 19:44:35 GMT  
		Size: 854.3 MB (854317461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f182832ad6ad5ea3d4b7320fd7bfea56fb9cf8413be904e52db6ed14c8d9e36f`  
		Last Modified: Tue, 08 Nov 2022 19:42:07 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:baaa6f55c06ab87b039a446d4c41afed1de673231c65262e7e453cd85f4911ac`  
		Last Modified: Thu, 17 Nov 2022 20:23:36 GMT  
		Size: 35.7 MB (35688341 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6880ebcecd161ca978b69ed9b0ad7576045802fd6e91f6d33c5fae68b77e3dc4`  
		Last Modified: Thu, 17 Nov 2022 20:23:27 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1af037205d33fcf851e821b2621162e4c95d77aa6736ca7ceff7f6816d52c776`  
		Last Modified: Thu, 17 Nov 2022 20:23:27 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:339867d3dc3e68861d0942f7f829addffa1f0416cb59f77c53730b2e1b9cb16f`  
		Last Modified: Thu, 17 Nov 2022 20:23:27 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v3.0`

```console
$ docker pull traefik@sha256:e27e08111cced4a2505f7e86c9987cdc88e841e00cc04d628c5d9e1dcd75577c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; s390x

### `traefik:v3.0` - linux; amd64

```console
$ docker pull traefik@sha256:224603be70dbfe0438286ab45c22b157b70234c8ac3afbcb15751d0e8b212f8e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.6 MB (40558414 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8b876a2fdfb1f94a358fb4c23f6e9bcd2855f5ce3fd6303f00d54b069d32580a`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Tue, 09 Aug 2022 17:20:00 GMT
ADD file:f77e3f51f020890d22997e6c2ca98968b75b8bc8c463341a2010ff0655d4c88f in / 
# Tue, 09 Aug 2022 17:20:01 GMT
CMD ["/bin/sh"]
# Fri, 07 Oct 2022 04:21:14 GMT
RUN apk --no-cache add ca-certificates tzdata
# Mon, 05 Dec 2022 21:36:42 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v3.0.0-beta1/traefik_v3.0.0-beta1_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Mon, 05 Dec 2022 21:36:42 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Mon, 05 Dec 2022 21:36:42 GMT
EXPOSE 80
# Mon, 05 Dec 2022 21:36:43 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 05 Dec 2022 21:36:43 GMT
CMD ["traefik"]
# Mon, 05 Dec 2022 21:36:43 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v3.0.0-beta1 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:4e4dc523606876763876f4a13f05642485a71df1b2d01800d1ad801fdef562d8`  
		Last Modified: Mon, 05 Dec 2022 21:37:19 GMT  
		Size: 37.1 MB (37061162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d669c768802639b8ed02105961df833c99d47466f0d3f568128b38f6564a6d5`  
		Last Modified: Mon, 05 Dec 2022 21:37:13 GMT  
		Size: 369.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v3.0` - linux; arm variant v6

```console
$ docker pull traefik@sha256:1a69ddf9abf4ec0a9b001b130e3362c704a6c9a6a9214a464142dd2a4e238b51
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.3 MB (38283031 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:02951a4586be09d87dc08106378ce66df26ac6b34bee71362d85a61212081c3e`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 10 Nov 2022 20:49:36 GMT
ADD file:89cb25f97e17bed5c56311280efe5cfa78422d8ffbe36232195d13f94d67417e in / 
# Thu, 10 Nov 2022 20:49:36 GMT
CMD ["/bin/sh"]
# Fri, 11 Nov 2022 11:58:35 GMT
RUN apk --no-cache add ca-certificates tzdata
# Mon, 05 Dec 2022 21:06:01 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v3.0.0-beta1/traefik_v3.0.0-beta1_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Mon, 05 Dec 2022 21:06:02 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Mon, 05 Dec 2022 21:06:02 GMT
EXPOSE 80
# Mon, 05 Dec 2022 21:06:02 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 05 Dec 2022 21:06:02 GMT
CMD ["traefik"]
# Mon, 05 Dec 2022 21:06:02 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v3.0.0-beta1 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:293b708aa6fb80967f27727d5c9c53ac9ba9cac376bed2ad02c17a5cca317b35`  
		Last Modified: Tue, 09 Aug 2022 17:50:52 GMT  
		Size: 2.6 MB (2631127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d346396c5843930d5c9d8e05ce83d5cc4fb94e7d986b9a31ed533e815c10e155`  
		Last Modified: Fri, 11 Nov 2022 12:00:08 GMT  
		Size: 666.4 KB (666362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2de3172f44924df50c9481f232e34ad82ccb08def5bacbf80082ae32ff1a9f59`  
		Last Modified: Mon, 05 Dec 2022 21:07:35 GMT  
		Size: 35.0 MB (34985173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92d3657bce77bb11dac6a174ca320a66f72b6817e719f16a78a3e8e2460d652c`  
		Last Modified: Mon, 05 Dec 2022 21:07:27 GMT  
		Size: 369.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v3.0` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:89cd35233bb361b5da3a3892ac97c01ed73494c437447893088040a470823c84
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.4 MB (37390044 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:abbe7b1ec0b0646f7c57c8ebafeb2ed6a35a981149e7b80bbe8a8e8418dfc06c`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 10 Nov 2022 20:39:46 GMT
ADD file:4b51a9d40f20d2beb29d0759b161d2b9403493453beb509de4e86a5d98513f16 in / 
# Thu, 10 Nov 2022 20:39:46 GMT
CMD ["/bin/sh"]
# Fri, 11 Nov 2022 11:00:35 GMT
RUN apk --no-cache add ca-certificates tzdata
# Mon, 05 Dec 2022 21:32:58 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v3.0.0-beta1/traefik_v3.0.0-beta1_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Mon, 05 Dec 2022 21:32:58 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Mon, 05 Dec 2022 21:32:58 GMT
EXPOSE 80
# Mon, 05 Dec 2022 21:32:58 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 05 Dec 2022 21:32:58 GMT
CMD ["traefik"]
# Mon, 05 Dec 2022 21:32:58 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v3.0.0-beta1 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:47517142f6ba87eca6b7bdca1e0df160b74671c81e4b9605dad38c1862a43be3`  
		Last Modified: Tue, 09 Aug 2022 17:40:55 GMT  
		Size: 2.7 MB (2718439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:249449b90f641a1b63eb9b2d4acd49b56306ca96cff71672364a6b3f00c4987f`  
		Last Modified: Fri, 11 Nov 2022 11:01:22 GMT  
		Size: 663.1 KB (663136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5eb4eafd343ee373719a84e6dafb493a427f2c0c5011760065e33981fadac29e`  
		Last Modified: Mon, 05 Dec 2022 21:33:34 GMT  
		Size: 34.0 MB (34008101 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84347e8cbd45c0add87bc3449d8dab6a64e1f748a86f2266df30510267cf352b`  
		Last Modified: Mon, 05 Dec 2022 21:33:30 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v3.0` - linux; s390x

```console
$ docker pull traefik@sha256:4335bf033a523decf7404c56d5b1f5066cdf0cadd7d88b11773a4e4fe786f46c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.1 MB (39122041 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:679c37472e0f51cd5077eb893416f86bbd67f0f657e44f9a3db5c0753d295600`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Tue, 09 Aug 2022 17:41:54 GMT
ADD file:7489fa84133e97e4f40b13dd5159989b3594c9627d9147bfc4e33134944cc368 in / 
# Tue, 09 Aug 2022 17:41:54 GMT
CMD ["/bin/sh"]
# Fri, 07 Oct 2022 09:56:58 GMT
RUN apk --no-cache add ca-certificates tzdata
# Mon, 05 Dec 2022 20:58:11 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v3.0.0-beta1/traefik_v3.0.0-beta1_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Mon, 05 Dec 2022 20:58:12 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Mon, 05 Dec 2022 20:58:13 GMT
EXPOSE 80
# Mon, 05 Dec 2022 20:58:13 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 05 Dec 2022 20:58:13 GMT
CMD ["traefik"]
# Mon, 05 Dec 2022 20:58:13 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v3.0.0-beta1 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:3201ac53116b6203e861c6fb526eed5481c79f118b246a8a4c674f3e864fc4de`  
		Last Modified: Mon, 05 Dec 2022 20:58:56 GMT  
		Size: 35.8 MB (35838073 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b56600e5855f954be9975df988daaf3149e939469976015c165aad1cd531c9ca`  
		Last Modified: Mon, 05 Dec 2022 20:58:51 GMT  
		Size: 369.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v3.0-windowsservercore-1809`

```console
$ docker pull traefik@sha256:5eeae50f78f79dd84fee1bb77fe7fe7384a13dbd32ebaa5c80bc9b15d83d1d30
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3650; amd64

### `traefik:v3.0-windowsservercore-1809` - windows version 10.0.17763.3650; amd64

```console
$ docker pull traefik@sha256:1caf484b3364fc839149585ff9e9df0e2f9b82a4d63d4298d0e1340ed97d82bb
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 GB (2816185547 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7adffb6e0e4ab0c0696bc04fd7838772060eef2bdc50aeb814ef49773e334801`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Sat, 05 Nov 2022 18:29:26 GMT
RUN Install update 10.0.17763.3650
# Tue, 08 Nov 2022 18:31:26 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Mon, 05 Dec 2022 21:19:02 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/traefik/traefik/releases/download/v3.0.0-beta1/traefik_v3.0.0-beta1_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Mon, 05 Dec 2022 21:19:03 GMT
EXPOSE 80
# Mon, 05 Dec 2022 21:19:04 GMT
ENTRYPOINT ["/traefik"]
# Mon, 05 Dec 2022 21:19:05 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v3.0.0-beta1 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:a48a3e4ae2de839d8e99bde16eb91d113fb2cf889bba472d0c4274851b5fb402`  
		Last Modified: Tue, 21 Jun 2022 18:30:17 GMT  
		Size: 1.9 GB (1924269350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c26cc6e4f9eb1ae415a5ead6f884cac597bbd57efa6cd042c878d5b54c9d2091`  
		Last Modified: Tue, 08 Nov 2022 19:44:35 GMT  
		Size: 854.3 MB (854317461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f182832ad6ad5ea3d4b7320fd7bfea56fb9cf8413be904e52db6ed14c8d9e36f`  
		Last Modified: Tue, 08 Nov 2022 19:42:07 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bf10c072ea1decad27162e33014b87a4a0d893a08f6259c83615886f7689580`  
		Last Modified: Mon, 05 Dec 2022 21:20:11 GMT  
		Size: 37.6 MB (37593045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b816ab54a1f9bf5eb43e0aea31c4b44fdec25fa6db44d02f58eb46cf021eb730`  
		Last Modified: Mon, 05 Dec 2022 21:19:57 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff05f49a360e835df322dccf350bd6ff8d907a67ce3ff32dad883a3e9ac66d61`  
		Last Modified: Mon, 05 Dec 2022 21:19:56 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9019e3961bc041a48bf292b9992be18498cc417cd524c779548b66686b7586c1`  
		Last Modified: Mon, 05 Dec 2022 21:19:57 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v3.0.0-beta1`

```console
$ docker pull traefik@sha256:e27e08111cced4a2505f7e86c9987cdc88e841e00cc04d628c5d9e1dcd75577c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; s390x

### `traefik:v3.0.0-beta1` - linux; amd64

```console
$ docker pull traefik@sha256:224603be70dbfe0438286ab45c22b157b70234c8ac3afbcb15751d0e8b212f8e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.6 MB (40558414 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8b876a2fdfb1f94a358fb4c23f6e9bcd2855f5ce3fd6303f00d54b069d32580a`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Tue, 09 Aug 2022 17:20:00 GMT
ADD file:f77e3f51f020890d22997e6c2ca98968b75b8bc8c463341a2010ff0655d4c88f in / 
# Tue, 09 Aug 2022 17:20:01 GMT
CMD ["/bin/sh"]
# Fri, 07 Oct 2022 04:21:14 GMT
RUN apk --no-cache add ca-certificates tzdata
# Mon, 05 Dec 2022 21:36:42 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v3.0.0-beta1/traefik_v3.0.0-beta1_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Mon, 05 Dec 2022 21:36:42 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Mon, 05 Dec 2022 21:36:42 GMT
EXPOSE 80
# Mon, 05 Dec 2022 21:36:43 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 05 Dec 2022 21:36:43 GMT
CMD ["traefik"]
# Mon, 05 Dec 2022 21:36:43 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v3.0.0-beta1 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:4e4dc523606876763876f4a13f05642485a71df1b2d01800d1ad801fdef562d8`  
		Last Modified: Mon, 05 Dec 2022 21:37:19 GMT  
		Size: 37.1 MB (37061162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d669c768802639b8ed02105961df833c99d47466f0d3f568128b38f6564a6d5`  
		Last Modified: Mon, 05 Dec 2022 21:37:13 GMT  
		Size: 369.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v3.0.0-beta1` - linux; arm variant v6

```console
$ docker pull traefik@sha256:1a69ddf9abf4ec0a9b001b130e3362c704a6c9a6a9214a464142dd2a4e238b51
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.3 MB (38283031 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:02951a4586be09d87dc08106378ce66df26ac6b34bee71362d85a61212081c3e`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 10 Nov 2022 20:49:36 GMT
ADD file:89cb25f97e17bed5c56311280efe5cfa78422d8ffbe36232195d13f94d67417e in / 
# Thu, 10 Nov 2022 20:49:36 GMT
CMD ["/bin/sh"]
# Fri, 11 Nov 2022 11:58:35 GMT
RUN apk --no-cache add ca-certificates tzdata
# Mon, 05 Dec 2022 21:06:01 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v3.0.0-beta1/traefik_v3.0.0-beta1_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Mon, 05 Dec 2022 21:06:02 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Mon, 05 Dec 2022 21:06:02 GMT
EXPOSE 80
# Mon, 05 Dec 2022 21:06:02 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 05 Dec 2022 21:06:02 GMT
CMD ["traefik"]
# Mon, 05 Dec 2022 21:06:02 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v3.0.0-beta1 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:293b708aa6fb80967f27727d5c9c53ac9ba9cac376bed2ad02c17a5cca317b35`  
		Last Modified: Tue, 09 Aug 2022 17:50:52 GMT  
		Size: 2.6 MB (2631127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d346396c5843930d5c9d8e05ce83d5cc4fb94e7d986b9a31ed533e815c10e155`  
		Last Modified: Fri, 11 Nov 2022 12:00:08 GMT  
		Size: 666.4 KB (666362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2de3172f44924df50c9481f232e34ad82ccb08def5bacbf80082ae32ff1a9f59`  
		Last Modified: Mon, 05 Dec 2022 21:07:35 GMT  
		Size: 35.0 MB (34985173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92d3657bce77bb11dac6a174ca320a66f72b6817e719f16a78a3e8e2460d652c`  
		Last Modified: Mon, 05 Dec 2022 21:07:27 GMT  
		Size: 369.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v3.0.0-beta1` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:89cd35233bb361b5da3a3892ac97c01ed73494c437447893088040a470823c84
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.4 MB (37390044 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:abbe7b1ec0b0646f7c57c8ebafeb2ed6a35a981149e7b80bbe8a8e8418dfc06c`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 10 Nov 2022 20:39:46 GMT
ADD file:4b51a9d40f20d2beb29d0759b161d2b9403493453beb509de4e86a5d98513f16 in / 
# Thu, 10 Nov 2022 20:39:46 GMT
CMD ["/bin/sh"]
# Fri, 11 Nov 2022 11:00:35 GMT
RUN apk --no-cache add ca-certificates tzdata
# Mon, 05 Dec 2022 21:32:58 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v3.0.0-beta1/traefik_v3.0.0-beta1_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Mon, 05 Dec 2022 21:32:58 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Mon, 05 Dec 2022 21:32:58 GMT
EXPOSE 80
# Mon, 05 Dec 2022 21:32:58 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 05 Dec 2022 21:32:58 GMT
CMD ["traefik"]
# Mon, 05 Dec 2022 21:32:58 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v3.0.0-beta1 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:47517142f6ba87eca6b7bdca1e0df160b74671c81e4b9605dad38c1862a43be3`  
		Last Modified: Tue, 09 Aug 2022 17:40:55 GMT  
		Size: 2.7 MB (2718439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:249449b90f641a1b63eb9b2d4acd49b56306ca96cff71672364a6b3f00c4987f`  
		Last Modified: Fri, 11 Nov 2022 11:01:22 GMT  
		Size: 663.1 KB (663136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5eb4eafd343ee373719a84e6dafb493a427f2c0c5011760065e33981fadac29e`  
		Last Modified: Mon, 05 Dec 2022 21:33:34 GMT  
		Size: 34.0 MB (34008101 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84347e8cbd45c0add87bc3449d8dab6a64e1f748a86f2266df30510267cf352b`  
		Last Modified: Mon, 05 Dec 2022 21:33:30 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v3.0.0-beta1` - linux; s390x

```console
$ docker pull traefik@sha256:4335bf033a523decf7404c56d5b1f5066cdf0cadd7d88b11773a4e4fe786f46c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.1 MB (39122041 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:679c37472e0f51cd5077eb893416f86bbd67f0f657e44f9a3db5c0753d295600`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Tue, 09 Aug 2022 17:41:54 GMT
ADD file:7489fa84133e97e4f40b13dd5159989b3594c9627d9147bfc4e33134944cc368 in / 
# Tue, 09 Aug 2022 17:41:54 GMT
CMD ["/bin/sh"]
# Fri, 07 Oct 2022 09:56:58 GMT
RUN apk --no-cache add ca-certificates tzdata
# Mon, 05 Dec 2022 20:58:11 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v3.0.0-beta1/traefik_v3.0.0-beta1_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Mon, 05 Dec 2022 20:58:12 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Mon, 05 Dec 2022 20:58:13 GMT
EXPOSE 80
# Mon, 05 Dec 2022 20:58:13 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 05 Dec 2022 20:58:13 GMT
CMD ["traefik"]
# Mon, 05 Dec 2022 20:58:13 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v3.0.0-beta1 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:3201ac53116b6203e861c6fb526eed5481c79f118b246a8a4c674f3e864fc4de`  
		Last Modified: Mon, 05 Dec 2022 20:58:56 GMT  
		Size: 35.8 MB (35838073 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b56600e5855f954be9975df988daaf3149e939469976015c165aad1cd531c9ca`  
		Last Modified: Mon, 05 Dec 2022 20:58:51 GMT  
		Size: 369.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v3.0.0-beta1-windowsservercore-1809`

```console
$ docker pull traefik@sha256:5eeae50f78f79dd84fee1bb77fe7fe7384a13dbd32ebaa5c80bc9b15d83d1d30
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3650; amd64

### `traefik:v3.0.0-beta1-windowsservercore-1809` - windows version 10.0.17763.3650; amd64

```console
$ docker pull traefik@sha256:1caf484b3364fc839149585ff9e9df0e2f9b82a4d63d4298d0e1340ed97d82bb
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 GB (2816185547 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7adffb6e0e4ab0c0696bc04fd7838772060eef2bdc50aeb814ef49773e334801`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Sat, 05 Nov 2022 18:29:26 GMT
RUN Install update 10.0.17763.3650
# Tue, 08 Nov 2022 18:31:26 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Mon, 05 Dec 2022 21:19:02 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/traefik/traefik/releases/download/v3.0.0-beta1/traefik_v3.0.0-beta1_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Mon, 05 Dec 2022 21:19:03 GMT
EXPOSE 80
# Mon, 05 Dec 2022 21:19:04 GMT
ENTRYPOINT ["/traefik"]
# Mon, 05 Dec 2022 21:19:05 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v3.0.0-beta1 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:a48a3e4ae2de839d8e99bde16eb91d113fb2cf889bba472d0c4274851b5fb402`  
		Last Modified: Tue, 21 Jun 2022 18:30:17 GMT  
		Size: 1.9 GB (1924269350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c26cc6e4f9eb1ae415a5ead6f884cac597bbd57efa6cd042c878d5b54c9d2091`  
		Last Modified: Tue, 08 Nov 2022 19:44:35 GMT  
		Size: 854.3 MB (854317461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f182832ad6ad5ea3d4b7320fd7bfea56fb9cf8413be904e52db6ed14c8d9e36f`  
		Last Modified: Tue, 08 Nov 2022 19:42:07 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bf10c072ea1decad27162e33014b87a4a0d893a08f6259c83615886f7689580`  
		Last Modified: Mon, 05 Dec 2022 21:20:11 GMT  
		Size: 37.6 MB (37593045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b816ab54a1f9bf5eb43e0aea31c4b44fdec25fa6db44d02f58eb46cf021eb730`  
		Last Modified: Mon, 05 Dec 2022 21:19:57 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff05f49a360e835df322dccf350bd6ff8d907a67ce3ff32dad883a3e9ac66d61`  
		Last Modified: Mon, 05 Dec 2022 21:19:56 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9019e3961bc041a48bf292b9992be18498cc417cd524c779548b66686b7586c1`  
		Last Modified: Mon, 05 Dec 2022 21:19:57 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:windowsservercore-1809`

```console
$ docker pull traefik@sha256:5523cb7aa12ec3d990b65e609c2be0f4cb343cb4efb4fa8277744807552b759a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3650; amd64

### `traefik:windowsservercore-1809` - windows version 10.0.17763.3650; amd64

```console
$ docker pull traefik@sha256:8ab499cb74de7d769293cd802f6cdc05ac5ffd6967979069c7a0abe022d83710
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 GB (2814280892 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:295756a7319650a07766dff97c4449914951d50d038b7e9dc956cd805c38ad7b`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Sat, 05 Nov 2022 18:29:26 GMT
RUN Install update 10.0.17763.3650
# Tue, 08 Nov 2022 18:31:26 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 17 Nov 2022 20:22:44 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/traefik/traefik/releases/download/v2.9.5/traefik_v2.9.5_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Thu, 17 Nov 2022 20:22:45 GMT
EXPOSE 80
# Thu, 17 Nov 2022 20:22:46 GMT
ENTRYPOINT ["/traefik"]
# Thu, 17 Nov 2022 20:22:47 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.9.5 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:a48a3e4ae2de839d8e99bde16eb91d113fb2cf889bba472d0c4274851b5fb402`  
		Last Modified: Tue, 21 Jun 2022 18:30:17 GMT  
		Size: 1.9 GB (1924269350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c26cc6e4f9eb1ae415a5ead6f884cac597bbd57efa6cd042c878d5b54c9d2091`  
		Last Modified: Tue, 08 Nov 2022 19:44:35 GMT  
		Size: 854.3 MB (854317461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f182832ad6ad5ea3d4b7320fd7bfea56fb9cf8413be904e52db6ed14c8d9e36f`  
		Last Modified: Tue, 08 Nov 2022 19:42:07 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:baaa6f55c06ab87b039a446d4c41afed1de673231c65262e7e453cd85f4911ac`  
		Last Modified: Thu, 17 Nov 2022 20:23:36 GMT  
		Size: 35.7 MB (35688341 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6880ebcecd161ca978b69ed9b0ad7576045802fd6e91f6d33c5fae68b77e3dc4`  
		Last Modified: Thu, 17 Nov 2022 20:23:27 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1af037205d33fcf851e821b2621162e4c95d77aa6736ca7ceff7f6816d52c776`  
		Last Modified: Thu, 17 Nov 2022 20:23:27 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:339867d3dc3e68861d0942f7f829addffa1f0416cb59f77c53730b2e1b9cb16f`  
		Last Modified: Thu, 17 Nov 2022 20:23:27 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
