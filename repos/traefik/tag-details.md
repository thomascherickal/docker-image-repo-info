<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `traefik`

-	[`traefik:2.10`](#traefik210)
-	[`traefik:2.10-windowsservercore-1809`](#traefik210-windowsservercore-1809)
-	[`traefik:2.10.7`](#traefik2107)
-	[`traefik:2.10.7-windowsservercore-1809`](#traefik2107-windowsservercore-1809)
-	[`traefik:3.0`](#traefik30)
-	[`traefik:3.0-windowsservercore-1809`](#traefik30-windowsservercore-1809)
-	[`traefik:3.0.0-beta5`](#traefik300-beta5)
-	[`traefik:3.0.0-beta5-windowsservercore-1809`](#traefik300-beta5-windowsservercore-1809)
-	[`traefik:beaufort`](#traefikbeaufort)
-	[`traefik:beaufort-windowsservercore-1809`](#traefikbeaufort-windowsservercore-1809)
-	[`traefik:latest`](#traefiklatest)
-	[`traefik:saintmarcelin`](#traefiksaintmarcelin)
-	[`traefik:saintmarcelin-windowsservercore-1809`](#traefiksaintmarcelin-windowsservercore-1809)
-	[`traefik:v2.10`](#traefikv210)
-	[`traefik:v2.10-windowsservercore-1809`](#traefikv210-windowsservercore-1809)
-	[`traefik:v2.10.7`](#traefikv2107)
-	[`traefik:v2.10.7-windowsservercore-1809`](#traefikv2107-windowsservercore-1809)
-	[`traefik:v3.0`](#traefikv30)
-	[`traefik:v3.0-windowsservercore-1809`](#traefikv30-windowsservercore-1809)
-	[`traefik:v3.0.0-beta5`](#traefikv300-beta5)
-	[`traefik:v3.0.0-beta5-windowsservercore-1809`](#traefikv300-beta5-windowsservercore-1809)
-	[`traefik:windowsservercore-1809`](#traefikwindowsservercore-1809)

## `traefik:2.10`

```console
$ docker pull traefik@sha256:c5181ddf303f1ccfd4bd6d1d9c4867b0500efb6089a0f9ccb16612438f6e934f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; s390x

### `traefik:2.10` - linux; amd64

```console
$ docker pull traefik@sha256:a98415716a91066ef5e442969887ebb3df7d80775b5bfa7b67fcaed989833d84
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.2 MB (43232645 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:64586c703ab17b91788664ba464f784acd4c8058a71f54bd26852a9e6140eff5`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 30 Nov 2023 23:22:52 GMT
ADD file:fc714080c3bcbbce7ac746a10d7b4355ffa36293a8d435d62cd5359ea8eb8364 in / 
# Thu, 30 Nov 2023 23:22:52 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 07:48:32 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 06 Dec 2023 19:48:15 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.10.7/traefik_v2.10.7_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Wed, 06 Dec 2023 19:48:16 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 06 Dec 2023 19:48:16 GMT
EXPOSE 80
# Wed, 06 Dec 2023 19:48:16 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 06 Dec 2023 19:48:16 GMT
CMD ["traefik"]
# Wed, 06 Dec 2023 19:48:16 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.10.7 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:c926b61bad3b94ae7351bafd0c184c159ebf0643b085f7ef1d47ecdc7316833c`  
		Last Modified: Thu, 30 Nov 2023 23:23:28 GMT  
		Size: 3.4 MB (3402422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9a399aa53557f9793ea869bf2e9d75a94c2432b2c8d8c7a9f940da0ebb4a8d0`  
		Last Modified: Fri, 01 Dec 2023 07:48:55 GMT  
		Size: 622.3 KB (622318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3106c23e29700a541b2b7f076be6af14e416aa36a315e95909a8f44655b2c1c6`  
		Last Modified: Wed, 06 Dec 2023 19:48:35 GMT  
		Size: 39.2 MB (39207537 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc067951b11fb09519e7620e2a9a0e84e216c660aed7a38f4f3cf004354e24e1`  
		Last Modified: Wed, 06 Dec 2023 19:48:28 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:2.10` - linux; arm variant v6

```console
$ docker pull traefik@sha256:82aec7a0d7f4ee2d6fa39b2ec4e729fcd5fc0b7ab55eb987bc79d66fc3abbb05
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.8 MB (40817977 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ad7a4e3d57c06a55f5132dcc35840b0705550dbfa3a6ee98e473877671acd539`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 30 Nov 2023 22:49:18 GMT
ADD file:dbf65487d049081dc2d39b3d99d2c64b6c89754e7e2996a46169d3512e59f32a in / 
# Thu, 30 Nov 2023 22:49:18 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 11:16:30 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 06 Dec 2023 19:49:34 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.10.7/traefik_v2.10.7_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Wed, 06 Dec 2023 19:49:34 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 06 Dec 2023 19:49:34 GMT
EXPOSE 80
# Wed, 06 Dec 2023 19:49:34 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 06 Dec 2023 19:49:35 GMT
CMD ["traefik"]
# Wed, 06 Dec 2023 19:49:35 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.10.7 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:85ae953f9e6740471d4e1440b27721679dc7a511e112eb73df467a4cde26e421`  
		Last Modified: Thu, 30 Nov 2023 22:49:40 GMT  
		Size: 3.1 MB (3146870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11cc333e699b1d6d62e16cf9f495bf1e6ecc7fd649ecb87389920df6793f0739`  
		Last Modified: Fri, 01 Dec 2023 11:16:56 GMT  
		Size: 622.7 KB (622708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4204dbb89422185322324d73ad620b6b37e65708e76befdc7c808a3ff33bdacb`  
		Last Modified: Wed, 06 Dec 2023 19:49:55 GMT  
		Size: 37.0 MB (37048032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1678da4540f9fd5354abf93fec0542e3639d54e99b21750e82108004a134094a`  
		Last Modified: Wed, 06 Dec 2023 19:49:49 GMT  
		Size: 367.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:2.10` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:1f03597e0370e10e95c948a490af4ab182e9185068e212ba6e621d43f7f73ca7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.2 MB (40214807 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cb72c2dc074ab16d1bd1a1a657d7c8baeb8265740f81fcbab3a1a0559255e922`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 30 Nov 2023 23:11:03 GMT
ADD file:d8a30995bbcd627f084912c728fda5483b6ba486de25af588a0956069d0bd7ad in / 
# Thu, 30 Nov 2023 23:11:03 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 09:31:02 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 06 Dec 2023 19:54:43 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.10.7/traefik_v2.10.7_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Wed, 06 Dec 2023 19:54:44 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 06 Dec 2023 19:54:44 GMT
EXPOSE 80
# Wed, 06 Dec 2023 19:54:44 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 06 Dec 2023 19:54:44 GMT
CMD ["traefik"]
# Wed, 06 Dec 2023 19:54:44 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.10.7 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:2c03dbb20264f09924f9eab176da44e5421e74a78b09531d3c63448a7baa7c59`  
		Last Modified: Thu, 30 Nov 2023 23:11:32 GMT  
		Size: 3.3 MB (3333033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:024ea96dbe9d8eecf209e531af8ecb6502f18063303473b3d8335b373efb8a00`  
		Last Modified: Fri, 01 Dec 2023 09:31:22 GMT  
		Size: 624.5 KB (624520 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45ca6f355517b7c96d4dc25ab437ed008b0a935537be122866a708c2805d696d`  
		Last Modified: Wed, 06 Dec 2023 19:55:02 GMT  
		Size: 36.3 MB (36256886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99c0b2a752e75ae8c19870e602af930cfc9fae869f307d23ca5d36eb2528247a`  
		Last Modified: Wed, 06 Dec 2023 19:54:58 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:2.10` - linux; s390x

```console
$ docker pull traefik@sha256:a58b6de73e9090815c8bb805c754e133f6f422f8eca41b624a5df0888cf70427
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **42.1 MB (42074693 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:41851b5c1e5d75171cf8c53ba3350760e266d0b903787f4b2990649a48609c7c`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 30 Nov 2023 22:42:08 GMT
ADD file:50d6643abf7df167a927decd69d193b980557ff73cca48dce86d57e2ff25ad45 in / 
# Thu, 30 Nov 2023 22:42:09 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 07:15:54 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 06 Dec 2023 19:43:39 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.10.7/traefik_v2.10.7_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Wed, 06 Dec 2023 19:43:46 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 06 Dec 2023 19:43:47 GMT
EXPOSE 80
# Wed, 06 Dec 2023 19:43:47 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 06 Dec 2023 19:43:48 GMT
CMD ["traefik"]
# Wed, 06 Dec 2023 19:43:48 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.10.7 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:2ea477e1c0c3db3337ee1d7c659f8c465021a65c036998ed3fa3b667d4b30153`  
		Last Modified: Thu, 30 Nov 2023 22:42:52 GMT  
		Size: 3.2 MB (3217454 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82efbc9b18f13c6e43de1b733586f19a1b70be32c1cafd608f77f7b23141186b`  
		Last Modified: Fri, 01 Dec 2023 07:16:40 GMT  
		Size: 622.8 KB (622836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23d79e9ff54bf72e763a67fc4b64f81abbe41b6854d7a90e223564c452ce7645`  
		Last Modified: Wed, 06 Dec 2023 19:44:17 GMT  
		Size: 38.2 MB (38234034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f352eba91b42f08dc4d865b23f67555a4e1f0d83fc9ce83dd0705843ff49978f`  
		Last Modified: Wed, 06 Dec 2023 19:44:08 GMT  
		Size: 369.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:2.10-windowsservercore-1809`

```console
$ docker pull traefik@sha256:997103b42ff82fc02e26323fc34626675978fcf84c34148a68a4e376fdc07223
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.5206; amd64

### `traefik:2.10-windowsservercore-1809` - windows version 10.0.17763.5206; amd64

```console
$ docker pull traefik@sha256:06f73ead67b5686b93a0b8fe093e13e419c0a5d0b419da55bf1fdfd57ea3d693
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.1 GB (2100437516 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c3a543f322817696bfe1ba7e91e9d8a1ffd40812dfa85a02964f932e791f7a65`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Mon, 04 Dec 2023 11:24:49 GMT
RUN Install update 10.0.17763.5206
# Tue, 12 Dec 2023 23:38:52 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 13 Dec 2023 05:39:33 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/traefik/traefik/releases/download/v2.10.7/traefik_v2.10.7_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Wed, 13 Dec 2023 05:39:34 GMT
EXPOSE 80
# Wed, 13 Dec 2023 05:39:35 GMT
ENTRYPOINT ["/traefik"]
# Wed, 13 Dec 2023 05:39:37 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.10.7 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e35ae5ad761bfd7e5fb48c234de8722eaa28e17e2c956816fecb417ab6259c29`  
		Last Modified: Tue, 12 Dec 2023 19:14:24 GMT  
		Size: 409.1 MB (409088642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:767e95390edb4050b2c57e1d564c9e4722c5ae776ebfb8907a539571a2609f7c`  
		Last Modified: Wed, 13 Dec 2023 00:04:16 GMT  
		Size: 1.3 KB (1331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bff8297f6fad9a7479830d3d1ea2b96f0687d0f83579d405544e13911ed987d8`  
		Last Modified: Wed, 13 Dec 2023 05:40:32 GMT  
		Size: 40.7 MB (40722910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fd9eab97690e5362be049befc774a9b7d7553a578050b9b48dfda36a0436c3b`  
		Last Modified: Wed, 13 Dec 2023 05:40:23 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd7ffc3c473c5e1dee69514c2e7db4368ef6a3039ec0e16aac676559a9f09d63`  
		Last Modified: Wed, 13 Dec 2023 05:40:23 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24eea685fcd95841874da2ede817120c73864d0ade3aa21ba06040b1f5f15ccd`  
		Last Modified: Wed, 13 Dec 2023 05:40:23 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:2.10.7`

```console
$ docker pull traefik@sha256:c5181ddf303f1ccfd4bd6d1d9c4867b0500efb6089a0f9ccb16612438f6e934f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; s390x

### `traefik:2.10.7` - linux; amd64

```console
$ docker pull traefik@sha256:a98415716a91066ef5e442969887ebb3df7d80775b5bfa7b67fcaed989833d84
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.2 MB (43232645 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:64586c703ab17b91788664ba464f784acd4c8058a71f54bd26852a9e6140eff5`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 30 Nov 2023 23:22:52 GMT
ADD file:fc714080c3bcbbce7ac746a10d7b4355ffa36293a8d435d62cd5359ea8eb8364 in / 
# Thu, 30 Nov 2023 23:22:52 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 07:48:32 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 06 Dec 2023 19:48:15 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.10.7/traefik_v2.10.7_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Wed, 06 Dec 2023 19:48:16 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 06 Dec 2023 19:48:16 GMT
EXPOSE 80
# Wed, 06 Dec 2023 19:48:16 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 06 Dec 2023 19:48:16 GMT
CMD ["traefik"]
# Wed, 06 Dec 2023 19:48:16 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.10.7 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:c926b61bad3b94ae7351bafd0c184c159ebf0643b085f7ef1d47ecdc7316833c`  
		Last Modified: Thu, 30 Nov 2023 23:23:28 GMT  
		Size: 3.4 MB (3402422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9a399aa53557f9793ea869bf2e9d75a94c2432b2c8d8c7a9f940da0ebb4a8d0`  
		Last Modified: Fri, 01 Dec 2023 07:48:55 GMT  
		Size: 622.3 KB (622318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3106c23e29700a541b2b7f076be6af14e416aa36a315e95909a8f44655b2c1c6`  
		Last Modified: Wed, 06 Dec 2023 19:48:35 GMT  
		Size: 39.2 MB (39207537 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc067951b11fb09519e7620e2a9a0e84e216c660aed7a38f4f3cf004354e24e1`  
		Last Modified: Wed, 06 Dec 2023 19:48:28 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:2.10.7` - linux; arm variant v6

```console
$ docker pull traefik@sha256:82aec7a0d7f4ee2d6fa39b2ec4e729fcd5fc0b7ab55eb987bc79d66fc3abbb05
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.8 MB (40817977 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ad7a4e3d57c06a55f5132dcc35840b0705550dbfa3a6ee98e473877671acd539`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 30 Nov 2023 22:49:18 GMT
ADD file:dbf65487d049081dc2d39b3d99d2c64b6c89754e7e2996a46169d3512e59f32a in / 
# Thu, 30 Nov 2023 22:49:18 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 11:16:30 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 06 Dec 2023 19:49:34 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.10.7/traefik_v2.10.7_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Wed, 06 Dec 2023 19:49:34 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 06 Dec 2023 19:49:34 GMT
EXPOSE 80
# Wed, 06 Dec 2023 19:49:34 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 06 Dec 2023 19:49:35 GMT
CMD ["traefik"]
# Wed, 06 Dec 2023 19:49:35 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.10.7 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:85ae953f9e6740471d4e1440b27721679dc7a511e112eb73df467a4cde26e421`  
		Last Modified: Thu, 30 Nov 2023 22:49:40 GMT  
		Size: 3.1 MB (3146870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11cc333e699b1d6d62e16cf9f495bf1e6ecc7fd649ecb87389920df6793f0739`  
		Last Modified: Fri, 01 Dec 2023 11:16:56 GMT  
		Size: 622.7 KB (622708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4204dbb89422185322324d73ad620b6b37e65708e76befdc7c808a3ff33bdacb`  
		Last Modified: Wed, 06 Dec 2023 19:49:55 GMT  
		Size: 37.0 MB (37048032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1678da4540f9fd5354abf93fec0542e3639d54e99b21750e82108004a134094a`  
		Last Modified: Wed, 06 Dec 2023 19:49:49 GMT  
		Size: 367.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:2.10.7` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:1f03597e0370e10e95c948a490af4ab182e9185068e212ba6e621d43f7f73ca7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.2 MB (40214807 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cb72c2dc074ab16d1bd1a1a657d7c8baeb8265740f81fcbab3a1a0559255e922`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 30 Nov 2023 23:11:03 GMT
ADD file:d8a30995bbcd627f084912c728fda5483b6ba486de25af588a0956069d0bd7ad in / 
# Thu, 30 Nov 2023 23:11:03 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 09:31:02 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 06 Dec 2023 19:54:43 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.10.7/traefik_v2.10.7_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Wed, 06 Dec 2023 19:54:44 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 06 Dec 2023 19:54:44 GMT
EXPOSE 80
# Wed, 06 Dec 2023 19:54:44 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 06 Dec 2023 19:54:44 GMT
CMD ["traefik"]
# Wed, 06 Dec 2023 19:54:44 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.10.7 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:2c03dbb20264f09924f9eab176da44e5421e74a78b09531d3c63448a7baa7c59`  
		Last Modified: Thu, 30 Nov 2023 23:11:32 GMT  
		Size: 3.3 MB (3333033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:024ea96dbe9d8eecf209e531af8ecb6502f18063303473b3d8335b373efb8a00`  
		Last Modified: Fri, 01 Dec 2023 09:31:22 GMT  
		Size: 624.5 KB (624520 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45ca6f355517b7c96d4dc25ab437ed008b0a935537be122866a708c2805d696d`  
		Last Modified: Wed, 06 Dec 2023 19:55:02 GMT  
		Size: 36.3 MB (36256886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99c0b2a752e75ae8c19870e602af930cfc9fae869f307d23ca5d36eb2528247a`  
		Last Modified: Wed, 06 Dec 2023 19:54:58 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:2.10.7` - linux; s390x

```console
$ docker pull traefik@sha256:a58b6de73e9090815c8bb805c754e133f6f422f8eca41b624a5df0888cf70427
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **42.1 MB (42074693 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:41851b5c1e5d75171cf8c53ba3350760e266d0b903787f4b2990649a48609c7c`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 30 Nov 2023 22:42:08 GMT
ADD file:50d6643abf7df167a927decd69d193b980557ff73cca48dce86d57e2ff25ad45 in / 
# Thu, 30 Nov 2023 22:42:09 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 07:15:54 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 06 Dec 2023 19:43:39 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.10.7/traefik_v2.10.7_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Wed, 06 Dec 2023 19:43:46 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 06 Dec 2023 19:43:47 GMT
EXPOSE 80
# Wed, 06 Dec 2023 19:43:47 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 06 Dec 2023 19:43:48 GMT
CMD ["traefik"]
# Wed, 06 Dec 2023 19:43:48 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.10.7 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:2ea477e1c0c3db3337ee1d7c659f8c465021a65c036998ed3fa3b667d4b30153`  
		Last Modified: Thu, 30 Nov 2023 22:42:52 GMT  
		Size: 3.2 MB (3217454 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82efbc9b18f13c6e43de1b733586f19a1b70be32c1cafd608f77f7b23141186b`  
		Last Modified: Fri, 01 Dec 2023 07:16:40 GMT  
		Size: 622.8 KB (622836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23d79e9ff54bf72e763a67fc4b64f81abbe41b6854d7a90e223564c452ce7645`  
		Last Modified: Wed, 06 Dec 2023 19:44:17 GMT  
		Size: 38.2 MB (38234034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f352eba91b42f08dc4d865b23f67555a4e1f0d83fc9ce83dd0705843ff49978f`  
		Last Modified: Wed, 06 Dec 2023 19:44:08 GMT  
		Size: 369.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:2.10.7-windowsservercore-1809`

```console
$ docker pull traefik@sha256:997103b42ff82fc02e26323fc34626675978fcf84c34148a68a4e376fdc07223
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.5206; amd64

### `traefik:2.10.7-windowsservercore-1809` - windows version 10.0.17763.5206; amd64

```console
$ docker pull traefik@sha256:06f73ead67b5686b93a0b8fe093e13e419c0a5d0b419da55bf1fdfd57ea3d693
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.1 GB (2100437516 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c3a543f322817696bfe1ba7e91e9d8a1ffd40812dfa85a02964f932e791f7a65`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Mon, 04 Dec 2023 11:24:49 GMT
RUN Install update 10.0.17763.5206
# Tue, 12 Dec 2023 23:38:52 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 13 Dec 2023 05:39:33 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/traefik/traefik/releases/download/v2.10.7/traefik_v2.10.7_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Wed, 13 Dec 2023 05:39:34 GMT
EXPOSE 80
# Wed, 13 Dec 2023 05:39:35 GMT
ENTRYPOINT ["/traefik"]
# Wed, 13 Dec 2023 05:39:37 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.10.7 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e35ae5ad761bfd7e5fb48c234de8722eaa28e17e2c956816fecb417ab6259c29`  
		Last Modified: Tue, 12 Dec 2023 19:14:24 GMT  
		Size: 409.1 MB (409088642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:767e95390edb4050b2c57e1d564c9e4722c5ae776ebfb8907a539571a2609f7c`  
		Last Modified: Wed, 13 Dec 2023 00:04:16 GMT  
		Size: 1.3 KB (1331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bff8297f6fad9a7479830d3d1ea2b96f0687d0f83579d405544e13911ed987d8`  
		Last Modified: Wed, 13 Dec 2023 05:40:32 GMT  
		Size: 40.7 MB (40722910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fd9eab97690e5362be049befc774a9b7d7553a578050b9b48dfda36a0436c3b`  
		Last Modified: Wed, 13 Dec 2023 05:40:23 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd7ffc3c473c5e1dee69514c2e7db4368ef6a3039ec0e16aac676559a9f09d63`  
		Last Modified: Wed, 13 Dec 2023 05:40:23 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24eea685fcd95841874da2ede817120c73864d0ade3aa21ba06040b1f5f15ccd`  
		Last Modified: Wed, 13 Dec 2023 05:40:23 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:3.0`

```console
$ docker pull traefik@sha256:ce055b97e7ddce1d9ad860b2c91758a352e19a08bb45d468ea4e7d41c59c017b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; s390x

### `traefik:3.0` - linux; amd64

```console
$ docker pull traefik@sha256:81083ca7e8b7cbb14c1b5834939d30ed44d07c603206536107b59fe5ce43354a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.3 MB (44345178 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3e86938ccd95920c271a708dc45abac8b7539d753100e665b6368650e9c7d387`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 30 Nov 2023 23:22:52 GMT
ADD file:fc714080c3bcbbce7ac746a10d7b4355ffa36293a8d435d62cd5359ea8eb8364 in / 
# Thu, 30 Nov 2023 23:22:52 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 07:48:32 GMT
RUN apk --no-cache add ca-certificates tzdata
# Fri, 01 Dec 2023 07:48:35 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v3.0.0-beta5/traefik_v3.0.0-beta5_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Fri, 01 Dec 2023 07:48:36 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Fri, 01 Dec 2023 07:48:36 GMT
EXPOSE 80
# Fri, 01 Dec 2023 07:48:36 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 01 Dec 2023 07:48:36 GMT
CMD ["traefik"]
# Fri, 01 Dec 2023 07:48:36 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v3.0.0-beta5 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:c926b61bad3b94ae7351bafd0c184c159ebf0643b085f7ef1d47ecdc7316833c`  
		Last Modified: Thu, 30 Nov 2023 23:23:28 GMT  
		Size: 3.4 MB (3402422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9a399aa53557f9793ea869bf2e9d75a94c2432b2c8d8c7a9f940da0ebb4a8d0`  
		Last Modified: Fri, 01 Dec 2023 07:48:55 GMT  
		Size: 622.3 KB (622318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d62260bbee40a0f38e26c4a29db64d721bc6e670abf702ccb1db26080ef3bf40`  
		Last Modified: Fri, 01 Dec 2023 07:49:00 GMT  
		Size: 40.3 MB (40320070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:914f5bd0bae1362ae6d98a35e8f3ba805b14d8b77fca148dde78dd8065aff5cc`  
		Last Modified: Fri, 01 Dec 2023 07:48:54 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:3.0` - linux; arm variant v6

```console
$ docker pull traefik@sha256:835cf31f190d3166b76fdb66c3c64f983b7322d3910568fdc7f1dba2edc99872
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.9 MB (41866984 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:923a9205fa07d41aaa539515b30c47db529c0d52bc260e215f431d32878055d4`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 30 Nov 2023 22:49:18 GMT
ADD file:dbf65487d049081dc2d39b3d99d2c64b6c89754e7e2996a46169d3512e59f32a in / 
# Thu, 30 Nov 2023 22:49:18 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 11:16:30 GMT
RUN apk --no-cache add ca-certificates tzdata
# Fri, 01 Dec 2023 11:16:36 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v3.0.0-beta5/traefik_v3.0.0-beta5_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Fri, 01 Dec 2023 11:16:36 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Fri, 01 Dec 2023 11:16:37 GMT
EXPOSE 80
# Fri, 01 Dec 2023 11:16:37 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 01 Dec 2023 11:16:37 GMT
CMD ["traefik"]
# Fri, 01 Dec 2023 11:16:37 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v3.0.0-beta5 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:85ae953f9e6740471d4e1440b27721679dc7a511e112eb73df467a4cde26e421`  
		Last Modified: Thu, 30 Nov 2023 22:49:40 GMT  
		Size: 3.1 MB (3146870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11cc333e699b1d6d62e16cf9f495bf1e6ecc7fd649ecb87389920df6793f0739`  
		Last Modified: Fri, 01 Dec 2023 11:16:56 GMT  
		Size: 622.7 KB (622708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc62d7aab18b0798e498306604d7723cf7f2cc5ae7499104c1eef861a086fd8d`  
		Last Modified: Fri, 01 Dec 2023 11:17:03 GMT  
		Size: 38.1 MB (38097038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ccce271aac024dc8b686f07a9bf5fec98ade00307e95b5b59a380775d29c7c3`  
		Last Modified: Fri, 01 Dec 2023 11:16:55 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:3.0` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:b6e7d584d987d2e26469097dfc91a8fa9f6adc4a1e71dd23a32217da3079344c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.3 MB (41268469 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6b4562434ac10018a86a131b3359ff872b1f9466cc9d5e16128f9b370f5ae039`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 30 Nov 2023 23:11:03 GMT
ADD file:d8a30995bbcd627f084912c728fda5483b6ba486de25af588a0956069d0bd7ad in / 
# Thu, 30 Nov 2023 23:11:03 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 09:31:02 GMT
RUN apk --no-cache add ca-certificates tzdata
# Fri, 01 Dec 2023 09:31:05 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v3.0.0-beta5/traefik_v3.0.0-beta5_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Fri, 01 Dec 2023 09:31:05 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Fri, 01 Dec 2023 09:31:05 GMT
EXPOSE 80
# Fri, 01 Dec 2023 09:31:06 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 01 Dec 2023 09:31:06 GMT
CMD ["traefik"]
# Fri, 01 Dec 2023 09:31:06 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v3.0.0-beta5 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:2c03dbb20264f09924f9eab176da44e5421e74a78b09531d3c63448a7baa7c59`  
		Last Modified: Thu, 30 Nov 2023 23:11:32 GMT  
		Size: 3.3 MB (3333033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:024ea96dbe9d8eecf209e531af8ecb6502f18063303473b3d8335b373efb8a00`  
		Last Modified: Fri, 01 Dec 2023 09:31:22 GMT  
		Size: 624.5 KB (624520 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:249cd436579a71f7b4135759cb7d63f65075a6c972c268fa802a76168f800efb`  
		Last Modified: Fri, 01 Dec 2023 09:31:26 GMT  
		Size: 37.3 MB (37310548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c392c89d42e973c6b26865d1ab85577dee3782a32e5dd99618305b2cb34e5519`  
		Last Modified: Fri, 01 Dec 2023 09:31:21 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:3.0` - linux; s390x

```console
$ docker pull traefik@sha256:6a9617e4af1dcd3756b867f5a0a80ef144157d1ca247e7bcdcccb0de3491d817
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.1 MB (43096564 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:95aada75904bde1d08d556aeb2d95b9febe6e1bf9bb053d4a20c7016ef5b753d`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 30 Nov 2023 22:42:08 GMT
ADD file:50d6643abf7df167a927decd69d193b980557ff73cca48dce86d57e2ff25ad45 in / 
# Thu, 30 Nov 2023 22:42:09 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 07:15:54 GMT
RUN apk --no-cache add ca-certificates tzdata
# Fri, 01 Dec 2023 07:16:00 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v3.0.0-beta5/traefik_v3.0.0-beta5_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Fri, 01 Dec 2023 07:16:04 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Fri, 01 Dec 2023 07:16:05 GMT
EXPOSE 80
# Fri, 01 Dec 2023 07:16:05 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 01 Dec 2023 07:16:05 GMT
CMD ["traefik"]
# Fri, 01 Dec 2023 07:16:05 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v3.0.0-beta5 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:2ea477e1c0c3db3337ee1d7c659f8c465021a65c036998ed3fa3b667d4b30153`  
		Last Modified: Thu, 30 Nov 2023 22:42:52 GMT  
		Size: 3.2 MB (3217454 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82efbc9b18f13c6e43de1b733586f19a1b70be32c1cafd608f77f7b23141186b`  
		Last Modified: Fri, 01 Dec 2023 07:16:40 GMT  
		Size: 622.8 KB (622836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:468d88f1731dd43e26dd4cd67ca7706cac23e69784c09d6a3c756990491266b2`  
		Last Modified: Fri, 01 Dec 2023 07:16:47 GMT  
		Size: 39.3 MB (39255906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4966766b6d36ef16ab755867f8f4240384b5df5f3699a20bc921ae2f38bea544`  
		Last Modified: Fri, 01 Dec 2023 07:16:40 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:3.0-windowsservercore-1809`

```console
$ docker pull traefik@sha256:0f412e66210777c883a54e671f60c95159b94d5b48596212dbbf46ed7d0ad155
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.5206; amd64

### `traefik:3.0-windowsservercore-1809` - windows version 10.0.17763.5206; amd64

```console
$ docker pull traefik@sha256:b0d1ace70fadf4ab2b19b1dff9e3bf079bc39a5e1e4f82b0990f8118ef7c2fbc
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.1 GB (2101540237 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5d31b5dd9bb9f459a762c01fa0bfebfd9988aec4cfc2dc4ae89f67621e26dd87`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Mon, 04 Dec 2023 11:24:49 GMT
RUN Install update 10.0.17763.5206
# Tue, 12 Dec 2023 23:38:52 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 13 Dec 2023 05:38:12 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/traefik/traefik/releases/download/v3.0.0-beta5/traefik_v3.0.0-beta5_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Wed, 13 Dec 2023 05:38:13 GMT
EXPOSE 80
# Wed, 13 Dec 2023 05:38:14 GMT
ENTRYPOINT ["/traefik"]
# Wed, 13 Dec 2023 05:38:14 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v3.0.0-beta5 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e35ae5ad761bfd7e5fb48c234de8722eaa28e17e2c956816fecb417ab6259c29`  
		Last Modified: Tue, 12 Dec 2023 19:14:24 GMT  
		Size: 409.1 MB (409088642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:767e95390edb4050b2c57e1d564c9e4722c5ae776ebfb8907a539571a2609f7c`  
		Last Modified: Wed, 13 Dec 2023 00:04:16 GMT  
		Size: 1.3 KB (1331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:deb6a249618abc946bb07da6a95961688fcff9fc27ba6028587dbc3b8e351040`  
		Last Modified: Wed, 13 Dec 2023 05:40:09 GMT  
		Size: 41.8 MB (41825635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4242fed3cdc37df02c943b51816721ed2f17d5e7910ee80c7a45e1aa8ba1515c`  
		Last Modified: Wed, 13 Dec 2023 05:39:59 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97ad766c58568f8acc07437c5a77230c7e2ce584a555d36af2efaccb45c29bb4`  
		Last Modified: Wed, 13 Dec 2023 05:39:59 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ec2c2c191a4791893dde01c1e4d8ecf7150791ff338a8c45fb741c5494915ef`  
		Last Modified: Wed, 13 Dec 2023 05:39:59 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:3.0.0-beta5`

```console
$ docker pull traefik@sha256:ce055b97e7ddce1d9ad860b2c91758a352e19a08bb45d468ea4e7d41c59c017b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; s390x

### `traefik:3.0.0-beta5` - linux; amd64

```console
$ docker pull traefik@sha256:81083ca7e8b7cbb14c1b5834939d30ed44d07c603206536107b59fe5ce43354a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.3 MB (44345178 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3e86938ccd95920c271a708dc45abac8b7539d753100e665b6368650e9c7d387`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 30 Nov 2023 23:22:52 GMT
ADD file:fc714080c3bcbbce7ac746a10d7b4355ffa36293a8d435d62cd5359ea8eb8364 in / 
# Thu, 30 Nov 2023 23:22:52 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 07:48:32 GMT
RUN apk --no-cache add ca-certificates tzdata
# Fri, 01 Dec 2023 07:48:35 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v3.0.0-beta5/traefik_v3.0.0-beta5_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Fri, 01 Dec 2023 07:48:36 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Fri, 01 Dec 2023 07:48:36 GMT
EXPOSE 80
# Fri, 01 Dec 2023 07:48:36 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 01 Dec 2023 07:48:36 GMT
CMD ["traefik"]
# Fri, 01 Dec 2023 07:48:36 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v3.0.0-beta5 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:c926b61bad3b94ae7351bafd0c184c159ebf0643b085f7ef1d47ecdc7316833c`  
		Last Modified: Thu, 30 Nov 2023 23:23:28 GMT  
		Size: 3.4 MB (3402422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9a399aa53557f9793ea869bf2e9d75a94c2432b2c8d8c7a9f940da0ebb4a8d0`  
		Last Modified: Fri, 01 Dec 2023 07:48:55 GMT  
		Size: 622.3 KB (622318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d62260bbee40a0f38e26c4a29db64d721bc6e670abf702ccb1db26080ef3bf40`  
		Last Modified: Fri, 01 Dec 2023 07:49:00 GMT  
		Size: 40.3 MB (40320070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:914f5bd0bae1362ae6d98a35e8f3ba805b14d8b77fca148dde78dd8065aff5cc`  
		Last Modified: Fri, 01 Dec 2023 07:48:54 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:3.0.0-beta5` - linux; arm variant v6

```console
$ docker pull traefik@sha256:835cf31f190d3166b76fdb66c3c64f983b7322d3910568fdc7f1dba2edc99872
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.9 MB (41866984 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:923a9205fa07d41aaa539515b30c47db529c0d52bc260e215f431d32878055d4`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 30 Nov 2023 22:49:18 GMT
ADD file:dbf65487d049081dc2d39b3d99d2c64b6c89754e7e2996a46169d3512e59f32a in / 
# Thu, 30 Nov 2023 22:49:18 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 11:16:30 GMT
RUN apk --no-cache add ca-certificates tzdata
# Fri, 01 Dec 2023 11:16:36 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v3.0.0-beta5/traefik_v3.0.0-beta5_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Fri, 01 Dec 2023 11:16:36 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Fri, 01 Dec 2023 11:16:37 GMT
EXPOSE 80
# Fri, 01 Dec 2023 11:16:37 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 01 Dec 2023 11:16:37 GMT
CMD ["traefik"]
# Fri, 01 Dec 2023 11:16:37 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v3.0.0-beta5 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:85ae953f9e6740471d4e1440b27721679dc7a511e112eb73df467a4cde26e421`  
		Last Modified: Thu, 30 Nov 2023 22:49:40 GMT  
		Size: 3.1 MB (3146870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11cc333e699b1d6d62e16cf9f495bf1e6ecc7fd649ecb87389920df6793f0739`  
		Last Modified: Fri, 01 Dec 2023 11:16:56 GMT  
		Size: 622.7 KB (622708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc62d7aab18b0798e498306604d7723cf7f2cc5ae7499104c1eef861a086fd8d`  
		Last Modified: Fri, 01 Dec 2023 11:17:03 GMT  
		Size: 38.1 MB (38097038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ccce271aac024dc8b686f07a9bf5fec98ade00307e95b5b59a380775d29c7c3`  
		Last Modified: Fri, 01 Dec 2023 11:16:55 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:3.0.0-beta5` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:b6e7d584d987d2e26469097dfc91a8fa9f6adc4a1e71dd23a32217da3079344c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.3 MB (41268469 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6b4562434ac10018a86a131b3359ff872b1f9466cc9d5e16128f9b370f5ae039`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 30 Nov 2023 23:11:03 GMT
ADD file:d8a30995bbcd627f084912c728fda5483b6ba486de25af588a0956069d0bd7ad in / 
# Thu, 30 Nov 2023 23:11:03 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 09:31:02 GMT
RUN apk --no-cache add ca-certificates tzdata
# Fri, 01 Dec 2023 09:31:05 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v3.0.0-beta5/traefik_v3.0.0-beta5_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Fri, 01 Dec 2023 09:31:05 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Fri, 01 Dec 2023 09:31:05 GMT
EXPOSE 80
# Fri, 01 Dec 2023 09:31:06 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 01 Dec 2023 09:31:06 GMT
CMD ["traefik"]
# Fri, 01 Dec 2023 09:31:06 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v3.0.0-beta5 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:2c03dbb20264f09924f9eab176da44e5421e74a78b09531d3c63448a7baa7c59`  
		Last Modified: Thu, 30 Nov 2023 23:11:32 GMT  
		Size: 3.3 MB (3333033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:024ea96dbe9d8eecf209e531af8ecb6502f18063303473b3d8335b373efb8a00`  
		Last Modified: Fri, 01 Dec 2023 09:31:22 GMT  
		Size: 624.5 KB (624520 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:249cd436579a71f7b4135759cb7d63f65075a6c972c268fa802a76168f800efb`  
		Last Modified: Fri, 01 Dec 2023 09:31:26 GMT  
		Size: 37.3 MB (37310548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c392c89d42e973c6b26865d1ab85577dee3782a32e5dd99618305b2cb34e5519`  
		Last Modified: Fri, 01 Dec 2023 09:31:21 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:3.0.0-beta5` - linux; s390x

```console
$ docker pull traefik@sha256:6a9617e4af1dcd3756b867f5a0a80ef144157d1ca247e7bcdcccb0de3491d817
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.1 MB (43096564 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:95aada75904bde1d08d556aeb2d95b9febe6e1bf9bb053d4a20c7016ef5b753d`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 30 Nov 2023 22:42:08 GMT
ADD file:50d6643abf7df167a927decd69d193b980557ff73cca48dce86d57e2ff25ad45 in / 
# Thu, 30 Nov 2023 22:42:09 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 07:15:54 GMT
RUN apk --no-cache add ca-certificates tzdata
# Fri, 01 Dec 2023 07:16:00 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v3.0.0-beta5/traefik_v3.0.0-beta5_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Fri, 01 Dec 2023 07:16:04 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Fri, 01 Dec 2023 07:16:05 GMT
EXPOSE 80
# Fri, 01 Dec 2023 07:16:05 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 01 Dec 2023 07:16:05 GMT
CMD ["traefik"]
# Fri, 01 Dec 2023 07:16:05 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v3.0.0-beta5 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:2ea477e1c0c3db3337ee1d7c659f8c465021a65c036998ed3fa3b667d4b30153`  
		Last Modified: Thu, 30 Nov 2023 22:42:52 GMT  
		Size: 3.2 MB (3217454 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82efbc9b18f13c6e43de1b733586f19a1b70be32c1cafd608f77f7b23141186b`  
		Last Modified: Fri, 01 Dec 2023 07:16:40 GMT  
		Size: 622.8 KB (622836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:468d88f1731dd43e26dd4cd67ca7706cac23e69784c09d6a3c756990491266b2`  
		Last Modified: Fri, 01 Dec 2023 07:16:47 GMT  
		Size: 39.3 MB (39255906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4966766b6d36ef16ab755867f8f4240384b5df5f3699a20bc921ae2f38bea544`  
		Last Modified: Fri, 01 Dec 2023 07:16:40 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:3.0.0-beta5-windowsservercore-1809`

```console
$ docker pull traefik@sha256:0f412e66210777c883a54e671f60c95159b94d5b48596212dbbf46ed7d0ad155
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.5206; amd64

### `traefik:3.0.0-beta5-windowsservercore-1809` - windows version 10.0.17763.5206; amd64

```console
$ docker pull traefik@sha256:b0d1ace70fadf4ab2b19b1dff9e3bf079bc39a5e1e4f82b0990f8118ef7c2fbc
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.1 GB (2101540237 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5d31b5dd9bb9f459a762c01fa0bfebfd9988aec4cfc2dc4ae89f67621e26dd87`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Mon, 04 Dec 2023 11:24:49 GMT
RUN Install update 10.0.17763.5206
# Tue, 12 Dec 2023 23:38:52 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 13 Dec 2023 05:38:12 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/traefik/traefik/releases/download/v3.0.0-beta5/traefik_v3.0.0-beta5_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Wed, 13 Dec 2023 05:38:13 GMT
EXPOSE 80
# Wed, 13 Dec 2023 05:38:14 GMT
ENTRYPOINT ["/traefik"]
# Wed, 13 Dec 2023 05:38:14 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v3.0.0-beta5 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e35ae5ad761bfd7e5fb48c234de8722eaa28e17e2c956816fecb417ab6259c29`  
		Last Modified: Tue, 12 Dec 2023 19:14:24 GMT  
		Size: 409.1 MB (409088642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:767e95390edb4050b2c57e1d564c9e4722c5ae776ebfb8907a539571a2609f7c`  
		Last Modified: Wed, 13 Dec 2023 00:04:16 GMT  
		Size: 1.3 KB (1331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:deb6a249618abc946bb07da6a95961688fcff9fc27ba6028587dbc3b8e351040`  
		Last Modified: Wed, 13 Dec 2023 05:40:09 GMT  
		Size: 41.8 MB (41825635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4242fed3cdc37df02c943b51816721ed2f17d5e7910ee80c7a45e1aa8ba1515c`  
		Last Modified: Wed, 13 Dec 2023 05:39:59 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97ad766c58568f8acc07437c5a77230c7e2ce584a555d36af2efaccb45c29bb4`  
		Last Modified: Wed, 13 Dec 2023 05:39:59 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ec2c2c191a4791893dde01c1e4d8ecf7150791ff338a8c45fb741c5494915ef`  
		Last Modified: Wed, 13 Dec 2023 05:39:59 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:beaufort`

```console
$ docker pull traefik@sha256:ce055b97e7ddce1d9ad860b2c91758a352e19a08bb45d468ea4e7d41c59c017b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; s390x

### `traefik:beaufort` - linux; amd64

```console
$ docker pull traefik@sha256:81083ca7e8b7cbb14c1b5834939d30ed44d07c603206536107b59fe5ce43354a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.3 MB (44345178 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3e86938ccd95920c271a708dc45abac8b7539d753100e665b6368650e9c7d387`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 30 Nov 2023 23:22:52 GMT
ADD file:fc714080c3bcbbce7ac746a10d7b4355ffa36293a8d435d62cd5359ea8eb8364 in / 
# Thu, 30 Nov 2023 23:22:52 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 07:48:32 GMT
RUN apk --no-cache add ca-certificates tzdata
# Fri, 01 Dec 2023 07:48:35 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v3.0.0-beta5/traefik_v3.0.0-beta5_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Fri, 01 Dec 2023 07:48:36 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Fri, 01 Dec 2023 07:48:36 GMT
EXPOSE 80
# Fri, 01 Dec 2023 07:48:36 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 01 Dec 2023 07:48:36 GMT
CMD ["traefik"]
# Fri, 01 Dec 2023 07:48:36 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v3.0.0-beta5 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:c926b61bad3b94ae7351bafd0c184c159ebf0643b085f7ef1d47ecdc7316833c`  
		Last Modified: Thu, 30 Nov 2023 23:23:28 GMT  
		Size: 3.4 MB (3402422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9a399aa53557f9793ea869bf2e9d75a94c2432b2c8d8c7a9f940da0ebb4a8d0`  
		Last Modified: Fri, 01 Dec 2023 07:48:55 GMT  
		Size: 622.3 KB (622318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d62260bbee40a0f38e26c4a29db64d721bc6e670abf702ccb1db26080ef3bf40`  
		Last Modified: Fri, 01 Dec 2023 07:49:00 GMT  
		Size: 40.3 MB (40320070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:914f5bd0bae1362ae6d98a35e8f3ba805b14d8b77fca148dde78dd8065aff5cc`  
		Last Modified: Fri, 01 Dec 2023 07:48:54 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:beaufort` - linux; arm variant v6

```console
$ docker pull traefik@sha256:835cf31f190d3166b76fdb66c3c64f983b7322d3910568fdc7f1dba2edc99872
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.9 MB (41866984 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:923a9205fa07d41aaa539515b30c47db529c0d52bc260e215f431d32878055d4`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 30 Nov 2023 22:49:18 GMT
ADD file:dbf65487d049081dc2d39b3d99d2c64b6c89754e7e2996a46169d3512e59f32a in / 
# Thu, 30 Nov 2023 22:49:18 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 11:16:30 GMT
RUN apk --no-cache add ca-certificates tzdata
# Fri, 01 Dec 2023 11:16:36 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v3.0.0-beta5/traefik_v3.0.0-beta5_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Fri, 01 Dec 2023 11:16:36 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Fri, 01 Dec 2023 11:16:37 GMT
EXPOSE 80
# Fri, 01 Dec 2023 11:16:37 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 01 Dec 2023 11:16:37 GMT
CMD ["traefik"]
# Fri, 01 Dec 2023 11:16:37 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v3.0.0-beta5 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:85ae953f9e6740471d4e1440b27721679dc7a511e112eb73df467a4cde26e421`  
		Last Modified: Thu, 30 Nov 2023 22:49:40 GMT  
		Size: 3.1 MB (3146870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11cc333e699b1d6d62e16cf9f495bf1e6ecc7fd649ecb87389920df6793f0739`  
		Last Modified: Fri, 01 Dec 2023 11:16:56 GMT  
		Size: 622.7 KB (622708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc62d7aab18b0798e498306604d7723cf7f2cc5ae7499104c1eef861a086fd8d`  
		Last Modified: Fri, 01 Dec 2023 11:17:03 GMT  
		Size: 38.1 MB (38097038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ccce271aac024dc8b686f07a9bf5fec98ade00307e95b5b59a380775d29c7c3`  
		Last Modified: Fri, 01 Dec 2023 11:16:55 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:beaufort` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:b6e7d584d987d2e26469097dfc91a8fa9f6adc4a1e71dd23a32217da3079344c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.3 MB (41268469 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6b4562434ac10018a86a131b3359ff872b1f9466cc9d5e16128f9b370f5ae039`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 30 Nov 2023 23:11:03 GMT
ADD file:d8a30995bbcd627f084912c728fda5483b6ba486de25af588a0956069d0bd7ad in / 
# Thu, 30 Nov 2023 23:11:03 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 09:31:02 GMT
RUN apk --no-cache add ca-certificates tzdata
# Fri, 01 Dec 2023 09:31:05 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v3.0.0-beta5/traefik_v3.0.0-beta5_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Fri, 01 Dec 2023 09:31:05 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Fri, 01 Dec 2023 09:31:05 GMT
EXPOSE 80
# Fri, 01 Dec 2023 09:31:06 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 01 Dec 2023 09:31:06 GMT
CMD ["traefik"]
# Fri, 01 Dec 2023 09:31:06 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v3.0.0-beta5 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:2c03dbb20264f09924f9eab176da44e5421e74a78b09531d3c63448a7baa7c59`  
		Last Modified: Thu, 30 Nov 2023 23:11:32 GMT  
		Size: 3.3 MB (3333033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:024ea96dbe9d8eecf209e531af8ecb6502f18063303473b3d8335b373efb8a00`  
		Last Modified: Fri, 01 Dec 2023 09:31:22 GMT  
		Size: 624.5 KB (624520 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:249cd436579a71f7b4135759cb7d63f65075a6c972c268fa802a76168f800efb`  
		Last Modified: Fri, 01 Dec 2023 09:31:26 GMT  
		Size: 37.3 MB (37310548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c392c89d42e973c6b26865d1ab85577dee3782a32e5dd99618305b2cb34e5519`  
		Last Modified: Fri, 01 Dec 2023 09:31:21 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:beaufort` - linux; s390x

```console
$ docker pull traefik@sha256:6a9617e4af1dcd3756b867f5a0a80ef144157d1ca247e7bcdcccb0de3491d817
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.1 MB (43096564 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:95aada75904bde1d08d556aeb2d95b9febe6e1bf9bb053d4a20c7016ef5b753d`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 30 Nov 2023 22:42:08 GMT
ADD file:50d6643abf7df167a927decd69d193b980557ff73cca48dce86d57e2ff25ad45 in / 
# Thu, 30 Nov 2023 22:42:09 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 07:15:54 GMT
RUN apk --no-cache add ca-certificates tzdata
# Fri, 01 Dec 2023 07:16:00 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v3.0.0-beta5/traefik_v3.0.0-beta5_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Fri, 01 Dec 2023 07:16:04 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Fri, 01 Dec 2023 07:16:05 GMT
EXPOSE 80
# Fri, 01 Dec 2023 07:16:05 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 01 Dec 2023 07:16:05 GMT
CMD ["traefik"]
# Fri, 01 Dec 2023 07:16:05 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v3.0.0-beta5 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:2ea477e1c0c3db3337ee1d7c659f8c465021a65c036998ed3fa3b667d4b30153`  
		Last Modified: Thu, 30 Nov 2023 22:42:52 GMT  
		Size: 3.2 MB (3217454 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82efbc9b18f13c6e43de1b733586f19a1b70be32c1cafd608f77f7b23141186b`  
		Last Modified: Fri, 01 Dec 2023 07:16:40 GMT  
		Size: 622.8 KB (622836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:468d88f1731dd43e26dd4cd67ca7706cac23e69784c09d6a3c756990491266b2`  
		Last Modified: Fri, 01 Dec 2023 07:16:47 GMT  
		Size: 39.3 MB (39255906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4966766b6d36ef16ab755867f8f4240384b5df5f3699a20bc921ae2f38bea544`  
		Last Modified: Fri, 01 Dec 2023 07:16:40 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:beaufort-windowsservercore-1809`

```console
$ docker pull traefik@sha256:0f412e66210777c883a54e671f60c95159b94d5b48596212dbbf46ed7d0ad155
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.5206; amd64

### `traefik:beaufort-windowsservercore-1809` - windows version 10.0.17763.5206; amd64

```console
$ docker pull traefik@sha256:b0d1ace70fadf4ab2b19b1dff9e3bf079bc39a5e1e4f82b0990f8118ef7c2fbc
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.1 GB (2101540237 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5d31b5dd9bb9f459a762c01fa0bfebfd9988aec4cfc2dc4ae89f67621e26dd87`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Mon, 04 Dec 2023 11:24:49 GMT
RUN Install update 10.0.17763.5206
# Tue, 12 Dec 2023 23:38:52 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 13 Dec 2023 05:38:12 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/traefik/traefik/releases/download/v3.0.0-beta5/traefik_v3.0.0-beta5_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Wed, 13 Dec 2023 05:38:13 GMT
EXPOSE 80
# Wed, 13 Dec 2023 05:38:14 GMT
ENTRYPOINT ["/traefik"]
# Wed, 13 Dec 2023 05:38:14 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v3.0.0-beta5 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e35ae5ad761bfd7e5fb48c234de8722eaa28e17e2c956816fecb417ab6259c29`  
		Last Modified: Tue, 12 Dec 2023 19:14:24 GMT  
		Size: 409.1 MB (409088642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:767e95390edb4050b2c57e1d564c9e4722c5ae776ebfb8907a539571a2609f7c`  
		Last Modified: Wed, 13 Dec 2023 00:04:16 GMT  
		Size: 1.3 KB (1331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:deb6a249618abc946bb07da6a95961688fcff9fc27ba6028587dbc3b8e351040`  
		Last Modified: Wed, 13 Dec 2023 05:40:09 GMT  
		Size: 41.8 MB (41825635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4242fed3cdc37df02c943b51816721ed2f17d5e7910ee80c7a45e1aa8ba1515c`  
		Last Modified: Wed, 13 Dec 2023 05:39:59 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97ad766c58568f8acc07437c5a77230c7e2ce584a555d36af2efaccb45c29bb4`  
		Last Modified: Wed, 13 Dec 2023 05:39:59 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ec2c2c191a4791893dde01c1e4d8ecf7150791ff338a8c45fb741c5494915ef`  
		Last Modified: Wed, 13 Dec 2023 05:39:59 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:latest`

```console
$ docker pull traefik@sha256:c5181ddf303f1ccfd4bd6d1d9c4867b0500efb6089a0f9ccb16612438f6e934f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; s390x

### `traefik:latest` - linux; amd64

```console
$ docker pull traefik@sha256:a98415716a91066ef5e442969887ebb3df7d80775b5bfa7b67fcaed989833d84
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.2 MB (43232645 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:64586c703ab17b91788664ba464f784acd4c8058a71f54bd26852a9e6140eff5`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 30 Nov 2023 23:22:52 GMT
ADD file:fc714080c3bcbbce7ac746a10d7b4355ffa36293a8d435d62cd5359ea8eb8364 in / 
# Thu, 30 Nov 2023 23:22:52 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 07:48:32 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 06 Dec 2023 19:48:15 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.10.7/traefik_v2.10.7_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Wed, 06 Dec 2023 19:48:16 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 06 Dec 2023 19:48:16 GMT
EXPOSE 80
# Wed, 06 Dec 2023 19:48:16 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 06 Dec 2023 19:48:16 GMT
CMD ["traefik"]
# Wed, 06 Dec 2023 19:48:16 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.10.7 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:c926b61bad3b94ae7351bafd0c184c159ebf0643b085f7ef1d47ecdc7316833c`  
		Last Modified: Thu, 30 Nov 2023 23:23:28 GMT  
		Size: 3.4 MB (3402422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9a399aa53557f9793ea869bf2e9d75a94c2432b2c8d8c7a9f940da0ebb4a8d0`  
		Last Modified: Fri, 01 Dec 2023 07:48:55 GMT  
		Size: 622.3 KB (622318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3106c23e29700a541b2b7f076be6af14e416aa36a315e95909a8f44655b2c1c6`  
		Last Modified: Wed, 06 Dec 2023 19:48:35 GMT  
		Size: 39.2 MB (39207537 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc067951b11fb09519e7620e2a9a0e84e216c660aed7a38f4f3cf004354e24e1`  
		Last Modified: Wed, 06 Dec 2023 19:48:28 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:latest` - linux; arm variant v6

```console
$ docker pull traefik@sha256:82aec7a0d7f4ee2d6fa39b2ec4e729fcd5fc0b7ab55eb987bc79d66fc3abbb05
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.8 MB (40817977 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ad7a4e3d57c06a55f5132dcc35840b0705550dbfa3a6ee98e473877671acd539`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 30 Nov 2023 22:49:18 GMT
ADD file:dbf65487d049081dc2d39b3d99d2c64b6c89754e7e2996a46169d3512e59f32a in / 
# Thu, 30 Nov 2023 22:49:18 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 11:16:30 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 06 Dec 2023 19:49:34 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.10.7/traefik_v2.10.7_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Wed, 06 Dec 2023 19:49:34 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 06 Dec 2023 19:49:34 GMT
EXPOSE 80
# Wed, 06 Dec 2023 19:49:34 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 06 Dec 2023 19:49:35 GMT
CMD ["traefik"]
# Wed, 06 Dec 2023 19:49:35 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.10.7 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:85ae953f9e6740471d4e1440b27721679dc7a511e112eb73df467a4cde26e421`  
		Last Modified: Thu, 30 Nov 2023 22:49:40 GMT  
		Size: 3.1 MB (3146870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11cc333e699b1d6d62e16cf9f495bf1e6ecc7fd649ecb87389920df6793f0739`  
		Last Modified: Fri, 01 Dec 2023 11:16:56 GMT  
		Size: 622.7 KB (622708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4204dbb89422185322324d73ad620b6b37e65708e76befdc7c808a3ff33bdacb`  
		Last Modified: Wed, 06 Dec 2023 19:49:55 GMT  
		Size: 37.0 MB (37048032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1678da4540f9fd5354abf93fec0542e3639d54e99b21750e82108004a134094a`  
		Last Modified: Wed, 06 Dec 2023 19:49:49 GMT  
		Size: 367.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:latest` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:1f03597e0370e10e95c948a490af4ab182e9185068e212ba6e621d43f7f73ca7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.2 MB (40214807 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cb72c2dc074ab16d1bd1a1a657d7c8baeb8265740f81fcbab3a1a0559255e922`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 30 Nov 2023 23:11:03 GMT
ADD file:d8a30995bbcd627f084912c728fda5483b6ba486de25af588a0956069d0bd7ad in / 
# Thu, 30 Nov 2023 23:11:03 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 09:31:02 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 06 Dec 2023 19:54:43 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.10.7/traefik_v2.10.7_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Wed, 06 Dec 2023 19:54:44 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 06 Dec 2023 19:54:44 GMT
EXPOSE 80
# Wed, 06 Dec 2023 19:54:44 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 06 Dec 2023 19:54:44 GMT
CMD ["traefik"]
# Wed, 06 Dec 2023 19:54:44 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.10.7 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:2c03dbb20264f09924f9eab176da44e5421e74a78b09531d3c63448a7baa7c59`  
		Last Modified: Thu, 30 Nov 2023 23:11:32 GMT  
		Size: 3.3 MB (3333033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:024ea96dbe9d8eecf209e531af8ecb6502f18063303473b3d8335b373efb8a00`  
		Last Modified: Fri, 01 Dec 2023 09:31:22 GMT  
		Size: 624.5 KB (624520 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45ca6f355517b7c96d4dc25ab437ed008b0a935537be122866a708c2805d696d`  
		Last Modified: Wed, 06 Dec 2023 19:55:02 GMT  
		Size: 36.3 MB (36256886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99c0b2a752e75ae8c19870e602af930cfc9fae869f307d23ca5d36eb2528247a`  
		Last Modified: Wed, 06 Dec 2023 19:54:58 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:latest` - linux; s390x

```console
$ docker pull traefik@sha256:a58b6de73e9090815c8bb805c754e133f6f422f8eca41b624a5df0888cf70427
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **42.1 MB (42074693 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:41851b5c1e5d75171cf8c53ba3350760e266d0b903787f4b2990649a48609c7c`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 30 Nov 2023 22:42:08 GMT
ADD file:50d6643abf7df167a927decd69d193b980557ff73cca48dce86d57e2ff25ad45 in / 
# Thu, 30 Nov 2023 22:42:09 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 07:15:54 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 06 Dec 2023 19:43:39 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.10.7/traefik_v2.10.7_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Wed, 06 Dec 2023 19:43:46 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 06 Dec 2023 19:43:47 GMT
EXPOSE 80
# Wed, 06 Dec 2023 19:43:47 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 06 Dec 2023 19:43:48 GMT
CMD ["traefik"]
# Wed, 06 Dec 2023 19:43:48 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.10.7 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:2ea477e1c0c3db3337ee1d7c659f8c465021a65c036998ed3fa3b667d4b30153`  
		Last Modified: Thu, 30 Nov 2023 22:42:52 GMT  
		Size: 3.2 MB (3217454 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82efbc9b18f13c6e43de1b733586f19a1b70be32c1cafd608f77f7b23141186b`  
		Last Modified: Fri, 01 Dec 2023 07:16:40 GMT  
		Size: 622.8 KB (622836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23d79e9ff54bf72e763a67fc4b64f81abbe41b6854d7a90e223564c452ce7645`  
		Last Modified: Wed, 06 Dec 2023 19:44:17 GMT  
		Size: 38.2 MB (38234034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f352eba91b42f08dc4d865b23f67555a4e1f0d83fc9ce83dd0705843ff49978f`  
		Last Modified: Wed, 06 Dec 2023 19:44:08 GMT  
		Size: 369.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:saintmarcelin`

```console
$ docker pull traefik@sha256:c5181ddf303f1ccfd4bd6d1d9c4867b0500efb6089a0f9ccb16612438f6e934f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; s390x

### `traefik:saintmarcelin` - linux; amd64

```console
$ docker pull traefik@sha256:a98415716a91066ef5e442969887ebb3df7d80775b5bfa7b67fcaed989833d84
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.2 MB (43232645 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:64586c703ab17b91788664ba464f784acd4c8058a71f54bd26852a9e6140eff5`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 30 Nov 2023 23:22:52 GMT
ADD file:fc714080c3bcbbce7ac746a10d7b4355ffa36293a8d435d62cd5359ea8eb8364 in / 
# Thu, 30 Nov 2023 23:22:52 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 07:48:32 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 06 Dec 2023 19:48:15 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.10.7/traefik_v2.10.7_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Wed, 06 Dec 2023 19:48:16 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 06 Dec 2023 19:48:16 GMT
EXPOSE 80
# Wed, 06 Dec 2023 19:48:16 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 06 Dec 2023 19:48:16 GMT
CMD ["traefik"]
# Wed, 06 Dec 2023 19:48:16 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.10.7 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:c926b61bad3b94ae7351bafd0c184c159ebf0643b085f7ef1d47ecdc7316833c`  
		Last Modified: Thu, 30 Nov 2023 23:23:28 GMT  
		Size: 3.4 MB (3402422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9a399aa53557f9793ea869bf2e9d75a94c2432b2c8d8c7a9f940da0ebb4a8d0`  
		Last Modified: Fri, 01 Dec 2023 07:48:55 GMT  
		Size: 622.3 KB (622318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3106c23e29700a541b2b7f076be6af14e416aa36a315e95909a8f44655b2c1c6`  
		Last Modified: Wed, 06 Dec 2023 19:48:35 GMT  
		Size: 39.2 MB (39207537 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc067951b11fb09519e7620e2a9a0e84e216c660aed7a38f4f3cf004354e24e1`  
		Last Modified: Wed, 06 Dec 2023 19:48:28 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:saintmarcelin` - linux; arm variant v6

```console
$ docker pull traefik@sha256:82aec7a0d7f4ee2d6fa39b2ec4e729fcd5fc0b7ab55eb987bc79d66fc3abbb05
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.8 MB (40817977 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ad7a4e3d57c06a55f5132dcc35840b0705550dbfa3a6ee98e473877671acd539`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 30 Nov 2023 22:49:18 GMT
ADD file:dbf65487d049081dc2d39b3d99d2c64b6c89754e7e2996a46169d3512e59f32a in / 
# Thu, 30 Nov 2023 22:49:18 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 11:16:30 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 06 Dec 2023 19:49:34 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.10.7/traefik_v2.10.7_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Wed, 06 Dec 2023 19:49:34 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 06 Dec 2023 19:49:34 GMT
EXPOSE 80
# Wed, 06 Dec 2023 19:49:34 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 06 Dec 2023 19:49:35 GMT
CMD ["traefik"]
# Wed, 06 Dec 2023 19:49:35 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.10.7 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:85ae953f9e6740471d4e1440b27721679dc7a511e112eb73df467a4cde26e421`  
		Last Modified: Thu, 30 Nov 2023 22:49:40 GMT  
		Size: 3.1 MB (3146870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11cc333e699b1d6d62e16cf9f495bf1e6ecc7fd649ecb87389920df6793f0739`  
		Last Modified: Fri, 01 Dec 2023 11:16:56 GMT  
		Size: 622.7 KB (622708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4204dbb89422185322324d73ad620b6b37e65708e76befdc7c808a3ff33bdacb`  
		Last Modified: Wed, 06 Dec 2023 19:49:55 GMT  
		Size: 37.0 MB (37048032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1678da4540f9fd5354abf93fec0542e3639d54e99b21750e82108004a134094a`  
		Last Modified: Wed, 06 Dec 2023 19:49:49 GMT  
		Size: 367.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:saintmarcelin` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:1f03597e0370e10e95c948a490af4ab182e9185068e212ba6e621d43f7f73ca7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.2 MB (40214807 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cb72c2dc074ab16d1bd1a1a657d7c8baeb8265740f81fcbab3a1a0559255e922`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 30 Nov 2023 23:11:03 GMT
ADD file:d8a30995bbcd627f084912c728fda5483b6ba486de25af588a0956069d0bd7ad in / 
# Thu, 30 Nov 2023 23:11:03 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 09:31:02 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 06 Dec 2023 19:54:43 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.10.7/traefik_v2.10.7_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Wed, 06 Dec 2023 19:54:44 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 06 Dec 2023 19:54:44 GMT
EXPOSE 80
# Wed, 06 Dec 2023 19:54:44 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 06 Dec 2023 19:54:44 GMT
CMD ["traefik"]
# Wed, 06 Dec 2023 19:54:44 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.10.7 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:2c03dbb20264f09924f9eab176da44e5421e74a78b09531d3c63448a7baa7c59`  
		Last Modified: Thu, 30 Nov 2023 23:11:32 GMT  
		Size: 3.3 MB (3333033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:024ea96dbe9d8eecf209e531af8ecb6502f18063303473b3d8335b373efb8a00`  
		Last Modified: Fri, 01 Dec 2023 09:31:22 GMT  
		Size: 624.5 KB (624520 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45ca6f355517b7c96d4dc25ab437ed008b0a935537be122866a708c2805d696d`  
		Last Modified: Wed, 06 Dec 2023 19:55:02 GMT  
		Size: 36.3 MB (36256886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99c0b2a752e75ae8c19870e602af930cfc9fae869f307d23ca5d36eb2528247a`  
		Last Modified: Wed, 06 Dec 2023 19:54:58 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:saintmarcelin` - linux; s390x

```console
$ docker pull traefik@sha256:a58b6de73e9090815c8bb805c754e133f6f422f8eca41b624a5df0888cf70427
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **42.1 MB (42074693 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:41851b5c1e5d75171cf8c53ba3350760e266d0b903787f4b2990649a48609c7c`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 30 Nov 2023 22:42:08 GMT
ADD file:50d6643abf7df167a927decd69d193b980557ff73cca48dce86d57e2ff25ad45 in / 
# Thu, 30 Nov 2023 22:42:09 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 07:15:54 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 06 Dec 2023 19:43:39 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.10.7/traefik_v2.10.7_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Wed, 06 Dec 2023 19:43:46 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 06 Dec 2023 19:43:47 GMT
EXPOSE 80
# Wed, 06 Dec 2023 19:43:47 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 06 Dec 2023 19:43:48 GMT
CMD ["traefik"]
# Wed, 06 Dec 2023 19:43:48 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.10.7 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:2ea477e1c0c3db3337ee1d7c659f8c465021a65c036998ed3fa3b667d4b30153`  
		Last Modified: Thu, 30 Nov 2023 22:42:52 GMT  
		Size: 3.2 MB (3217454 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82efbc9b18f13c6e43de1b733586f19a1b70be32c1cafd608f77f7b23141186b`  
		Last Modified: Fri, 01 Dec 2023 07:16:40 GMT  
		Size: 622.8 KB (622836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23d79e9ff54bf72e763a67fc4b64f81abbe41b6854d7a90e223564c452ce7645`  
		Last Modified: Wed, 06 Dec 2023 19:44:17 GMT  
		Size: 38.2 MB (38234034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f352eba91b42f08dc4d865b23f67555a4e1f0d83fc9ce83dd0705843ff49978f`  
		Last Modified: Wed, 06 Dec 2023 19:44:08 GMT  
		Size: 369.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:saintmarcelin-windowsservercore-1809`

```console
$ docker pull traefik@sha256:997103b42ff82fc02e26323fc34626675978fcf84c34148a68a4e376fdc07223
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.5206; amd64

### `traefik:saintmarcelin-windowsservercore-1809` - windows version 10.0.17763.5206; amd64

```console
$ docker pull traefik@sha256:06f73ead67b5686b93a0b8fe093e13e419c0a5d0b419da55bf1fdfd57ea3d693
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.1 GB (2100437516 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c3a543f322817696bfe1ba7e91e9d8a1ffd40812dfa85a02964f932e791f7a65`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Mon, 04 Dec 2023 11:24:49 GMT
RUN Install update 10.0.17763.5206
# Tue, 12 Dec 2023 23:38:52 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 13 Dec 2023 05:39:33 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/traefik/traefik/releases/download/v2.10.7/traefik_v2.10.7_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Wed, 13 Dec 2023 05:39:34 GMT
EXPOSE 80
# Wed, 13 Dec 2023 05:39:35 GMT
ENTRYPOINT ["/traefik"]
# Wed, 13 Dec 2023 05:39:37 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.10.7 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e35ae5ad761bfd7e5fb48c234de8722eaa28e17e2c956816fecb417ab6259c29`  
		Last Modified: Tue, 12 Dec 2023 19:14:24 GMT  
		Size: 409.1 MB (409088642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:767e95390edb4050b2c57e1d564c9e4722c5ae776ebfb8907a539571a2609f7c`  
		Last Modified: Wed, 13 Dec 2023 00:04:16 GMT  
		Size: 1.3 KB (1331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bff8297f6fad9a7479830d3d1ea2b96f0687d0f83579d405544e13911ed987d8`  
		Last Modified: Wed, 13 Dec 2023 05:40:32 GMT  
		Size: 40.7 MB (40722910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fd9eab97690e5362be049befc774a9b7d7553a578050b9b48dfda36a0436c3b`  
		Last Modified: Wed, 13 Dec 2023 05:40:23 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd7ffc3c473c5e1dee69514c2e7db4368ef6a3039ec0e16aac676559a9f09d63`  
		Last Modified: Wed, 13 Dec 2023 05:40:23 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24eea685fcd95841874da2ede817120c73864d0ade3aa21ba06040b1f5f15ccd`  
		Last Modified: Wed, 13 Dec 2023 05:40:23 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v2.10`

```console
$ docker pull traefik@sha256:c5181ddf303f1ccfd4bd6d1d9c4867b0500efb6089a0f9ccb16612438f6e934f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; s390x

### `traefik:v2.10` - linux; amd64

```console
$ docker pull traefik@sha256:a98415716a91066ef5e442969887ebb3df7d80775b5bfa7b67fcaed989833d84
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.2 MB (43232645 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:64586c703ab17b91788664ba464f784acd4c8058a71f54bd26852a9e6140eff5`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 30 Nov 2023 23:22:52 GMT
ADD file:fc714080c3bcbbce7ac746a10d7b4355ffa36293a8d435d62cd5359ea8eb8364 in / 
# Thu, 30 Nov 2023 23:22:52 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 07:48:32 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 06 Dec 2023 19:48:15 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.10.7/traefik_v2.10.7_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Wed, 06 Dec 2023 19:48:16 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 06 Dec 2023 19:48:16 GMT
EXPOSE 80
# Wed, 06 Dec 2023 19:48:16 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 06 Dec 2023 19:48:16 GMT
CMD ["traefik"]
# Wed, 06 Dec 2023 19:48:16 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.10.7 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:c926b61bad3b94ae7351bafd0c184c159ebf0643b085f7ef1d47ecdc7316833c`  
		Last Modified: Thu, 30 Nov 2023 23:23:28 GMT  
		Size: 3.4 MB (3402422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9a399aa53557f9793ea869bf2e9d75a94c2432b2c8d8c7a9f940da0ebb4a8d0`  
		Last Modified: Fri, 01 Dec 2023 07:48:55 GMT  
		Size: 622.3 KB (622318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3106c23e29700a541b2b7f076be6af14e416aa36a315e95909a8f44655b2c1c6`  
		Last Modified: Wed, 06 Dec 2023 19:48:35 GMT  
		Size: 39.2 MB (39207537 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc067951b11fb09519e7620e2a9a0e84e216c660aed7a38f4f3cf004354e24e1`  
		Last Modified: Wed, 06 Dec 2023 19:48:28 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v2.10` - linux; arm variant v6

```console
$ docker pull traefik@sha256:82aec7a0d7f4ee2d6fa39b2ec4e729fcd5fc0b7ab55eb987bc79d66fc3abbb05
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.8 MB (40817977 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ad7a4e3d57c06a55f5132dcc35840b0705550dbfa3a6ee98e473877671acd539`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 30 Nov 2023 22:49:18 GMT
ADD file:dbf65487d049081dc2d39b3d99d2c64b6c89754e7e2996a46169d3512e59f32a in / 
# Thu, 30 Nov 2023 22:49:18 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 11:16:30 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 06 Dec 2023 19:49:34 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.10.7/traefik_v2.10.7_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Wed, 06 Dec 2023 19:49:34 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 06 Dec 2023 19:49:34 GMT
EXPOSE 80
# Wed, 06 Dec 2023 19:49:34 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 06 Dec 2023 19:49:35 GMT
CMD ["traefik"]
# Wed, 06 Dec 2023 19:49:35 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.10.7 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:85ae953f9e6740471d4e1440b27721679dc7a511e112eb73df467a4cde26e421`  
		Last Modified: Thu, 30 Nov 2023 22:49:40 GMT  
		Size: 3.1 MB (3146870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11cc333e699b1d6d62e16cf9f495bf1e6ecc7fd649ecb87389920df6793f0739`  
		Last Modified: Fri, 01 Dec 2023 11:16:56 GMT  
		Size: 622.7 KB (622708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4204dbb89422185322324d73ad620b6b37e65708e76befdc7c808a3ff33bdacb`  
		Last Modified: Wed, 06 Dec 2023 19:49:55 GMT  
		Size: 37.0 MB (37048032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1678da4540f9fd5354abf93fec0542e3639d54e99b21750e82108004a134094a`  
		Last Modified: Wed, 06 Dec 2023 19:49:49 GMT  
		Size: 367.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v2.10` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:1f03597e0370e10e95c948a490af4ab182e9185068e212ba6e621d43f7f73ca7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.2 MB (40214807 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cb72c2dc074ab16d1bd1a1a657d7c8baeb8265740f81fcbab3a1a0559255e922`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 30 Nov 2023 23:11:03 GMT
ADD file:d8a30995bbcd627f084912c728fda5483b6ba486de25af588a0956069d0bd7ad in / 
# Thu, 30 Nov 2023 23:11:03 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 09:31:02 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 06 Dec 2023 19:54:43 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.10.7/traefik_v2.10.7_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Wed, 06 Dec 2023 19:54:44 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 06 Dec 2023 19:54:44 GMT
EXPOSE 80
# Wed, 06 Dec 2023 19:54:44 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 06 Dec 2023 19:54:44 GMT
CMD ["traefik"]
# Wed, 06 Dec 2023 19:54:44 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.10.7 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:2c03dbb20264f09924f9eab176da44e5421e74a78b09531d3c63448a7baa7c59`  
		Last Modified: Thu, 30 Nov 2023 23:11:32 GMT  
		Size: 3.3 MB (3333033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:024ea96dbe9d8eecf209e531af8ecb6502f18063303473b3d8335b373efb8a00`  
		Last Modified: Fri, 01 Dec 2023 09:31:22 GMT  
		Size: 624.5 KB (624520 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45ca6f355517b7c96d4dc25ab437ed008b0a935537be122866a708c2805d696d`  
		Last Modified: Wed, 06 Dec 2023 19:55:02 GMT  
		Size: 36.3 MB (36256886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99c0b2a752e75ae8c19870e602af930cfc9fae869f307d23ca5d36eb2528247a`  
		Last Modified: Wed, 06 Dec 2023 19:54:58 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v2.10` - linux; s390x

```console
$ docker pull traefik@sha256:a58b6de73e9090815c8bb805c754e133f6f422f8eca41b624a5df0888cf70427
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **42.1 MB (42074693 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:41851b5c1e5d75171cf8c53ba3350760e266d0b903787f4b2990649a48609c7c`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 30 Nov 2023 22:42:08 GMT
ADD file:50d6643abf7df167a927decd69d193b980557ff73cca48dce86d57e2ff25ad45 in / 
# Thu, 30 Nov 2023 22:42:09 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 07:15:54 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 06 Dec 2023 19:43:39 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.10.7/traefik_v2.10.7_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Wed, 06 Dec 2023 19:43:46 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 06 Dec 2023 19:43:47 GMT
EXPOSE 80
# Wed, 06 Dec 2023 19:43:47 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 06 Dec 2023 19:43:48 GMT
CMD ["traefik"]
# Wed, 06 Dec 2023 19:43:48 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.10.7 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:2ea477e1c0c3db3337ee1d7c659f8c465021a65c036998ed3fa3b667d4b30153`  
		Last Modified: Thu, 30 Nov 2023 22:42:52 GMT  
		Size: 3.2 MB (3217454 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82efbc9b18f13c6e43de1b733586f19a1b70be32c1cafd608f77f7b23141186b`  
		Last Modified: Fri, 01 Dec 2023 07:16:40 GMT  
		Size: 622.8 KB (622836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23d79e9ff54bf72e763a67fc4b64f81abbe41b6854d7a90e223564c452ce7645`  
		Last Modified: Wed, 06 Dec 2023 19:44:17 GMT  
		Size: 38.2 MB (38234034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f352eba91b42f08dc4d865b23f67555a4e1f0d83fc9ce83dd0705843ff49978f`  
		Last Modified: Wed, 06 Dec 2023 19:44:08 GMT  
		Size: 369.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v2.10-windowsservercore-1809`

```console
$ docker pull traefik@sha256:997103b42ff82fc02e26323fc34626675978fcf84c34148a68a4e376fdc07223
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.5206; amd64

### `traefik:v2.10-windowsservercore-1809` - windows version 10.0.17763.5206; amd64

```console
$ docker pull traefik@sha256:06f73ead67b5686b93a0b8fe093e13e419c0a5d0b419da55bf1fdfd57ea3d693
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.1 GB (2100437516 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c3a543f322817696bfe1ba7e91e9d8a1ffd40812dfa85a02964f932e791f7a65`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Mon, 04 Dec 2023 11:24:49 GMT
RUN Install update 10.0.17763.5206
# Tue, 12 Dec 2023 23:38:52 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 13 Dec 2023 05:39:33 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/traefik/traefik/releases/download/v2.10.7/traefik_v2.10.7_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Wed, 13 Dec 2023 05:39:34 GMT
EXPOSE 80
# Wed, 13 Dec 2023 05:39:35 GMT
ENTRYPOINT ["/traefik"]
# Wed, 13 Dec 2023 05:39:37 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.10.7 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e35ae5ad761bfd7e5fb48c234de8722eaa28e17e2c956816fecb417ab6259c29`  
		Last Modified: Tue, 12 Dec 2023 19:14:24 GMT  
		Size: 409.1 MB (409088642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:767e95390edb4050b2c57e1d564c9e4722c5ae776ebfb8907a539571a2609f7c`  
		Last Modified: Wed, 13 Dec 2023 00:04:16 GMT  
		Size: 1.3 KB (1331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bff8297f6fad9a7479830d3d1ea2b96f0687d0f83579d405544e13911ed987d8`  
		Last Modified: Wed, 13 Dec 2023 05:40:32 GMT  
		Size: 40.7 MB (40722910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fd9eab97690e5362be049befc774a9b7d7553a578050b9b48dfda36a0436c3b`  
		Last Modified: Wed, 13 Dec 2023 05:40:23 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd7ffc3c473c5e1dee69514c2e7db4368ef6a3039ec0e16aac676559a9f09d63`  
		Last Modified: Wed, 13 Dec 2023 05:40:23 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24eea685fcd95841874da2ede817120c73864d0ade3aa21ba06040b1f5f15ccd`  
		Last Modified: Wed, 13 Dec 2023 05:40:23 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v2.10.7`

```console
$ docker pull traefik@sha256:c5181ddf303f1ccfd4bd6d1d9c4867b0500efb6089a0f9ccb16612438f6e934f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; s390x

### `traefik:v2.10.7` - linux; amd64

```console
$ docker pull traefik@sha256:a98415716a91066ef5e442969887ebb3df7d80775b5bfa7b67fcaed989833d84
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.2 MB (43232645 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:64586c703ab17b91788664ba464f784acd4c8058a71f54bd26852a9e6140eff5`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 30 Nov 2023 23:22:52 GMT
ADD file:fc714080c3bcbbce7ac746a10d7b4355ffa36293a8d435d62cd5359ea8eb8364 in / 
# Thu, 30 Nov 2023 23:22:52 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 07:48:32 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 06 Dec 2023 19:48:15 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.10.7/traefik_v2.10.7_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Wed, 06 Dec 2023 19:48:16 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 06 Dec 2023 19:48:16 GMT
EXPOSE 80
# Wed, 06 Dec 2023 19:48:16 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 06 Dec 2023 19:48:16 GMT
CMD ["traefik"]
# Wed, 06 Dec 2023 19:48:16 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.10.7 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:c926b61bad3b94ae7351bafd0c184c159ebf0643b085f7ef1d47ecdc7316833c`  
		Last Modified: Thu, 30 Nov 2023 23:23:28 GMT  
		Size: 3.4 MB (3402422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9a399aa53557f9793ea869bf2e9d75a94c2432b2c8d8c7a9f940da0ebb4a8d0`  
		Last Modified: Fri, 01 Dec 2023 07:48:55 GMT  
		Size: 622.3 KB (622318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3106c23e29700a541b2b7f076be6af14e416aa36a315e95909a8f44655b2c1c6`  
		Last Modified: Wed, 06 Dec 2023 19:48:35 GMT  
		Size: 39.2 MB (39207537 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc067951b11fb09519e7620e2a9a0e84e216c660aed7a38f4f3cf004354e24e1`  
		Last Modified: Wed, 06 Dec 2023 19:48:28 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v2.10.7` - linux; arm variant v6

```console
$ docker pull traefik@sha256:82aec7a0d7f4ee2d6fa39b2ec4e729fcd5fc0b7ab55eb987bc79d66fc3abbb05
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.8 MB (40817977 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ad7a4e3d57c06a55f5132dcc35840b0705550dbfa3a6ee98e473877671acd539`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 30 Nov 2023 22:49:18 GMT
ADD file:dbf65487d049081dc2d39b3d99d2c64b6c89754e7e2996a46169d3512e59f32a in / 
# Thu, 30 Nov 2023 22:49:18 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 11:16:30 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 06 Dec 2023 19:49:34 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.10.7/traefik_v2.10.7_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Wed, 06 Dec 2023 19:49:34 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 06 Dec 2023 19:49:34 GMT
EXPOSE 80
# Wed, 06 Dec 2023 19:49:34 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 06 Dec 2023 19:49:35 GMT
CMD ["traefik"]
# Wed, 06 Dec 2023 19:49:35 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.10.7 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:85ae953f9e6740471d4e1440b27721679dc7a511e112eb73df467a4cde26e421`  
		Last Modified: Thu, 30 Nov 2023 22:49:40 GMT  
		Size: 3.1 MB (3146870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11cc333e699b1d6d62e16cf9f495bf1e6ecc7fd649ecb87389920df6793f0739`  
		Last Modified: Fri, 01 Dec 2023 11:16:56 GMT  
		Size: 622.7 KB (622708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4204dbb89422185322324d73ad620b6b37e65708e76befdc7c808a3ff33bdacb`  
		Last Modified: Wed, 06 Dec 2023 19:49:55 GMT  
		Size: 37.0 MB (37048032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1678da4540f9fd5354abf93fec0542e3639d54e99b21750e82108004a134094a`  
		Last Modified: Wed, 06 Dec 2023 19:49:49 GMT  
		Size: 367.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v2.10.7` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:1f03597e0370e10e95c948a490af4ab182e9185068e212ba6e621d43f7f73ca7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.2 MB (40214807 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cb72c2dc074ab16d1bd1a1a657d7c8baeb8265740f81fcbab3a1a0559255e922`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 30 Nov 2023 23:11:03 GMT
ADD file:d8a30995bbcd627f084912c728fda5483b6ba486de25af588a0956069d0bd7ad in / 
# Thu, 30 Nov 2023 23:11:03 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 09:31:02 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 06 Dec 2023 19:54:43 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.10.7/traefik_v2.10.7_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Wed, 06 Dec 2023 19:54:44 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 06 Dec 2023 19:54:44 GMT
EXPOSE 80
# Wed, 06 Dec 2023 19:54:44 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 06 Dec 2023 19:54:44 GMT
CMD ["traefik"]
# Wed, 06 Dec 2023 19:54:44 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.10.7 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:2c03dbb20264f09924f9eab176da44e5421e74a78b09531d3c63448a7baa7c59`  
		Last Modified: Thu, 30 Nov 2023 23:11:32 GMT  
		Size: 3.3 MB (3333033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:024ea96dbe9d8eecf209e531af8ecb6502f18063303473b3d8335b373efb8a00`  
		Last Modified: Fri, 01 Dec 2023 09:31:22 GMT  
		Size: 624.5 KB (624520 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45ca6f355517b7c96d4dc25ab437ed008b0a935537be122866a708c2805d696d`  
		Last Modified: Wed, 06 Dec 2023 19:55:02 GMT  
		Size: 36.3 MB (36256886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99c0b2a752e75ae8c19870e602af930cfc9fae869f307d23ca5d36eb2528247a`  
		Last Modified: Wed, 06 Dec 2023 19:54:58 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v2.10.7` - linux; s390x

```console
$ docker pull traefik@sha256:a58b6de73e9090815c8bb805c754e133f6f422f8eca41b624a5df0888cf70427
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **42.1 MB (42074693 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:41851b5c1e5d75171cf8c53ba3350760e266d0b903787f4b2990649a48609c7c`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 30 Nov 2023 22:42:08 GMT
ADD file:50d6643abf7df167a927decd69d193b980557ff73cca48dce86d57e2ff25ad45 in / 
# Thu, 30 Nov 2023 22:42:09 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 07:15:54 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 06 Dec 2023 19:43:39 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.10.7/traefik_v2.10.7_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Wed, 06 Dec 2023 19:43:46 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 06 Dec 2023 19:43:47 GMT
EXPOSE 80
# Wed, 06 Dec 2023 19:43:47 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 06 Dec 2023 19:43:48 GMT
CMD ["traefik"]
# Wed, 06 Dec 2023 19:43:48 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.10.7 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:2ea477e1c0c3db3337ee1d7c659f8c465021a65c036998ed3fa3b667d4b30153`  
		Last Modified: Thu, 30 Nov 2023 22:42:52 GMT  
		Size: 3.2 MB (3217454 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82efbc9b18f13c6e43de1b733586f19a1b70be32c1cafd608f77f7b23141186b`  
		Last Modified: Fri, 01 Dec 2023 07:16:40 GMT  
		Size: 622.8 KB (622836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23d79e9ff54bf72e763a67fc4b64f81abbe41b6854d7a90e223564c452ce7645`  
		Last Modified: Wed, 06 Dec 2023 19:44:17 GMT  
		Size: 38.2 MB (38234034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f352eba91b42f08dc4d865b23f67555a4e1f0d83fc9ce83dd0705843ff49978f`  
		Last Modified: Wed, 06 Dec 2023 19:44:08 GMT  
		Size: 369.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v2.10.7-windowsservercore-1809`

```console
$ docker pull traefik@sha256:997103b42ff82fc02e26323fc34626675978fcf84c34148a68a4e376fdc07223
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.5206; amd64

### `traefik:v2.10.7-windowsservercore-1809` - windows version 10.0.17763.5206; amd64

```console
$ docker pull traefik@sha256:06f73ead67b5686b93a0b8fe093e13e419c0a5d0b419da55bf1fdfd57ea3d693
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.1 GB (2100437516 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c3a543f322817696bfe1ba7e91e9d8a1ffd40812dfa85a02964f932e791f7a65`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Mon, 04 Dec 2023 11:24:49 GMT
RUN Install update 10.0.17763.5206
# Tue, 12 Dec 2023 23:38:52 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 13 Dec 2023 05:39:33 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/traefik/traefik/releases/download/v2.10.7/traefik_v2.10.7_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Wed, 13 Dec 2023 05:39:34 GMT
EXPOSE 80
# Wed, 13 Dec 2023 05:39:35 GMT
ENTRYPOINT ["/traefik"]
# Wed, 13 Dec 2023 05:39:37 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.10.7 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e35ae5ad761bfd7e5fb48c234de8722eaa28e17e2c956816fecb417ab6259c29`  
		Last Modified: Tue, 12 Dec 2023 19:14:24 GMT  
		Size: 409.1 MB (409088642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:767e95390edb4050b2c57e1d564c9e4722c5ae776ebfb8907a539571a2609f7c`  
		Last Modified: Wed, 13 Dec 2023 00:04:16 GMT  
		Size: 1.3 KB (1331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bff8297f6fad9a7479830d3d1ea2b96f0687d0f83579d405544e13911ed987d8`  
		Last Modified: Wed, 13 Dec 2023 05:40:32 GMT  
		Size: 40.7 MB (40722910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fd9eab97690e5362be049befc774a9b7d7553a578050b9b48dfda36a0436c3b`  
		Last Modified: Wed, 13 Dec 2023 05:40:23 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd7ffc3c473c5e1dee69514c2e7db4368ef6a3039ec0e16aac676559a9f09d63`  
		Last Modified: Wed, 13 Dec 2023 05:40:23 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24eea685fcd95841874da2ede817120c73864d0ade3aa21ba06040b1f5f15ccd`  
		Last Modified: Wed, 13 Dec 2023 05:40:23 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v3.0`

```console
$ docker pull traefik@sha256:ce055b97e7ddce1d9ad860b2c91758a352e19a08bb45d468ea4e7d41c59c017b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; s390x

### `traefik:v3.0` - linux; amd64

```console
$ docker pull traefik@sha256:81083ca7e8b7cbb14c1b5834939d30ed44d07c603206536107b59fe5ce43354a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.3 MB (44345178 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3e86938ccd95920c271a708dc45abac8b7539d753100e665b6368650e9c7d387`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 30 Nov 2023 23:22:52 GMT
ADD file:fc714080c3bcbbce7ac746a10d7b4355ffa36293a8d435d62cd5359ea8eb8364 in / 
# Thu, 30 Nov 2023 23:22:52 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 07:48:32 GMT
RUN apk --no-cache add ca-certificates tzdata
# Fri, 01 Dec 2023 07:48:35 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v3.0.0-beta5/traefik_v3.0.0-beta5_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Fri, 01 Dec 2023 07:48:36 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Fri, 01 Dec 2023 07:48:36 GMT
EXPOSE 80
# Fri, 01 Dec 2023 07:48:36 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 01 Dec 2023 07:48:36 GMT
CMD ["traefik"]
# Fri, 01 Dec 2023 07:48:36 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v3.0.0-beta5 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:c926b61bad3b94ae7351bafd0c184c159ebf0643b085f7ef1d47ecdc7316833c`  
		Last Modified: Thu, 30 Nov 2023 23:23:28 GMT  
		Size: 3.4 MB (3402422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9a399aa53557f9793ea869bf2e9d75a94c2432b2c8d8c7a9f940da0ebb4a8d0`  
		Last Modified: Fri, 01 Dec 2023 07:48:55 GMT  
		Size: 622.3 KB (622318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d62260bbee40a0f38e26c4a29db64d721bc6e670abf702ccb1db26080ef3bf40`  
		Last Modified: Fri, 01 Dec 2023 07:49:00 GMT  
		Size: 40.3 MB (40320070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:914f5bd0bae1362ae6d98a35e8f3ba805b14d8b77fca148dde78dd8065aff5cc`  
		Last Modified: Fri, 01 Dec 2023 07:48:54 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v3.0` - linux; arm variant v6

```console
$ docker pull traefik@sha256:835cf31f190d3166b76fdb66c3c64f983b7322d3910568fdc7f1dba2edc99872
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.9 MB (41866984 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:923a9205fa07d41aaa539515b30c47db529c0d52bc260e215f431d32878055d4`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 30 Nov 2023 22:49:18 GMT
ADD file:dbf65487d049081dc2d39b3d99d2c64b6c89754e7e2996a46169d3512e59f32a in / 
# Thu, 30 Nov 2023 22:49:18 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 11:16:30 GMT
RUN apk --no-cache add ca-certificates tzdata
# Fri, 01 Dec 2023 11:16:36 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v3.0.0-beta5/traefik_v3.0.0-beta5_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Fri, 01 Dec 2023 11:16:36 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Fri, 01 Dec 2023 11:16:37 GMT
EXPOSE 80
# Fri, 01 Dec 2023 11:16:37 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 01 Dec 2023 11:16:37 GMT
CMD ["traefik"]
# Fri, 01 Dec 2023 11:16:37 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v3.0.0-beta5 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:85ae953f9e6740471d4e1440b27721679dc7a511e112eb73df467a4cde26e421`  
		Last Modified: Thu, 30 Nov 2023 22:49:40 GMT  
		Size: 3.1 MB (3146870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11cc333e699b1d6d62e16cf9f495bf1e6ecc7fd649ecb87389920df6793f0739`  
		Last Modified: Fri, 01 Dec 2023 11:16:56 GMT  
		Size: 622.7 KB (622708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc62d7aab18b0798e498306604d7723cf7f2cc5ae7499104c1eef861a086fd8d`  
		Last Modified: Fri, 01 Dec 2023 11:17:03 GMT  
		Size: 38.1 MB (38097038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ccce271aac024dc8b686f07a9bf5fec98ade00307e95b5b59a380775d29c7c3`  
		Last Modified: Fri, 01 Dec 2023 11:16:55 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v3.0` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:b6e7d584d987d2e26469097dfc91a8fa9f6adc4a1e71dd23a32217da3079344c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.3 MB (41268469 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6b4562434ac10018a86a131b3359ff872b1f9466cc9d5e16128f9b370f5ae039`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 30 Nov 2023 23:11:03 GMT
ADD file:d8a30995bbcd627f084912c728fda5483b6ba486de25af588a0956069d0bd7ad in / 
# Thu, 30 Nov 2023 23:11:03 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 09:31:02 GMT
RUN apk --no-cache add ca-certificates tzdata
# Fri, 01 Dec 2023 09:31:05 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v3.0.0-beta5/traefik_v3.0.0-beta5_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Fri, 01 Dec 2023 09:31:05 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Fri, 01 Dec 2023 09:31:05 GMT
EXPOSE 80
# Fri, 01 Dec 2023 09:31:06 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 01 Dec 2023 09:31:06 GMT
CMD ["traefik"]
# Fri, 01 Dec 2023 09:31:06 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v3.0.0-beta5 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:2c03dbb20264f09924f9eab176da44e5421e74a78b09531d3c63448a7baa7c59`  
		Last Modified: Thu, 30 Nov 2023 23:11:32 GMT  
		Size: 3.3 MB (3333033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:024ea96dbe9d8eecf209e531af8ecb6502f18063303473b3d8335b373efb8a00`  
		Last Modified: Fri, 01 Dec 2023 09:31:22 GMT  
		Size: 624.5 KB (624520 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:249cd436579a71f7b4135759cb7d63f65075a6c972c268fa802a76168f800efb`  
		Last Modified: Fri, 01 Dec 2023 09:31:26 GMT  
		Size: 37.3 MB (37310548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c392c89d42e973c6b26865d1ab85577dee3782a32e5dd99618305b2cb34e5519`  
		Last Modified: Fri, 01 Dec 2023 09:31:21 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v3.0` - linux; s390x

```console
$ docker pull traefik@sha256:6a9617e4af1dcd3756b867f5a0a80ef144157d1ca247e7bcdcccb0de3491d817
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.1 MB (43096564 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:95aada75904bde1d08d556aeb2d95b9febe6e1bf9bb053d4a20c7016ef5b753d`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 30 Nov 2023 22:42:08 GMT
ADD file:50d6643abf7df167a927decd69d193b980557ff73cca48dce86d57e2ff25ad45 in / 
# Thu, 30 Nov 2023 22:42:09 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 07:15:54 GMT
RUN apk --no-cache add ca-certificates tzdata
# Fri, 01 Dec 2023 07:16:00 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v3.0.0-beta5/traefik_v3.0.0-beta5_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Fri, 01 Dec 2023 07:16:04 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Fri, 01 Dec 2023 07:16:05 GMT
EXPOSE 80
# Fri, 01 Dec 2023 07:16:05 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 01 Dec 2023 07:16:05 GMT
CMD ["traefik"]
# Fri, 01 Dec 2023 07:16:05 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v3.0.0-beta5 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:2ea477e1c0c3db3337ee1d7c659f8c465021a65c036998ed3fa3b667d4b30153`  
		Last Modified: Thu, 30 Nov 2023 22:42:52 GMT  
		Size: 3.2 MB (3217454 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82efbc9b18f13c6e43de1b733586f19a1b70be32c1cafd608f77f7b23141186b`  
		Last Modified: Fri, 01 Dec 2023 07:16:40 GMT  
		Size: 622.8 KB (622836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:468d88f1731dd43e26dd4cd67ca7706cac23e69784c09d6a3c756990491266b2`  
		Last Modified: Fri, 01 Dec 2023 07:16:47 GMT  
		Size: 39.3 MB (39255906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4966766b6d36ef16ab755867f8f4240384b5df5f3699a20bc921ae2f38bea544`  
		Last Modified: Fri, 01 Dec 2023 07:16:40 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v3.0-windowsservercore-1809`

```console
$ docker pull traefik@sha256:0f412e66210777c883a54e671f60c95159b94d5b48596212dbbf46ed7d0ad155
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.5206; amd64

### `traefik:v3.0-windowsservercore-1809` - windows version 10.0.17763.5206; amd64

```console
$ docker pull traefik@sha256:b0d1ace70fadf4ab2b19b1dff9e3bf079bc39a5e1e4f82b0990f8118ef7c2fbc
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.1 GB (2101540237 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5d31b5dd9bb9f459a762c01fa0bfebfd9988aec4cfc2dc4ae89f67621e26dd87`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Mon, 04 Dec 2023 11:24:49 GMT
RUN Install update 10.0.17763.5206
# Tue, 12 Dec 2023 23:38:52 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 13 Dec 2023 05:38:12 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/traefik/traefik/releases/download/v3.0.0-beta5/traefik_v3.0.0-beta5_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Wed, 13 Dec 2023 05:38:13 GMT
EXPOSE 80
# Wed, 13 Dec 2023 05:38:14 GMT
ENTRYPOINT ["/traefik"]
# Wed, 13 Dec 2023 05:38:14 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v3.0.0-beta5 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e35ae5ad761bfd7e5fb48c234de8722eaa28e17e2c956816fecb417ab6259c29`  
		Last Modified: Tue, 12 Dec 2023 19:14:24 GMT  
		Size: 409.1 MB (409088642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:767e95390edb4050b2c57e1d564c9e4722c5ae776ebfb8907a539571a2609f7c`  
		Last Modified: Wed, 13 Dec 2023 00:04:16 GMT  
		Size: 1.3 KB (1331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:deb6a249618abc946bb07da6a95961688fcff9fc27ba6028587dbc3b8e351040`  
		Last Modified: Wed, 13 Dec 2023 05:40:09 GMT  
		Size: 41.8 MB (41825635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4242fed3cdc37df02c943b51816721ed2f17d5e7910ee80c7a45e1aa8ba1515c`  
		Last Modified: Wed, 13 Dec 2023 05:39:59 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97ad766c58568f8acc07437c5a77230c7e2ce584a555d36af2efaccb45c29bb4`  
		Last Modified: Wed, 13 Dec 2023 05:39:59 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ec2c2c191a4791893dde01c1e4d8ecf7150791ff338a8c45fb741c5494915ef`  
		Last Modified: Wed, 13 Dec 2023 05:39:59 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v3.0.0-beta5`

```console
$ docker pull traefik@sha256:ce055b97e7ddce1d9ad860b2c91758a352e19a08bb45d468ea4e7d41c59c017b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; s390x

### `traefik:v3.0.0-beta5` - linux; amd64

```console
$ docker pull traefik@sha256:81083ca7e8b7cbb14c1b5834939d30ed44d07c603206536107b59fe5ce43354a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.3 MB (44345178 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3e86938ccd95920c271a708dc45abac8b7539d753100e665b6368650e9c7d387`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 30 Nov 2023 23:22:52 GMT
ADD file:fc714080c3bcbbce7ac746a10d7b4355ffa36293a8d435d62cd5359ea8eb8364 in / 
# Thu, 30 Nov 2023 23:22:52 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 07:48:32 GMT
RUN apk --no-cache add ca-certificates tzdata
# Fri, 01 Dec 2023 07:48:35 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v3.0.0-beta5/traefik_v3.0.0-beta5_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Fri, 01 Dec 2023 07:48:36 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Fri, 01 Dec 2023 07:48:36 GMT
EXPOSE 80
# Fri, 01 Dec 2023 07:48:36 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 01 Dec 2023 07:48:36 GMT
CMD ["traefik"]
# Fri, 01 Dec 2023 07:48:36 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v3.0.0-beta5 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:c926b61bad3b94ae7351bafd0c184c159ebf0643b085f7ef1d47ecdc7316833c`  
		Last Modified: Thu, 30 Nov 2023 23:23:28 GMT  
		Size: 3.4 MB (3402422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9a399aa53557f9793ea869bf2e9d75a94c2432b2c8d8c7a9f940da0ebb4a8d0`  
		Last Modified: Fri, 01 Dec 2023 07:48:55 GMT  
		Size: 622.3 KB (622318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d62260bbee40a0f38e26c4a29db64d721bc6e670abf702ccb1db26080ef3bf40`  
		Last Modified: Fri, 01 Dec 2023 07:49:00 GMT  
		Size: 40.3 MB (40320070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:914f5bd0bae1362ae6d98a35e8f3ba805b14d8b77fca148dde78dd8065aff5cc`  
		Last Modified: Fri, 01 Dec 2023 07:48:54 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v3.0.0-beta5` - linux; arm variant v6

```console
$ docker pull traefik@sha256:835cf31f190d3166b76fdb66c3c64f983b7322d3910568fdc7f1dba2edc99872
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.9 MB (41866984 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:923a9205fa07d41aaa539515b30c47db529c0d52bc260e215f431d32878055d4`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 30 Nov 2023 22:49:18 GMT
ADD file:dbf65487d049081dc2d39b3d99d2c64b6c89754e7e2996a46169d3512e59f32a in / 
# Thu, 30 Nov 2023 22:49:18 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 11:16:30 GMT
RUN apk --no-cache add ca-certificates tzdata
# Fri, 01 Dec 2023 11:16:36 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v3.0.0-beta5/traefik_v3.0.0-beta5_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Fri, 01 Dec 2023 11:16:36 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Fri, 01 Dec 2023 11:16:37 GMT
EXPOSE 80
# Fri, 01 Dec 2023 11:16:37 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 01 Dec 2023 11:16:37 GMT
CMD ["traefik"]
# Fri, 01 Dec 2023 11:16:37 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v3.0.0-beta5 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:85ae953f9e6740471d4e1440b27721679dc7a511e112eb73df467a4cde26e421`  
		Last Modified: Thu, 30 Nov 2023 22:49:40 GMT  
		Size: 3.1 MB (3146870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11cc333e699b1d6d62e16cf9f495bf1e6ecc7fd649ecb87389920df6793f0739`  
		Last Modified: Fri, 01 Dec 2023 11:16:56 GMT  
		Size: 622.7 KB (622708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc62d7aab18b0798e498306604d7723cf7f2cc5ae7499104c1eef861a086fd8d`  
		Last Modified: Fri, 01 Dec 2023 11:17:03 GMT  
		Size: 38.1 MB (38097038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ccce271aac024dc8b686f07a9bf5fec98ade00307e95b5b59a380775d29c7c3`  
		Last Modified: Fri, 01 Dec 2023 11:16:55 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v3.0.0-beta5` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:b6e7d584d987d2e26469097dfc91a8fa9f6adc4a1e71dd23a32217da3079344c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.3 MB (41268469 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6b4562434ac10018a86a131b3359ff872b1f9466cc9d5e16128f9b370f5ae039`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 30 Nov 2023 23:11:03 GMT
ADD file:d8a30995bbcd627f084912c728fda5483b6ba486de25af588a0956069d0bd7ad in / 
# Thu, 30 Nov 2023 23:11:03 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 09:31:02 GMT
RUN apk --no-cache add ca-certificates tzdata
# Fri, 01 Dec 2023 09:31:05 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v3.0.0-beta5/traefik_v3.0.0-beta5_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Fri, 01 Dec 2023 09:31:05 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Fri, 01 Dec 2023 09:31:05 GMT
EXPOSE 80
# Fri, 01 Dec 2023 09:31:06 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 01 Dec 2023 09:31:06 GMT
CMD ["traefik"]
# Fri, 01 Dec 2023 09:31:06 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v3.0.0-beta5 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:2c03dbb20264f09924f9eab176da44e5421e74a78b09531d3c63448a7baa7c59`  
		Last Modified: Thu, 30 Nov 2023 23:11:32 GMT  
		Size: 3.3 MB (3333033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:024ea96dbe9d8eecf209e531af8ecb6502f18063303473b3d8335b373efb8a00`  
		Last Modified: Fri, 01 Dec 2023 09:31:22 GMT  
		Size: 624.5 KB (624520 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:249cd436579a71f7b4135759cb7d63f65075a6c972c268fa802a76168f800efb`  
		Last Modified: Fri, 01 Dec 2023 09:31:26 GMT  
		Size: 37.3 MB (37310548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c392c89d42e973c6b26865d1ab85577dee3782a32e5dd99618305b2cb34e5519`  
		Last Modified: Fri, 01 Dec 2023 09:31:21 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v3.0.0-beta5` - linux; s390x

```console
$ docker pull traefik@sha256:6a9617e4af1dcd3756b867f5a0a80ef144157d1ca247e7bcdcccb0de3491d817
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.1 MB (43096564 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:95aada75904bde1d08d556aeb2d95b9febe6e1bf9bb053d4a20c7016ef5b753d`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 30 Nov 2023 22:42:08 GMT
ADD file:50d6643abf7df167a927decd69d193b980557ff73cca48dce86d57e2ff25ad45 in / 
# Thu, 30 Nov 2023 22:42:09 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 07:15:54 GMT
RUN apk --no-cache add ca-certificates tzdata
# Fri, 01 Dec 2023 07:16:00 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v3.0.0-beta5/traefik_v3.0.0-beta5_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Fri, 01 Dec 2023 07:16:04 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Fri, 01 Dec 2023 07:16:05 GMT
EXPOSE 80
# Fri, 01 Dec 2023 07:16:05 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 01 Dec 2023 07:16:05 GMT
CMD ["traefik"]
# Fri, 01 Dec 2023 07:16:05 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v3.0.0-beta5 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:2ea477e1c0c3db3337ee1d7c659f8c465021a65c036998ed3fa3b667d4b30153`  
		Last Modified: Thu, 30 Nov 2023 22:42:52 GMT  
		Size: 3.2 MB (3217454 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82efbc9b18f13c6e43de1b733586f19a1b70be32c1cafd608f77f7b23141186b`  
		Last Modified: Fri, 01 Dec 2023 07:16:40 GMT  
		Size: 622.8 KB (622836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:468d88f1731dd43e26dd4cd67ca7706cac23e69784c09d6a3c756990491266b2`  
		Last Modified: Fri, 01 Dec 2023 07:16:47 GMT  
		Size: 39.3 MB (39255906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4966766b6d36ef16ab755867f8f4240384b5df5f3699a20bc921ae2f38bea544`  
		Last Modified: Fri, 01 Dec 2023 07:16:40 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v3.0.0-beta5-windowsservercore-1809`

```console
$ docker pull traefik@sha256:0f412e66210777c883a54e671f60c95159b94d5b48596212dbbf46ed7d0ad155
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.5206; amd64

### `traefik:v3.0.0-beta5-windowsservercore-1809` - windows version 10.0.17763.5206; amd64

```console
$ docker pull traefik@sha256:b0d1ace70fadf4ab2b19b1dff9e3bf079bc39a5e1e4f82b0990f8118ef7c2fbc
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.1 GB (2101540237 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5d31b5dd9bb9f459a762c01fa0bfebfd9988aec4cfc2dc4ae89f67621e26dd87`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Mon, 04 Dec 2023 11:24:49 GMT
RUN Install update 10.0.17763.5206
# Tue, 12 Dec 2023 23:38:52 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 13 Dec 2023 05:38:12 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/traefik/traefik/releases/download/v3.0.0-beta5/traefik_v3.0.0-beta5_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Wed, 13 Dec 2023 05:38:13 GMT
EXPOSE 80
# Wed, 13 Dec 2023 05:38:14 GMT
ENTRYPOINT ["/traefik"]
# Wed, 13 Dec 2023 05:38:14 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v3.0.0-beta5 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e35ae5ad761bfd7e5fb48c234de8722eaa28e17e2c956816fecb417ab6259c29`  
		Last Modified: Tue, 12 Dec 2023 19:14:24 GMT  
		Size: 409.1 MB (409088642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:767e95390edb4050b2c57e1d564c9e4722c5ae776ebfb8907a539571a2609f7c`  
		Last Modified: Wed, 13 Dec 2023 00:04:16 GMT  
		Size: 1.3 KB (1331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:deb6a249618abc946bb07da6a95961688fcff9fc27ba6028587dbc3b8e351040`  
		Last Modified: Wed, 13 Dec 2023 05:40:09 GMT  
		Size: 41.8 MB (41825635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4242fed3cdc37df02c943b51816721ed2f17d5e7910ee80c7a45e1aa8ba1515c`  
		Last Modified: Wed, 13 Dec 2023 05:39:59 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97ad766c58568f8acc07437c5a77230c7e2ce584a555d36af2efaccb45c29bb4`  
		Last Modified: Wed, 13 Dec 2023 05:39:59 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ec2c2c191a4791893dde01c1e4d8ecf7150791ff338a8c45fb741c5494915ef`  
		Last Modified: Wed, 13 Dec 2023 05:39:59 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:windowsservercore-1809`

```console
$ docker pull traefik@sha256:997103b42ff82fc02e26323fc34626675978fcf84c34148a68a4e376fdc07223
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.5206; amd64

### `traefik:windowsservercore-1809` - windows version 10.0.17763.5206; amd64

```console
$ docker pull traefik@sha256:06f73ead67b5686b93a0b8fe093e13e419c0a5d0b419da55bf1fdfd57ea3d693
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.1 GB (2100437516 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c3a543f322817696bfe1ba7e91e9d8a1ffd40812dfa85a02964f932e791f7a65`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Mon, 04 Dec 2023 11:24:49 GMT
RUN Install update 10.0.17763.5206
# Tue, 12 Dec 2023 23:38:52 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 13 Dec 2023 05:39:33 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/traefik/traefik/releases/download/v2.10.7/traefik_v2.10.7_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Wed, 13 Dec 2023 05:39:34 GMT
EXPOSE 80
# Wed, 13 Dec 2023 05:39:35 GMT
ENTRYPOINT ["/traefik"]
# Wed, 13 Dec 2023 05:39:37 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.10.7 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e35ae5ad761bfd7e5fb48c234de8722eaa28e17e2c956816fecb417ab6259c29`  
		Last Modified: Tue, 12 Dec 2023 19:14:24 GMT  
		Size: 409.1 MB (409088642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:767e95390edb4050b2c57e1d564c9e4722c5ae776ebfb8907a539571a2609f7c`  
		Last Modified: Wed, 13 Dec 2023 00:04:16 GMT  
		Size: 1.3 KB (1331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bff8297f6fad9a7479830d3d1ea2b96f0687d0f83579d405544e13911ed987d8`  
		Last Modified: Wed, 13 Dec 2023 05:40:32 GMT  
		Size: 40.7 MB (40722910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fd9eab97690e5362be049befc774a9b7d7553a578050b9b48dfda36a0436c3b`  
		Last Modified: Wed, 13 Dec 2023 05:40:23 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd7ffc3c473c5e1dee69514c2e7db4368ef6a3039ec0e16aac676559a9f09d63`  
		Last Modified: Wed, 13 Dec 2023 05:40:23 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24eea685fcd95841874da2ede817120c73864d0ade3aa21ba06040b1f5f15ccd`  
		Last Modified: Wed, 13 Dec 2023 05:40:23 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
