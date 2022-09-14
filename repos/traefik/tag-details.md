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
-	[`traefik:2.8.5`](#traefik285)
-	[`traefik:2.8.5-windowsservercore-1809`](#traefik285-windowsservercore-1809)
-	[`traefik:2.9`](#traefik29)
-	[`traefik:2.9-windowsservercore-1809`](#traefik29-windowsservercore-1809)
-	[`traefik:2.9.0-rc2`](#traefik290-rc2)
-	[`traefik:2.9.0-rc2-windowsservercore-1809`](#traefik290-rc2-windowsservercore-1809)
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
-	[`traefik:v2.8`](#traefikv28)
-	[`traefik:v2.8-windowsservercore-1809`](#traefikv28-windowsservercore-1809)
-	[`traefik:v2.8.5`](#traefikv285)
-	[`traefik:v2.8.5-windowsservercore-1809`](#traefikv285-windowsservercore-1809)
-	[`traefik:v2.9`](#traefikv29)
-	[`traefik:v2.9-windowsservercore-1809`](#traefikv29-windowsservercore-1809)
-	[`traefik:v2.9.0-rc2`](#traefikv290-rc2)
-	[`traefik:v2.9.0-rc2-windowsservercore-1809`](#traefikv290-rc2-windowsservercore-1809)
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

## `traefik:2.8`

```console
$ docker pull traefik@sha256:6793742cf3482a10529b4d18952c720bde9e75e9956a4f5f860179f74a771ab7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; s390x

### `traefik:2.8` - linux; amd64

```console
$ docker pull traefik@sha256:9c663ef4155d64740028190a643f8cc21f5994b106475f790947d79ae9d93179
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.3 MB (33287410 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2caeed3432ab5acef8c4b71b525fb0e563f4923c96c601f8d0d6d889e5a2400c`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Tue, 09 Aug 2022 17:20:00 GMT
ADD file:f77e3f51f020890d22997e6c2ca98968b75b8bc8c463341a2010ff0655d4c88f in / 
# Tue, 09 Aug 2022 17:20:01 GMT
CMD ["/bin/sh"]
# Wed, 10 Aug 2022 01:24:52 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 14 Sep 2022 00:11:02 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.8.5/traefik_v2.8.5_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Wed, 14 Sep 2022 00:11:02 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 14 Sep 2022 00:11:02 GMT
EXPOSE 80
# Wed, 14 Sep 2022 00:11:03 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 14 Sep 2022 00:11:03 GMT
CMD ["traefik"]
# Wed, 14 Sep 2022 00:11:03 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.8.5 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:6bd3e1d95bf998a67bca95f32d5302a4b29a7f769dac8717b4a4010bca9f831b`  
		Last Modified: Wed, 14 Sep 2022 00:11:32 GMT  
		Size: 29.8 MB (29781857 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d269864b08bee0be42edc298f20fd989aa3a4611c472091809a0a0f180b418e4`  
		Last Modified: Wed, 14 Sep 2022 00:11:27 GMT  
		Size: 367.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:2.8` - linux; arm variant v6

```console
$ docker pull traefik@sha256:643f60f24294106bfe36e7b1c78031ecfd0bfd94565de3bdf04a36c3fa7cddb7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.4 MB (31416332 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4079bfbc61f417592a2daff4261b15468b2222f1ffbb4ed08d988eeb5ece3602`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Tue, 09 Aug 2022 17:49:29 GMT
ADD file:89cb25f97e17bed5c56311280efe5cfa78422d8ffbe36232195d13f94d67417e in / 
# Tue, 09 Aug 2022 17:49:29 GMT
CMD ["/bin/sh"]
# Thu, 11 Aug 2022 01:14:12 GMT
RUN apk --no-cache add ca-certificates tzdata
# Tue, 13 Sep 2022 17:49:51 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.8.5/traefik_v2.8.5_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Tue, 13 Sep 2022 17:49:51 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Tue, 13 Sep 2022 17:49:51 GMT
EXPOSE 80
# Tue, 13 Sep 2022 17:49:52 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 13 Sep 2022 17:49:52 GMT
CMD ["traefik"]
# Tue, 13 Sep 2022 17:49:52 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.8.5 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:168e12f01d9663d75ad85257e0fc771695a1b0256facbf3e55c05fd6c815c990`  
		Last Modified: Tue, 13 Sep 2022 17:51:20 GMT  
		Size: 28.1 MB (28098796 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c46c5e0d6400c1577faaa4b41baab6b0ac42755d3fe7a3c031a1ba159cb756e`  
		Last Modified: Tue, 13 Sep 2022 17:51:10 GMT  
		Size: 367.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:2.8` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:13ce7a5dc88cf420bdb4cf574fb5154774ecd5a08290c04375caa3c4431c8c18
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.6 MB (30578838 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8b4f3c81e83b1ab10bb06af37849c73b3bb4cf7e83bb31aa1a40829cbfc4e5fe`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Tue, 09 Aug 2022 17:39:51 GMT
ADD file:4b51a9d40f20d2beb29d0759b161d2b9403493453beb509de4e86a5d98513f16 in / 
# Tue, 09 Aug 2022 17:39:51 GMT
CMD ["/bin/sh"]
# Wed, 10 Aug 2022 06:10:52 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 14 Sep 2022 02:03:27 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.8.5/traefik_v2.8.5_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Wed, 14 Sep 2022 02:03:28 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 14 Sep 2022 02:03:28 GMT
EXPOSE 80
# Wed, 14 Sep 2022 02:03:29 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 14 Sep 2022 02:03:30 GMT
CMD ["traefik"]
# Wed, 14 Sep 2022 02:03:31 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.8.5 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:b1d629b95887fb97125620d51a69b9a4b51ec3a75ff37f9e3878b83d8a2bc573`  
		Last Modified: Wed, 14 Sep 2022 02:04:24 GMT  
		Size: 27.2 MB (27177636 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f3664d2a35c1a60ae1b15981994e7bebefe4ac64d031ecc280c68391c3432d8`  
		Last Modified: Wed, 14 Sep 2022 02:04:20 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:2.8` - linux; s390x

```console
$ docker pull traefik@sha256:dbbef98bd5e072eae0d938fb0990208e7a09f9f3410badf59db381c1866155c6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.0 MB (31979649 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2d3d91b058afd21ca437377b7473a52073aa0b11fc5ef28725cc3ceb5352e912`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Tue, 09 Aug 2022 17:41:54 GMT
ADD file:7489fa84133e97e4f40b13dd5159989b3594c9627d9147bfc4e33134944cc368 in / 
# Tue, 09 Aug 2022 17:41:54 GMT
CMD ["/bin/sh"]
# Wed, 10 Aug 2022 05:50:07 GMT
RUN apk --no-cache add ca-certificates tzdata
# Tue, 13 Sep 2022 17:42:04 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.8.5/traefik_v2.8.5_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Tue, 13 Sep 2022 17:42:06 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Tue, 13 Sep 2022 17:42:06 GMT
EXPOSE 80
# Tue, 13 Sep 2022 17:42:06 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 13 Sep 2022 17:42:06 GMT
CMD ["traefik"]
# Tue, 13 Sep 2022 17:42:06 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.8.5 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:b9e70ad72dd57510b0aca527260bc2a85e4aa206a12a38c3811619286f798d78`  
		Last Modified: Tue, 13 Sep 2022 17:42:32 GMT  
		Size: 28.7 MB (28686667 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2ec4b4277bc0631824764df320de8fd7c7f98f5b13b57f2f8791e3ed6810ff2`  
		Last Modified: Tue, 13 Sep 2022 17:42:28 GMT  
		Size: 367.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:2.8-windowsservercore-1809`

```console
$ docker pull traefik@sha256:84b80d25f3a2267384a31d438bea47b75256258fe5c7d2d458312c5b35842792
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3406; amd64

### `traefik:2.8-windowsservercore-1809` - windows version 10.0.17763.3406; amd64

```console
$ docker pull traefik@sha256:b7c78f8739641f8fb17ba16db5d4467fdc984239aea8c15a6a425d61a5a63726
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2733827197 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c628896d0a4bd9460b62a375fc22a99bb1c32bac428e3c5f3143bdaa85116816`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Fri, 09 Sep 2022 22:43:02 GMT
RUN Install update 10.0.17763.3406
# Tue, 13 Sep 2022 18:21:27 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 13 Sep 2022 18:23:34 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/traefik/traefik/releases/download/v2.8.5/traefik_v2.8.5_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Tue, 13 Sep 2022 18:23:35 GMT
EXPOSE 80
# Tue, 13 Sep 2022 18:23:36 GMT
ENTRYPOINT ["/traefik"]
# Tue, 13 Sep 2022 18:23:37 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.8.5 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:0a5a7a7fc317e347125a1f57626cf99448c897d1e193cb39b3389d0309790b1f`  
		Last Modified: Tue, 13 Sep 2022 18:25:31 GMT  
		Size: 30.3 MB (30256782 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1f48547d8e38f8f77d5668596e89f09cec313c88209ad1cb20cc912c938b6e2`  
		Last Modified: Tue, 13 Sep 2022 18:25:24 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f2c407588e5d1afb60580e8e82e167721e88544f91ff4e62a263ad4f7fea54b`  
		Last Modified: Tue, 13 Sep 2022 18:25:24 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e68faac36cb0c791f445fba14ab5ebe23ebca7a8e86628366c62aac87d03183f`  
		Last Modified: Tue, 13 Sep 2022 18:25:24 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:2.8.5`

```console
$ docker pull traefik@sha256:6793742cf3482a10529b4d18952c720bde9e75e9956a4f5f860179f74a771ab7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; s390x

### `traefik:2.8.5` - linux; amd64

```console
$ docker pull traefik@sha256:9c663ef4155d64740028190a643f8cc21f5994b106475f790947d79ae9d93179
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.3 MB (33287410 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2caeed3432ab5acef8c4b71b525fb0e563f4923c96c601f8d0d6d889e5a2400c`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Tue, 09 Aug 2022 17:20:00 GMT
ADD file:f77e3f51f020890d22997e6c2ca98968b75b8bc8c463341a2010ff0655d4c88f in / 
# Tue, 09 Aug 2022 17:20:01 GMT
CMD ["/bin/sh"]
# Wed, 10 Aug 2022 01:24:52 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 14 Sep 2022 00:11:02 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.8.5/traefik_v2.8.5_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Wed, 14 Sep 2022 00:11:02 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 14 Sep 2022 00:11:02 GMT
EXPOSE 80
# Wed, 14 Sep 2022 00:11:03 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 14 Sep 2022 00:11:03 GMT
CMD ["traefik"]
# Wed, 14 Sep 2022 00:11:03 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.8.5 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:6bd3e1d95bf998a67bca95f32d5302a4b29a7f769dac8717b4a4010bca9f831b`  
		Last Modified: Wed, 14 Sep 2022 00:11:32 GMT  
		Size: 29.8 MB (29781857 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d269864b08bee0be42edc298f20fd989aa3a4611c472091809a0a0f180b418e4`  
		Last Modified: Wed, 14 Sep 2022 00:11:27 GMT  
		Size: 367.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:2.8.5` - linux; arm variant v6

```console
$ docker pull traefik@sha256:643f60f24294106bfe36e7b1c78031ecfd0bfd94565de3bdf04a36c3fa7cddb7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.4 MB (31416332 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4079bfbc61f417592a2daff4261b15468b2222f1ffbb4ed08d988eeb5ece3602`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Tue, 09 Aug 2022 17:49:29 GMT
ADD file:89cb25f97e17bed5c56311280efe5cfa78422d8ffbe36232195d13f94d67417e in / 
# Tue, 09 Aug 2022 17:49:29 GMT
CMD ["/bin/sh"]
# Thu, 11 Aug 2022 01:14:12 GMT
RUN apk --no-cache add ca-certificates tzdata
# Tue, 13 Sep 2022 17:49:51 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.8.5/traefik_v2.8.5_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Tue, 13 Sep 2022 17:49:51 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Tue, 13 Sep 2022 17:49:51 GMT
EXPOSE 80
# Tue, 13 Sep 2022 17:49:52 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 13 Sep 2022 17:49:52 GMT
CMD ["traefik"]
# Tue, 13 Sep 2022 17:49:52 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.8.5 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:168e12f01d9663d75ad85257e0fc771695a1b0256facbf3e55c05fd6c815c990`  
		Last Modified: Tue, 13 Sep 2022 17:51:20 GMT  
		Size: 28.1 MB (28098796 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c46c5e0d6400c1577faaa4b41baab6b0ac42755d3fe7a3c031a1ba159cb756e`  
		Last Modified: Tue, 13 Sep 2022 17:51:10 GMT  
		Size: 367.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:2.8.5` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:13ce7a5dc88cf420bdb4cf574fb5154774ecd5a08290c04375caa3c4431c8c18
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.6 MB (30578838 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8b4f3c81e83b1ab10bb06af37849c73b3bb4cf7e83bb31aa1a40829cbfc4e5fe`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Tue, 09 Aug 2022 17:39:51 GMT
ADD file:4b51a9d40f20d2beb29d0759b161d2b9403493453beb509de4e86a5d98513f16 in / 
# Tue, 09 Aug 2022 17:39:51 GMT
CMD ["/bin/sh"]
# Wed, 10 Aug 2022 06:10:52 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 14 Sep 2022 02:03:27 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.8.5/traefik_v2.8.5_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Wed, 14 Sep 2022 02:03:28 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 14 Sep 2022 02:03:28 GMT
EXPOSE 80
# Wed, 14 Sep 2022 02:03:29 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 14 Sep 2022 02:03:30 GMT
CMD ["traefik"]
# Wed, 14 Sep 2022 02:03:31 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.8.5 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:b1d629b95887fb97125620d51a69b9a4b51ec3a75ff37f9e3878b83d8a2bc573`  
		Last Modified: Wed, 14 Sep 2022 02:04:24 GMT  
		Size: 27.2 MB (27177636 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f3664d2a35c1a60ae1b15981994e7bebefe4ac64d031ecc280c68391c3432d8`  
		Last Modified: Wed, 14 Sep 2022 02:04:20 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:2.8.5` - linux; s390x

```console
$ docker pull traefik@sha256:dbbef98bd5e072eae0d938fb0990208e7a09f9f3410badf59db381c1866155c6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.0 MB (31979649 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2d3d91b058afd21ca437377b7473a52073aa0b11fc5ef28725cc3ceb5352e912`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Tue, 09 Aug 2022 17:41:54 GMT
ADD file:7489fa84133e97e4f40b13dd5159989b3594c9627d9147bfc4e33134944cc368 in / 
# Tue, 09 Aug 2022 17:41:54 GMT
CMD ["/bin/sh"]
# Wed, 10 Aug 2022 05:50:07 GMT
RUN apk --no-cache add ca-certificates tzdata
# Tue, 13 Sep 2022 17:42:04 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.8.5/traefik_v2.8.5_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Tue, 13 Sep 2022 17:42:06 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Tue, 13 Sep 2022 17:42:06 GMT
EXPOSE 80
# Tue, 13 Sep 2022 17:42:06 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 13 Sep 2022 17:42:06 GMT
CMD ["traefik"]
# Tue, 13 Sep 2022 17:42:06 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.8.5 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:b9e70ad72dd57510b0aca527260bc2a85e4aa206a12a38c3811619286f798d78`  
		Last Modified: Tue, 13 Sep 2022 17:42:32 GMT  
		Size: 28.7 MB (28686667 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2ec4b4277bc0631824764df320de8fd7c7f98f5b13b57f2f8791e3ed6810ff2`  
		Last Modified: Tue, 13 Sep 2022 17:42:28 GMT  
		Size: 367.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:2.8.5-windowsservercore-1809`

```console
$ docker pull traefik@sha256:84b80d25f3a2267384a31d438bea47b75256258fe5c7d2d458312c5b35842792
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3406; amd64

### `traefik:2.8.5-windowsservercore-1809` - windows version 10.0.17763.3406; amd64

```console
$ docker pull traefik@sha256:b7c78f8739641f8fb17ba16db5d4467fdc984239aea8c15a6a425d61a5a63726
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2733827197 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c628896d0a4bd9460b62a375fc22a99bb1c32bac428e3c5f3143bdaa85116816`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Fri, 09 Sep 2022 22:43:02 GMT
RUN Install update 10.0.17763.3406
# Tue, 13 Sep 2022 18:21:27 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 13 Sep 2022 18:23:34 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/traefik/traefik/releases/download/v2.8.5/traefik_v2.8.5_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Tue, 13 Sep 2022 18:23:35 GMT
EXPOSE 80
# Tue, 13 Sep 2022 18:23:36 GMT
ENTRYPOINT ["/traefik"]
# Tue, 13 Sep 2022 18:23:37 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.8.5 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:0a5a7a7fc317e347125a1f57626cf99448c897d1e193cb39b3389d0309790b1f`  
		Last Modified: Tue, 13 Sep 2022 18:25:31 GMT  
		Size: 30.3 MB (30256782 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1f48547d8e38f8f77d5668596e89f09cec313c88209ad1cb20cc912c938b6e2`  
		Last Modified: Tue, 13 Sep 2022 18:25:24 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f2c407588e5d1afb60580e8e82e167721e88544f91ff4e62a263ad4f7fea54b`  
		Last Modified: Tue, 13 Sep 2022 18:25:24 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e68faac36cb0c791f445fba14ab5ebe23ebca7a8e86628366c62aac87d03183f`  
		Last Modified: Tue, 13 Sep 2022 18:25:24 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:2.9`

```console
$ docker pull traefik@sha256:85a6cc7ef661a606c90f582a84a1574ab2a7699b03319f34a39bfaab143c7a2f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; s390x

### `traefik:2.9` - linux; amd64

```console
$ docker pull traefik@sha256:860e745b5a8c128ba7f834f709041de2b2576b1b2b8600961b6609c68896a950
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.4 MB (33415001 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:733f54fee3cb63f8b6c4318fbd00695fb4e7c1b0d83e24a2ccfd33b3d9c1b7c7`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Tue, 09 Aug 2022 17:20:00 GMT
ADD file:f77e3f51f020890d22997e6c2ca98968b75b8bc8c463341a2010ff0655d4c88f in / 
# Tue, 09 Aug 2022 17:20:01 GMT
CMD ["/bin/sh"]
# Wed, 10 Aug 2022 01:24:52 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 14 Sep 2022 17:31:12 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.9.0-rc2/traefik_v2.9.0-rc2_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Wed, 14 Sep 2022 17:31:12 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 14 Sep 2022 17:31:12 GMT
EXPOSE 80
# Wed, 14 Sep 2022 17:31:12 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 14 Sep 2022 17:31:12 GMT
CMD ["traefik"]
# Wed, 14 Sep 2022 17:31:12 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.9.0-rc2 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:1057a6f424b8065718d448e1341e44cc810c2efa5867ea06905a6155babb55cd`  
		Last Modified: Wed, 14 Sep 2022 17:31:48 GMT  
		Size: 29.9 MB (29909447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a53d84e31a10b690ee5915568293cefec447442f2a91c66c910c73a18ece40d7`  
		Last Modified: Wed, 14 Sep 2022 17:31:43 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:2.9` - linux; arm variant v6

```console
$ docker pull traefik@sha256:eab6cd20bed0ad8dfca482d1bdae2ba5a118cfa00a9086c2410ab059d6c26433
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.5 MB (31534900 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:43151892a1801b8be839577e0ae491e7ece6fa9206013b45f25b30d03df66f56`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Tue, 09 Aug 2022 17:49:29 GMT
ADD file:89cb25f97e17bed5c56311280efe5cfa78422d8ffbe36232195d13f94d67417e in / 
# Tue, 09 Aug 2022 17:49:29 GMT
CMD ["/bin/sh"]
# Thu, 11 Aug 2022 01:14:12 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 14 Sep 2022 16:49:40 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.9.0-rc2/traefik_v2.9.0-rc2_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Wed, 14 Sep 2022 16:49:40 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 14 Sep 2022 16:49:40 GMT
EXPOSE 80
# Wed, 14 Sep 2022 16:49:41 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 14 Sep 2022 16:49:41 GMT
CMD ["traefik"]
# Wed, 14 Sep 2022 16:49:41 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.9.0-rc2 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:e576a8d45a56333d4da8afd2ce3fd479e43dddfdaa224ecd0e06e049a68535f7`  
		Last Modified: Wed, 14 Sep 2022 16:51:06 GMT  
		Size: 28.2 MB (28217364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c553eb1fce4b36e147b198d55eccfe90c8e9a652a8186a179b66d72b21ba982`  
		Last Modified: Wed, 14 Sep 2022 16:50:59 GMT  
		Size: 367.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:2.9` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:942c80da34fd238da2411af8283c699b381e058bcb946b8d17c20a5543b126e4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.7 MB (30704146 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d905851689f22b1d5f2bf66996d4f107fa1d6a117d3f337e0385f6ef17a31964`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Tue, 09 Aug 2022 17:39:51 GMT
ADD file:4b51a9d40f20d2beb29d0759b161d2b9403493453beb509de4e86a5d98513f16 in / 
# Tue, 09 Aug 2022 17:39:51 GMT
CMD ["/bin/sh"]
# Wed, 10 Aug 2022 06:10:52 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 14 Sep 2022 17:48:53 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.9.0-rc2/traefik_v2.9.0-rc2_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Wed, 14 Sep 2022 17:48:55 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 14 Sep 2022 17:48:55 GMT
EXPOSE 80
# Wed, 14 Sep 2022 17:48:56 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 14 Sep 2022 17:48:57 GMT
CMD ["traefik"]
# Wed, 14 Sep 2022 17:48:58 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.9.0-rc2 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:90b7f8f6407af93928b4badc4e761d40e8913c6e1e1f5f3af889b67604ae2255`  
		Last Modified: Wed, 14 Sep 2022 17:50:03 GMT  
		Size: 27.3 MB (27302946 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:933489f19e2e5f601df880072d17e7726d2514e99a1fe6e3c297e290779e75d7`  
		Last Modified: Wed, 14 Sep 2022 17:50:00 GMT  
		Size: 366.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:2.9` - linux; s390x

```console
$ docker pull traefik@sha256:bd27728d6ed0565479ffcd1b1b1296eb5b8e3fdf1589302968884893c7f5286b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.1 MB (32104507 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c87694a06b62bdebebdc3950b2fcb8dc6f4ed3e34dd82d7baca9e2d77d840936`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Tue, 09 Aug 2022 17:41:54 GMT
ADD file:7489fa84133e97e4f40b13dd5159989b3594c9627d9147bfc4e33134944cc368 in / 
# Tue, 09 Aug 2022 17:41:54 GMT
CMD ["/bin/sh"]
# Wed, 10 Aug 2022 05:50:07 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 14 Sep 2022 17:44:01 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.9.0-rc2/traefik_v2.9.0-rc2_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Wed, 14 Sep 2022 17:44:02 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 14 Sep 2022 17:44:03 GMT
EXPOSE 80
# Wed, 14 Sep 2022 17:44:03 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 14 Sep 2022 17:44:03 GMT
CMD ["traefik"]
# Wed, 14 Sep 2022 17:44:03 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.9.0-rc2 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:97d39fe8daa11aed96420967fc20a46039da1f9685afa7c75c3a4644a8b5304f`  
		Last Modified: Wed, 14 Sep 2022 17:44:44 GMT  
		Size: 28.8 MB (28811524 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00c529102fa59c1aec188d12d972ed922d09a291141a8acf50e394c771a7c7a3`  
		Last Modified: Wed, 14 Sep 2022 17:44:40 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:2.9-windowsservercore-1809`

```console
$ docker pull traefik@sha256:b000b4e6e3726b437b7b1ace6b4c9e55cb7cc349da368bcd67c5ef957f57e191
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3406; amd64

### `traefik:2.9-windowsservercore-1809` - windows version 10.0.17763.3406; amd64

```console
$ docker pull traefik@sha256:64e18eca374103f73e24568789ffb3c52c6a7b78e0c9c559dedf7929420ed0d0
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2733959697 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c0a892b2b4ba43a03cfff3fc8019d56e3974b0c5d642017973fcd5bec1fa130e`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Fri, 09 Sep 2022 22:43:02 GMT
RUN Install update 10.0.17763.3406
# Tue, 13 Sep 2022 18:21:27 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 14 Sep 2022 19:41:53 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/traefik/traefik/releases/download/v2.9.0-rc2/traefik_v2.9.0-rc2_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Wed, 14 Sep 2022 19:41:54 GMT
EXPOSE 80
# Wed, 14 Sep 2022 19:41:55 GMT
ENTRYPOINT ["/traefik"]
# Wed, 14 Sep 2022 19:41:56 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.9.0-rc2 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:6fd1d5543f6a70571fa830e350046a78addb303a36ede4233fa8fe4d809517ea`  
		Last Modified: Wed, 14 Sep 2022 19:42:48 GMT  
		Size: 30.4 MB (30389286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a88c552a6644064f7e4cba6d62cb1ccd22b59ccd989274c4e559c84dd9feb7ca`  
		Last Modified: Wed, 14 Sep 2022 19:42:42 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d70373754967f4a871e0e588a00155117e2932a7866ec732a6d7e64f919e4333`  
		Last Modified: Wed, 14 Sep 2022 19:42:42 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6170fe9fdc8d3820a4f4029ffc052a215b267811ac3a4cd5ee044cee7e93aa5`  
		Last Modified: Wed, 14 Sep 2022 19:42:42 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:2.9.0-rc2`

```console
$ docker pull traefik@sha256:85a6cc7ef661a606c90f582a84a1574ab2a7699b03319f34a39bfaab143c7a2f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; s390x

### `traefik:2.9.0-rc2` - linux; amd64

```console
$ docker pull traefik@sha256:860e745b5a8c128ba7f834f709041de2b2576b1b2b8600961b6609c68896a950
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.4 MB (33415001 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:733f54fee3cb63f8b6c4318fbd00695fb4e7c1b0d83e24a2ccfd33b3d9c1b7c7`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Tue, 09 Aug 2022 17:20:00 GMT
ADD file:f77e3f51f020890d22997e6c2ca98968b75b8bc8c463341a2010ff0655d4c88f in / 
# Tue, 09 Aug 2022 17:20:01 GMT
CMD ["/bin/sh"]
# Wed, 10 Aug 2022 01:24:52 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 14 Sep 2022 17:31:12 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.9.0-rc2/traefik_v2.9.0-rc2_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Wed, 14 Sep 2022 17:31:12 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 14 Sep 2022 17:31:12 GMT
EXPOSE 80
# Wed, 14 Sep 2022 17:31:12 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 14 Sep 2022 17:31:12 GMT
CMD ["traefik"]
# Wed, 14 Sep 2022 17:31:12 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.9.0-rc2 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:1057a6f424b8065718d448e1341e44cc810c2efa5867ea06905a6155babb55cd`  
		Last Modified: Wed, 14 Sep 2022 17:31:48 GMT  
		Size: 29.9 MB (29909447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a53d84e31a10b690ee5915568293cefec447442f2a91c66c910c73a18ece40d7`  
		Last Modified: Wed, 14 Sep 2022 17:31:43 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:2.9.0-rc2` - linux; arm variant v6

```console
$ docker pull traefik@sha256:eab6cd20bed0ad8dfca482d1bdae2ba5a118cfa00a9086c2410ab059d6c26433
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.5 MB (31534900 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:43151892a1801b8be839577e0ae491e7ece6fa9206013b45f25b30d03df66f56`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Tue, 09 Aug 2022 17:49:29 GMT
ADD file:89cb25f97e17bed5c56311280efe5cfa78422d8ffbe36232195d13f94d67417e in / 
# Tue, 09 Aug 2022 17:49:29 GMT
CMD ["/bin/sh"]
# Thu, 11 Aug 2022 01:14:12 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 14 Sep 2022 16:49:40 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.9.0-rc2/traefik_v2.9.0-rc2_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Wed, 14 Sep 2022 16:49:40 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 14 Sep 2022 16:49:40 GMT
EXPOSE 80
# Wed, 14 Sep 2022 16:49:41 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 14 Sep 2022 16:49:41 GMT
CMD ["traefik"]
# Wed, 14 Sep 2022 16:49:41 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.9.0-rc2 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:e576a8d45a56333d4da8afd2ce3fd479e43dddfdaa224ecd0e06e049a68535f7`  
		Last Modified: Wed, 14 Sep 2022 16:51:06 GMT  
		Size: 28.2 MB (28217364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c553eb1fce4b36e147b198d55eccfe90c8e9a652a8186a179b66d72b21ba982`  
		Last Modified: Wed, 14 Sep 2022 16:50:59 GMT  
		Size: 367.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:2.9.0-rc2` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:942c80da34fd238da2411af8283c699b381e058bcb946b8d17c20a5543b126e4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.7 MB (30704146 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d905851689f22b1d5f2bf66996d4f107fa1d6a117d3f337e0385f6ef17a31964`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Tue, 09 Aug 2022 17:39:51 GMT
ADD file:4b51a9d40f20d2beb29d0759b161d2b9403493453beb509de4e86a5d98513f16 in / 
# Tue, 09 Aug 2022 17:39:51 GMT
CMD ["/bin/sh"]
# Wed, 10 Aug 2022 06:10:52 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 14 Sep 2022 17:48:53 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.9.0-rc2/traefik_v2.9.0-rc2_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Wed, 14 Sep 2022 17:48:55 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 14 Sep 2022 17:48:55 GMT
EXPOSE 80
# Wed, 14 Sep 2022 17:48:56 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 14 Sep 2022 17:48:57 GMT
CMD ["traefik"]
# Wed, 14 Sep 2022 17:48:58 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.9.0-rc2 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:90b7f8f6407af93928b4badc4e761d40e8913c6e1e1f5f3af889b67604ae2255`  
		Last Modified: Wed, 14 Sep 2022 17:50:03 GMT  
		Size: 27.3 MB (27302946 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:933489f19e2e5f601df880072d17e7726d2514e99a1fe6e3c297e290779e75d7`  
		Last Modified: Wed, 14 Sep 2022 17:50:00 GMT  
		Size: 366.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:2.9.0-rc2` - linux; s390x

```console
$ docker pull traefik@sha256:bd27728d6ed0565479ffcd1b1b1296eb5b8e3fdf1589302968884893c7f5286b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.1 MB (32104507 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c87694a06b62bdebebdc3950b2fcb8dc6f4ed3e34dd82d7baca9e2d77d840936`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Tue, 09 Aug 2022 17:41:54 GMT
ADD file:7489fa84133e97e4f40b13dd5159989b3594c9627d9147bfc4e33134944cc368 in / 
# Tue, 09 Aug 2022 17:41:54 GMT
CMD ["/bin/sh"]
# Wed, 10 Aug 2022 05:50:07 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 14 Sep 2022 17:44:01 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.9.0-rc2/traefik_v2.9.0-rc2_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Wed, 14 Sep 2022 17:44:02 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 14 Sep 2022 17:44:03 GMT
EXPOSE 80
# Wed, 14 Sep 2022 17:44:03 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 14 Sep 2022 17:44:03 GMT
CMD ["traefik"]
# Wed, 14 Sep 2022 17:44:03 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.9.0-rc2 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:97d39fe8daa11aed96420967fc20a46039da1f9685afa7c75c3a4644a8b5304f`  
		Last Modified: Wed, 14 Sep 2022 17:44:44 GMT  
		Size: 28.8 MB (28811524 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00c529102fa59c1aec188d12d972ed922d09a291141a8acf50e394c771a7c7a3`  
		Last Modified: Wed, 14 Sep 2022 17:44:40 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:2.9.0-rc2-windowsservercore-1809`

```console
$ docker pull traefik@sha256:b000b4e6e3726b437b7b1ace6b4c9e55cb7cc349da368bcd67c5ef957f57e191
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3406; amd64

### `traefik:2.9.0-rc2-windowsservercore-1809` - windows version 10.0.17763.3406; amd64

```console
$ docker pull traefik@sha256:64e18eca374103f73e24568789ffb3c52c6a7b78e0c9c559dedf7929420ed0d0
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2733959697 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c0a892b2b4ba43a03cfff3fc8019d56e3974b0c5d642017973fcd5bec1fa130e`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Fri, 09 Sep 2022 22:43:02 GMT
RUN Install update 10.0.17763.3406
# Tue, 13 Sep 2022 18:21:27 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 14 Sep 2022 19:41:53 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/traefik/traefik/releases/download/v2.9.0-rc2/traefik_v2.9.0-rc2_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Wed, 14 Sep 2022 19:41:54 GMT
EXPOSE 80
# Wed, 14 Sep 2022 19:41:55 GMT
ENTRYPOINT ["/traefik"]
# Wed, 14 Sep 2022 19:41:56 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.9.0-rc2 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:6fd1d5543f6a70571fa830e350046a78addb303a36ede4233fa8fe4d809517ea`  
		Last Modified: Wed, 14 Sep 2022 19:42:48 GMT  
		Size: 30.4 MB (30389286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a88c552a6644064f7e4cba6d62cb1ccd22b59ccd989274c4e559c84dd9feb7ca`  
		Last Modified: Wed, 14 Sep 2022 19:42:42 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d70373754967f4a871e0e588a00155117e2932a7866ec732a6d7e64f919e4333`  
		Last Modified: Wed, 14 Sep 2022 19:42:42 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6170fe9fdc8d3820a4f4029ffc052a215b267811ac3a4cd5ee044cee7e93aa5`  
		Last Modified: Wed, 14 Sep 2022 19:42:42 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:beaufort`

```console
$ docker pull traefik@sha256:85a6cc7ef661a606c90f582a84a1574ab2a7699b03319f34a39bfaab143c7a2f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; s390x

### `traefik:beaufort` - linux; amd64

```console
$ docker pull traefik@sha256:860e745b5a8c128ba7f834f709041de2b2576b1b2b8600961b6609c68896a950
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.4 MB (33415001 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:733f54fee3cb63f8b6c4318fbd00695fb4e7c1b0d83e24a2ccfd33b3d9c1b7c7`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Tue, 09 Aug 2022 17:20:00 GMT
ADD file:f77e3f51f020890d22997e6c2ca98968b75b8bc8c463341a2010ff0655d4c88f in / 
# Tue, 09 Aug 2022 17:20:01 GMT
CMD ["/bin/sh"]
# Wed, 10 Aug 2022 01:24:52 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 14 Sep 2022 17:31:12 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.9.0-rc2/traefik_v2.9.0-rc2_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Wed, 14 Sep 2022 17:31:12 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 14 Sep 2022 17:31:12 GMT
EXPOSE 80
# Wed, 14 Sep 2022 17:31:12 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 14 Sep 2022 17:31:12 GMT
CMD ["traefik"]
# Wed, 14 Sep 2022 17:31:12 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.9.0-rc2 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:1057a6f424b8065718d448e1341e44cc810c2efa5867ea06905a6155babb55cd`  
		Last Modified: Wed, 14 Sep 2022 17:31:48 GMT  
		Size: 29.9 MB (29909447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a53d84e31a10b690ee5915568293cefec447442f2a91c66c910c73a18ece40d7`  
		Last Modified: Wed, 14 Sep 2022 17:31:43 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:beaufort` - linux; arm variant v6

```console
$ docker pull traefik@sha256:eab6cd20bed0ad8dfca482d1bdae2ba5a118cfa00a9086c2410ab059d6c26433
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.5 MB (31534900 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:43151892a1801b8be839577e0ae491e7ece6fa9206013b45f25b30d03df66f56`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Tue, 09 Aug 2022 17:49:29 GMT
ADD file:89cb25f97e17bed5c56311280efe5cfa78422d8ffbe36232195d13f94d67417e in / 
# Tue, 09 Aug 2022 17:49:29 GMT
CMD ["/bin/sh"]
# Thu, 11 Aug 2022 01:14:12 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 14 Sep 2022 16:49:40 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.9.0-rc2/traefik_v2.9.0-rc2_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Wed, 14 Sep 2022 16:49:40 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 14 Sep 2022 16:49:40 GMT
EXPOSE 80
# Wed, 14 Sep 2022 16:49:41 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 14 Sep 2022 16:49:41 GMT
CMD ["traefik"]
# Wed, 14 Sep 2022 16:49:41 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.9.0-rc2 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:e576a8d45a56333d4da8afd2ce3fd479e43dddfdaa224ecd0e06e049a68535f7`  
		Last Modified: Wed, 14 Sep 2022 16:51:06 GMT  
		Size: 28.2 MB (28217364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c553eb1fce4b36e147b198d55eccfe90c8e9a652a8186a179b66d72b21ba982`  
		Last Modified: Wed, 14 Sep 2022 16:50:59 GMT  
		Size: 367.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:beaufort` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:942c80da34fd238da2411af8283c699b381e058bcb946b8d17c20a5543b126e4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.7 MB (30704146 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d905851689f22b1d5f2bf66996d4f107fa1d6a117d3f337e0385f6ef17a31964`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Tue, 09 Aug 2022 17:39:51 GMT
ADD file:4b51a9d40f20d2beb29d0759b161d2b9403493453beb509de4e86a5d98513f16 in / 
# Tue, 09 Aug 2022 17:39:51 GMT
CMD ["/bin/sh"]
# Wed, 10 Aug 2022 06:10:52 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 14 Sep 2022 17:48:53 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.9.0-rc2/traefik_v2.9.0-rc2_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Wed, 14 Sep 2022 17:48:55 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 14 Sep 2022 17:48:55 GMT
EXPOSE 80
# Wed, 14 Sep 2022 17:48:56 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 14 Sep 2022 17:48:57 GMT
CMD ["traefik"]
# Wed, 14 Sep 2022 17:48:58 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.9.0-rc2 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:90b7f8f6407af93928b4badc4e761d40e8913c6e1e1f5f3af889b67604ae2255`  
		Last Modified: Wed, 14 Sep 2022 17:50:03 GMT  
		Size: 27.3 MB (27302946 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:933489f19e2e5f601df880072d17e7726d2514e99a1fe6e3c297e290779e75d7`  
		Last Modified: Wed, 14 Sep 2022 17:50:00 GMT  
		Size: 366.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:beaufort` - linux; s390x

```console
$ docker pull traefik@sha256:bd27728d6ed0565479ffcd1b1b1296eb5b8e3fdf1589302968884893c7f5286b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.1 MB (32104507 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c87694a06b62bdebebdc3950b2fcb8dc6f4ed3e34dd82d7baca9e2d77d840936`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Tue, 09 Aug 2022 17:41:54 GMT
ADD file:7489fa84133e97e4f40b13dd5159989b3594c9627d9147bfc4e33134944cc368 in / 
# Tue, 09 Aug 2022 17:41:54 GMT
CMD ["/bin/sh"]
# Wed, 10 Aug 2022 05:50:07 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 14 Sep 2022 17:44:01 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.9.0-rc2/traefik_v2.9.0-rc2_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Wed, 14 Sep 2022 17:44:02 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 14 Sep 2022 17:44:03 GMT
EXPOSE 80
# Wed, 14 Sep 2022 17:44:03 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 14 Sep 2022 17:44:03 GMT
CMD ["traefik"]
# Wed, 14 Sep 2022 17:44:03 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.9.0-rc2 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:97d39fe8daa11aed96420967fc20a46039da1f9685afa7c75c3a4644a8b5304f`  
		Last Modified: Wed, 14 Sep 2022 17:44:44 GMT  
		Size: 28.8 MB (28811524 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00c529102fa59c1aec188d12d972ed922d09a291141a8acf50e394c771a7c7a3`  
		Last Modified: Wed, 14 Sep 2022 17:44:40 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:beaufort-windowsservercore-1809`

```console
$ docker pull traefik@sha256:b000b4e6e3726b437b7b1ace6b4c9e55cb7cc349da368bcd67c5ef957f57e191
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3406; amd64

### `traefik:beaufort-windowsservercore-1809` - windows version 10.0.17763.3406; amd64

```console
$ docker pull traefik@sha256:64e18eca374103f73e24568789ffb3c52c6a7b78e0c9c559dedf7929420ed0d0
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2733959697 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c0a892b2b4ba43a03cfff3fc8019d56e3974b0c5d642017973fcd5bec1fa130e`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Fri, 09 Sep 2022 22:43:02 GMT
RUN Install update 10.0.17763.3406
# Tue, 13 Sep 2022 18:21:27 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 14 Sep 2022 19:41:53 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/traefik/traefik/releases/download/v2.9.0-rc2/traefik_v2.9.0-rc2_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Wed, 14 Sep 2022 19:41:54 GMT
EXPOSE 80
# Wed, 14 Sep 2022 19:41:55 GMT
ENTRYPOINT ["/traefik"]
# Wed, 14 Sep 2022 19:41:56 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.9.0-rc2 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:6fd1d5543f6a70571fa830e350046a78addb303a36ede4233fa8fe4d809517ea`  
		Last Modified: Wed, 14 Sep 2022 19:42:48 GMT  
		Size: 30.4 MB (30389286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a88c552a6644064f7e4cba6d62cb1ccd22b59ccd989274c4e559c84dd9feb7ca`  
		Last Modified: Wed, 14 Sep 2022 19:42:42 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d70373754967f4a871e0e588a00155117e2932a7866ec732a6d7e64f919e4333`  
		Last Modified: Wed, 14 Sep 2022 19:42:42 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6170fe9fdc8d3820a4f4029ffc052a215b267811ac3a4cd5ee044cee7e93aa5`  
		Last Modified: Wed, 14 Sep 2022 19:42:42 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:latest`

```console
$ docker pull traefik@sha256:6793742cf3482a10529b4d18952c720bde9e75e9956a4f5f860179f74a771ab7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; s390x

### `traefik:latest` - linux; amd64

```console
$ docker pull traefik@sha256:9c663ef4155d64740028190a643f8cc21f5994b106475f790947d79ae9d93179
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.3 MB (33287410 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2caeed3432ab5acef8c4b71b525fb0e563f4923c96c601f8d0d6d889e5a2400c`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Tue, 09 Aug 2022 17:20:00 GMT
ADD file:f77e3f51f020890d22997e6c2ca98968b75b8bc8c463341a2010ff0655d4c88f in / 
# Tue, 09 Aug 2022 17:20:01 GMT
CMD ["/bin/sh"]
# Wed, 10 Aug 2022 01:24:52 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 14 Sep 2022 00:11:02 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.8.5/traefik_v2.8.5_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Wed, 14 Sep 2022 00:11:02 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 14 Sep 2022 00:11:02 GMT
EXPOSE 80
# Wed, 14 Sep 2022 00:11:03 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 14 Sep 2022 00:11:03 GMT
CMD ["traefik"]
# Wed, 14 Sep 2022 00:11:03 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.8.5 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:6bd3e1d95bf998a67bca95f32d5302a4b29a7f769dac8717b4a4010bca9f831b`  
		Last Modified: Wed, 14 Sep 2022 00:11:32 GMT  
		Size: 29.8 MB (29781857 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d269864b08bee0be42edc298f20fd989aa3a4611c472091809a0a0f180b418e4`  
		Last Modified: Wed, 14 Sep 2022 00:11:27 GMT  
		Size: 367.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:latest` - linux; arm variant v6

```console
$ docker pull traefik@sha256:643f60f24294106bfe36e7b1c78031ecfd0bfd94565de3bdf04a36c3fa7cddb7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.4 MB (31416332 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4079bfbc61f417592a2daff4261b15468b2222f1ffbb4ed08d988eeb5ece3602`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Tue, 09 Aug 2022 17:49:29 GMT
ADD file:89cb25f97e17bed5c56311280efe5cfa78422d8ffbe36232195d13f94d67417e in / 
# Tue, 09 Aug 2022 17:49:29 GMT
CMD ["/bin/sh"]
# Thu, 11 Aug 2022 01:14:12 GMT
RUN apk --no-cache add ca-certificates tzdata
# Tue, 13 Sep 2022 17:49:51 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.8.5/traefik_v2.8.5_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Tue, 13 Sep 2022 17:49:51 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Tue, 13 Sep 2022 17:49:51 GMT
EXPOSE 80
# Tue, 13 Sep 2022 17:49:52 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 13 Sep 2022 17:49:52 GMT
CMD ["traefik"]
# Tue, 13 Sep 2022 17:49:52 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.8.5 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:168e12f01d9663d75ad85257e0fc771695a1b0256facbf3e55c05fd6c815c990`  
		Last Modified: Tue, 13 Sep 2022 17:51:20 GMT  
		Size: 28.1 MB (28098796 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c46c5e0d6400c1577faaa4b41baab6b0ac42755d3fe7a3c031a1ba159cb756e`  
		Last Modified: Tue, 13 Sep 2022 17:51:10 GMT  
		Size: 367.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:latest` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:13ce7a5dc88cf420bdb4cf574fb5154774ecd5a08290c04375caa3c4431c8c18
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.6 MB (30578838 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8b4f3c81e83b1ab10bb06af37849c73b3bb4cf7e83bb31aa1a40829cbfc4e5fe`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Tue, 09 Aug 2022 17:39:51 GMT
ADD file:4b51a9d40f20d2beb29d0759b161d2b9403493453beb509de4e86a5d98513f16 in / 
# Tue, 09 Aug 2022 17:39:51 GMT
CMD ["/bin/sh"]
# Wed, 10 Aug 2022 06:10:52 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 14 Sep 2022 02:03:27 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.8.5/traefik_v2.8.5_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Wed, 14 Sep 2022 02:03:28 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 14 Sep 2022 02:03:28 GMT
EXPOSE 80
# Wed, 14 Sep 2022 02:03:29 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 14 Sep 2022 02:03:30 GMT
CMD ["traefik"]
# Wed, 14 Sep 2022 02:03:31 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.8.5 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:b1d629b95887fb97125620d51a69b9a4b51ec3a75ff37f9e3878b83d8a2bc573`  
		Last Modified: Wed, 14 Sep 2022 02:04:24 GMT  
		Size: 27.2 MB (27177636 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f3664d2a35c1a60ae1b15981994e7bebefe4ac64d031ecc280c68391c3432d8`  
		Last Modified: Wed, 14 Sep 2022 02:04:20 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:latest` - linux; s390x

```console
$ docker pull traefik@sha256:dbbef98bd5e072eae0d938fb0990208e7a09f9f3410badf59db381c1866155c6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.0 MB (31979649 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2d3d91b058afd21ca437377b7473a52073aa0b11fc5ef28725cc3ceb5352e912`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Tue, 09 Aug 2022 17:41:54 GMT
ADD file:7489fa84133e97e4f40b13dd5159989b3594c9627d9147bfc4e33134944cc368 in / 
# Tue, 09 Aug 2022 17:41:54 GMT
CMD ["/bin/sh"]
# Wed, 10 Aug 2022 05:50:07 GMT
RUN apk --no-cache add ca-certificates tzdata
# Tue, 13 Sep 2022 17:42:04 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.8.5/traefik_v2.8.5_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Tue, 13 Sep 2022 17:42:06 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Tue, 13 Sep 2022 17:42:06 GMT
EXPOSE 80
# Tue, 13 Sep 2022 17:42:06 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 13 Sep 2022 17:42:06 GMT
CMD ["traefik"]
# Tue, 13 Sep 2022 17:42:06 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.8.5 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:b9e70ad72dd57510b0aca527260bc2a85e4aa206a12a38c3811619286f798d78`  
		Last Modified: Tue, 13 Sep 2022 17:42:32 GMT  
		Size: 28.7 MB (28686667 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2ec4b4277bc0631824764df320de8fd7c7f98f5b13b57f2f8791e3ed6810ff2`  
		Last Modified: Tue, 13 Sep 2022 17:42:28 GMT  
		Size: 367.0 B  
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

## `traefik:v2.8`

```console
$ docker pull traefik@sha256:6793742cf3482a10529b4d18952c720bde9e75e9956a4f5f860179f74a771ab7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; s390x

### `traefik:v2.8` - linux; amd64

```console
$ docker pull traefik@sha256:9c663ef4155d64740028190a643f8cc21f5994b106475f790947d79ae9d93179
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.3 MB (33287410 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2caeed3432ab5acef8c4b71b525fb0e563f4923c96c601f8d0d6d889e5a2400c`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Tue, 09 Aug 2022 17:20:00 GMT
ADD file:f77e3f51f020890d22997e6c2ca98968b75b8bc8c463341a2010ff0655d4c88f in / 
# Tue, 09 Aug 2022 17:20:01 GMT
CMD ["/bin/sh"]
# Wed, 10 Aug 2022 01:24:52 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 14 Sep 2022 00:11:02 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.8.5/traefik_v2.8.5_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Wed, 14 Sep 2022 00:11:02 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 14 Sep 2022 00:11:02 GMT
EXPOSE 80
# Wed, 14 Sep 2022 00:11:03 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 14 Sep 2022 00:11:03 GMT
CMD ["traefik"]
# Wed, 14 Sep 2022 00:11:03 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.8.5 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:6bd3e1d95bf998a67bca95f32d5302a4b29a7f769dac8717b4a4010bca9f831b`  
		Last Modified: Wed, 14 Sep 2022 00:11:32 GMT  
		Size: 29.8 MB (29781857 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d269864b08bee0be42edc298f20fd989aa3a4611c472091809a0a0f180b418e4`  
		Last Modified: Wed, 14 Sep 2022 00:11:27 GMT  
		Size: 367.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v2.8` - linux; arm variant v6

```console
$ docker pull traefik@sha256:643f60f24294106bfe36e7b1c78031ecfd0bfd94565de3bdf04a36c3fa7cddb7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.4 MB (31416332 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4079bfbc61f417592a2daff4261b15468b2222f1ffbb4ed08d988eeb5ece3602`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Tue, 09 Aug 2022 17:49:29 GMT
ADD file:89cb25f97e17bed5c56311280efe5cfa78422d8ffbe36232195d13f94d67417e in / 
# Tue, 09 Aug 2022 17:49:29 GMT
CMD ["/bin/sh"]
# Thu, 11 Aug 2022 01:14:12 GMT
RUN apk --no-cache add ca-certificates tzdata
# Tue, 13 Sep 2022 17:49:51 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.8.5/traefik_v2.8.5_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Tue, 13 Sep 2022 17:49:51 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Tue, 13 Sep 2022 17:49:51 GMT
EXPOSE 80
# Tue, 13 Sep 2022 17:49:52 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 13 Sep 2022 17:49:52 GMT
CMD ["traefik"]
# Tue, 13 Sep 2022 17:49:52 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.8.5 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:168e12f01d9663d75ad85257e0fc771695a1b0256facbf3e55c05fd6c815c990`  
		Last Modified: Tue, 13 Sep 2022 17:51:20 GMT  
		Size: 28.1 MB (28098796 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c46c5e0d6400c1577faaa4b41baab6b0ac42755d3fe7a3c031a1ba159cb756e`  
		Last Modified: Tue, 13 Sep 2022 17:51:10 GMT  
		Size: 367.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v2.8` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:13ce7a5dc88cf420bdb4cf574fb5154774ecd5a08290c04375caa3c4431c8c18
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.6 MB (30578838 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8b4f3c81e83b1ab10bb06af37849c73b3bb4cf7e83bb31aa1a40829cbfc4e5fe`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Tue, 09 Aug 2022 17:39:51 GMT
ADD file:4b51a9d40f20d2beb29d0759b161d2b9403493453beb509de4e86a5d98513f16 in / 
# Tue, 09 Aug 2022 17:39:51 GMT
CMD ["/bin/sh"]
# Wed, 10 Aug 2022 06:10:52 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 14 Sep 2022 02:03:27 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.8.5/traefik_v2.8.5_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Wed, 14 Sep 2022 02:03:28 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 14 Sep 2022 02:03:28 GMT
EXPOSE 80
# Wed, 14 Sep 2022 02:03:29 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 14 Sep 2022 02:03:30 GMT
CMD ["traefik"]
# Wed, 14 Sep 2022 02:03:31 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.8.5 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:b1d629b95887fb97125620d51a69b9a4b51ec3a75ff37f9e3878b83d8a2bc573`  
		Last Modified: Wed, 14 Sep 2022 02:04:24 GMT  
		Size: 27.2 MB (27177636 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f3664d2a35c1a60ae1b15981994e7bebefe4ac64d031ecc280c68391c3432d8`  
		Last Modified: Wed, 14 Sep 2022 02:04:20 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v2.8` - linux; s390x

```console
$ docker pull traefik@sha256:dbbef98bd5e072eae0d938fb0990208e7a09f9f3410badf59db381c1866155c6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.0 MB (31979649 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2d3d91b058afd21ca437377b7473a52073aa0b11fc5ef28725cc3ceb5352e912`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Tue, 09 Aug 2022 17:41:54 GMT
ADD file:7489fa84133e97e4f40b13dd5159989b3594c9627d9147bfc4e33134944cc368 in / 
# Tue, 09 Aug 2022 17:41:54 GMT
CMD ["/bin/sh"]
# Wed, 10 Aug 2022 05:50:07 GMT
RUN apk --no-cache add ca-certificates tzdata
# Tue, 13 Sep 2022 17:42:04 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.8.5/traefik_v2.8.5_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Tue, 13 Sep 2022 17:42:06 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Tue, 13 Sep 2022 17:42:06 GMT
EXPOSE 80
# Tue, 13 Sep 2022 17:42:06 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 13 Sep 2022 17:42:06 GMT
CMD ["traefik"]
# Tue, 13 Sep 2022 17:42:06 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.8.5 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:b9e70ad72dd57510b0aca527260bc2a85e4aa206a12a38c3811619286f798d78`  
		Last Modified: Tue, 13 Sep 2022 17:42:32 GMT  
		Size: 28.7 MB (28686667 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2ec4b4277bc0631824764df320de8fd7c7f98f5b13b57f2f8791e3ed6810ff2`  
		Last Modified: Tue, 13 Sep 2022 17:42:28 GMT  
		Size: 367.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v2.8-windowsservercore-1809`

```console
$ docker pull traefik@sha256:84b80d25f3a2267384a31d438bea47b75256258fe5c7d2d458312c5b35842792
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3406; amd64

### `traefik:v2.8-windowsservercore-1809` - windows version 10.0.17763.3406; amd64

```console
$ docker pull traefik@sha256:b7c78f8739641f8fb17ba16db5d4467fdc984239aea8c15a6a425d61a5a63726
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2733827197 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c628896d0a4bd9460b62a375fc22a99bb1c32bac428e3c5f3143bdaa85116816`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Fri, 09 Sep 2022 22:43:02 GMT
RUN Install update 10.0.17763.3406
# Tue, 13 Sep 2022 18:21:27 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 13 Sep 2022 18:23:34 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/traefik/traefik/releases/download/v2.8.5/traefik_v2.8.5_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Tue, 13 Sep 2022 18:23:35 GMT
EXPOSE 80
# Tue, 13 Sep 2022 18:23:36 GMT
ENTRYPOINT ["/traefik"]
# Tue, 13 Sep 2022 18:23:37 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.8.5 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:0a5a7a7fc317e347125a1f57626cf99448c897d1e193cb39b3389d0309790b1f`  
		Last Modified: Tue, 13 Sep 2022 18:25:31 GMT  
		Size: 30.3 MB (30256782 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1f48547d8e38f8f77d5668596e89f09cec313c88209ad1cb20cc912c938b6e2`  
		Last Modified: Tue, 13 Sep 2022 18:25:24 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f2c407588e5d1afb60580e8e82e167721e88544f91ff4e62a263ad4f7fea54b`  
		Last Modified: Tue, 13 Sep 2022 18:25:24 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e68faac36cb0c791f445fba14ab5ebe23ebca7a8e86628366c62aac87d03183f`  
		Last Modified: Tue, 13 Sep 2022 18:25:24 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v2.8.5`

```console
$ docker pull traefik@sha256:6793742cf3482a10529b4d18952c720bde9e75e9956a4f5f860179f74a771ab7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; s390x

### `traefik:v2.8.5` - linux; amd64

```console
$ docker pull traefik@sha256:9c663ef4155d64740028190a643f8cc21f5994b106475f790947d79ae9d93179
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.3 MB (33287410 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2caeed3432ab5acef8c4b71b525fb0e563f4923c96c601f8d0d6d889e5a2400c`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Tue, 09 Aug 2022 17:20:00 GMT
ADD file:f77e3f51f020890d22997e6c2ca98968b75b8bc8c463341a2010ff0655d4c88f in / 
# Tue, 09 Aug 2022 17:20:01 GMT
CMD ["/bin/sh"]
# Wed, 10 Aug 2022 01:24:52 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 14 Sep 2022 00:11:02 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.8.5/traefik_v2.8.5_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Wed, 14 Sep 2022 00:11:02 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 14 Sep 2022 00:11:02 GMT
EXPOSE 80
# Wed, 14 Sep 2022 00:11:03 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 14 Sep 2022 00:11:03 GMT
CMD ["traefik"]
# Wed, 14 Sep 2022 00:11:03 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.8.5 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:6bd3e1d95bf998a67bca95f32d5302a4b29a7f769dac8717b4a4010bca9f831b`  
		Last Modified: Wed, 14 Sep 2022 00:11:32 GMT  
		Size: 29.8 MB (29781857 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d269864b08bee0be42edc298f20fd989aa3a4611c472091809a0a0f180b418e4`  
		Last Modified: Wed, 14 Sep 2022 00:11:27 GMT  
		Size: 367.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v2.8.5` - linux; arm variant v6

```console
$ docker pull traefik@sha256:643f60f24294106bfe36e7b1c78031ecfd0bfd94565de3bdf04a36c3fa7cddb7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.4 MB (31416332 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4079bfbc61f417592a2daff4261b15468b2222f1ffbb4ed08d988eeb5ece3602`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Tue, 09 Aug 2022 17:49:29 GMT
ADD file:89cb25f97e17bed5c56311280efe5cfa78422d8ffbe36232195d13f94d67417e in / 
# Tue, 09 Aug 2022 17:49:29 GMT
CMD ["/bin/sh"]
# Thu, 11 Aug 2022 01:14:12 GMT
RUN apk --no-cache add ca-certificates tzdata
# Tue, 13 Sep 2022 17:49:51 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.8.5/traefik_v2.8.5_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Tue, 13 Sep 2022 17:49:51 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Tue, 13 Sep 2022 17:49:51 GMT
EXPOSE 80
# Tue, 13 Sep 2022 17:49:52 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 13 Sep 2022 17:49:52 GMT
CMD ["traefik"]
# Tue, 13 Sep 2022 17:49:52 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.8.5 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:168e12f01d9663d75ad85257e0fc771695a1b0256facbf3e55c05fd6c815c990`  
		Last Modified: Tue, 13 Sep 2022 17:51:20 GMT  
		Size: 28.1 MB (28098796 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c46c5e0d6400c1577faaa4b41baab6b0ac42755d3fe7a3c031a1ba159cb756e`  
		Last Modified: Tue, 13 Sep 2022 17:51:10 GMT  
		Size: 367.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v2.8.5` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:13ce7a5dc88cf420bdb4cf574fb5154774ecd5a08290c04375caa3c4431c8c18
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.6 MB (30578838 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8b4f3c81e83b1ab10bb06af37849c73b3bb4cf7e83bb31aa1a40829cbfc4e5fe`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Tue, 09 Aug 2022 17:39:51 GMT
ADD file:4b51a9d40f20d2beb29d0759b161d2b9403493453beb509de4e86a5d98513f16 in / 
# Tue, 09 Aug 2022 17:39:51 GMT
CMD ["/bin/sh"]
# Wed, 10 Aug 2022 06:10:52 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 14 Sep 2022 02:03:27 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.8.5/traefik_v2.8.5_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Wed, 14 Sep 2022 02:03:28 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 14 Sep 2022 02:03:28 GMT
EXPOSE 80
# Wed, 14 Sep 2022 02:03:29 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 14 Sep 2022 02:03:30 GMT
CMD ["traefik"]
# Wed, 14 Sep 2022 02:03:31 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.8.5 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:b1d629b95887fb97125620d51a69b9a4b51ec3a75ff37f9e3878b83d8a2bc573`  
		Last Modified: Wed, 14 Sep 2022 02:04:24 GMT  
		Size: 27.2 MB (27177636 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f3664d2a35c1a60ae1b15981994e7bebefe4ac64d031ecc280c68391c3432d8`  
		Last Modified: Wed, 14 Sep 2022 02:04:20 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v2.8.5` - linux; s390x

```console
$ docker pull traefik@sha256:dbbef98bd5e072eae0d938fb0990208e7a09f9f3410badf59db381c1866155c6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.0 MB (31979649 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2d3d91b058afd21ca437377b7473a52073aa0b11fc5ef28725cc3ceb5352e912`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Tue, 09 Aug 2022 17:41:54 GMT
ADD file:7489fa84133e97e4f40b13dd5159989b3594c9627d9147bfc4e33134944cc368 in / 
# Tue, 09 Aug 2022 17:41:54 GMT
CMD ["/bin/sh"]
# Wed, 10 Aug 2022 05:50:07 GMT
RUN apk --no-cache add ca-certificates tzdata
# Tue, 13 Sep 2022 17:42:04 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.8.5/traefik_v2.8.5_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Tue, 13 Sep 2022 17:42:06 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Tue, 13 Sep 2022 17:42:06 GMT
EXPOSE 80
# Tue, 13 Sep 2022 17:42:06 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 13 Sep 2022 17:42:06 GMT
CMD ["traefik"]
# Tue, 13 Sep 2022 17:42:06 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.8.5 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:b9e70ad72dd57510b0aca527260bc2a85e4aa206a12a38c3811619286f798d78`  
		Last Modified: Tue, 13 Sep 2022 17:42:32 GMT  
		Size: 28.7 MB (28686667 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2ec4b4277bc0631824764df320de8fd7c7f98f5b13b57f2f8791e3ed6810ff2`  
		Last Modified: Tue, 13 Sep 2022 17:42:28 GMT  
		Size: 367.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v2.8.5-windowsservercore-1809`

```console
$ docker pull traefik@sha256:84b80d25f3a2267384a31d438bea47b75256258fe5c7d2d458312c5b35842792
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3406; amd64

### `traefik:v2.8.5-windowsservercore-1809` - windows version 10.0.17763.3406; amd64

```console
$ docker pull traefik@sha256:b7c78f8739641f8fb17ba16db5d4467fdc984239aea8c15a6a425d61a5a63726
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2733827197 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c628896d0a4bd9460b62a375fc22a99bb1c32bac428e3c5f3143bdaa85116816`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Fri, 09 Sep 2022 22:43:02 GMT
RUN Install update 10.0.17763.3406
# Tue, 13 Sep 2022 18:21:27 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 13 Sep 2022 18:23:34 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/traefik/traefik/releases/download/v2.8.5/traefik_v2.8.5_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Tue, 13 Sep 2022 18:23:35 GMT
EXPOSE 80
# Tue, 13 Sep 2022 18:23:36 GMT
ENTRYPOINT ["/traefik"]
# Tue, 13 Sep 2022 18:23:37 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.8.5 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:0a5a7a7fc317e347125a1f57626cf99448c897d1e193cb39b3389d0309790b1f`  
		Last Modified: Tue, 13 Sep 2022 18:25:31 GMT  
		Size: 30.3 MB (30256782 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1f48547d8e38f8f77d5668596e89f09cec313c88209ad1cb20cc912c938b6e2`  
		Last Modified: Tue, 13 Sep 2022 18:25:24 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f2c407588e5d1afb60580e8e82e167721e88544f91ff4e62a263ad4f7fea54b`  
		Last Modified: Tue, 13 Sep 2022 18:25:24 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e68faac36cb0c791f445fba14ab5ebe23ebca7a8e86628366c62aac87d03183f`  
		Last Modified: Tue, 13 Sep 2022 18:25:24 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v2.9`

```console
$ docker pull traefik@sha256:85a6cc7ef661a606c90f582a84a1574ab2a7699b03319f34a39bfaab143c7a2f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; s390x

### `traefik:v2.9` - linux; amd64

```console
$ docker pull traefik@sha256:860e745b5a8c128ba7f834f709041de2b2576b1b2b8600961b6609c68896a950
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.4 MB (33415001 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:733f54fee3cb63f8b6c4318fbd00695fb4e7c1b0d83e24a2ccfd33b3d9c1b7c7`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Tue, 09 Aug 2022 17:20:00 GMT
ADD file:f77e3f51f020890d22997e6c2ca98968b75b8bc8c463341a2010ff0655d4c88f in / 
# Tue, 09 Aug 2022 17:20:01 GMT
CMD ["/bin/sh"]
# Wed, 10 Aug 2022 01:24:52 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 14 Sep 2022 17:31:12 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.9.0-rc2/traefik_v2.9.0-rc2_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Wed, 14 Sep 2022 17:31:12 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 14 Sep 2022 17:31:12 GMT
EXPOSE 80
# Wed, 14 Sep 2022 17:31:12 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 14 Sep 2022 17:31:12 GMT
CMD ["traefik"]
# Wed, 14 Sep 2022 17:31:12 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.9.0-rc2 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:1057a6f424b8065718d448e1341e44cc810c2efa5867ea06905a6155babb55cd`  
		Last Modified: Wed, 14 Sep 2022 17:31:48 GMT  
		Size: 29.9 MB (29909447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a53d84e31a10b690ee5915568293cefec447442f2a91c66c910c73a18ece40d7`  
		Last Modified: Wed, 14 Sep 2022 17:31:43 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v2.9` - linux; arm variant v6

```console
$ docker pull traefik@sha256:eab6cd20bed0ad8dfca482d1bdae2ba5a118cfa00a9086c2410ab059d6c26433
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.5 MB (31534900 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:43151892a1801b8be839577e0ae491e7ece6fa9206013b45f25b30d03df66f56`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Tue, 09 Aug 2022 17:49:29 GMT
ADD file:89cb25f97e17bed5c56311280efe5cfa78422d8ffbe36232195d13f94d67417e in / 
# Tue, 09 Aug 2022 17:49:29 GMT
CMD ["/bin/sh"]
# Thu, 11 Aug 2022 01:14:12 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 14 Sep 2022 16:49:40 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.9.0-rc2/traefik_v2.9.0-rc2_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Wed, 14 Sep 2022 16:49:40 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 14 Sep 2022 16:49:40 GMT
EXPOSE 80
# Wed, 14 Sep 2022 16:49:41 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 14 Sep 2022 16:49:41 GMT
CMD ["traefik"]
# Wed, 14 Sep 2022 16:49:41 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.9.0-rc2 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:e576a8d45a56333d4da8afd2ce3fd479e43dddfdaa224ecd0e06e049a68535f7`  
		Last Modified: Wed, 14 Sep 2022 16:51:06 GMT  
		Size: 28.2 MB (28217364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c553eb1fce4b36e147b198d55eccfe90c8e9a652a8186a179b66d72b21ba982`  
		Last Modified: Wed, 14 Sep 2022 16:50:59 GMT  
		Size: 367.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v2.9` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:942c80da34fd238da2411af8283c699b381e058bcb946b8d17c20a5543b126e4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.7 MB (30704146 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d905851689f22b1d5f2bf66996d4f107fa1d6a117d3f337e0385f6ef17a31964`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Tue, 09 Aug 2022 17:39:51 GMT
ADD file:4b51a9d40f20d2beb29d0759b161d2b9403493453beb509de4e86a5d98513f16 in / 
# Tue, 09 Aug 2022 17:39:51 GMT
CMD ["/bin/sh"]
# Wed, 10 Aug 2022 06:10:52 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 14 Sep 2022 17:48:53 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.9.0-rc2/traefik_v2.9.0-rc2_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Wed, 14 Sep 2022 17:48:55 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 14 Sep 2022 17:48:55 GMT
EXPOSE 80
# Wed, 14 Sep 2022 17:48:56 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 14 Sep 2022 17:48:57 GMT
CMD ["traefik"]
# Wed, 14 Sep 2022 17:48:58 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.9.0-rc2 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:90b7f8f6407af93928b4badc4e761d40e8913c6e1e1f5f3af889b67604ae2255`  
		Last Modified: Wed, 14 Sep 2022 17:50:03 GMT  
		Size: 27.3 MB (27302946 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:933489f19e2e5f601df880072d17e7726d2514e99a1fe6e3c297e290779e75d7`  
		Last Modified: Wed, 14 Sep 2022 17:50:00 GMT  
		Size: 366.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v2.9` - linux; s390x

```console
$ docker pull traefik@sha256:bd27728d6ed0565479ffcd1b1b1296eb5b8e3fdf1589302968884893c7f5286b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.1 MB (32104507 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c87694a06b62bdebebdc3950b2fcb8dc6f4ed3e34dd82d7baca9e2d77d840936`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Tue, 09 Aug 2022 17:41:54 GMT
ADD file:7489fa84133e97e4f40b13dd5159989b3594c9627d9147bfc4e33134944cc368 in / 
# Tue, 09 Aug 2022 17:41:54 GMT
CMD ["/bin/sh"]
# Wed, 10 Aug 2022 05:50:07 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 14 Sep 2022 17:44:01 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.9.0-rc2/traefik_v2.9.0-rc2_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Wed, 14 Sep 2022 17:44:02 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 14 Sep 2022 17:44:03 GMT
EXPOSE 80
# Wed, 14 Sep 2022 17:44:03 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 14 Sep 2022 17:44:03 GMT
CMD ["traefik"]
# Wed, 14 Sep 2022 17:44:03 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.9.0-rc2 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:97d39fe8daa11aed96420967fc20a46039da1f9685afa7c75c3a4644a8b5304f`  
		Last Modified: Wed, 14 Sep 2022 17:44:44 GMT  
		Size: 28.8 MB (28811524 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00c529102fa59c1aec188d12d972ed922d09a291141a8acf50e394c771a7c7a3`  
		Last Modified: Wed, 14 Sep 2022 17:44:40 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v2.9-windowsservercore-1809`

```console
$ docker pull traefik@sha256:b000b4e6e3726b437b7b1ace6b4c9e55cb7cc349da368bcd67c5ef957f57e191
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3406; amd64

### `traefik:v2.9-windowsservercore-1809` - windows version 10.0.17763.3406; amd64

```console
$ docker pull traefik@sha256:64e18eca374103f73e24568789ffb3c52c6a7b78e0c9c559dedf7929420ed0d0
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2733959697 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c0a892b2b4ba43a03cfff3fc8019d56e3974b0c5d642017973fcd5bec1fa130e`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Fri, 09 Sep 2022 22:43:02 GMT
RUN Install update 10.0.17763.3406
# Tue, 13 Sep 2022 18:21:27 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 14 Sep 2022 19:41:53 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/traefik/traefik/releases/download/v2.9.0-rc2/traefik_v2.9.0-rc2_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Wed, 14 Sep 2022 19:41:54 GMT
EXPOSE 80
# Wed, 14 Sep 2022 19:41:55 GMT
ENTRYPOINT ["/traefik"]
# Wed, 14 Sep 2022 19:41:56 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.9.0-rc2 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:6fd1d5543f6a70571fa830e350046a78addb303a36ede4233fa8fe4d809517ea`  
		Last Modified: Wed, 14 Sep 2022 19:42:48 GMT  
		Size: 30.4 MB (30389286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a88c552a6644064f7e4cba6d62cb1ccd22b59ccd989274c4e559c84dd9feb7ca`  
		Last Modified: Wed, 14 Sep 2022 19:42:42 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d70373754967f4a871e0e588a00155117e2932a7866ec732a6d7e64f919e4333`  
		Last Modified: Wed, 14 Sep 2022 19:42:42 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6170fe9fdc8d3820a4f4029ffc052a215b267811ac3a4cd5ee044cee7e93aa5`  
		Last Modified: Wed, 14 Sep 2022 19:42:42 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v2.9.0-rc2`

```console
$ docker pull traefik@sha256:85a6cc7ef661a606c90f582a84a1574ab2a7699b03319f34a39bfaab143c7a2f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; s390x

### `traefik:v2.9.0-rc2` - linux; amd64

```console
$ docker pull traefik@sha256:860e745b5a8c128ba7f834f709041de2b2576b1b2b8600961b6609c68896a950
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.4 MB (33415001 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:733f54fee3cb63f8b6c4318fbd00695fb4e7c1b0d83e24a2ccfd33b3d9c1b7c7`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Tue, 09 Aug 2022 17:20:00 GMT
ADD file:f77e3f51f020890d22997e6c2ca98968b75b8bc8c463341a2010ff0655d4c88f in / 
# Tue, 09 Aug 2022 17:20:01 GMT
CMD ["/bin/sh"]
# Wed, 10 Aug 2022 01:24:52 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 14 Sep 2022 17:31:12 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.9.0-rc2/traefik_v2.9.0-rc2_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Wed, 14 Sep 2022 17:31:12 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 14 Sep 2022 17:31:12 GMT
EXPOSE 80
# Wed, 14 Sep 2022 17:31:12 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 14 Sep 2022 17:31:12 GMT
CMD ["traefik"]
# Wed, 14 Sep 2022 17:31:12 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.9.0-rc2 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:1057a6f424b8065718d448e1341e44cc810c2efa5867ea06905a6155babb55cd`  
		Last Modified: Wed, 14 Sep 2022 17:31:48 GMT  
		Size: 29.9 MB (29909447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a53d84e31a10b690ee5915568293cefec447442f2a91c66c910c73a18ece40d7`  
		Last Modified: Wed, 14 Sep 2022 17:31:43 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v2.9.0-rc2` - linux; arm variant v6

```console
$ docker pull traefik@sha256:eab6cd20bed0ad8dfca482d1bdae2ba5a118cfa00a9086c2410ab059d6c26433
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.5 MB (31534900 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:43151892a1801b8be839577e0ae491e7ece6fa9206013b45f25b30d03df66f56`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Tue, 09 Aug 2022 17:49:29 GMT
ADD file:89cb25f97e17bed5c56311280efe5cfa78422d8ffbe36232195d13f94d67417e in / 
# Tue, 09 Aug 2022 17:49:29 GMT
CMD ["/bin/sh"]
# Thu, 11 Aug 2022 01:14:12 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 14 Sep 2022 16:49:40 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.9.0-rc2/traefik_v2.9.0-rc2_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Wed, 14 Sep 2022 16:49:40 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 14 Sep 2022 16:49:40 GMT
EXPOSE 80
# Wed, 14 Sep 2022 16:49:41 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 14 Sep 2022 16:49:41 GMT
CMD ["traefik"]
# Wed, 14 Sep 2022 16:49:41 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.9.0-rc2 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:e576a8d45a56333d4da8afd2ce3fd479e43dddfdaa224ecd0e06e049a68535f7`  
		Last Modified: Wed, 14 Sep 2022 16:51:06 GMT  
		Size: 28.2 MB (28217364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c553eb1fce4b36e147b198d55eccfe90c8e9a652a8186a179b66d72b21ba982`  
		Last Modified: Wed, 14 Sep 2022 16:50:59 GMT  
		Size: 367.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v2.9.0-rc2` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:942c80da34fd238da2411af8283c699b381e058bcb946b8d17c20a5543b126e4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.7 MB (30704146 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d905851689f22b1d5f2bf66996d4f107fa1d6a117d3f337e0385f6ef17a31964`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Tue, 09 Aug 2022 17:39:51 GMT
ADD file:4b51a9d40f20d2beb29d0759b161d2b9403493453beb509de4e86a5d98513f16 in / 
# Tue, 09 Aug 2022 17:39:51 GMT
CMD ["/bin/sh"]
# Wed, 10 Aug 2022 06:10:52 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 14 Sep 2022 17:48:53 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.9.0-rc2/traefik_v2.9.0-rc2_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Wed, 14 Sep 2022 17:48:55 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 14 Sep 2022 17:48:55 GMT
EXPOSE 80
# Wed, 14 Sep 2022 17:48:56 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 14 Sep 2022 17:48:57 GMT
CMD ["traefik"]
# Wed, 14 Sep 2022 17:48:58 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.9.0-rc2 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:90b7f8f6407af93928b4badc4e761d40e8913c6e1e1f5f3af889b67604ae2255`  
		Last Modified: Wed, 14 Sep 2022 17:50:03 GMT  
		Size: 27.3 MB (27302946 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:933489f19e2e5f601df880072d17e7726d2514e99a1fe6e3c297e290779e75d7`  
		Last Modified: Wed, 14 Sep 2022 17:50:00 GMT  
		Size: 366.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v2.9.0-rc2` - linux; s390x

```console
$ docker pull traefik@sha256:bd27728d6ed0565479ffcd1b1b1296eb5b8e3fdf1589302968884893c7f5286b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.1 MB (32104507 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c87694a06b62bdebebdc3950b2fcb8dc6f4ed3e34dd82d7baca9e2d77d840936`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Tue, 09 Aug 2022 17:41:54 GMT
ADD file:7489fa84133e97e4f40b13dd5159989b3594c9627d9147bfc4e33134944cc368 in / 
# Tue, 09 Aug 2022 17:41:54 GMT
CMD ["/bin/sh"]
# Wed, 10 Aug 2022 05:50:07 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 14 Sep 2022 17:44:01 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.9.0-rc2/traefik_v2.9.0-rc2_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Wed, 14 Sep 2022 17:44:02 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 14 Sep 2022 17:44:03 GMT
EXPOSE 80
# Wed, 14 Sep 2022 17:44:03 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 14 Sep 2022 17:44:03 GMT
CMD ["traefik"]
# Wed, 14 Sep 2022 17:44:03 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.9.0-rc2 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:97d39fe8daa11aed96420967fc20a46039da1f9685afa7c75c3a4644a8b5304f`  
		Last Modified: Wed, 14 Sep 2022 17:44:44 GMT  
		Size: 28.8 MB (28811524 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00c529102fa59c1aec188d12d972ed922d09a291141a8acf50e394c771a7c7a3`  
		Last Modified: Wed, 14 Sep 2022 17:44:40 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v2.9.0-rc2-windowsservercore-1809`

```console
$ docker pull traefik@sha256:b000b4e6e3726b437b7b1ace6b4c9e55cb7cc349da368bcd67c5ef957f57e191
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3406; amd64

### `traefik:v2.9.0-rc2-windowsservercore-1809` - windows version 10.0.17763.3406; amd64

```console
$ docker pull traefik@sha256:64e18eca374103f73e24568789ffb3c52c6a7b78e0c9c559dedf7929420ed0d0
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2733959697 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c0a892b2b4ba43a03cfff3fc8019d56e3974b0c5d642017973fcd5bec1fa130e`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Fri, 09 Sep 2022 22:43:02 GMT
RUN Install update 10.0.17763.3406
# Tue, 13 Sep 2022 18:21:27 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 14 Sep 2022 19:41:53 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/traefik/traefik/releases/download/v2.9.0-rc2/traefik_v2.9.0-rc2_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Wed, 14 Sep 2022 19:41:54 GMT
EXPOSE 80
# Wed, 14 Sep 2022 19:41:55 GMT
ENTRYPOINT ["/traefik"]
# Wed, 14 Sep 2022 19:41:56 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.9.0-rc2 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:6fd1d5543f6a70571fa830e350046a78addb303a36ede4233fa8fe4d809517ea`  
		Last Modified: Wed, 14 Sep 2022 19:42:48 GMT  
		Size: 30.4 MB (30389286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a88c552a6644064f7e4cba6d62cb1ccd22b59ccd989274c4e559c84dd9feb7ca`  
		Last Modified: Wed, 14 Sep 2022 19:42:42 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d70373754967f4a871e0e588a00155117e2932a7866ec732a6d7e64f919e4333`  
		Last Modified: Wed, 14 Sep 2022 19:42:42 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6170fe9fdc8d3820a4f4029ffc052a215b267811ac3a4cd5ee044cee7e93aa5`  
		Last Modified: Wed, 14 Sep 2022 19:42:42 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:vacherin`

```console
$ docker pull traefik@sha256:6793742cf3482a10529b4d18952c720bde9e75e9956a4f5f860179f74a771ab7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; s390x

### `traefik:vacherin` - linux; amd64

```console
$ docker pull traefik@sha256:9c663ef4155d64740028190a643f8cc21f5994b106475f790947d79ae9d93179
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.3 MB (33287410 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2caeed3432ab5acef8c4b71b525fb0e563f4923c96c601f8d0d6d889e5a2400c`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Tue, 09 Aug 2022 17:20:00 GMT
ADD file:f77e3f51f020890d22997e6c2ca98968b75b8bc8c463341a2010ff0655d4c88f in / 
# Tue, 09 Aug 2022 17:20:01 GMT
CMD ["/bin/sh"]
# Wed, 10 Aug 2022 01:24:52 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 14 Sep 2022 00:11:02 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.8.5/traefik_v2.8.5_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Wed, 14 Sep 2022 00:11:02 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 14 Sep 2022 00:11:02 GMT
EXPOSE 80
# Wed, 14 Sep 2022 00:11:03 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 14 Sep 2022 00:11:03 GMT
CMD ["traefik"]
# Wed, 14 Sep 2022 00:11:03 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.8.5 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:6bd3e1d95bf998a67bca95f32d5302a4b29a7f769dac8717b4a4010bca9f831b`  
		Last Modified: Wed, 14 Sep 2022 00:11:32 GMT  
		Size: 29.8 MB (29781857 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d269864b08bee0be42edc298f20fd989aa3a4611c472091809a0a0f180b418e4`  
		Last Modified: Wed, 14 Sep 2022 00:11:27 GMT  
		Size: 367.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:vacherin` - linux; arm variant v6

```console
$ docker pull traefik@sha256:643f60f24294106bfe36e7b1c78031ecfd0bfd94565de3bdf04a36c3fa7cddb7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.4 MB (31416332 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4079bfbc61f417592a2daff4261b15468b2222f1ffbb4ed08d988eeb5ece3602`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Tue, 09 Aug 2022 17:49:29 GMT
ADD file:89cb25f97e17bed5c56311280efe5cfa78422d8ffbe36232195d13f94d67417e in / 
# Tue, 09 Aug 2022 17:49:29 GMT
CMD ["/bin/sh"]
# Thu, 11 Aug 2022 01:14:12 GMT
RUN apk --no-cache add ca-certificates tzdata
# Tue, 13 Sep 2022 17:49:51 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.8.5/traefik_v2.8.5_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Tue, 13 Sep 2022 17:49:51 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Tue, 13 Sep 2022 17:49:51 GMT
EXPOSE 80
# Tue, 13 Sep 2022 17:49:52 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 13 Sep 2022 17:49:52 GMT
CMD ["traefik"]
# Tue, 13 Sep 2022 17:49:52 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.8.5 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:168e12f01d9663d75ad85257e0fc771695a1b0256facbf3e55c05fd6c815c990`  
		Last Modified: Tue, 13 Sep 2022 17:51:20 GMT  
		Size: 28.1 MB (28098796 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c46c5e0d6400c1577faaa4b41baab6b0ac42755d3fe7a3c031a1ba159cb756e`  
		Last Modified: Tue, 13 Sep 2022 17:51:10 GMT  
		Size: 367.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:vacherin` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:13ce7a5dc88cf420bdb4cf574fb5154774ecd5a08290c04375caa3c4431c8c18
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.6 MB (30578838 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8b4f3c81e83b1ab10bb06af37849c73b3bb4cf7e83bb31aa1a40829cbfc4e5fe`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Tue, 09 Aug 2022 17:39:51 GMT
ADD file:4b51a9d40f20d2beb29d0759b161d2b9403493453beb509de4e86a5d98513f16 in / 
# Tue, 09 Aug 2022 17:39:51 GMT
CMD ["/bin/sh"]
# Wed, 10 Aug 2022 06:10:52 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 14 Sep 2022 02:03:27 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.8.5/traefik_v2.8.5_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Wed, 14 Sep 2022 02:03:28 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 14 Sep 2022 02:03:28 GMT
EXPOSE 80
# Wed, 14 Sep 2022 02:03:29 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 14 Sep 2022 02:03:30 GMT
CMD ["traefik"]
# Wed, 14 Sep 2022 02:03:31 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.8.5 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:b1d629b95887fb97125620d51a69b9a4b51ec3a75ff37f9e3878b83d8a2bc573`  
		Last Modified: Wed, 14 Sep 2022 02:04:24 GMT  
		Size: 27.2 MB (27177636 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f3664d2a35c1a60ae1b15981994e7bebefe4ac64d031ecc280c68391c3432d8`  
		Last Modified: Wed, 14 Sep 2022 02:04:20 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:vacherin` - linux; s390x

```console
$ docker pull traefik@sha256:dbbef98bd5e072eae0d938fb0990208e7a09f9f3410badf59db381c1866155c6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.0 MB (31979649 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2d3d91b058afd21ca437377b7473a52073aa0b11fc5ef28725cc3ceb5352e912`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Tue, 09 Aug 2022 17:41:54 GMT
ADD file:7489fa84133e97e4f40b13dd5159989b3594c9627d9147bfc4e33134944cc368 in / 
# Tue, 09 Aug 2022 17:41:54 GMT
CMD ["/bin/sh"]
# Wed, 10 Aug 2022 05:50:07 GMT
RUN apk --no-cache add ca-certificates tzdata
# Tue, 13 Sep 2022 17:42:04 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.8.5/traefik_v2.8.5_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Tue, 13 Sep 2022 17:42:06 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Tue, 13 Sep 2022 17:42:06 GMT
EXPOSE 80
# Tue, 13 Sep 2022 17:42:06 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 13 Sep 2022 17:42:06 GMT
CMD ["traefik"]
# Tue, 13 Sep 2022 17:42:06 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.8.5 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:b9e70ad72dd57510b0aca527260bc2a85e4aa206a12a38c3811619286f798d78`  
		Last Modified: Tue, 13 Sep 2022 17:42:32 GMT  
		Size: 28.7 MB (28686667 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2ec4b4277bc0631824764df320de8fd7c7f98f5b13b57f2f8791e3ed6810ff2`  
		Last Modified: Tue, 13 Sep 2022 17:42:28 GMT  
		Size: 367.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:vacherin-windowsservercore-1809`

```console
$ docker pull traefik@sha256:84b80d25f3a2267384a31d438bea47b75256258fe5c7d2d458312c5b35842792
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3406; amd64

### `traefik:vacherin-windowsservercore-1809` - windows version 10.0.17763.3406; amd64

```console
$ docker pull traefik@sha256:b7c78f8739641f8fb17ba16db5d4467fdc984239aea8c15a6a425d61a5a63726
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2733827197 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c628896d0a4bd9460b62a375fc22a99bb1c32bac428e3c5f3143bdaa85116816`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Fri, 09 Sep 2022 22:43:02 GMT
RUN Install update 10.0.17763.3406
# Tue, 13 Sep 2022 18:21:27 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 13 Sep 2022 18:23:34 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/traefik/traefik/releases/download/v2.8.5/traefik_v2.8.5_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Tue, 13 Sep 2022 18:23:35 GMT
EXPOSE 80
# Tue, 13 Sep 2022 18:23:36 GMT
ENTRYPOINT ["/traefik"]
# Tue, 13 Sep 2022 18:23:37 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.8.5 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:0a5a7a7fc317e347125a1f57626cf99448c897d1e193cb39b3389d0309790b1f`  
		Last Modified: Tue, 13 Sep 2022 18:25:31 GMT  
		Size: 30.3 MB (30256782 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1f48547d8e38f8f77d5668596e89f09cec313c88209ad1cb20cc912c938b6e2`  
		Last Modified: Tue, 13 Sep 2022 18:25:24 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f2c407588e5d1afb60580e8e82e167721e88544f91ff4e62a263ad4f7fea54b`  
		Last Modified: Tue, 13 Sep 2022 18:25:24 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e68faac36cb0c791f445fba14ab5ebe23ebca7a8e86628366c62aac87d03183f`  
		Last Modified: Tue, 13 Sep 2022 18:25:24 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:windowsservercore-1809`

```console
$ docker pull traefik@sha256:84b80d25f3a2267384a31d438bea47b75256258fe5c7d2d458312c5b35842792
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3406; amd64

### `traefik:windowsservercore-1809` - windows version 10.0.17763.3406; amd64

```console
$ docker pull traefik@sha256:b7c78f8739641f8fb17ba16db5d4467fdc984239aea8c15a6a425d61a5a63726
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2733827197 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c628896d0a4bd9460b62a375fc22a99bb1c32bac428e3c5f3143bdaa85116816`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Fri, 09 Sep 2022 22:43:02 GMT
RUN Install update 10.0.17763.3406
# Tue, 13 Sep 2022 18:21:27 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 13 Sep 2022 18:23:34 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/traefik/traefik/releases/download/v2.8.5/traefik_v2.8.5_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Tue, 13 Sep 2022 18:23:35 GMT
EXPOSE 80
# Tue, 13 Sep 2022 18:23:36 GMT
ENTRYPOINT ["/traefik"]
# Tue, 13 Sep 2022 18:23:37 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.8.5 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:0a5a7a7fc317e347125a1f57626cf99448c897d1e193cb39b3389d0309790b1f`  
		Last Modified: Tue, 13 Sep 2022 18:25:31 GMT  
		Size: 30.3 MB (30256782 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1f48547d8e38f8f77d5668596e89f09cec313c88209ad1cb20cc912c938b6e2`  
		Last Modified: Tue, 13 Sep 2022 18:25:24 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f2c407588e5d1afb60580e8e82e167721e88544f91ff4e62a263ad4f7fea54b`  
		Last Modified: Tue, 13 Sep 2022 18:25:24 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e68faac36cb0c791f445fba14ab5ebe23ebca7a8e86628366c62aac87d03183f`  
		Last Modified: Tue, 13 Sep 2022 18:25:24 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
