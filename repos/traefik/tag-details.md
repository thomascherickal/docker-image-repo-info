<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `traefik`

-	[`traefik:1.7`](#traefik17)
-	[`traefik:1.7-alpine`](#traefik17-alpine)
-	[`traefik:1.7-windowsservercore-1809`](#traefik17-windowsservercore-1809)
-	[`traefik:1.7.28`](#traefik1728)
-	[`traefik:1.7.28-alpine`](#traefik1728-alpine)
-	[`traefik:1.7.28-windowsservercore-1809`](#traefik1728-windowsservercore-1809)
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
-	[`traefik:v1.7.28`](#traefikv1728)
-	[`traefik:v1.7.28-alpine`](#traefikv1728-alpine)
-	[`traefik:v1.7.28-windowsservercore-1809`](#traefikv1728-windowsservercore-1809)
-	[`traefik:v2.4`](#traefikv24)
-	[`traefik:v2.4-windowsservercore-1809`](#traefikv24-windowsservercore-1809)
-	[`traefik:v2.4.8`](#traefikv248)
-	[`traefik:v2.4.8-windowsservercore-1809`](#traefikv248-windowsservercore-1809)
-	[`traefik:windowsservercore-1809`](#traefikwindowsservercore-1809)

## `traefik:1.7`

```console
$ docker pull traefik@sha256:77db9c383b8294a959674d42306499048046046e144b6a7e7dfd0dc516e80571
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:1.7` - linux; amd64

```console
$ docker pull traefik@sha256:af9ee4f13d77fdc35fd8c2d571b042001080754a5e69efca671bf3b382e29163
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **21.6 MB (21555693 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:11f7f6e41b0f0ee2d4e8ce90d77a2cf0615f0cfcd2b9e8d5cade2e564745d8f5`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Tue, 09 Mar 2021 01:32:48 GMT
COPY file:cd6264d9a7514a8fbc3eb7b400566d36178794d2b757959812cc3abc6f13a97b in /etc/ssl/certs/ 
# Tue, 09 Mar 2021 01:32:49 GMT
COPY dir:379603788862c2a6c57432d70b0a67f561fe00310e1b958c9ecf85381b1c9cd9 in /usr/share/ 
# Tue, 09 Mar 2021 01:32:49 GMT
COPY file:94b9997cc55c7732c9fc173c119f980e4a38eba20b96a90170a3d7fade75f0eb in / 
# Tue, 09 Mar 2021 01:32:50 GMT
EXPOSE 80
# Tue, 09 Mar 2021 01:32:50 GMT
VOLUME [/tmp]
# Tue, 09 Mar 2021 01:32:50 GMT
ENTRYPOINT ["/traefik"]
# Tue, 09 Mar 2021 01:32:50 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.28 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:7432563bc6a93a4a26e4fa5e0465d309dbfe1a4f5c13f945a90070f2acdcd897`  
		Last Modified: Tue, 09 Mar 2021 01:34:03 GMT  
		Size: 21.1 MB (21116000 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:1.7` - linux; arm variant v6

```console
$ docker pull traefik@sha256:5eea4ce43832fb4fe06e6a76f4be2ee702cd7406bca2eeb28e7b8886b857fb60
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **20.2 MB (20207939 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a16dc71c18edfa988002598f7753875525a253977c27360950d4277cb5a12afb`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Thu, 17 Dec 2020 00:26:47 GMT
COPY file:cd6264d9a7514a8fbc3eb7b400566d36178794d2b757959812cc3abc6f13a97b in /etc/ssl/certs/ 
# Wed, 24 Feb 2021 23:34:19 GMT
COPY dir:379603788862c2a6c57432d70b0a67f561fe00310e1b958c9ecf85381b1c9cd9 in /usr/share/ 
# Wed, 24 Feb 2021 23:34:26 GMT
COPY file:3d9c1552db5b4c73ac7fe21268eeb20506f000d2e59d7be76697f45a50d32c64 in / 
# Wed, 24 Feb 2021 23:34:29 GMT
EXPOSE 80
# Wed, 24 Feb 2021 23:34:30 GMT
VOLUME [/tmp]
# Wed, 24 Feb 2021 23:34:31 GMT
ENTRYPOINT ["/traefik"]
# Wed, 24 Feb 2021 23:34:33 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.28 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:1eb5b49b6d2a16c38104badd82447927b16f7ba253b84d47c329449b778bb19d`  
		Last Modified: Wed, 24 Feb 2021 23:36:21 GMT  
		Size: 19.8 MB (19768211 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:1.7` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:ea16e7c67604fa93b41900462522a8a595106d85a2320d07d84d7a39f9dd1ef0
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **19.9 MB (19925754 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:03d91b88a063e66b3027cc082d06fa36b001cc4ddc8d7cb3aad1e284f2a30f49`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Thu, 17 Dec 2020 00:27:56 GMT
COPY file:cd6264d9a7514a8fbc3eb7b400566d36178794d2b757959812cc3abc6f13a97b in /etc/ssl/certs/ 
# Thu, 25 Feb 2021 04:23:55 GMT
COPY dir:379603788862c2a6c57432d70b0a67f561fe00310e1b958c9ecf85381b1c9cd9 in /usr/share/ 
# Thu, 25 Feb 2021 04:23:57 GMT
COPY file:6bab4a8fc3d272fc29bc5ff42634cb12785fea9e23b0cf50f077702217bb6c03 in / 
# Thu, 25 Feb 2021 04:23:58 GMT
EXPOSE 80
# Thu, 25 Feb 2021 04:23:58 GMT
VOLUME [/tmp]
# Thu, 25 Feb 2021 04:23:59 GMT
ENTRYPOINT ["/traefik"]
# Thu, 25 Feb 2021 04:24:00 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.28 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:9fa98c5ef5e644f69a6a2346c2be14df34ac2e02195fcb75676fc1fe178f81b6`  
		Last Modified: Thu, 25 Feb 2021 04:25:21 GMT  
		Size: 19.5 MB (19486050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:1.7-alpine`

```console
$ docker pull traefik@sha256:6f6ed7c4780aca850dd2d8a88e483c91a3e7e061bb28b912e72dd21056c45b27
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:1.7-alpine` - linux; amd64

```console
$ docker pull traefik@sha256:11eab5d88ab546b5ffa5a5554809cd7f7f110c77976245d17f7192d8ebd27cd1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **24.6 MB (24606157 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c4ca93cce099f0cf7572f844fb03f2691539392bf54558b5c1a08a8616b63107`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 25 Mar 2021 22:19:43 GMT
ADD file:05adf37fc1a41a31d8e0e0b9371a01161abc0d348adacbc81689a1a34e8fe12d in / 
# Thu, 25 Mar 2021 22:19:43 GMT
CMD ["/bin/sh"]
# Fri, 26 Mar 2021 09:42:59 GMT
RUN apk --no-cache add ca-certificates tzdata
# Fri, 26 Mar 2021 09:43:11 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/traefik/traefik/releases/download/v1.7.28/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Fri, 26 Mar 2021 09:43:11 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Fri, 26 Mar 2021 09:43:12 GMT
EXPOSE 80
# Fri, 26 Mar 2021 09:43:12 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 26 Mar 2021 09:43:12 GMT
CMD ["traefik"]
# Fri, 26 Mar 2021 09:43:12 GMT
LABEL org.opencontainers.image.vendor=traefik org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.28 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:839b45e0263abc8ab2dc0bfabc91a19947e932ffbd551a93970ea3ee971eadf6`  
		Last Modified: Thu, 25 Mar 2021 22:20:47 GMT  
		Size: 2.8 MB (2815332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f381c65aaaa0ed2d90609a1d94ca65fa057410a866389f0a380395c0f30dad9`  
		Last Modified: Fri, 26 Mar 2021 09:43:39 GMT  
		Size: 674.2 KB (674197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:201bd2f8d389731241ad12464a3c0e8dcf27fe7e8c5f26413ad17ec311573347`  
		Last Modified: Fri, 26 Mar 2021 09:44:08 GMT  
		Size: 21.1 MB (21116259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80eb8a05c6f082aedf128e275ce47294e63622bb8c19c53affb9bc9d6a3ac590`  
		Last Modified: Fri, 26 Mar 2021 09:44:04 GMT  
		Size: 369.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:1.7-alpine` - linux; arm variant v6

```console
$ docker pull traefik@sha256:31f0451328ced172b21c6254efec3ad8b0b93e74eed52d0121815324d02e21be
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.1 MB (23066960 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3981997446a1cad72ae513fb79a7443ffe0bc5b3c55413d0f9053f1021be6a09`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 25 Mar 2021 22:51:39 GMT
ADD file:f9e7465b7bf9cb6b234d24519c80b22b9da7894ea0337e0ac44920114773c8a9 in / 
# Thu, 25 Mar 2021 22:51:48 GMT
CMD ["/bin/sh"]
# Fri, 26 Mar 2021 10:23:59 GMT
RUN apk --no-cache add ca-certificates tzdata
# Fri, 26 Mar 2021 10:24:28 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/traefik/traefik/releases/download/v1.7.28/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Fri, 26 Mar 2021 10:24:29 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Fri, 26 Mar 2021 10:24:30 GMT
EXPOSE 80
# Fri, 26 Mar 2021 10:24:31 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 26 Mar 2021 10:24:33 GMT
CMD ["traefik"]
# Fri, 26 Mar 2021 10:24:34 GMT
LABEL org.opencontainers.image.vendor=traefik org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.28 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:275240b4b3a35cb935b35bfb1a8700e2b9ca100cd6e33ca8a6f83d056016bd61`  
		Last Modified: Thu, 25 Mar 2021 22:55:29 GMT  
		Size: 2.6 MB (2621328 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb7337eab7080efd44e620f96e74185d0ffeacba100c69045459249b2d3a3dd3`  
		Last Modified: Fri, 26 Mar 2021 10:25:07 GMT  
		Size: 677.0 KB (677007 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5393b92d65d5d154de06bb7fc8c8db2941f5f9c0536df8b348e963b63f7950f7`  
		Last Modified: Fri, 26 Mar 2021 10:25:33 GMT  
		Size: 19.8 MB (19768257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79773a7a5681d8dae4c1295c9a3354d8e59fd7e97153321d294f44c97f25ef83`  
		Last Modified: Fri, 26 Mar 2021 10:25:26 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:1.7-alpine` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:52e34452769038558151c3dbd0871763a9f5110ec680bbf7ad1bc4394c75de0f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **22.9 MB (22887814 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b10fb481f0a98ede8ac59c98224a31223ef8a8987c4490786685e024b3155d82`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 25 Mar 2021 22:41:33 GMT
ADD file:6fca680ab44d711c282deb126e7ad2f7ab51d84a6364192a4913e178f7d393a0 in / 
# Thu, 25 Mar 2021 22:41:38 GMT
CMD ["/bin/sh"]
# Fri, 26 Mar 2021 08:08:01 GMT
RUN apk --no-cache add ca-certificates tzdata
# Fri, 26 Mar 2021 08:08:24 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/traefik/traefik/releases/download/v1.7.28/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Fri, 26 Mar 2021 08:08:25 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Fri, 26 Mar 2021 08:08:26 GMT
EXPOSE 80
# Fri, 26 Mar 2021 08:08:27 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 26 Mar 2021 08:08:28 GMT
CMD ["traefik"]
# Fri, 26 Mar 2021 08:08:29 GMT
LABEL org.opencontainers.image.vendor=traefik org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.28 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:47185b9379cb432a7a6711ec279fdcb33fe0426be145e1bf61879568c9b54054`  
		Last Modified: Thu, 25 Mar 2021 22:45:46 GMT  
		Size: 2.7 MB (2725878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b107397c029a94008575072c0901eae0ac7977a9fe1fa05ed8e45757387f3be`  
		Last Modified: Fri, 26 Mar 2021 08:11:41 GMT  
		Size: 675.5 KB (675534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ec8eb5a4ab439b7e6632255add989c9df999239aff3b7c29caf94804b1c1e27`  
		Last Modified: Fri, 26 Mar 2021 08:12:05 GMT  
		Size: 19.5 MB (19486034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fba170bddfe05b0a040b3b25f421d499e4baf856e607552b0b9c90e49095415`  
		Last Modified: Fri, 26 Mar 2021 08:12:00 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:1.7-windowsservercore-1809`

```console
$ docker pull traefik@sha256:1a72007aed918f7be894ed6e10cd3f55a29a146785eacece8553c04640f3d809
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1817; amd64

### `traefik:1.7-windowsservercore-1809` - windows version 10.0.17763.1817; amd64

```console
$ docker pull traefik@sha256:76c78ecdfc533e552dc56a5469bc408dc38029acdc4d25347baf57dd14e0af6e
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2492116033 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4e6360dd33aca46bebf924fba8e817df599a404f2440fd9d311519d11c2a4f75`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 27 Feb 2021 09:32:06 GMT
RUN Install update 1809-amd64
# Wed, 10 Mar 2021 13:08:20 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Mar 2021 22:45:52 GMT
RUN Invoke-WebRequest     -Uri "https://github.com/traefik/traefik/releases/download/v1.7.28/traefik_windows-amd64.exe"     -OutFile "/traefik.exe"
# Wed, 10 Mar 2021 22:45:53 GMT
EXPOSE 80
# Wed, 10 Mar 2021 22:45:55 GMT
ENTRYPOINT ["/traefik"]
# Wed, 10 Mar 2021 22:45:56 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.28 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5ff1512f88ecd4ff0a91ade34d43733c48834433e35f062f80e6e70d706f8d73`  
		Size: 743.2 MB (743201590 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ebe61daec6d671bc2c1c6fe61ac9825fb552e9cef3672d0a7dbec719d125ae64`  
		Last Modified: Wed, 10 Mar 2021 13:21:09 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c01ec7e8fcbdf93c7395f18256527489b510fe69665c091ffb6d71278bf9aafe`  
		Last Modified: Wed, 10 Mar 2021 22:47:40 GMT  
		Size: 30.6 MB (30575844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afd90db339e07111b4a805bd4b081d78ba3dfe7db4bf9f207e0ac638a901671d`  
		Last Modified: Wed, 10 Mar 2021 22:46:59 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89dffb25733d38bdbe1dedc4e3ef916319ab71fb03cc9be7168c119df4f8a37d`  
		Last Modified: Wed, 10 Mar 2021 22:46:59 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97445bcb41cca852497b41557ab320aac9a24c5ba6867f77aa005249fb6a0d78`  
		Last Modified: Wed, 10 Mar 2021 22:46:59 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:1.7.28`

```console
$ docker pull traefik@sha256:77db9c383b8294a959674d42306499048046046e144b6a7e7dfd0dc516e80571
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:1.7.28` - linux; amd64

```console
$ docker pull traefik@sha256:af9ee4f13d77fdc35fd8c2d571b042001080754a5e69efca671bf3b382e29163
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **21.6 MB (21555693 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:11f7f6e41b0f0ee2d4e8ce90d77a2cf0615f0cfcd2b9e8d5cade2e564745d8f5`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Tue, 09 Mar 2021 01:32:48 GMT
COPY file:cd6264d9a7514a8fbc3eb7b400566d36178794d2b757959812cc3abc6f13a97b in /etc/ssl/certs/ 
# Tue, 09 Mar 2021 01:32:49 GMT
COPY dir:379603788862c2a6c57432d70b0a67f561fe00310e1b958c9ecf85381b1c9cd9 in /usr/share/ 
# Tue, 09 Mar 2021 01:32:49 GMT
COPY file:94b9997cc55c7732c9fc173c119f980e4a38eba20b96a90170a3d7fade75f0eb in / 
# Tue, 09 Mar 2021 01:32:50 GMT
EXPOSE 80
# Tue, 09 Mar 2021 01:32:50 GMT
VOLUME [/tmp]
# Tue, 09 Mar 2021 01:32:50 GMT
ENTRYPOINT ["/traefik"]
# Tue, 09 Mar 2021 01:32:50 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.28 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:7432563bc6a93a4a26e4fa5e0465d309dbfe1a4f5c13f945a90070f2acdcd897`  
		Last Modified: Tue, 09 Mar 2021 01:34:03 GMT  
		Size: 21.1 MB (21116000 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:1.7.28` - linux; arm variant v6

```console
$ docker pull traefik@sha256:5eea4ce43832fb4fe06e6a76f4be2ee702cd7406bca2eeb28e7b8886b857fb60
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **20.2 MB (20207939 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a16dc71c18edfa988002598f7753875525a253977c27360950d4277cb5a12afb`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Thu, 17 Dec 2020 00:26:47 GMT
COPY file:cd6264d9a7514a8fbc3eb7b400566d36178794d2b757959812cc3abc6f13a97b in /etc/ssl/certs/ 
# Wed, 24 Feb 2021 23:34:19 GMT
COPY dir:379603788862c2a6c57432d70b0a67f561fe00310e1b958c9ecf85381b1c9cd9 in /usr/share/ 
# Wed, 24 Feb 2021 23:34:26 GMT
COPY file:3d9c1552db5b4c73ac7fe21268eeb20506f000d2e59d7be76697f45a50d32c64 in / 
# Wed, 24 Feb 2021 23:34:29 GMT
EXPOSE 80
# Wed, 24 Feb 2021 23:34:30 GMT
VOLUME [/tmp]
# Wed, 24 Feb 2021 23:34:31 GMT
ENTRYPOINT ["/traefik"]
# Wed, 24 Feb 2021 23:34:33 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.28 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:1eb5b49b6d2a16c38104badd82447927b16f7ba253b84d47c329449b778bb19d`  
		Last Modified: Wed, 24 Feb 2021 23:36:21 GMT  
		Size: 19.8 MB (19768211 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:1.7.28` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:ea16e7c67604fa93b41900462522a8a595106d85a2320d07d84d7a39f9dd1ef0
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **19.9 MB (19925754 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:03d91b88a063e66b3027cc082d06fa36b001cc4ddc8d7cb3aad1e284f2a30f49`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Thu, 17 Dec 2020 00:27:56 GMT
COPY file:cd6264d9a7514a8fbc3eb7b400566d36178794d2b757959812cc3abc6f13a97b in /etc/ssl/certs/ 
# Thu, 25 Feb 2021 04:23:55 GMT
COPY dir:379603788862c2a6c57432d70b0a67f561fe00310e1b958c9ecf85381b1c9cd9 in /usr/share/ 
# Thu, 25 Feb 2021 04:23:57 GMT
COPY file:6bab4a8fc3d272fc29bc5ff42634cb12785fea9e23b0cf50f077702217bb6c03 in / 
# Thu, 25 Feb 2021 04:23:58 GMT
EXPOSE 80
# Thu, 25 Feb 2021 04:23:58 GMT
VOLUME [/tmp]
# Thu, 25 Feb 2021 04:23:59 GMT
ENTRYPOINT ["/traefik"]
# Thu, 25 Feb 2021 04:24:00 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.28 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:9fa98c5ef5e644f69a6a2346c2be14df34ac2e02195fcb75676fc1fe178f81b6`  
		Last Modified: Thu, 25 Feb 2021 04:25:21 GMT  
		Size: 19.5 MB (19486050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:1.7.28-alpine`

```console
$ docker pull traefik@sha256:6f6ed7c4780aca850dd2d8a88e483c91a3e7e061bb28b912e72dd21056c45b27
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:1.7.28-alpine` - linux; amd64

```console
$ docker pull traefik@sha256:11eab5d88ab546b5ffa5a5554809cd7f7f110c77976245d17f7192d8ebd27cd1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **24.6 MB (24606157 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c4ca93cce099f0cf7572f844fb03f2691539392bf54558b5c1a08a8616b63107`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 25 Mar 2021 22:19:43 GMT
ADD file:05adf37fc1a41a31d8e0e0b9371a01161abc0d348adacbc81689a1a34e8fe12d in / 
# Thu, 25 Mar 2021 22:19:43 GMT
CMD ["/bin/sh"]
# Fri, 26 Mar 2021 09:42:59 GMT
RUN apk --no-cache add ca-certificates tzdata
# Fri, 26 Mar 2021 09:43:11 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/traefik/traefik/releases/download/v1.7.28/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Fri, 26 Mar 2021 09:43:11 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Fri, 26 Mar 2021 09:43:12 GMT
EXPOSE 80
# Fri, 26 Mar 2021 09:43:12 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 26 Mar 2021 09:43:12 GMT
CMD ["traefik"]
# Fri, 26 Mar 2021 09:43:12 GMT
LABEL org.opencontainers.image.vendor=traefik org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.28 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:839b45e0263abc8ab2dc0bfabc91a19947e932ffbd551a93970ea3ee971eadf6`  
		Last Modified: Thu, 25 Mar 2021 22:20:47 GMT  
		Size: 2.8 MB (2815332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f381c65aaaa0ed2d90609a1d94ca65fa057410a866389f0a380395c0f30dad9`  
		Last Modified: Fri, 26 Mar 2021 09:43:39 GMT  
		Size: 674.2 KB (674197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:201bd2f8d389731241ad12464a3c0e8dcf27fe7e8c5f26413ad17ec311573347`  
		Last Modified: Fri, 26 Mar 2021 09:44:08 GMT  
		Size: 21.1 MB (21116259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80eb8a05c6f082aedf128e275ce47294e63622bb8c19c53affb9bc9d6a3ac590`  
		Last Modified: Fri, 26 Mar 2021 09:44:04 GMT  
		Size: 369.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:1.7.28-alpine` - linux; arm variant v6

```console
$ docker pull traefik@sha256:31f0451328ced172b21c6254efec3ad8b0b93e74eed52d0121815324d02e21be
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.1 MB (23066960 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3981997446a1cad72ae513fb79a7443ffe0bc5b3c55413d0f9053f1021be6a09`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 25 Mar 2021 22:51:39 GMT
ADD file:f9e7465b7bf9cb6b234d24519c80b22b9da7894ea0337e0ac44920114773c8a9 in / 
# Thu, 25 Mar 2021 22:51:48 GMT
CMD ["/bin/sh"]
# Fri, 26 Mar 2021 10:23:59 GMT
RUN apk --no-cache add ca-certificates tzdata
# Fri, 26 Mar 2021 10:24:28 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/traefik/traefik/releases/download/v1.7.28/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Fri, 26 Mar 2021 10:24:29 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Fri, 26 Mar 2021 10:24:30 GMT
EXPOSE 80
# Fri, 26 Mar 2021 10:24:31 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 26 Mar 2021 10:24:33 GMT
CMD ["traefik"]
# Fri, 26 Mar 2021 10:24:34 GMT
LABEL org.opencontainers.image.vendor=traefik org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.28 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:275240b4b3a35cb935b35bfb1a8700e2b9ca100cd6e33ca8a6f83d056016bd61`  
		Last Modified: Thu, 25 Mar 2021 22:55:29 GMT  
		Size: 2.6 MB (2621328 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb7337eab7080efd44e620f96e74185d0ffeacba100c69045459249b2d3a3dd3`  
		Last Modified: Fri, 26 Mar 2021 10:25:07 GMT  
		Size: 677.0 KB (677007 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5393b92d65d5d154de06bb7fc8c8db2941f5f9c0536df8b348e963b63f7950f7`  
		Last Modified: Fri, 26 Mar 2021 10:25:33 GMT  
		Size: 19.8 MB (19768257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79773a7a5681d8dae4c1295c9a3354d8e59fd7e97153321d294f44c97f25ef83`  
		Last Modified: Fri, 26 Mar 2021 10:25:26 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:1.7.28-alpine` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:52e34452769038558151c3dbd0871763a9f5110ec680bbf7ad1bc4394c75de0f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **22.9 MB (22887814 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b10fb481f0a98ede8ac59c98224a31223ef8a8987c4490786685e024b3155d82`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 25 Mar 2021 22:41:33 GMT
ADD file:6fca680ab44d711c282deb126e7ad2f7ab51d84a6364192a4913e178f7d393a0 in / 
# Thu, 25 Mar 2021 22:41:38 GMT
CMD ["/bin/sh"]
# Fri, 26 Mar 2021 08:08:01 GMT
RUN apk --no-cache add ca-certificates tzdata
# Fri, 26 Mar 2021 08:08:24 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/traefik/traefik/releases/download/v1.7.28/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Fri, 26 Mar 2021 08:08:25 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Fri, 26 Mar 2021 08:08:26 GMT
EXPOSE 80
# Fri, 26 Mar 2021 08:08:27 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 26 Mar 2021 08:08:28 GMT
CMD ["traefik"]
# Fri, 26 Mar 2021 08:08:29 GMT
LABEL org.opencontainers.image.vendor=traefik org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.28 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:47185b9379cb432a7a6711ec279fdcb33fe0426be145e1bf61879568c9b54054`  
		Last Modified: Thu, 25 Mar 2021 22:45:46 GMT  
		Size: 2.7 MB (2725878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b107397c029a94008575072c0901eae0ac7977a9fe1fa05ed8e45757387f3be`  
		Last Modified: Fri, 26 Mar 2021 08:11:41 GMT  
		Size: 675.5 KB (675534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ec8eb5a4ab439b7e6632255add989c9df999239aff3b7c29caf94804b1c1e27`  
		Last Modified: Fri, 26 Mar 2021 08:12:05 GMT  
		Size: 19.5 MB (19486034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fba170bddfe05b0a040b3b25f421d499e4baf856e607552b0b9c90e49095415`  
		Last Modified: Fri, 26 Mar 2021 08:12:00 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:1.7.28-windowsservercore-1809`

```console
$ docker pull traefik@sha256:1a72007aed918f7be894ed6e10cd3f55a29a146785eacece8553c04640f3d809
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1817; amd64

### `traefik:1.7.28-windowsservercore-1809` - windows version 10.0.17763.1817; amd64

```console
$ docker pull traefik@sha256:76c78ecdfc533e552dc56a5469bc408dc38029acdc4d25347baf57dd14e0af6e
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2492116033 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4e6360dd33aca46bebf924fba8e817df599a404f2440fd9d311519d11c2a4f75`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 27 Feb 2021 09:32:06 GMT
RUN Install update 1809-amd64
# Wed, 10 Mar 2021 13:08:20 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Mar 2021 22:45:52 GMT
RUN Invoke-WebRequest     -Uri "https://github.com/traefik/traefik/releases/download/v1.7.28/traefik_windows-amd64.exe"     -OutFile "/traefik.exe"
# Wed, 10 Mar 2021 22:45:53 GMT
EXPOSE 80
# Wed, 10 Mar 2021 22:45:55 GMT
ENTRYPOINT ["/traefik"]
# Wed, 10 Mar 2021 22:45:56 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.28 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5ff1512f88ecd4ff0a91ade34d43733c48834433e35f062f80e6e70d706f8d73`  
		Size: 743.2 MB (743201590 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ebe61daec6d671bc2c1c6fe61ac9825fb552e9cef3672d0a7dbec719d125ae64`  
		Last Modified: Wed, 10 Mar 2021 13:21:09 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c01ec7e8fcbdf93c7395f18256527489b510fe69665c091ffb6d71278bf9aafe`  
		Last Modified: Wed, 10 Mar 2021 22:47:40 GMT  
		Size: 30.6 MB (30575844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afd90db339e07111b4a805bd4b081d78ba3dfe7db4bf9f207e0ac638a901671d`  
		Last Modified: Wed, 10 Mar 2021 22:46:59 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89dffb25733d38bdbe1dedc4e3ef916319ab71fb03cc9be7168c119df4f8a37d`  
		Last Modified: Wed, 10 Mar 2021 22:46:59 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97445bcb41cca852497b41557ab320aac9a24c5ba6867f77aa005249fb6a0d78`  
		Last Modified: Wed, 10 Mar 2021 22:46:59 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:2.4`

```console
$ docker pull traefik@sha256:2781953cc6d6445ec49ac487bc7d94f512ac4e413ca73611be36d63ceda42751
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:2.4` - linux; amd64

```console
$ docker pull traefik@sha256:297a4433372208769fb51168387ba56c048aa44113d4151be25e65dc158f916e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.8 MB (27827415 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:286716bfc172eecb6c7ed89847c944e0b0fed67fae2aba67fff284f6067df72c`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 25 Mar 2021 22:19:43 GMT
ADD file:05adf37fc1a41a31d8e0e0b9371a01161abc0d348adacbc81689a1a34e8fe12d in / 
# Thu, 25 Mar 2021 22:19:43 GMT
CMD ["/bin/sh"]
# Fri, 26 Mar 2021 09:42:59 GMT
RUN apk --no-cache add ca-certificates tzdata
# Fri, 26 Mar 2021 09:43:03 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.4.8/traefik_v2.4.8_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Fri, 26 Mar 2021 09:43:03 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Fri, 26 Mar 2021 09:43:03 GMT
EXPOSE 80
# Fri, 26 Mar 2021 09:43:04 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 26 Mar 2021 09:43:04 GMT
CMD ["traefik"]
# Fri, 26 Mar 2021 09:43:04 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.4.8 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:839b45e0263abc8ab2dc0bfabc91a19947e932ffbd551a93970ea3ee971eadf6`  
		Last Modified: Thu, 25 Mar 2021 22:20:47 GMT  
		Size: 2.8 MB (2815332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f381c65aaaa0ed2d90609a1d94ca65fa057410a866389f0a380395c0f30dad9`  
		Last Modified: Fri, 26 Mar 2021 09:43:39 GMT  
		Size: 674.2 KB (674197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f52a6f52c94839cba99c68125ffa1f8b521d969568b40f44ab87c7a2c0bd0876`  
		Last Modified: Fri, 26 Mar 2021 09:43:43 GMT  
		Size: 24.3 MB (24337518 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cb70c84da2b1068118347f8ae35e9bfa59c54684e205a6ef3159986776fc9f1`  
		Last Modified: Fri, 26 Mar 2021 09:43:38 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:2.4` - linux; arm variant v6

```console
$ docker pull traefik@sha256:8f5dafd50b571ddc6c6b8a9115fd2c8a4c5d84e09ae7db01625792506d980857
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.0 MB (26025821 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3754212e4b35fda67d7a32a946ebd55e9a660513f12aca82a22c57bba32781b4`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 25 Mar 2021 22:51:39 GMT
ADD file:f9e7465b7bf9cb6b234d24519c80b22b9da7894ea0337e0ac44920114773c8a9 in / 
# Thu, 25 Mar 2021 22:51:48 GMT
CMD ["/bin/sh"]
# Fri, 26 Mar 2021 10:23:59 GMT
RUN apk --no-cache add ca-certificates tzdata
# Fri, 26 Mar 2021 10:24:11 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.4.8/traefik_v2.4.8_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Fri, 26 Mar 2021 10:24:12 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Fri, 26 Mar 2021 10:24:13 GMT
EXPOSE 80
# Fri, 26 Mar 2021 10:24:14 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 26 Mar 2021 10:24:14 GMT
CMD ["traefik"]
# Fri, 26 Mar 2021 10:24:15 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.4.8 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:275240b4b3a35cb935b35bfb1a8700e2b9ca100cd6e33ca8a6f83d056016bd61`  
		Last Modified: Thu, 25 Mar 2021 22:55:29 GMT  
		Size: 2.6 MB (2621328 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb7337eab7080efd44e620f96e74185d0ffeacba100c69045459249b2d3a3dd3`  
		Last Modified: Fri, 26 Mar 2021 10:25:07 GMT  
		Size: 677.0 KB (677007 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:081d5433014b8e5186e1a9d24a8e4a4c298bb5d5f570b7677d84f77c76560541`  
		Last Modified: Fri, 26 Mar 2021 10:25:16 GMT  
		Size: 22.7 MB (22727118 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e75eb7078a4331e9b051b8d5d92b8882769d692d7505a70754de8357dc195a9`  
		Last Modified: Fri, 26 Mar 2021 10:25:07 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:2.4` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:9bb3516baf888fa5c81008c445ff63804f556ff68fee752a8c17fc8a8150db78
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.5 MB (25475525 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e1089720f9d91464f0161c603353bab15f2014e49e5228e134abae8bb3812600`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 25 Mar 2021 22:41:33 GMT
ADD file:6fca680ab44d711c282deb126e7ad2f7ab51d84a6364192a4913e178f7d393a0 in / 
# Thu, 25 Mar 2021 22:41:38 GMT
CMD ["/bin/sh"]
# Fri, 26 Mar 2021 08:08:01 GMT
RUN apk --no-cache add ca-certificates tzdata
# Fri, 26 Mar 2021 08:08:06 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.4.8/traefik_v2.4.8_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Fri, 26 Mar 2021 08:08:07 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Fri, 26 Mar 2021 08:08:09 GMT
EXPOSE 80
# Fri, 26 Mar 2021 08:08:09 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 26 Mar 2021 08:08:11 GMT
CMD ["traefik"]
# Fri, 26 Mar 2021 08:08:13 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.4.8 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:47185b9379cb432a7a6711ec279fdcb33fe0426be145e1bf61879568c9b54054`  
		Last Modified: Thu, 25 Mar 2021 22:45:46 GMT  
		Size: 2.7 MB (2725878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b107397c029a94008575072c0901eae0ac7977a9fe1fa05ed8e45757387f3be`  
		Last Modified: Fri, 26 Mar 2021 08:11:41 GMT  
		Size: 675.5 KB (675534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9cf36803d5e7ca9b3042d1847d12ee10baacbcf8e84b0aad89b7d9267714e29`  
		Last Modified: Fri, 26 Mar 2021 08:11:47 GMT  
		Size: 22.1 MB (22073745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf95742e6b158cadc348dddbb20aa9c7461bfe1441a1f5f3171117ac99538428`  
		Last Modified: Fri, 26 Mar 2021 08:11:41 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:2.4-windowsservercore-1809`

```console
$ docker pull traefik@sha256:37b2b7f435939b597589efb591686eca5a0e6ae850d1c80ec0cb3f996c05d24f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1817; amd64

### `traefik:2.4-windowsservercore-1809` - windows version 10.0.17763.1817; amd64

```console
$ docker pull traefik@sha256:9345ce86759b6cc6053762a836111a43408fa15fc5571fba77ea93b43deefa00
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2495650153 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f005e85992474d2eb3b06c7502a58d38c633edde288a548518128cd3e938f79c`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 27 Feb 2021 09:32:06 GMT
RUN Install update 1809-amd64
# Wed, 10 Mar 2021 13:08:20 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 24 Mar 2021 01:16:17 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/traefik/traefik/releases/download/v2.4.8/traefik_v2.4.8_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Wed, 24 Mar 2021 01:16:19 GMT
EXPOSE 80
# Wed, 24 Mar 2021 01:16:20 GMT
ENTRYPOINT ["/traefik"]
# Wed, 24 Mar 2021 01:16:21 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.4.8 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5ff1512f88ecd4ff0a91ade34d43733c48834433e35f062f80e6e70d706f8d73`  
		Size: 743.2 MB (743201590 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ebe61daec6d671bc2c1c6fe61ac9825fb552e9cef3672d0a7dbec719d125ae64`  
		Last Modified: Wed, 10 Mar 2021 13:21:09 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:138871c226c89b2e75588935069c544f0c8ce5f68930fab95af0e4ca5a825d73`  
		Last Modified: Wed, 24 Mar 2021 01:17:09 GMT  
		Size: 34.1 MB (34109955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b8574b4de7673b299ad666f81cd495bcfac5bf87fb33d4ef2781bdfcef30267`  
		Last Modified: Wed, 24 Mar 2021 01:16:56 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efb49e94abf40397ca09c966a1b4beb9579a20cb39ca8c9e17299ff206eb038e`  
		Last Modified: Wed, 24 Mar 2021 01:16:56 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c2d3f9210f45b7cb7f4c1ea77897d4576fcff778e51504d060afb3b28f4ae94`  
		Last Modified: Wed, 24 Mar 2021 01:16:56 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:2.4.8`

```console
$ docker pull traefik@sha256:2781953cc6d6445ec49ac487bc7d94f512ac4e413ca73611be36d63ceda42751
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:2.4.8` - linux; amd64

```console
$ docker pull traefik@sha256:297a4433372208769fb51168387ba56c048aa44113d4151be25e65dc158f916e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.8 MB (27827415 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:286716bfc172eecb6c7ed89847c944e0b0fed67fae2aba67fff284f6067df72c`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 25 Mar 2021 22:19:43 GMT
ADD file:05adf37fc1a41a31d8e0e0b9371a01161abc0d348adacbc81689a1a34e8fe12d in / 
# Thu, 25 Mar 2021 22:19:43 GMT
CMD ["/bin/sh"]
# Fri, 26 Mar 2021 09:42:59 GMT
RUN apk --no-cache add ca-certificates tzdata
# Fri, 26 Mar 2021 09:43:03 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.4.8/traefik_v2.4.8_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Fri, 26 Mar 2021 09:43:03 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Fri, 26 Mar 2021 09:43:03 GMT
EXPOSE 80
# Fri, 26 Mar 2021 09:43:04 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 26 Mar 2021 09:43:04 GMT
CMD ["traefik"]
# Fri, 26 Mar 2021 09:43:04 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.4.8 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:839b45e0263abc8ab2dc0bfabc91a19947e932ffbd551a93970ea3ee971eadf6`  
		Last Modified: Thu, 25 Mar 2021 22:20:47 GMT  
		Size: 2.8 MB (2815332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f381c65aaaa0ed2d90609a1d94ca65fa057410a866389f0a380395c0f30dad9`  
		Last Modified: Fri, 26 Mar 2021 09:43:39 GMT  
		Size: 674.2 KB (674197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f52a6f52c94839cba99c68125ffa1f8b521d969568b40f44ab87c7a2c0bd0876`  
		Last Modified: Fri, 26 Mar 2021 09:43:43 GMT  
		Size: 24.3 MB (24337518 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cb70c84da2b1068118347f8ae35e9bfa59c54684e205a6ef3159986776fc9f1`  
		Last Modified: Fri, 26 Mar 2021 09:43:38 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:2.4.8` - linux; arm variant v6

```console
$ docker pull traefik@sha256:8f5dafd50b571ddc6c6b8a9115fd2c8a4c5d84e09ae7db01625792506d980857
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.0 MB (26025821 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3754212e4b35fda67d7a32a946ebd55e9a660513f12aca82a22c57bba32781b4`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 25 Mar 2021 22:51:39 GMT
ADD file:f9e7465b7bf9cb6b234d24519c80b22b9da7894ea0337e0ac44920114773c8a9 in / 
# Thu, 25 Mar 2021 22:51:48 GMT
CMD ["/bin/sh"]
# Fri, 26 Mar 2021 10:23:59 GMT
RUN apk --no-cache add ca-certificates tzdata
# Fri, 26 Mar 2021 10:24:11 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.4.8/traefik_v2.4.8_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Fri, 26 Mar 2021 10:24:12 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Fri, 26 Mar 2021 10:24:13 GMT
EXPOSE 80
# Fri, 26 Mar 2021 10:24:14 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 26 Mar 2021 10:24:14 GMT
CMD ["traefik"]
# Fri, 26 Mar 2021 10:24:15 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.4.8 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:275240b4b3a35cb935b35bfb1a8700e2b9ca100cd6e33ca8a6f83d056016bd61`  
		Last Modified: Thu, 25 Mar 2021 22:55:29 GMT  
		Size: 2.6 MB (2621328 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb7337eab7080efd44e620f96e74185d0ffeacba100c69045459249b2d3a3dd3`  
		Last Modified: Fri, 26 Mar 2021 10:25:07 GMT  
		Size: 677.0 KB (677007 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:081d5433014b8e5186e1a9d24a8e4a4c298bb5d5f570b7677d84f77c76560541`  
		Last Modified: Fri, 26 Mar 2021 10:25:16 GMT  
		Size: 22.7 MB (22727118 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e75eb7078a4331e9b051b8d5d92b8882769d692d7505a70754de8357dc195a9`  
		Last Modified: Fri, 26 Mar 2021 10:25:07 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:2.4.8` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:9bb3516baf888fa5c81008c445ff63804f556ff68fee752a8c17fc8a8150db78
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.5 MB (25475525 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e1089720f9d91464f0161c603353bab15f2014e49e5228e134abae8bb3812600`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 25 Mar 2021 22:41:33 GMT
ADD file:6fca680ab44d711c282deb126e7ad2f7ab51d84a6364192a4913e178f7d393a0 in / 
# Thu, 25 Mar 2021 22:41:38 GMT
CMD ["/bin/sh"]
# Fri, 26 Mar 2021 08:08:01 GMT
RUN apk --no-cache add ca-certificates tzdata
# Fri, 26 Mar 2021 08:08:06 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.4.8/traefik_v2.4.8_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Fri, 26 Mar 2021 08:08:07 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Fri, 26 Mar 2021 08:08:09 GMT
EXPOSE 80
# Fri, 26 Mar 2021 08:08:09 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 26 Mar 2021 08:08:11 GMT
CMD ["traefik"]
# Fri, 26 Mar 2021 08:08:13 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.4.8 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:47185b9379cb432a7a6711ec279fdcb33fe0426be145e1bf61879568c9b54054`  
		Last Modified: Thu, 25 Mar 2021 22:45:46 GMT  
		Size: 2.7 MB (2725878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b107397c029a94008575072c0901eae0ac7977a9fe1fa05ed8e45757387f3be`  
		Last Modified: Fri, 26 Mar 2021 08:11:41 GMT  
		Size: 675.5 KB (675534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9cf36803d5e7ca9b3042d1847d12ee10baacbcf8e84b0aad89b7d9267714e29`  
		Last Modified: Fri, 26 Mar 2021 08:11:47 GMT  
		Size: 22.1 MB (22073745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf95742e6b158cadc348dddbb20aa9c7461bfe1441a1f5f3171117ac99538428`  
		Last Modified: Fri, 26 Mar 2021 08:11:41 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:2.4.8-windowsservercore-1809`

```console
$ docker pull traefik@sha256:37b2b7f435939b597589efb591686eca5a0e6ae850d1c80ec0cb3f996c05d24f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1817; amd64

### `traefik:2.4.8-windowsservercore-1809` - windows version 10.0.17763.1817; amd64

```console
$ docker pull traefik@sha256:9345ce86759b6cc6053762a836111a43408fa15fc5571fba77ea93b43deefa00
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2495650153 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f005e85992474d2eb3b06c7502a58d38c633edde288a548518128cd3e938f79c`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 27 Feb 2021 09:32:06 GMT
RUN Install update 1809-amd64
# Wed, 10 Mar 2021 13:08:20 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 24 Mar 2021 01:16:17 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/traefik/traefik/releases/download/v2.4.8/traefik_v2.4.8_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Wed, 24 Mar 2021 01:16:19 GMT
EXPOSE 80
# Wed, 24 Mar 2021 01:16:20 GMT
ENTRYPOINT ["/traefik"]
# Wed, 24 Mar 2021 01:16:21 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.4.8 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5ff1512f88ecd4ff0a91ade34d43733c48834433e35f062f80e6e70d706f8d73`  
		Size: 743.2 MB (743201590 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ebe61daec6d671bc2c1c6fe61ac9825fb552e9cef3672d0a7dbec719d125ae64`  
		Last Modified: Wed, 10 Mar 2021 13:21:09 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:138871c226c89b2e75588935069c544f0c8ce5f68930fab95af0e4ca5a825d73`  
		Last Modified: Wed, 24 Mar 2021 01:17:09 GMT  
		Size: 34.1 MB (34109955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b8574b4de7673b299ad666f81cd495bcfac5bf87fb33d4ef2781bdfcef30267`  
		Last Modified: Wed, 24 Mar 2021 01:16:56 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efb49e94abf40397ca09c966a1b4beb9579a20cb39ca8c9e17299ff206eb038e`  
		Last Modified: Wed, 24 Mar 2021 01:16:56 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c2d3f9210f45b7cb7f4c1ea77897d4576fcff778e51504d060afb3b28f4ae94`  
		Last Modified: Wed, 24 Mar 2021 01:16:56 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:latest`

```console
$ docker pull traefik@sha256:2781953cc6d6445ec49ac487bc7d94f512ac4e413ca73611be36d63ceda42751
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:latest` - linux; amd64

```console
$ docker pull traefik@sha256:297a4433372208769fb51168387ba56c048aa44113d4151be25e65dc158f916e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.8 MB (27827415 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:286716bfc172eecb6c7ed89847c944e0b0fed67fae2aba67fff284f6067df72c`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 25 Mar 2021 22:19:43 GMT
ADD file:05adf37fc1a41a31d8e0e0b9371a01161abc0d348adacbc81689a1a34e8fe12d in / 
# Thu, 25 Mar 2021 22:19:43 GMT
CMD ["/bin/sh"]
# Fri, 26 Mar 2021 09:42:59 GMT
RUN apk --no-cache add ca-certificates tzdata
# Fri, 26 Mar 2021 09:43:03 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.4.8/traefik_v2.4.8_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Fri, 26 Mar 2021 09:43:03 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Fri, 26 Mar 2021 09:43:03 GMT
EXPOSE 80
# Fri, 26 Mar 2021 09:43:04 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 26 Mar 2021 09:43:04 GMT
CMD ["traefik"]
# Fri, 26 Mar 2021 09:43:04 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.4.8 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:839b45e0263abc8ab2dc0bfabc91a19947e932ffbd551a93970ea3ee971eadf6`  
		Last Modified: Thu, 25 Mar 2021 22:20:47 GMT  
		Size: 2.8 MB (2815332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f381c65aaaa0ed2d90609a1d94ca65fa057410a866389f0a380395c0f30dad9`  
		Last Modified: Fri, 26 Mar 2021 09:43:39 GMT  
		Size: 674.2 KB (674197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f52a6f52c94839cba99c68125ffa1f8b521d969568b40f44ab87c7a2c0bd0876`  
		Last Modified: Fri, 26 Mar 2021 09:43:43 GMT  
		Size: 24.3 MB (24337518 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cb70c84da2b1068118347f8ae35e9bfa59c54684e205a6ef3159986776fc9f1`  
		Last Modified: Fri, 26 Mar 2021 09:43:38 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:latest` - linux; arm variant v6

```console
$ docker pull traefik@sha256:8f5dafd50b571ddc6c6b8a9115fd2c8a4c5d84e09ae7db01625792506d980857
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.0 MB (26025821 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3754212e4b35fda67d7a32a946ebd55e9a660513f12aca82a22c57bba32781b4`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 25 Mar 2021 22:51:39 GMT
ADD file:f9e7465b7bf9cb6b234d24519c80b22b9da7894ea0337e0ac44920114773c8a9 in / 
# Thu, 25 Mar 2021 22:51:48 GMT
CMD ["/bin/sh"]
# Fri, 26 Mar 2021 10:23:59 GMT
RUN apk --no-cache add ca-certificates tzdata
# Fri, 26 Mar 2021 10:24:11 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.4.8/traefik_v2.4.8_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Fri, 26 Mar 2021 10:24:12 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Fri, 26 Mar 2021 10:24:13 GMT
EXPOSE 80
# Fri, 26 Mar 2021 10:24:14 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 26 Mar 2021 10:24:14 GMT
CMD ["traefik"]
# Fri, 26 Mar 2021 10:24:15 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.4.8 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:275240b4b3a35cb935b35bfb1a8700e2b9ca100cd6e33ca8a6f83d056016bd61`  
		Last Modified: Thu, 25 Mar 2021 22:55:29 GMT  
		Size: 2.6 MB (2621328 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb7337eab7080efd44e620f96e74185d0ffeacba100c69045459249b2d3a3dd3`  
		Last Modified: Fri, 26 Mar 2021 10:25:07 GMT  
		Size: 677.0 KB (677007 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:081d5433014b8e5186e1a9d24a8e4a4c298bb5d5f570b7677d84f77c76560541`  
		Last Modified: Fri, 26 Mar 2021 10:25:16 GMT  
		Size: 22.7 MB (22727118 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e75eb7078a4331e9b051b8d5d92b8882769d692d7505a70754de8357dc195a9`  
		Last Modified: Fri, 26 Mar 2021 10:25:07 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:latest` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:9bb3516baf888fa5c81008c445ff63804f556ff68fee752a8c17fc8a8150db78
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.5 MB (25475525 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e1089720f9d91464f0161c603353bab15f2014e49e5228e134abae8bb3812600`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 25 Mar 2021 22:41:33 GMT
ADD file:6fca680ab44d711c282deb126e7ad2f7ab51d84a6364192a4913e178f7d393a0 in / 
# Thu, 25 Mar 2021 22:41:38 GMT
CMD ["/bin/sh"]
# Fri, 26 Mar 2021 08:08:01 GMT
RUN apk --no-cache add ca-certificates tzdata
# Fri, 26 Mar 2021 08:08:06 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.4.8/traefik_v2.4.8_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Fri, 26 Mar 2021 08:08:07 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Fri, 26 Mar 2021 08:08:09 GMT
EXPOSE 80
# Fri, 26 Mar 2021 08:08:09 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 26 Mar 2021 08:08:11 GMT
CMD ["traefik"]
# Fri, 26 Mar 2021 08:08:13 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.4.8 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:47185b9379cb432a7a6711ec279fdcb33fe0426be145e1bf61879568c9b54054`  
		Last Modified: Thu, 25 Mar 2021 22:45:46 GMT  
		Size: 2.7 MB (2725878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b107397c029a94008575072c0901eae0ac7977a9fe1fa05ed8e45757387f3be`  
		Last Modified: Fri, 26 Mar 2021 08:11:41 GMT  
		Size: 675.5 KB (675534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9cf36803d5e7ca9b3042d1847d12ee10baacbcf8e84b0aad89b7d9267714e29`  
		Last Modified: Fri, 26 Mar 2021 08:11:47 GMT  
		Size: 22.1 MB (22073745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf95742e6b158cadc348dddbb20aa9c7461bfe1441a1f5f3171117ac99538428`  
		Last Modified: Fri, 26 Mar 2021 08:11:41 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:livarot`

```console
$ docker pull traefik@sha256:2781953cc6d6445ec49ac487bc7d94f512ac4e413ca73611be36d63ceda42751
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:livarot` - linux; amd64

```console
$ docker pull traefik@sha256:297a4433372208769fb51168387ba56c048aa44113d4151be25e65dc158f916e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.8 MB (27827415 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:286716bfc172eecb6c7ed89847c944e0b0fed67fae2aba67fff284f6067df72c`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 25 Mar 2021 22:19:43 GMT
ADD file:05adf37fc1a41a31d8e0e0b9371a01161abc0d348adacbc81689a1a34e8fe12d in / 
# Thu, 25 Mar 2021 22:19:43 GMT
CMD ["/bin/sh"]
# Fri, 26 Mar 2021 09:42:59 GMT
RUN apk --no-cache add ca-certificates tzdata
# Fri, 26 Mar 2021 09:43:03 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.4.8/traefik_v2.4.8_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Fri, 26 Mar 2021 09:43:03 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Fri, 26 Mar 2021 09:43:03 GMT
EXPOSE 80
# Fri, 26 Mar 2021 09:43:04 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 26 Mar 2021 09:43:04 GMT
CMD ["traefik"]
# Fri, 26 Mar 2021 09:43:04 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.4.8 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:839b45e0263abc8ab2dc0bfabc91a19947e932ffbd551a93970ea3ee971eadf6`  
		Last Modified: Thu, 25 Mar 2021 22:20:47 GMT  
		Size: 2.8 MB (2815332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f381c65aaaa0ed2d90609a1d94ca65fa057410a866389f0a380395c0f30dad9`  
		Last Modified: Fri, 26 Mar 2021 09:43:39 GMT  
		Size: 674.2 KB (674197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f52a6f52c94839cba99c68125ffa1f8b521d969568b40f44ab87c7a2c0bd0876`  
		Last Modified: Fri, 26 Mar 2021 09:43:43 GMT  
		Size: 24.3 MB (24337518 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cb70c84da2b1068118347f8ae35e9bfa59c54684e205a6ef3159986776fc9f1`  
		Last Modified: Fri, 26 Mar 2021 09:43:38 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:livarot` - linux; arm variant v6

```console
$ docker pull traefik@sha256:8f5dafd50b571ddc6c6b8a9115fd2c8a4c5d84e09ae7db01625792506d980857
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.0 MB (26025821 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3754212e4b35fda67d7a32a946ebd55e9a660513f12aca82a22c57bba32781b4`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 25 Mar 2021 22:51:39 GMT
ADD file:f9e7465b7bf9cb6b234d24519c80b22b9da7894ea0337e0ac44920114773c8a9 in / 
# Thu, 25 Mar 2021 22:51:48 GMT
CMD ["/bin/sh"]
# Fri, 26 Mar 2021 10:23:59 GMT
RUN apk --no-cache add ca-certificates tzdata
# Fri, 26 Mar 2021 10:24:11 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.4.8/traefik_v2.4.8_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Fri, 26 Mar 2021 10:24:12 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Fri, 26 Mar 2021 10:24:13 GMT
EXPOSE 80
# Fri, 26 Mar 2021 10:24:14 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 26 Mar 2021 10:24:14 GMT
CMD ["traefik"]
# Fri, 26 Mar 2021 10:24:15 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.4.8 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:275240b4b3a35cb935b35bfb1a8700e2b9ca100cd6e33ca8a6f83d056016bd61`  
		Last Modified: Thu, 25 Mar 2021 22:55:29 GMT  
		Size: 2.6 MB (2621328 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb7337eab7080efd44e620f96e74185d0ffeacba100c69045459249b2d3a3dd3`  
		Last Modified: Fri, 26 Mar 2021 10:25:07 GMT  
		Size: 677.0 KB (677007 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:081d5433014b8e5186e1a9d24a8e4a4c298bb5d5f570b7677d84f77c76560541`  
		Last Modified: Fri, 26 Mar 2021 10:25:16 GMT  
		Size: 22.7 MB (22727118 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e75eb7078a4331e9b051b8d5d92b8882769d692d7505a70754de8357dc195a9`  
		Last Modified: Fri, 26 Mar 2021 10:25:07 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:livarot` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:9bb3516baf888fa5c81008c445ff63804f556ff68fee752a8c17fc8a8150db78
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.5 MB (25475525 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e1089720f9d91464f0161c603353bab15f2014e49e5228e134abae8bb3812600`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 25 Mar 2021 22:41:33 GMT
ADD file:6fca680ab44d711c282deb126e7ad2f7ab51d84a6364192a4913e178f7d393a0 in / 
# Thu, 25 Mar 2021 22:41:38 GMT
CMD ["/bin/sh"]
# Fri, 26 Mar 2021 08:08:01 GMT
RUN apk --no-cache add ca-certificates tzdata
# Fri, 26 Mar 2021 08:08:06 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.4.8/traefik_v2.4.8_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Fri, 26 Mar 2021 08:08:07 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Fri, 26 Mar 2021 08:08:09 GMT
EXPOSE 80
# Fri, 26 Mar 2021 08:08:09 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 26 Mar 2021 08:08:11 GMT
CMD ["traefik"]
# Fri, 26 Mar 2021 08:08:13 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.4.8 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:47185b9379cb432a7a6711ec279fdcb33fe0426be145e1bf61879568c9b54054`  
		Last Modified: Thu, 25 Mar 2021 22:45:46 GMT  
		Size: 2.7 MB (2725878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b107397c029a94008575072c0901eae0ac7977a9fe1fa05ed8e45757387f3be`  
		Last Modified: Fri, 26 Mar 2021 08:11:41 GMT  
		Size: 675.5 KB (675534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9cf36803d5e7ca9b3042d1847d12ee10baacbcf8e84b0aad89b7d9267714e29`  
		Last Modified: Fri, 26 Mar 2021 08:11:47 GMT  
		Size: 22.1 MB (22073745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf95742e6b158cadc348dddbb20aa9c7461bfe1441a1f5f3171117ac99538428`  
		Last Modified: Fri, 26 Mar 2021 08:11:41 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:livarot-windowsservercore-1809`

```console
$ docker pull traefik@sha256:37b2b7f435939b597589efb591686eca5a0e6ae850d1c80ec0cb3f996c05d24f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1817; amd64

### `traefik:livarot-windowsservercore-1809` - windows version 10.0.17763.1817; amd64

```console
$ docker pull traefik@sha256:9345ce86759b6cc6053762a836111a43408fa15fc5571fba77ea93b43deefa00
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2495650153 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f005e85992474d2eb3b06c7502a58d38c633edde288a548518128cd3e938f79c`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 27 Feb 2021 09:32:06 GMT
RUN Install update 1809-amd64
# Wed, 10 Mar 2021 13:08:20 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 24 Mar 2021 01:16:17 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/traefik/traefik/releases/download/v2.4.8/traefik_v2.4.8_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Wed, 24 Mar 2021 01:16:19 GMT
EXPOSE 80
# Wed, 24 Mar 2021 01:16:20 GMT
ENTRYPOINT ["/traefik"]
# Wed, 24 Mar 2021 01:16:21 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.4.8 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5ff1512f88ecd4ff0a91ade34d43733c48834433e35f062f80e6e70d706f8d73`  
		Size: 743.2 MB (743201590 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ebe61daec6d671bc2c1c6fe61ac9825fb552e9cef3672d0a7dbec719d125ae64`  
		Last Modified: Wed, 10 Mar 2021 13:21:09 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:138871c226c89b2e75588935069c544f0c8ce5f68930fab95af0e4ca5a825d73`  
		Last Modified: Wed, 24 Mar 2021 01:17:09 GMT  
		Size: 34.1 MB (34109955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b8574b4de7673b299ad666f81cd495bcfac5bf87fb33d4ef2781bdfcef30267`  
		Last Modified: Wed, 24 Mar 2021 01:16:56 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efb49e94abf40397ca09c966a1b4beb9579a20cb39ca8c9e17299ff206eb038e`  
		Last Modified: Wed, 24 Mar 2021 01:16:56 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c2d3f9210f45b7cb7f4c1ea77897d4576fcff778e51504d060afb3b28f4ae94`  
		Last Modified: Wed, 24 Mar 2021 01:16:56 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:maroilles`

```console
$ docker pull traefik@sha256:77db9c383b8294a959674d42306499048046046e144b6a7e7dfd0dc516e80571
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:maroilles` - linux; amd64

```console
$ docker pull traefik@sha256:af9ee4f13d77fdc35fd8c2d571b042001080754a5e69efca671bf3b382e29163
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **21.6 MB (21555693 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:11f7f6e41b0f0ee2d4e8ce90d77a2cf0615f0cfcd2b9e8d5cade2e564745d8f5`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Tue, 09 Mar 2021 01:32:48 GMT
COPY file:cd6264d9a7514a8fbc3eb7b400566d36178794d2b757959812cc3abc6f13a97b in /etc/ssl/certs/ 
# Tue, 09 Mar 2021 01:32:49 GMT
COPY dir:379603788862c2a6c57432d70b0a67f561fe00310e1b958c9ecf85381b1c9cd9 in /usr/share/ 
# Tue, 09 Mar 2021 01:32:49 GMT
COPY file:94b9997cc55c7732c9fc173c119f980e4a38eba20b96a90170a3d7fade75f0eb in / 
# Tue, 09 Mar 2021 01:32:50 GMT
EXPOSE 80
# Tue, 09 Mar 2021 01:32:50 GMT
VOLUME [/tmp]
# Tue, 09 Mar 2021 01:32:50 GMT
ENTRYPOINT ["/traefik"]
# Tue, 09 Mar 2021 01:32:50 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.28 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:7432563bc6a93a4a26e4fa5e0465d309dbfe1a4f5c13f945a90070f2acdcd897`  
		Last Modified: Tue, 09 Mar 2021 01:34:03 GMT  
		Size: 21.1 MB (21116000 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:maroilles` - linux; arm variant v6

```console
$ docker pull traefik@sha256:5eea4ce43832fb4fe06e6a76f4be2ee702cd7406bca2eeb28e7b8886b857fb60
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **20.2 MB (20207939 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a16dc71c18edfa988002598f7753875525a253977c27360950d4277cb5a12afb`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Thu, 17 Dec 2020 00:26:47 GMT
COPY file:cd6264d9a7514a8fbc3eb7b400566d36178794d2b757959812cc3abc6f13a97b in /etc/ssl/certs/ 
# Wed, 24 Feb 2021 23:34:19 GMT
COPY dir:379603788862c2a6c57432d70b0a67f561fe00310e1b958c9ecf85381b1c9cd9 in /usr/share/ 
# Wed, 24 Feb 2021 23:34:26 GMT
COPY file:3d9c1552db5b4c73ac7fe21268eeb20506f000d2e59d7be76697f45a50d32c64 in / 
# Wed, 24 Feb 2021 23:34:29 GMT
EXPOSE 80
# Wed, 24 Feb 2021 23:34:30 GMT
VOLUME [/tmp]
# Wed, 24 Feb 2021 23:34:31 GMT
ENTRYPOINT ["/traefik"]
# Wed, 24 Feb 2021 23:34:33 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.28 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:1eb5b49b6d2a16c38104badd82447927b16f7ba253b84d47c329449b778bb19d`  
		Last Modified: Wed, 24 Feb 2021 23:36:21 GMT  
		Size: 19.8 MB (19768211 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:maroilles` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:ea16e7c67604fa93b41900462522a8a595106d85a2320d07d84d7a39f9dd1ef0
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **19.9 MB (19925754 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:03d91b88a063e66b3027cc082d06fa36b001cc4ddc8d7cb3aad1e284f2a30f49`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Thu, 17 Dec 2020 00:27:56 GMT
COPY file:cd6264d9a7514a8fbc3eb7b400566d36178794d2b757959812cc3abc6f13a97b in /etc/ssl/certs/ 
# Thu, 25 Feb 2021 04:23:55 GMT
COPY dir:379603788862c2a6c57432d70b0a67f561fe00310e1b958c9ecf85381b1c9cd9 in /usr/share/ 
# Thu, 25 Feb 2021 04:23:57 GMT
COPY file:6bab4a8fc3d272fc29bc5ff42634cb12785fea9e23b0cf50f077702217bb6c03 in / 
# Thu, 25 Feb 2021 04:23:58 GMT
EXPOSE 80
# Thu, 25 Feb 2021 04:23:58 GMT
VOLUME [/tmp]
# Thu, 25 Feb 2021 04:23:59 GMT
ENTRYPOINT ["/traefik"]
# Thu, 25 Feb 2021 04:24:00 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.28 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:9fa98c5ef5e644f69a6a2346c2be14df34ac2e02195fcb75676fc1fe178f81b6`  
		Last Modified: Thu, 25 Feb 2021 04:25:21 GMT  
		Size: 19.5 MB (19486050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:maroilles-alpine`

```console
$ docker pull traefik@sha256:6f6ed7c4780aca850dd2d8a88e483c91a3e7e061bb28b912e72dd21056c45b27
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:maroilles-alpine` - linux; amd64

```console
$ docker pull traefik@sha256:11eab5d88ab546b5ffa5a5554809cd7f7f110c77976245d17f7192d8ebd27cd1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **24.6 MB (24606157 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c4ca93cce099f0cf7572f844fb03f2691539392bf54558b5c1a08a8616b63107`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 25 Mar 2021 22:19:43 GMT
ADD file:05adf37fc1a41a31d8e0e0b9371a01161abc0d348adacbc81689a1a34e8fe12d in / 
# Thu, 25 Mar 2021 22:19:43 GMT
CMD ["/bin/sh"]
# Fri, 26 Mar 2021 09:42:59 GMT
RUN apk --no-cache add ca-certificates tzdata
# Fri, 26 Mar 2021 09:43:11 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/traefik/traefik/releases/download/v1.7.28/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Fri, 26 Mar 2021 09:43:11 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Fri, 26 Mar 2021 09:43:12 GMT
EXPOSE 80
# Fri, 26 Mar 2021 09:43:12 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 26 Mar 2021 09:43:12 GMT
CMD ["traefik"]
# Fri, 26 Mar 2021 09:43:12 GMT
LABEL org.opencontainers.image.vendor=traefik org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.28 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:839b45e0263abc8ab2dc0bfabc91a19947e932ffbd551a93970ea3ee971eadf6`  
		Last Modified: Thu, 25 Mar 2021 22:20:47 GMT  
		Size: 2.8 MB (2815332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f381c65aaaa0ed2d90609a1d94ca65fa057410a866389f0a380395c0f30dad9`  
		Last Modified: Fri, 26 Mar 2021 09:43:39 GMT  
		Size: 674.2 KB (674197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:201bd2f8d389731241ad12464a3c0e8dcf27fe7e8c5f26413ad17ec311573347`  
		Last Modified: Fri, 26 Mar 2021 09:44:08 GMT  
		Size: 21.1 MB (21116259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80eb8a05c6f082aedf128e275ce47294e63622bb8c19c53affb9bc9d6a3ac590`  
		Last Modified: Fri, 26 Mar 2021 09:44:04 GMT  
		Size: 369.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:maroilles-alpine` - linux; arm variant v6

```console
$ docker pull traefik@sha256:31f0451328ced172b21c6254efec3ad8b0b93e74eed52d0121815324d02e21be
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.1 MB (23066960 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3981997446a1cad72ae513fb79a7443ffe0bc5b3c55413d0f9053f1021be6a09`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 25 Mar 2021 22:51:39 GMT
ADD file:f9e7465b7bf9cb6b234d24519c80b22b9da7894ea0337e0ac44920114773c8a9 in / 
# Thu, 25 Mar 2021 22:51:48 GMT
CMD ["/bin/sh"]
# Fri, 26 Mar 2021 10:23:59 GMT
RUN apk --no-cache add ca-certificates tzdata
# Fri, 26 Mar 2021 10:24:28 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/traefik/traefik/releases/download/v1.7.28/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Fri, 26 Mar 2021 10:24:29 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Fri, 26 Mar 2021 10:24:30 GMT
EXPOSE 80
# Fri, 26 Mar 2021 10:24:31 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 26 Mar 2021 10:24:33 GMT
CMD ["traefik"]
# Fri, 26 Mar 2021 10:24:34 GMT
LABEL org.opencontainers.image.vendor=traefik org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.28 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:275240b4b3a35cb935b35bfb1a8700e2b9ca100cd6e33ca8a6f83d056016bd61`  
		Last Modified: Thu, 25 Mar 2021 22:55:29 GMT  
		Size: 2.6 MB (2621328 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb7337eab7080efd44e620f96e74185d0ffeacba100c69045459249b2d3a3dd3`  
		Last Modified: Fri, 26 Mar 2021 10:25:07 GMT  
		Size: 677.0 KB (677007 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5393b92d65d5d154de06bb7fc8c8db2941f5f9c0536df8b348e963b63f7950f7`  
		Last Modified: Fri, 26 Mar 2021 10:25:33 GMT  
		Size: 19.8 MB (19768257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79773a7a5681d8dae4c1295c9a3354d8e59fd7e97153321d294f44c97f25ef83`  
		Last Modified: Fri, 26 Mar 2021 10:25:26 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:maroilles-alpine` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:52e34452769038558151c3dbd0871763a9f5110ec680bbf7ad1bc4394c75de0f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **22.9 MB (22887814 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b10fb481f0a98ede8ac59c98224a31223ef8a8987c4490786685e024b3155d82`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 25 Mar 2021 22:41:33 GMT
ADD file:6fca680ab44d711c282deb126e7ad2f7ab51d84a6364192a4913e178f7d393a0 in / 
# Thu, 25 Mar 2021 22:41:38 GMT
CMD ["/bin/sh"]
# Fri, 26 Mar 2021 08:08:01 GMT
RUN apk --no-cache add ca-certificates tzdata
# Fri, 26 Mar 2021 08:08:24 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/traefik/traefik/releases/download/v1.7.28/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Fri, 26 Mar 2021 08:08:25 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Fri, 26 Mar 2021 08:08:26 GMT
EXPOSE 80
# Fri, 26 Mar 2021 08:08:27 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 26 Mar 2021 08:08:28 GMT
CMD ["traefik"]
# Fri, 26 Mar 2021 08:08:29 GMT
LABEL org.opencontainers.image.vendor=traefik org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.28 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:47185b9379cb432a7a6711ec279fdcb33fe0426be145e1bf61879568c9b54054`  
		Last Modified: Thu, 25 Mar 2021 22:45:46 GMT  
		Size: 2.7 MB (2725878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b107397c029a94008575072c0901eae0ac7977a9fe1fa05ed8e45757387f3be`  
		Last Modified: Fri, 26 Mar 2021 08:11:41 GMT  
		Size: 675.5 KB (675534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ec8eb5a4ab439b7e6632255add989c9df999239aff3b7c29caf94804b1c1e27`  
		Last Modified: Fri, 26 Mar 2021 08:12:05 GMT  
		Size: 19.5 MB (19486034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fba170bddfe05b0a040b3b25f421d499e4baf856e607552b0b9c90e49095415`  
		Last Modified: Fri, 26 Mar 2021 08:12:00 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:maroilles-windowsservercore-1809`

```console
$ docker pull traefik@sha256:1a72007aed918f7be894ed6e10cd3f55a29a146785eacece8553c04640f3d809
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1817; amd64

### `traefik:maroilles-windowsservercore-1809` - windows version 10.0.17763.1817; amd64

```console
$ docker pull traefik@sha256:76c78ecdfc533e552dc56a5469bc408dc38029acdc4d25347baf57dd14e0af6e
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2492116033 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4e6360dd33aca46bebf924fba8e817df599a404f2440fd9d311519d11c2a4f75`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 27 Feb 2021 09:32:06 GMT
RUN Install update 1809-amd64
# Wed, 10 Mar 2021 13:08:20 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Mar 2021 22:45:52 GMT
RUN Invoke-WebRequest     -Uri "https://github.com/traefik/traefik/releases/download/v1.7.28/traefik_windows-amd64.exe"     -OutFile "/traefik.exe"
# Wed, 10 Mar 2021 22:45:53 GMT
EXPOSE 80
# Wed, 10 Mar 2021 22:45:55 GMT
ENTRYPOINT ["/traefik"]
# Wed, 10 Mar 2021 22:45:56 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.28 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5ff1512f88ecd4ff0a91ade34d43733c48834433e35f062f80e6e70d706f8d73`  
		Size: 743.2 MB (743201590 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ebe61daec6d671bc2c1c6fe61ac9825fb552e9cef3672d0a7dbec719d125ae64`  
		Last Modified: Wed, 10 Mar 2021 13:21:09 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c01ec7e8fcbdf93c7395f18256527489b510fe69665c091ffb6d71278bf9aafe`  
		Last Modified: Wed, 10 Mar 2021 22:47:40 GMT  
		Size: 30.6 MB (30575844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afd90db339e07111b4a805bd4b081d78ba3dfe7db4bf9f207e0ac638a901671d`  
		Last Modified: Wed, 10 Mar 2021 22:46:59 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89dffb25733d38bdbe1dedc4e3ef916319ab71fb03cc9be7168c119df4f8a37d`  
		Last Modified: Wed, 10 Mar 2021 22:46:59 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97445bcb41cca852497b41557ab320aac9a24c5ba6867f77aa005249fb6a0d78`  
		Last Modified: Wed, 10 Mar 2021 22:46:59 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v1.7`

```console
$ docker pull traefik@sha256:77db9c383b8294a959674d42306499048046046e144b6a7e7dfd0dc516e80571
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:v1.7` - linux; amd64

```console
$ docker pull traefik@sha256:af9ee4f13d77fdc35fd8c2d571b042001080754a5e69efca671bf3b382e29163
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **21.6 MB (21555693 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:11f7f6e41b0f0ee2d4e8ce90d77a2cf0615f0cfcd2b9e8d5cade2e564745d8f5`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Tue, 09 Mar 2021 01:32:48 GMT
COPY file:cd6264d9a7514a8fbc3eb7b400566d36178794d2b757959812cc3abc6f13a97b in /etc/ssl/certs/ 
# Tue, 09 Mar 2021 01:32:49 GMT
COPY dir:379603788862c2a6c57432d70b0a67f561fe00310e1b958c9ecf85381b1c9cd9 in /usr/share/ 
# Tue, 09 Mar 2021 01:32:49 GMT
COPY file:94b9997cc55c7732c9fc173c119f980e4a38eba20b96a90170a3d7fade75f0eb in / 
# Tue, 09 Mar 2021 01:32:50 GMT
EXPOSE 80
# Tue, 09 Mar 2021 01:32:50 GMT
VOLUME [/tmp]
# Tue, 09 Mar 2021 01:32:50 GMT
ENTRYPOINT ["/traefik"]
# Tue, 09 Mar 2021 01:32:50 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.28 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:7432563bc6a93a4a26e4fa5e0465d309dbfe1a4f5c13f945a90070f2acdcd897`  
		Last Modified: Tue, 09 Mar 2021 01:34:03 GMT  
		Size: 21.1 MB (21116000 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v1.7` - linux; arm variant v6

```console
$ docker pull traefik@sha256:5eea4ce43832fb4fe06e6a76f4be2ee702cd7406bca2eeb28e7b8886b857fb60
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **20.2 MB (20207939 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a16dc71c18edfa988002598f7753875525a253977c27360950d4277cb5a12afb`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Thu, 17 Dec 2020 00:26:47 GMT
COPY file:cd6264d9a7514a8fbc3eb7b400566d36178794d2b757959812cc3abc6f13a97b in /etc/ssl/certs/ 
# Wed, 24 Feb 2021 23:34:19 GMT
COPY dir:379603788862c2a6c57432d70b0a67f561fe00310e1b958c9ecf85381b1c9cd9 in /usr/share/ 
# Wed, 24 Feb 2021 23:34:26 GMT
COPY file:3d9c1552db5b4c73ac7fe21268eeb20506f000d2e59d7be76697f45a50d32c64 in / 
# Wed, 24 Feb 2021 23:34:29 GMT
EXPOSE 80
# Wed, 24 Feb 2021 23:34:30 GMT
VOLUME [/tmp]
# Wed, 24 Feb 2021 23:34:31 GMT
ENTRYPOINT ["/traefik"]
# Wed, 24 Feb 2021 23:34:33 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.28 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:1eb5b49b6d2a16c38104badd82447927b16f7ba253b84d47c329449b778bb19d`  
		Last Modified: Wed, 24 Feb 2021 23:36:21 GMT  
		Size: 19.8 MB (19768211 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v1.7` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:ea16e7c67604fa93b41900462522a8a595106d85a2320d07d84d7a39f9dd1ef0
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **19.9 MB (19925754 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:03d91b88a063e66b3027cc082d06fa36b001cc4ddc8d7cb3aad1e284f2a30f49`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Thu, 17 Dec 2020 00:27:56 GMT
COPY file:cd6264d9a7514a8fbc3eb7b400566d36178794d2b757959812cc3abc6f13a97b in /etc/ssl/certs/ 
# Thu, 25 Feb 2021 04:23:55 GMT
COPY dir:379603788862c2a6c57432d70b0a67f561fe00310e1b958c9ecf85381b1c9cd9 in /usr/share/ 
# Thu, 25 Feb 2021 04:23:57 GMT
COPY file:6bab4a8fc3d272fc29bc5ff42634cb12785fea9e23b0cf50f077702217bb6c03 in / 
# Thu, 25 Feb 2021 04:23:58 GMT
EXPOSE 80
# Thu, 25 Feb 2021 04:23:58 GMT
VOLUME [/tmp]
# Thu, 25 Feb 2021 04:23:59 GMT
ENTRYPOINT ["/traefik"]
# Thu, 25 Feb 2021 04:24:00 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.28 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:9fa98c5ef5e644f69a6a2346c2be14df34ac2e02195fcb75676fc1fe178f81b6`  
		Last Modified: Thu, 25 Feb 2021 04:25:21 GMT  
		Size: 19.5 MB (19486050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v1.7-alpine`

```console
$ docker pull traefik@sha256:6f6ed7c4780aca850dd2d8a88e483c91a3e7e061bb28b912e72dd21056c45b27
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:v1.7-alpine` - linux; amd64

```console
$ docker pull traefik@sha256:11eab5d88ab546b5ffa5a5554809cd7f7f110c77976245d17f7192d8ebd27cd1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **24.6 MB (24606157 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c4ca93cce099f0cf7572f844fb03f2691539392bf54558b5c1a08a8616b63107`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 25 Mar 2021 22:19:43 GMT
ADD file:05adf37fc1a41a31d8e0e0b9371a01161abc0d348adacbc81689a1a34e8fe12d in / 
# Thu, 25 Mar 2021 22:19:43 GMT
CMD ["/bin/sh"]
# Fri, 26 Mar 2021 09:42:59 GMT
RUN apk --no-cache add ca-certificates tzdata
# Fri, 26 Mar 2021 09:43:11 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/traefik/traefik/releases/download/v1.7.28/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Fri, 26 Mar 2021 09:43:11 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Fri, 26 Mar 2021 09:43:12 GMT
EXPOSE 80
# Fri, 26 Mar 2021 09:43:12 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 26 Mar 2021 09:43:12 GMT
CMD ["traefik"]
# Fri, 26 Mar 2021 09:43:12 GMT
LABEL org.opencontainers.image.vendor=traefik org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.28 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:839b45e0263abc8ab2dc0bfabc91a19947e932ffbd551a93970ea3ee971eadf6`  
		Last Modified: Thu, 25 Mar 2021 22:20:47 GMT  
		Size: 2.8 MB (2815332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f381c65aaaa0ed2d90609a1d94ca65fa057410a866389f0a380395c0f30dad9`  
		Last Modified: Fri, 26 Mar 2021 09:43:39 GMT  
		Size: 674.2 KB (674197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:201bd2f8d389731241ad12464a3c0e8dcf27fe7e8c5f26413ad17ec311573347`  
		Last Modified: Fri, 26 Mar 2021 09:44:08 GMT  
		Size: 21.1 MB (21116259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80eb8a05c6f082aedf128e275ce47294e63622bb8c19c53affb9bc9d6a3ac590`  
		Last Modified: Fri, 26 Mar 2021 09:44:04 GMT  
		Size: 369.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v1.7-alpine` - linux; arm variant v6

```console
$ docker pull traefik@sha256:31f0451328ced172b21c6254efec3ad8b0b93e74eed52d0121815324d02e21be
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.1 MB (23066960 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3981997446a1cad72ae513fb79a7443ffe0bc5b3c55413d0f9053f1021be6a09`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 25 Mar 2021 22:51:39 GMT
ADD file:f9e7465b7bf9cb6b234d24519c80b22b9da7894ea0337e0ac44920114773c8a9 in / 
# Thu, 25 Mar 2021 22:51:48 GMT
CMD ["/bin/sh"]
# Fri, 26 Mar 2021 10:23:59 GMT
RUN apk --no-cache add ca-certificates tzdata
# Fri, 26 Mar 2021 10:24:28 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/traefik/traefik/releases/download/v1.7.28/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Fri, 26 Mar 2021 10:24:29 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Fri, 26 Mar 2021 10:24:30 GMT
EXPOSE 80
# Fri, 26 Mar 2021 10:24:31 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 26 Mar 2021 10:24:33 GMT
CMD ["traefik"]
# Fri, 26 Mar 2021 10:24:34 GMT
LABEL org.opencontainers.image.vendor=traefik org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.28 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:275240b4b3a35cb935b35bfb1a8700e2b9ca100cd6e33ca8a6f83d056016bd61`  
		Last Modified: Thu, 25 Mar 2021 22:55:29 GMT  
		Size: 2.6 MB (2621328 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb7337eab7080efd44e620f96e74185d0ffeacba100c69045459249b2d3a3dd3`  
		Last Modified: Fri, 26 Mar 2021 10:25:07 GMT  
		Size: 677.0 KB (677007 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5393b92d65d5d154de06bb7fc8c8db2941f5f9c0536df8b348e963b63f7950f7`  
		Last Modified: Fri, 26 Mar 2021 10:25:33 GMT  
		Size: 19.8 MB (19768257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79773a7a5681d8dae4c1295c9a3354d8e59fd7e97153321d294f44c97f25ef83`  
		Last Modified: Fri, 26 Mar 2021 10:25:26 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v1.7-alpine` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:52e34452769038558151c3dbd0871763a9f5110ec680bbf7ad1bc4394c75de0f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **22.9 MB (22887814 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b10fb481f0a98ede8ac59c98224a31223ef8a8987c4490786685e024b3155d82`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 25 Mar 2021 22:41:33 GMT
ADD file:6fca680ab44d711c282deb126e7ad2f7ab51d84a6364192a4913e178f7d393a0 in / 
# Thu, 25 Mar 2021 22:41:38 GMT
CMD ["/bin/sh"]
# Fri, 26 Mar 2021 08:08:01 GMT
RUN apk --no-cache add ca-certificates tzdata
# Fri, 26 Mar 2021 08:08:24 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/traefik/traefik/releases/download/v1.7.28/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Fri, 26 Mar 2021 08:08:25 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Fri, 26 Mar 2021 08:08:26 GMT
EXPOSE 80
# Fri, 26 Mar 2021 08:08:27 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 26 Mar 2021 08:08:28 GMT
CMD ["traefik"]
# Fri, 26 Mar 2021 08:08:29 GMT
LABEL org.opencontainers.image.vendor=traefik org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.28 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:47185b9379cb432a7a6711ec279fdcb33fe0426be145e1bf61879568c9b54054`  
		Last Modified: Thu, 25 Mar 2021 22:45:46 GMT  
		Size: 2.7 MB (2725878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b107397c029a94008575072c0901eae0ac7977a9fe1fa05ed8e45757387f3be`  
		Last Modified: Fri, 26 Mar 2021 08:11:41 GMT  
		Size: 675.5 KB (675534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ec8eb5a4ab439b7e6632255add989c9df999239aff3b7c29caf94804b1c1e27`  
		Last Modified: Fri, 26 Mar 2021 08:12:05 GMT  
		Size: 19.5 MB (19486034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fba170bddfe05b0a040b3b25f421d499e4baf856e607552b0b9c90e49095415`  
		Last Modified: Fri, 26 Mar 2021 08:12:00 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v1.7-windowsservercore-1809`

```console
$ docker pull traefik@sha256:1a72007aed918f7be894ed6e10cd3f55a29a146785eacece8553c04640f3d809
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1817; amd64

### `traefik:v1.7-windowsservercore-1809` - windows version 10.0.17763.1817; amd64

```console
$ docker pull traefik@sha256:76c78ecdfc533e552dc56a5469bc408dc38029acdc4d25347baf57dd14e0af6e
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2492116033 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4e6360dd33aca46bebf924fba8e817df599a404f2440fd9d311519d11c2a4f75`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 27 Feb 2021 09:32:06 GMT
RUN Install update 1809-amd64
# Wed, 10 Mar 2021 13:08:20 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Mar 2021 22:45:52 GMT
RUN Invoke-WebRequest     -Uri "https://github.com/traefik/traefik/releases/download/v1.7.28/traefik_windows-amd64.exe"     -OutFile "/traefik.exe"
# Wed, 10 Mar 2021 22:45:53 GMT
EXPOSE 80
# Wed, 10 Mar 2021 22:45:55 GMT
ENTRYPOINT ["/traefik"]
# Wed, 10 Mar 2021 22:45:56 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.28 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5ff1512f88ecd4ff0a91ade34d43733c48834433e35f062f80e6e70d706f8d73`  
		Size: 743.2 MB (743201590 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ebe61daec6d671bc2c1c6fe61ac9825fb552e9cef3672d0a7dbec719d125ae64`  
		Last Modified: Wed, 10 Mar 2021 13:21:09 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c01ec7e8fcbdf93c7395f18256527489b510fe69665c091ffb6d71278bf9aafe`  
		Last Modified: Wed, 10 Mar 2021 22:47:40 GMT  
		Size: 30.6 MB (30575844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afd90db339e07111b4a805bd4b081d78ba3dfe7db4bf9f207e0ac638a901671d`  
		Last Modified: Wed, 10 Mar 2021 22:46:59 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89dffb25733d38bdbe1dedc4e3ef916319ab71fb03cc9be7168c119df4f8a37d`  
		Last Modified: Wed, 10 Mar 2021 22:46:59 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97445bcb41cca852497b41557ab320aac9a24c5ba6867f77aa005249fb6a0d78`  
		Last Modified: Wed, 10 Mar 2021 22:46:59 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v1.7.28`

```console
$ docker pull traefik@sha256:77db9c383b8294a959674d42306499048046046e144b6a7e7dfd0dc516e80571
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:v1.7.28` - linux; amd64

```console
$ docker pull traefik@sha256:af9ee4f13d77fdc35fd8c2d571b042001080754a5e69efca671bf3b382e29163
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **21.6 MB (21555693 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:11f7f6e41b0f0ee2d4e8ce90d77a2cf0615f0cfcd2b9e8d5cade2e564745d8f5`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Tue, 09 Mar 2021 01:32:48 GMT
COPY file:cd6264d9a7514a8fbc3eb7b400566d36178794d2b757959812cc3abc6f13a97b in /etc/ssl/certs/ 
# Tue, 09 Mar 2021 01:32:49 GMT
COPY dir:379603788862c2a6c57432d70b0a67f561fe00310e1b958c9ecf85381b1c9cd9 in /usr/share/ 
# Tue, 09 Mar 2021 01:32:49 GMT
COPY file:94b9997cc55c7732c9fc173c119f980e4a38eba20b96a90170a3d7fade75f0eb in / 
# Tue, 09 Mar 2021 01:32:50 GMT
EXPOSE 80
# Tue, 09 Mar 2021 01:32:50 GMT
VOLUME [/tmp]
# Tue, 09 Mar 2021 01:32:50 GMT
ENTRYPOINT ["/traefik"]
# Tue, 09 Mar 2021 01:32:50 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.28 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:7432563bc6a93a4a26e4fa5e0465d309dbfe1a4f5c13f945a90070f2acdcd897`  
		Last Modified: Tue, 09 Mar 2021 01:34:03 GMT  
		Size: 21.1 MB (21116000 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v1.7.28` - linux; arm variant v6

```console
$ docker pull traefik@sha256:5eea4ce43832fb4fe06e6a76f4be2ee702cd7406bca2eeb28e7b8886b857fb60
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **20.2 MB (20207939 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a16dc71c18edfa988002598f7753875525a253977c27360950d4277cb5a12afb`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Thu, 17 Dec 2020 00:26:47 GMT
COPY file:cd6264d9a7514a8fbc3eb7b400566d36178794d2b757959812cc3abc6f13a97b in /etc/ssl/certs/ 
# Wed, 24 Feb 2021 23:34:19 GMT
COPY dir:379603788862c2a6c57432d70b0a67f561fe00310e1b958c9ecf85381b1c9cd9 in /usr/share/ 
# Wed, 24 Feb 2021 23:34:26 GMT
COPY file:3d9c1552db5b4c73ac7fe21268eeb20506f000d2e59d7be76697f45a50d32c64 in / 
# Wed, 24 Feb 2021 23:34:29 GMT
EXPOSE 80
# Wed, 24 Feb 2021 23:34:30 GMT
VOLUME [/tmp]
# Wed, 24 Feb 2021 23:34:31 GMT
ENTRYPOINT ["/traefik"]
# Wed, 24 Feb 2021 23:34:33 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.28 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:1eb5b49b6d2a16c38104badd82447927b16f7ba253b84d47c329449b778bb19d`  
		Last Modified: Wed, 24 Feb 2021 23:36:21 GMT  
		Size: 19.8 MB (19768211 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v1.7.28` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:ea16e7c67604fa93b41900462522a8a595106d85a2320d07d84d7a39f9dd1ef0
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **19.9 MB (19925754 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:03d91b88a063e66b3027cc082d06fa36b001cc4ddc8d7cb3aad1e284f2a30f49`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Thu, 17 Dec 2020 00:27:56 GMT
COPY file:cd6264d9a7514a8fbc3eb7b400566d36178794d2b757959812cc3abc6f13a97b in /etc/ssl/certs/ 
# Thu, 25 Feb 2021 04:23:55 GMT
COPY dir:379603788862c2a6c57432d70b0a67f561fe00310e1b958c9ecf85381b1c9cd9 in /usr/share/ 
# Thu, 25 Feb 2021 04:23:57 GMT
COPY file:6bab4a8fc3d272fc29bc5ff42634cb12785fea9e23b0cf50f077702217bb6c03 in / 
# Thu, 25 Feb 2021 04:23:58 GMT
EXPOSE 80
# Thu, 25 Feb 2021 04:23:58 GMT
VOLUME [/tmp]
# Thu, 25 Feb 2021 04:23:59 GMT
ENTRYPOINT ["/traefik"]
# Thu, 25 Feb 2021 04:24:00 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.28 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:9fa98c5ef5e644f69a6a2346c2be14df34ac2e02195fcb75676fc1fe178f81b6`  
		Last Modified: Thu, 25 Feb 2021 04:25:21 GMT  
		Size: 19.5 MB (19486050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v1.7.28-alpine`

```console
$ docker pull traefik@sha256:6f6ed7c4780aca850dd2d8a88e483c91a3e7e061bb28b912e72dd21056c45b27
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:v1.7.28-alpine` - linux; amd64

```console
$ docker pull traefik@sha256:11eab5d88ab546b5ffa5a5554809cd7f7f110c77976245d17f7192d8ebd27cd1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **24.6 MB (24606157 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c4ca93cce099f0cf7572f844fb03f2691539392bf54558b5c1a08a8616b63107`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 25 Mar 2021 22:19:43 GMT
ADD file:05adf37fc1a41a31d8e0e0b9371a01161abc0d348adacbc81689a1a34e8fe12d in / 
# Thu, 25 Mar 2021 22:19:43 GMT
CMD ["/bin/sh"]
# Fri, 26 Mar 2021 09:42:59 GMT
RUN apk --no-cache add ca-certificates tzdata
# Fri, 26 Mar 2021 09:43:11 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/traefik/traefik/releases/download/v1.7.28/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Fri, 26 Mar 2021 09:43:11 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Fri, 26 Mar 2021 09:43:12 GMT
EXPOSE 80
# Fri, 26 Mar 2021 09:43:12 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 26 Mar 2021 09:43:12 GMT
CMD ["traefik"]
# Fri, 26 Mar 2021 09:43:12 GMT
LABEL org.opencontainers.image.vendor=traefik org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.28 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:839b45e0263abc8ab2dc0bfabc91a19947e932ffbd551a93970ea3ee971eadf6`  
		Last Modified: Thu, 25 Mar 2021 22:20:47 GMT  
		Size: 2.8 MB (2815332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f381c65aaaa0ed2d90609a1d94ca65fa057410a866389f0a380395c0f30dad9`  
		Last Modified: Fri, 26 Mar 2021 09:43:39 GMT  
		Size: 674.2 KB (674197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:201bd2f8d389731241ad12464a3c0e8dcf27fe7e8c5f26413ad17ec311573347`  
		Last Modified: Fri, 26 Mar 2021 09:44:08 GMT  
		Size: 21.1 MB (21116259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80eb8a05c6f082aedf128e275ce47294e63622bb8c19c53affb9bc9d6a3ac590`  
		Last Modified: Fri, 26 Mar 2021 09:44:04 GMT  
		Size: 369.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v1.7.28-alpine` - linux; arm variant v6

```console
$ docker pull traefik@sha256:31f0451328ced172b21c6254efec3ad8b0b93e74eed52d0121815324d02e21be
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.1 MB (23066960 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3981997446a1cad72ae513fb79a7443ffe0bc5b3c55413d0f9053f1021be6a09`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 25 Mar 2021 22:51:39 GMT
ADD file:f9e7465b7bf9cb6b234d24519c80b22b9da7894ea0337e0ac44920114773c8a9 in / 
# Thu, 25 Mar 2021 22:51:48 GMT
CMD ["/bin/sh"]
# Fri, 26 Mar 2021 10:23:59 GMT
RUN apk --no-cache add ca-certificates tzdata
# Fri, 26 Mar 2021 10:24:28 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/traefik/traefik/releases/download/v1.7.28/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Fri, 26 Mar 2021 10:24:29 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Fri, 26 Mar 2021 10:24:30 GMT
EXPOSE 80
# Fri, 26 Mar 2021 10:24:31 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 26 Mar 2021 10:24:33 GMT
CMD ["traefik"]
# Fri, 26 Mar 2021 10:24:34 GMT
LABEL org.opencontainers.image.vendor=traefik org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.28 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:275240b4b3a35cb935b35bfb1a8700e2b9ca100cd6e33ca8a6f83d056016bd61`  
		Last Modified: Thu, 25 Mar 2021 22:55:29 GMT  
		Size: 2.6 MB (2621328 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb7337eab7080efd44e620f96e74185d0ffeacba100c69045459249b2d3a3dd3`  
		Last Modified: Fri, 26 Mar 2021 10:25:07 GMT  
		Size: 677.0 KB (677007 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5393b92d65d5d154de06bb7fc8c8db2941f5f9c0536df8b348e963b63f7950f7`  
		Last Modified: Fri, 26 Mar 2021 10:25:33 GMT  
		Size: 19.8 MB (19768257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79773a7a5681d8dae4c1295c9a3354d8e59fd7e97153321d294f44c97f25ef83`  
		Last Modified: Fri, 26 Mar 2021 10:25:26 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v1.7.28-alpine` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:52e34452769038558151c3dbd0871763a9f5110ec680bbf7ad1bc4394c75de0f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **22.9 MB (22887814 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b10fb481f0a98ede8ac59c98224a31223ef8a8987c4490786685e024b3155d82`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 25 Mar 2021 22:41:33 GMT
ADD file:6fca680ab44d711c282deb126e7ad2f7ab51d84a6364192a4913e178f7d393a0 in / 
# Thu, 25 Mar 2021 22:41:38 GMT
CMD ["/bin/sh"]
# Fri, 26 Mar 2021 08:08:01 GMT
RUN apk --no-cache add ca-certificates tzdata
# Fri, 26 Mar 2021 08:08:24 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/traefik/traefik/releases/download/v1.7.28/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Fri, 26 Mar 2021 08:08:25 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Fri, 26 Mar 2021 08:08:26 GMT
EXPOSE 80
# Fri, 26 Mar 2021 08:08:27 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 26 Mar 2021 08:08:28 GMT
CMD ["traefik"]
# Fri, 26 Mar 2021 08:08:29 GMT
LABEL org.opencontainers.image.vendor=traefik org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.28 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:47185b9379cb432a7a6711ec279fdcb33fe0426be145e1bf61879568c9b54054`  
		Last Modified: Thu, 25 Mar 2021 22:45:46 GMT  
		Size: 2.7 MB (2725878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b107397c029a94008575072c0901eae0ac7977a9fe1fa05ed8e45757387f3be`  
		Last Modified: Fri, 26 Mar 2021 08:11:41 GMT  
		Size: 675.5 KB (675534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ec8eb5a4ab439b7e6632255add989c9df999239aff3b7c29caf94804b1c1e27`  
		Last Modified: Fri, 26 Mar 2021 08:12:05 GMT  
		Size: 19.5 MB (19486034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fba170bddfe05b0a040b3b25f421d499e4baf856e607552b0b9c90e49095415`  
		Last Modified: Fri, 26 Mar 2021 08:12:00 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v1.7.28-windowsservercore-1809`

```console
$ docker pull traefik@sha256:1a72007aed918f7be894ed6e10cd3f55a29a146785eacece8553c04640f3d809
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1817; amd64

### `traefik:v1.7.28-windowsservercore-1809` - windows version 10.0.17763.1817; amd64

```console
$ docker pull traefik@sha256:76c78ecdfc533e552dc56a5469bc408dc38029acdc4d25347baf57dd14e0af6e
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2492116033 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4e6360dd33aca46bebf924fba8e817df599a404f2440fd9d311519d11c2a4f75`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 27 Feb 2021 09:32:06 GMT
RUN Install update 1809-amd64
# Wed, 10 Mar 2021 13:08:20 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Mar 2021 22:45:52 GMT
RUN Invoke-WebRequest     -Uri "https://github.com/traefik/traefik/releases/download/v1.7.28/traefik_windows-amd64.exe"     -OutFile "/traefik.exe"
# Wed, 10 Mar 2021 22:45:53 GMT
EXPOSE 80
# Wed, 10 Mar 2021 22:45:55 GMT
ENTRYPOINT ["/traefik"]
# Wed, 10 Mar 2021 22:45:56 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.28 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5ff1512f88ecd4ff0a91ade34d43733c48834433e35f062f80e6e70d706f8d73`  
		Size: 743.2 MB (743201590 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ebe61daec6d671bc2c1c6fe61ac9825fb552e9cef3672d0a7dbec719d125ae64`  
		Last Modified: Wed, 10 Mar 2021 13:21:09 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c01ec7e8fcbdf93c7395f18256527489b510fe69665c091ffb6d71278bf9aafe`  
		Last Modified: Wed, 10 Mar 2021 22:47:40 GMT  
		Size: 30.6 MB (30575844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afd90db339e07111b4a805bd4b081d78ba3dfe7db4bf9f207e0ac638a901671d`  
		Last Modified: Wed, 10 Mar 2021 22:46:59 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89dffb25733d38bdbe1dedc4e3ef916319ab71fb03cc9be7168c119df4f8a37d`  
		Last Modified: Wed, 10 Mar 2021 22:46:59 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97445bcb41cca852497b41557ab320aac9a24c5ba6867f77aa005249fb6a0d78`  
		Last Modified: Wed, 10 Mar 2021 22:46:59 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v2.4`

```console
$ docker pull traefik@sha256:2781953cc6d6445ec49ac487bc7d94f512ac4e413ca73611be36d63ceda42751
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:v2.4` - linux; amd64

```console
$ docker pull traefik@sha256:297a4433372208769fb51168387ba56c048aa44113d4151be25e65dc158f916e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.8 MB (27827415 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:286716bfc172eecb6c7ed89847c944e0b0fed67fae2aba67fff284f6067df72c`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 25 Mar 2021 22:19:43 GMT
ADD file:05adf37fc1a41a31d8e0e0b9371a01161abc0d348adacbc81689a1a34e8fe12d in / 
# Thu, 25 Mar 2021 22:19:43 GMT
CMD ["/bin/sh"]
# Fri, 26 Mar 2021 09:42:59 GMT
RUN apk --no-cache add ca-certificates tzdata
# Fri, 26 Mar 2021 09:43:03 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.4.8/traefik_v2.4.8_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Fri, 26 Mar 2021 09:43:03 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Fri, 26 Mar 2021 09:43:03 GMT
EXPOSE 80
# Fri, 26 Mar 2021 09:43:04 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 26 Mar 2021 09:43:04 GMT
CMD ["traefik"]
# Fri, 26 Mar 2021 09:43:04 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.4.8 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:839b45e0263abc8ab2dc0bfabc91a19947e932ffbd551a93970ea3ee971eadf6`  
		Last Modified: Thu, 25 Mar 2021 22:20:47 GMT  
		Size: 2.8 MB (2815332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f381c65aaaa0ed2d90609a1d94ca65fa057410a866389f0a380395c0f30dad9`  
		Last Modified: Fri, 26 Mar 2021 09:43:39 GMT  
		Size: 674.2 KB (674197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f52a6f52c94839cba99c68125ffa1f8b521d969568b40f44ab87c7a2c0bd0876`  
		Last Modified: Fri, 26 Mar 2021 09:43:43 GMT  
		Size: 24.3 MB (24337518 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cb70c84da2b1068118347f8ae35e9bfa59c54684e205a6ef3159986776fc9f1`  
		Last Modified: Fri, 26 Mar 2021 09:43:38 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v2.4` - linux; arm variant v6

```console
$ docker pull traefik@sha256:8f5dafd50b571ddc6c6b8a9115fd2c8a4c5d84e09ae7db01625792506d980857
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.0 MB (26025821 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3754212e4b35fda67d7a32a946ebd55e9a660513f12aca82a22c57bba32781b4`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 25 Mar 2021 22:51:39 GMT
ADD file:f9e7465b7bf9cb6b234d24519c80b22b9da7894ea0337e0ac44920114773c8a9 in / 
# Thu, 25 Mar 2021 22:51:48 GMT
CMD ["/bin/sh"]
# Fri, 26 Mar 2021 10:23:59 GMT
RUN apk --no-cache add ca-certificates tzdata
# Fri, 26 Mar 2021 10:24:11 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.4.8/traefik_v2.4.8_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Fri, 26 Mar 2021 10:24:12 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Fri, 26 Mar 2021 10:24:13 GMT
EXPOSE 80
# Fri, 26 Mar 2021 10:24:14 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 26 Mar 2021 10:24:14 GMT
CMD ["traefik"]
# Fri, 26 Mar 2021 10:24:15 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.4.8 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:275240b4b3a35cb935b35bfb1a8700e2b9ca100cd6e33ca8a6f83d056016bd61`  
		Last Modified: Thu, 25 Mar 2021 22:55:29 GMT  
		Size: 2.6 MB (2621328 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb7337eab7080efd44e620f96e74185d0ffeacba100c69045459249b2d3a3dd3`  
		Last Modified: Fri, 26 Mar 2021 10:25:07 GMT  
		Size: 677.0 KB (677007 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:081d5433014b8e5186e1a9d24a8e4a4c298bb5d5f570b7677d84f77c76560541`  
		Last Modified: Fri, 26 Mar 2021 10:25:16 GMT  
		Size: 22.7 MB (22727118 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e75eb7078a4331e9b051b8d5d92b8882769d692d7505a70754de8357dc195a9`  
		Last Modified: Fri, 26 Mar 2021 10:25:07 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v2.4` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:9bb3516baf888fa5c81008c445ff63804f556ff68fee752a8c17fc8a8150db78
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.5 MB (25475525 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e1089720f9d91464f0161c603353bab15f2014e49e5228e134abae8bb3812600`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 25 Mar 2021 22:41:33 GMT
ADD file:6fca680ab44d711c282deb126e7ad2f7ab51d84a6364192a4913e178f7d393a0 in / 
# Thu, 25 Mar 2021 22:41:38 GMT
CMD ["/bin/sh"]
# Fri, 26 Mar 2021 08:08:01 GMT
RUN apk --no-cache add ca-certificates tzdata
# Fri, 26 Mar 2021 08:08:06 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.4.8/traefik_v2.4.8_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Fri, 26 Mar 2021 08:08:07 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Fri, 26 Mar 2021 08:08:09 GMT
EXPOSE 80
# Fri, 26 Mar 2021 08:08:09 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 26 Mar 2021 08:08:11 GMT
CMD ["traefik"]
# Fri, 26 Mar 2021 08:08:13 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.4.8 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:47185b9379cb432a7a6711ec279fdcb33fe0426be145e1bf61879568c9b54054`  
		Last Modified: Thu, 25 Mar 2021 22:45:46 GMT  
		Size: 2.7 MB (2725878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b107397c029a94008575072c0901eae0ac7977a9fe1fa05ed8e45757387f3be`  
		Last Modified: Fri, 26 Mar 2021 08:11:41 GMT  
		Size: 675.5 KB (675534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9cf36803d5e7ca9b3042d1847d12ee10baacbcf8e84b0aad89b7d9267714e29`  
		Last Modified: Fri, 26 Mar 2021 08:11:47 GMT  
		Size: 22.1 MB (22073745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf95742e6b158cadc348dddbb20aa9c7461bfe1441a1f5f3171117ac99538428`  
		Last Modified: Fri, 26 Mar 2021 08:11:41 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v2.4-windowsservercore-1809`

```console
$ docker pull traefik@sha256:37b2b7f435939b597589efb591686eca5a0e6ae850d1c80ec0cb3f996c05d24f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1817; amd64

### `traefik:v2.4-windowsservercore-1809` - windows version 10.0.17763.1817; amd64

```console
$ docker pull traefik@sha256:9345ce86759b6cc6053762a836111a43408fa15fc5571fba77ea93b43deefa00
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2495650153 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f005e85992474d2eb3b06c7502a58d38c633edde288a548518128cd3e938f79c`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 27 Feb 2021 09:32:06 GMT
RUN Install update 1809-amd64
# Wed, 10 Mar 2021 13:08:20 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 24 Mar 2021 01:16:17 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/traefik/traefik/releases/download/v2.4.8/traefik_v2.4.8_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Wed, 24 Mar 2021 01:16:19 GMT
EXPOSE 80
# Wed, 24 Mar 2021 01:16:20 GMT
ENTRYPOINT ["/traefik"]
# Wed, 24 Mar 2021 01:16:21 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.4.8 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5ff1512f88ecd4ff0a91ade34d43733c48834433e35f062f80e6e70d706f8d73`  
		Size: 743.2 MB (743201590 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ebe61daec6d671bc2c1c6fe61ac9825fb552e9cef3672d0a7dbec719d125ae64`  
		Last Modified: Wed, 10 Mar 2021 13:21:09 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:138871c226c89b2e75588935069c544f0c8ce5f68930fab95af0e4ca5a825d73`  
		Last Modified: Wed, 24 Mar 2021 01:17:09 GMT  
		Size: 34.1 MB (34109955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b8574b4de7673b299ad666f81cd495bcfac5bf87fb33d4ef2781bdfcef30267`  
		Last Modified: Wed, 24 Mar 2021 01:16:56 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efb49e94abf40397ca09c966a1b4beb9579a20cb39ca8c9e17299ff206eb038e`  
		Last Modified: Wed, 24 Mar 2021 01:16:56 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c2d3f9210f45b7cb7f4c1ea77897d4576fcff778e51504d060afb3b28f4ae94`  
		Last Modified: Wed, 24 Mar 2021 01:16:56 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v2.4.8`

```console
$ docker pull traefik@sha256:2781953cc6d6445ec49ac487bc7d94f512ac4e413ca73611be36d63ceda42751
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:v2.4.8` - linux; amd64

```console
$ docker pull traefik@sha256:297a4433372208769fb51168387ba56c048aa44113d4151be25e65dc158f916e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.8 MB (27827415 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:286716bfc172eecb6c7ed89847c944e0b0fed67fae2aba67fff284f6067df72c`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 25 Mar 2021 22:19:43 GMT
ADD file:05adf37fc1a41a31d8e0e0b9371a01161abc0d348adacbc81689a1a34e8fe12d in / 
# Thu, 25 Mar 2021 22:19:43 GMT
CMD ["/bin/sh"]
# Fri, 26 Mar 2021 09:42:59 GMT
RUN apk --no-cache add ca-certificates tzdata
# Fri, 26 Mar 2021 09:43:03 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.4.8/traefik_v2.4.8_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Fri, 26 Mar 2021 09:43:03 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Fri, 26 Mar 2021 09:43:03 GMT
EXPOSE 80
# Fri, 26 Mar 2021 09:43:04 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 26 Mar 2021 09:43:04 GMT
CMD ["traefik"]
# Fri, 26 Mar 2021 09:43:04 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.4.8 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:839b45e0263abc8ab2dc0bfabc91a19947e932ffbd551a93970ea3ee971eadf6`  
		Last Modified: Thu, 25 Mar 2021 22:20:47 GMT  
		Size: 2.8 MB (2815332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f381c65aaaa0ed2d90609a1d94ca65fa057410a866389f0a380395c0f30dad9`  
		Last Modified: Fri, 26 Mar 2021 09:43:39 GMT  
		Size: 674.2 KB (674197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f52a6f52c94839cba99c68125ffa1f8b521d969568b40f44ab87c7a2c0bd0876`  
		Last Modified: Fri, 26 Mar 2021 09:43:43 GMT  
		Size: 24.3 MB (24337518 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cb70c84da2b1068118347f8ae35e9bfa59c54684e205a6ef3159986776fc9f1`  
		Last Modified: Fri, 26 Mar 2021 09:43:38 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v2.4.8` - linux; arm variant v6

```console
$ docker pull traefik@sha256:8f5dafd50b571ddc6c6b8a9115fd2c8a4c5d84e09ae7db01625792506d980857
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.0 MB (26025821 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3754212e4b35fda67d7a32a946ebd55e9a660513f12aca82a22c57bba32781b4`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 25 Mar 2021 22:51:39 GMT
ADD file:f9e7465b7bf9cb6b234d24519c80b22b9da7894ea0337e0ac44920114773c8a9 in / 
# Thu, 25 Mar 2021 22:51:48 GMT
CMD ["/bin/sh"]
# Fri, 26 Mar 2021 10:23:59 GMT
RUN apk --no-cache add ca-certificates tzdata
# Fri, 26 Mar 2021 10:24:11 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.4.8/traefik_v2.4.8_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Fri, 26 Mar 2021 10:24:12 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Fri, 26 Mar 2021 10:24:13 GMT
EXPOSE 80
# Fri, 26 Mar 2021 10:24:14 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 26 Mar 2021 10:24:14 GMT
CMD ["traefik"]
# Fri, 26 Mar 2021 10:24:15 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.4.8 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:275240b4b3a35cb935b35bfb1a8700e2b9ca100cd6e33ca8a6f83d056016bd61`  
		Last Modified: Thu, 25 Mar 2021 22:55:29 GMT  
		Size: 2.6 MB (2621328 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb7337eab7080efd44e620f96e74185d0ffeacba100c69045459249b2d3a3dd3`  
		Last Modified: Fri, 26 Mar 2021 10:25:07 GMT  
		Size: 677.0 KB (677007 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:081d5433014b8e5186e1a9d24a8e4a4c298bb5d5f570b7677d84f77c76560541`  
		Last Modified: Fri, 26 Mar 2021 10:25:16 GMT  
		Size: 22.7 MB (22727118 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e75eb7078a4331e9b051b8d5d92b8882769d692d7505a70754de8357dc195a9`  
		Last Modified: Fri, 26 Mar 2021 10:25:07 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v2.4.8` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:9bb3516baf888fa5c81008c445ff63804f556ff68fee752a8c17fc8a8150db78
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.5 MB (25475525 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e1089720f9d91464f0161c603353bab15f2014e49e5228e134abae8bb3812600`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 25 Mar 2021 22:41:33 GMT
ADD file:6fca680ab44d711c282deb126e7ad2f7ab51d84a6364192a4913e178f7d393a0 in / 
# Thu, 25 Mar 2021 22:41:38 GMT
CMD ["/bin/sh"]
# Fri, 26 Mar 2021 08:08:01 GMT
RUN apk --no-cache add ca-certificates tzdata
# Fri, 26 Mar 2021 08:08:06 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.4.8/traefik_v2.4.8_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Fri, 26 Mar 2021 08:08:07 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Fri, 26 Mar 2021 08:08:09 GMT
EXPOSE 80
# Fri, 26 Mar 2021 08:08:09 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 26 Mar 2021 08:08:11 GMT
CMD ["traefik"]
# Fri, 26 Mar 2021 08:08:13 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.4.8 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:47185b9379cb432a7a6711ec279fdcb33fe0426be145e1bf61879568c9b54054`  
		Last Modified: Thu, 25 Mar 2021 22:45:46 GMT  
		Size: 2.7 MB (2725878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b107397c029a94008575072c0901eae0ac7977a9fe1fa05ed8e45757387f3be`  
		Last Modified: Fri, 26 Mar 2021 08:11:41 GMT  
		Size: 675.5 KB (675534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9cf36803d5e7ca9b3042d1847d12ee10baacbcf8e84b0aad89b7d9267714e29`  
		Last Modified: Fri, 26 Mar 2021 08:11:47 GMT  
		Size: 22.1 MB (22073745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf95742e6b158cadc348dddbb20aa9c7461bfe1441a1f5f3171117ac99538428`  
		Last Modified: Fri, 26 Mar 2021 08:11:41 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v2.4.8-windowsservercore-1809`

```console
$ docker pull traefik@sha256:37b2b7f435939b597589efb591686eca5a0e6ae850d1c80ec0cb3f996c05d24f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1817; amd64

### `traefik:v2.4.8-windowsservercore-1809` - windows version 10.0.17763.1817; amd64

```console
$ docker pull traefik@sha256:9345ce86759b6cc6053762a836111a43408fa15fc5571fba77ea93b43deefa00
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2495650153 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f005e85992474d2eb3b06c7502a58d38c633edde288a548518128cd3e938f79c`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 27 Feb 2021 09:32:06 GMT
RUN Install update 1809-amd64
# Wed, 10 Mar 2021 13:08:20 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 24 Mar 2021 01:16:17 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/traefik/traefik/releases/download/v2.4.8/traefik_v2.4.8_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Wed, 24 Mar 2021 01:16:19 GMT
EXPOSE 80
# Wed, 24 Mar 2021 01:16:20 GMT
ENTRYPOINT ["/traefik"]
# Wed, 24 Mar 2021 01:16:21 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.4.8 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5ff1512f88ecd4ff0a91ade34d43733c48834433e35f062f80e6e70d706f8d73`  
		Size: 743.2 MB (743201590 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ebe61daec6d671bc2c1c6fe61ac9825fb552e9cef3672d0a7dbec719d125ae64`  
		Last Modified: Wed, 10 Mar 2021 13:21:09 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:138871c226c89b2e75588935069c544f0c8ce5f68930fab95af0e4ca5a825d73`  
		Last Modified: Wed, 24 Mar 2021 01:17:09 GMT  
		Size: 34.1 MB (34109955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b8574b4de7673b299ad666f81cd495bcfac5bf87fb33d4ef2781bdfcef30267`  
		Last Modified: Wed, 24 Mar 2021 01:16:56 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efb49e94abf40397ca09c966a1b4beb9579a20cb39ca8c9e17299ff206eb038e`  
		Last Modified: Wed, 24 Mar 2021 01:16:56 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c2d3f9210f45b7cb7f4c1ea77897d4576fcff778e51504d060afb3b28f4ae94`  
		Last Modified: Wed, 24 Mar 2021 01:16:56 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:windowsservercore-1809`

```console
$ docker pull traefik@sha256:37b2b7f435939b597589efb591686eca5a0e6ae850d1c80ec0cb3f996c05d24f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1817; amd64

### `traefik:windowsservercore-1809` - windows version 10.0.17763.1817; amd64

```console
$ docker pull traefik@sha256:9345ce86759b6cc6053762a836111a43408fa15fc5571fba77ea93b43deefa00
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2495650153 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f005e85992474d2eb3b06c7502a58d38c633edde288a548518128cd3e938f79c`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 27 Feb 2021 09:32:06 GMT
RUN Install update 1809-amd64
# Wed, 10 Mar 2021 13:08:20 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 24 Mar 2021 01:16:17 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/traefik/traefik/releases/download/v2.4.8/traefik_v2.4.8_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Wed, 24 Mar 2021 01:16:19 GMT
EXPOSE 80
# Wed, 24 Mar 2021 01:16:20 GMT
ENTRYPOINT ["/traefik"]
# Wed, 24 Mar 2021 01:16:21 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.4.8 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5ff1512f88ecd4ff0a91ade34d43733c48834433e35f062f80e6e70d706f8d73`  
		Size: 743.2 MB (743201590 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ebe61daec6d671bc2c1c6fe61ac9825fb552e9cef3672d0a7dbec719d125ae64`  
		Last Modified: Wed, 10 Mar 2021 13:21:09 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:138871c226c89b2e75588935069c544f0c8ce5f68930fab95af0e4ca5a825d73`  
		Last Modified: Wed, 24 Mar 2021 01:17:09 GMT  
		Size: 34.1 MB (34109955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b8574b4de7673b299ad666f81cd495bcfac5bf87fb33d4ef2781bdfcef30267`  
		Last Modified: Wed, 24 Mar 2021 01:16:56 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efb49e94abf40397ca09c966a1b4beb9579a20cb39ca8c9e17299ff206eb038e`  
		Last Modified: Wed, 24 Mar 2021 01:16:56 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c2d3f9210f45b7cb7f4c1ea77897d4576fcff778e51504d060afb3b28f4ae94`  
		Last Modified: Wed, 24 Mar 2021 01:16:56 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
