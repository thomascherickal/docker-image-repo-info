<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `traefik`

-	[`traefik:1.7`](#traefik17)
-	[`traefik:1.7-alpine`](#traefik17-alpine)
-	[`traefik:1.7-windowsservercore-1809`](#traefik17-windowsservercore-1809)
-	[`traefik:1.7.34`](#traefik1734)
-	[`traefik:1.7.34-alpine`](#traefik1734-alpine)
-	[`traefik:1.7.34-windowsservercore-1809`](#traefik1734-windowsservercore-1809)
-	[`traefik:2.8`](#traefik28)
-	[`traefik:2.8-windowsservercore-1809`](#traefik28-windowsservercore-1809)
-	[`traefik:2.8.4`](#traefik284)
-	[`traefik:2.8.4-windowsservercore-1809`](#traefik284-windowsservercore-1809)
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
-	[`traefik:v2.8`](#traefikv28)
-	[`traefik:v2.8-windowsservercore-1809`](#traefikv28-windowsservercore-1809)
-	[`traefik:v2.8.4`](#traefikv284)
-	[`traefik:v2.8.4-windowsservercore-1809`](#traefikv284-windowsservercore-1809)
-	[`traefik:vacherin`](#traefikvacherin)
-	[`traefik:vacherin-windowsservercore-1809`](#traefikvacherin-windowsservercore-1809)
-	[`traefik:windowsservercore-1809`](#traefikwindowsservercore-1809)

## `traefik:1.7`

```console
$ docker pull traefik@sha256:bd12a7039c4736697cab4ee722d4f7683ee292b5b47b861a44a007a30c0581dd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:1.7` - linux; amd64

```console
$ docker pull traefik@sha256:221d4ca433d21b148f21168a3c71aeb10d776f7d9051fb612b10be1d703f9c36
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **22.6 MB (22614032 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fd7cc9150335f309f34597c684d908b517b7aa428c550fa8f63dd1a19bafbfe4`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Wed, 10 Aug 2022 01:25:18 GMT
COPY file:48964762d0c961c28f59ebd3ea194fb6486cf2bd9a9cf1780f6702d88bd7b7d9 in /etc/ssl/certs/ 
# Wed, 10 Aug 2022 01:25:19 GMT
COPY dir:a84372748b89eb90478bb1b120b7c8fff3112421d7f93e50fbeae3f53adc6788 in /usr/share/ 
# Wed, 10 Aug 2022 01:25:20 GMT
COPY file:36217e5a6056bef26cfff395c8af8c1010a61dbe8d62b2c7869ca221e2a6302c in / 
# Wed, 10 Aug 2022 01:25:20 GMT
EXPOSE 80
# Wed, 10 Aug 2022 01:25:20 GMT
VOLUME [/tmp]
# Wed, 10 Aug 2022 01:25:20 GMT
ENTRYPOINT ["/traefik"]
# Wed, 10 Aug 2022 01:25:20 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.34 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:dcf6dab73e17be4a506f9432554b84ca5af22b6ca8d3a28551e98fd1c05660dc`  
		Last Modified: Wed, 10 Aug 2022 01:26:26 GMT  
		Size: 123.5 KB (123538 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd04e95cb63652c8a3323efd5c36bdcf17166632bd5bbf9c5c72092392094ebb`  
		Last Modified: Wed, 10 Aug 2022 01:26:26 GMT  
		Size: 328.5 KB (328542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bc5ce073739868727c7f64505383cab253c15631bf675c2b65bb384d4ae4b1e`  
		Last Modified: Wed, 10 Aug 2022 01:26:30 GMT  
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
$ docker pull traefik@sha256:ee80ec61ce7968fa7680b289cc4e0cb29933f0d254c962f4ba94b87de29bbbe7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **20.6 MB (20583416 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:72b9e44203aa217fc68aff257b65b34390dec5720d4c89a2c3722476af10cdef`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Wed, 10 Aug 2022 06:11:29 GMT
COPY file:48964762d0c961c28f59ebd3ea194fb6486cf2bd9a9cf1780f6702d88bd7b7d9 in /etc/ssl/certs/ 
# Wed, 10 Aug 2022 06:11:30 GMT
COPY dir:a84372748b89eb90478bb1b120b7c8fff3112421d7f93e50fbeae3f53adc6788 in /usr/share/ 
# Wed, 10 Aug 2022 06:11:31 GMT
COPY file:60330593b6644f3f519fd13ce8ee34c2c7ab9994a1420afabbc01926dd1230dd in / 
# Wed, 10 Aug 2022 06:11:31 GMT
EXPOSE 80
# Wed, 10 Aug 2022 06:11:32 GMT
VOLUME [/tmp]
# Wed, 10 Aug 2022 06:11:33 GMT
ENTRYPOINT ["/traefik"]
# Wed, 10 Aug 2022 06:11:34 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.34 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:45ff194111b414e1aa5548434d84e56dbd11ebe2589d05ac6498a25d0e8adfcd`  
		Last Modified: Wed, 10 Aug 2022 06:13:02 GMT  
		Size: 123.5 KB (123544 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0a00cc3745cda02ead5281ab2de73712088f63bdf0bb2e31932d82d8d4c4236`  
		Last Modified: Wed, 10 Aug 2022 06:13:02 GMT  
		Size: 328.5 KB (328525 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c10648c89e22ebcc358eb0f5e84d1de66c1d49da6d460218007ffe19f65baafc`  
		Last Modified: Wed, 10 Aug 2022 06:13:05 GMT  
		Size: 20.1 MB (20131347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:1.7-alpine`

```console
$ docker pull traefik@sha256:a65ea31d38ab997c3ec977ca7e46192823ef829c298574e0365c1878f5e447f9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:1.7-alpine` - linux; amd64

```console
$ docker pull traefik@sha256:fa0b479bcd6943cf3eee0f076f096253cd87d60eedbd550c5c46093f8a272aae
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.7 MB (25670985 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d93d266ccb4853b50019238b20d45befbbb64114d2780ee6582d87058faf9269`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Tue, 09 Aug 2022 17:20:07 GMT
ADD file:b9bd10cf83356cb7281baa0fbaca5186cf27491f59eda87abe57f83a5aaf5ec1 in / 
# Tue, 09 Aug 2022 17:20:08 GMT
CMD ["/bin/sh"]
# Wed, 10 Aug 2022 01:25:03 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 10 Aug 2022 01:25:09 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/traefik/traefik/releases/download/v1.7.34/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Wed, 10 Aug 2022 01:25:09 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 10 Aug 2022 01:25:10 GMT
EXPOSE 80
# Wed, 10 Aug 2022 01:25:10 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 10 Aug 2022 01:25:10 GMT
CMD ["traefik"]
# Wed, 10 Aug 2022 01:25:10 GMT
LABEL org.opencontainers.image.vendor=traefik org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.34 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:c7ed990a2339ee598662849de4f56e2241399f5a32340c8c4a7bbd5378a12b5f`  
		Last Modified: Tue, 09 Aug 2022 17:21:06 GMT  
		Size: 2.8 MB (2827489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d36b44d0cfa5b827ecf36e664752a4e5b8fc1a4f901a85763621072762da0045`  
		Last Modified: Wed, 10 Aug 2022 01:26:06 GMT  
		Size: 681.1 KB (681068 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b256a1bd7d5e289332916c16569dec3cdb78eb91cfe968dad1be3abaa6592a54`  
		Last Modified: Wed, 10 Aug 2022 01:26:10 GMT  
		Size: 22.2 MB (22162060 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b7ca5c826b27e2f48e1984235d4742a75652cd7682a0769fe815acabae80ddf`  
		Last Modified: Wed, 10 Aug 2022 01:26:06 GMT  
		Size: 368.0 B  
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
$ docker pull traefik@sha256:4164df484f4b6b89d809c899cefaae2bfd7962eacf756ca417989965c5783b28
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.5 MB (23536220 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8c6e41da4eded9e8dcedab7d754e6ea8327030df73dd4edc84cdc91ebcb8a95d`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Tue, 09 Aug 2022 17:39:59 GMT
ADD file:b312c8f512719efd09811d17c2b250bbad03cf3f90c135a00695cc8e152f4ee2 in / 
# Tue, 09 Aug 2022 17:39:59 GMT
CMD ["/bin/sh"]
# Wed, 10 Aug 2022 06:11:07 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 10 Aug 2022 06:11:14 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/traefik/traefik/releases/download/v1.7.34/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Wed, 10 Aug 2022 06:11:15 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 10 Aug 2022 06:11:15 GMT
EXPOSE 80
# Wed, 10 Aug 2022 06:11:16 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 10 Aug 2022 06:11:17 GMT
CMD ["traefik"]
# Wed, 10 Aug 2022 06:11:18 GMT
LABEL org.opencontainers.image.vendor=traefik org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.34 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:90cda3b7c32511829cd5ae9074240c36c34507085acb6e55b96f993740d2be93`  
		Last Modified: Tue, 09 Aug 2022 17:41:06 GMT  
		Size: 2.7 MB (2722153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed77a2aa4d354461d4394dcedb6b641f6298c516ba832a174652464a19b489f7`  
		Last Modified: Wed, 10 Aug 2022 06:12:39 GMT  
		Size: 682.3 KB (682314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3eb22d62b1873f7ed10c4ea0a5503cd0d75bddc18adbc0bb5ecd44e4e6ae9f50`  
		Last Modified: Wed, 10 Aug 2022 06:12:42 GMT  
		Size: 20.1 MB (20131384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2aedce2bbbad30ed9b4ae17a9bda0fff6ad652d205bd6d2a65ea86b8c33dddd`  
		Last Modified: Wed, 10 Aug 2022 06:12:39 GMT  
		Size: 369.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:1.7-windowsservercore-1809`

```console
$ docker pull traefik@sha256:0f10109d86f347d0326edc28ce65ac4f3d485e4e282b52505d9507e9da36b0c4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3287; amd64

### `traefik:1.7-windowsservercore-1809` - windows version 10.0.17763.3287; amd64

```console
$ docker pull traefik@sha256:23182fb91cd4c2bd2311cf57479594893425702f0afc632520a6fc74b432e62c
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2700555687 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a756bb07a27a99c1a7997636266ee330bea763938462d1fda845abd62753ba8c`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Sat, 06 Aug 2022 18:30:32 GMT
RUN Install update 10.0.17763.3287
# Wed, 10 Aug 2022 12:16:16 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Aug 2022 19:22:52 GMT
RUN Invoke-WebRequest     -Uri "https://github.com/traefik/traefik/releases/download/v1.7.34/traefik_windows-amd64.exe"     -OutFile "/traefik.exe"
# Wed, 10 Aug 2022 19:22:53 GMT
EXPOSE 80
# Wed, 10 Aug 2022 19:22:54 GMT
ENTRYPOINT ["/traefik"]
# Wed, 10 Aug 2022 19:22:55 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.34 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:b111c3320c949bea81612bf4554f1b6592c2f504920b5bf57ba340a1d4d52c93`  
		Size: 1.9 GB (1877166088 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:294d77ac553d7210b662d07674ef9e39a6c2e88dc15b9d2788d51e509bc8b54e`  
		Size: 800.5 MB (800546641 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:d64f32398ff5e4ac4cbab317ffed87a2fbf4e4a37210284dba19f2929d631a95`  
		Last Modified: Wed, 10 Aug 2022 12:42:57 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bf2328c550caf93706630a4a6283a81124bce25f56889a67c42b6ea61409d06`  
		Last Modified: Wed, 10 Aug 2022 19:23:47 GMT  
		Size: 22.8 MB (22837223 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04c547d744d6ccc5c0fec076a7f15bd63ec8c73cb2027d023cf00cef0557cd6b`  
		Last Modified: Wed, 10 Aug 2022 19:23:41 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44e0ce1d03f2cd24f681a3b6038c2d11b03bdbf4ca8afe42f489f5c648788629`  
		Last Modified: Wed, 10 Aug 2022 19:23:41 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67d76a3107ed7e08ba9416baf4eb08e87395e64b4c9c4f0d728520f8164ca5a0`  
		Last Modified: Wed, 10 Aug 2022 19:23:42 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:1.7.34`

```console
$ docker pull traefik@sha256:bd12a7039c4736697cab4ee722d4f7683ee292b5b47b861a44a007a30c0581dd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:1.7.34` - linux; amd64

```console
$ docker pull traefik@sha256:221d4ca433d21b148f21168a3c71aeb10d776f7d9051fb612b10be1d703f9c36
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **22.6 MB (22614032 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fd7cc9150335f309f34597c684d908b517b7aa428c550fa8f63dd1a19bafbfe4`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Wed, 10 Aug 2022 01:25:18 GMT
COPY file:48964762d0c961c28f59ebd3ea194fb6486cf2bd9a9cf1780f6702d88bd7b7d9 in /etc/ssl/certs/ 
# Wed, 10 Aug 2022 01:25:19 GMT
COPY dir:a84372748b89eb90478bb1b120b7c8fff3112421d7f93e50fbeae3f53adc6788 in /usr/share/ 
# Wed, 10 Aug 2022 01:25:20 GMT
COPY file:36217e5a6056bef26cfff395c8af8c1010a61dbe8d62b2c7869ca221e2a6302c in / 
# Wed, 10 Aug 2022 01:25:20 GMT
EXPOSE 80
# Wed, 10 Aug 2022 01:25:20 GMT
VOLUME [/tmp]
# Wed, 10 Aug 2022 01:25:20 GMT
ENTRYPOINT ["/traefik"]
# Wed, 10 Aug 2022 01:25:20 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.34 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:dcf6dab73e17be4a506f9432554b84ca5af22b6ca8d3a28551e98fd1c05660dc`  
		Last Modified: Wed, 10 Aug 2022 01:26:26 GMT  
		Size: 123.5 KB (123538 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd04e95cb63652c8a3323efd5c36bdcf17166632bd5bbf9c5c72092392094ebb`  
		Last Modified: Wed, 10 Aug 2022 01:26:26 GMT  
		Size: 328.5 KB (328542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bc5ce073739868727c7f64505383cab253c15631bf675c2b65bb384d4ae4b1e`  
		Last Modified: Wed, 10 Aug 2022 01:26:30 GMT  
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
$ docker pull traefik@sha256:ee80ec61ce7968fa7680b289cc4e0cb29933f0d254c962f4ba94b87de29bbbe7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **20.6 MB (20583416 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:72b9e44203aa217fc68aff257b65b34390dec5720d4c89a2c3722476af10cdef`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Wed, 10 Aug 2022 06:11:29 GMT
COPY file:48964762d0c961c28f59ebd3ea194fb6486cf2bd9a9cf1780f6702d88bd7b7d9 in /etc/ssl/certs/ 
# Wed, 10 Aug 2022 06:11:30 GMT
COPY dir:a84372748b89eb90478bb1b120b7c8fff3112421d7f93e50fbeae3f53adc6788 in /usr/share/ 
# Wed, 10 Aug 2022 06:11:31 GMT
COPY file:60330593b6644f3f519fd13ce8ee34c2c7ab9994a1420afabbc01926dd1230dd in / 
# Wed, 10 Aug 2022 06:11:31 GMT
EXPOSE 80
# Wed, 10 Aug 2022 06:11:32 GMT
VOLUME [/tmp]
# Wed, 10 Aug 2022 06:11:33 GMT
ENTRYPOINT ["/traefik"]
# Wed, 10 Aug 2022 06:11:34 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.34 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:45ff194111b414e1aa5548434d84e56dbd11ebe2589d05ac6498a25d0e8adfcd`  
		Last Modified: Wed, 10 Aug 2022 06:13:02 GMT  
		Size: 123.5 KB (123544 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0a00cc3745cda02ead5281ab2de73712088f63bdf0bb2e31932d82d8d4c4236`  
		Last Modified: Wed, 10 Aug 2022 06:13:02 GMT  
		Size: 328.5 KB (328525 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c10648c89e22ebcc358eb0f5e84d1de66c1d49da6d460218007ffe19f65baafc`  
		Last Modified: Wed, 10 Aug 2022 06:13:05 GMT  
		Size: 20.1 MB (20131347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:1.7.34-alpine`

```console
$ docker pull traefik@sha256:a65ea31d38ab997c3ec977ca7e46192823ef829c298574e0365c1878f5e447f9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:1.7.34-alpine` - linux; amd64

```console
$ docker pull traefik@sha256:fa0b479bcd6943cf3eee0f076f096253cd87d60eedbd550c5c46093f8a272aae
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.7 MB (25670985 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d93d266ccb4853b50019238b20d45befbbb64114d2780ee6582d87058faf9269`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Tue, 09 Aug 2022 17:20:07 GMT
ADD file:b9bd10cf83356cb7281baa0fbaca5186cf27491f59eda87abe57f83a5aaf5ec1 in / 
# Tue, 09 Aug 2022 17:20:08 GMT
CMD ["/bin/sh"]
# Wed, 10 Aug 2022 01:25:03 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 10 Aug 2022 01:25:09 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/traefik/traefik/releases/download/v1.7.34/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Wed, 10 Aug 2022 01:25:09 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 10 Aug 2022 01:25:10 GMT
EXPOSE 80
# Wed, 10 Aug 2022 01:25:10 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 10 Aug 2022 01:25:10 GMT
CMD ["traefik"]
# Wed, 10 Aug 2022 01:25:10 GMT
LABEL org.opencontainers.image.vendor=traefik org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.34 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:c7ed990a2339ee598662849de4f56e2241399f5a32340c8c4a7bbd5378a12b5f`  
		Last Modified: Tue, 09 Aug 2022 17:21:06 GMT  
		Size: 2.8 MB (2827489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d36b44d0cfa5b827ecf36e664752a4e5b8fc1a4f901a85763621072762da0045`  
		Last Modified: Wed, 10 Aug 2022 01:26:06 GMT  
		Size: 681.1 KB (681068 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b256a1bd7d5e289332916c16569dec3cdb78eb91cfe968dad1be3abaa6592a54`  
		Last Modified: Wed, 10 Aug 2022 01:26:10 GMT  
		Size: 22.2 MB (22162060 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b7ca5c826b27e2f48e1984235d4742a75652cd7682a0769fe815acabae80ddf`  
		Last Modified: Wed, 10 Aug 2022 01:26:06 GMT  
		Size: 368.0 B  
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
$ docker pull traefik@sha256:4164df484f4b6b89d809c899cefaae2bfd7962eacf756ca417989965c5783b28
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.5 MB (23536220 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8c6e41da4eded9e8dcedab7d754e6ea8327030df73dd4edc84cdc91ebcb8a95d`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Tue, 09 Aug 2022 17:39:59 GMT
ADD file:b312c8f512719efd09811d17c2b250bbad03cf3f90c135a00695cc8e152f4ee2 in / 
# Tue, 09 Aug 2022 17:39:59 GMT
CMD ["/bin/sh"]
# Wed, 10 Aug 2022 06:11:07 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 10 Aug 2022 06:11:14 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/traefik/traefik/releases/download/v1.7.34/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Wed, 10 Aug 2022 06:11:15 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 10 Aug 2022 06:11:15 GMT
EXPOSE 80
# Wed, 10 Aug 2022 06:11:16 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 10 Aug 2022 06:11:17 GMT
CMD ["traefik"]
# Wed, 10 Aug 2022 06:11:18 GMT
LABEL org.opencontainers.image.vendor=traefik org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.34 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:90cda3b7c32511829cd5ae9074240c36c34507085acb6e55b96f993740d2be93`  
		Last Modified: Tue, 09 Aug 2022 17:41:06 GMT  
		Size: 2.7 MB (2722153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed77a2aa4d354461d4394dcedb6b641f6298c516ba832a174652464a19b489f7`  
		Last Modified: Wed, 10 Aug 2022 06:12:39 GMT  
		Size: 682.3 KB (682314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3eb22d62b1873f7ed10c4ea0a5503cd0d75bddc18adbc0bb5ecd44e4e6ae9f50`  
		Last Modified: Wed, 10 Aug 2022 06:12:42 GMT  
		Size: 20.1 MB (20131384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2aedce2bbbad30ed9b4ae17a9bda0fff6ad652d205bd6d2a65ea86b8c33dddd`  
		Last Modified: Wed, 10 Aug 2022 06:12:39 GMT  
		Size: 369.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:1.7.34-windowsservercore-1809`

```console
$ docker pull traefik@sha256:0f10109d86f347d0326edc28ce65ac4f3d485e4e282b52505d9507e9da36b0c4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3287; amd64

### `traefik:1.7.34-windowsservercore-1809` - windows version 10.0.17763.3287; amd64

```console
$ docker pull traefik@sha256:23182fb91cd4c2bd2311cf57479594893425702f0afc632520a6fc74b432e62c
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2700555687 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a756bb07a27a99c1a7997636266ee330bea763938462d1fda845abd62753ba8c`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Sat, 06 Aug 2022 18:30:32 GMT
RUN Install update 10.0.17763.3287
# Wed, 10 Aug 2022 12:16:16 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Aug 2022 19:22:52 GMT
RUN Invoke-WebRequest     -Uri "https://github.com/traefik/traefik/releases/download/v1.7.34/traefik_windows-amd64.exe"     -OutFile "/traefik.exe"
# Wed, 10 Aug 2022 19:22:53 GMT
EXPOSE 80
# Wed, 10 Aug 2022 19:22:54 GMT
ENTRYPOINT ["/traefik"]
# Wed, 10 Aug 2022 19:22:55 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.34 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:b111c3320c949bea81612bf4554f1b6592c2f504920b5bf57ba340a1d4d52c93`  
		Size: 1.9 GB (1877166088 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:294d77ac553d7210b662d07674ef9e39a6c2e88dc15b9d2788d51e509bc8b54e`  
		Size: 800.5 MB (800546641 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:d64f32398ff5e4ac4cbab317ffed87a2fbf4e4a37210284dba19f2929d631a95`  
		Last Modified: Wed, 10 Aug 2022 12:42:57 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bf2328c550caf93706630a4a6283a81124bce25f56889a67c42b6ea61409d06`  
		Last Modified: Wed, 10 Aug 2022 19:23:47 GMT  
		Size: 22.8 MB (22837223 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04c547d744d6ccc5c0fec076a7f15bd63ec8c73cb2027d023cf00cef0557cd6b`  
		Last Modified: Wed, 10 Aug 2022 19:23:41 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44e0ce1d03f2cd24f681a3b6038c2d11b03bdbf4ca8afe42f489f5c648788629`  
		Last Modified: Wed, 10 Aug 2022 19:23:41 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67d76a3107ed7e08ba9416baf4eb08e87395e64b4c9c4f0d728520f8164ca5a0`  
		Last Modified: Wed, 10 Aug 2022 19:23:42 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:2.8`

```console
$ docker pull traefik@sha256:9717bde18a6e109c63a88e4b67725500c701768d7c044fc64c83efdb892b5738
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; s390x

### `traefik:2.8` - linux; amd64

```console
$ docker pull traefik@sha256:c0ee1d98d82d145d449d468c9f7cecf099c224b0efa23d72f8d976548dc6ff98
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.3 MB (33280383 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9d00af07cc7c91c3470ab5fb46d2caef28f984d258f110f77a7cd2b148fc93b4`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Tue, 09 Aug 2022 17:20:00 GMT
ADD file:f77e3f51f020890d22997e6c2ca98968b75b8bc8c463341a2010ff0655d4c88f in / 
# Tue, 09 Aug 2022 17:20:01 GMT
CMD ["/bin/sh"]
# Wed, 10 Aug 2022 01:24:52 GMT
RUN apk --no-cache add ca-certificates tzdata
# Fri, 02 Sep 2022 20:50:13 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.8.4/traefik_v2.8.4_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Fri, 02 Sep 2022 20:50:14 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Fri, 02 Sep 2022 20:50:14 GMT
EXPOSE 80
# Fri, 02 Sep 2022 20:50:14 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 02 Sep 2022 20:50:14 GMT
CMD ["traefik"]
# Fri, 02 Sep 2022 20:50:14 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.8.4 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:9621f1afde84053b2f9b6ff34fc7f7460712247c01cbab483c5fa7132cf782ca`  
		Last Modified: Tue, 09 Aug 2022 17:20:52 GMT  
		Size: 2.8 MB (2823512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0448c16748457249205ca0475f796fa6c4661fdcbf2d618c5241bdf9c4b12f9a`  
		Last Modified: Wed, 10 Aug 2022 01:25:43 GMT  
		Size: 681.7 KB (681674 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4b54ed04da5e95dc580e80f0518e3c13b776377f5404327988acec675e499ab`  
		Last Modified: Fri, 02 Sep 2022 20:50:44 GMT  
		Size: 29.8 MB (29774829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9447aa44267fb53387d49c2e1fc049f08581306fca07488baab643e3f559d90b`  
		Last Modified: Fri, 02 Sep 2022 20:50:39 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:2.8` - linux; arm variant v6

```console
$ docker pull traefik@sha256:524dea2468148d17e36e8685b1ae6bb8b32fc824dc67d9ae0d006f78c205c9ba
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.4 MB (31406635 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a470b476d302ab7cd2965d189b989a1ebeafc3b3f51c3fc9a3f7352590ad8c75`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Tue, 09 Aug 2022 17:49:29 GMT
ADD file:89cb25f97e17bed5c56311280efe5cfa78422d8ffbe36232195d13f94d67417e in / 
# Tue, 09 Aug 2022 17:49:29 GMT
CMD ["/bin/sh"]
# Thu, 11 Aug 2022 01:14:12 GMT
RUN apk --no-cache add ca-certificates tzdata
# Fri, 02 Sep 2022 19:49:39 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.8.4/traefik_v2.8.4_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Fri, 02 Sep 2022 19:49:39 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Fri, 02 Sep 2022 19:49:39 GMT
EXPOSE 80
# Fri, 02 Sep 2022 19:49:39 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 02 Sep 2022 19:49:39 GMT
CMD ["traefik"]
# Fri, 02 Sep 2022 19:49:40 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.8.4 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:2184ddf72fafdec856907308b0832d0cb9fa3f18d27bc8923d31bf537000722a`  
		Last Modified: Fri, 02 Sep 2022 19:50:45 GMT  
		Size: 28.1 MB (28089099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70bab47ff3f98940f7fa7d3eb55a81c68ba899a88b3b57e7e2ff3574eb5c2ca5`  
		Last Modified: Fri, 02 Sep 2022 19:50:39 GMT  
		Size: 367.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:2.8` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:3af1ee8b3fff09a9e7bc958150245c14eebf6910fee151320b716a0ce0278b80
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.6 MB (30575438 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:148847c384149af925afcbbf2a63d3d9537e1c3e0e3fc4778ce849c30fc414a9`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Tue, 09 Aug 2022 17:39:51 GMT
ADD file:4b51a9d40f20d2beb29d0759b161d2b9403493453beb509de4e86a5d98513f16 in / 
# Tue, 09 Aug 2022 17:39:51 GMT
CMD ["/bin/sh"]
# Wed, 10 Aug 2022 06:10:52 GMT
RUN apk --no-cache add ca-certificates tzdata
# Fri, 02 Sep 2022 21:02:06 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.8.4/traefik_v2.8.4_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Fri, 02 Sep 2022 21:02:08 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Fri, 02 Sep 2022 21:02:08 GMT
EXPOSE 80
# Fri, 02 Sep 2022 21:02:09 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 02 Sep 2022 21:02:10 GMT
CMD ["traefik"]
# Fri, 02 Sep 2022 21:02:11 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.8.4 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:47517142f6ba87eca6b7bdca1e0df160b74671c81e4b9605dad38c1862a43be3`  
		Last Modified: Tue, 09 Aug 2022 17:40:55 GMT  
		Size: 2.7 MB (2718439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:966c95a60d9885fe2865b5aef2abf3c8e02dbfcd48f4b9978e47205d35c9a2c1`  
		Last Modified: Wed, 10 Aug 2022 06:12:12 GMT  
		Size: 682.4 KB (682395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97c489cee492d2fe706c61d150982ab2113f63f0b0325eecfcc529c715a025de`  
		Last Modified: Fri, 02 Sep 2022 21:03:03 GMT  
		Size: 27.2 MB (27174235 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb23e7c7b06001a1723b46152cba68a658ef913e0fcd9ce6a675782ee6e91153`  
		Last Modified: Fri, 02 Sep 2022 21:02:58 GMT  
		Size: 369.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:2.8` - linux; s390x

```console
$ docker pull traefik@sha256:0ae44e1db4e8692764f89bc9c6713b5a8f2454a49fb958670f1ce097d771f2d4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.0 MB (31970417 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:907601fe3e786e8291296b20b082a843538ba24e2cb77764166e496ec811d23f`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Tue, 09 Aug 2022 17:41:54 GMT
ADD file:7489fa84133e97e4f40b13dd5159989b3594c9627d9147bfc4e33134944cc368 in / 
# Tue, 09 Aug 2022 17:41:54 GMT
CMD ["/bin/sh"]
# Wed, 10 Aug 2022 05:50:07 GMT
RUN apk --no-cache add ca-certificates tzdata
# Fri, 02 Sep 2022 21:18:57 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.8.4/traefik_v2.8.4_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Fri, 02 Sep 2022 21:19:02 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Fri, 02 Sep 2022 21:19:03 GMT
EXPOSE 80
# Fri, 02 Sep 2022 21:19:03 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 02 Sep 2022 21:19:04 GMT
CMD ["traefik"]
# Fri, 02 Sep 2022 21:19:05 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.8.4 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:cdf710f5b7ee39c5124c50c753228dc9b8b1c1c0a1a38f1413487548565445c3`  
		Last Modified: Tue, 09 Aug 2022 17:42:56 GMT  
		Size: 2.6 MB (2606087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d94fe8753c6b15e6f67f3ca19edd0d0c2c0d8f6596878b0a6e212d71d3ae470d`  
		Last Modified: Wed, 10 Aug 2022 05:50:57 GMT  
		Size: 686.5 KB (686528 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a7fc896b96c1b9c8a8c7d6ab0cec469b6114d366b8cc7732f19d5913ad818d1`  
		Last Modified: Fri, 02 Sep 2022 21:19:39 GMT  
		Size: 28.7 MB (28677434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ba0189892c09ebd907a8f9e1885c492cd37742dd2d614b034515e31dda3ec17`  
		Last Modified: Fri, 02 Sep 2022 21:19:34 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:2.8-windowsservercore-1809`

```console
$ docker pull traefik@sha256:e21df88b973943eb3d1fb6882f9aa8f1bfb76f5c91ca24d86b18bbc05814d23f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3287; amd64

### `traefik:2.8-windowsservercore-1809` - windows version 10.0.17763.3287; amd64

```console
$ docker pull traefik@sha256:888c8204cbe36566704c0ff5d27aaba93ddda7fb8705077d813c3776f3720fb7
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2707978103 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:16fe5cbe222e4fdaa4f0280fbb0c434f102b72aadc7759f356eaa9eb475401e1`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Sat, 06 Aug 2022 18:30:32 GMT
RUN Install update 10.0.17763.3287
# Wed, 10 Aug 2022 12:16:16 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Fri, 02 Sep 2022 20:16:28 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/traefik/traefik/releases/download/v2.8.4/traefik_v2.8.4_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Fri, 02 Sep 2022 20:16:29 GMT
EXPOSE 80
# Fri, 02 Sep 2022 20:16:30 GMT
ENTRYPOINT ["/traefik"]
# Fri, 02 Sep 2022 20:16:31 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.8.4 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:b111c3320c949bea81612bf4554f1b6592c2f504920b5bf57ba340a1d4d52c93`  
		Size: 1.9 GB (1877166088 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:294d77ac553d7210b662d07674ef9e39a6c2e88dc15b9d2788d51e509bc8b54e`  
		Size: 800.5 MB (800546641 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:d64f32398ff5e4ac4cbab317ffed87a2fbf4e4a37210284dba19f2929d631a95`  
		Last Modified: Wed, 10 Aug 2022 12:42:57 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0313b7cb0203c87fdae2ed13c632236f1787bce1ad528657ed30a38ddbf5235`  
		Last Modified: Fri, 02 Sep 2022 20:17:11 GMT  
		Size: 30.3 MB (30259693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be311a3bfd74b89aba7388644de2836f16ccd492641301a25dc40a8d95bdcf1c`  
		Last Modified: Fri, 02 Sep 2022 20:17:05 GMT  
		Size: 1.4 KB (1389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81354628ab86c777160694d48d5d428248dff2d7621fc494da604be40c91e403`  
		Last Modified: Fri, 02 Sep 2022 20:17:05 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8c2a232471cae5193369cbc619007f710b7ea681e38f34a91f7a19213940d82`  
		Last Modified: Fri, 02 Sep 2022 20:17:05 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:2.8.4`

```console
$ docker pull traefik@sha256:9717bde18a6e109c63a88e4b67725500c701768d7c044fc64c83efdb892b5738
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; s390x

### `traefik:2.8.4` - linux; amd64

```console
$ docker pull traefik@sha256:c0ee1d98d82d145d449d468c9f7cecf099c224b0efa23d72f8d976548dc6ff98
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.3 MB (33280383 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9d00af07cc7c91c3470ab5fb46d2caef28f984d258f110f77a7cd2b148fc93b4`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Tue, 09 Aug 2022 17:20:00 GMT
ADD file:f77e3f51f020890d22997e6c2ca98968b75b8bc8c463341a2010ff0655d4c88f in / 
# Tue, 09 Aug 2022 17:20:01 GMT
CMD ["/bin/sh"]
# Wed, 10 Aug 2022 01:24:52 GMT
RUN apk --no-cache add ca-certificates tzdata
# Fri, 02 Sep 2022 20:50:13 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.8.4/traefik_v2.8.4_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Fri, 02 Sep 2022 20:50:14 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Fri, 02 Sep 2022 20:50:14 GMT
EXPOSE 80
# Fri, 02 Sep 2022 20:50:14 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 02 Sep 2022 20:50:14 GMT
CMD ["traefik"]
# Fri, 02 Sep 2022 20:50:14 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.8.4 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:9621f1afde84053b2f9b6ff34fc7f7460712247c01cbab483c5fa7132cf782ca`  
		Last Modified: Tue, 09 Aug 2022 17:20:52 GMT  
		Size: 2.8 MB (2823512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0448c16748457249205ca0475f796fa6c4661fdcbf2d618c5241bdf9c4b12f9a`  
		Last Modified: Wed, 10 Aug 2022 01:25:43 GMT  
		Size: 681.7 KB (681674 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4b54ed04da5e95dc580e80f0518e3c13b776377f5404327988acec675e499ab`  
		Last Modified: Fri, 02 Sep 2022 20:50:44 GMT  
		Size: 29.8 MB (29774829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9447aa44267fb53387d49c2e1fc049f08581306fca07488baab643e3f559d90b`  
		Last Modified: Fri, 02 Sep 2022 20:50:39 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:2.8.4` - linux; arm variant v6

```console
$ docker pull traefik@sha256:524dea2468148d17e36e8685b1ae6bb8b32fc824dc67d9ae0d006f78c205c9ba
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.4 MB (31406635 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a470b476d302ab7cd2965d189b989a1ebeafc3b3f51c3fc9a3f7352590ad8c75`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Tue, 09 Aug 2022 17:49:29 GMT
ADD file:89cb25f97e17bed5c56311280efe5cfa78422d8ffbe36232195d13f94d67417e in / 
# Tue, 09 Aug 2022 17:49:29 GMT
CMD ["/bin/sh"]
# Thu, 11 Aug 2022 01:14:12 GMT
RUN apk --no-cache add ca-certificates tzdata
# Fri, 02 Sep 2022 19:49:39 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.8.4/traefik_v2.8.4_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Fri, 02 Sep 2022 19:49:39 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Fri, 02 Sep 2022 19:49:39 GMT
EXPOSE 80
# Fri, 02 Sep 2022 19:49:39 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 02 Sep 2022 19:49:39 GMT
CMD ["traefik"]
# Fri, 02 Sep 2022 19:49:40 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.8.4 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:2184ddf72fafdec856907308b0832d0cb9fa3f18d27bc8923d31bf537000722a`  
		Last Modified: Fri, 02 Sep 2022 19:50:45 GMT  
		Size: 28.1 MB (28089099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70bab47ff3f98940f7fa7d3eb55a81c68ba899a88b3b57e7e2ff3574eb5c2ca5`  
		Last Modified: Fri, 02 Sep 2022 19:50:39 GMT  
		Size: 367.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:2.8.4` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:3af1ee8b3fff09a9e7bc958150245c14eebf6910fee151320b716a0ce0278b80
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.6 MB (30575438 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:148847c384149af925afcbbf2a63d3d9537e1c3e0e3fc4778ce849c30fc414a9`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Tue, 09 Aug 2022 17:39:51 GMT
ADD file:4b51a9d40f20d2beb29d0759b161d2b9403493453beb509de4e86a5d98513f16 in / 
# Tue, 09 Aug 2022 17:39:51 GMT
CMD ["/bin/sh"]
# Wed, 10 Aug 2022 06:10:52 GMT
RUN apk --no-cache add ca-certificates tzdata
# Fri, 02 Sep 2022 21:02:06 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.8.4/traefik_v2.8.4_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Fri, 02 Sep 2022 21:02:08 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Fri, 02 Sep 2022 21:02:08 GMT
EXPOSE 80
# Fri, 02 Sep 2022 21:02:09 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 02 Sep 2022 21:02:10 GMT
CMD ["traefik"]
# Fri, 02 Sep 2022 21:02:11 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.8.4 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:47517142f6ba87eca6b7bdca1e0df160b74671c81e4b9605dad38c1862a43be3`  
		Last Modified: Tue, 09 Aug 2022 17:40:55 GMT  
		Size: 2.7 MB (2718439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:966c95a60d9885fe2865b5aef2abf3c8e02dbfcd48f4b9978e47205d35c9a2c1`  
		Last Modified: Wed, 10 Aug 2022 06:12:12 GMT  
		Size: 682.4 KB (682395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97c489cee492d2fe706c61d150982ab2113f63f0b0325eecfcc529c715a025de`  
		Last Modified: Fri, 02 Sep 2022 21:03:03 GMT  
		Size: 27.2 MB (27174235 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb23e7c7b06001a1723b46152cba68a658ef913e0fcd9ce6a675782ee6e91153`  
		Last Modified: Fri, 02 Sep 2022 21:02:58 GMT  
		Size: 369.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:2.8.4` - linux; s390x

```console
$ docker pull traefik@sha256:0ae44e1db4e8692764f89bc9c6713b5a8f2454a49fb958670f1ce097d771f2d4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.0 MB (31970417 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:907601fe3e786e8291296b20b082a843538ba24e2cb77764166e496ec811d23f`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Tue, 09 Aug 2022 17:41:54 GMT
ADD file:7489fa84133e97e4f40b13dd5159989b3594c9627d9147bfc4e33134944cc368 in / 
# Tue, 09 Aug 2022 17:41:54 GMT
CMD ["/bin/sh"]
# Wed, 10 Aug 2022 05:50:07 GMT
RUN apk --no-cache add ca-certificates tzdata
# Fri, 02 Sep 2022 21:18:57 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.8.4/traefik_v2.8.4_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Fri, 02 Sep 2022 21:19:02 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Fri, 02 Sep 2022 21:19:03 GMT
EXPOSE 80
# Fri, 02 Sep 2022 21:19:03 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 02 Sep 2022 21:19:04 GMT
CMD ["traefik"]
# Fri, 02 Sep 2022 21:19:05 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.8.4 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:cdf710f5b7ee39c5124c50c753228dc9b8b1c1c0a1a38f1413487548565445c3`  
		Last Modified: Tue, 09 Aug 2022 17:42:56 GMT  
		Size: 2.6 MB (2606087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d94fe8753c6b15e6f67f3ca19edd0d0c2c0d8f6596878b0a6e212d71d3ae470d`  
		Last Modified: Wed, 10 Aug 2022 05:50:57 GMT  
		Size: 686.5 KB (686528 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a7fc896b96c1b9c8a8c7d6ab0cec469b6114d366b8cc7732f19d5913ad818d1`  
		Last Modified: Fri, 02 Sep 2022 21:19:39 GMT  
		Size: 28.7 MB (28677434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ba0189892c09ebd907a8f9e1885c492cd37742dd2d614b034515e31dda3ec17`  
		Last Modified: Fri, 02 Sep 2022 21:19:34 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:2.8.4-windowsservercore-1809`

```console
$ docker pull traefik@sha256:e21df88b973943eb3d1fb6882f9aa8f1bfb76f5c91ca24d86b18bbc05814d23f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3287; amd64

### `traefik:2.8.4-windowsservercore-1809` - windows version 10.0.17763.3287; amd64

```console
$ docker pull traefik@sha256:888c8204cbe36566704c0ff5d27aaba93ddda7fb8705077d813c3776f3720fb7
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2707978103 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:16fe5cbe222e4fdaa4f0280fbb0c434f102b72aadc7759f356eaa9eb475401e1`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Sat, 06 Aug 2022 18:30:32 GMT
RUN Install update 10.0.17763.3287
# Wed, 10 Aug 2022 12:16:16 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Fri, 02 Sep 2022 20:16:28 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/traefik/traefik/releases/download/v2.8.4/traefik_v2.8.4_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Fri, 02 Sep 2022 20:16:29 GMT
EXPOSE 80
# Fri, 02 Sep 2022 20:16:30 GMT
ENTRYPOINT ["/traefik"]
# Fri, 02 Sep 2022 20:16:31 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.8.4 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:b111c3320c949bea81612bf4554f1b6592c2f504920b5bf57ba340a1d4d52c93`  
		Size: 1.9 GB (1877166088 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:294d77ac553d7210b662d07674ef9e39a6c2e88dc15b9d2788d51e509bc8b54e`  
		Size: 800.5 MB (800546641 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:d64f32398ff5e4ac4cbab317ffed87a2fbf4e4a37210284dba19f2929d631a95`  
		Last Modified: Wed, 10 Aug 2022 12:42:57 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0313b7cb0203c87fdae2ed13c632236f1787bce1ad528657ed30a38ddbf5235`  
		Last Modified: Fri, 02 Sep 2022 20:17:11 GMT  
		Size: 30.3 MB (30259693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be311a3bfd74b89aba7388644de2836f16ccd492641301a25dc40a8d95bdcf1c`  
		Last Modified: Fri, 02 Sep 2022 20:17:05 GMT  
		Size: 1.4 KB (1389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81354628ab86c777160694d48d5d428248dff2d7621fc494da604be40c91e403`  
		Last Modified: Fri, 02 Sep 2022 20:17:05 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8c2a232471cae5193369cbc619007f710b7ea681e38f34a91f7a19213940d82`  
		Last Modified: Fri, 02 Sep 2022 20:17:05 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:latest`

```console
$ docker pull traefik@sha256:9717bde18a6e109c63a88e4b67725500c701768d7c044fc64c83efdb892b5738
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; s390x

### `traefik:latest` - linux; amd64

```console
$ docker pull traefik@sha256:c0ee1d98d82d145d449d468c9f7cecf099c224b0efa23d72f8d976548dc6ff98
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.3 MB (33280383 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9d00af07cc7c91c3470ab5fb46d2caef28f984d258f110f77a7cd2b148fc93b4`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Tue, 09 Aug 2022 17:20:00 GMT
ADD file:f77e3f51f020890d22997e6c2ca98968b75b8bc8c463341a2010ff0655d4c88f in / 
# Tue, 09 Aug 2022 17:20:01 GMT
CMD ["/bin/sh"]
# Wed, 10 Aug 2022 01:24:52 GMT
RUN apk --no-cache add ca-certificates tzdata
# Fri, 02 Sep 2022 20:50:13 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.8.4/traefik_v2.8.4_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Fri, 02 Sep 2022 20:50:14 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Fri, 02 Sep 2022 20:50:14 GMT
EXPOSE 80
# Fri, 02 Sep 2022 20:50:14 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 02 Sep 2022 20:50:14 GMT
CMD ["traefik"]
# Fri, 02 Sep 2022 20:50:14 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.8.4 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:9621f1afde84053b2f9b6ff34fc7f7460712247c01cbab483c5fa7132cf782ca`  
		Last Modified: Tue, 09 Aug 2022 17:20:52 GMT  
		Size: 2.8 MB (2823512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0448c16748457249205ca0475f796fa6c4661fdcbf2d618c5241bdf9c4b12f9a`  
		Last Modified: Wed, 10 Aug 2022 01:25:43 GMT  
		Size: 681.7 KB (681674 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4b54ed04da5e95dc580e80f0518e3c13b776377f5404327988acec675e499ab`  
		Last Modified: Fri, 02 Sep 2022 20:50:44 GMT  
		Size: 29.8 MB (29774829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9447aa44267fb53387d49c2e1fc049f08581306fca07488baab643e3f559d90b`  
		Last Modified: Fri, 02 Sep 2022 20:50:39 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:latest` - linux; arm variant v6

```console
$ docker pull traefik@sha256:524dea2468148d17e36e8685b1ae6bb8b32fc824dc67d9ae0d006f78c205c9ba
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.4 MB (31406635 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a470b476d302ab7cd2965d189b989a1ebeafc3b3f51c3fc9a3f7352590ad8c75`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Tue, 09 Aug 2022 17:49:29 GMT
ADD file:89cb25f97e17bed5c56311280efe5cfa78422d8ffbe36232195d13f94d67417e in / 
# Tue, 09 Aug 2022 17:49:29 GMT
CMD ["/bin/sh"]
# Thu, 11 Aug 2022 01:14:12 GMT
RUN apk --no-cache add ca-certificates tzdata
# Fri, 02 Sep 2022 19:49:39 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.8.4/traefik_v2.8.4_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Fri, 02 Sep 2022 19:49:39 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Fri, 02 Sep 2022 19:49:39 GMT
EXPOSE 80
# Fri, 02 Sep 2022 19:49:39 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 02 Sep 2022 19:49:39 GMT
CMD ["traefik"]
# Fri, 02 Sep 2022 19:49:40 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.8.4 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:2184ddf72fafdec856907308b0832d0cb9fa3f18d27bc8923d31bf537000722a`  
		Last Modified: Fri, 02 Sep 2022 19:50:45 GMT  
		Size: 28.1 MB (28089099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70bab47ff3f98940f7fa7d3eb55a81c68ba899a88b3b57e7e2ff3574eb5c2ca5`  
		Last Modified: Fri, 02 Sep 2022 19:50:39 GMT  
		Size: 367.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:latest` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:3af1ee8b3fff09a9e7bc958150245c14eebf6910fee151320b716a0ce0278b80
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.6 MB (30575438 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:148847c384149af925afcbbf2a63d3d9537e1c3e0e3fc4778ce849c30fc414a9`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Tue, 09 Aug 2022 17:39:51 GMT
ADD file:4b51a9d40f20d2beb29d0759b161d2b9403493453beb509de4e86a5d98513f16 in / 
# Tue, 09 Aug 2022 17:39:51 GMT
CMD ["/bin/sh"]
# Wed, 10 Aug 2022 06:10:52 GMT
RUN apk --no-cache add ca-certificates tzdata
# Fri, 02 Sep 2022 21:02:06 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.8.4/traefik_v2.8.4_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Fri, 02 Sep 2022 21:02:08 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Fri, 02 Sep 2022 21:02:08 GMT
EXPOSE 80
# Fri, 02 Sep 2022 21:02:09 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 02 Sep 2022 21:02:10 GMT
CMD ["traefik"]
# Fri, 02 Sep 2022 21:02:11 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.8.4 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:47517142f6ba87eca6b7bdca1e0df160b74671c81e4b9605dad38c1862a43be3`  
		Last Modified: Tue, 09 Aug 2022 17:40:55 GMT  
		Size: 2.7 MB (2718439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:966c95a60d9885fe2865b5aef2abf3c8e02dbfcd48f4b9978e47205d35c9a2c1`  
		Last Modified: Wed, 10 Aug 2022 06:12:12 GMT  
		Size: 682.4 KB (682395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97c489cee492d2fe706c61d150982ab2113f63f0b0325eecfcc529c715a025de`  
		Last Modified: Fri, 02 Sep 2022 21:03:03 GMT  
		Size: 27.2 MB (27174235 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb23e7c7b06001a1723b46152cba68a658ef913e0fcd9ce6a675782ee6e91153`  
		Last Modified: Fri, 02 Sep 2022 21:02:58 GMT  
		Size: 369.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:latest` - linux; s390x

```console
$ docker pull traefik@sha256:0ae44e1db4e8692764f89bc9c6713b5a8f2454a49fb958670f1ce097d771f2d4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.0 MB (31970417 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:907601fe3e786e8291296b20b082a843538ba24e2cb77764166e496ec811d23f`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Tue, 09 Aug 2022 17:41:54 GMT
ADD file:7489fa84133e97e4f40b13dd5159989b3594c9627d9147bfc4e33134944cc368 in / 
# Tue, 09 Aug 2022 17:41:54 GMT
CMD ["/bin/sh"]
# Wed, 10 Aug 2022 05:50:07 GMT
RUN apk --no-cache add ca-certificates tzdata
# Fri, 02 Sep 2022 21:18:57 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.8.4/traefik_v2.8.4_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Fri, 02 Sep 2022 21:19:02 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Fri, 02 Sep 2022 21:19:03 GMT
EXPOSE 80
# Fri, 02 Sep 2022 21:19:03 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 02 Sep 2022 21:19:04 GMT
CMD ["traefik"]
# Fri, 02 Sep 2022 21:19:05 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.8.4 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:cdf710f5b7ee39c5124c50c753228dc9b8b1c1c0a1a38f1413487548565445c3`  
		Last Modified: Tue, 09 Aug 2022 17:42:56 GMT  
		Size: 2.6 MB (2606087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d94fe8753c6b15e6f67f3ca19edd0d0c2c0d8f6596878b0a6e212d71d3ae470d`  
		Last Modified: Wed, 10 Aug 2022 05:50:57 GMT  
		Size: 686.5 KB (686528 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a7fc896b96c1b9c8a8c7d6ab0cec469b6114d366b8cc7732f19d5913ad818d1`  
		Last Modified: Fri, 02 Sep 2022 21:19:39 GMT  
		Size: 28.7 MB (28677434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ba0189892c09ebd907a8f9e1885c492cd37742dd2d614b034515e31dda3ec17`  
		Last Modified: Fri, 02 Sep 2022 21:19:34 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:maroilles`

```console
$ docker pull traefik@sha256:bd12a7039c4736697cab4ee722d4f7683ee292b5b47b861a44a007a30c0581dd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:maroilles` - linux; amd64

```console
$ docker pull traefik@sha256:221d4ca433d21b148f21168a3c71aeb10d776f7d9051fb612b10be1d703f9c36
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **22.6 MB (22614032 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fd7cc9150335f309f34597c684d908b517b7aa428c550fa8f63dd1a19bafbfe4`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Wed, 10 Aug 2022 01:25:18 GMT
COPY file:48964762d0c961c28f59ebd3ea194fb6486cf2bd9a9cf1780f6702d88bd7b7d9 in /etc/ssl/certs/ 
# Wed, 10 Aug 2022 01:25:19 GMT
COPY dir:a84372748b89eb90478bb1b120b7c8fff3112421d7f93e50fbeae3f53adc6788 in /usr/share/ 
# Wed, 10 Aug 2022 01:25:20 GMT
COPY file:36217e5a6056bef26cfff395c8af8c1010a61dbe8d62b2c7869ca221e2a6302c in / 
# Wed, 10 Aug 2022 01:25:20 GMT
EXPOSE 80
# Wed, 10 Aug 2022 01:25:20 GMT
VOLUME [/tmp]
# Wed, 10 Aug 2022 01:25:20 GMT
ENTRYPOINT ["/traefik"]
# Wed, 10 Aug 2022 01:25:20 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.34 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:dcf6dab73e17be4a506f9432554b84ca5af22b6ca8d3a28551e98fd1c05660dc`  
		Last Modified: Wed, 10 Aug 2022 01:26:26 GMT  
		Size: 123.5 KB (123538 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd04e95cb63652c8a3323efd5c36bdcf17166632bd5bbf9c5c72092392094ebb`  
		Last Modified: Wed, 10 Aug 2022 01:26:26 GMT  
		Size: 328.5 KB (328542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bc5ce073739868727c7f64505383cab253c15631bf675c2b65bb384d4ae4b1e`  
		Last Modified: Wed, 10 Aug 2022 01:26:30 GMT  
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
$ docker pull traefik@sha256:ee80ec61ce7968fa7680b289cc4e0cb29933f0d254c962f4ba94b87de29bbbe7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **20.6 MB (20583416 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:72b9e44203aa217fc68aff257b65b34390dec5720d4c89a2c3722476af10cdef`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Wed, 10 Aug 2022 06:11:29 GMT
COPY file:48964762d0c961c28f59ebd3ea194fb6486cf2bd9a9cf1780f6702d88bd7b7d9 in /etc/ssl/certs/ 
# Wed, 10 Aug 2022 06:11:30 GMT
COPY dir:a84372748b89eb90478bb1b120b7c8fff3112421d7f93e50fbeae3f53adc6788 in /usr/share/ 
# Wed, 10 Aug 2022 06:11:31 GMT
COPY file:60330593b6644f3f519fd13ce8ee34c2c7ab9994a1420afabbc01926dd1230dd in / 
# Wed, 10 Aug 2022 06:11:31 GMT
EXPOSE 80
# Wed, 10 Aug 2022 06:11:32 GMT
VOLUME [/tmp]
# Wed, 10 Aug 2022 06:11:33 GMT
ENTRYPOINT ["/traefik"]
# Wed, 10 Aug 2022 06:11:34 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.34 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:45ff194111b414e1aa5548434d84e56dbd11ebe2589d05ac6498a25d0e8adfcd`  
		Last Modified: Wed, 10 Aug 2022 06:13:02 GMT  
		Size: 123.5 KB (123544 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0a00cc3745cda02ead5281ab2de73712088f63bdf0bb2e31932d82d8d4c4236`  
		Last Modified: Wed, 10 Aug 2022 06:13:02 GMT  
		Size: 328.5 KB (328525 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c10648c89e22ebcc358eb0f5e84d1de66c1d49da6d460218007ffe19f65baafc`  
		Last Modified: Wed, 10 Aug 2022 06:13:05 GMT  
		Size: 20.1 MB (20131347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:maroilles-alpine`

```console
$ docker pull traefik@sha256:a65ea31d38ab997c3ec977ca7e46192823ef829c298574e0365c1878f5e447f9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:maroilles-alpine` - linux; amd64

```console
$ docker pull traefik@sha256:fa0b479bcd6943cf3eee0f076f096253cd87d60eedbd550c5c46093f8a272aae
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.7 MB (25670985 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d93d266ccb4853b50019238b20d45befbbb64114d2780ee6582d87058faf9269`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Tue, 09 Aug 2022 17:20:07 GMT
ADD file:b9bd10cf83356cb7281baa0fbaca5186cf27491f59eda87abe57f83a5aaf5ec1 in / 
# Tue, 09 Aug 2022 17:20:08 GMT
CMD ["/bin/sh"]
# Wed, 10 Aug 2022 01:25:03 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 10 Aug 2022 01:25:09 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/traefik/traefik/releases/download/v1.7.34/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Wed, 10 Aug 2022 01:25:09 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 10 Aug 2022 01:25:10 GMT
EXPOSE 80
# Wed, 10 Aug 2022 01:25:10 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 10 Aug 2022 01:25:10 GMT
CMD ["traefik"]
# Wed, 10 Aug 2022 01:25:10 GMT
LABEL org.opencontainers.image.vendor=traefik org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.34 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:c7ed990a2339ee598662849de4f56e2241399f5a32340c8c4a7bbd5378a12b5f`  
		Last Modified: Tue, 09 Aug 2022 17:21:06 GMT  
		Size: 2.8 MB (2827489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d36b44d0cfa5b827ecf36e664752a4e5b8fc1a4f901a85763621072762da0045`  
		Last Modified: Wed, 10 Aug 2022 01:26:06 GMT  
		Size: 681.1 KB (681068 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b256a1bd7d5e289332916c16569dec3cdb78eb91cfe968dad1be3abaa6592a54`  
		Last Modified: Wed, 10 Aug 2022 01:26:10 GMT  
		Size: 22.2 MB (22162060 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b7ca5c826b27e2f48e1984235d4742a75652cd7682a0769fe815acabae80ddf`  
		Last Modified: Wed, 10 Aug 2022 01:26:06 GMT  
		Size: 368.0 B  
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
$ docker pull traefik@sha256:4164df484f4b6b89d809c899cefaae2bfd7962eacf756ca417989965c5783b28
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.5 MB (23536220 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8c6e41da4eded9e8dcedab7d754e6ea8327030df73dd4edc84cdc91ebcb8a95d`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Tue, 09 Aug 2022 17:39:59 GMT
ADD file:b312c8f512719efd09811d17c2b250bbad03cf3f90c135a00695cc8e152f4ee2 in / 
# Tue, 09 Aug 2022 17:39:59 GMT
CMD ["/bin/sh"]
# Wed, 10 Aug 2022 06:11:07 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 10 Aug 2022 06:11:14 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/traefik/traefik/releases/download/v1.7.34/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Wed, 10 Aug 2022 06:11:15 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 10 Aug 2022 06:11:15 GMT
EXPOSE 80
# Wed, 10 Aug 2022 06:11:16 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 10 Aug 2022 06:11:17 GMT
CMD ["traefik"]
# Wed, 10 Aug 2022 06:11:18 GMT
LABEL org.opencontainers.image.vendor=traefik org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.34 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:90cda3b7c32511829cd5ae9074240c36c34507085acb6e55b96f993740d2be93`  
		Last Modified: Tue, 09 Aug 2022 17:41:06 GMT  
		Size: 2.7 MB (2722153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed77a2aa4d354461d4394dcedb6b641f6298c516ba832a174652464a19b489f7`  
		Last Modified: Wed, 10 Aug 2022 06:12:39 GMT  
		Size: 682.3 KB (682314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3eb22d62b1873f7ed10c4ea0a5503cd0d75bddc18adbc0bb5ecd44e4e6ae9f50`  
		Last Modified: Wed, 10 Aug 2022 06:12:42 GMT  
		Size: 20.1 MB (20131384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2aedce2bbbad30ed9b4ae17a9bda0fff6ad652d205bd6d2a65ea86b8c33dddd`  
		Last Modified: Wed, 10 Aug 2022 06:12:39 GMT  
		Size: 369.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:maroilles-windowsservercore-1809`

```console
$ docker pull traefik@sha256:0f10109d86f347d0326edc28ce65ac4f3d485e4e282b52505d9507e9da36b0c4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3287; amd64

### `traefik:maroilles-windowsservercore-1809` - windows version 10.0.17763.3287; amd64

```console
$ docker pull traefik@sha256:23182fb91cd4c2bd2311cf57479594893425702f0afc632520a6fc74b432e62c
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2700555687 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a756bb07a27a99c1a7997636266ee330bea763938462d1fda845abd62753ba8c`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Sat, 06 Aug 2022 18:30:32 GMT
RUN Install update 10.0.17763.3287
# Wed, 10 Aug 2022 12:16:16 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Aug 2022 19:22:52 GMT
RUN Invoke-WebRequest     -Uri "https://github.com/traefik/traefik/releases/download/v1.7.34/traefik_windows-amd64.exe"     -OutFile "/traefik.exe"
# Wed, 10 Aug 2022 19:22:53 GMT
EXPOSE 80
# Wed, 10 Aug 2022 19:22:54 GMT
ENTRYPOINT ["/traefik"]
# Wed, 10 Aug 2022 19:22:55 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.34 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:b111c3320c949bea81612bf4554f1b6592c2f504920b5bf57ba340a1d4d52c93`  
		Size: 1.9 GB (1877166088 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:294d77ac553d7210b662d07674ef9e39a6c2e88dc15b9d2788d51e509bc8b54e`  
		Size: 800.5 MB (800546641 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:d64f32398ff5e4ac4cbab317ffed87a2fbf4e4a37210284dba19f2929d631a95`  
		Last Modified: Wed, 10 Aug 2022 12:42:57 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bf2328c550caf93706630a4a6283a81124bce25f56889a67c42b6ea61409d06`  
		Last Modified: Wed, 10 Aug 2022 19:23:47 GMT  
		Size: 22.8 MB (22837223 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04c547d744d6ccc5c0fec076a7f15bd63ec8c73cb2027d023cf00cef0557cd6b`  
		Last Modified: Wed, 10 Aug 2022 19:23:41 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44e0ce1d03f2cd24f681a3b6038c2d11b03bdbf4ca8afe42f489f5c648788629`  
		Last Modified: Wed, 10 Aug 2022 19:23:41 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67d76a3107ed7e08ba9416baf4eb08e87395e64b4c9c4f0d728520f8164ca5a0`  
		Last Modified: Wed, 10 Aug 2022 19:23:42 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v1.7`

```console
$ docker pull traefik@sha256:bd12a7039c4736697cab4ee722d4f7683ee292b5b47b861a44a007a30c0581dd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:v1.7` - linux; amd64

```console
$ docker pull traefik@sha256:221d4ca433d21b148f21168a3c71aeb10d776f7d9051fb612b10be1d703f9c36
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **22.6 MB (22614032 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fd7cc9150335f309f34597c684d908b517b7aa428c550fa8f63dd1a19bafbfe4`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Wed, 10 Aug 2022 01:25:18 GMT
COPY file:48964762d0c961c28f59ebd3ea194fb6486cf2bd9a9cf1780f6702d88bd7b7d9 in /etc/ssl/certs/ 
# Wed, 10 Aug 2022 01:25:19 GMT
COPY dir:a84372748b89eb90478bb1b120b7c8fff3112421d7f93e50fbeae3f53adc6788 in /usr/share/ 
# Wed, 10 Aug 2022 01:25:20 GMT
COPY file:36217e5a6056bef26cfff395c8af8c1010a61dbe8d62b2c7869ca221e2a6302c in / 
# Wed, 10 Aug 2022 01:25:20 GMT
EXPOSE 80
# Wed, 10 Aug 2022 01:25:20 GMT
VOLUME [/tmp]
# Wed, 10 Aug 2022 01:25:20 GMT
ENTRYPOINT ["/traefik"]
# Wed, 10 Aug 2022 01:25:20 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.34 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:dcf6dab73e17be4a506f9432554b84ca5af22b6ca8d3a28551e98fd1c05660dc`  
		Last Modified: Wed, 10 Aug 2022 01:26:26 GMT  
		Size: 123.5 KB (123538 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd04e95cb63652c8a3323efd5c36bdcf17166632bd5bbf9c5c72092392094ebb`  
		Last Modified: Wed, 10 Aug 2022 01:26:26 GMT  
		Size: 328.5 KB (328542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bc5ce073739868727c7f64505383cab253c15631bf675c2b65bb384d4ae4b1e`  
		Last Modified: Wed, 10 Aug 2022 01:26:30 GMT  
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
$ docker pull traefik@sha256:ee80ec61ce7968fa7680b289cc4e0cb29933f0d254c962f4ba94b87de29bbbe7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **20.6 MB (20583416 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:72b9e44203aa217fc68aff257b65b34390dec5720d4c89a2c3722476af10cdef`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Wed, 10 Aug 2022 06:11:29 GMT
COPY file:48964762d0c961c28f59ebd3ea194fb6486cf2bd9a9cf1780f6702d88bd7b7d9 in /etc/ssl/certs/ 
# Wed, 10 Aug 2022 06:11:30 GMT
COPY dir:a84372748b89eb90478bb1b120b7c8fff3112421d7f93e50fbeae3f53adc6788 in /usr/share/ 
# Wed, 10 Aug 2022 06:11:31 GMT
COPY file:60330593b6644f3f519fd13ce8ee34c2c7ab9994a1420afabbc01926dd1230dd in / 
# Wed, 10 Aug 2022 06:11:31 GMT
EXPOSE 80
# Wed, 10 Aug 2022 06:11:32 GMT
VOLUME [/tmp]
# Wed, 10 Aug 2022 06:11:33 GMT
ENTRYPOINT ["/traefik"]
# Wed, 10 Aug 2022 06:11:34 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.34 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:45ff194111b414e1aa5548434d84e56dbd11ebe2589d05ac6498a25d0e8adfcd`  
		Last Modified: Wed, 10 Aug 2022 06:13:02 GMT  
		Size: 123.5 KB (123544 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0a00cc3745cda02ead5281ab2de73712088f63bdf0bb2e31932d82d8d4c4236`  
		Last Modified: Wed, 10 Aug 2022 06:13:02 GMT  
		Size: 328.5 KB (328525 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c10648c89e22ebcc358eb0f5e84d1de66c1d49da6d460218007ffe19f65baafc`  
		Last Modified: Wed, 10 Aug 2022 06:13:05 GMT  
		Size: 20.1 MB (20131347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v1.7-alpine`

```console
$ docker pull traefik@sha256:a65ea31d38ab997c3ec977ca7e46192823ef829c298574e0365c1878f5e447f9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:v1.7-alpine` - linux; amd64

```console
$ docker pull traefik@sha256:fa0b479bcd6943cf3eee0f076f096253cd87d60eedbd550c5c46093f8a272aae
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.7 MB (25670985 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d93d266ccb4853b50019238b20d45befbbb64114d2780ee6582d87058faf9269`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Tue, 09 Aug 2022 17:20:07 GMT
ADD file:b9bd10cf83356cb7281baa0fbaca5186cf27491f59eda87abe57f83a5aaf5ec1 in / 
# Tue, 09 Aug 2022 17:20:08 GMT
CMD ["/bin/sh"]
# Wed, 10 Aug 2022 01:25:03 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 10 Aug 2022 01:25:09 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/traefik/traefik/releases/download/v1.7.34/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Wed, 10 Aug 2022 01:25:09 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 10 Aug 2022 01:25:10 GMT
EXPOSE 80
# Wed, 10 Aug 2022 01:25:10 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 10 Aug 2022 01:25:10 GMT
CMD ["traefik"]
# Wed, 10 Aug 2022 01:25:10 GMT
LABEL org.opencontainers.image.vendor=traefik org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.34 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:c7ed990a2339ee598662849de4f56e2241399f5a32340c8c4a7bbd5378a12b5f`  
		Last Modified: Tue, 09 Aug 2022 17:21:06 GMT  
		Size: 2.8 MB (2827489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d36b44d0cfa5b827ecf36e664752a4e5b8fc1a4f901a85763621072762da0045`  
		Last Modified: Wed, 10 Aug 2022 01:26:06 GMT  
		Size: 681.1 KB (681068 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b256a1bd7d5e289332916c16569dec3cdb78eb91cfe968dad1be3abaa6592a54`  
		Last Modified: Wed, 10 Aug 2022 01:26:10 GMT  
		Size: 22.2 MB (22162060 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b7ca5c826b27e2f48e1984235d4742a75652cd7682a0769fe815acabae80ddf`  
		Last Modified: Wed, 10 Aug 2022 01:26:06 GMT  
		Size: 368.0 B  
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
$ docker pull traefik@sha256:4164df484f4b6b89d809c899cefaae2bfd7962eacf756ca417989965c5783b28
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.5 MB (23536220 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8c6e41da4eded9e8dcedab7d754e6ea8327030df73dd4edc84cdc91ebcb8a95d`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Tue, 09 Aug 2022 17:39:59 GMT
ADD file:b312c8f512719efd09811d17c2b250bbad03cf3f90c135a00695cc8e152f4ee2 in / 
# Tue, 09 Aug 2022 17:39:59 GMT
CMD ["/bin/sh"]
# Wed, 10 Aug 2022 06:11:07 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 10 Aug 2022 06:11:14 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/traefik/traefik/releases/download/v1.7.34/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Wed, 10 Aug 2022 06:11:15 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 10 Aug 2022 06:11:15 GMT
EXPOSE 80
# Wed, 10 Aug 2022 06:11:16 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 10 Aug 2022 06:11:17 GMT
CMD ["traefik"]
# Wed, 10 Aug 2022 06:11:18 GMT
LABEL org.opencontainers.image.vendor=traefik org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.34 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:90cda3b7c32511829cd5ae9074240c36c34507085acb6e55b96f993740d2be93`  
		Last Modified: Tue, 09 Aug 2022 17:41:06 GMT  
		Size: 2.7 MB (2722153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed77a2aa4d354461d4394dcedb6b641f6298c516ba832a174652464a19b489f7`  
		Last Modified: Wed, 10 Aug 2022 06:12:39 GMT  
		Size: 682.3 KB (682314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3eb22d62b1873f7ed10c4ea0a5503cd0d75bddc18adbc0bb5ecd44e4e6ae9f50`  
		Last Modified: Wed, 10 Aug 2022 06:12:42 GMT  
		Size: 20.1 MB (20131384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2aedce2bbbad30ed9b4ae17a9bda0fff6ad652d205bd6d2a65ea86b8c33dddd`  
		Last Modified: Wed, 10 Aug 2022 06:12:39 GMT  
		Size: 369.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v1.7-windowsservercore-1809`

```console
$ docker pull traefik@sha256:0f10109d86f347d0326edc28ce65ac4f3d485e4e282b52505d9507e9da36b0c4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3287; amd64

### `traefik:v1.7-windowsservercore-1809` - windows version 10.0.17763.3287; amd64

```console
$ docker pull traefik@sha256:23182fb91cd4c2bd2311cf57479594893425702f0afc632520a6fc74b432e62c
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2700555687 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a756bb07a27a99c1a7997636266ee330bea763938462d1fda845abd62753ba8c`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Sat, 06 Aug 2022 18:30:32 GMT
RUN Install update 10.0.17763.3287
# Wed, 10 Aug 2022 12:16:16 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Aug 2022 19:22:52 GMT
RUN Invoke-WebRequest     -Uri "https://github.com/traefik/traefik/releases/download/v1.7.34/traefik_windows-amd64.exe"     -OutFile "/traefik.exe"
# Wed, 10 Aug 2022 19:22:53 GMT
EXPOSE 80
# Wed, 10 Aug 2022 19:22:54 GMT
ENTRYPOINT ["/traefik"]
# Wed, 10 Aug 2022 19:22:55 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.34 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:b111c3320c949bea81612bf4554f1b6592c2f504920b5bf57ba340a1d4d52c93`  
		Size: 1.9 GB (1877166088 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:294d77ac553d7210b662d07674ef9e39a6c2e88dc15b9d2788d51e509bc8b54e`  
		Size: 800.5 MB (800546641 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:d64f32398ff5e4ac4cbab317ffed87a2fbf4e4a37210284dba19f2929d631a95`  
		Last Modified: Wed, 10 Aug 2022 12:42:57 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bf2328c550caf93706630a4a6283a81124bce25f56889a67c42b6ea61409d06`  
		Last Modified: Wed, 10 Aug 2022 19:23:47 GMT  
		Size: 22.8 MB (22837223 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04c547d744d6ccc5c0fec076a7f15bd63ec8c73cb2027d023cf00cef0557cd6b`  
		Last Modified: Wed, 10 Aug 2022 19:23:41 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44e0ce1d03f2cd24f681a3b6038c2d11b03bdbf4ca8afe42f489f5c648788629`  
		Last Modified: Wed, 10 Aug 2022 19:23:41 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67d76a3107ed7e08ba9416baf4eb08e87395e64b4c9c4f0d728520f8164ca5a0`  
		Last Modified: Wed, 10 Aug 2022 19:23:42 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v1.7.34`

```console
$ docker pull traefik@sha256:bd12a7039c4736697cab4ee722d4f7683ee292b5b47b861a44a007a30c0581dd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:v1.7.34` - linux; amd64

```console
$ docker pull traefik@sha256:221d4ca433d21b148f21168a3c71aeb10d776f7d9051fb612b10be1d703f9c36
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **22.6 MB (22614032 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fd7cc9150335f309f34597c684d908b517b7aa428c550fa8f63dd1a19bafbfe4`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Wed, 10 Aug 2022 01:25:18 GMT
COPY file:48964762d0c961c28f59ebd3ea194fb6486cf2bd9a9cf1780f6702d88bd7b7d9 in /etc/ssl/certs/ 
# Wed, 10 Aug 2022 01:25:19 GMT
COPY dir:a84372748b89eb90478bb1b120b7c8fff3112421d7f93e50fbeae3f53adc6788 in /usr/share/ 
# Wed, 10 Aug 2022 01:25:20 GMT
COPY file:36217e5a6056bef26cfff395c8af8c1010a61dbe8d62b2c7869ca221e2a6302c in / 
# Wed, 10 Aug 2022 01:25:20 GMT
EXPOSE 80
# Wed, 10 Aug 2022 01:25:20 GMT
VOLUME [/tmp]
# Wed, 10 Aug 2022 01:25:20 GMT
ENTRYPOINT ["/traefik"]
# Wed, 10 Aug 2022 01:25:20 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.34 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:dcf6dab73e17be4a506f9432554b84ca5af22b6ca8d3a28551e98fd1c05660dc`  
		Last Modified: Wed, 10 Aug 2022 01:26:26 GMT  
		Size: 123.5 KB (123538 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd04e95cb63652c8a3323efd5c36bdcf17166632bd5bbf9c5c72092392094ebb`  
		Last Modified: Wed, 10 Aug 2022 01:26:26 GMT  
		Size: 328.5 KB (328542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bc5ce073739868727c7f64505383cab253c15631bf675c2b65bb384d4ae4b1e`  
		Last Modified: Wed, 10 Aug 2022 01:26:30 GMT  
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
$ docker pull traefik@sha256:ee80ec61ce7968fa7680b289cc4e0cb29933f0d254c962f4ba94b87de29bbbe7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **20.6 MB (20583416 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:72b9e44203aa217fc68aff257b65b34390dec5720d4c89a2c3722476af10cdef`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Wed, 10 Aug 2022 06:11:29 GMT
COPY file:48964762d0c961c28f59ebd3ea194fb6486cf2bd9a9cf1780f6702d88bd7b7d9 in /etc/ssl/certs/ 
# Wed, 10 Aug 2022 06:11:30 GMT
COPY dir:a84372748b89eb90478bb1b120b7c8fff3112421d7f93e50fbeae3f53adc6788 in /usr/share/ 
# Wed, 10 Aug 2022 06:11:31 GMT
COPY file:60330593b6644f3f519fd13ce8ee34c2c7ab9994a1420afabbc01926dd1230dd in / 
# Wed, 10 Aug 2022 06:11:31 GMT
EXPOSE 80
# Wed, 10 Aug 2022 06:11:32 GMT
VOLUME [/tmp]
# Wed, 10 Aug 2022 06:11:33 GMT
ENTRYPOINT ["/traefik"]
# Wed, 10 Aug 2022 06:11:34 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.34 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:45ff194111b414e1aa5548434d84e56dbd11ebe2589d05ac6498a25d0e8adfcd`  
		Last Modified: Wed, 10 Aug 2022 06:13:02 GMT  
		Size: 123.5 KB (123544 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0a00cc3745cda02ead5281ab2de73712088f63bdf0bb2e31932d82d8d4c4236`  
		Last Modified: Wed, 10 Aug 2022 06:13:02 GMT  
		Size: 328.5 KB (328525 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c10648c89e22ebcc358eb0f5e84d1de66c1d49da6d460218007ffe19f65baafc`  
		Last Modified: Wed, 10 Aug 2022 06:13:05 GMT  
		Size: 20.1 MB (20131347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v1.7.34-alpine`

```console
$ docker pull traefik@sha256:a65ea31d38ab997c3ec977ca7e46192823ef829c298574e0365c1878f5e447f9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:v1.7.34-alpine` - linux; amd64

```console
$ docker pull traefik@sha256:fa0b479bcd6943cf3eee0f076f096253cd87d60eedbd550c5c46093f8a272aae
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.7 MB (25670985 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d93d266ccb4853b50019238b20d45befbbb64114d2780ee6582d87058faf9269`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Tue, 09 Aug 2022 17:20:07 GMT
ADD file:b9bd10cf83356cb7281baa0fbaca5186cf27491f59eda87abe57f83a5aaf5ec1 in / 
# Tue, 09 Aug 2022 17:20:08 GMT
CMD ["/bin/sh"]
# Wed, 10 Aug 2022 01:25:03 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 10 Aug 2022 01:25:09 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/traefik/traefik/releases/download/v1.7.34/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Wed, 10 Aug 2022 01:25:09 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 10 Aug 2022 01:25:10 GMT
EXPOSE 80
# Wed, 10 Aug 2022 01:25:10 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 10 Aug 2022 01:25:10 GMT
CMD ["traefik"]
# Wed, 10 Aug 2022 01:25:10 GMT
LABEL org.opencontainers.image.vendor=traefik org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.34 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:c7ed990a2339ee598662849de4f56e2241399f5a32340c8c4a7bbd5378a12b5f`  
		Last Modified: Tue, 09 Aug 2022 17:21:06 GMT  
		Size: 2.8 MB (2827489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d36b44d0cfa5b827ecf36e664752a4e5b8fc1a4f901a85763621072762da0045`  
		Last Modified: Wed, 10 Aug 2022 01:26:06 GMT  
		Size: 681.1 KB (681068 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b256a1bd7d5e289332916c16569dec3cdb78eb91cfe968dad1be3abaa6592a54`  
		Last Modified: Wed, 10 Aug 2022 01:26:10 GMT  
		Size: 22.2 MB (22162060 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b7ca5c826b27e2f48e1984235d4742a75652cd7682a0769fe815acabae80ddf`  
		Last Modified: Wed, 10 Aug 2022 01:26:06 GMT  
		Size: 368.0 B  
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
$ docker pull traefik@sha256:4164df484f4b6b89d809c899cefaae2bfd7962eacf756ca417989965c5783b28
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.5 MB (23536220 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8c6e41da4eded9e8dcedab7d754e6ea8327030df73dd4edc84cdc91ebcb8a95d`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Tue, 09 Aug 2022 17:39:59 GMT
ADD file:b312c8f512719efd09811d17c2b250bbad03cf3f90c135a00695cc8e152f4ee2 in / 
# Tue, 09 Aug 2022 17:39:59 GMT
CMD ["/bin/sh"]
# Wed, 10 Aug 2022 06:11:07 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 10 Aug 2022 06:11:14 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/traefik/traefik/releases/download/v1.7.34/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Wed, 10 Aug 2022 06:11:15 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 10 Aug 2022 06:11:15 GMT
EXPOSE 80
# Wed, 10 Aug 2022 06:11:16 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 10 Aug 2022 06:11:17 GMT
CMD ["traefik"]
# Wed, 10 Aug 2022 06:11:18 GMT
LABEL org.opencontainers.image.vendor=traefik org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.34 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:90cda3b7c32511829cd5ae9074240c36c34507085acb6e55b96f993740d2be93`  
		Last Modified: Tue, 09 Aug 2022 17:41:06 GMT  
		Size: 2.7 MB (2722153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed77a2aa4d354461d4394dcedb6b641f6298c516ba832a174652464a19b489f7`  
		Last Modified: Wed, 10 Aug 2022 06:12:39 GMT  
		Size: 682.3 KB (682314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3eb22d62b1873f7ed10c4ea0a5503cd0d75bddc18adbc0bb5ecd44e4e6ae9f50`  
		Last Modified: Wed, 10 Aug 2022 06:12:42 GMT  
		Size: 20.1 MB (20131384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2aedce2bbbad30ed9b4ae17a9bda0fff6ad652d205bd6d2a65ea86b8c33dddd`  
		Last Modified: Wed, 10 Aug 2022 06:12:39 GMT  
		Size: 369.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v1.7.34-windowsservercore-1809`

```console
$ docker pull traefik@sha256:0f10109d86f347d0326edc28ce65ac4f3d485e4e282b52505d9507e9da36b0c4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3287; amd64

### `traefik:v1.7.34-windowsservercore-1809` - windows version 10.0.17763.3287; amd64

```console
$ docker pull traefik@sha256:23182fb91cd4c2bd2311cf57479594893425702f0afc632520a6fc74b432e62c
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2700555687 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a756bb07a27a99c1a7997636266ee330bea763938462d1fda845abd62753ba8c`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Sat, 06 Aug 2022 18:30:32 GMT
RUN Install update 10.0.17763.3287
# Wed, 10 Aug 2022 12:16:16 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Aug 2022 19:22:52 GMT
RUN Invoke-WebRequest     -Uri "https://github.com/traefik/traefik/releases/download/v1.7.34/traefik_windows-amd64.exe"     -OutFile "/traefik.exe"
# Wed, 10 Aug 2022 19:22:53 GMT
EXPOSE 80
# Wed, 10 Aug 2022 19:22:54 GMT
ENTRYPOINT ["/traefik"]
# Wed, 10 Aug 2022 19:22:55 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.34 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:b111c3320c949bea81612bf4554f1b6592c2f504920b5bf57ba340a1d4d52c93`  
		Size: 1.9 GB (1877166088 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:294d77ac553d7210b662d07674ef9e39a6c2e88dc15b9d2788d51e509bc8b54e`  
		Size: 800.5 MB (800546641 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:d64f32398ff5e4ac4cbab317ffed87a2fbf4e4a37210284dba19f2929d631a95`  
		Last Modified: Wed, 10 Aug 2022 12:42:57 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bf2328c550caf93706630a4a6283a81124bce25f56889a67c42b6ea61409d06`  
		Last Modified: Wed, 10 Aug 2022 19:23:47 GMT  
		Size: 22.8 MB (22837223 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04c547d744d6ccc5c0fec076a7f15bd63ec8c73cb2027d023cf00cef0557cd6b`  
		Last Modified: Wed, 10 Aug 2022 19:23:41 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44e0ce1d03f2cd24f681a3b6038c2d11b03bdbf4ca8afe42f489f5c648788629`  
		Last Modified: Wed, 10 Aug 2022 19:23:41 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67d76a3107ed7e08ba9416baf4eb08e87395e64b4c9c4f0d728520f8164ca5a0`  
		Last Modified: Wed, 10 Aug 2022 19:23:42 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v2.8`

```console
$ docker pull traefik@sha256:9717bde18a6e109c63a88e4b67725500c701768d7c044fc64c83efdb892b5738
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; s390x

### `traefik:v2.8` - linux; amd64

```console
$ docker pull traefik@sha256:c0ee1d98d82d145d449d468c9f7cecf099c224b0efa23d72f8d976548dc6ff98
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.3 MB (33280383 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9d00af07cc7c91c3470ab5fb46d2caef28f984d258f110f77a7cd2b148fc93b4`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Tue, 09 Aug 2022 17:20:00 GMT
ADD file:f77e3f51f020890d22997e6c2ca98968b75b8bc8c463341a2010ff0655d4c88f in / 
# Tue, 09 Aug 2022 17:20:01 GMT
CMD ["/bin/sh"]
# Wed, 10 Aug 2022 01:24:52 GMT
RUN apk --no-cache add ca-certificates tzdata
# Fri, 02 Sep 2022 20:50:13 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.8.4/traefik_v2.8.4_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Fri, 02 Sep 2022 20:50:14 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Fri, 02 Sep 2022 20:50:14 GMT
EXPOSE 80
# Fri, 02 Sep 2022 20:50:14 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 02 Sep 2022 20:50:14 GMT
CMD ["traefik"]
# Fri, 02 Sep 2022 20:50:14 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.8.4 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:9621f1afde84053b2f9b6ff34fc7f7460712247c01cbab483c5fa7132cf782ca`  
		Last Modified: Tue, 09 Aug 2022 17:20:52 GMT  
		Size: 2.8 MB (2823512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0448c16748457249205ca0475f796fa6c4661fdcbf2d618c5241bdf9c4b12f9a`  
		Last Modified: Wed, 10 Aug 2022 01:25:43 GMT  
		Size: 681.7 KB (681674 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4b54ed04da5e95dc580e80f0518e3c13b776377f5404327988acec675e499ab`  
		Last Modified: Fri, 02 Sep 2022 20:50:44 GMT  
		Size: 29.8 MB (29774829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9447aa44267fb53387d49c2e1fc049f08581306fca07488baab643e3f559d90b`  
		Last Modified: Fri, 02 Sep 2022 20:50:39 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v2.8` - linux; arm variant v6

```console
$ docker pull traefik@sha256:524dea2468148d17e36e8685b1ae6bb8b32fc824dc67d9ae0d006f78c205c9ba
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.4 MB (31406635 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a470b476d302ab7cd2965d189b989a1ebeafc3b3f51c3fc9a3f7352590ad8c75`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Tue, 09 Aug 2022 17:49:29 GMT
ADD file:89cb25f97e17bed5c56311280efe5cfa78422d8ffbe36232195d13f94d67417e in / 
# Tue, 09 Aug 2022 17:49:29 GMT
CMD ["/bin/sh"]
# Thu, 11 Aug 2022 01:14:12 GMT
RUN apk --no-cache add ca-certificates tzdata
# Fri, 02 Sep 2022 19:49:39 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.8.4/traefik_v2.8.4_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Fri, 02 Sep 2022 19:49:39 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Fri, 02 Sep 2022 19:49:39 GMT
EXPOSE 80
# Fri, 02 Sep 2022 19:49:39 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 02 Sep 2022 19:49:39 GMT
CMD ["traefik"]
# Fri, 02 Sep 2022 19:49:40 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.8.4 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:2184ddf72fafdec856907308b0832d0cb9fa3f18d27bc8923d31bf537000722a`  
		Last Modified: Fri, 02 Sep 2022 19:50:45 GMT  
		Size: 28.1 MB (28089099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70bab47ff3f98940f7fa7d3eb55a81c68ba899a88b3b57e7e2ff3574eb5c2ca5`  
		Last Modified: Fri, 02 Sep 2022 19:50:39 GMT  
		Size: 367.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v2.8` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:3af1ee8b3fff09a9e7bc958150245c14eebf6910fee151320b716a0ce0278b80
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.6 MB (30575438 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:148847c384149af925afcbbf2a63d3d9537e1c3e0e3fc4778ce849c30fc414a9`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Tue, 09 Aug 2022 17:39:51 GMT
ADD file:4b51a9d40f20d2beb29d0759b161d2b9403493453beb509de4e86a5d98513f16 in / 
# Tue, 09 Aug 2022 17:39:51 GMT
CMD ["/bin/sh"]
# Wed, 10 Aug 2022 06:10:52 GMT
RUN apk --no-cache add ca-certificates tzdata
# Fri, 02 Sep 2022 21:02:06 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.8.4/traefik_v2.8.4_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Fri, 02 Sep 2022 21:02:08 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Fri, 02 Sep 2022 21:02:08 GMT
EXPOSE 80
# Fri, 02 Sep 2022 21:02:09 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 02 Sep 2022 21:02:10 GMT
CMD ["traefik"]
# Fri, 02 Sep 2022 21:02:11 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.8.4 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:47517142f6ba87eca6b7bdca1e0df160b74671c81e4b9605dad38c1862a43be3`  
		Last Modified: Tue, 09 Aug 2022 17:40:55 GMT  
		Size: 2.7 MB (2718439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:966c95a60d9885fe2865b5aef2abf3c8e02dbfcd48f4b9978e47205d35c9a2c1`  
		Last Modified: Wed, 10 Aug 2022 06:12:12 GMT  
		Size: 682.4 KB (682395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97c489cee492d2fe706c61d150982ab2113f63f0b0325eecfcc529c715a025de`  
		Last Modified: Fri, 02 Sep 2022 21:03:03 GMT  
		Size: 27.2 MB (27174235 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb23e7c7b06001a1723b46152cba68a658ef913e0fcd9ce6a675782ee6e91153`  
		Last Modified: Fri, 02 Sep 2022 21:02:58 GMT  
		Size: 369.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v2.8` - linux; s390x

```console
$ docker pull traefik@sha256:0ae44e1db4e8692764f89bc9c6713b5a8f2454a49fb958670f1ce097d771f2d4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.0 MB (31970417 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:907601fe3e786e8291296b20b082a843538ba24e2cb77764166e496ec811d23f`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Tue, 09 Aug 2022 17:41:54 GMT
ADD file:7489fa84133e97e4f40b13dd5159989b3594c9627d9147bfc4e33134944cc368 in / 
# Tue, 09 Aug 2022 17:41:54 GMT
CMD ["/bin/sh"]
# Wed, 10 Aug 2022 05:50:07 GMT
RUN apk --no-cache add ca-certificates tzdata
# Fri, 02 Sep 2022 21:18:57 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.8.4/traefik_v2.8.4_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Fri, 02 Sep 2022 21:19:02 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Fri, 02 Sep 2022 21:19:03 GMT
EXPOSE 80
# Fri, 02 Sep 2022 21:19:03 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 02 Sep 2022 21:19:04 GMT
CMD ["traefik"]
# Fri, 02 Sep 2022 21:19:05 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.8.4 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:cdf710f5b7ee39c5124c50c753228dc9b8b1c1c0a1a38f1413487548565445c3`  
		Last Modified: Tue, 09 Aug 2022 17:42:56 GMT  
		Size: 2.6 MB (2606087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d94fe8753c6b15e6f67f3ca19edd0d0c2c0d8f6596878b0a6e212d71d3ae470d`  
		Last Modified: Wed, 10 Aug 2022 05:50:57 GMT  
		Size: 686.5 KB (686528 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a7fc896b96c1b9c8a8c7d6ab0cec469b6114d366b8cc7732f19d5913ad818d1`  
		Last Modified: Fri, 02 Sep 2022 21:19:39 GMT  
		Size: 28.7 MB (28677434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ba0189892c09ebd907a8f9e1885c492cd37742dd2d614b034515e31dda3ec17`  
		Last Modified: Fri, 02 Sep 2022 21:19:34 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v2.8-windowsservercore-1809`

```console
$ docker pull traefik@sha256:e21df88b973943eb3d1fb6882f9aa8f1bfb76f5c91ca24d86b18bbc05814d23f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3287; amd64

### `traefik:v2.8-windowsservercore-1809` - windows version 10.0.17763.3287; amd64

```console
$ docker pull traefik@sha256:888c8204cbe36566704c0ff5d27aaba93ddda7fb8705077d813c3776f3720fb7
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2707978103 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:16fe5cbe222e4fdaa4f0280fbb0c434f102b72aadc7759f356eaa9eb475401e1`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Sat, 06 Aug 2022 18:30:32 GMT
RUN Install update 10.0.17763.3287
# Wed, 10 Aug 2022 12:16:16 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Fri, 02 Sep 2022 20:16:28 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/traefik/traefik/releases/download/v2.8.4/traefik_v2.8.4_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Fri, 02 Sep 2022 20:16:29 GMT
EXPOSE 80
# Fri, 02 Sep 2022 20:16:30 GMT
ENTRYPOINT ["/traefik"]
# Fri, 02 Sep 2022 20:16:31 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.8.4 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:b111c3320c949bea81612bf4554f1b6592c2f504920b5bf57ba340a1d4d52c93`  
		Size: 1.9 GB (1877166088 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:294d77ac553d7210b662d07674ef9e39a6c2e88dc15b9d2788d51e509bc8b54e`  
		Size: 800.5 MB (800546641 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:d64f32398ff5e4ac4cbab317ffed87a2fbf4e4a37210284dba19f2929d631a95`  
		Last Modified: Wed, 10 Aug 2022 12:42:57 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0313b7cb0203c87fdae2ed13c632236f1787bce1ad528657ed30a38ddbf5235`  
		Last Modified: Fri, 02 Sep 2022 20:17:11 GMT  
		Size: 30.3 MB (30259693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be311a3bfd74b89aba7388644de2836f16ccd492641301a25dc40a8d95bdcf1c`  
		Last Modified: Fri, 02 Sep 2022 20:17:05 GMT  
		Size: 1.4 KB (1389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81354628ab86c777160694d48d5d428248dff2d7621fc494da604be40c91e403`  
		Last Modified: Fri, 02 Sep 2022 20:17:05 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8c2a232471cae5193369cbc619007f710b7ea681e38f34a91f7a19213940d82`  
		Last Modified: Fri, 02 Sep 2022 20:17:05 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v2.8.4`

```console
$ docker pull traefik@sha256:9717bde18a6e109c63a88e4b67725500c701768d7c044fc64c83efdb892b5738
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; s390x

### `traefik:v2.8.4` - linux; amd64

```console
$ docker pull traefik@sha256:c0ee1d98d82d145d449d468c9f7cecf099c224b0efa23d72f8d976548dc6ff98
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.3 MB (33280383 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9d00af07cc7c91c3470ab5fb46d2caef28f984d258f110f77a7cd2b148fc93b4`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Tue, 09 Aug 2022 17:20:00 GMT
ADD file:f77e3f51f020890d22997e6c2ca98968b75b8bc8c463341a2010ff0655d4c88f in / 
# Tue, 09 Aug 2022 17:20:01 GMT
CMD ["/bin/sh"]
# Wed, 10 Aug 2022 01:24:52 GMT
RUN apk --no-cache add ca-certificates tzdata
# Fri, 02 Sep 2022 20:50:13 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.8.4/traefik_v2.8.4_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Fri, 02 Sep 2022 20:50:14 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Fri, 02 Sep 2022 20:50:14 GMT
EXPOSE 80
# Fri, 02 Sep 2022 20:50:14 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 02 Sep 2022 20:50:14 GMT
CMD ["traefik"]
# Fri, 02 Sep 2022 20:50:14 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.8.4 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:9621f1afde84053b2f9b6ff34fc7f7460712247c01cbab483c5fa7132cf782ca`  
		Last Modified: Tue, 09 Aug 2022 17:20:52 GMT  
		Size: 2.8 MB (2823512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0448c16748457249205ca0475f796fa6c4661fdcbf2d618c5241bdf9c4b12f9a`  
		Last Modified: Wed, 10 Aug 2022 01:25:43 GMT  
		Size: 681.7 KB (681674 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4b54ed04da5e95dc580e80f0518e3c13b776377f5404327988acec675e499ab`  
		Last Modified: Fri, 02 Sep 2022 20:50:44 GMT  
		Size: 29.8 MB (29774829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9447aa44267fb53387d49c2e1fc049f08581306fca07488baab643e3f559d90b`  
		Last Modified: Fri, 02 Sep 2022 20:50:39 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v2.8.4` - linux; arm variant v6

```console
$ docker pull traefik@sha256:524dea2468148d17e36e8685b1ae6bb8b32fc824dc67d9ae0d006f78c205c9ba
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.4 MB (31406635 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a470b476d302ab7cd2965d189b989a1ebeafc3b3f51c3fc9a3f7352590ad8c75`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Tue, 09 Aug 2022 17:49:29 GMT
ADD file:89cb25f97e17bed5c56311280efe5cfa78422d8ffbe36232195d13f94d67417e in / 
# Tue, 09 Aug 2022 17:49:29 GMT
CMD ["/bin/sh"]
# Thu, 11 Aug 2022 01:14:12 GMT
RUN apk --no-cache add ca-certificates tzdata
# Fri, 02 Sep 2022 19:49:39 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.8.4/traefik_v2.8.4_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Fri, 02 Sep 2022 19:49:39 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Fri, 02 Sep 2022 19:49:39 GMT
EXPOSE 80
# Fri, 02 Sep 2022 19:49:39 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 02 Sep 2022 19:49:39 GMT
CMD ["traefik"]
# Fri, 02 Sep 2022 19:49:40 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.8.4 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:2184ddf72fafdec856907308b0832d0cb9fa3f18d27bc8923d31bf537000722a`  
		Last Modified: Fri, 02 Sep 2022 19:50:45 GMT  
		Size: 28.1 MB (28089099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70bab47ff3f98940f7fa7d3eb55a81c68ba899a88b3b57e7e2ff3574eb5c2ca5`  
		Last Modified: Fri, 02 Sep 2022 19:50:39 GMT  
		Size: 367.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v2.8.4` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:3af1ee8b3fff09a9e7bc958150245c14eebf6910fee151320b716a0ce0278b80
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.6 MB (30575438 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:148847c384149af925afcbbf2a63d3d9537e1c3e0e3fc4778ce849c30fc414a9`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Tue, 09 Aug 2022 17:39:51 GMT
ADD file:4b51a9d40f20d2beb29d0759b161d2b9403493453beb509de4e86a5d98513f16 in / 
# Tue, 09 Aug 2022 17:39:51 GMT
CMD ["/bin/sh"]
# Wed, 10 Aug 2022 06:10:52 GMT
RUN apk --no-cache add ca-certificates tzdata
# Fri, 02 Sep 2022 21:02:06 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.8.4/traefik_v2.8.4_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Fri, 02 Sep 2022 21:02:08 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Fri, 02 Sep 2022 21:02:08 GMT
EXPOSE 80
# Fri, 02 Sep 2022 21:02:09 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 02 Sep 2022 21:02:10 GMT
CMD ["traefik"]
# Fri, 02 Sep 2022 21:02:11 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.8.4 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:47517142f6ba87eca6b7bdca1e0df160b74671c81e4b9605dad38c1862a43be3`  
		Last Modified: Tue, 09 Aug 2022 17:40:55 GMT  
		Size: 2.7 MB (2718439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:966c95a60d9885fe2865b5aef2abf3c8e02dbfcd48f4b9978e47205d35c9a2c1`  
		Last Modified: Wed, 10 Aug 2022 06:12:12 GMT  
		Size: 682.4 KB (682395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97c489cee492d2fe706c61d150982ab2113f63f0b0325eecfcc529c715a025de`  
		Last Modified: Fri, 02 Sep 2022 21:03:03 GMT  
		Size: 27.2 MB (27174235 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb23e7c7b06001a1723b46152cba68a658ef913e0fcd9ce6a675782ee6e91153`  
		Last Modified: Fri, 02 Sep 2022 21:02:58 GMT  
		Size: 369.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v2.8.4` - linux; s390x

```console
$ docker pull traefik@sha256:0ae44e1db4e8692764f89bc9c6713b5a8f2454a49fb958670f1ce097d771f2d4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.0 MB (31970417 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:907601fe3e786e8291296b20b082a843538ba24e2cb77764166e496ec811d23f`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Tue, 09 Aug 2022 17:41:54 GMT
ADD file:7489fa84133e97e4f40b13dd5159989b3594c9627d9147bfc4e33134944cc368 in / 
# Tue, 09 Aug 2022 17:41:54 GMT
CMD ["/bin/sh"]
# Wed, 10 Aug 2022 05:50:07 GMT
RUN apk --no-cache add ca-certificates tzdata
# Fri, 02 Sep 2022 21:18:57 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.8.4/traefik_v2.8.4_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Fri, 02 Sep 2022 21:19:02 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Fri, 02 Sep 2022 21:19:03 GMT
EXPOSE 80
# Fri, 02 Sep 2022 21:19:03 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 02 Sep 2022 21:19:04 GMT
CMD ["traefik"]
# Fri, 02 Sep 2022 21:19:05 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.8.4 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:cdf710f5b7ee39c5124c50c753228dc9b8b1c1c0a1a38f1413487548565445c3`  
		Last Modified: Tue, 09 Aug 2022 17:42:56 GMT  
		Size: 2.6 MB (2606087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d94fe8753c6b15e6f67f3ca19edd0d0c2c0d8f6596878b0a6e212d71d3ae470d`  
		Last Modified: Wed, 10 Aug 2022 05:50:57 GMT  
		Size: 686.5 KB (686528 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a7fc896b96c1b9c8a8c7d6ab0cec469b6114d366b8cc7732f19d5913ad818d1`  
		Last Modified: Fri, 02 Sep 2022 21:19:39 GMT  
		Size: 28.7 MB (28677434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ba0189892c09ebd907a8f9e1885c492cd37742dd2d614b034515e31dda3ec17`  
		Last Modified: Fri, 02 Sep 2022 21:19:34 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v2.8.4-windowsservercore-1809`

```console
$ docker pull traefik@sha256:e21df88b973943eb3d1fb6882f9aa8f1bfb76f5c91ca24d86b18bbc05814d23f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3287; amd64

### `traefik:v2.8.4-windowsservercore-1809` - windows version 10.0.17763.3287; amd64

```console
$ docker pull traefik@sha256:888c8204cbe36566704c0ff5d27aaba93ddda7fb8705077d813c3776f3720fb7
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2707978103 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:16fe5cbe222e4fdaa4f0280fbb0c434f102b72aadc7759f356eaa9eb475401e1`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Sat, 06 Aug 2022 18:30:32 GMT
RUN Install update 10.0.17763.3287
# Wed, 10 Aug 2022 12:16:16 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Fri, 02 Sep 2022 20:16:28 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/traefik/traefik/releases/download/v2.8.4/traefik_v2.8.4_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Fri, 02 Sep 2022 20:16:29 GMT
EXPOSE 80
# Fri, 02 Sep 2022 20:16:30 GMT
ENTRYPOINT ["/traefik"]
# Fri, 02 Sep 2022 20:16:31 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.8.4 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:b111c3320c949bea81612bf4554f1b6592c2f504920b5bf57ba340a1d4d52c93`  
		Size: 1.9 GB (1877166088 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:294d77ac553d7210b662d07674ef9e39a6c2e88dc15b9d2788d51e509bc8b54e`  
		Size: 800.5 MB (800546641 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:d64f32398ff5e4ac4cbab317ffed87a2fbf4e4a37210284dba19f2929d631a95`  
		Last Modified: Wed, 10 Aug 2022 12:42:57 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0313b7cb0203c87fdae2ed13c632236f1787bce1ad528657ed30a38ddbf5235`  
		Last Modified: Fri, 02 Sep 2022 20:17:11 GMT  
		Size: 30.3 MB (30259693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be311a3bfd74b89aba7388644de2836f16ccd492641301a25dc40a8d95bdcf1c`  
		Last Modified: Fri, 02 Sep 2022 20:17:05 GMT  
		Size: 1.4 KB (1389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81354628ab86c777160694d48d5d428248dff2d7621fc494da604be40c91e403`  
		Last Modified: Fri, 02 Sep 2022 20:17:05 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8c2a232471cae5193369cbc619007f710b7ea681e38f34a91f7a19213940d82`  
		Last Modified: Fri, 02 Sep 2022 20:17:05 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:vacherin`

```console
$ docker pull traefik@sha256:9717bde18a6e109c63a88e4b67725500c701768d7c044fc64c83efdb892b5738
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; s390x

### `traefik:vacherin` - linux; amd64

```console
$ docker pull traefik@sha256:c0ee1d98d82d145d449d468c9f7cecf099c224b0efa23d72f8d976548dc6ff98
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.3 MB (33280383 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9d00af07cc7c91c3470ab5fb46d2caef28f984d258f110f77a7cd2b148fc93b4`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Tue, 09 Aug 2022 17:20:00 GMT
ADD file:f77e3f51f020890d22997e6c2ca98968b75b8bc8c463341a2010ff0655d4c88f in / 
# Tue, 09 Aug 2022 17:20:01 GMT
CMD ["/bin/sh"]
# Wed, 10 Aug 2022 01:24:52 GMT
RUN apk --no-cache add ca-certificates tzdata
# Fri, 02 Sep 2022 20:50:13 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.8.4/traefik_v2.8.4_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Fri, 02 Sep 2022 20:50:14 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Fri, 02 Sep 2022 20:50:14 GMT
EXPOSE 80
# Fri, 02 Sep 2022 20:50:14 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 02 Sep 2022 20:50:14 GMT
CMD ["traefik"]
# Fri, 02 Sep 2022 20:50:14 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.8.4 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:9621f1afde84053b2f9b6ff34fc7f7460712247c01cbab483c5fa7132cf782ca`  
		Last Modified: Tue, 09 Aug 2022 17:20:52 GMT  
		Size: 2.8 MB (2823512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0448c16748457249205ca0475f796fa6c4661fdcbf2d618c5241bdf9c4b12f9a`  
		Last Modified: Wed, 10 Aug 2022 01:25:43 GMT  
		Size: 681.7 KB (681674 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4b54ed04da5e95dc580e80f0518e3c13b776377f5404327988acec675e499ab`  
		Last Modified: Fri, 02 Sep 2022 20:50:44 GMT  
		Size: 29.8 MB (29774829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9447aa44267fb53387d49c2e1fc049f08581306fca07488baab643e3f559d90b`  
		Last Modified: Fri, 02 Sep 2022 20:50:39 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:vacherin` - linux; arm variant v6

```console
$ docker pull traefik@sha256:524dea2468148d17e36e8685b1ae6bb8b32fc824dc67d9ae0d006f78c205c9ba
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.4 MB (31406635 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a470b476d302ab7cd2965d189b989a1ebeafc3b3f51c3fc9a3f7352590ad8c75`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Tue, 09 Aug 2022 17:49:29 GMT
ADD file:89cb25f97e17bed5c56311280efe5cfa78422d8ffbe36232195d13f94d67417e in / 
# Tue, 09 Aug 2022 17:49:29 GMT
CMD ["/bin/sh"]
# Thu, 11 Aug 2022 01:14:12 GMT
RUN apk --no-cache add ca-certificates tzdata
# Fri, 02 Sep 2022 19:49:39 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.8.4/traefik_v2.8.4_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Fri, 02 Sep 2022 19:49:39 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Fri, 02 Sep 2022 19:49:39 GMT
EXPOSE 80
# Fri, 02 Sep 2022 19:49:39 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 02 Sep 2022 19:49:39 GMT
CMD ["traefik"]
# Fri, 02 Sep 2022 19:49:40 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.8.4 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:2184ddf72fafdec856907308b0832d0cb9fa3f18d27bc8923d31bf537000722a`  
		Last Modified: Fri, 02 Sep 2022 19:50:45 GMT  
		Size: 28.1 MB (28089099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70bab47ff3f98940f7fa7d3eb55a81c68ba899a88b3b57e7e2ff3574eb5c2ca5`  
		Last Modified: Fri, 02 Sep 2022 19:50:39 GMT  
		Size: 367.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:vacherin` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:3af1ee8b3fff09a9e7bc958150245c14eebf6910fee151320b716a0ce0278b80
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.6 MB (30575438 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:148847c384149af925afcbbf2a63d3d9537e1c3e0e3fc4778ce849c30fc414a9`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Tue, 09 Aug 2022 17:39:51 GMT
ADD file:4b51a9d40f20d2beb29d0759b161d2b9403493453beb509de4e86a5d98513f16 in / 
# Tue, 09 Aug 2022 17:39:51 GMT
CMD ["/bin/sh"]
# Wed, 10 Aug 2022 06:10:52 GMT
RUN apk --no-cache add ca-certificates tzdata
# Fri, 02 Sep 2022 21:02:06 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.8.4/traefik_v2.8.4_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Fri, 02 Sep 2022 21:02:08 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Fri, 02 Sep 2022 21:02:08 GMT
EXPOSE 80
# Fri, 02 Sep 2022 21:02:09 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 02 Sep 2022 21:02:10 GMT
CMD ["traefik"]
# Fri, 02 Sep 2022 21:02:11 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.8.4 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:47517142f6ba87eca6b7bdca1e0df160b74671c81e4b9605dad38c1862a43be3`  
		Last Modified: Tue, 09 Aug 2022 17:40:55 GMT  
		Size: 2.7 MB (2718439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:966c95a60d9885fe2865b5aef2abf3c8e02dbfcd48f4b9978e47205d35c9a2c1`  
		Last Modified: Wed, 10 Aug 2022 06:12:12 GMT  
		Size: 682.4 KB (682395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97c489cee492d2fe706c61d150982ab2113f63f0b0325eecfcc529c715a025de`  
		Last Modified: Fri, 02 Sep 2022 21:03:03 GMT  
		Size: 27.2 MB (27174235 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb23e7c7b06001a1723b46152cba68a658ef913e0fcd9ce6a675782ee6e91153`  
		Last Modified: Fri, 02 Sep 2022 21:02:58 GMT  
		Size: 369.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:vacherin` - linux; s390x

```console
$ docker pull traefik@sha256:0ae44e1db4e8692764f89bc9c6713b5a8f2454a49fb958670f1ce097d771f2d4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.0 MB (31970417 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:907601fe3e786e8291296b20b082a843538ba24e2cb77764166e496ec811d23f`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Tue, 09 Aug 2022 17:41:54 GMT
ADD file:7489fa84133e97e4f40b13dd5159989b3594c9627d9147bfc4e33134944cc368 in / 
# Tue, 09 Aug 2022 17:41:54 GMT
CMD ["/bin/sh"]
# Wed, 10 Aug 2022 05:50:07 GMT
RUN apk --no-cache add ca-certificates tzdata
# Fri, 02 Sep 2022 21:18:57 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.8.4/traefik_v2.8.4_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Fri, 02 Sep 2022 21:19:02 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Fri, 02 Sep 2022 21:19:03 GMT
EXPOSE 80
# Fri, 02 Sep 2022 21:19:03 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 02 Sep 2022 21:19:04 GMT
CMD ["traefik"]
# Fri, 02 Sep 2022 21:19:05 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.8.4 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:cdf710f5b7ee39c5124c50c753228dc9b8b1c1c0a1a38f1413487548565445c3`  
		Last Modified: Tue, 09 Aug 2022 17:42:56 GMT  
		Size: 2.6 MB (2606087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d94fe8753c6b15e6f67f3ca19edd0d0c2c0d8f6596878b0a6e212d71d3ae470d`  
		Last Modified: Wed, 10 Aug 2022 05:50:57 GMT  
		Size: 686.5 KB (686528 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a7fc896b96c1b9c8a8c7d6ab0cec469b6114d366b8cc7732f19d5913ad818d1`  
		Last Modified: Fri, 02 Sep 2022 21:19:39 GMT  
		Size: 28.7 MB (28677434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ba0189892c09ebd907a8f9e1885c492cd37742dd2d614b034515e31dda3ec17`  
		Last Modified: Fri, 02 Sep 2022 21:19:34 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:vacherin-windowsservercore-1809`

```console
$ docker pull traefik@sha256:e21df88b973943eb3d1fb6882f9aa8f1bfb76f5c91ca24d86b18bbc05814d23f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3287; amd64

### `traefik:vacherin-windowsservercore-1809` - windows version 10.0.17763.3287; amd64

```console
$ docker pull traefik@sha256:888c8204cbe36566704c0ff5d27aaba93ddda7fb8705077d813c3776f3720fb7
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2707978103 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:16fe5cbe222e4fdaa4f0280fbb0c434f102b72aadc7759f356eaa9eb475401e1`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Sat, 06 Aug 2022 18:30:32 GMT
RUN Install update 10.0.17763.3287
# Wed, 10 Aug 2022 12:16:16 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Fri, 02 Sep 2022 20:16:28 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/traefik/traefik/releases/download/v2.8.4/traefik_v2.8.4_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Fri, 02 Sep 2022 20:16:29 GMT
EXPOSE 80
# Fri, 02 Sep 2022 20:16:30 GMT
ENTRYPOINT ["/traefik"]
# Fri, 02 Sep 2022 20:16:31 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.8.4 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:b111c3320c949bea81612bf4554f1b6592c2f504920b5bf57ba340a1d4d52c93`  
		Size: 1.9 GB (1877166088 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:294d77ac553d7210b662d07674ef9e39a6c2e88dc15b9d2788d51e509bc8b54e`  
		Size: 800.5 MB (800546641 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:d64f32398ff5e4ac4cbab317ffed87a2fbf4e4a37210284dba19f2929d631a95`  
		Last Modified: Wed, 10 Aug 2022 12:42:57 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0313b7cb0203c87fdae2ed13c632236f1787bce1ad528657ed30a38ddbf5235`  
		Last Modified: Fri, 02 Sep 2022 20:17:11 GMT  
		Size: 30.3 MB (30259693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be311a3bfd74b89aba7388644de2836f16ccd492641301a25dc40a8d95bdcf1c`  
		Last Modified: Fri, 02 Sep 2022 20:17:05 GMT  
		Size: 1.4 KB (1389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81354628ab86c777160694d48d5d428248dff2d7621fc494da604be40c91e403`  
		Last Modified: Fri, 02 Sep 2022 20:17:05 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8c2a232471cae5193369cbc619007f710b7ea681e38f34a91f7a19213940d82`  
		Last Modified: Fri, 02 Sep 2022 20:17:05 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:windowsservercore-1809`

```console
$ docker pull traefik@sha256:e21df88b973943eb3d1fb6882f9aa8f1bfb76f5c91ca24d86b18bbc05814d23f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3287; amd64

### `traefik:windowsservercore-1809` - windows version 10.0.17763.3287; amd64

```console
$ docker pull traefik@sha256:888c8204cbe36566704c0ff5d27aaba93ddda7fb8705077d813c3776f3720fb7
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2707978103 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:16fe5cbe222e4fdaa4f0280fbb0c434f102b72aadc7759f356eaa9eb475401e1`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Sat, 06 Aug 2022 18:30:32 GMT
RUN Install update 10.0.17763.3287
# Wed, 10 Aug 2022 12:16:16 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Fri, 02 Sep 2022 20:16:28 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/traefik/traefik/releases/download/v2.8.4/traefik_v2.8.4_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Fri, 02 Sep 2022 20:16:29 GMT
EXPOSE 80
# Fri, 02 Sep 2022 20:16:30 GMT
ENTRYPOINT ["/traefik"]
# Fri, 02 Sep 2022 20:16:31 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.8.4 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:b111c3320c949bea81612bf4554f1b6592c2f504920b5bf57ba340a1d4d52c93`  
		Size: 1.9 GB (1877166088 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:294d77ac553d7210b662d07674ef9e39a6c2e88dc15b9d2788d51e509bc8b54e`  
		Size: 800.5 MB (800546641 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:d64f32398ff5e4ac4cbab317ffed87a2fbf4e4a37210284dba19f2929d631a95`  
		Last Modified: Wed, 10 Aug 2022 12:42:57 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0313b7cb0203c87fdae2ed13c632236f1787bce1ad528657ed30a38ddbf5235`  
		Last Modified: Fri, 02 Sep 2022 20:17:11 GMT  
		Size: 30.3 MB (30259693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be311a3bfd74b89aba7388644de2836f16ccd492641301a25dc40a8d95bdcf1c`  
		Last Modified: Fri, 02 Sep 2022 20:17:05 GMT  
		Size: 1.4 KB (1389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81354628ab86c777160694d48d5d428248dff2d7621fc494da604be40c91e403`  
		Last Modified: Fri, 02 Sep 2022 20:17:05 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8c2a232471cae5193369cbc619007f710b7ea681e38f34a91f7a19213940d82`  
		Last Modified: Fri, 02 Sep 2022 20:17:05 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
