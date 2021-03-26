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
$ docker pull traefik@sha256:2fe12e2958a0324f0ec02d858e7475fc8962b85e59d4c43a1f1bfd8b87f1059d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:1.7-alpine` - linux; amd64

```console
$ docker pull traefik@sha256:71f17992f437d3bbde3be6510b559159426e0bf22ee16af4b4f388a6d1193aa8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **24.6 MB (24606120 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:90599305b6e12aa47a2e1f5231cff859c4e3f649a14063df98ff5ddcaa9264e8`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 24 Feb 2021 20:20:11 GMT
ADD file:7eeea546ecde7a036bf634c08719879d32c7ec6ae599708cd91dc1b830735223 in / 
# Wed, 24 Feb 2021 20:20:12 GMT
CMD ["/bin/sh"]
# Tue, 09 Mar 2021 01:32:30 GMT
RUN apk --no-cache add ca-certificates tzdata
# Tue, 09 Mar 2021 01:32:41 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/traefik/traefik/releases/download/v1.7.28/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Tue, 09 Mar 2021 01:32:41 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Tue, 09 Mar 2021 01:32:41 GMT
EXPOSE 80
# Tue, 09 Mar 2021 01:32:42 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 09 Mar 2021 01:32:42 GMT
CMD ["traefik"]
# Tue, 09 Mar 2021 01:32:42 GMT
LABEL org.opencontainers.image.vendor=traefik org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.28 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:e95f33c60a645d6d31f52fdc334aecec0d79a1b410789eae37fbf69efcd587ab`  
		Last Modified: Wed, 24 Feb 2021 20:20:43 GMT  
		Size: 2.8 MB (2815313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e824fcc855ce466fcd783344fbc46e46eb8f786d642a60d7b75aecc31c0396d`  
		Last Modified: Tue, 09 Mar 2021 01:33:13 GMT  
		Size: 674.2 KB (674166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d0a7f1c496515ee0f8f5dc274c699158012873705bcfb5d3527832885b8dd05`  
		Last Modified: Tue, 09 Mar 2021 01:33:41 GMT  
		Size: 21.1 MB (21116273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5952bd804d03e773a53210515aaf4c07475739f157d0a13d352f34cfb1b9131d`  
		Last Modified: Tue, 09 Mar 2021 01:33:38 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:1.7-alpine` - linux; arm variant v6

```console
$ docker pull traefik@sha256:f3ab2c547fbc76d59301ed2f0464b796b57b4f5373ab9dfef877a1bc58464bbd
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.1 MB (23066669 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c7ff9159190f81182f781e4191b0558c229fb328121a58e6e9254409ddf3fae4`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 24 Feb 2021 20:50:45 GMT
ADD file:72743cfd9913f13553e700f9d9cfdc17b9dc793ebeeb337fd5fe02dc962d4b63 in / 
# Wed, 24 Feb 2021 20:50:46 GMT
CMD ["/bin/sh"]
# Wed, 24 Feb 2021 23:33:31 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 24 Feb 2021 23:33:52 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/traefik/traefik/releases/download/v1.7.28/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Wed, 24 Feb 2021 23:33:53 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 24 Feb 2021 23:33:54 GMT
EXPOSE 80
# Wed, 24 Feb 2021 23:33:55 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 24 Feb 2021 23:33:57 GMT
CMD ["traefik"]
# Wed, 24 Feb 2021 23:33:59 GMT
LABEL org.opencontainers.image.vendor=traefik org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.28 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:10e3bc1a9288f315752811ab2f438cb080f27de72c30375566135a542c8e03a1`  
		Last Modified: Wed, 24 Feb 2021 20:51:26 GMT  
		Size: 2.6 MB (2621066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c95c78170691d118707d7ee1e0fde756aca169be42fe54416c614386b5d73e82`  
		Last Modified: Wed, 24 Feb 2021 23:35:10 GMT  
		Size: 677.0 KB (677008 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e7f44cfea47b86361203a25aa879b8217da817bae7fd6dded70220a2fdf0ad7`  
		Last Modified: Wed, 24 Feb 2021 23:35:57 GMT  
		Size: 19.8 MB (19768227 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8ae25bca5f8bb1dbf5672bf0cea027f288f0b2a7f7fd9df3f07c5e2bfb5e2bb`  
		Last Modified: Wed, 24 Feb 2021 23:35:41 GMT  
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
$ docker pull traefik@sha256:2fe12e2958a0324f0ec02d858e7475fc8962b85e59d4c43a1f1bfd8b87f1059d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:1.7.28-alpine` - linux; amd64

```console
$ docker pull traefik@sha256:71f17992f437d3bbde3be6510b559159426e0bf22ee16af4b4f388a6d1193aa8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **24.6 MB (24606120 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:90599305b6e12aa47a2e1f5231cff859c4e3f649a14063df98ff5ddcaa9264e8`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 24 Feb 2021 20:20:11 GMT
ADD file:7eeea546ecde7a036bf634c08719879d32c7ec6ae599708cd91dc1b830735223 in / 
# Wed, 24 Feb 2021 20:20:12 GMT
CMD ["/bin/sh"]
# Tue, 09 Mar 2021 01:32:30 GMT
RUN apk --no-cache add ca-certificates tzdata
# Tue, 09 Mar 2021 01:32:41 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/traefik/traefik/releases/download/v1.7.28/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Tue, 09 Mar 2021 01:32:41 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Tue, 09 Mar 2021 01:32:41 GMT
EXPOSE 80
# Tue, 09 Mar 2021 01:32:42 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 09 Mar 2021 01:32:42 GMT
CMD ["traefik"]
# Tue, 09 Mar 2021 01:32:42 GMT
LABEL org.opencontainers.image.vendor=traefik org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.28 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:e95f33c60a645d6d31f52fdc334aecec0d79a1b410789eae37fbf69efcd587ab`  
		Last Modified: Wed, 24 Feb 2021 20:20:43 GMT  
		Size: 2.8 MB (2815313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e824fcc855ce466fcd783344fbc46e46eb8f786d642a60d7b75aecc31c0396d`  
		Last Modified: Tue, 09 Mar 2021 01:33:13 GMT  
		Size: 674.2 KB (674166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d0a7f1c496515ee0f8f5dc274c699158012873705bcfb5d3527832885b8dd05`  
		Last Modified: Tue, 09 Mar 2021 01:33:41 GMT  
		Size: 21.1 MB (21116273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5952bd804d03e773a53210515aaf4c07475739f157d0a13d352f34cfb1b9131d`  
		Last Modified: Tue, 09 Mar 2021 01:33:38 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:1.7.28-alpine` - linux; arm variant v6

```console
$ docker pull traefik@sha256:f3ab2c547fbc76d59301ed2f0464b796b57b4f5373ab9dfef877a1bc58464bbd
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.1 MB (23066669 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c7ff9159190f81182f781e4191b0558c229fb328121a58e6e9254409ddf3fae4`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 24 Feb 2021 20:50:45 GMT
ADD file:72743cfd9913f13553e700f9d9cfdc17b9dc793ebeeb337fd5fe02dc962d4b63 in / 
# Wed, 24 Feb 2021 20:50:46 GMT
CMD ["/bin/sh"]
# Wed, 24 Feb 2021 23:33:31 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 24 Feb 2021 23:33:52 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/traefik/traefik/releases/download/v1.7.28/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Wed, 24 Feb 2021 23:33:53 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 24 Feb 2021 23:33:54 GMT
EXPOSE 80
# Wed, 24 Feb 2021 23:33:55 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 24 Feb 2021 23:33:57 GMT
CMD ["traefik"]
# Wed, 24 Feb 2021 23:33:59 GMT
LABEL org.opencontainers.image.vendor=traefik org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.28 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:10e3bc1a9288f315752811ab2f438cb080f27de72c30375566135a542c8e03a1`  
		Last Modified: Wed, 24 Feb 2021 20:51:26 GMT  
		Size: 2.6 MB (2621066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c95c78170691d118707d7ee1e0fde756aca169be42fe54416c614386b5d73e82`  
		Last Modified: Wed, 24 Feb 2021 23:35:10 GMT  
		Size: 677.0 KB (677008 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e7f44cfea47b86361203a25aa879b8217da817bae7fd6dded70220a2fdf0ad7`  
		Last Modified: Wed, 24 Feb 2021 23:35:57 GMT  
		Size: 19.8 MB (19768227 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8ae25bca5f8bb1dbf5672bf0cea027f288f0b2a7f7fd9df3f07c5e2bfb5e2bb`  
		Last Modified: Wed, 24 Feb 2021 23:35:41 GMT  
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
$ docker pull traefik@sha256:b0e4c5d21dfd58478272d81fdb3ee4f032b738fe24260aeeb4fdb8c30168724f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:2.4` - linux; amd64

```console
$ docker pull traefik@sha256:f77782c1c613d08aabe67413e2ab34a20d18a424779be6802868eb90d7c1b2eb
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.8 MB (27827359 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2f3ef29ff3457efbc81bd711e18c29898902f608c21fc21928d43640aa00d74a`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 24 Feb 2021 20:20:11 GMT
ADD file:7eeea546ecde7a036bf634c08719879d32c7ec6ae599708cd91dc1b830735223 in / 
# Wed, 24 Feb 2021 20:20:12 GMT
CMD ["/bin/sh"]
# Tue, 09 Mar 2021 01:32:30 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 24 Mar 2021 01:39:31 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.4.8/traefik_v2.4.8_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Wed, 24 Mar 2021 01:39:31 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 24 Mar 2021 01:39:31 GMT
EXPOSE 80
# Wed, 24 Mar 2021 01:39:31 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 24 Mar 2021 01:39:31 GMT
CMD ["traefik"]
# Wed, 24 Mar 2021 01:39:32 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.4.8 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:e95f33c60a645d6d31f52fdc334aecec0d79a1b410789eae37fbf69efcd587ab`  
		Last Modified: Wed, 24 Feb 2021 20:20:43 GMT  
		Size: 2.8 MB (2815313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e824fcc855ce466fcd783344fbc46e46eb8f786d642a60d7b75aecc31c0396d`  
		Last Modified: Tue, 09 Mar 2021 01:33:13 GMT  
		Size: 674.2 KB (674166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d517a5c81aa99d6c7b3f5ba63d79cf9b29dcad97262ecace92ed87a033b9d3f3`  
		Last Modified: Wed, 24 Mar 2021 01:40:03 GMT  
		Size: 24.3 MB (24337512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc6216d750eb51a362ec1238b390c1d4f3d67fe760d7519b18cc734241057d6b`  
		Last Modified: Wed, 24 Mar 2021 01:39:58 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:2.4` - linux; arm variant v6

```console
$ docker pull traefik@sha256:36bdc8b0f979eec6df4e0e48a10cb03d06122760428cae889dd33185b7eaa50b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.0 MB (26025549 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:924cde150cf56c858ae139d9eb5aec198367c7ff2391b6f51e17c2039914fa8c`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 24 Feb 2021 20:50:45 GMT
ADD file:72743cfd9913f13553e700f9d9cfdc17b9dc793ebeeb337fd5fe02dc962d4b63 in / 
# Wed, 24 Feb 2021 20:50:46 GMT
CMD ["/bin/sh"]
# Wed, 24 Feb 2021 23:33:31 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 24 Mar 2021 02:29:20 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.4.8/traefik_v2.4.8_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Wed, 24 Mar 2021 02:29:21 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 24 Mar 2021 02:29:22 GMT
EXPOSE 80
# Wed, 24 Mar 2021 02:29:22 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 24 Mar 2021 02:29:23 GMT
CMD ["traefik"]
# Wed, 24 Mar 2021 02:29:24 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.4.8 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:10e3bc1a9288f315752811ab2f438cb080f27de72c30375566135a542c8e03a1`  
		Last Modified: Wed, 24 Feb 2021 20:51:26 GMT  
		Size: 2.6 MB (2621066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c95c78170691d118707d7ee1e0fde756aca169be42fe54416c614386b5d73e82`  
		Last Modified: Wed, 24 Feb 2021 23:35:10 GMT  
		Size: 677.0 KB (677008 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0fdec5ae7c7320d5327a0bdac6ecc6a94a3f358a45742c63f49bffe7da6cfb2`  
		Last Modified: Wed, 24 Mar 2021 02:30:02 GMT  
		Size: 22.7 MB (22727107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fa947f44a6dc4bfa180888f202ded6f0dba5e77a1967e6c9c30244091b2b338`  
		Last Modified: Wed, 24 Mar 2021 02:29:53 GMT  
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
$ docker pull traefik@sha256:b0e4c5d21dfd58478272d81fdb3ee4f032b738fe24260aeeb4fdb8c30168724f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:2.4.8` - linux; amd64

```console
$ docker pull traefik@sha256:f77782c1c613d08aabe67413e2ab34a20d18a424779be6802868eb90d7c1b2eb
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.8 MB (27827359 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2f3ef29ff3457efbc81bd711e18c29898902f608c21fc21928d43640aa00d74a`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 24 Feb 2021 20:20:11 GMT
ADD file:7eeea546ecde7a036bf634c08719879d32c7ec6ae599708cd91dc1b830735223 in / 
# Wed, 24 Feb 2021 20:20:12 GMT
CMD ["/bin/sh"]
# Tue, 09 Mar 2021 01:32:30 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 24 Mar 2021 01:39:31 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.4.8/traefik_v2.4.8_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Wed, 24 Mar 2021 01:39:31 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 24 Mar 2021 01:39:31 GMT
EXPOSE 80
# Wed, 24 Mar 2021 01:39:31 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 24 Mar 2021 01:39:31 GMT
CMD ["traefik"]
# Wed, 24 Mar 2021 01:39:32 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.4.8 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:e95f33c60a645d6d31f52fdc334aecec0d79a1b410789eae37fbf69efcd587ab`  
		Last Modified: Wed, 24 Feb 2021 20:20:43 GMT  
		Size: 2.8 MB (2815313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e824fcc855ce466fcd783344fbc46e46eb8f786d642a60d7b75aecc31c0396d`  
		Last Modified: Tue, 09 Mar 2021 01:33:13 GMT  
		Size: 674.2 KB (674166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d517a5c81aa99d6c7b3f5ba63d79cf9b29dcad97262ecace92ed87a033b9d3f3`  
		Last Modified: Wed, 24 Mar 2021 01:40:03 GMT  
		Size: 24.3 MB (24337512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc6216d750eb51a362ec1238b390c1d4f3d67fe760d7519b18cc734241057d6b`  
		Last Modified: Wed, 24 Mar 2021 01:39:58 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:2.4.8` - linux; arm variant v6

```console
$ docker pull traefik@sha256:36bdc8b0f979eec6df4e0e48a10cb03d06122760428cae889dd33185b7eaa50b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.0 MB (26025549 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:924cde150cf56c858ae139d9eb5aec198367c7ff2391b6f51e17c2039914fa8c`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 24 Feb 2021 20:50:45 GMT
ADD file:72743cfd9913f13553e700f9d9cfdc17b9dc793ebeeb337fd5fe02dc962d4b63 in / 
# Wed, 24 Feb 2021 20:50:46 GMT
CMD ["/bin/sh"]
# Wed, 24 Feb 2021 23:33:31 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 24 Mar 2021 02:29:20 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.4.8/traefik_v2.4.8_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Wed, 24 Mar 2021 02:29:21 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 24 Mar 2021 02:29:22 GMT
EXPOSE 80
# Wed, 24 Mar 2021 02:29:22 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 24 Mar 2021 02:29:23 GMT
CMD ["traefik"]
# Wed, 24 Mar 2021 02:29:24 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.4.8 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:10e3bc1a9288f315752811ab2f438cb080f27de72c30375566135a542c8e03a1`  
		Last Modified: Wed, 24 Feb 2021 20:51:26 GMT  
		Size: 2.6 MB (2621066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c95c78170691d118707d7ee1e0fde756aca169be42fe54416c614386b5d73e82`  
		Last Modified: Wed, 24 Feb 2021 23:35:10 GMT  
		Size: 677.0 KB (677008 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0fdec5ae7c7320d5327a0bdac6ecc6a94a3f358a45742c63f49bffe7da6cfb2`  
		Last Modified: Wed, 24 Mar 2021 02:30:02 GMT  
		Size: 22.7 MB (22727107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fa947f44a6dc4bfa180888f202ded6f0dba5e77a1967e6c9c30244091b2b338`  
		Last Modified: Wed, 24 Mar 2021 02:29:53 GMT  
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
$ docker pull traefik@sha256:b0e4c5d21dfd58478272d81fdb3ee4f032b738fe24260aeeb4fdb8c30168724f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:latest` - linux; amd64

```console
$ docker pull traefik@sha256:f77782c1c613d08aabe67413e2ab34a20d18a424779be6802868eb90d7c1b2eb
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.8 MB (27827359 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2f3ef29ff3457efbc81bd711e18c29898902f608c21fc21928d43640aa00d74a`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 24 Feb 2021 20:20:11 GMT
ADD file:7eeea546ecde7a036bf634c08719879d32c7ec6ae599708cd91dc1b830735223 in / 
# Wed, 24 Feb 2021 20:20:12 GMT
CMD ["/bin/sh"]
# Tue, 09 Mar 2021 01:32:30 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 24 Mar 2021 01:39:31 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.4.8/traefik_v2.4.8_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Wed, 24 Mar 2021 01:39:31 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 24 Mar 2021 01:39:31 GMT
EXPOSE 80
# Wed, 24 Mar 2021 01:39:31 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 24 Mar 2021 01:39:31 GMT
CMD ["traefik"]
# Wed, 24 Mar 2021 01:39:32 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.4.8 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:e95f33c60a645d6d31f52fdc334aecec0d79a1b410789eae37fbf69efcd587ab`  
		Last Modified: Wed, 24 Feb 2021 20:20:43 GMT  
		Size: 2.8 MB (2815313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e824fcc855ce466fcd783344fbc46e46eb8f786d642a60d7b75aecc31c0396d`  
		Last Modified: Tue, 09 Mar 2021 01:33:13 GMT  
		Size: 674.2 KB (674166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d517a5c81aa99d6c7b3f5ba63d79cf9b29dcad97262ecace92ed87a033b9d3f3`  
		Last Modified: Wed, 24 Mar 2021 01:40:03 GMT  
		Size: 24.3 MB (24337512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc6216d750eb51a362ec1238b390c1d4f3d67fe760d7519b18cc734241057d6b`  
		Last Modified: Wed, 24 Mar 2021 01:39:58 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:latest` - linux; arm variant v6

```console
$ docker pull traefik@sha256:36bdc8b0f979eec6df4e0e48a10cb03d06122760428cae889dd33185b7eaa50b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.0 MB (26025549 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:924cde150cf56c858ae139d9eb5aec198367c7ff2391b6f51e17c2039914fa8c`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 24 Feb 2021 20:50:45 GMT
ADD file:72743cfd9913f13553e700f9d9cfdc17b9dc793ebeeb337fd5fe02dc962d4b63 in / 
# Wed, 24 Feb 2021 20:50:46 GMT
CMD ["/bin/sh"]
# Wed, 24 Feb 2021 23:33:31 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 24 Mar 2021 02:29:20 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.4.8/traefik_v2.4.8_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Wed, 24 Mar 2021 02:29:21 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 24 Mar 2021 02:29:22 GMT
EXPOSE 80
# Wed, 24 Mar 2021 02:29:22 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 24 Mar 2021 02:29:23 GMT
CMD ["traefik"]
# Wed, 24 Mar 2021 02:29:24 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.4.8 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:10e3bc1a9288f315752811ab2f438cb080f27de72c30375566135a542c8e03a1`  
		Last Modified: Wed, 24 Feb 2021 20:51:26 GMT  
		Size: 2.6 MB (2621066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c95c78170691d118707d7ee1e0fde756aca169be42fe54416c614386b5d73e82`  
		Last Modified: Wed, 24 Feb 2021 23:35:10 GMT  
		Size: 677.0 KB (677008 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0fdec5ae7c7320d5327a0bdac6ecc6a94a3f358a45742c63f49bffe7da6cfb2`  
		Last Modified: Wed, 24 Mar 2021 02:30:02 GMT  
		Size: 22.7 MB (22727107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fa947f44a6dc4bfa180888f202ded6f0dba5e77a1967e6c9c30244091b2b338`  
		Last Modified: Wed, 24 Mar 2021 02:29:53 GMT  
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
$ docker pull traefik@sha256:b0e4c5d21dfd58478272d81fdb3ee4f032b738fe24260aeeb4fdb8c30168724f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:livarot` - linux; amd64

```console
$ docker pull traefik@sha256:f77782c1c613d08aabe67413e2ab34a20d18a424779be6802868eb90d7c1b2eb
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.8 MB (27827359 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2f3ef29ff3457efbc81bd711e18c29898902f608c21fc21928d43640aa00d74a`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 24 Feb 2021 20:20:11 GMT
ADD file:7eeea546ecde7a036bf634c08719879d32c7ec6ae599708cd91dc1b830735223 in / 
# Wed, 24 Feb 2021 20:20:12 GMT
CMD ["/bin/sh"]
# Tue, 09 Mar 2021 01:32:30 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 24 Mar 2021 01:39:31 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.4.8/traefik_v2.4.8_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Wed, 24 Mar 2021 01:39:31 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 24 Mar 2021 01:39:31 GMT
EXPOSE 80
# Wed, 24 Mar 2021 01:39:31 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 24 Mar 2021 01:39:31 GMT
CMD ["traefik"]
# Wed, 24 Mar 2021 01:39:32 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.4.8 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:e95f33c60a645d6d31f52fdc334aecec0d79a1b410789eae37fbf69efcd587ab`  
		Last Modified: Wed, 24 Feb 2021 20:20:43 GMT  
		Size: 2.8 MB (2815313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e824fcc855ce466fcd783344fbc46e46eb8f786d642a60d7b75aecc31c0396d`  
		Last Modified: Tue, 09 Mar 2021 01:33:13 GMT  
		Size: 674.2 KB (674166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d517a5c81aa99d6c7b3f5ba63d79cf9b29dcad97262ecace92ed87a033b9d3f3`  
		Last Modified: Wed, 24 Mar 2021 01:40:03 GMT  
		Size: 24.3 MB (24337512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc6216d750eb51a362ec1238b390c1d4f3d67fe760d7519b18cc734241057d6b`  
		Last Modified: Wed, 24 Mar 2021 01:39:58 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:livarot` - linux; arm variant v6

```console
$ docker pull traefik@sha256:36bdc8b0f979eec6df4e0e48a10cb03d06122760428cae889dd33185b7eaa50b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.0 MB (26025549 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:924cde150cf56c858ae139d9eb5aec198367c7ff2391b6f51e17c2039914fa8c`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 24 Feb 2021 20:50:45 GMT
ADD file:72743cfd9913f13553e700f9d9cfdc17b9dc793ebeeb337fd5fe02dc962d4b63 in / 
# Wed, 24 Feb 2021 20:50:46 GMT
CMD ["/bin/sh"]
# Wed, 24 Feb 2021 23:33:31 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 24 Mar 2021 02:29:20 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.4.8/traefik_v2.4.8_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Wed, 24 Mar 2021 02:29:21 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 24 Mar 2021 02:29:22 GMT
EXPOSE 80
# Wed, 24 Mar 2021 02:29:22 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 24 Mar 2021 02:29:23 GMT
CMD ["traefik"]
# Wed, 24 Mar 2021 02:29:24 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.4.8 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:10e3bc1a9288f315752811ab2f438cb080f27de72c30375566135a542c8e03a1`  
		Last Modified: Wed, 24 Feb 2021 20:51:26 GMT  
		Size: 2.6 MB (2621066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c95c78170691d118707d7ee1e0fde756aca169be42fe54416c614386b5d73e82`  
		Last Modified: Wed, 24 Feb 2021 23:35:10 GMT  
		Size: 677.0 KB (677008 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0fdec5ae7c7320d5327a0bdac6ecc6a94a3f358a45742c63f49bffe7da6cfb2`  
		Last Modified: Wed, 24 Mar 2021 02:30:02 GMT  
		Size: 22.7 MB (22727107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fa947f44a6dc4bfa180888f202ded6f0dba5e77a1967e6c9c30244091b2b338`  
		Last Modified: Wed, 24 Mar 2021 02:29:53 GMT  
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
$ docker pull traefik@sha256:2fe12e2958a0324f0ec02d858e7475fc8962b85e59d4c43a1f1bfd8b87f1059d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:maroilles-alpine` - linux; amd64

```console
$ docker pull traefik@sha256:71f17992f437d3bbde3be6510b559159426e0bf22ee16af4b4f388a6d1193aa8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **24.6 MB (24606120 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:90599305b6e12aa47a2e1f5231cff859c4e3f649a14063df98ff5ddcaa9264e8`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 24 Feb 2021 20:20:11 GMT
ADD file:7eeea546ecde7a036bf634c08719879d32c7ec6ae599708cd91dc1b830735223 in / 
# Wed, 24 Feb 2021 20:20:12 GMT
CMD ["/bin/sh"]
# Tue, 09 Mar 2021 01:32:30 GMT
RUN apk --no-cache add ca-certificates tzdata
# Tue, 09 Mar 2021 01:32:41 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/traefik/traefik/releases/download/v1.7.28/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Tue, 09 Mar 2021 01:32:41 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Tue, 09 Mar 2021 01:32:41 GMT
EXPOSE 80
# Tue, 09 Mar 2021 01:32:42 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 09 Mar 2021 01:32:42 GMT
CMD ["traefik"]
# Tue, 09 Mar 2021 01:32:42 GMT
LABEL org.opencontainers.image.vendor=traefik org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.28 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:e95f33c60a645d6d31f52fdc334aecec0d79a1b410789eae37fbf69efcd587ab`  
		Last Modified: Wed, 24 Feb 2021 20:20:43 GMT  
		Size: 2.8 MB (2815313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e824fcc855ce466fcd783344fbc46e46eb8f786d642a60d7b75aecc31c0396d`  
		Last Modified: Tue, 09 Mar 2021 01:33:13 GMT  
		Size: 674.2 KB (674166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d0a7f1c496515ee0f8f5dc274c699158012873705bcfb5d3527832885b8dd05`  
		Last Modified: Tue, 09 Mar 2021 01:33:41 GMT  
		Size: 21.1 MB (21116273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5952bd804d03e773a53210515aaf4c07475739f157d0a13d352f34cfb1b9131d`  
		Last Modified: Tue, 09 Mar 2021 01:33:38 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:maroilles-alpine` - linux; arm variant v6

```console
$ docker pull traefik@sha256:f3ab2c547fbc76d59301ed2f0464b796b57b4f5373ab9dfef877a1bc58464bbd
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.1 MB (23066669 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c7ff9159190f81182f781e4191b0558c229fb328121a58e6e9254409ddf3fae4`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 24 Feb 2021 20:50:45 GMT
ADD file:72743cfd9913f13553e700f9d9cfdc17b9dc793ebeeb337fd5fe02dc962d4b63 in / 
# Wed, 24 Feb 2021 20:50:46 GMT
CMD ["/bin/sh"]
# Wed, 24 Feb 2021 23:33:31 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 24 Feb 2021 23:33:52 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/traefik/traefik/releases/download/v1.7.28/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Wed, 24 Feb 2021 23:33:53 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 24 Feb 2021 23:33:54 GMT
EXPOSE 80
# Wed, 24 Feb 2021 23:33:55 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 24 Feb 2021 23:33:57 GMT
CMD ["traefik"]
# Wed, 24 Feb 2021 23:33:59 GMT
LABEL org.opencontainers.image.vendor=traefik org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.28 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:10e3bc1a9288f315752811ab2f438cb080f27de72c30375566135a542c8e03a1`  
		Last Modified: Wed, 24 Feb 2021 20:51:26 GMT  
		Size: 2.6 MB (2621066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c95c78170691d118707d7ee1e0fde756aca169be42fe54416c614386b5d73e82`  
		Last Modified: Wed, 24 Feb 2021 23:35:10 GMT  
		Size: 677.0 KB (677008 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e7f44cfea47b86361203a25aa879b8217da817bae7fd6dded70220a2fdf0ad7`  
		Last Modified: Wed, 24 Feb 2021 23:35:57 GMT  
		Size: 19.8 MB (19768227 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8ae25bca5f8bb1dbf5672bf0cea027f288f0b2a7f7fd9df3f07c5e2bfb5e2bb`  
		Last Modified: Wed, 24 Feb 2021 23:35:41 GMT  
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
$ docker pull traefik@sha256:2fe12e2958a0324f0ec02d858e7475fc8962b85e59d4c43a1f1bfd8b87f1059d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:v1.7-alpine` - linux; amd64

```console
$ docker pull traefik@sha256:71f17992f437d3bbde3be6510b559159426e0bf22ee16af4b4f388a6d1193aa8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **24.6 MB (24606120 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:90599305b6e12aa47a2e1f5231cff859c4e3f649a14063df98ff5ddcaa9264e8`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 24 Feb 2021 20:20:11 GMT
ADD file:7eeea546ecde7a036bf634c08719879d32c7ec6ae599708cd91dc1b830735223 in / 
# Wed, 24 Feb 2021 20:20:12 GMT
CMD ["/bin/sh"]
# Tue, 09 Mar 2021 01:32:30 GMT
RUN apk --no-cache add ca-certificates tzdata
# Tue, 09 Mar 2021 01:32:41 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/traefik/traefik/releases/download/v1.7.28/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Tue, 09 Mar 2021 01:32:41 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Tue, 09 Mar 2021 01:32:41 GMT
EXPOSE 80
# Tue, 09 Mar 2021 01:32:42 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 09 Mar 2021 01:32:42 GMT
CMD ["traefik"]
# Tue, 09 Mar 2021 01:32:42 GMT
LABEL org.opencontainers.image.vendor=traefik org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.28 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:e95f33c60a645d6d31f52fdc334aecec0d79a1b410789eae37fbf69efcd587ab`  
		Last Modified: Wed, 24 Feb 2021 20:20:43 GMT  
		Size: 2.8 MB (2815313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e824fcc855ce466fcd783344fbc46e46eb8f786d642a60d7b75aecc31c0396d`  
		Last Modified: Tue, 09 Mar 2021 01:33:13 GMT  
		Size: 674.2 KB (674166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d0a7f1c496515ee0f8f5dc274c699158012873705bcfb5d3527832885b8dd05`  
		Last Modified: Tue, 09 Mar 2021 01:33:41 GMT  
		Size: 21.1 MB (21116273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5952bd804d03e773a53210515aaf4c07475739f157d0a13d352f34cfb1b9131d`  
		Last Modified: Tue, 09 Mar 2021 01:33:38 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v1.7-alpine` - linux; arm variant v6

```console
$ docker pull traefik@sha256:f3ab2c547fbc76d59301ed2f0464b796b57b4f5373ab9dfef877a1bc58464bbd
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.1 MB (23066669 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c7ff9159190f81182f781e4191b0558c229fb328121a58e6e9254409ddf3fae4`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 24 Feb 2021 20:50:45 GMT
ADD file:72743cfd9913f13553e700f9d9cfdc17b9dc793ebeeb337fd5fe02dc962d4b63 in / 
# Wed, 24 Feb 2021 20:50:46 GMT
CMD ["/bin/sh"]
# Wed, 24 Feb 2021 23:33:31 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 24 Feb 2021 23:33:52 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/traefik/traefik/releases/download/v1.7.28/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Wed, 24 Feb 2021 23:33:53 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 24 Feb 2021 23:33:54 GMT
EXPOSE 80
# Wed, 24 Feb 2021 23:33:55 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 24 Feb 2021 23:33:57 GMT
CMD ["traefik"]
# Wed, 24 Feb 2021 23:33:59 GMT
LABEL org.opencontainers.image.vendor=traefik org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.28 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:10e3bc1a9288f315752811ab2f438cb080f27de72c30375566135a542c8e03a1`  
		Last Modified: Wed, 24 Feb 2021 20:51:26 GMT  
		Size: 2.6 MB (2621066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c95c78170691d118707d7ee1e0fde756aca169be42fe54416c614386b5d73e82`  
		Last Modified: Wed, 24 Feb 2021 23:35:10 GMT  
		Size: 677.0 KB (677008 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e7f44cfea47b86361203a25aa879b8217da817bae7fd6dded70220a2fdf0ad7`  
		Last Modified: Wed, 24 Feb 2021 23:35:57 GMT  
		Size: 19.8 MB (19768227 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8ae25bca5f8bb1dbf5672bf0cea027f288f0b2a7f7fd9df3f07c5e2bfb5e2bb`  
		Last Modified: Wed, 24 Feb 2021 23:35:41 GMT  
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
$ docker pull traefik@sha256:2fe12e2958a0324f0ec02d858e7475fc8962b85e59d4c43a1f1bfd8b87f1059d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:v1.7.28-alpine` - linux; amd64

```console
$ docker pull traefik@sha256:71f17992f437d3bbde3be6510b559159426e0bf22ee16af4b4f388a6d1193aa8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **24.6 MB (24606120 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:90599305b6e12aa47a2e1f5231cff859c4e3f649a14063df98ff5ddcaa9264e8`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 24 Feb 2021 20:20:11 GMT
ADD file:7eeea546ecde7a036bf634c08719879d32c7ec6ae599708cd91dc1b830735223 in / 
# Wed, 24 Feb 2021 20:20:12 GMT
CMD ["/bin/sh"]
# Tue, 09 Mar 2021 01:32:30 GMT
RUN apk --no-cache add ca-certificates tzdata
# Tue, 09 Mar 2021 01:32:41 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/traefik/traefik/releases/download/v1.7.28/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Tue, 09 Mar 2021 01:32:41 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Tue, 09 Mar 2021 01:32:41 GMT
EXPOSE 80
# Tue, 09 Mar 2021 01:32:42 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 09 Mar 2021 01:32:42 GMT
CMD ["traefik"]
# Tue, 09 Mar 2021 01:32:42 GMT
LABEL org.opencontainers.image.vendor=traefik org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.28 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:e95f33c60a645d6d31f52fdc334aecec0d79a1b410789eae37fbf69efcd587ab`  
		Last Modified: Wed, 24 Feb 2021 20:20:43 GMT  
		Size: 2.8 MB (2815313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e824fcc855ce466fcd783344fbc46e46eb8f786d642a60d7b75aecc31c0396d`  
		Last Modified: Tue, 09 Mar 2021 01:33:13 GMT  
		Size: 674.2 KB (674166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d0a7f1c496515ee0f8f5dc274c699158012873705bcfb5d3527832885b8dd05`  
		Last Modified: Tue, 09 Mar 2021 01:33:41 GMT  
		Size: 21.1 MB (21116273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5952bd804d03e773a53210515aaf4c07475739f157d0a13d352f34cfb1b9131d`  
		Last Modified: Tue, 09 Mar 2021 01:33:38 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v1.7.28-alpine` - linux; arm variant v6

```console
$ docker pull traefik@sha256:f3ab2c547fbc76d59301ed2f0464b796b57b4f5373ab9dfef877a1bc58464bbd
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.1 MB (23066669 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c7ff9159190f81182f781e4191b0558c229fb328121a58e6e9254409ddf3fae4`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 24 Feb 2021 20:50:45 GMT
ADD file:72743cfd9913f13553e700f9d9cfdc17b9dc793ebeeb337fd5fe02dc962d4b63 in / 
# Wed, 24 Feb 2021 20:50:46 GMT
CMD ["/bin/sh"]
# Wed, 24 Feb 2021 23:33:31 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 24 Feb 2021 23:33:52 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/traefik/traefik/releases/download/v1.7.28/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Wed, 24 Feb 2021 23:33:53 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 24 Feb 2021 23:33:54 GMT
EXPOSE 80
# Wed, 24 Feb 2021 23:33:55 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 24 Feb 2021 23:33:57 GMT
CMD ["traefik"]
# Wed, 24 Feb 2021 23:33:59 GMT
LABEL org.opencontainers.image.vendor=traefik org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.28 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:10e3bc1a9288f315752811ab2f438cb080f27de72c30375566135a542c8e03a1`  
		Last Modified: Wed, 24 Feb 2021 20:51:26 GMT  
		Size: 2.6 MB (2621066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c95c78170691d118707d7ee1e0fde756aca169be42fe54416c614386b5d73e82`  
		Last Modified: Wed, 24 Feb 2021 23:35:10 GMT  
		Size: 677.0 KB (677008 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e7f44cfea47b86361203a25aa879b8217da817bae7fd6dded70220a2fdf0ad7`  
		Last Modified: Wed, 24 Feb 2021 23:35:57 GMT  
		Size: 19.8 MB (19768227 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8ae25bca5f8bb1dbf5672bf0cea027f288f0b2a7f7fd9df3f07c5e2bfb5e2bb`  
		Last Modified: Wed, 24 Feb 2021 23:35:41 GMT  
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
$ docker pull traefik@sha256:b0e4c5d21dfd58478272d81fdb3ee4f032b738fe24260aeeb4fdb8c30168724f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:v2.4` - linux; amd64

```console
$ docker pull traefik@sha256:f77782c1c613d08aabe67413e2ab34a20d18a424779be6802868eb90d7c1b2eb
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.8 MB (27827359 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2f3ef29ff3457efbc81bd711e18c29898902f608c21fc21928d43640aa00d74a`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 24 Feb 2021 20:20:11 GMT
ADD file:7eeea546ecde7a036bf634c08719879d32c7ec6ae599708cd91dc1b830735223 in / 
# Wed, 24 Feb 2021 20:20:12 GMT
CMD ["/bin/sh"]
# Tue, 09 Mar 2021 01:32:30 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 24 Mar 2021 01:39:31 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.4.8/traefik_v2.4.8_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Wed, 24 Mar 2021 01:39:31 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 24 Mar 2021 01:39:31 GMT
EXPOSE 80
# Wed, 24 Mar 2021 01:39:31 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 24 Mar 2021 01:39:31 GMT
CMD ["traefik"]
# Wed, 24 Mar 2021 01:39:32 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.4.8 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:e95f33c60a645d6d31f52fdc334aecec0d79a1b410789eae37fbf69efcd587ab`  
		Last Modified: Wed, 24 Feb 2021 20:20:43 GMT  
		Size: 2.8 MB (2815313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e824fcc855ce466fcd783344fbc46e46eb8f786d642a60d7b75aecc31c0396d`  
		Last Modified: Tue, 09 Mar 2021 01:33:13 GMT  
		Size: 674.2 KB (674166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d517a5c81aa99d6c7b3f5ba63d79cf9b29dcad97262ecace92ed87a033b9d3f3`  
		Last Modified: Wed, 24 Mar 2021 01:40:03 GMT  
		Size: 24.3 MB (24337512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc6216d750eb51a362ec1238b390c1d4f3d67fe760d7519b18cc734241057d6b`  
		Last Modified: Wed, 24 Mar 2021 01:39:58 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v2.4` - linux; arm variant v6

```console
$ docker pull traefik@sha256:36bdc8b0f979eec6df4e0e48a10cb03d06122760428cae889dd33185b7eaa50b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.0 MB (26025549 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:924cde150cf56c858ae139d9eb5aec198367c7ff2391b6f51e17c2039914fa8c`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 24 Feb 2021 20:50:45 GMT
ADD file:72743cfd9913f13553e700f9d9cfdc17b9dc793ebeeb337fd5fe02dc962d4b63 in / 
# Wed, 24 Feb 2021 20:50:46 GMT
CMD ["/bin/sh"]
# Wed, 24 Feb 2021 23:33:31 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 24 Mar 2021 02:29:20 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.4.8/traefik_v2.4.8_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Wed, 24 Mar 2021 02:29:21 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 24 Mar 2021 02:29:22 GMT
EXPOSE 80
# Wed, 24 Mar 2021 02:29:22 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 24 Mar 2021 02:29:23 GMT
CMD ["traefik"]
# Wed, 24 Mar 2021 02:29:24 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.4.8 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:10e3bc1a9288f315752811ab2f438cb080f27de72c30375566135a542c8e03a1`  
		Last Modified: Wed, 24 Feb 2021 20:51:26 GMT  
		Size: 2.6 MB (2621066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c95c78170691d118707d7ee1e0fde756aca169be42fe54416c614386b5d73e82`  
		Last Modified: Wed, 24 Feb 2021 23:35:10 GMT  
		Size: 677.0 KB (677008 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0fdec5ae7c7320d5327a0bdac6ecc6a94a3f358a45742c63f49bffe7da6cfb2`  
		Last Modified: Wed, 24 Mar 2021 02:30:02 GMT  
		Size: 22.7 MB (22727107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fa947f44a6dc4bfa180888f202ded6f0dba5e77a1967e6c9c30244091b2b338`  
		Last Modified: Wed, 24 Mar 2021 02:29:53 GMT  
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
$ docker pull traefik@sha256:b0e4c5d21dfd58478272d81fdb3ee4f032b738fe24260aeeb4fdb8c30168724f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:v2.4.8` - linux; amd64

```console
$ docker pull traefik@sha256:f77782c1c613d08aabe67413e2ab34a20d18a424779be6802868eb90d7c1b2eb
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.8 MB (27827359 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2f3ef29ff3457efbc81bd711e18c29898902f608c21fc21928d43640aa00d74a`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 24 Feb 2021 20:20:11 GMT
ADD file:7eeea546ecde7a036bf634c08719879d32c7ec6ae599708cd91dc1b830735223 in / 
# Wed, 24 Feb 2021 20:20:12 GMT
CMD ["/bin/sh"]
# Tue, 09 Mar 2021 01:32:30 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 24 Mar 2021 01:39:31 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.4.8/traefik_v2.4.8_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Wed, 24 Mar 2021 01:39:31 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 24 Mar 2021 01:39:31 GMT
EXPOSE 80
# Wed, 24 Mar 2021 01:39:31 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 24 Mar 2021 01:39:31 GMT
CMD ["traefik"]
# Wed, 24 Mar 2021 01:39:32 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.4.8 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:e95f33c60a645d6d31f52fdc334aecec0d79a1b410789eae37fbf69efcd587ab`  
		Last Modified: Wed, 24 Feb 2021 20:20:43 GMT  
		Size: 2.8 MB (2815313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e824fcc855ce466fcd783344fbc46e46eb8f786d642a60d7b75aecc31c0396d`  
		Last Modified: Tue, 09 Mar 2021 01:33:13 GMT  
		Size: 674.2 KB (674166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d517a5c81aa99d6c7b3f5ba63d79cf9b29dcad97262ecace92ed87a033b9d3f3`  
		Last Modified: Wed, 24 Mar 2021 01:40:03 GMT  
		Size: 24.3 MB (24337512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc6216d750eb51a362ec1238b390c1d4f3d67fe760d7519b18cc734241057d6b`  
		Last Modified: Wed, 24 Mar 2021 01:39:58 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v2.4.8` - linux; arm variant v6

```console
$ docker pull traefik@sha256:36bdc8b0f979eec6df4e0e48a10cb03d06122760428cae889dd33185b7eaa50b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.0 MB (26025549 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:924cde150cf56c858ae139d9eb5aec198367c7ff2391b6f51e17c2039914fa8c`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 24 Feb 2021 20:50:45 GMT
ADD file:72743cfd9913f13553e700f9d9cfdc17b9dc793ebeeb337fd5fe02dc962d4b63 in / 
# Wed, 24 Feb 2021 20:50:46 GMT
CMD ["/bin/sh"]
# Wed, 24 Feb 2021 23:33:31 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 24 Mar 2021 02:29:20 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.4.8/traefik_v2.4.8_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Wed, 24 Mar 2021 02:29:21 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 24 Mar 2021 02:29:22 GMT
EXPOSE 80
# Wed, 24 Mar 2021 02:29:22 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 24 Mar 2021 02:29:23 GMT
CMD ["traefik"]
# Wed, 24 Mar 2021 02:29:24 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.4.8 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:10e3bc1a9288f315752811ab2f438cb080f27de72c30375566135a542c8e03a1`  
		Last Modified: Wed, 24 Feb 2021 20:51:26 GMT  
		Size: 2.6 MB (2621066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c95c78170691d118707d7ee1e0fde756aca169be42fe54416c614386b5d73e82`  
		Last Modified: Wed, 24 Feb 2021 23:35:10 GMT  
		Size: 677.0 KB (677008 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0fdec5ae7c7320d5327a0bdac6ecc6a94a3f358a45742c63f49bffe7da6cfb2`  
		Last Modified: Wed, 24 Mar 2021 02:30:02 GMT  
		Size: 22.7 MB (22727107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fa947f44a6dc4bfa180888f202ded6f0dba5e77a1967e6c9c30244091b2b338`  
		Last Modified: Wed, 24 Mar 2021 02:29:53 GMT  
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
