<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `traefik`

-	[`traefik:1.7`](#traefik17)
-	[`traefik:1.7-alpine`](#traefik17-alpine)
-	[`traefik:1.7-windowsservercore-1809`](#traefik17-windowsservercore-1809)
-	[`traefik:1.7.34`](#traefik1734)
-	[`traefik:1.7.34-alpine`](#traefik1734-alpine)
-	[`traefik:1.7.34-windowsservercore-1809`](#traefik1734-windowsservercore-1809)
-	[`traefik:2.6`](#traefik26)
-	[`traefik:2.6-windowsservercore-1809`](#traefik26-windowsservercore-1809)
-	[`traefik:2.6.1`](#traefik261)
-	[`traefik:2.6.1-windowsservercore-1809`](#traefik261-windowsservercore-1809)
-	[`traefik:latest`](#traefiklatest)
-	[`traefik:maroilles`](#traefikmaroilles)
-	[`traefik:maroilles-alpine`](#traefikmaroilles-alpine)
-	[`traefik:maroilles-windowsservercore-1809`](#traefikmaroilles-windowsservercore-1809)
-	[`traefik:rocamadour`](#traefikrocamadour)
-	[`traefik:rocamadour-windowsservercore-1809`](#traefikrocamadour-windowsservercore-1809)
-	[`traefik:v1.7`](#traefikv17)
-	[`traefik:v1.7-alpine`](#traefikv17-alpine)
-	[`traefik:v1.7-windowsservercore-1809`](#traefikv17-windowsservercore-1809)
-	[`traefik:v1.7.34`](#traefikv1734)
-	[`traefik:v1.7.34-alpine`](#traefikv1734-alpine)
-	[`traefik:v1.7.34-windowsservercore-1809`](#traefikv1734-windowsservercore-1809)
-	[`traefik:v2.6`](#traefikv26)
-	[`traefik:v2.6-windowsservercore-1809`](#traefikv26-windowsservercore-1809)
-	[`traefik:v2.6.1`](#traefikv261)
-	[`traefik:v2.6.1-windowsservercore-1809`](#traefikv261-windowsservercore-1809)
-	[`traefik:windowsservercore-1809`](#traefikwindowsservercore-1809)

## `traefik:1.7`

```console
$ docker pull traefik@sha256:1d8a41ae1bd54c9e9a5e0cc8da9002638932c53cc3d50c6f0c172238374ebe8f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:1.7` - linux; amd64

```console
$ docker pull traefik@sha256:f705216279431ed8ab470318736acd767794a847acda2db325e3e159574bd03c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **22.6 MB (22607863 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:43de28b34d397393ca2d0ec8bd6923735fab787f8c3bd3dab0719cd256fcc010`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Fri, 18 Mar 2022 06:23:36 GMT
COPY file:8536203e9de8580f4424aff73a3be4185daba1818e4bfa286f2b290d1459aeb9 in /etc/ssl/certs/ 
# Fri, 18 Mar 2022 06:23:37 GMT
COPY dir:a84372748b89eb90478bb1b120b7c8fff3112421d7f93e50fbeae3f53adc6788 in /usr/share/ 
# Fri, 18 Mar 2022 06:23:38 GMT
COPY file:36217e5a6056bef26cfff395c8af8c1010a61dbe8d62b2c7869ca221e2a6302c in / 
# Fri, 18 Mar 2022 06:23:39 GMT
EXPOSE 80
# Fri, 18 Mar 2022 06:23:39 GMT
VOLUME [/tmp]
# Fri, 18 Mar 2022 06:23:39 GMT
ENTRYPOINT ["/traefik"]
# Fri, 18 Mar 2022 06:23:39 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.34 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:903e84870d1b7b581b2c6c362c74751a258cb8e2dbb443bddcd36fe8f29a20ab`  
		Last Modified: Fri, 18 Mar 2022 06:24:59 GMT  
		Size: 117.4 KB (117389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:914ae7a2b8652023026596365a1dfe88e317d16b1cc8099ee03c20357c95716e`  
		Last Modified: Fri, 18 Mar 2022 06:25:00 GMT  
		Size: 328.5 KB (328522 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f483c7bcad16f6ac0813c7a4704d4dc9319bfd6533f10c888b5e2ca21c72dc44`  
		Last Modified: Fri, 18 Mar 2022 06:25:05 GMT  
		Size: 22.2 MB (22161952 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:1.7` - linux; arm variant v6

```console
$ docker pull traefik@sha256:fe6bde6e9349ec036bc3aaec90c095006425bface50ee2f449e0d196cb5850c7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **21.1 MB (21069186 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5a5c3451377ef5e2379e4bc19691fb6c14b1a2215326833336e1db9e16cc5ca3`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Thu, 17 Mar 2022 22:45:25 GMT
COPY file:8536203e9de8580f4424aff73a3be4185daba1818e4bfa286f2b290d1459aeb9 in /etc/ssl/certs/ 
# Thu, 17 Mar 2022 22:45:27 GMT
COPY dir:a84372748b89eb90478bb1b120b7c8fff3112421d7f93e50fbeae3f53adc6788 in /usr/share/ 
# Thu, 17 Mar 2022 22:45:32 GMT
COPY file:5d1e7e81e8b77b4f8828eeaf0d30a0f135a949b51396f12ae22af376c36d3129 in / 
# Thu, 17 Mar 2022 22:45:33 GMT
EXPOSE 80
# Thu, 17 Mar 2022 22:45:33 GMT
VOLUME [/tmp]
# Thu, 17 Mar 2022 22:45:34 GMT
ENTRYPOINT ["/traefik"]
# Thu, 17 Mar 2022 22:45:34 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.34 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:27b61c1d4effca5c7137bfe0c8b6a3a228418ef37998781ad6cc7372c6f7e98f`  
		Last Modified: Thu, 17 Mar 2022 22:48:17 GMT  
		Size: 117.4 KB (117390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98aae3b48a316f885b1d485fee6b2ffffb3c2c7dea49cea01019d4c103b204da`  
		Last Modified: Thu, 17 Mar 2022 22:48:18 GMT  
		Size: 328.5 KB (328514 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a82873a2be1cc2b2dfbc565c4bf9960f32b61892f49f0911ec1ac7e310210c3d`  
		Last Modified: Thu, 17 Mar 2022 22:48:34 GMT  
		Size: 20.6 MB (20623282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:1.7` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:c2930d3e36f7feb98470b85e8bc9fce0016fc5eadbc805249e63d6a458eb2323
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **20.6 MB (20577242 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f7338e148255e82dd93286a1f87db35f499d4e391d7f5f3e1bfb6c71ed4ec2d4`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Thu, 17 Mar 2022 21:07:07 GMT
COPY file:8536203e9de8580f4424aff73a3be4185daba1818e4bfa286f2b290d1459aeb9 in /etc/ssl/certs/ 
# Thu, 17 Mar 2022 21:07:08 GMT
COPY dir:a84372748b89eb90478bb1b120b7c8fff3112421d7f93e50fbeae3f53adc6788 in /usr/share/ 
# Thu, 17 Mar 2022 21:07:09 GMT
COPY file:60330593b6644f3f519fd13ce8ee34c2c7ab9994a1420afabbc01926dd1230dd in / 
# Thu, 17 Mar 2022 21:07:09 GMT
EXPOSE 80
# Thu, 17 Mar 2022 21:07:10 GMT
VOLUME [/tmp]
# Thu, 17 Mar 2022 21:07:11 GMT
ENTRYPOINT ["/traefik"]
# Thu, 17 Mar 2022 21:07:12 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.34 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:86cd07830d2730c0aa24f0e47380af5ef760945b5049a2e72a8ebe0675ed6d34`  
		Last Modified: Thu, 17 Mar 2022 21:08:41 GMT  
		Size: 117.4 KB (117390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:135b9e65a5ea0b642df02ea2cf73c74a353d1cbfa3b95d048a4adbf0bacf9653`  
		Last Modified: Thu, 17 Mar 2022 21:08:41 GMT  
		Size: 328.5 KB (328505 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bee8fa09b05c38fc9116b1446ac3d204200577fd9bfb1801d684657dc722b74b`  
		Last Modified: Thu, 17 Mar 2022 21:08:45 GMT  
		Size: 20.1 MB (20131347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:1.7-alpine`

```console
$ docker pull traefik@sha256:8ac75422d559a55193d20df11116ea951ad962f7dcdf3bd76a51f81f460de821
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:1.7-alpine` - linux; amd64

```console
$ docker pull traefik@sha256:04c41c7c3ff03d006e93029fb6bce95a448a32900c47487cf2f54f4df2d42f56
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.6 MB (25645268 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9eb8c5f993e88b67da6b9d2b5ee0a09e7f6a576c70e19f8bd1031adae54418ca`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 17 Mar 2022 15:19:26 GMT
ADD file:8ec3735d4b1b4b070607b94e3bd360117b07dc26e1baf5dd485b49b3413e8fff in / 
# Thu, 17 Mar 2022 15:19:26 GMT
CMD ["/bin/sh"]
# Fri, 18 Mar 2022 06:23:06 GMT
RUN apk --no-cache add ca-certificates tzdata
# Fri, 18 Mar 2022 06:23:24 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/traefik/traefik/releases/download/v1.7.34/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Fri, 18 Mar 2022 06:23:24 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Fri, 18 Mar 2022 06:23:24 GMT
EXPOSE 80
# Fri, 18 Mar 2022 06:23:24 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 18 Mar 2022 06:23:24 GMT
CMD ["traefik"]
# Fri, 18 Mar 2022 06:23:25 GMT
LABEL org.opencontainers.image.vendor=traefik org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.34 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:36ccefbf3d8a9a1b18baaa9cbf0f3ad50e8a7b751656c74df359900a318cbffc`  
		Last Modified: Thu, 17 Mar 2022 15:20:13 GMT  
		Size: 2.8 MB (2816169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d66f86d3f60579f394506161f82aafee52b414cd58c1060e18ca607a4fc9fbc4`  
		Last Modified: Fri, 18 Mar 2022 06:24:10 GMT  
		Size: 666.7 KB (666670 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b9a06ba42895ffa47fb412ee9c0fe6cc5c33d4bf08ca4a76e74f7040bc82206`  
		Last Modified: Fri, 18 Mar 2022 06:24:42 GMT  
		Size: 22.2 MB (22162062 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b266beb8763fa8eeb482f01673624fb468758ac98bb28cc16881d8f94e1f54c`  
		Last Modified: Fri, 18 Mar 2022 06:24:36 GMT  
		Size: 367.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:1.7-alpine` - linux; arm variant v6

```console
$ docker pull traefik@sha256:08be027ed453b435111cb912908324ee1f5f0d77db60b6d6f9f10003d2c62674
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.9 MB (23925625 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d5fbe3dd0a206256fa43655ee4af71da94003b6377978bc54ccdb219452f1bcc`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 17 Mar 2022 14:32:33 GMT
ADD file:8f1611b9334907a82945fdb21e17ee41541ab95050fc199c60fca662759171a5 in / 
# Thu, 17 Mar 2022 14:32:33 GMT
CMD ["/bin/sh"]
# Thu, 17 Mar 2022 22:44:31 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 17 Mar 2022 22:45:03 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/traefik/traefik/releases/download/v1.7.34/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Thu, 17 Mar 2022 22:45:03 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 17 Mar 2022 22:45:04 GMT
EXPOSE 80
# Thu, 17 Mar 2022 22:45:05 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 17 Mar 2022 22:45:05 GMT
CMD ["traefik"]
# Thu, 17 Mar 2022 22:45:06 GMT
LABEL org.opencontainers.image.vendor=traefik org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.34 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:4025825e6ef43541c3a3e1ecb0092bc1b098e792051c7e338d6da54f66b19661`  
		Last Modified: Thu, 17 Mar 2022 14:34:09 GMT  
		Size: 2.6 MB (2629364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acc61b01c9ae829babc4ec995a57d752de240cbe8e3a8660191d3d21fc589a5f`  
		Last Modified: Thu, 17 Mar 2022 22:46:57 GMT  
		Size: 672.5 KB (672470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:244182210987061535c909a9a2aace43df0eb4ee95953b8813c3792dd4ba5b37`  
		Last Modified: Thu, 17 Mar 2022 22:47:55 GMT  
		Size: 20.6 MB (20623423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb981a93f73996a8309c5494870b9e83074dae0470e145590d2148af320281cf`  
		Last Modified: Thu, 17 Mar 2022 22:47:40 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:1.7-alpine` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:1e7c544b79ed103ad6d22cd9941ca3416e02897a9cb7f75120f6fd5f1949d90c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.5 MB (23515893 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:11a718e3a556a699675cb6d5655875c7240cd58d718536719147125b9d171870`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 17 Mar 2022 18:43:12 GMT
ADD file:611998b78638b13e78919dd4635674032ab233f9b7aae6f62beaf6634cd18b9e in / 
# Thu, 17 Mar 2022 18:43:13 GMT
CMD ["/bin/sh"]
# Thu, 17 Mar 2022 21:06:35 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 17 Mar 2022 21:06:53 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/traefik/traefik/releases/download/v1.7.34/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Thu, 17 Mar 2022 21:06:55 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 17 Mar 2022 21:06:55 GMT
EXPOSE 80
# Thu, 17 Mar 2022 21:06:56 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 17 Mar 2022 21:06:57 GMT
CMD ["traefik"]
# Thu, 17 Mar 2022 21:06:58 GMT
LABEL org.opencontainers.image.vendor=traefik org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.34 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:93a1719cf26168d3a85db2594d76b17ccc4b25996620bceed3c2a13eaa165325`  
		Last Modified: Thu, 17 Mar 2022 18:44:00 GMT  
		Size: 2.7 MB (2715888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d012a4d53d2ad42f0d1b24f774778f1ea2d1c67cfdd0a1611fb7652fac92fc9b`  
		Last Modified: Thu, 17 Mar 2022 21:07:51 GMT  
		Size: 668.3 KB (668255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe57c71a6e6bc8b2eda9db22fd05c14079977728ba28062721c5d71106b23ab9`  
		Last Modified: Thu, 17 Mar 2022 21:08:21 GMT  
		Size: 20.1 MB (20131382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:535366a8854793a298d798c23544e4ad0849c13ce51c5687ad00f9864bebe75a`  
		Last Modified: Thu, 17 Mar 2022 21:08:18 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:1.7-windowsservercore-1809`

```console
$ docker pull traefik@sha256:85ffe3d43fd4929a0e48d226e018af240fbbd8ea9a03685f74f1c78c432f85b3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2686; amd64

### `traefik:1.7-windowsservercore-1809` - windows version 10.0.17763.2686; amd64

```console
$ docker pull traefik@sha256:67d210fa3d7dcb1ebc3b3b5f3bfdaac7d18195e1bb2b83fa2c1b1f48d09b08dd
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2738303983 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d6ebd04310fbdd68b4e7225310f8a6f2dec3a0330af0d02b74a9a0e35b79945b`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 03 Mar 2022 15:05:04 GMT
RUN Install update 1809-amd64
# Tue, 08 Mar 2022 19:31:54 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Mar 2022 18:53:09 GMT
RUN Invoke-WebRequest     -Uri "https://github.com/traefik/traefik/releases/download/v1.7.34/traefik_windows-amd64.exe"     -OutFile "/traefik.exe"
# Wed, 09 Mar 2022 18:53:10 GMT
EXPOSE 80
# Wed, 09 Mar 2022 18:53:11 GMT
ENTRYPOINT ["/traefik"]
# Wed, 09 Mar 2022 18:53:12 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.34 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:0a6173b79e25f2ebc0ed51b0ac32a6f65ca5a3bbfcbeab8b74a6c24324121dea`  
		Size: 997.1 MB (997119751 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a42bef5ec276ee3f8dd3545bf050f4ab85c8191392884f5d5ad6af6ae6e2eed2`  
		Last Modified: Tue, 08 Mar 2022 20:01:19 GMT  
		Size: 1.3 KB (1323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fd63edc5d2bde654b771ee58c8e9bb78539127758e862053223f402d3eaea68`  
		Last Modified: Wed, 09 Mar 2022 18:54:50 GMT  
		Size: 22.8 MB (22845783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cefe3e1f9703a33ffdf92a9c03b8a4738222fe08ea99aded6416f848aa300e9`  
		Last Modified: Wed, 09 Mar 2022 18:54:27 GMT  
		Size: 1.4 KB (1446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:939f3b18eb0ddb1cb4c6b01a2abc4127403c6a67c630a8c05c6be5f43ab74acc`  
		Last Modified: Wed, 09 Mar 2022 18:54:26 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35bcba10ab84d161e2dc32a48f6bc15da23d8aabdb22bbf4a89499ce18583d46`  
		Last Modified: Wed, 09 Mar 2022 18:54:26 GMT  
		Size: 1.4 KB (1389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:1.7.34`

```console
$ docker pull traefik@sha256:1d8a41ae1bd54c9e9a5e0cc8da9002638932c53cc3d50c6f0c172238374ebe8f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:1.7.34` - linux; amd64

```console
$ docker pull traefik@sha256:f705216279431ed8ab470318736acd767794a847acda2db325e3e159574bd03c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **22.6 MB (22607863 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:43de28b34d397393ca2d0ec8bd6923735fab787f8c3bd3dab0719cd256fcc010`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Fri, 18 Mar 2022 06:23:36 GMT
COPY file:8536203e9de8580f4424aff73a3be4185daba1818e4bfa286f2b290d1459aeb9 in /etc/ssl/certs/ 
# Fri, 18 Mar 2022 06:23:37 GMT
COPY dir:a84372748b89eb90478bb1b120b7c8fff3112421d7f93e50fbeae3f53adc6788 in /usr/share/ 
# Fri, 18 Mar 2022 06:23:38 GMT
COPY file:36217e5a6056bef26cfff395c8af8c1010a61dbe8d62b2c7869ca221e2a6302c in / 
# Fri, 18 Mar 2022 06:23:39 GMT
EXPOSE 80
# Fri, 18 Mar 2022 06:23:39 GMT
VOLUME [/tmp]
# Fri, 18 Mar 2022 06:23:39 GMT
ENTRYPOINT ["/traefik"]
# Fri, 18 Mar 2022 06:23:39 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.34 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:903e84870d1b7b581b2c6c362c74751a258cb8e2dbb443bddcd36fe8f29a20ab`  
		Last Modified: Fri, 18 Mar 2022 06:24:59 GMT  
		Size: 117.4 KB (117389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:914ae7a2b8652023026596365a1dfe88e317d16b1cc8099ee03c20357c95716e`  
		Last Modified: Fri, 18 Mar 2022 06:25:00 GMT  
		Size: 328.5 KB (328522 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f483c7bcad16f6ac0813c7a4704d4dc9319bfd6533f10c888b5e2ca21c72dc44`  
		Last Modified: Fri, 18 Mar 2022 06:25:05 GMT  
		Size: 22.2 MB (22161952 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:1.7.34` - linux; arm variant v6

```console
$ docker pull traefik@sha256:fe6bde6e9349ec036bc3aaec90c095006425bface50ee2f449e0d196cb5850c7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **21.1 MB (21069186 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5a5c3451377ef5e2379e4bc19691fb6c14b1a2215326833336e1db9e16cc5ca3`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Thu, 17 Mar 2022 22:45:25 GMT
COPY file:8536203e9de8580f4424aff73a3be4185daba1818e4bfa286f2b290d1459aeb9 in /etc/ssl/certs/ 
# Thu, 17 Mar 2022 22:45:27 GMT
COPY dir:a84372748b89eb90478bb1b120b7c8fff3112421d7f93e50fbeae3f53adc6788 in /usr/share/ 
# Thu, 17 Mar 2022 22:45:32 GMT
COPY file:5d1e7e81e8b77b4f8828eeaf0d30a0f135a949b51396f12ae22af376c36d3129 in / 
# Thu, 17 Mar 2022 22:45:33 GMT
EXPOSE 80
# Thu, 17 Mar 2022 22:45:33 GMT
VOLUME [/tmp]
# Thu, 17 Mar 2022 22:45:34 GMT
ENTRYPOINT ["/traefik"]
# Thu, 17 Mar 2022 22:45:34 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.34 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:27b61c1d4effca5c7137bfe0c8b6a3a228418ef37998781ad6cc7372c6f7e98f`  
		Last Modified: Thu, 17 Mar 2022 22:48:17 GMT  
		Size: 117.4 KB (117390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98aae3b48a316f885b1d485fee6b2ffffb3c2c7dea49cea01019d4c103b204da`  
		Last Modified: Thu, 17 Mar 2022 22:48:18 GMT  
		Size: 328.5 KB (328514 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a82873a2be1cc2b2dfbc565c4bf9960f32b61892f49f0911ec1ac7e310210c3d`  
		Last Modified: Thu, 17 Mar 2022 22:48:34 GMT  
		Size: 20.6 MB (20623282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:1.7.34` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:c2930d3e36f7feb98470b85e8bc9fce0016fc5eadbc805249e63d6a458eb2323
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **20.6 MB (20577242 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f7338e148255e82dd93286a1f87db35f499d4e391d7f5f3e1bfb6c71ed4ec2d4`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Thu, 17 Mar 2022 21:07:07 GMT
COPY file:8536203e9de8580f4424aff73a3be4185daba1818e4bfa286f2b290d1459aeb9 in /etc/ssl/certs/ 
# Thu, 17 Mar 2022 21:07:08 GMT
COPY dir:a84372748b89eb90478bb1b120b7c8fff3112421d7f93e50fbeae3f53adc6788 in /usr/share/ 
# Thu, 17 Mar 2022 21:07:09 GMT
COPY file:60330593b6644f3f519fd13ce8ee34c2c7ab9994a1420afabbc01926dd1230dd in / 
# Thu, 17 Mar 2022 21:07:09 GMT
EXPOSE 80
# Thu, 17 Mar 2022 21:07:10 GMT
VOLUME [/tmp]
# Thu, 17 Mar 2022 21:07:11 GMT
ENTRYPOINT ["/traefik"]
# Thu, 17 Mar 2022 21:07:12 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.34 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:86cd07830d2730c0aa24f0e47380af5ef760945b5049a2e72a8ebe0675ed6d34`  
		Last Modified: Thu, 17 Mar 2022 21:08:41 GMT  
		Size: 117.4 KB (117390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:135b9e65a5ea0b642df02ea2cf73c74a353d1cbfa3b95d048a4adbf0bacf9653`  
		Last Modified: Thu, 17 Mar 2022 21:08:41 GMT  
		Size: 328.5 KB (328505 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bee8fa09b05c38fc9116b1446ac3d204200577fd9bfb1801d684657dc722b74b`  
		Last Modified: Thu, 17 Mar 2022 21:08:45 GMT  
		Size: 20.1 MB (20131347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:1.7.34-alpine`

```console
$ docker pull traefik@sha256:8ac75422d559a55193d20df11116ea951ad962f7dcdf3bd76a51f81f460de821
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:1.7.34-alpine` - linux; amd64

```console
$ docker pull traefik@sha256:04c41c7c3ff03d006e93029fb6bce95a448a32900c47487cf2f54f4df2d42f56
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.6 MB (25645268 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9eb8c5f993e88b67da6b9d2b5ee0a09e7f6a576c70e19f8bd1031adae54418ca`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 17 Mar 2022 15:19:26 GMT
ADD file:8ec3735d4b1b4b070607b94e3bd360117b07dc26e1baf5dd485b49b3413e8fff in / 
# Thu, 17 Mar 2022 15:19:26 GMT
CMD ["/bin/sh"]
# Fri, 18 Mar 2022 06:23:06 GMT
RUN apk --no-cache add ca-certificates tzdata
# Fri, 18 Mar 2022 06:23:24 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/traefik/traefik/releases/download/v1.7.34/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Fri, 18 Mar 2022 06:23:24 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Fri, 18 Mar 2022 06:23:24 GMT
EXPOSE 80
# Fri, 18 Mar 2022 06:23:24 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 18 Mar 2022 06:23:24 GMT
CMD ["traefik"]
# Fri, 18 Mar 2022 06:23:25 GMT
LABEL org.opencontainers.image.vendor=traefik org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.34 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:36ccefbf3d8a9a1b18baaa9cbf0f3ad50e8a7b751656c74df359900a318cbffc`  
		Last Modified: Thu, 17 Mar 2022 15:20:13 GMT  
		Size: 2.8 MB (2816169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d66f86d3f60579f394506161f82aafee52b414cd58c1060e18ca607a4fc9fbc4`  
		Last Modified: Fri, 18 Mar 2022 06:24:10 GMT  
		Size: 666.7 KB (666670 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b9a06ba42895ffa47fb412ee9c0fe6cc5c33d4bf08ca4a76e74f7040bc82206`  
		Last Modified: Fri, 18 Mar 2022 06:24:42 GMT  
		Size: 22.2 MB (22162062 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b266beb8763fa8eeb482f01673624fb468758ac98bb28cc16881d8f94e1f54c`  
		Last Modified: Fri, 18 Mar 2022 06:24:36 GMT  
		Size: 367.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:1.7.34-alpine` - linux; arm variant v6

```console
$ docker pull traefik@sha256:08be027ed453b435111cb912908324ee1f5f0d77db60b6d6f9f10003d2c62674
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.9 MB (23925625 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d5fbe3dd0a206256fa43655ee4af71da94003b6377978bc54ccdb219452f1bcc`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 17 Mar 2022 14:32:33 GMT
ADD file:8f1611b9334907a82945fdb21e17ee41541ab95050fc199c60fca662759171a5 in / 
# Thu, 17 Mar 2022 14:32:33 GMT
CMD ["/bin/sh"]
# Thu, 17 Mar 2022 22:44:31 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 17 Mar 2022 22:45:03 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/traefik/traefik/releases/download/v1.7.34/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Thu, 17 Mar 2022 22:45:03 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 17 Mar 2022 22:45:04 GMT
EXPOSE 80
# Thu, 17 Mar 2022 22:45:05 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 17 Mar 2022 22:45:05 GMT
CMD ["traefik"]
# Thu, 17 Mar 2022 22:45:06 GMT
LABEL org.opencontainers.image.vendor=traefik org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.34 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:4025825e6ef43541c3a3e1ecb0092bc1b098e792051c7e338d6da54f66b19661`  
		Last Modified: Thu, 17 Mar 2022 14:34:09 GMT  
		Size: 2.6 MB (2629364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acc61b01c9ae829babc4ec995a57d752de240cbe8e3a8660191d3d21fc589a5f`  
		Last Modified: Thu, 17 Mar 2022 22:46:57 GMT  
		Size: 672.5 KB (672470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:244182210987061535c909a9a2aace43df0eb4ee95953b8813c3792dd4ba5b37`  
		Last Modified: Thu, 17 Mar 2022 22:47:55 GMT  
		Size: 20.6 MB (20623423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb981a93f73996a8309c5494870b9e83074dae0470e145590d2148af320281cf`  
		Last Modified: Thu, 17 Mar 2022 22:47:40 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:1.7.34-alpine` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:1e7c544b79ed103ad6d22cd9941ca3416e02897a9cb7f75120f6fd5f1949d90c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.5 MB (23515893 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:11a718e3a556a699675cb6d5655875c7240cd58d718536719147125b9d171870`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 17 Mar 2022 18:43:12 GMT
ADD file:611998b78638b13e78919dd4635674032ab233f9b7aae6f62beaf6634cd18b9e in / 
# Thu, 17 Mar 2022 18:43:13 GMT
CMD ["/bin/sh"]
# Thu, 17 Mar 2022 21:06:35 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 17 Mar 2022 21:06:53 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/traefik/traefik/releases/download/v1.7.34/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Thu, 17 Mar 2022 21:06:55 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 17 Mar 2022 21:06:55 GMT
EXPOSE 80
# Thu, 17 Mar 2022 21:06:56 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 17 Mar 2022 21:06:57 GMT
CMD ["traefik"]
# Thu, 17 Mar 2022 21:06:58 GMT
LABEL org.opencontainers.image.vendor=traefik org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.34 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:93a1719cf26168d3a85db2594d76b17ccc4b25996620bceed3c2a13eaa165325`  
		Last Modified: Thu, 17 Mar 2022 18:44:00 GMT  
		Size: 2.7 MB (2715888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d012a4d53d2ad42f0d1b24f774778f1ea2d1c67cfdd0a1611fb7652fac92fc9b`  
		Last Modified: Thu, 17 Mar 2022 21:07:51 GMT  
		Size: 668.3 KB (668255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe57c71a6e6bc8b2eda9db22fd05c14079977728ba28062721c5d71106b23ab9`  
		Last Modified: Thu, 17 Mar 2022 21:08:21 GMT  
		Size: 20.1 MB (20131382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:535366a8854793a298d798c23544e4ad0849c13ce51c5687ad00f9864bebe75a`  
		Last Modified: Thu, 17 Mar 2022 21:08:18 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:1.7.34-windowsservercore-1809`

```console
$ docker pull traefik@sha256:85ffe3d43fd4929a0e48d226e018af240fbbd8ea9a03685f74f1c78c432f85b3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2686; amd64

### `traefik:1.7.34-windowsservercore-1809` - windows version 10.0.17763.2686; amd64

```console
$ docker pull traefik@sha256:67d210fa3d7dcb1ebc3b3b5f3bfdaac7d18195e1bb2b83fa2c1b1f48d09b08dd
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2738303983 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d6ebd04310fbdd68b4e7225310f8a6f2dec3a0330af0d02b74a9a0e35b79945b`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 03 Mar 2022 15:05:04 GMT
RUN Install update 1809-amd64
# Tue, 08 Mar 2022 19:31:54 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Mar 2022 18:53:09 GMT
RUN Invoke-WebRequest     -Uri "https://github.com/traefik/traefik/releases/download/v1.7.34/traefik_windows-amd64.exe"     -OutFile "/traefik.exe"
# Wed, 09 Mar 2022 18:53:10 GMT
EXPOSE 80
# Wed, 09 Mar 2022 18:53:11 GMT
ENTRYPOINT ["/traefik"]
# Wed, 09 Mar 2022 18:53:12 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.34 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:0a6173b79e25f2ebc0ed51b0ac32a6f65ca5a3bbfcbeab8b74a6c24324121dea`  
		Size: 997.1 MB (997119751 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a42bef5ec276ee3f8dd3545bf050f4ab85c8191392884f5d5ad6af6ae6e2eed2`  
		Last Modified: Tue, 08 Mar 2022 20:01:19 GMT  
		Size: 1.3 KB (1323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fd63edc5d2bde654b771ee58c8e9bb78539127758e862053223f402d3eaea68`  
		Last Modified: Wed, 09 Mar 2022 18:54:50 GMT  
		Size: 22.8 MB (22845783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cefe3e1f9703a33ffdf92a9c03b8a4738222fe08ea99aded6416f848aa300e9`  
		Last Modified: Wed, 09 Mar 2022 18:54:27 GMT  
		Size: 1.4 KB (1446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:939f3b18eb0ddb1cb4c6b01a2abc4127403c6a67c630a8c05c6be5f43ab74acc`  
		Last Modified: Wed, 09 Mar 2022 18:54:26 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35bcba10ab84d161e2dc32a48f6bc15da23d8aabdb22bbf4a89499ce18583d46`  
		Last Modified: Wed, 09 Mar 2022 18:54:26 GMT  
		Size: 1.4 KB (1389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:2.6`

```console
$ docker pull traefik@sha256:a94f8efcbdccb28e591fc04a3dce0cf5947e1b564c6d471a5945b09f130dfd86
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:2.6` - linux; amd64

```console
$ docker pull traefik@sha256:f3a0e9a0bdf260cf8c25c6ad7ee05cb05c3966d1058303b971b7057fc68a6457
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.3 MB (30325710 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cf9fa2c5f0d2e4c1cbf00e8ea973d74c8d11b1567205f5edc7284fdb0de166b3`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 17 Mar 2022 15:19:26 GMT
ADD file:8ec3735d4b1b4b070607b94e3bd360117b07dc26e1baf5dd485b49b3413e8fff in / 
# Thu, 17 Mar 2022 15:19:26 GMT
CMD ["/bin/sh"]
# Fri, 18 Mar 2022 06:23:06 GMT
RUN apk --no-cache add ca-certificates tzdata
# Fri, 18 Mar 2022 06:23:11 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.6.1/traefik_v2.6.1_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Fri, 18 Mar 2022 06:23:12 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Fri, 18 Mar 2022 06:23:12 GMT
EXPOSE 80
# Fri, 18 Mar 2022 06:23:12 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 18 Mar 2022 06:23:12 GMT
CMD ["traefik"]
# Fri, 18 Mar 2022 06:23:12 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.6.1 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:36ccefbf3d8a9a1b18baaa9cbf0f3ad50e8a7b751656c74df359900a318cbffc`  
		Last Modified: Thu, 17 Mar 2022 15:20:13 GMT  
		Size: 2.8 MB (2816169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d66f86d3f60579f394506161f82aafee52b414cd58c1060e18ca607a4fc9fbc4`  
		Last Modified: Fri, 18 Mar 2022 06:24:10 GMT  
		Size: 666.7 KB (666670 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01c1ca55dba5b4d567cb01859f50449eb49d7531bcde631825000d0135927d3d`  
		Last Modified: Fri, 18 Mar 2022 06:24:16 GMT  
		Size: 26.8 MB (26842504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:139a4e0ca97e6f942624418ee448c126f2084e4a79b2946064a434a48c3e8fbc`  
		Last Modified: Fri, 18 Mar 2022 06:24:10 GMT  
		Size: 367.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:2.6` - linux; arm variant v6

```console
$ docker pull traefik@sha256:2ff4bf1842307e9179d2c71959da827be092f581742b9751096bb1f55df78267
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.5 MB (28492404 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4eb2cddfb6417b47e508ee363f0b5a36a19bf5981662b7280742bc56aae3684e`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 17 Mar 2022 14:32:33 GMT
ADD file:8f1611b9334907a82945fdb21e17ee41541ab95050fc199c60fca662759171a5 in / 
# Thu, 17 Mar 2022 14:32:33 GMT
CMD ["/bin/sh"]
# Thu, 17 Mar 2022 22:44:31 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 17 Mar 2022 22:44:38 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.6.1/traefik_v2.6.1_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 17 Mar 2022 22:44:39 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 17 Mar 2022 22:44:39 GMT
EXPOSE 80
# Thu, 17 Mar 2022 22:44:40 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 17 Mar 2022 22:44:40 GMT
CMD ["traefik"]
# Thu, 17 Mar 2022 22:44:41 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.6.1 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:4025825e6ef43541c3a3e1ecb0092bc1b098e792051c7e338d6da54f66b19661`  
		Last Modified: Thu, 17 Mar 2022 14:34:09 GMT  
		Size: 2.6 MB (2629364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acc61b01c9ae829babc4ec995a57d752de240cbe8e3a8660191d3d21fc589a5f`  
		Last Modified: Thu, 17 Mar 2022 22:46:57 GMT  
		Size: 672.5 KB (672470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9054064868f20b2649a2e2a9141b8f8e9f915a8c0b21859cd801f175d7e2851b`  
		Last Modified: Thu, 17 Mar 2022 22:47:14 GMT  
		Size: 25.2 MB (25190202 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1be114305d9910bdd128e32db0ec6aef6c4ef92e6857b290d41387df34aeef2b`  
		Last Modified: Thu, 17 Mar 2022 22:46:57 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:2.6` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:57bea358260f808ed121400b19702fd8f6ac362f394ecdac9b55ab43c95d2940
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.9 MB (27867844 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:89657e32bf0a480cfe729a2bfb2ff094c143fab533f470e63d8c9b9faf123308`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 17 Mar 2022 18:43:12 GMT
ADD file:611998b78638b13e78919dd4635674032ab233f9b7aae6f62beaf6634cd18b9e in / 
# Thu, 17 Mar 2022 18:43:13 GMT
CMD ["/bin/sh"]
# Thu, 17 Mar 2022 21:06:35 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 17 Mar 2022 21:06:38 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.6.1/traefik_v2.6.1_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 17 Mar 2022 21:06:39 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 17 Mar 2022 21:06:39 GMT
EXPOSE 80
# Thu, 17 Mar 2022 21:06:40 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 17 Mar 2022 21:06:41 GMT
CMD ["traefik"]
# Thu, 17 Mar 2022 21:06:42 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.6.1 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:93a1719cf26168d3a85db2594d76b17ccc4b25996620bceed3c2a13eaa165325`  
		Last Modified: Thu, 17 Mar 2022 18:44:00 GMT  
		Size: 2.7 MB (2715888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d012a4d53d2ad42f0d1b24f774778f1ea2d1c67cfdd0a1611fb7652fac92fc9b`  
		Last Modified: Thu, 17 Mar 2022 21:07:51 GMT  
		Size: 668.3 KB (668255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8efd5dcd64fe25305ce09060a42d89619e8dbfb06e5be5633e1abc05d30445c5`  
		Last Modified: Thu, 17 Mar 2022 21:07:55 GMT  
		Size: 24.5 MB (24483333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1eb6f2eaa89fe53dae137bd6cd91f8ef241feeae582ecdf82d83834d8bd3733b`  
		Last Modified: Thu, 17 Mar 2022 21:07:50 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:2.6-windowsservercore-1809`

```console
$ docker pull traefik@sha256:b80deb28063ace6076665281bd27560fd3430b7b39f5bd15503c640defb8cf49
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2686; amd64

### `traefik:2.6-windowsservercore-1809` - windows version 10.0.17763.2686; amd64

```console
$ docker pull traefik@sha256:f57bdfbb46114920642abf2d1345012ecdb600175d227e38a2e681a1ebabfbd6
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2742866391 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2bf552045eeb764b54471001b799a24b4fa37c54b3aa7dbfa24c133f83d4ffb9`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 03 Mar 2022 15:05:04 GMT
RUN Install update 1809-amd64
# Tue, 08 Mar 2022 19:31:54 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Mar 2022 18:51:55 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/traefik/traefik/releases/download/v2.6.1/traefik_v2.6.1_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Wed, 09 Mar 2022 18:51:56 GMT
EXPOSE 80
# Wed, 09 Mar 2022 18:51:57 GMT
ENTRYPOINT ["/traefik"]
# Wed, 09 Mar 2022 18:51:58 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.6.1 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:0a6173b79e25f2ebc0ed51b0ac32a6f65ca5a3bbfcbeab8b74a6c24324121dea`  
		Size: 997.1 MB (997119751 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a42bef5ec276ee3f8dd3545bf050f4ab85c8191392884f5d5ad6af6ae6e2eed2`  
		Last Modified: Tue, 08 Mar 2022 20:01:19 GMT  
		Size: 1.3 KB (1323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61d553f74a3b073844e4c127831b8beebc1b835dc85e7c94513c77cc5c92e162`  
		Last Modified: Wed, 09 Mar 2022 18:54:08 GMT  
		Size: 27.4 MB (27408215 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2ef09b6978e9dfcd8c026989ac01b7a2a1acc1d57e058284c45efdfb0f0dd8a`  
		Last Modified: Wed, 09 Mar 2022 18:53:40 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc092ecf87d8664357e1628d8189f5c4c42972eb1dbcb6081f06524b75e0d8b5`  
		Last Modified: Wed, 09 Mar 2022 18:53:40 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8eebfe3ad70b0f95c3a0f566473bf5c42bbaf14434a4298c864e34bbcdf5e33`  
		Last Modified: Wed, 09 Mar 2022 18:53:40 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:2.6.1`

```console
$ docker pull traefik@sha256:a94f8efcbdccb28e591fc04a3dce0cf5947e1b564c6d471a5945b09f130dfd86
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:2.6.1` - linux; amd64

```console
$ docker pull traefik@sha256:f3a0e9a0bdf260cf8c25c6ad7ee05cb05c3966d1058303b971b7057fc68a6457
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.3 MB (30325710 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cf9fa2c5f0d2e4c1cbf00e8ea973d74c8d11b1567205f5edc7284fdb0de166b3`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 17 Mar 2022 15:19:26 GMT
ADD file:8ec3735d4b1b4b070607b94e3bd360117b07dc26e1baf5dd485b49b3413e8fff in / 
# Thu, 17 Mar 2022 15:19:26 GMT
CMD ["/bin/sh"]
# Fri, 18 Mar 2022 06:23:06 GMT
RUN apk --no-cache add ca-certificates tzdata
# Fri, 18 Mar 2022 06:23:11 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.6.1/traefik_v2.6.1_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Fri, 18 Mar 2022 06:23:12 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Fri, 18 Mar 2022 06:23:12 GMT
EXPOSE 80
# Fri, 18 Mar 2022 06:23:12 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 18 Mar 2022 06:23:12 GMT
CMD ["traefik"]
# Fri, 18 Mar 2022 06:23:12 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.6.1 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:36ccefbf3d8a9a1b18baaa9cbf0f3ad50e8a7b751656c74df359900a318cbffc`  
		Last Modified: Thu, 17 Mar 2022 15:20:13 GMT  
		Size: 2.8 MB (2816169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d66f86d3f60579f394506161f82aafee52b414cd58c1060e18ca607a4fc9fbc4`  
		Last Modified: Fri, 18 Mar 2022 06:24:10 GMT  
		Size: 666.7 KB (666670 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01c1ca55dba5b4d567cb01859f50449eb49d7531bcde631825000d0135927d3d`  
		Last Modified: Fri, 18 Mar 2022 06:24:16 GMT  
		Size: 26.8 MB (26842504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:139a4e0ca97e6f942624418ee448c126f2084e4a79b2946064a434a48c3e8fbc`  
		Last Modified: Fri, 18 Mar 2022 06:24:10 GMT  
		Size: 367.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:2.6.1` - linux; arm variant v6

```console
$ docker pull traefik@sha256:2ff4bf1842307e9179d2c71959da827be092f581742b9751096bb1f55df78267
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.5 MB (28492404 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4eb2cddfb6417b47e508ee363f0b5a36a19bf5981662b7280742bc56aae3684e`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 17 Mar 2022 14:32:33 GMT
ADD file:8f1611b9334907a82945fdb21e17ee41541ab95050fc199c60fca662759171a5 in / 
# Thu, 17 Mar 2022 14:32:33 GMT
CMD ["/bin/sh"]
# Thu, 17 Mar 2022 22:44:31 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 17 Mar 2022 22:44:38 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.6.1/traefik_v2.6.1_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 17 Mar 2022 22:44:39 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 17 Mar 2022 22:44:39 GMT
EXPOSE 80
# Thu, 17 Mar 2022 22:44:40 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 17 Mar 2022 22:44:40 GMT
CMD ["traefik"]
# Thu, 17 Mar 2022 22:44:41 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.6.1 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:4025825e6ef43541c3a3e1ecb0092bc1b098e792051c7e338d6da54f66b19661`  
		Last Modified: Thu, 17 Mar 2022 14:34:09 GMT  
		Size: 2.6 MB (2629364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acc61b01c9ae829babc4ec995a57d752de240cbe8e3a8660191d3d21fc589a5f`  
		Last Modified: Thu, 17 Mar 2022 22:46:57 GMT  
		Size: 672.5 KB (672470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9054064868f20b2649a2e2a9141b8f8e9f915a8c0b21859cd801f175d7e2851b`  
		Last Modified: Thu, 17 Mar 2022 22:47:14 GMT  
		Size: 25.2 MB (25190202 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1be114305d9910bdd128e32db0ec6aef6c4ef92e6857b290d41387df34aeef2b`  
		Last Modified: Thu, 17 Mar 2022 22:46:57 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:2.6.1` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:57bea358260f808ed121400b19702fd8f6ac362f394ecdac9b55ab43c95d2940
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.9 MB (27867844 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:89657e32bf0a480cfe729a2bfb2ff094c143fab533f470e63d8c9b9faf123308`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 17 Mar 2022 18:43:12 GMT
ADD file:611998b78638b13e78919dd4635674032ab233f9b7aae6f62beaf6634cd18b9e in / 
# Thu, 17 Mar 2022 18:43:13 GMT
CMD ["/bin/sh"]
# Thu, 17 Mar 2022 21:06:35 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 17 Mar 2022 21:06:38 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.6.1/traefik_v2.6.1_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 17 Mar 2022 21:06:39 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 17 Mar 2022 21:06:39 GMT
EXPOSE 80
# Thu, 17 Mar 2022 21:06:40 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 17 Mar 2022 21:06:41 GMT
CMD ["traefik"]
# Thu, 17 Mar 2022 21:06:42 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.6.1 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:93a1719cf26168d3a85db2594d76b17ccc4b25996620bceed3c2a13eaa165325`  
		Last Modified: Thu, 17 Mar 2022 18:44:00 GMT  
		Size: 2.7 MB (2715888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d012a4d53d2ad42f0d1b24f774778f1ea2d1c67cfdd0a1611fb7652fac92fc9b`  
		Last Modified: Thu, 17 Mar 2022 21:07:51 GMT  
		Size: 668.3 KB (668255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8efd5dcd64fe25305ce09060a42d89619e8dbfb06e5be5633e1abc05d30445c5`  
		Last Modified: Thu, 17 Mar 2022 21:07:55 GMT  
		Size: 24.5 MB (24483333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1eb6f2eaa89fe53dae137bd6cd91f8ef241feeae582ecdf82d83834d8bd3733b`  
		Last Modified: Thu, 17 Mar 2022 21:07:50 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:2.6.1-windowsservercore-1809`

```console
$ docker pull traefik@sha256:b80deb28063ace6076665281bd27560fd3430b7b39f5bd15503c640defb8cf49
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2686; amd64

### `traefik:2.6.1-windowsservercore-1809` - windows version 10.0.17763.2686; amd64

```console
$ docker pull traefik@sha256:f57bdfbb46114920642abf2d1345012ecdb600175d227e38a2e681a1ebabfbd6
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2742866391 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2bf552045eeb764b54471001b799a24b4fa37c54b3aa7dbfa24c133f83d4ffb9`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 03 Mar 2022 15:05:04 GMT
RUN Install update 1809-amd64
# Tue, 08 Mar 2022 19:31:54 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Mar 2022 18:51:55 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/traefik/traefik/releases/download/v2.6.1/traefik_v2.6.1_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Wed, 09 Mar 2022 18:51:56 GMT
EXPOSE 80
# Wed, 09 Mar 2022 18:51:57 GMT
ENTRYPOINT ["/traefik"]
# Wed, 09 Mar 2022 18:51:58 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.6.1 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:0a6173b79e25f2ebc0ed51b0ac32a6f65ca5a3bbfcbeab8b74a6c24324121dea`  
		Size: 997.1 MB (997119751 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a42bef5ec276ee3f8dd3545bf050f4ab85c8191392884f5d5ad6af6ae6e2eed2`  
		Last Modified: Tue, 08 Mar 2022 20:01:19 GMT  
		Size: 1.3 KB (1323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61d553f74a3b073844e4c127831b8beebc1b835dc85e7c94513c77cc5c92e162`  
		Last Modified: Wed, 09 Mar 2022 18:54:08 GMT  
		Size: 27.4 MB (27408215 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2ef09b6978e9dfcd8c026989ac01b7a2a1acc1d57e058284c45efdfb0f0dd8a`  
		Last Modified: Wed, 09 Mar 2022 18:53:40 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc092ecf87d8664357e1628d8189f5c4c42972eb1dbcb6081f06524b75e0d8b5`  
		Last Modified: Wed, 09 Mar 2022 18:53:40 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8eebfe3ad70b0f95c3a0f566473bf5c42bbaf14434a4298c864e34bbcdf5e33`  
		Last Modified: Wed, 09 Mar 2022 18:53:40 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:latest`

```console
$ docker pull traefik@sha256:a94f8efcbdccb28e591fc04a3dce0cf5947e1b564c6d471a5945b09f130dfd86
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:latest` - linux; amd64

```console
$ docker pull traefik@sha256:f3a0e9a0bdf260cf8c25c6ad7ee05cb05c3966d1058303b971b7057fc68a6457
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.3 MB (30325710 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cf9fa2c5f0d2e4c1cbf00e8ea973d74c8d11b1567205f5edc7284fdb0de166b3`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 17 Mar 2022 15:19:26 GMT
ADD file:8ec3735d4b1b4b070607b94e3bd360117b07dc26e1baf5dd485b49b3413e8fff in / 
# Thu, 17 Mar 2022 15:19:26 GMT
CMD ["/bin/sh"]
# Fri, 18 Mar 2022 06:23:06 GMT
RUN apk --no-cache add ca-certificates tzdata
# Fri, 18 Mar 2022 06:23:11 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.6.1/traefik_v2.6.1_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Fri, 18 Mar 2022 06:23:12 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Fri, 18 Mar 2022 06:23:12 GMT
EXPOSE 80
# Fri, 18 Mar 2022 06:23:12 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 18 Mar 2022 06:23:12 GMT
CMD ["traefik"]
# Fri, 18 Mar 2022 06:23:12 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.6.1 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:36ccefbf3d8a9a1b18baaa9cbf0f3ad50e8a7b751656c74df359900a318cbffc`  
		Last Modified: Thu, 17 Mar 2022 15:20:13 GMT  
		Size: 2.8 MB (2816169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d66f86d3f60579f394506161f82aafee52b414cd58c1060e18ca607a4fc9fbc4`  
		Last Modified: Fri, 18 Mar 2022 06:24:10 GMT  
		Size: 666.7 KB (666670 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01c1ca55dba5b4d567cb01859f50449eb49d7531bcde631825000d0135927d3d`  
		Last Modified: Fri, 18 Mar 2022 06:24:16 GMT  
		Size: 26.8 MB (26842504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:139a4e0ca97e6f942624418ee448c126f2084e4a79b2946064a434a48c3e8fbc`  
		Last Modified: Fri, 18 Mar 2022 06:24:10 GMT  
		Size: 367.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:latest` - linux; arm variant v6

```console
$ docker pull traefik@sha256:2ff4bf1842307e9179d2c71959da827be092f581742b9751096bb1f55df78267
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.5 MB (28492404 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4eb2cddfb6417b47e508ee363f0b5a36a19bf5981662b7280742bc56aae3684e`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 17 Mar 2022 14:32:33 GMT
ADD file:8f1611b9334907a82945fdb21e17ee41541ab95050fc199c60fca662759171a5 in / 
# Thu, 17 Mar 2022 14:32:33 GMT
CMD ["/bin/sh"]
# Thu, 17 Mar 2022 22:44:31 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 17 Mar 2022 22:44:38 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.6.1/traefik_v2.6.1_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 17 Mar 2022 22:44:39 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 17 Mar 2022 22:44:39 GMT
EXPOSE 80
# Thu, 17 Mar 2022 22:44:40 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 17 Mar 2022 22:44:40 GMT
CMD ["traefik"]
# Thu, 17 Mar 2022 22:44:41 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.6.1 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:4025825e6ef43541c3a3e1ecb0092bc1b098e792051c7e338d6da54f66b19661`  
		Last Modified: Thu, 17 Mar 2022 14:34:09 GMT  
		Size: 2.6 MB (2629364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acc61b01c9ae829babc4ec995a57d752de240cbe8e3a8660191d3d21fc589a5f`  
		Last Modified: Thu, 17 Mar 2022 22:46:57 GMT  
		Size: 672.5 KB (672470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9054064868f20b2649a2e2a9141b8f8e9f915a8c0b21859cd801f175d7e2851b`  
		Last Modified: Thu, 17 Mar 2022 22:47:14 GMT  
		Size: 25.2 MB (25190202 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1be114305d9910bdd128e32db0ec6aef6c4ef92e6857b290d41387df34aeef2b`  
		Last Modified: Thu, 17 Mar 2022 22:46:57 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:latest` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:57bea358260f808ed121400b19702fd8f6ac362f394ecdac9b55ab43c95d2940
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.9 MB (27867844 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:89657e32bf0a480cfe729a2bfb2ff094c143fab533f470e63d8c9b9faf123308`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 17 Mar 2022 18:43:12 GMT
ADD file:611998b78638b13e78919dd4635674032ab233f9b7aae6f62beaf6634cd18b9e in / 
# Thu, 17 Mar 2022 18:43:13 GMT
CMD ["/bin/sh"]
# Thu, 17 Mar 2022 21:06:35 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 17 Mar 2022 21:06:38 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.6.1/traefik_v2.6.1_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 17 Mar 2022 21:06:39 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 17 Mar 2022 21:06:39 GMT
EXPOSE 80
# Thu, 17 Mar 2022 21:06:40 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 17 Mar 2022 21:06:41 GMT
CMD ["traefik"]
# Thu, 17 Mar 2022 21:06:42 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.6.1 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:93a1719cf26168d3a85db2594d76b17ccc4b25996620bceed3c2a13eaa165325`  
		Last Modified: Thu, 17 Mar 2022 18:44:00 GMT  
		Size: 2.7 MB (2715888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d012a4d53d2ad42f0d1b24f774778f1ea2d1c67cfdd0a1611fb7652fac92fc9b`  
		Last Modified: Thu, 17 Mar 2022 21:07:51 GMT  
		Size: 668.3 KB (668255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8efd5dcd64fe25305ce09060a42d89619e8dbfb06e5be5633e1abc05d30445c5`  
		Last Modified: Thu, 17 Mar 2022 21:07:55 GMT  
		Size: 24.5 MB (24483333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1eb6f2eaa89fe53dae137bd6cd91f8ef241feeae582ecdf82d83834d8bd3733b`  
		Last Modified: Thu, 17 Mar 2022 21:07:50 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:maroilles`

```console
$ docker pull traefik@sha256:1d8a41ae1bd54c9e9a5e0cc8da9002638932c53cc3d50c6f0c172238374ebe8f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:maroilles` - linux; amd64

```console
$ docker pull traefik@sha256:f705216279431ed8ab470318736acd767794a847acda2db325e3e159574bd03c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **22.6 MB (22607863 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:43de28b34d397393ca2d0ec8bd6923735fab787f8c3bd3dab0719cd256fcc010`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Fri, 18 Mar 2022 06:23:36 GMT
COPY file:8536203e9de8580f4424aff73a3be4185daba1818e4bfa286f2b290d1459aeb9 in /etc/ssl/certs/ 
# Fri, 18 Mar 2022 06:23:37 GMT
COPY dir:a84372748b89eb90478bb1b120b7c8fff3112421d7f93e50fbeae3f53adc6788 in /usr/share/ 
# Fri, 18 Mar 2022 06:23:38 GMT
COPY file:36217e5a6056bef26cfff395c8af8c1010a61dbe8d62b2c7869ca221e2a6302c in / 
# Fri, 18 Mar 2022 06:23:39 GMT
EXPOSE 80
# Fri, 18 Mar 2022 06:23:39 GMT
VOLUME [/tmp]
# Fri, 18 Mar 2022 06:23:39 GMT
ENTRYPOINT ["/traefik"]
# Fri, 18 Mar 2022 06:23:39 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.34 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:903e84870d1b7b581b2c6c362c74751a258cb8e2dbb443bddcd36fe8f29a20ab`  
		Last Modified: Fri, 18 Mar 2022 06:24:59 GMT  
		Size: 117.4 KB (117389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:914ae7a2b8652023026596365a1dfe88e317d16b1cc8099ee03c20357c95716e`  
		Last Modified: Fri, 18 Mar 2022 06:25:00 GMT  
		Size: 328.5 KB (328522 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f483c7bcad16f6ac0813c7a4704d4dc9319bfd6533f10c888b5e2ca21c72dc44`  
		Last Modified: Fri, 18 Mar 2022 06:25:05 GMT  
		Size: 22.2 MB (22161952 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:maroilles` - linux; arm variant v6

```console
$ docker pull traefik@sha256:fe6bde6e9349ec036bc3aaec90c095006425bface50ee2f449e0d196cb5850c7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **21.1 MB (21069186 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5a5c3451377ef5e2379e4bc19691fb6c14b1a2215326833336e1db9e16cc5ca3`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Thu, 17 Mar 2022 22:45:25 GMT
COPY file:8536203e9de8580f4424aff73a3be4185daba1818e4bfa286f2b290d1459aeb9 in /etc/ssl/certs/ 
# Thu, 17 Mar 2022 22:45:27 GMT
COPY dir:a84372748b89eb90478bb1b120b7c8fff3112421d7f93e50fbeae3f53adc6788 in /usr/share/ 
# Thu, 17 Mar 2022 22:45:32 GMT
COPY file:5d1e7e81e8b77b4f8828eeaf0d30a0f135a949b51396f12ae22af376c36d3129 in / 
# Thu, 17 Mar 2022 22:45:33 GMT
EXPOSE 80
# Thu, 17 Mar 2022 22:45:33 GMT
VOLUME [/tmp]
# Thu, 17 Mar 2022 22:45:34 GMT
ENTRYPOINT ["/traefik"]
# Thu, 17 Mar 2022 22:45:34 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.34 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:27b61c1d4effca5c7137bfe0c8b6a3a228418ef37998781ad6cc7372c6f7e98f`  
		Last Modified: Thu, 17 Mar 2022 22:48:17 GMT  
		Size: 117.4 KB (117390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98aae3b48a316f885b1d485fee6b2ffffb3c2c7dea49cea01019d4c103b204da`  
		Last Modified: Thu, 17 Mar 2022 22:48:18 GMT  
		Size: 328.5 KB (328514 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a82873a2be1cc2b2dfbc565c4bf9960f32b61892f49f0911ec1ac7e310210c3d`  
		Last Modified: Thu, 17 Mar 2022 22:48:34 GMT  
		Size: 20.6 MB (20623282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:maroilles` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:c2930d3e36f7feb98470b85e8bc9fce0016fc5eadbc805249e63d6a458eb2323
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **20.6 MB (20577242 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f7338e148255e82dd93286a1f87db35f499d4e391d7f5f3e1bfb6c71ed4ec2d4`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Thu, 17 Mar 2022 21:07:07 GMT
COPY file:8536203e9de8580f4424aff73a3be4185daba1818e4bfa286f2b290d1459aeb9 in /etc/ssl/certs/ 
# Thu, 17 Mar 2022 21:07:08 GMT
COPY dir:a84372748b89eb90478bb1b120b7c8fff3112421d7f93e50fbeae3f53adc6788 in /usr/share/ 
# Thu, 17 Mar 2022 21:07:09 GMT
COPY file:60330593b6644f3f519fd13ce8ee34c2c7ab9994a1420afabbc01926dd1230dd in / 
# Thu, 17 Mar 2022 21:07:09 GMT
EXPOSE 80
# Thu, 17 Mar 2022 21:07:10 GMT
VOLUME [/tmp]
# Thu, 17 Mar 2022 21:07:11 GMT
ENTRYPOINT ["/traefik"]
# Thu, 17 Mar 2022 21:07:12 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.34 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:86cd07830d2730c0aa24f0e47380af5ef760945b5049a2e72a8ebe0675ed6d34`  
		Last Modified: Thu, 17 Mar 2022 21:08:41 GMT  
		Size: 117.4 KB (117390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:135b9e65a5ea0b642df02ea2cf73c74a353d1cbfa3b95d048a4adbf0bacf9653`  
		Last Modified: Thu, 17 Mar 2022 21:08:41 GMT  
		Size: 328.5 KB (328505 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bee8fa09b05c38fc9116b1446ac3d204200577fd9bfb1801d684657dc722b74b`  
		Last Modified: Thu, 17 Mar 2022 21:08:45 GMT  
		Size: 20.1 MB (20131347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:maroilles-alpine`

```console
$ docker pull traefik@sha256:8ac75422d559a55193d20df11116ea951ad962f7dcdf3bd76a51f81f460de821
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:maroilles-alpine` - linux; amd64

```console
$ docker pull traefik@sha256:04c41c7c3ff03d006e93029fb6bce95a448a32900c47487cf2f54f4df2d42f56
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.6 MB (25645268 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9eb8c5f993e88b67da6b9d2b5ee0a09e7f6a576c70e19f8bd1031adae54418ca`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 17 Mar 2022 15:19:26 GMT
ADD file:8ec3735d4b1b4b070607b94e3bd360117b07dc26e1baf5dd485b49b3413e8fff in / 
# Thu, 17 Mar 2022 15:19:26 GMT
CMD ["/bin/sh"]
# Fri, 18 Mar 2022 06:23:06 GMT
RUN apk --no-cache add ca-certificates tzdata
# Fri, 18 Mar 2022 06:23:24 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/traefik/traefik/releases/download/v1.7.34/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Fri, 18 Mar 2022 06:23:24 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Fri, 18 Mar 2022 06:23:24 GMT
EXPOSE 80
# Fri, 18 Mar 2022 06:23:24 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 18 Mar 2022 06:23:24 GMT
CMD ["traefik"]
# Fri, 18 Mar 2022 06:23:25 GMT
LABEL org.opencontainers.image.vendor=traefik org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.34 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:36ccefbf3d8a9a1b18baaa9cbf0f3ad50e8a7b751656c74df359900a318cbffc`  
		Last Modified: Thu, 17 Mar 2022 15:20:13 GMT  
		Size: 2.8 MB (2816169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d66f86d3f60579f394506161f82aafee52b414cd58c1060e18ca607a4fc9fbc4`  
		Last Modified: Fri, 18 Mar 2022 06:24:10 GMT  
		Size: 666.7 KB (666670 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b9a06ba42895ffa47fb412ee9c0fe6cc5c33d4bf08ca4a76e74f7040bc82206`  
		Last Modified: Fri, 18 Mar 2022 06:24:42 GMT  
		Size: 22.2 MB (22162062 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b266beb8763fa8eeb482f01673624fb468758ac98bb28cc16881d8f94e1f54c`  
		Last Modified: Fri, 18 Mar 2022 06:24:36 GMT  
		Size: 367.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:maroilles-alpine` - linux; arm variant v6

```console
$ docker pull traefik@sha256:08be027ed453b435111cb912908324ee1f5f0d77db60b6d6f9f10003d2c62674
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.9 MB (23925625 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d5fbe3dd0a206256fa43655ee4af71da94003b6377978bc54ccdb219452f1bcc`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 17 Mar 2022 14:32:33 GMT
ADD file:8f1611b9334907a82945fdb21e17ee41541ab95050fc199c60fca662759171a5 in / 
# Thu, 17 Mar 2022 14:32:33 GMT
CMD ["/bin/sh"]
# Thu, 17 Mar 2022 22:44:31 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 17 Mar 2022 22:45:03 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/traefik/traefik/releases/download/v1.7.34/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Thu, 17 Mar 2022 22:45:03 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 17 Mar 2022 22:45:04 GMT
EXPOSE 80
# Thu, 17 Mar 2022 22:45:05 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 17 Mar 2022 22:45:05 GMT
CMD ["traefik"]
# Thu, 17 Mar 2022 22:45:06 GMT
LABEL org.opencontainers.image.vendor=traefik org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.34 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:4025825e6ef43541c3a3e1ecb0092bc1b098e792051c7e338d6da54f66b19661`  
		Last Modified: Thu, 17 Mar 2022 14:34:09 GMT  
		Size: 2.6 MB (2629364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acc61b01c9ae829babc4ec995a57d752de240cbe8e3a8660191d3d21fc589a5f`  
		Last Modified: Thu, 17 Mar 2022 22:46:57 GMT  
		Size: 672.5 KB (672470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:244182210987061535c909a9a2aace43df0eb4ee95953b8813c3792dd4ba5b37`  
		Last Modified: Thu, 17 Mar 2022 22:47:55 GMT  
		Size: 20.6 MB (20623423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb981a93f73996a8309c5494870b9e83074dae0470e145590d2148af320281cf`  
		Last Modified: Thu, 17 Mar 2022 22:47:40 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:maroilles-alpine` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:1e7c544b79ed103ad6d22cd9941ca3416e02897a9cb7f75120f6fd5f1949d90c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.5 MB (23515893 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:11a718e3a556a699675cb6d5655875c7240cd58d718536719147125b9d171870`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 17 Mar 2022 18:43:12 GMT
ADD file:611998b78638b13e78919dd4635674032ab233f9b7aae6f62beaf6634cd18b9e in / 
# Thu, 17 Mar 2022 18:43:13 GMT
CMD ["/bin/sh"]
# Thu, 17 Mar 2022 21:06:35 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 17 Mar 2022 21:06:53 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/traefik/traefik/releases/download/v1.7.34/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Thu, 17 Mar 2022 21:06:55 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 17 Mar 2022 21:06:55 GMT
EXPOSE 80
# Thu, 17 Mar 2022 21:06:56 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 17 Mar 2022 21:06:57 GMT
CMD ["traefik"]
# Thu, 17 Mar 2022 21:06:58 GMT
LABEL org.opencontainers.image.vendor=traefik org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.34 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:93a1719cf26168d3a85db2594d76b17ccc4b25996620bceed3c2a13eaa165325`  
		Last Modified: Thu, 17 Mar 2022 18:44:00 GMT  
		Size: 2.7 MB (2715888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d012a4d53d2ad42f0d1b24f774778f1ea2d1c67cfdd0a1611fb7652fac92fc9b`  
		Last Modified: Thu, 17 Mar 2022 21:07:51 GMT  
		Size: 668.3 KB (668255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe57c71a6e6bc8b2eda9db22fd05c14079977728ba28062721c5d71106b23ab9`  
		Last Modified: Thu, 17 Mar 2022 21:08:21 GMT  
		Size: 20.1 MB (20131382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:535366a8854793a298d798c23544e4ad0849c13ce51c5687ad00f9864bebe75a`  
		Last Modified: Thu, 17 Mar 2022 21:08:18 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:maroilles-windowsservercore-1809`

```console
$ docker pull traefik@sha256:85ffe3d43fd4929a0e48d226e018af240fbbd8ea9a03685f74f1c78c432f85b3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2686; amd64

### `traefik:maroilles-windowsservercore-1809` - windows version 10.0.17763.2686; amd64

```console
$ docker pull traefik@sha256:67d210fa3d7dcb1ebc3b3b5f3bfdaac7d18195e1bb2b83fa2c1b1f48d09b08dd
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2738303983 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d6ebd04310fbdd68b4e7225310f8a6f2dec3a0330af0d02b74a9a0e35b79945b`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 03 Mar 2022 15:05:04 GMT
RUN Install update 1809-amd64
# Tue, 08 Mar 2022 19:31:54 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Mar 2022 18:53:09 GMT
RUN Invoke-WebRequest     -Uri "https://github.com/traefik/traefik/releases/download/v1.7.34/traefik_windows-amd64.exe"     -OutFile "/traefik.exe"
# Wed, 09 Mar 2022 18:53:10 GMT
EXPOSE 80
# Wed, 09 Mar 2022 18:53:11 GMT
ENTRYPOINT ["/traefik"]
# Wed, 09 Mar 2022 18:53:12 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.34 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:0a6173b79e25f2ebc0ed51b0ac32a6f65ca5a3bbfcbeab8b74a6c24324121dea`  
		Size: 997.1 MB (997119751 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a42bef5ec276ee3f8dd3545bf050f4ab85c8191392884f5d5ad6af6ae6e2eed2`  
		Last Modified: Tue, 08 Mar 2022 20:01:19 GMT  
		Size: 1.3 KB (1323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fd63edc5d2bde654b771ee58c8e9bb78539127758e862053223f402d3eaea68`  
		Last Modified: Wed, 09 Mar 2022 18:54:50 GMT  
		Size: 22.8 MB (22845783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cefe3e1f9703a33ffdf92a9c03b8a4738222fe08ea99aded6416f848aa300e9`  
		Last Modified: Wed, 09 Mar 2022 18:54:27 GMT  
		Size: 1.4 KB (1446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:939f3b18eb0ddb1cb4c6b01a2abc4127403c6a67c630a8c05c6be5f43ab74acc`  
		Last Modified: Wed, 09 Mar 2022 18:54:26 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35bcba10ab84d161e2dc32a48f6bc15da23d8aabdb22bbf4a89499ce18583d46`  
		Last Modified: Wed, 09 Mar 2022 18:54:26 GMT  
		Size: 1.4 KB (1389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:rocamadour`

```console
$ docker pull traefik@sha256:a94f8efcbdccb28e591fc04a3dce0cf5947e1b564c6d471a5945b09f130dfd86
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:rocamadour` - linux; amd64

```console
$ docker pull traefik@sha256:f3a0e9a0bdf260cf8c25c6ad7ee05cb05c3966d1058303b971b7057fc68a6457
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.3 MB (30325710 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cf9fa2c5f0d2e4c1cbf00e8ea973d74c8d11b1567205f5edc7284fdb0de166b3`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 17 Mar 2022 15:19:26 GMT
ADD file:8ec3735d4b1b4b070607b94e3bd360117b07dc26e1baf5dd485b49b3413e8fff in / 
# Thu, 17 Mar 2022 15:19:26 GMT
CMD ["/bin/sh"]
# Fri, 18 Mar 2022 06:23:06 GMT
RUN apk --no-cache add ca-certificates tzdata
# Fri, 18 Mar 2022 06:23:11 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.6.1/traefik_v2.6.1_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Fri, 18 Mar 2022 06:23:12 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Fri, 18 Mar 2022 06:23:12 GMT
EXPOSE 80
# Fri, 18 Mar 2022 06:23:12 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 18 Mar 2022 06:23:12 GMT
CMD ["traefik"]
# Fri, 18 Mar 2022 06:23:12 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.6.1 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:36ccefbf3d8a9a1b18baaa9cbf0f3ad50e8a7b751656c74df359900a318cbffc`  
		Last Modified: Thu, 17 Mar 2022 15:20:13 GMT  
		Size: 2.8 MB (2816169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d66f86d3f60579f394506161f82aafee52b414cd58c1060e18ca607a4fc9fbc4`  
		Last Modified: Fri, 18 Mar 2022 06:24:10 GMT  
		Size: 666.7 KB (666670 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01c1ca55dba5b4d567cb01859f50449eb49d7531bcde631825000d0135927d3d`  
		Last Modified: Fri, 18 Mar 2022 06:24:16 GMT  
		Size: 26.8 MB (26842504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:139a4e0ca97e6f942624418ee448c126f2084e4a79b2946064a434a48c3e8fbc`  
		Last Modified: Fri, 18 Mar 2022 06:24:10 GMT  
		Size: 367.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:rocamadour` - linux; arm variant v6

```console
$ docker pull traefik@sha256:2ff4bf1842307e9179d2c71959da827be092f581742b9751096bb1f55df78267
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.5 MB (28492404 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4eb2cddfb6417b47e508ee363f0b5a36a19bf5981662b7280742bc56aae3684e`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 17 Mar 2022 14:32:33 GMT
ADD file:8f1611b9334907a82945fdb21e17ee41541ab95050fc199c60fca662759171a5 in / 
# Thu, 17 Mar 2022 14:32:33 GMT
CMD ["/bin/sh"]
# Thu, 17 Mar 2022 22:44:31 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 17 Mar 2022 22:44:38 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.6.1/traefik_v2.6.1_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 17 Mar 2022 22:44:39 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 17 Mar 2022 22:44:39 GMT
EXPOSE 80
# Thu, 17 Mar 2022 22:44:40 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 17 Mar 2022 22:44:40 GMT
CMD ["traefik"]
# Thu, 17 Mar 2022 22:44:41 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.6.1 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:4025825e6ef43541c3a3e1ecb0092bc1b098e792051c7e338d6da54f66b19661`  
		Last Modified: Thu, 17 Mar 2022 14:34:09 GMT  
		Size: 2.6 MB (2629364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acc61b01c9ae829babc4ec995a57d752de240cbe8e3a8660191d3d21fc589a5f`  
		Last Modified: Thu, 17 Mar 2022 22:46:57 GMT  
		Size: 672.5 KB (672470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9054064868f20b2649a2e2a9141b8f8e9f915a8c0b21859cd801f175d7e2851b`  
		Last Modified: Thu, 17 Mar 2022 22:47:14 GMT  
		Size: 25.2 MB (25190202 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1be114305d9910bdd128e32db0ec6aef6c4ef92e6857b290d41387df34aeef2b`  
		Last Modified: Thu, 17 Mar 2022 22:46:57 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:rocamadour` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:57bea358260f808ed121400b19702fd8f6ac362f394ecdac9b55ab43c95d2940
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.9 MB (27867844 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:89657e32bf0a480cfe729a2bfb2ff094c143fab533f470e63d8c9b9faf123308`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 17 Mar 2022 18:43:12 GMT
ADD file:611998b78638b13e78919dd4635674032ab233f9b7aae6f62beaf6634cd18b9e in / 
# Thu, 17 Mar 2022 18:43:13 GMT
CMD ["/bin/sh"]
# Thu, 17 Mar 2022 21:06:35 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 17 Mar 2022 21:06:38 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.6.1/traefik_v2.6.1_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 17 Mar 2022 21:06:39 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 17 Mar 2022 21:06:39 GMT
EXPOSE 80
# Thu, 17 Mar 2022 21:06:40 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 17 Mar 2022 21:06:41 GMT
CMD ["traefik"]
# Thu, 17 Mar 2022 21:06:42 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.6.1 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:93a1719cf26168d3a85db2594d76b17ccc4b25996620bceed3c2a13eaa165325`  
		Last Modified: Thu, 17 Mar 2022 18:44:00 GMT  
		Size: 2.7 MB (2715888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d012a4d53d2ad42f0d1b24f774778f1ea2d1c67cfdd0a1611fb7652fac92fc9b`  
		Last Modified: Thu, 17 Mar 2022 21:07:51 GMT  
		Size: 668.3 KB (668255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8efd5dcd64fe25305ce09060a42d89619e8dbfb06e5be5633e1abc05d30445c5`  
		Last Modified: Thu, 17 Mar 2022 21:07:55 GMT  
		Size: 24.5 MB (24483333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1eb6f2eaa89fe53dae137bd6cd91f8ef241feeae582ecdf82d83834d8bd3733b`  
		Last Modified: Thu, 17 Mar 2022 21:07:50 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:rocamadour-windowsservercore-1809`

```console
$ docker pull traefik@sha256:b80deb28063ace6076665281bd27560fd3430b7b39f5bd15503c640defb8cf49
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2686; amd64

### `traefik:rocamadour-windowsservercore-1809` - windows version 10.0.17763.2686; amd64

```console
$ docker pull traefik@sha256:f57bdfbb46114920642abf2d1345012ecdb600175d227e38a2e681a1ebabfbd6
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2742866391 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2bf552045eeb764b54471001b799a24b4fa37c54b3aa7dbfa24c133f83d4ffb9`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 03 Mar 2022 15:05:04 GMT
RUN Install update 1809-amd64
# Tue, 08 Mar 2022 19:31:54 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Mar 2022 18:51:55 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/traefik/traefik/releases/download/v2.6.1/traefik_v2.6.1_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Wed, 09 Mar 2022 18:51:56 GMT
EXPOSE 80
# Wed, 09 Mar 2022 18:51:57 GMT
ENTRYPOINT ["/traefik"]
# Wed, 09 Mar 2022 18:51:58 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.6.1 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:0a6173b79e25f2ebc0ed51b0ac32a6f65ca5a3bbfcbeab8b74a6c24324121dea`  
		Size: 997.1 MB (997119751 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a42bef5ec276ee3f8dd3545bf050f4ab85c8191392884f5d5ad6af6ae6e2eed2`  
		Last Modified: Tue, 08 Mar 2022 20:01:19 GMT  
		Size: 1.3 KB (1323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61d553f74a3b073844e4c127831b8beebc1b835dc85e7c94513c77cc5c92e162`  
		Last Modified: Wed, 09 Mar 2022 18:54:08 GMT  
		Size: 27.4 MB (27408215 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2ef09b6978e9dfcd8c026989ac01b7a2a1acc1d57e058284c45efdfb0f0dd8a`  
		Last Modified: Wed, 09 Mar 2022 18:53:40 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc092ecf87d8664357e1628d8189f5c4c42972eb1dbcb6081f06524b75e0d8b5`  
		Last Modified: Wed, 09 Mar 2022 18:53:40 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8eebfe3ad70b0f95c3a0f566473bf5c42bbaf14434a4298c864e34bbcdf5e33`  
		Last Modified: Wed, 09 Mar 2022 18:53:40 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v1.7`

```console
$ docker pull traefik@sha256:1d8a41ae1bd54c9e9a5e0cc8da9002638932c53cc3d50c6f0c172238374ebe8f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:v1.7` - linux; amd64

```console
$ docker pull traefik@sha256:f705216279431ed8ab470318736acd767794a847acda2db325e3e159574bd03c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **22.6 MB (22607863 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:43de28b34d397393ca2d0ec8bd6923735fab787f8c3bd3dab0719cd256fcc010`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Fri, 18 Mar 2022 06:23:36 GMT
COPY file:8536203e9de8580f4424aff73a3be4185daba1818e4bfa286f2b290d1459aeb9 in /etc/ssl/certs/ 
# Fri, 18 Mar 2022 06:23:37 GMT
COPY dir:a84372748b89eb90478bb1b120b7c8fff3112421d7f93e50fbeae3f53adc6788 in /usr/share/ 
# Fri, 18 Mar 2022 06:23:38 GMT
COPY file:36217e5a6056bef26cfff395c8af8c1010a61dbe8d62b2c7869ca221e2a6302c in / 
# Fri, 18 Mar 2022 06:23:39 GMT
EXPOSE 80
# Fri, 18 Mar 2022 06:23:39 GMT
VOLUME [/tmp]
# Fri, 18 Mar 2022 06:23:39 GMT
ENTRYPOINT ["/traefik"]
# Fri, 18 Mar 2022 06:23:39 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.34 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:903e84870d1b7b581b2c6c362c74751a258cb8e2dbb443bddcd36fe8f29a20ab`  
		Last Modified: Fri, 18 Mar 2022 06:24:59 GMT  
		Size: 117.4 KB (117389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:914ae7a2b8652023026596365a1dfe88e317d16b1cc8099ee03c20357c95716e`  
		Last Modified: Fri, 18 Mar 2022 06:25:00 GMT  
		Size: 328.5 KB (328522 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f483c7bcad16f6ac0813c7a4704d4dc9319bfd6533f10c888b5e2ca21c72dc44`  
		Last Modified: Fri, 18 Mar 2022 06:25:05 GMT  
		Size: 22.2 MB (22161952 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v1.7` - linux; arm variant v6

```console
$ docker pull traefik@sha256:fe6bde6e9349ec036bc3aaec90c095006425bface50ee2f449e0d196cb5850c7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **21.1 MB (21069186 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5a5c3451377ef5e2379e4bc19691fb6c14b1a2215326833336e1db9e16cc5ca3`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Thu, 17 Mar 2022 22:45:25 GMT
COPY file:8536203e9de8580f4424aff73a3be4185daba1818e4bfa286f2b290d1459aeb9 in /etc/ssl/certs/ 
# Thu, 17 Mar 2022 22:45:27 GMT
COPY dir:a84372748b89eb90478bb1b120b7c8fff3112421d7f93e50fbeae3f53adc6788 in /usr/share/ 
# Thu, 17 Mar 2022 22:45:32 GMT
COPY file:5d1e7e81e8b77b4f8828eeaf0d30a0f135a949b51396f12ae22af376c36d3129 in / 
# Thu, 17 Mar 2022 22:45:33 GMT
EXPOSE 80
# Thu, 17 Mar 2022 22:45:33 GMT
VOLUME [/tmp]
# Thu, 17 Mar 2022 22:45:34 GMT
ENTRYPOINT ["/traefik"]
# Thu, 17 Mar 2022 22:45:34 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.34 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:27b61c1d4effca5c7137bfe0c8b6a3a228418ef37998781ad6cc7372c6f7e98f`  
		Last Modified: Thu, 17 Mar 2022 22:48:17 GMT  
		Size: 117.4 KB (117390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98aae3b48a316f885b1d485fee6b2ffffb3c2c7dea49cea01019d4c103b204da`  
		Last Modified: Thu, 17 Mar 2022 22:48:18 GMT  
		Size: 328.5 KB (328514 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a82873a2be1cc2b2dfbc565c4bf9960f32b61892f49f0911ec1ac7e310210c3d`  
		Last Modified: Thu, 17 Mar 2022 22:48:34 GMT  
		Size: 20.6 MB (20623282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v1.7` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:c2930d3e36f7feb98470b85e8bc9fce0016fc5eadbc805249e63d6a458eb2323
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **20.6 MB (20577242 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f7338e148255e82dd93286a1f87db35f499d4e391d7f5f3e1bfb6c71ed4ec2d4`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Thu, 17 Mar 2022 21:07:07 GMT
COPY file:8536203e9de8580f4424aff73a3be4185daba1818e4bfa286f2b290d1459aeb9 in /etc/ssl/certs/ 
# Thu, 17 Mar 2022 21:07:08 GMT
COPY dir:a84372748b89eb90478bb1b120b7c8fff3112421d7f93e50fbeae3f53adc6788 in /usr/share/ 
# Thu, 17 Mar 2022 21:07:09 GMT
COPY file:60330593b6644f3f519fd13ce8ee34c2c7ab9994a1420afabbc01926dd1230dd in / 
# Thu, 17 Mar 2022 21:07:09 GMT
EXPOSE 80
# Thu, 17 Mar 2022 21:07:10 GMT
VOLUME [/tmp]
# Thu, 17 Mar 2022 21:07:11 GMT
ENTRYPOINT ["/traefik"]
# Thu, 17 Mar 2022 21:07:12 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.34 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:86cd07830d2730c0aa24f0e47380af5ef760945b5049a2e72a8ebe0675ed6d34`  
		Last Modified: Thu, 17 Mar 2022 21:08:41 GMT  
		Size: 117.4 KB (117390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:135b9e65a5ea0b642df02ea2cf73c74a353d1cbfa3b95d048a4adbf0bacf9653`  
		Last Modified: Thu, 17 Mar 2022 21:08:41 GMT  
		Size: 328.5 KB (328505 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bee8fa09b05c38fc9116b1446ac3d204200577fd9bfb1801d684657dc722b74b`  
		Last Modified: Thu, 17 Mar 2022 21:08:45 GMT  
		Size: 20.1 MB (20131347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v1.7-alpine`

```console
$ docker pull traefik@sha256:8ac75422d559a55193d20df11116ea951ad962f7dcdf3bd76a51f81f460de821
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:v1.7-alpine` - linux; amd64

```console
$ docker pull traefik@sha256:04c41c7c3ff03d006e93029fb6bce95a448a32900c47487cf2f54f4df2d42f56
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.6 MB (25645268 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9eb8c5f993e88b67da6b9d2b5ee0a09e7f6a576c70e19f8bd1031adae54418ca`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 17 Mar 2022 15:19:26 GMT
ADD file:8ec3735d4b1b4b070607b94e3bd360117b07dc26e1baf5dd485b49b3413e8fff in / 
# Thu, 17 Mar 2022 15:19:26 GMT
CMD ["/bin/sh"]
# Fri, 18 Mar 2022 06:23:06 GMT
RUN apk --no-cache add ca-certificates tzdata
# Fri, 18 Mar 2022 06:23:24 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/traefik/traefik/releases/download/v1.7.34/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Fri, 18 Mar 2022 06:23:24 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Fri, 18 Mar 2022 06:23:24 GMT
EXPOSE 80
# Fri, 18 Mar 2022 06:23:24 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 18 Mar 2022 06:23:24 GMT
CMD ["traefik"]
# Fri, 18 Mar 2022 06:23:25 GMT
LABEL org.opencontainers.image.vendor=traefik org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.34 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:36ccefbf3d8a9a1b18baaa9cbf0f3ad50e8a7b751656c74df359900a318cbffc`  
		Last Modified: Thu, 17 Mar 2022 15:20:13 GMT  
		Size: 2.8 MB (2816169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d66f86d3f60579f394506161f82aafee52b414cd58c1060e18ca607a4fc9fbc4`  
		Last Modified: Fri, 18 Mar 2022 06:24:10 GMT  
		Size: 666.7 KB (666670 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b9a06ba42895ffa47fb412ee9c0fe6cc5c33d4bf08ca4a76e74f7040bc82206`  
		Last Modified: Fri, 18 Mar 2022 06:24:42 GMT  
		Size: 22.2 MB (22162062 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b266beb8763fa8eeb482f01673624fb468758ac98bb28cc16881d8f94e1f54c`  
		Last Modified: Fri, 18 Mar 2022 06:24:36 GMT  
		Size: 367.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v1.7-alpine` - linux; arm variant v6

```console
$ docker pull traefik@sha256:08be027ed453b435111cb912908324ee1f5f0d77db60b6d6f9f10003d2c62674
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.9 MB (23925625 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d5fbe3dd0a206256fa43655ee4af71da94003b6377978bc54ccdb219452f1bcc`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 17 Mar 2022 14:32:33 GMT
ADD file:8f1611b9334907a82945fdb21e17ee41541ab95050fc199c60fca662759171a5 in / 
# Thu, 17 Mar 2022 14:32:33 GMT
CMD ["/bin/sh"]
# Thu, 17 Mar 2022 22:44:31 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 17 Mar 2022 22:45:03 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/traefik/traefik/releases/download/v1.7.34/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Thu, 17 Mar 2022 22:45:03 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 17 Mar 2022 22:45:04 GMT
EXPOSE 80
# Thu, 17 Mar 2022 22:45:05 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 17 Mar 2022 22:45:05 GMT
CMD ["traefik"]
# Thu, 17 Mar 2022 22:45:06 GMT
LABEL org.opencontainers.image.vendor=traefik org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.34 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:4025825e6ef43541c3a3e1ecb0092bc1b098e792051c7e338d6da54f66b19661`  
		Last Modified: Thu, 17 Mar 2022 14:34:09 GMT  
		Size: 2.6 MB (2629364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acc61b01c9ae829babc4ec995a57d752de240cbe8e3a8660191d3d21fc589a5f`  
		Last Modified: Thu, 17 Mar 2022 22:46:57 GMT  
		Size: 672.5 KB (672470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:244182210987061535c909a9a2aace43df0eb4ee95953b8813c3792dd4ba5b37`  
		Last Modified: Thu, 17 Mar 2022 22:47:55 GMT  
		Size: 20.6 MB (20623423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb981a93f73996a8309c5494870b9e83074dae0470e145590d2148af320281cf`  
		Last Modified: Thu, 17 Mar 2022 22:47:40 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v1.7-alpine` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:1e7c544b79ed103ad6d22cd9941ca3416e02897a9cb7f75120f6fd5f1949d90c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.5 MB (23515893 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:11a718e3a556a699675cb6d5655875c7240cd58d718536719147125b9d171870`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 17 Mar 2022 18:43:12 GMT
ADD file:611998b78638b13e78919dd4635674032ab233f9b7aae6f62beaf6634cd18b9e in / 
# Thu, 17 Mar 2022 18:43:13 GMT
CMD ["/bin/sh"]
# Thu, 17 Mar 2022 21:06:35 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 17 Mar 2022 21:06:53 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/traefik/traefik/releases/download/v1.7.34/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Thu, 17 Mar 2022 21:06:55 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 17 Mar 2022 21:06:55 GMT
EXPOSE 80
# Thu, 17 Mar 2022 21:06:56 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 17 Mar 2022 21:06:57 GMT
CMD ["traefik"]
# Thu, 17 Mar 2022 21:06:58 GMT
LABEL org.opencontainers.image.vendor=traefik org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.34 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:93a1719cf26168d3a85db2594d76b17ccc4b25996620bceed3c2a13eaa165325`  
		Last Modified: Thu, 17 Mar 2022 18:44:00 GMT  
		Size: 2.7 MB (2715888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d012a4d53d2ad42f0d1b24f774778f1ea2d1c67cfdd0a1611fb7652fac92fc9b`  
		Last Modified: Thu, 17 Mar 2022 21:07:51 GMT  
		Size: 668.3 KB (668255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe57c71a6e6bc8b2eda9db22fd05c14079977728ba28062721c5d71106b23ab9`  
		Last Modified: Thu, 17 Mar 2022 21:08:21 GMT  
		Size: 20.1 MB (20131382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:535366a8854793a298d798c23544e4ad0849c13ce51c5687ad00f9864bebe75a`  
		Last Modified: Thu, 17 Mar 2022 21:08:18 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v1.7-windowsservercore-1809`

```console
$ docker pull traefik@sha256:85ffe3d43fd4929a0e48d226e018af240fbbd8ea9a03685f74f1c78c432f85b3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2686; amd64

### `traefik:v1.7-windowsservercore-1809` - windows version 10.0.17763.2686; amd64

```console
$ docker pull traefik@sha256:67d210fa3d7dcb1ebc3b3b5f3bfdaac7d18195e1bb2b83fa2c1b1f48d09b08dd
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2738303983 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d6ebd04310fbdd68b4e7225310f8a6f2dec3a0330af0d02b74a9a0e35b79945b`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 03 Mar 2022 15:05:04 GMT
RUN Install update 1809-amd64
# Tue, 08 Mar 2022 19:31:54 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Mar 2022 18:53:09 GMT
RUN Invoke-WebRequest     -Uri "https://github.com/traefik/traefik/releases/download/v1.7.34/traefik_windows-amd64.exe"     -OutFile "/traefik.exe"
# Wed, 09 Mar 2022 18:53:10 GMT
EXPOSE 80
# Wed, 09 Mar 2022 18:53:11 GMT
ENTRYPOINT ["/traefik"]
# Wed, 09 Mar 2022 18:53:12 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.34 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:0a6173b79e25f2ebc0ed51b0ac32a6f65ca5a3bbfcbeab8b74a6c24324121dea`  
		Size: 997.1 MB (997119751 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a42bef5ec276ee3f8dd3545bf050f4ab85c8191392884f5d5ad6af6ae6e2eed2`  
		Last Modified: Tue, 08 Mar 2022 20:01:19 GMT  
		Size: 1.3 KB (1323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fd63edc5d2bde654b771ee58c8e9bb78539127758e862053223f402d3eaea68`  
		Last Modified: Wed, 09 Mar 2022 18:54:50 GMT  
		Size: 22.8 MB (22845783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cefe3e1f9703a33ffdf92a9c03b8a4738222fe08ea99aded6416f848aa300e9`  
		Last Modified: Wed, 09 Mar 2022 18:54:27 GMT  
		Size: 1.4 KB (1446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:939f3b18eb0ddb1cb4c6b01a2abc4127403c6a67c630a8c05c6be5f43ab74acc`  
		Last Modified: Wed, 09 Mar 2022 18:54:26 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35bcba10ab84d161e2dc32a48f6bc15da23d8aabdb22bbf4a89499ce18583d46`  
		Last Modified: Wed, 09 Mar 2022 18:54:26 GMT  
		Size: 1.4 KB (1389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v1.7.34`

```console
$ docker pull traefik@sha256:1d8a41ae1bd54c9e9a5e0cc8da9002638932c53cc3d50c6f0c172238374ebe8f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:v1.7.34` - linux; amd64

```console
$ docker pull traefik@sha256:f705216279431ed8ab470318736acd767794a847acda2db325e3e159574bd03c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **22.6 MB (22607863 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:43de28b34d397393ca2d0ec8bd6923735fab787f8c3bd3dab0719cd256fcc010`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Fri, 18 Mar 2022 06:23:36 GMT
COPY file:8536203e9de8580f4424aff73a3be4185daba1818e4bfa286f2b290d1459aeb9 in /etc/ssl/certs/ 
# Fri, 18 Mar 2022 06:23:37 GMT
COPY dir:a84372748b89eb90478bb1b120b7c8fff3112421d7f93e50fbeae3f53adc6788 in /usr/share/ 
# Fri, 18 Mar 2022 06:23:38 GMT
COPY file:36217e5a6056bef26cfff395c8af8c1010a61dbe8d62b2c7869ca221e2a6302c in / 
# Fri, 18 Mar 2022 06:23:39 GMT
EXPOSE 80
# Fri, 18 Mar 2022 06:23:39 GMT
VOLUME [/tmp]
# Fri, 18 Mar 2022 06:23:39 GMT
ENTRYPOINT ["/traefik"]
# Fri, 18 Mar 2022 06:23:39 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.34 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:903e84870d1b7b581b2c6c362c74751a258cb8e2dbb443bddcd36fe8f29a20ab`  
		Last Modified: Fri, 18 Mar 2022 06:24:59 GMT  
		Size: 117.4 KB (117389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:914ae7a2b8652023026596365a1dfe88e317d16b1cc8099ee03c20357c95716e`  
		Last Modified: Fri, 18 Mar 2022 06:25:00 GMT  
		Size: 328.5 KB (328522 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f483c7bcad16f6ac0813c7a4704d4dc9319bfd6533f10c888b5e2ca21c72dc44`  
		Last Modified: Fri, 18 Mar 2022 06:25:05 GMT  
		Size: 22.2 MB (22161952 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v1.7.34` - linux; arm variant v6

```console
$ docker pull traefik@sha256:fe6bde6e9349ec036bc3aaec90c095006425bface50ee2f449e0d196cb5850c7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **21.1 MB (21069186 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5a5c3451377ef5e2379e4bc19691fb6c14b1a2215326833336e1db9e16cc5ca3`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Thu, 17 Mar 2022 22:45:25 GMT
COPY file:8536203e9de8580f4424aff73a3be4185daba1818e4bfa286f2b290d1459aeb9 in /etc/ssl/certs/ 
# Thu, 17 Mar 2022 22:45:27 GMT
COPY dir:a84372748b89eb90478bb1b120b7c8fff3112421d7f93e50fbeae3f53adc6788 in /usr/share/ 
# Thu, 17 Mar 2022 22:45:32 GMT
COPY file:5d1e7e81e8b77b4f8828eeaf0d30a0f135a949b51396f12ae22af376c36d3129 in / 
# Thu, 17 Mar 2022 22:45:33 GMT
EXPOSE 80
# Thu, 17 Mar 2022 22:45:33 GMT
VOLUME [/tmp]
# Thu, 17 Mar 2022 22:45:34 GMT
ENTRYPOINT ["/traefik"]
# Thu, 17 Mar 2022 22:45:34 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.34 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:27b61c1d4effca5c7137bfe0c8b6a3a228418ef37998781ad6cc7372c6f7e98f`  
		Last Modified: Thu, 17 Mar 2022 22:48:17 GMT  
		Size: 117.4 KB (117390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98aae3b48a316f885b1d485fee6b2ffffb3c2c7dea49cea01019d4c103b204da`  
		Last Modified: Thu, 17 Mar 2022 22:48:18 GMT  
		Size: 328.5 KB (328514 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a82873a2be1cc2b2dfbc565c4bf9960f32b61892f49f0911ec1ac7e310210c3d`  
		Last Modified: Thu, 17 Mar 2022 22:48:34 GMT  
		Size: 20.6 MB (20623282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v1.7.34` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:c2930d3e36f7feb98470b85e8bc9fce0016fc5eadbc805249e63d6a458eb2323
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **20.6 MB (20577242 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f7338e148255e82dd93286a1f87db35f499d4e391d7f5f3e1bfb6c71ed4ec2d4`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Thu, 17 Mar 2022 21:07:07 GMT
COPY file:8536203e9de8580f4424aff73a3be4185daba1818e4bfa286f2b290d1459aeb9 in /etc/ssl/certs/ 
# Thu, 17 Mar 2022 21:07:08 GMT
COPY dir:a84372748b89eb90478bb1b120b7c8fff3112421d7f93e50fbeae3f53adc6788 in /usr/share/ 
# Thu, 17 Mar 2022 21:07:09 GMT
COPY file:60330593b6644f3f519fd13ce8ee34c2c7ab9994a1420afabbc01926dd1230dd in / 
# Thu, 17 Mar 2022 21:07:09 GMT
EXPOSE 80
# Thu, 17 Mar 2022 21:07:10 GMT
VOLUME [/tmp]
# Thu, 17 Mar 2022 21:07:11 GMT
ENTRYPOINT ["/traefik"]
# Thu, 17 Mar 2022 21:07:12 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.34 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:86cd07830d2730c0aa24f0e47380af5ef760945b5049a2e72a8ebe0675ed6d34`  
		Last Modified: Thu, 17 Mar 2022 21:08:41 GMT  
		Size: 117.4 KB (117390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:135b9e65a5ea0b642df02ea2cf73c74a353d1cbfa3b95d048a4adbf0bacf9653`  
		Last Modified: Thu, 17 Mar 2022 21:08:41 GMT  
		Size: 328.5 KB (328505 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bee8fa09b05c38fc9116b1446ac3d204200577fd9bfb1801d684657dc722b74b`  
		Last Modified: Thu, 17 Mar 2022 21:08:45 GMT  
		Size: 20.1 MB (20131347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v1.7.34-alpine`

```console
$ docker pull traefik@sha256:8ac75422d559a55193d20df11116ea951ad962f7dcdf3bd76a51f81f460de821
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:v1.7.34-alpine` - linux; amd64

```console
$ docker pull traefik@sha256:04c41c7c3ff03d006e93029fb6bce95a448a32900c47487cf2f54f4df2d42f56
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.6 MB (25645268 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9eb8c5f993e88b67da6b9d2b5ee0a09e7f6a576c70e19f8bd1031adae54418ca`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 17 Mar 2022 15:19:26 GMT
ADD file:8ec3735d4b1b4b070607b94e3bd360117b07dc26e1baf5dd485b49b3413e8fff in / 
# Thu, 17 Mar 2022 15:19:26 GMT
CMD ["/bin/sh"]
# Fri, 18 Mar 2022 06:23:06 GMT
RUN apk --no-cache add ca-certificates tzdata
# Fri, 18 Mar 2022 06:23:24 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/traefik/traefik/releases/download/v1.7.34/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Fri, 18 Mar 2022 06:23:24 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Fri, 18 Mar 2022 06:23:24 GMT
EXPOSE 80
# Fri, 18 Mar 2022 06:23:24 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 18 Mar 2022 06:23:24 GMT
CMD ["traefik"]
# Fri, 18 Mar 2022 06:23:25 GMT
LABEL org.opencontainers.image.vendor=traefik org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.34 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:36ccefbf3d8a9a1b18baaa9cbf0f3ad50e8a7b751656c74df359900a318cbffc`  
		Last Modified: Thu, 17 Mar 2022 15:20:13 GMT  
		Size: 2.8 MB (2816169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d66f86d3f60579f394506161f82aafee52b414cd58c1060e18ca607a4fc9fbc4`  
		Last Modified: Fri, 18 Mar 2022 06:24:10 GMT  
		Size: 666.7 KB (666670 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b9a06ba42895ffa47fb412ee9c0fe6cc5c33d4bf08ca4a76e74f7040bc82206`  
		Last Modified: Fri, 18 Mar 2022 06:24:42 GMT  
		Size: 22.2 MB (22162062 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b266beb8763fa8eeb482f01673624fb468758ac98bb28cc16881d8f94e1f54c`  
		Last Modified: Fri, 18 Mar 2022 06:24:36 GMT  
		Size: 367.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v1.7.34-alpine` - linux; arm variant v6

```console
$ docker pull traefik@sha256:08be027ed453b435111cb912908324ee1f5f0d77db60b6d6f9f10003d2c62674
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.9 MB (23925625 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d5fbe3dd0a206256fa43655ee4af71da94003b6377978bc54ccdb219452f1bcc`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 17 Mar 2022 14:32:33 GMT
ADD file:8f1611b9334907a82945fdb21e17ee41541ab95050fc199c60fca662759171a5 in / 
# Thu, 17 Mar 2022 14:32:33 GMT
CMD ["/bin/sh"]
# Thu, 17 Mar 2022 22:44:31 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 17 Mar 2022 22:45:03 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/traefik/traefik/releases/download/v1.7.34/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Thu, 17 Mar 2022 22:45:03 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 17 Mar 2022 22:45:04 GMT
EXPOSE 80
# Thu, 17 Mar 2022 22:45:05 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 17 Mar 2022 22:45:05 GMT
CMD ["traefik"]
# Thu, 17 Mar 2022 22:45:06 GMT
LABEL org.opencontainers.image.vendor=traefik org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.34 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:4025825e6ef43541c3a3e1ecb0092bc1b098e792051c7e338d6da54f66b19661`  
		Last Modified: Thu, 17 Mar 2022 14:34:09 GMT  
		Size: 2.6 MB (2629364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acc61b01c9ae829babc4ec995a57d752de240cbe8e3a8660191d3d21fc589a5f`  
		Last Modified: Thu, 17 Mar 2022 22:46:57 GMT  
		Size: 672.5 KB (672470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:244182210987061535c909a9a2aace43df0eb4ee95953b8813c3792dd4ba5b37`  
		Last Modified: Thu, 17 Mar 2022 22:47:55 GMT  
		Size: 20.6 MB (20623423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb981a93f73996a8309c5494870b9e83074dae0470e145590d2148af320281cf`  
		Last Modified: Thu, 17 Mar 2022 22:47:40 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v1.7.34-alpine` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:1e7c544b79ed103ad6d22cd9941ca3416e02897a9cb7f75120f6fd5f1949d90c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.5 MB (23515893 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:11a718e3a556a699675cb6d5655875c7240cd58d718536719147125b9d171870`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 17 Mar 2022 18:43:12 GMT
ADD file:611998b78638b13e78919dd4635674032ab233f9b7aae6f62beaf6634cd18b9e in / 
# Thu, 17 Mar 2022 18:43:13 GMT
CMD ["/bin/sh"]
# Thu, 17 Mar 2022 21:06:35 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 17 Mar 2022 21:06:53 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/traefik/traefik/releases/download/v1.7.34/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Thu, 17 Mar 2022 21:06:55 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 17 Mar 2022 21:06:55 GMT
EXPOSE 80
# Thu, 17 Mar 2022 21:06:56 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 17 Mar 2022 21:06:57 GMT
CMD ["traefik"]
# Thu, 17 Mar 2022 21:06:58 GMT
LABEL org.opencontainers.image.vendor=traefik org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.34 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:93a1719cf26168d3a85db2594d76b17ccc4b25996620bceed3c2a13eaa165325`  
		Last Modified: Thu, 17 Mar 2022 18:44:00 GMT  
		Size: 2.7 MB (2715888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d012a4d53d2ad42f0d1b24f774778f1ea2d1c67cfdd0a1611fb7652fac92fc9b`  
		Last Modified: Thu, 17 Mar 2022 21:07:51 GMT  
		Size: 668.3 KB (668255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe57c71a6e6bc8b2eda9db22fd05c14079977728ba28062721c5d71106b23ab9`  
		Last Modified: Thu, 17 Mar 2022 21:08:21 GMT  
		Size: 20.1 MB (20131382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:535366a8854793a298d798c23544e4ad0849c13ce51c5687ad00f9864bebe75a`  
		Last Modified: Thu, 17 Mar 2022 21:08:18 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v1.7.34-windowsservercore-1809`

```console
$ docker pull traefik@sha256:85ffe3d43fd4929a0e48d226e018af240fbbd8ea9a03685f74f1c78c432f85b3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2686; amd64

### `traefik:v1.7.34-windowsservercore-1809` - windows version 10.0.17763.2686; amd64

```console
$ docker pull traefik@sha256:67d210fa3d7dcb1ebc3b3b5f3bfdaac7d18195e1bb2b83fa2c1b1f48d09b08dd
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2738303983 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d6ebd04310fbdd68b4e7225310f8a6f2dec3a0330af0d02b74a9a0e35b79945b`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 03 Mar 2022 15:05:04 GMT
RUN Install update 1809-amd64
# Tue, 08 Mar 2022 19:31:54 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Mar 2022 18:53:09 GMT
RUN Invoke-WebRequest     -Uri "https://github.com/traefik/traefik/releases/download/v1.7.34/traefik_windows-amd64.exe"     -OutFile "/traefik.exe"
# Wed, 09 Mar 2022 18:53:10 GMT
EXPOSE 80
# Wed, 09 Mar 2022 18:53:11 GMT
ENTRYPOINT ["/traefik"]
# Wed, 09 Mar 2022 18:53:12 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.34 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:0a6173b79e25f2ebc0ed51b0ac32a6f65ca5a3bbfcbeab8b74a6c24324121dea`  
		Size: 997.1 MB (997119751 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a42bef5ec276ee3f8dd3545bf050f4ab85c8191392884f5d5ad6af6ae6e2eed2`  
		Last Modified: Tue, 08 Mar 2022 20:01:19 GMT  
		Size: 1.3 KB (1323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fd63edc5d2bde654b771ee58c8e9bb78539127758e862053223f402d3eaea68`  
		Last Modified: Wed, 09 Mar 2022 18:54:50 GMT  
		Size: 22.8 MB (22845783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cefe3e1f9703a33ffdf92a9c03b8a4738222fe08ea99aded6416f848aa300e9`  
		Last Modified: Wed, 09 Mar 2022 18:54:27 GMT  
		Size: 1.4 KB (1446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:939f3b18eb0ddb1cb4c6b01a2abc4127403c6a67c630a8c05c6be5f43ab74acc`  
		Last Modified: Wed, 09 Mar 2022 18:54:26 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35bcba10ab84d161e2dc32a48f6bc15da23d8aabdb22bbf4a89499ce18583d46`  
		Last Modified: Wed, 09 Mar 2022 18:54:26 GMT  
		Size: 1.4 KB (1389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v2.6`

```console
$ docker pull traefik@sha256:a94f8efcbdccb28e591fc04a3dce0cf5947e1b564c6d471a5945b09f130dfd86
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:v2.6` - linux; amd64

```console
$ docker pull traefik@sha256:f3a0e9a0bdf260cf8c25c6ad7ee05cb05c3966d1058303b971b7057fc68a6457
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.3 MB (30325710 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cf9fa2c5f0d2e4c1cbf00e8ea973d74c8d11b1567205f5edc7284fdb0de166b3`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 17 Mar 2022 15:19:26 GMT
ADD file:8ec3735d4b1b4b070607b94e3bd360117b07dc26e1baf5dd485b49b3413e8fff in / 
# Thu, 17 Mar 2022 15:19:26 GMT
CMD ["/bin/sh"]
# Fri, 18 Mar 2022 06:23:06 GMT
RUN apk --no-cache add ca-certificates tzdata
# Fri, 18 Mar 2022 06:23:11 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.6.1/traefik_v2.6.1_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Fri, 18 Mar 2022 06:23:12 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Fri, 18 Mar 2022 06:23:12 GMT
EXPOSE 80
# Fri, 18 Mar 2022 06:23:12 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 18 Mar 2022 06:23:12 GMT
CMD ["traefik"]
# Fri, 18 Mar 2022 06:23:12 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.6.1 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:36ccefbf3d8a9a1b18baaa9cbf0f3ad50e8a7b751656c74df359900a318cbffc`  
		Last Modified: Thu, 17 Mar 2022 15:20:13 GMT  
		Size: 2.8 MB (2816169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d66f86d3f60579f394506161f82aafee52b414cd58c1060e18ca607a4fc9fbc4`  
		Last Modified: Fri, 18 Mar 2022 06:24:10 GMT  
		Size: 666.7 KB (666670 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01c1ca55dba5b4d567cb01859f50449eb49d7531bcde631825000d0135927d3d`  
		Last Modified: Fri, 18 Mar 2022 06:24:16 GMT  
		Size: 26.8 MB (26842504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:139a4e0ca97e6f942624418ee448c126f2084e4a79b2946064a434a48c3e8fbc`  
		Last Modified: Fri, 18 Mar 2022 06:24:10 GMT  
		Size: 367.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v2.6` - linux; arm variant v6

```console
$ docker pull traefik@sha256:2ff4bf1842307e9179d2c71959da827be092f581742b9751096bb1f55df78267
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.5 MB (28492404 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4eb2cddfb6417b47e508ee363f0b5a36a19bf5981662b7280742bc56aae3684e`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 17 Mar 2022 14:32:33 GMT
ADD file:8f1611b9334907a82945fdb21e17ee41541ab95050fc199c60fca662759171a5 in / 
# Thu, 17 Mar 2022 14:32:33 GMT
CMD ["/bin/sh"]
# Thu, 17 Mar 2022 22:44:31 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 17 Mar 2022 22:44:38 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.6.1/traefik_v2.6.1_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 17 Mar 2022 22:44:39 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 17 Mar 2022 22:44:39 GMT
EXPOSE 80
# Thu, 17 Mar 2022 22:44:40 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 17 Mar 2022 22:44:40 GMT
CMD ["traefik"]
# Thu, 17 Mar 2022 22:44:41 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.6.1 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:4025825e6ef43541c3a3e1ecb0092bc1b098e792051c7e338d6da54f66b19661`  
		Last Modified: Thu, 17 Mar 2022 14:34:09 GMT  
		Size: 2.6 MB (2629364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acc61b01c9ae829babc4ec995a57d752de240cbe8e3a8660191d3d21fc589a5f`  
		Last Modified: Thu, 17 Mar 2022 22:46:57 GMT  
		Size: 672.5 KB (672470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9054064868f20b2649a2e2a9141b8f8e9f915a8c0b21859cd801f175d7e2851b`  
		Last Modified: Thu, 17 Mar 2022 22:47:14 GMT  
		Size: 25.2 MB (25190202 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1be114305d9910bdd128e32db0ec6aef6c4ef92e6857b290d41387df34aeef2b`  
		Last Modified: Thu, 17 Mar 2022 22:46:57 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v2.6` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:57bea358260f808ed121400b19702fd8f6ac362f394ecdac9b55ab43c95d2940
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.9 MB (27867844 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:89657e32bf0a480cfe729a2bfb2ff094c143fab533f470e63d8c9b9faf123308`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 17 Mar 2022 18:43:12 GMT
ADD file:611998b78638b13e78919dd4635674032ab233f9b7aae6f62beaf6634cd18b9e in / 
# Thu, 17 Mar 2022 18:43:13 GMT
CMD ["/bin/sh"]
# Thu, 17 Mar 2022 21:06:35 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 17 Mar 2022 21:06:38 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.6.1/traefik_v2.6.1_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 17 Mar 2022 21:06:39 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 17 Mar 2022 21:06:39 GMT
EXPOSE 80
# Thu, 17 Mar 2022 21:06:40 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 17 Mar 2022 21:06:41 GMT
CMD ["traefik"]
# Thu, 17 Mar 2022 21:06:42 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.6.1 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:93a1719cf26168d3a85db2594d76b17ccc4b25996620bceed3c2a13eaa165325`  
		Last Modified: Thu, 17 Mar 2022 18:44:00 GMT  
		Size: 2.7 MB (2715888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d012a4d53d2ad42f0d1b24f774778f1ea2d1c67cfdd0a1611fb7652fac92fc9b`  
		Last Modified: Thu, 17 Mar 2022 21:07:51 GMT  
		Size: 668.3 KB (668255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8efd5dcd64fe25305ce09060a42d89619e8dbfb06e5be5633e1abc05d30445c5`  
		Last Modified: Thu, 17 Mar 2022 21:07:55 GMT  
		Size: 24.5 MB (24483333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1eb6f2eaa89fe53dae137bd6cd91f8ef241feeae582ecdf82d83834d8bd3733b`  
		Last Modified: Thu, 17 Mar 2022 21:07:50 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v2.6-windowsservercore-1809`

```console
$ docker pull traefik@sha256:b80deb28063ace6076665281bd27560fd3430b7b39f5bd15503c640defb8cf49
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2686; amd64

### `traefik:v2.6-windowsservercore-1809` - windows version 10.0.17763.2686; amd64

```console
$ docker pull traefik@sha256:f57bdfbb46114920642abf2d1345012ecdb600175d227e38a2e681a1ebabfbd6
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2742866391 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2bf552045eeb764b54471001b799a24b4fa37c54b3aa7dbfa24c133f83d4ffb9`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 03 Mar 2022 15:05:04 GMT
RUN Install update 1809-amd64
# Tue, 08 Mar 2022 19:31:54 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Mar 2022 18:51:55 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/traefik/traefik/releases/download/v2.6.1/traefik_v2.6.1_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Wed, 09 Mar 2022 18:51:56 GMT
EXPOSE 80
# Wed, 09 Mar 2022 18:51:57 GMT
ENTRYPOINT ["/traefik"]
# Wed, 09 Mar 2022 18:51:58 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.6.1 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:0a6173b79e25f2ebc0ed51b0ac32a6f65ca5a3bbfcbeab8b74a6c24324121dea`  
		Size: 997.1 MB (997119751 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a42bef5ec276ee3f8dd3545bf050f4ab85c8191392884f5d5ad6af6ae6e2eed2`  
		Last Modified: Tue, 08 Mar 2022 20:01:19 GMT  
		Size: 1.3 KB (1323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61d553f74a3b073844e4c127831b8beebc1b835dc85e7c94513c77cc5c92e162`  
		Last Modified: Wed, 09 Mar 2022 18:54:08 GMT  
		Size: 27.4 MB (27408215 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2ef09b6978e9dfcd8c026989ac01b7a2a1acc1d57e058284c45efdfb0f0dd8a`  
		Last Modified: Wed, 09 Mar 2022 18:53:40 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc092ecf87d8664357e1628d8189f5c4c42972eb1dbcb6081f06524b75e0d8b5`  
		Last Modified: Wed, 09 Mar 2022 18:53:40 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8eebfe3ad70b0f95c3a0f566473bf5c42bbaf14434a4298c864e34bbcdf5e33`  
		Last Modified: Wed, 09 Mar 2022 18:53:40 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v2.6.1`

```console
$ docker pull traefik@sha256:a94f8efcbdccb28e591fc04a3dce0cf5947e1b564c6d471a5945b09f130dfd86
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:v2.6.1` - linux; amd64

```console
$ docker pull traefik@sha256:f3a0e9a0bdf260cf8c25c6ad7ee05cb05c3966d1058303b971b7057fc68a6457
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.3 MB (30325710 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cf9fa2c5f0d2e4c1cbf00e8ea973d74c8d11b1567205f5edc7284fdb0de166b3`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 17 Mar 2022 15:19:26 GMT
ADD file:8ec3735d4b1b4b070607b94e3bd360117b07dc26e1baf5dd485b49b3413e8fff in / 
# Thu, 17 Mar 2022 15:19:26 GMT
CMD ["/bin/sh"]
# Fri, 18 Mar 2022 06:23:06 GMT
RUN apk --no-cache add ca-certificates tzdata
# Fri, 18 Mar 2022 06:23:11 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.6.1/traefik_v2.6.1_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Fri, 18 Mar 2022 06:23:12 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Fri, 18 Mar 2022 06:23:12 GMT
EXPOSE 80
# Fri, 18 Mar 2022 06:23:12 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 18 Mar 2022 06:23:12 GMT
CMD ["traefik"]
# Fri, 18 Mar 2022 06:23:12 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.6.1 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:36ccefbf3d8a9a1b18baaa9cbf0f3ad50e8a7b751656c74df359900a318cbffc`  
		Last Modified: Thu, 17 Mar 2022 15:20:13 GMT  
		Size: 2.8 MB (2816169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d66f86d3f60579f394506161f82aafee52b414cd58c1060e18ca607a4fc9fbc4`  
		Last Modified: Fri, 18 Mar 2022 06:24:10 GMT  
		Size: 666.7 KB (666670 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01c1ca55dba5b4d567cb01859f50449eb49d7531bcde631825000d0135927d3d`  
		Last Modified: Fri, 18 Mar 2022 06:24:16 GMT  
		Size: 26.8 MB (26842504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:139a4e0ca97e6f942624418ee448c126f2084e4a79b2946064a434a48c3e8fbc`  
		Last Modified: Fri, 18 Mar 2022 06:24:10 GMT  
		Size: 367.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v2.6.1` - linux; arm variant v6

```console
$ docker pull traefik@sha256:2ff4bf1842307e9179d2c71959da827be092f581742b9751096bb1f55df78267
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.5 MB (28492404 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4eb2cddfb6417b47e508ee363f0b5a36a19bf5981662b7280742bc56aae3684e`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 17 Mar 2022 14:32:33 GMT
ADD file:8f1611b9334907a82945fdb21e17ee41541ab95050fc199c60fca662759171a5 in / 
# Thu, 17 Mar 2022 14:32:33 GMT
CMD ["/bin/sh"]
# Thu, 17 Mar 2022 22:44:31 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 17 Mar 2022 22:44:38 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.6.1/traefik_v2.6.1_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 17 Mar 2022 22:44:39 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 17 Mar 2022 22:44:39 GMT
EXPOSE 80
# Thu, 17 Mar 2022 22:44:40 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 17 Mar 2022 22:44:40 GMT
CMD ["traefik"]
# Thu, 17 Mar 2022 22:44:41 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.6.1 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:4025825e6ef43541c3a3e1ecb0092bc1b098e792051c7e338d6da54f66b19661`  
		Last Modified: Thu, 17 Mar 2022 14:34:09 GMT  
		Size: 2.6 MB (2629364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acc61b01c9ae829babc4ec995a57d752de240cbe8e3a8660191d3d21fc589a5f`  
		Last Modified: Thu, 17 Mar 2022 22:46:57 GMT  
		Size: 672.5 KB (672470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9054064868f20b2649a2e2a9141b8f8e9f915a8c0b21859cd801f175d7e2851b`  
		Last Modified: Thu, 17 Mar 2022 22:47:14 GMT  
		Size: 25.2 MB (25190202 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1be114305d9910bdd128e32db0ec6aef6c4ef92e6857b290d41387df34aeef2b`  
		Last Modified: Thu, 17 Mar 2022 22:46:57 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v2.6.1` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:57bea358260f808ed121400b19702fd8f6ac362f394ecdac9b55ab43c95d2940
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.9 MB (27867844 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:89657e32bf0a480cfe729a2bfb2ff094c143fab533f470e63d8c9b9faf123308`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 17 Mar 2022 18:43:12 GMT
ADD file:611998b78638b13e78919dd4635674032ab233f9b7aae6f62beaf6634cd18b9e in / 
# Thu, 17 Mar 2022 18:43:13 GMT
CMD ["/bin/sh"]
# Thu, 17 Mar 2022 21:06:35 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 17 Mar 2022 21:06:38 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.6.1/traefik_v2.6.1_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 17 Mar 2022 21:06:39 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 17 Mar 2022 21:06:39 GMT
EXPOSE 80
# Thu, 17 Mar 2022 21:06:40 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 17 Mar 2022 21:06:41 GMT
CMD ["traefik"]
# Thu, 17 Mar 2022 21:06:42 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.6.1 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:93a1719cf26168d3a85db2594d76b17ccc4b25996620bceed3c2a13eaa165325`  
		Last Modified: Thu, 17 Mar 2022 18:44:00 GMT  
		Size: 2.7 MB (2715888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d012a4d53d2ad42f0d1b24f774778f1ea2d1c67cfdd0a1611fb7652fac92fc9b`  
		Last Modified: Thu, 17 Mar 2022 21:07:51 GMT  
		Size: 668.3 KB (668255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8efd5dcd64fe25305ce09060a42d89619e8dbfb06e5be5633e1abc05d30445c5`  
		Last Modified: Thu, 17 Mar 2022 21:07:55 GMT  
		Size: 24.5 MB (24483333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1eb6f2eaa89fe53dae137bd6cd91f8ef241feeae582ecdf82d83834d8bd3733b`  
		Last Modified: Thu, 17 Mar 2022 21:07:50 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v2.6.1-windowsservercore-1809`

```console
$ docker pull traefik@sha256:b80deb28063ace6076665281bd27560fd3430b7b39f5bd15503c640defb8cf49
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2686; amd64

### `traefik:v2.6.1-windowsservercore-1809` - windows version 10.0.17763.2686; amd64

```console
$ docker pull traefik@sha256:f57bdfbb46114920642abf2d1345012ecdb600175d227e38a2e681a1ebabfbd6
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2742866391 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2bf552045eeb764b54471001b799a24b4fa37c54b3aa7dbfa24c133f83d4ffb9`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 03 Mar 2022 15:05:04 GMT
RUN Install update 1809-amd64
# Tue, 08 Mar 2022 19:31:54 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Mar 2022 18:51:55 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/traefik/traefik/releases/download/v2.6.1/traefik_v2.6.1_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Wed, 09 Mar 2022 18:51:56 GMT
EXPOSE 80
# Wed, 09 Mar 2022 18:51:57 GMT
ENTRYPOINT ["/traefik"]
# Wed, 09 Mar 2022 18:51:58 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.6.1 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:0a6173b79e25f2ebc0ed51b0ac32a6f65ca5a3bbfcbeab8b74a6c24324121dea`  
		Size: 997.1 MB (997119751 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a42bef5ec276ee3f8dd3545bf050f4ab85c8191392884f5d5ad6af6ae6e2eed2`  
		Last Modified: Tue, 08 Mar 2022 20:01:19 GMT  
		Size: 1.3 KB (1323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61d553f74a3b073844e4c127831b8beebc1b835dc85e7c94513c77cc5c92e162`  
		Last Modified: Wed, 09 Mar 2022 18:54:08 GMT  
		Size: 27.4 MB (27408215 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2ef09b6978e9dfcd8c026989ac01b7a2a1acc1d57e058284c45efdfb0f0dd8a`  
		Last Modified: Wed, 09 Mar 2022 18:53:40 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc092ecf87d8664357e1628d8189f5c4c42972eb1dbcb6081f06524b75e0d8b5`  
		Last Modified: Wed, 09 Mar 2022 18:53:40 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8eebfe3ad70b0f95c3a0f566473bf5c42bbaf14434a4298c864e34bbcdf5e33`  
		Last Modified: Wed, 09 Mar 2022 18:53:40 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:windowsservercore-1809`

```console
$ docker pull traefik@sha256:b80deb28063ace6076665281bd27560fd3430b7b39f5bd15503c640defb8cf49
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2686; amd64

### `traefik:windowsservercore-1809` - windows version 10.0.17763.2686; amd64

```console
$ docker pull traefik@sha256:f57bdfbb46114920642abf2d1345012ecdb600175d227e38a2e681a1ebabfbd6
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2742866391 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2bf552045eeb764b54471001b799a24b4fa37c54b3aa7dbfa24c133f83d4ffb9`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 03 Mar 2022 15:05:04 GMT
RUN Install update 1809-amd64
# Tue, 08 Mar 2022 19:31:54 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Mar 2022 18:51:55 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/traefik/traefik/releases/download/v2.6.1/traefik_v2.6.1_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Wed, 09 Mar 2022 18:51:56 GMT
EXPOSE 80
# Wed, 09 Mar 2022 18:51:57 GMT
ENTRYPOINT ["/traefik"]
# Wed, 09 Mar 2022 18:51:58 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.6.1 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:0a6173b79e25f2ebc0ed51b0ac32a6f65ca5a3bbfcbeab8b74a6c24324121dea`  
		Size: 997.1 MB (997119751 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a42bef5ec276ee3f8dd3545bf050f4ab85c8191392884f5d5ad6af6ae6e2eed2`  
		Last Modified: Tue, 08 Mar 2022 20:01:19 GMT  
		Size: 1.3 KB (1323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61d553f74a3b073844e4c127831b8beebc1b835dc85e7c94513c77cc5c92e162`  
		Last Modified: Wed, 09 Mar 2022 18:54:08 GMT  
		Size: 27.4 MB (27408215 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2ef09b6978e9dfcd8c026989ac01b7a2a1acc1d57e058284c45efdfb0f0dd8a`  
		Last Modified: Wed, 09 Mar 2022 18:53:40 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc092ecf87d8664357e1628d8189f5c4c42972eb1dbcb6081f06524b75e0d8b5`  
		Last Modified: Wed, 09 Mar 2022 18:53:40 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8eebfe3ad70b0f95c3a0f566473bf5c42bbaf14434a4298c864e34bbcdf5e33`  
		Last Modified: Wed, 09 Mar 2022 18:53:40 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
