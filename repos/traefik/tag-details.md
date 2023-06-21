<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `traefik`

-	[`traefik:2.10`](#traefik210)
-	[`traefik:2.10-windowsservercore-1809`](#traefik210-windowsservercore-1809)
-	[`traefik:2.10.3`](#traefik2103)
-	[`traefik:2.10.3-windowsservercore-1809`](#traefik2103-windowsservercore-1809)
-	[`traefik:3.0`](#traefik30)
-	[`traefik:3.0-windowsservercore-1809`](#traefik30-windowsservercore-1809)
-	[`traefik:3.0.0-beta2`](#traefik300-beta2)
-	[`traefik:3.0.0-beta2-windowsservercore-1809`](#traefik300-beta2-windowsservercore-1809)
-	[`traefik:beaufort`](#traefikbeaufort)
-	[`traefik:beaufort-windowsservercore-1809`](#traefikbeaufort-windowsservercore-1809)
-	[`traefik:latest`](#traefiklatest)
-	[`traefik:saintmarcelin`](#traefiksaintmarcelin)
-	[`traefik:saintmarcelin-windowsservercore-1809`](#traefiksaintmarcelin-windowsservercore-1809)
-	[`traefik:v2.10`](#traefikv210)
-	[`traefik:v2.10-windowsservercore-1809`](#traefikv210-windowsservercore-1809)
-	[`traefik:v2.10.3`](#traefikv2103)
-	[`traefik:v2.10.3-windowsservercore-1809`](#traefikv2103-windowsservercore-1809)
-	[`traefik:v3.0`](#traefikv30)
-	[`traefik:v3.0-windowsservercore-1809`](#traefikv30-windowsservercore-1809)
-	[`traefik:v3.0.0-beta2`](#traefikv300-beta2)
-	[`traefik:v3.0.0-beta2-windowsservercore-1809`](#traefikv300-beta2-windowsservercore-1809)
-	[`traefik:windowsservercore-1809`](#traefikwindowsservercore-1809)

## `traefik:2.10`

```console
$ docker pull traefik@sha256:c272e8c32fb7356c2166bc5d170ab0a2c73da7bfec561234c52f255ece1dd07c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; s390x

### `traefik:2.10` - linux; amd64

```console
$ docker pull traefik@sha256:79c24d0686fa0679cde49f275e694afb7ef6d182b9fe21a219463e2a6bfe4ece
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.2 MB (41246766 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a07d037aae0a48737ff74bbd136e6a809cb25af2fd7754a2168e038a5b9534eb`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 14 Jun 2023 20:41:58 GMT
ADD file:1da756d12551a0e3e793e02ef87432d69d4968937bd11bed0af215db19dd94cd in / 
# Wed, 14 Jun 2023 20:41:59 GMT
CMD ["/bin/sh"]
# Wed, 21 Jun 2023 00:26:12 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 21 Jun 2023 00:26:15 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.10.3/traefik_v2.10.3_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Wed, 21 Jun 2023 00:26:16 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 21 Jun 2023 00:26:16 GMT
EXPOSE 80
# Wed, 21 Jun 2023 00:26:16 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 21 Jun 2023 00:26:16 GMT
CMD ["traefik"]
# Wed, 21 Jun 2023 00:26:16 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.10.3 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:31e352740f534f9ad170f75378a84fe453d6156e40700b882d737a8f4a6988a3`  
		Last Modified: Wed, 14 Jun 2023 20:42:26 GMT  
		Size: 3.4 MB (3397879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b9a9b499d7ae3ed84aef77186cbd2b1ae5418ddc653e721702ec1a35fa324a3`  
		Last Modified: Wed, 21 Jun 2023 00:26:31 GMT  
		Size: 622.2 KB (622241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d581263ee7dc4ec5a72666259aadc3c7072d84df3ef862f3b3737b8392eb09d4`  
		Last Modified: Wed, 21 Jun 2023 00:26:36 GMT  
		Size: 37.2 MB (37226281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5f0f39a1a90d628163b34d2a35ff662ec098d350ce46a3737f1905c7dc2f954`  
		Last Modified: Wed, 21 Jun 2023 00:26:30 GMT  
		Size: 365.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:2.10` - linux; arm variant v6

```console
$ docker pull traefik@sha256:bf02196efc8a2e8a41c9cba0363d89f7c64d294e70c7f2e36f46d2f7a1405e69
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.8 MB (38806469 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6a8dac0c0e2cda3bc1bdbd21f6b252c8cfb432270813b0e32421cdcd16a40707`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 14 Jun 2023 18:49:20 GMT
ADD file:4213782693bf27a9a6de23bc924ef0c4fb6b2d56010fc07b25f81edeba83b0d4 in / 
# Wed, 14 Jun 2023 18:49:20 GMT
CMD ["/bin/sh"]
# Tue, 20 Jun 2023 22:49:44 GMT
RUN apk --no-cache add ca-certificates tzdata
# Tue, 20 Jun 2023 22:49:48 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.10.3/traefik_v2.10.3_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Tue, 20 Jun 2023 22:49:49 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Tue, 20 Jun 2023 22:49:49 GMT
EXPOSE 80
# Tue, 20 Jun 2023 22:49:49 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 20 Jun 2023 22:49:49 GMT
CMD ["traefik"]
# Tue, 20 Jun 2023 22:49:49 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.10.3 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:7836be94d3024e2042069c1095caba0b391f70c4b3d34a0475a503239d73dfba`  
		Last Modified: Wed, 14 Jun 2023 18:49:46 GMT  
		Size: 3.1 MB (3143353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be273dc11f4147c3910cbabccdb1e28523a1cb24f3f849c4c36c5a2ce46bd092`  
		Last Modified: Tue, 20 Jun 2023 22:50:03 GMT  
		Size: 622.7 KB (622687 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:053ac18b4541fcb4b8456e7b5db6257d6201478c985190a80138c877c6b54962`  
		Last Modified: Tue, 20 Jun 2023 22:50:09 GMT  
		Size: 35.0 MB (35040063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c3b139cedf00b646032b604d4f6a681890378569bb9fff6767c64e2e5d6bdb7`  
		Last Modified: Tue, 20 Jun 2023 22:50:03 GMT  
		Size: 366.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:2.10` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:3c5daac31719a3158b5ba95d98fa7987ec31a971803c9aca2dca7e02022b23e8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.0 MB (38039994 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:28c14b3be10b718677713d790e913fc0743b8c9703c0dc5d4984a30526cf53f3`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 14 Jun 2023 20:48:58 GMT
ADD file:289c2fac17119508ced527225d445747cd177111b4a0018a6b04948ecb3b5e29 in / 
# Wed, 14 Jun 2023 20:48:58 GMT
CMD ["/bin/sh"]
# Tue, 20 Jun 2023 23:21:47 GMT
RUN apk --no-cache add ca-certificates tzdata
# Tue, 20 Jun 2023 23:21:50 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.10.3/traefik_v2.10.3_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Tue, 20 Jun 2023 23:21:50 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Tue, 20 Jun 2023 23:21:50 GMT
EXPOSE 80
# Tue, 20 Jun 2023 23:21:50 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 20 Jun 2023 23:21:50 GMT
CMD ["traefik"]
# Tue, 20 Jun 2023 23:21:50 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.10.3 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:8c6d1654570f041603f4cef49c320c8f6f3e401324913009d92a19132cbf1ac0`  
		Last Modified: Wed, 14 Jun 2023 20:49:23 GMT  
		Size: 3.3 MB (3329251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b960a271861d2b8bee110ab4afb7ec842665bbbd31f1bb9c1c279cd78d925fc`  
		Last Modified: Tue, 20 Jun 2023 23:22:04 GMT  
		Size: 624.5 KB (624502 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:754fa8e2a433d2589523d839325fd39c00d1a345d3e30234db2d388fdf21d845`  
		Last Modified: Tue, 20 Jun 2023 23:22:08 GMT  
		Size: 34.1 MB (34085876 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e6c2fdac2a73f03934e5e0d484b0746a11e42421db9f59e1eec0e7550b7bf59`  
		Last Modified: Tue, 20 Jun 2023 23:22:04 GMT  
		Size: 365.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:2.10` - linux; s390x

```console
$ docker pull traefik@sha256:9b2e7255584bc1bdf07b8ff66cb3c9ce52c952af2009751c311c9e793f3b3040
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.9 MB (39925281 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5eeb14a180e79a1752259e241dc5b9d14fd6eeabdc2776f52e5bca7fd723c5fd`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 15 Jun 2023 05:18:38 GMT
ADD file:a59beca78118ebf4f86cc1685237dc3a29a519401a70668da520beaa3d29eb7a in / 
# Thu, 15 Jun 2023 05:18:38 GMT
CMD ["/bin/sh"]
# Tue, 20 Jun 2023 22:49:13 GMT
RUN apk --no-cache add ca-certificates tzdata
# Tue, 20 Jun 2023 22:49:18 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.10.3/traefik_v2.10.3_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Tue, 20 Jun 2023 22:49:20 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Tue, 20 Jun 2023 22:49:20 GMT
EXPOSE 80
# Tue, 20 Jun 2023 22:49:20 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 20 Jun 2023 22:49:20 GMT
CMD ["traefik"]
# Tue, 20 Jun 2023 22:49:20 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.10.3 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:998cc98447b44e5f0fe799dce691412796ba586ab22eb7c99aebf9d45f34833b`  
		Last Modified: Thu, 15 Jun 2023 05:29:38 GMT  
		Size: 3.2 MB (3213497 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b6fdd3c34275458c3ea0a8688ec24b8c7698ce5a31715673ae57aa8dd5b0844`  
		Last Modified: Tue, 20 Jun 2023 22:49:39 GMT  
		Size: 622.8 KB (622821 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c041a673abae644852705ba64c910a0ebec6c0ea502a06264644f44da6e2e2d`  
		Last Modified: Tue, 20 Jun 2023 22:49:44 GMT  
		Size: 36.1 MB (36088597 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdef234383c44175d81f3fd1a8a0d6970aee17a833bcd7d578a690d36c46efb1`  
		Last Modified: Tue, 20 Jun 2023 22:49:39 GMT  
		Size: 366.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:2.10-windowsservercore-1809`

```console
$ docker pull traefik@sha256:dc03c1897e7fa9697744289086dfd429fc4b22694446bb29881671bd63335f55
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4499; amd64

### `traefik:2.10-windowsservercore-1809` - windows version 10.0.17763.4499; amd64

```console
$ docker pull traefik@sha256:b61a301ec003fdfb61afa059050468dfd19e329b91adc04b989378307c01e5b9
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.7 GB (1688297643 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c40b4425780339ae5ed986b0312fde45ee26d18c675994fa07879d3ba8ba802f`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Wed, 14 Jun 2023 17:39:58 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 20 Jun 2023 23:18:02 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/traefik/traefik/releases/download/v2.10.3/traefik_v2.10.3_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Tue, 20 Jun 2023 23:18:04 GMT
EXPOSE 80
# Tue, 20 Jun 2023 23:18:05 GMT
ENTRYPOINT ["/traefik"]
# Tue, 20 Jun 2023 23:18:06 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.10.3 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b712a9a082fd391beaa9ca7c8e6c3fda37b0ad8d29cc4663173ed973b961d342`  
		Last Modified: Wed, 14 Jun 2023 18:21:55 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6ae7661d409041f0b91655d0629e3756f67688eabbeb2d46f7c44b9e110614a`  
		Last Modified: Tue, 20 Jun 2023 23:18:40 GMT  
		Size: 37.7 MB (37671801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eda08f2fb0ae872eb7d6aee508ca42acf0aa7d71c4cc8b22b2acd32a8dac9307`  
		Last Modified: Tue, 20 Jun 2023 23:18:30 GMT  
		Size: 1.3 KB (1301 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7fc4c49780e0c6b8e9d6e2577ae7f3597396920dbd9c744ace14c79b3db639e`  
		Last Modified: Tue, 20 Jun 2023 23:18:30 GMT  
		Size: 1.4 KB (1362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7546eab39455c2a7df3171964211f93193cc95597a50435a4c7e5e3ee22b6f2`  
		Last Modified: Tue, 20 Jun 2023 23:18:30 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:2.10.3`

```console
$ docker pull traefik@sha256:c272e8c32fb7356c2166bc5d170ab0a2c73da7bfec561234c52f255ece1dd07c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; s390x

### `traefik:2.10.3` - linux; amd64

```console
$ docker pull traefik@sha256:79c24d0686fa0679cde49f275e694afb7ef6d182b9fe21a219463e2a6bfe4ece
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.2 MB (41246766 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a07d037aae0a48737ff74bbd136e6a809cb25af2fd7754a2168e038a5b9534eb`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 14 Jun 2023 20:41:58 GMT
ADD file:1da756d12551a0e3e793e02ef87432d69d4968937bd11bed0af215db19dd94cd in / 
# Wed, 14 Jun 2023 20:41:59 GMT
CMD ["/bin/sh"]
# Wed, 21 Jun 2023 00:26:12 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 21 Jun 2023 00:26:15 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.10.3/traefik_v2.10.3_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Wed, 21 Jun 2023 00:26:16 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 21 Jun 2023 00:26:16 GMT
EXPOSE 80
# Wed, 21 Jun 2023 00:26:16 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 21 Jun 2023 00:26:16 GMT
CMD ["traefik"]
# Wed, 21 Jun 2023 00:26:16 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.10.3 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:31e352740f534f9ad170f75378a84fe453d6156e40700b882d737a8f4a6988a3`  
		Last Modified: Wed, 14 Jun 2023 20:42:26 GMT  
		Size: 3.4 MB (3397879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b9a9b499d7ae3ed84aef77186cbd2b1ae5418ddc653e721702ec1a35fa324a3`  
		Last Modified: Wed, 21 Jun 2023 00:26:31 GMT  
		Size: 622.2 KB (622241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d581263ee7dc4ec5a72666259aadc3c7072d84df3ef862f3b3737b8392eb09d4`  
		Last Modified: Wed, 21 Jun 2023 00:26:36 GMT  
		Size: 37.2 MB (37226281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5f0f39a1a90d628163b34d2a35ff662ec098d350ce46a3737f1905c7dc2f954`  
		Last Modified: Wed, 21 Jun 2023 00:26:30 GMT  
		Size: 365.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:2.10.3` - linux; arm variant v6

```console
$ docker pull traefik@sha256:bf02196efc8a2e8a41c9cba0363d89f7c64d294e70c7f2e36f46d2f7a1405e69
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.8 MB (38806469 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6a8dac0c0e2cda3bc1bdbd21f6b252c8cfb432270813b0e32421cdcd16a40707`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 14 Jun 2023 18:49:20 GMT
ADD file:4213782693bf27a9a6de23bc924ef0c4fb6b2d56010fc07b25f81edeba83b0d4 in / 
# Wed, 14 Jun 2023 18:49:20 GMT
CMD ["/bin/sh"]
# Tue, 20 Jun 2023 22:49:44 GMT
RUN apk --no-cache add ca-certificates tzdata
# Tue, 20 Jun 2023 22:49:48 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.10.3/traefik_v2.10.3_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Tue, 20 Jun 2023 22:49:49 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Tue, 20 Jun 2023 22:49:49 GMT
EXPOSE 80
# Tue, 20 Jun 2023 22:49:49 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 20 Jun 2023 22:49:49 GMT
CMD ["traefik"]
# Tue, 20 Jun 2023 22:49:49 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.10.3 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:7836be94d3024e2042069c1095caba0b391f70c4b3d34a0475a503239d73dfba`  
		Last Modified: Wed, 14 Jun 2023 18:49:46 GMT  
		Size: 3.1 MB (3143353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be273dc11f4147c3910cbabccdb1e28523a1cb24f3f849c4c36c5a2ce46bd092`  
		Last Modified: Tue, 20 Jun 2023 22:50:03 GMT  
		Size: 622.7 KB (622687 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:053ac18b4541fcb4b8456e7b5db6257d6201478c985190a80138c877c6b54962`  
		Last Modified: Tue, 20 Jun 2023 22:50:09 GMT  
		Size: 35.0 MB (35040063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c3b139cedf00b646032b604d4f6a681890378569bb9fff6767c64e2e5d6bdb7`  
		Last Modified: Tue, 20 Jun 2023 22:50:03 GMT  
		Size: 366.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:2.10.3` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:3c5daac31719a3158b5ba95d98fa7987ec31a971803c9aca2dca7e02022b23e8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.0 MB (38039994 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:28c14b3be10b718677713d790e913fc0743b8c9703c0dc5d4984a30526cf53f3`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 14 Jun 2023 20:48:58 GMT
ADD file:289c2fac17119508ced527225d445747cd177111b4a0018a6b04948ecb3b5e29 in / 
# Wed, 14 Jun 2023 20:48:58 GMT
CMD ["/bin/sh"]
# Tue, 20 Jun 2023 23:21:47 GMT
RUN apk --no-cache add ca-certificates tzdata
# Tue, 20 Jun 2023 23:21:50 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.10.3/traefik_v2.10.3_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Tue, 20 Jun 2023 23:21:50 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Tue, 20 Jun 2023 23:21:50 GMT
EXPOSE 80
# Tue, 20 Jun 2023 23:21:50 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 20 Jun 2023 23:21:50 GMT
CMD ["traefik"]
# Tue, 20 Jun 2023 23:21:50 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.10.3 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:8c6d1654570f041603f4cef49c320c8f6f3e401324913009d92a19132cbf1ac0`  
		Last Modified: Wed, 14 Jun 2023 20:49:23 GMT  
		Size: 3.3 MB (3329251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b960a271861d2b8bee110ab4afb7ec842665bbbd31f1bb9c1c279cd78d925fc`  
		Last Modified: Tue, 20 Jun 2023 23:22:04 GMT  
		Size: 624.5 KB (624502 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:754fa8e2a433d2589523d839325fd39c00d1a345d3e30234db2d388fdf21d845`  
		Last Modified: Tue, 20 Jun 2023 23:22:08 GMT  
		Size: 34.1 MB (34085876 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e6c2fdac2a73f03934e5e0d484b0746a11e42421db9f59e1eec0e7550b7bf59`  
		Last Modified: Tue, 20 Jun 2023 23:22:04 GMT  
		Size: 365.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:2.10.3` - linux; s390x

```console
$ docker pull traefik@sha256:9b2e7255584bc1bdf07b8ff66cb3c9ce52c952af2009751c311c9e793f3b3040
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.9 MB (39925281 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5eeb14a180e79a1752259e241dc5b9d14fd6eeabdc2776f52e5bca7fd723c5fd`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 15 Jun 2023 05:18:38 GMT
ADD file:a59beca78118ebf4f86cc1685237dc3a29a519401a70668da520beaa3d29eb7a in / 
# Thu, 15 Jun 2023 05:18:38 GMT
CMD ["/bin/sh"]
# Tue, 20 Jun 2023 22:49:13 GMT
RUN apk --no-cache add ca-certificates tzdata
# Tue, 20 Jun 2023 22:49:18 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.10.3/traefik_v2.10.3_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Tue, 20 Jun 2023 22:49:20 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Tue, 20 Jun 2023 22:49:20 GMT
EXPOSE 80
# Tue, 20 Jun 2023 22:49:20 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 20 Jun 2023 22:49:20 GMT
CMD ["traefik"]
# Tue, 20 Jun 2023 22:49:20 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.10.3 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:998cc98447b44e5f0fe799dce691412796ba586ab22eb7c99aebf9d45f34833b`  
		Last Modified: Thu, 15 Jun 2023 05:29:38 GMT  
		Size: 3.2 MB (3213497 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b6fdd3c34275458c3ea0a8688ec24b8c7698ce5a31715673ae57aa8dd5b0844`  
		Last Modified: Tue, 20 Jun 2023 22:49:39 GMT  
		Size: 622.8 KB (622821 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c041a673abae644852705ba64c910a0ebec6c0ea502a06264644f44da6e2e2d`  
		Last Modified: Tue, 20 Jun 2023 22:49:44 GMT  
		Size: 36.1 MB (36088597 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdef234383c44175d81f3fd1a8a0d6970aee17a833bcd7d578a690d36c46efb1`  
		Last Modified: Tue, 20 Jun 2023 22:49:39 GMT  
		Size: 366.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:2.10.3-windowsservercore-1809`

```console
$ docker pull traefik@sha256:dc03c1897e7fa9697744289086dfd429fc4b22694446bb29881671bd63335f55
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4499; amd64

### `traefik:2.10.3-windowsservercore-1809` - windows version 10.0.17763.4499; amd64

```console
$ docker pull traefik@sha256:b61a301ec003fdfb61afa059050468dfd19e329b91adc04b989378307c01e5b9
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.7 GB (1688297643 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c40b4425780339ae5ed986b0312fde45ee26d18c675994fa07879d3ba8ba802f`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Wed, 14 Jun 2023 17:39:58 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 20 Jun 2023 23:18:02 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/traefik/traefik/releases/download/v2.10.3/traefik_v2.10.3_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Tue, 20 Jun 2023 23:18:04 GMT
EXPOSE 80
# Tue, 20 Jun 2023 23:18:05 GMT
ENTRYPOINT ["/traefik"]
# Tue, 20 Jun 2023 23:18:06 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.10.3 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b712a9a082fd391beaa9ca7c8e6c3fda37b0ad8d29cc4663173ed973b961d342`  
		Last Modified: Wed, 14 Jun 2023 18:21:55 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6ae7661d409041f0b91655d0629e3756f67688eabbeb2d46f7c44b9e110614a`  
		Last Modified: Tue, 20 Jun 2023 23:18:40 GMT  
		Size: 37.7 MB (37671801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eda08f2fb0ae872eb7d6aee508ca42acf0aa7d71c4cc8b22b2acd32a8dac9307`  
		Last Modified: Tue, 20 Jun 2023 23:18:30 GMT  
		Size: 1.3 KB (1301 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7fc4c49780e0c6b8e9d6e2577ae7f3597396920dbd9c744ace14c79b3db639e`  
		Last Modified: Tue, 20 Jun 2023 23:18:30 GMT  
		Size: 1.4 KB (1362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7546eab39455c2a7df3171964211f93193cc95597a50435a4c7e5e3ee22b6f2`  
		Last Modified: Tue, 20 Jun 2023 23:18:30 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:3.0`

```console
$ docker pull traefik@sha256:366345ddd7c17a8d273696797a375c5144e3a5242bdb39a2855baaec2bd6851c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; s390x

### `traefik:3.0` - linux; amd64

```console
$ docker pull traefik@sha256:5f3e471200c36a65618b50719f8f467530a9895a61f87bda0bb437b5718ac327
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.6 MB (40562366 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c08e518a729607ef1142c8a57a82ab9df16bcd47e4e5a6874d07467e07a87dd0`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 14 Jun 2023 20:42:13 GMT
ADD file:4fa8e307f595ecff485113fb0ec6e2320979eaa6fb3eb467d2433771a6f016e6 in / 
# Wed, 14 Jun 2023 20:42:13 GMT
CMD ["/bin/sh"]
# Thu, 15 Jun 2023 06:27:27 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 15 Jun 2023 06:27:31 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v3.0.0-beta2/traefik_v3.0.0-beta2_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 15 Jun 2023 06:27:31 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 15 Jun 2023 06:27:31 GMT
EXPOSE 80
# Thu, 15 Jun 2023 06:27:31 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 15 Jun 2023 06:27:31 GMT
CMD ["traefik"]
# Thu, 15 Jun 2023 06:27:31 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v3.0.0-beta2 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:0cdfa0c98ed79707cd91c5dd7ebd282aa2b976d86a9e699d7fc188cdb6be390e`  
		Last Modified: Wed, 14 Jun 2023 20:42:58 GMT  
		Size: 2.8 MB (2825916 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75174169df6666c22d9a3c3085ea1eacd10478e79c70bbd53abc6cf647134b86`  
		Last Modified: Thu, 15 Jun 2023 06:27:51 GMT  
		Size: 661.2 KB (661203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4920635d165c3cb67e2ee3fd37aec68049e9730086d72999c5d926fd5a2b5bdb`  
		Last Modified: Thu, 15 Jun 2023 06:27:56 GMT  
		Size: 37.1 MB (37074878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:133801879169abc43871a5a32c77fb651e1ae90c3233a0cce11b6ead5c526c79`  
		Last Modified: Thu, 15 Jun 2023 06:27:50 GMT  
		Size: 369.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:3.0` - linux; arm variant v6

```console
$ docker pull traefik@sha256:0e010dd7b60c3960f903b07854cae707e691496f1491f0447ca2635b5a374a6d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.3 MB (38289085 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ee0012c6d54cfd4da66d0da5e01f3dc4f70609eec928ce429e71a5efa02c96b3`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 14 Jun 2023 18:49:32 GMT
ADD file:b987db82fa4ce6e623de49a50612c1fd91c5ab2209a62a5727ab3436c2923e91 in / 
# Wed, 14 Jun 2023 18:49:32 GMT
CMD ["/bin/sh"]
# Wed, 14 Jun 2023 20:12:22 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 14 Jun 2023 20:12:26 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v3.0.0-beta2/traefik_v3.0.0-beta2_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Wed, 14 Jun 2023 20:12:26 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 14 Jun 2023 20:12:26 GMT
EXPOSE 80
# Wed, 14 Jun 2023 20:12:26 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 14 Jun 2023 20:12:26 GMT
CMD ["traefik"]
# Wed, 14 Jun 2023 20:12:26 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v3.0.0-beta2 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:41c5c5b38e13af18def277385607129664fb24993d262d4b601a381e776482a9`  
		Last Modified: Wed, 14 Jun 2023 18:50:19 GMT  
		Size: 2.6 MB (2633060 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:718cfe2cb66c053a8fdb09adf88b20a52f260f22abd38cba68cc2838ee33e73d`  
		Last Modified: Wed, 14 Jun 2023 20:12:46 GMT  
		Size: 666.3 KB (666349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47b2cef5f2c79471c563b3c10376140084b51c097de00e9be0b758219ab95e5c`  
		Last Modified: Wed, 14 Jun 2023 20:12:52 GMT  
		Size: 35.0 MB (34989308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66078e59ed6730404193e57cea654480d0731663c7a068349344e0a681d1c660`  
		Last Modified: Wed, 14 Jun 2023 20:12:46 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:3.0` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:70a1b62539b384a09d98e22bea5212f0120150377a85a599839d35897a55ef3b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.4 MB (37406948 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ebe5414a44cb1b3f5ada2c4d4477d9bb6c73103354707edb71a0adfb2138efb4`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 14 Jun 2023 20:49:10 GMT
ADD file:2b463f242cb7bf946452bb4781838348ecbe80da144fbab09f51d7e050dc68f3 in / 
# Wed, 14 Jun 2023 20:49:11 GMT
CMD ["/bin/sh"]
# Thu, 15 Jun 2023 07:10:02 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 15 Jun 2023 07:10:05 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v3.0.0-beta2/traefik_v3.0.0-beta2_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 15 Jun 2023 07:10:05 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 15 Jun 2023 07:10:05 GMT
EXPOSE 80
# Thu, 15 Jun 2023 07:10:05 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 15 Jun 2023 07:10:06 GMT
CMD ["traefik"]
# Thu, 15 Jun 2023 07:10:06 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v3.0.0-beta2 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:a147224bf413aeffbbfcdcb5104d35c647256a5c32083f4d8134f09a4e74ddeb`  
		Last Modified: Wed, 14 Jun 2023 20:49:52 GMT  
		Size: 2.7 MB (2720801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d273c78104fe60b8d6b0a1d68c0b259293bd972e3ff515bc403a8bfbff6d88a9`  
		Last Modified: Thu, 15 Jun 2023 07:10:24 GMT  
		Size: 662.3 KB (662262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2be3d50287a2f7fba1e120466ee42285469a74914da1378df40803a29c6245f3`  
		Last Modified: Thu, 15 Jun 2023 07:10:28 GMT  
		Size: 34.0 MB (34023516 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:452eba291077ce9af0d14edf868a5522679b04016d43f8a2e05b194d2618d210`  
		Last Modified: Thu, 15 Jun 2023 07:10:24 GMT  
		Size: 369.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:3.0` - linux; s390x

```console
$ docker pull traefik@sha256:feacc7d5c4b3a2d20dcbfc15e95e848cbc3b83820b99cafd9807db1863b65891
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.1 MB (39130249 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:af3c57f022e7ac6f998e72d571ec87f092a10f19341601105cd3f5c2b767d2ad`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 15 Jun 2023 05:22:08 GMT
ADD file:243e0553a1216040e760e1a7ce7119b10b477e081d792fa29e8c17403a8785ff in / 
# Thu, 15 Jun 2023 05:22:08 GMT
CMD ["/bin/sh"]
# Fri, 16 Jun 2023 16:39:46 GMT
RUN apk --no-cache add ca-certificates tzdata
# Fri, 16 Jun 2023 16:39:50 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v3.0.0-beta2/traefik_v3.0.0-beta2_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Fri, 16 Jun 2023 16:39:52 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Fri, 16 Jun 2023 16:39:52 GMT
EXPOSE 80
# Fri, 16 Jun 2023 16:39:52 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 16 Jun 2023 16:39:52 GMT
CMD ["traefik"]
# Fri, 16 Jun 2023 16:39:52 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v3.0.0-beta2 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:66238d49bc5bf7485c63b2671ef3c879dd2015902b151f6f5e7d178cf472c9f2`  
		Last Modified: Thu, 15 Jun 2023 05:32:59 GMT  
		Size: 2.6 MB (2608705 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42d9a3c534bf80ba9a88587c1fd786fafea714685bd2abfac3984c6ddfda55b2`  
		Last Modified: Fri, 16 Jun 2023 16:40:22 GMT  
		Size: 665.7 KB (665740 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72fef4a8a0cc5f1eea5507fd77aa05a9500cb4d1ef385312c7bcbae389046009`  
		Last Modified: Fri, 16 Jun 2023 16:40:28 GMT  
		Size: 35.9 MB (35855437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f5a752b613a2cf39692fa7636be262af8c16ac0a46e8abf8702c047ab934522`  
		Last Modified: Fri, 16 Jun 2023 16:40:22 GMT  
		Size: 367.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:3.0-windowsservercore-1809`

```console
$ docker pull traefik@sha256:468282899a6f9b06f9fca5ebb1a3a5bf030b45e63e0508f36f75ad7792100318
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4499; amd64

### `traefik:3.0-windowsservercore-1809` - windows version 10.0.17763.4499; amd64

```console
$ docker pull traefik@sha256:58a44dc3d5c4e9816d6873d753a6074c23aa7a462052f72f8fb60172ae00773b
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.7 GB (1688143673 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:01f1804410c439a02c3fbb603e3dc9c1a10922016750389db87aed22db51adb2`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Wed, 14 Jun 2023 17:39:58 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 14 Jun 2023 23:20:14 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/traefik/traefik/releases/download/v3.0.0-beta2/traefik_v3.0.0-beta2_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Wed, 14 Jun 2023 23:20:15 GMT
EXPOSE 80
# Wed, 14 Jun 2023 23:20:15 GMT
ENTRYPOINT ["/traefik"]
# Wed, 14 Jun 2023 23:20:16 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v3.0.0-beta2 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b712a9a082fd391beaa9ca7c8e6c3fda37b0ad8d29cc4663173ed973b961d342`  
		Last Modified: Wed, 14 Jun 2023 18:21:55 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a9b4e4d63720e53bc602ec5afd594ae87dc8d306b5873781d0fd3055f818c16`  
		Last Modified: Wed, 14 Jun 2023 23:21:42 GMT  
		Size: 37.5 MB (37517697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef864bbe2da9a6fc6aba62dc459a1b659d3d46ada2e3a1a04ee8b7c02a6f4e92`  
		Last Modified: Wed, 14 Jun 2023 23:21:33 GMT  
		Size: 1.4 KB (1377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2213ec09fd524be95c6a826c50e14f52e9e639e66c3572d56f438bac3cf98bab`  
		Last Modified: Wed, 14 Jun 2023 23:21:33 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58cd9c99e4865330e999c8136c9600504c563b6c37779e28663ff1421a7ac516`  
		Last Modified: Wed, 14 Jun 2023 23:21:33 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:3.0.0-beta2`

```console
$ docker pull traefik@sha256:366345ddd7c17a8d273696797a375c5144e3a5242bdb39a2855baaec2bd6851c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; s390x

### `traefik:3.0.0-beta2` - linux; amd64

```console
$ docker pull traefik@sha256:5f3e471200c36a65618b50719f8f467530a9895a61f87bda0bb437b5718ac327
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.6 MB (40562366 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c08e518a729607ef1142c8a57a82ab9df16bcd47e4e5a6874d07467e07a87dd0`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 14 Jun 2023 20:42:13 GMT
ADD file:4fa8e307f595ecff485113fb0ec6e2320979eaa6fb3eb467d2433771a6f016e6 in / 
# Wed, 14 Jun 2023 20:42:13 GMT
CMD ["/bin/sh"]
# Thu, 15 Jun 2023 06:27:27 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 15 Jun 2023 06:27:31 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v3.0.0-beta2/traefik_v3.0.0-beta2_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 15 Jun 2023 06:27:31 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 15 Jun 2023 06:27:31 GMT
EXPOSE 80
# Thu, 15 Jun 2023 06:27:31 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 15 Jun 2023 06:27:31 GMT
CMD ["traefik"]
# Thu, 15 Jun 2023 06:27:31 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v3.0.0-beta2 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:0cdfa0c98ed79707cd91c5dd7ebd282aa2b976d86a9e699d7fc188cdb6be390e`  
		Last Modified: Wed, 14 Jun 2023 20:42:58 GMT  
		Size: 2.8 MB (2825916 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75174169df6666c22d9a3c3085ea1eacd10478e79c70bbd53abc6cf647134b86`  
		Last Modified: Thu, 15 Jun 2023 06:27:51 GMT  
		Size: 661.2 KB (661203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4920635d165c3cb67e2ee3fd37aec68049e9730086d72999c5d926fd5a2b5bdb`  
		Last Modified: Thu, 15 Jun 2023 06:27:56 GMT  
		Size: 37.1 MB (37074878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:133801879169abc43871a5a32c77fb651e1ae90c3233a0cce11b6ead5c526c79`  
		Last Modified: Thu, 15 Jun 2023 06:27:50 GMT  
		Size: 369.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:3.0.0-beta2` - linux; arm variant v6

```console
$ docker pull traefik@sha256:0e010dd7b60c3960f903b07854cae707e691496f1491f0447ca2635b5a374a6d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.3 MB (38289085 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ee0012c6d54cfd4da66d0da5e01f3dc4f70609eec928ce429e71a5efa02c96b3`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 14 Jun 2023 18:49:32 GMT
ADD file:b987db82fa4ce6e623de49a50612c1fd91c5ab2209a62a5727ab3436c2923e91 in / 
# Wed, 14 Jun 2023 18:49:32 GMT
CMD ["/bin/sh"]
# Wed, 14 Jun 2023 20:12:22 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 14 Jun 2023 20:12:26 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v3.0.0-beta2/traefik_v3.0.0-beta2_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Wed, 14 Jun 2023 20:12:26 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 14 Jun 2023 20:12:26 GMT
EXPOSE 80
# Wed, 14 Jun 2023 20:12:26 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 14 Jun 2023 20:12:26 GMT
CMD ["traefik"]
# Wed, 14 Jun 2023 20:12:26 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v3.0.0-beta2 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:41c5c5b38e13af18def277385607129664fb24993d262d4b601a381e776482a9`  
		Last Modified: Wed, 14 Jun 2023 18:50:19 GMT  
		Size: 2.6 MB (2633060 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:718cfe2cb66c053a8fdb09adf88b20a52f260f22abd38cba68cc2838ee33e73d`  
		Last Modified: Wed, 14 Jun 2023 20:12:46 GMT  
		Size: 666.3 KB (666349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47b2cef5f2c79471c563b3c10376140084b51c097de00e9be0b758219ab95e5c`  
		Last Modified: Wed, 14 Jun 2023 20:12:52 GMT  
		Size: 35.0 MB (34989308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66078e59ed6730404193e57cea654480d0731663c7a068349344e0a681d1c660`  
		Last Modified: Wed, 14 Jun 2023 20:12:46 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:3.0.0-beta2` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:70a1b62539b384a09d98e22bea5212f0120150377a85a599839d35897a55ef3b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.4 MB (37406948 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ebe5414a44cb1b3f5ada2c4d4477d9bb6c73103354707edb71a0adfb2138efb4`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 14 Jun 2023 20:49:10 GMT
ADD file:2b463f242cb7bf946452bb4781838348ecbe80da144fbab09f51d7e050dc68f3 in / 
# Wed, 14 Jun 2023 20:49:11 GMT
CMD ["/bin/sh"]
# Thu, 15 Jun 2023 07:10:02 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 15 Jun 2023 07:10:05 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v3.0.0-beta2/traefik_v3.0.0-beta2_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 15 Jun 2023 07:10:05 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 15 Jun 2023 07:10:05 GMT
EXPOSE 80
# Thu, 15 Jun 2023 07:10:05 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 15 Jun 2023 07:10:06 GMT
CMD ["traefik"]
# Thu, 15 Jun 2023 07:10:06 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v3.0.0-beta2 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:a147224bf413aeffbbfcdcb5104d35c647256a5c32083f4d8134f09a4e74ddeb`  
		Last Modified: Wed, 14 Jun 2023 20:49:52 GMT  
		Size: 2.7 MB (2720801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d273c78104fe60b8d6b0a1d68c0b259293bd972e3ff515bc403a8bfbff6d88a9`  
		Last Modified: Thu, 15 Jun 2023 07:10:24 GMT  
		Size: 662.3 KB (662262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2be3d50287a2f7fba1e120466ee42285469a74914da1378df40803a29c6245f3`  
		Last Modified: Thu, 15 Jun 2023 07:10:28 GMT  
		Size: 34.0 MB (34023516 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:452eba291077ce9af0d14edf868a5522679b04016d43f8a2e05b194d2618d210`  
		Last Modified: Thu, 15 Jun 2023 07:10:24 GMT  
		Size: 369.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:3.0.0-beta2` - linux; s390x

```console
$ docker pull traefik@sha256:feacc7d5c4b3a2d20dcbfc15e95e848cbc3b83820b99cafd9807db1863b65891
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.1 MB (39130249 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:af3c57f022e7ac6f998e72d571ec87f092a10f19341601105cd3f5c2b767d2ad`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 15 Jun 2023 05:22:08 GMT
ADD file:243e0553a1216040e760e1a7ce7119b10b477e081d792fa29e8c17403a8785ff in / 
# Thu, 15 Jun 2023 05:22:08 GMT
CMD ["/bin/sh"]
# Fri, 16 Jun 2023 16:39:46 GMT
RUN apk --no-cache add ca-certificates tzdata
# Fri, 16 Jun 2023 16:39:50 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v3.0.0-beta2/traefik_v3.0.0-beta2_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Fri, 16 Jun 2023 16:39:52 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Fri, 16 Jun 2023 16:39:52 GMT
EXPOSE 80
# Fri, 16 Jun 2023 16:39:52 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 16 Jun 2023 16:39:52 GMT
CMD ["traefik"]
# Fri, 16 Jun 2023 16:39:52 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v3.0.0-beta2 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:66238d49bc5bf7485c63b2671ef3c879dd2015902b151f6f5e7d178cf472c9f2`  
		Last Modified: Thu, 15 Jun 2023 05:32:59 GMT  
		Size: 2.6 MB (2608705 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42d9a3c534bf80ba9a88587c1fd786fafea714685bd2abfac3984c6ddfda55b2`  
		Last Modified: Fri, 16 Jun 2023 16:40:22 GMT  
		Size: 665.7 KB (665740 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72fef4a8a0cc5f1eea5507fd77aa05a9500cb4d1ef385312c7bcbae389046009`  
		Last Modified: Fri, 16 Jun 2023 16:40:28 GMT  
		Size: 35.9 MB (35855437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f5a752b613a2cf39692fa7636be262af8c16ac0a46e8abf8702c047ab934522`  
		Last Modified: Fri, 16 Jun 2023 16:40:22 GMT  
		Size: 367.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:3.0.0-beta2-windowsservercore-1809`

```console
$ docker pull traefik@sha256:468282899a6f9b06f9fca5ebb1a3a5bf030b45e63e0508f36f75ad7792100318
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4499; amd64

### `traefik:3.0.0-beta2-windowsservercore-1809` - windows version 10.0.17763.4499; amd64

```console
$ docker pull traefik@sha256:58a44dc3d5c4e9816d6873d753a6074c23aa7a462052f72f8fb60172ae00773b
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.7 GB (1688143673 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:01f1804410c439a02c3fbb603e3dc9c1a10922016750389db87aed22db51adb2`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Wed, 14 Jun 2023 17:39:58 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 14 Jun 2023 23:20:14 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/traefik/traefik/releases/download/v3.0.0-beta2/traefik_v3.0.0-beta2_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Wed, 14 Jun 2023 23:20:15 GMT
EXPOSE 80
# Wed, 14 Jun 2023 23:20:15 GMT
ENTRYPOINT ["/traefik"]
# Wed, 14 Jun 2023 23:20:16 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v3.0.0-beta2 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b712a9a082fd391beaa9ca7c8e6c3fda37b0ad8d29cc4663173ed973b961d342`  
		Last Modified: Wed, 14 Jun 2023 18:21:55 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a9b4e4d63720e53bc602ec5afd594ae87dc8d306b5873781d0fd3055f818c16`  
		Last Modified: Wed, 14 Jun 2023 23:21:42 GMT  
		Size: 37.5 MB (37517697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef864bbe2da9a6fc6aba62dc459a1b659d3d46ada2e3a1a04ee8b7c02a6f4e92`  
		Last Modified: Wed, 14 Jun 2023 23:21:33 GMT  
		Size: 1.4 KB (1377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2213ec09fd524be95c6a826c50e14f52e9e639e66c3572d56f438bac3cf98bab`  
		Last Modified: Wed, 14 Jun 2023 23:21:33 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58cd9c99e4865330e999c8136c9600504c563b6c37779e28663ff1421a7ac516`  
		Last Modified: Wed, 14 Jun 2023 23:21:33 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:beaufort`

```console
$ docker pull traefik@sha256:366345ddd7c17a8d273696797a375c5144e3a5242bdb39a2855baaec2bd6851c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; s390x

### `traefik:beaufort` - linux; amd64

```console
$ docker pull traefik@sha256:5f3e471200c36a65618b50719f8f467530a9895a61f87bda0bb437b5718ac327
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.6 MB (40562366 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c08e518a729607ef1142c8a57a82ab9df16bcd47e4e5a6874d07467e07a87dd0`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 14 Jun 2023 20:42:13 GMT
ADD file:4fa8e307f595ecff485113fb0ec6e2320979eaa6fb3eb467d2433771a6f016e6 in / 
# Wed, 14 Jun 2023 20:42:13 GMT
CMD ["/bin/sh"]
# Thu, 15 Jun 2023 06:27:27 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 15 Jun 2023 06:27:31 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v3.0.0-beta2/traefik_v3.0.0-beta2_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 15 Jun 2023 06:27:31 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 15 Jun 2023 06:27:31 GMT
EXPOSE 80
# Thu, 15 Jun 2023 06:27:31 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 15 Jun 2023 06:27:31 GMT
CMD ["traefik"]
# Thu, 15 Jun 2023 06:27:31 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v3.0.0-beta2 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:0cdfa0c98ed79707cd91c5dd7ebd282aa2b976d86a9e699d7fc188cdb6be390e`  
		Last Modified: Wed, 14 Jun 2023 20:42:58 GMT  
		Size: 2.8 MB (2825916 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75174169df6666c22d9a3c3085ea1eacd10478e79c70bbd53abc6cf647134b86`  
		Last Modified: Thu, 15 Jun 2023 06:27:51 GMT  
		Size: 661.2 KB (661203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4920635d165c3cb67e2ee3fd37aec68049e9730086d72999c5d926fd5a2b5bdb`  
		Last Modified: Thu, 15 Jun 2023 06:27:56 GMT  
		Size: 37.1 MB (37074878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:133801879169abc43871a5a32c77fb651e1ae90c3233a0cce11b6ead5c526c79`  
		Last Modified: Thu, 15 Jun 2023 06:27:50 GMT  
		Size: 369.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:beaufort` - linux; arm variant v6

```console
$ docker pull traefik@sha256:0e010dd7b60c3960f903b07854cae707e691496f1491f0447ca2635b5a374a6d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.3 MB (38289085 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ee0012c6d54cfd4da66d0da5e01f3dc4f70609eec928ce429e71a5efa02c96b3`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 14 Jun 2023 18:49:32 GMT
ADD file:b987db82fa4ce6e623de49a50612c1fd91c5ab2209a62a5727ab3436c2923e91 in / 
# Wed, 14 Jun 2023 18:49:32 GMT
CMD ["/bin/sh"]
# Wed, 14 Jun 2023 20:12:22 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 14 Jun 2023 20:12:26 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v3.0.0-beta2/traefik_v3.0.0-beta2_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Wed, 14 Jun 2023 20:12:26 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 14 Jun 2023 20:12:26 GMT
EXPOSE 80
# Wed, 14 Jun 2023 20:12:26 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 14 Jun 2023 20:12:26 GMT
CMD ["traefik"]
# Wed, 14 Jun 2023 20:12:26 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v3.0.0-beta2 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:41c5c5b38e13af18def277385607129664fb24993d262d4b601a381e776482a9`  
		Last Modified: Wed, 14 Jun 2023 18:50:19 GMT  
		Size: 2.6 MB (2633060 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:718cfe2cb66c053a8fdb09adf88b20a52f260f22abd38cba68cc2838ee33e73d`  
		Last Modified: Wed, 14 Jun 2023 20:12:46 GMT  
		Size: 666.3 KB (666349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47b2cef5f2c79471c563b3c10376140084b51c097de00e9be0b758219ab95e5c`  
		Last Modified: Wed, 14 Jun 2023 20:12:52 GMT  
		Size: 35.0 MB (34989308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66078e59ed6730404193e57cea654480d0731663c7a068349344e0a681d1c660`  
		Last Modified: Wed, 14 Jun 2023 20:12:46 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:beaufort` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:70a1b62539b384a09d98e22bea5212f0120150377a85a599839d35897a55ef3b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.4 MB (37406948 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ebe5414a44cb1b3f5ada2c4d4477d9bb6c73103354707edb71a0adfb2138efb4`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 14 Jun 2023 20:49:10 GMT
ADD file:2b463f242cb7bf946452bb4781838348ecbe80da144fbab09f51d7e050dc68f3 in / 
# Wed, 14 Jun 2023 20:49:11 GMT
CMD ["/bin/sh"]
# Thu, 15 Jun 2023 07:10:02 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 15 Jun 2023 07:10:05 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v3.0.0-beta2/traefik_v3.0.0-beta2_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 15 Jun 2023 07:10:05 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 15 Jun 2023 07:10:05 GMT
EXPOSE 80
# Thu, 15 Jun 2023 07:10:05 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 15 Jun 2023 07:10:06 GMT
CMD ["traefik"]
# Thu, 15 Jun 2023 07:10:06 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v3.0.0-beta2 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:a147224bf413aeffbbfcdcb5104d35c647256a5c32083f4d8134f09a4e74ddeb`  
		Last Modified: Wed, 14 Jun 2023 20:49:52 GMT  
		Size: 2.7 MB (2720801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d273c78104fe60b8d6b0a1d68c0b259293bd972e3ff515bc403a8bfbff6d88a9`  
		Last Modified: Thu, 15 Jun 2023 07:10:24 GMT  
		Size: 662.3 KB (662262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2be3d50287a2f7fba1e120466ee42285469a74914da1378df40803a29c6245f3`  
		Last Modified: Thu, 15 Jun 2023 07:10:28 GMT  
		Size: 34.0 MB (34023516 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:452eba291077ce9af0d14edf868a5522679b04016d43f8a2e05b194d2618d210`  
		Last Modified: Thu, 15 Jun 2023 07:10:24 GMT  
		Size: 369.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:beaufort` - linux; s390x

```console
$ docker pull traefik@sha256:feacc7d5c4b3a2d20dcbfc15e95e848cbc3b83820b99cafd9807db1863b65891
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.1 MB (39130249 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:af3c57f022e7ac6f998e72d571ec87f092a10f19341601105cd3f5c2b767d2ad`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 15 Jun 2023 05:22:08 GMT
ADD file:243e0553a1216040e760e1a7ce7119b10b477e081d792fa29e8c17403a8785ff in / 
# Thu, 15 Jun 2023 05:22:08 GMT
CMD ["/bin/sh"]
# Fri, 16 Jun 2023 16:39:46 GMT
RUN apk --no-cache add ca-certificates tzdata
# Fri, 16 Jun 2023 16:39:50 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v3.0.0-beta2/traefik_v3.0.0-beta2_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Fri, 16 Jun 2023 16:39:52 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Fri, 16 Jun 2023 16:39:52 GMT
EXPOSE 80
# Fri, 16 Jun 2023 16:39:52 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 16 Jun 2023 16:39:52 GMT
CMD ["traefik"]
# Fri, 16 Jun 2023 16:39:52 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v3.0.0-beta2 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:66238d49bc5bf7485c63b2671ef3c879dd2015902b151f6f5e7d178cf472c9f2`  
		Last Modified: Thu, 15 Jun 2023 05:32:59 GMT  
		Size: 2.6 MB (2608705 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42d9a3c534bf80ba9a88587c1fd786fafea714685bd2abfac3984c6ddfda55b2`  
		Last Modified: Fri, 16 Jun 2023 16:40:22 GMT  
		Size: 665.7 KB (665740 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72fef4a8a0cc5f1eea5507fd77aa05a9500cb4d1ef385312c7bcbae389046009`  
		Last Modified: Fri, 16 Jun 2023 16:40:28 GMT  
		Size: 35.9 MB (35855437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f5a752b613a2cf39692fa7636be262af8c16ac0a46e8abf8702c047ab934522`  
		Last Modified: Fri, 16 Jun 2023 16:40:22 GMT  
		Size: 367.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:beaufort-windowsservercore-1809`

```console
$ docker pull traefik@sha256:468282899a6f9b06f9fca5ebb1a3a5bf030b45e63e0508f36f75ad7792100318
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4499; amd64

### `traefik:beaufort-windowsservercore-1809` - windows version 10.0.17763.4499; amd64

```console
$ docker pull traefik@sha256:58a44dc3d5c4e9816d6873d753a6074c23aa7a462052f72f8fb60172ae00773b
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.7 GB (1688143673 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:01f1804410c439a02c3fbb603e3dc9c1a10922016750389db87aed22db51adb2`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Wed, 14 Jun 2023 17:39:58 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 14 Jun 2023 23:20:14 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/traefik/traefik/releases/download/v3.0.0-beta2/traefik_v3.0.0-beta2_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Wed, 14 Jun 2023 23:20:15 GMT
EXPOSE 80
# Wed, 14 Jun 2023 23:20:15 GMT
ENTRYPOINT ["/traefik"]
# Wed, 14 Jun 2023 23:20:16 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v3.0.0-beta2 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b712a9a082fd391beaa9ca7c8e6c3fda37b0ad8d29cc4663173ed973b961d342`  
		Last Modified: Wed, 14 Jun 2023 18:21:55 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a9b4e4d63720e53bc602ec5afd594ae87dc8d306b5873781d0fd3055f818c16`  
		Last Modified: Wed, 14 Jun 2023 23:21:42 GMT  
		Size: 37.5 MB (37517697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef864bbe2da9a6fc6aba62dc459a1b659d3d46ada2e3a1a04ee8b7c02a6f4e92`  
		Last Modified: Wed, 14 Jun 2023 23:21:33 GMT  
		Size: 1.4 KB (1377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2213ec09fd524be95c6a826c50e14f52e9e639e66c3572d56f438bac3cf98bab`  
		Last Modified: Wed, 14 Jun 2023 23:21:33 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58cd9c99e4865330e999c8136c9600504c563b6c37779e28663ff1421a7ac516`  
		Last Modified: Wed, 14 Jun 2023 23:21:33 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:latest`

```console
$ docker pull traefik@sha256:c272e8c32fb7356c2166bc5d170ab0a2c73da7bfec561234c52f255ece1dd07c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; s390x

### `traefik:latest` - linux; amd64

```console
$ docker pull traefik@sha256:79c24d0686fa0679cde49f275e694afb7ef6d182b9fe21a219463e2a6bfe4ece
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.2 MB (41246766 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a07d037aae0a48737ff74bbd136e6a809cb25af2fd7754a2168e038a5b9534eb`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 14 Jun 2023 20:41:58 GMT
ADD file:1da756d12551a0e3e793e02ef87432d69d4968937bd11bed0af215db19dd94cd in / 
# Wed, 14 Jun 2023 20:41:59 GMT
CMD ["/bin/sh"]
# Wed, 21 Jun 2023 00:26:12 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 21 Jun 2023 00:26:15 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.10.3/traefik_v2.10.3_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Wed, 21 Jun 2023 00:26:16 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 21 Jun 2023 00:26:16 GMT
EXPOSE 80
# Wed, 21 Jun 2023 00:26:16 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 21 Jun 2023 00:26:16 GMT
CMD ["traefik"]
# Wed, 21 Jun 2023 00:26:16 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.10.3 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:31e352740f534f9ad170f75378a84fe453d6156e40700b882d737a8f4a6988a3`  
		Last Modified: Wed, 14 Jun 2023 20:42:26 GMT  
		Size: 3.4 MB (3397879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b9a9b499d7ae3ed84aef77186cbd2b1ae5418ddc653e721702ec1a35fa324a3`  
		Last Modified: Wed, 21 Jun 2023 00:26:31 GMT  
		Size: 622.2 KB (622241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d581263ee7dc4ec5a72666259aadc3c7072d84df3ef862f3b3737b8392eb09d4`  
		Last Modified: Wed, 21 Jun 2023 00:26:36 GMT  
		Size: 37.2 MB (37226281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5f0f39a1a90d628163b34d2a35ff662ec098d350ce46a3737f1905c7dc2f954`  
		Last Modified: Wed, 21 Jun 2023 00:26:30 GMT  
		Size: 365.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:latest` - linux; arm variant v6

```console
$ docker pull traefik@sha256:bf02196efc8a2e8a41c9cba0363d89f7c64d294e70c7f2e36f46d2f7a1405e69
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.8 MB (38806469 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6a8dac0c0e2cda3bc1bdbd21f6b252c8cfb432270813b0e32421cdcd16a40707`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 14 Jun 2023 18:49:20 GMT
ADD file:4213782693bf27a9a6de23bc924ef0c4fb6b2d56010fc07b25f81edeba83b0d4 in / 
# Wed, 14 Jun 2023 18:49:20 GMT
CMD ["/bin/sh"]
# Tue, 20 Jun 2023 22:49:44 GMT
RUN apk --no-cache add ca-certificates tzdata
# Tue, 20 Jun 2023 22:49:48 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.10.3/traefik_v2.10.3_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Tue, 20 Jun 2023 22:49:49 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Tue, 20 Jun 2023 22:49:49 GMT
EXPOSE 80
# Tue, 20 Jun 2023 22:49:49 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 20 Jun 2023 22:49:49 GMT
CMD ["traefik"]
# Tue, 20 Jun 2023 22:49:49 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.10.3 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:7836be94d3024e2042069c1095caba0b391f70c4b3d34a0475a503239d73dfba`  
		Last Modified: Wed, 14 Jun 2023 18:49:46 GMT  
		Size: 3.1 MB (3143353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be273dc11f4147c3910cbabccdb1e28523a1cb24f3f849c4c36c5a2ce46bd092`  
		Last Modified: Tue, 20 Jun 2023 22:50:03 GMT  
		Size: 622.7 KB (622687 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:053ac18b4541fcb4b8456e7b5db6257d6201478c985190a80138c877c6b54962`  
		Last Modified: Tue, 20 Jun 2023 22:50:09 GMT  
		Size: 35.0 MB (35040063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c3b139cedf00b646032b604d4f6a681890378569bb9fff6767c64e2e5d6bdb7`  
		Last Modified: Tue, 20 Jun 2023 22:50:03 GMT  
		Size: 366.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:latest` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:3c5daac31719a3158b5ba95d98fa7987ec31a971803c9aca2dca7e02022b23e8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.0 MB (38039994 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:28c14b3be10b718677713d790e913fc0743b8c9703c0dc5d4984a30526cf53f3`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 14 Jun 2023 20:48:58 GMT
ADD file:289c2fac17119508ced527225d445747cd177111b4a0018a6b04948ecb3b5e29 in / 
# Wed, 14 Jun 2023 20:48:58 GMT
CMD ["/bin/sh"]
# Tue, 20 Jun 2023 23:21:47 GMT
RUN apk --no-cache add ca-certificates tzdata
# Tue, 20 Jun 2023 23:21:50 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.10.3/traefik_v2.10.3_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Tue, 20 Jun 2023 23:21:50 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Tue, 20 Jun 2023 23:21:50 GMT
EXPOSE 80
# Tue, 20 Jun 2023 23:21:50 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 20 Jun 2023 23:21:50 GMT
CMD ["traefik"]
# Tue, 20 Jun 2023 23:21:50 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.10.3 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:8c6d1654570f041603f4cef49c320c8f6f3e401324913009d92a19132cbf1ac0`  
		Last Modified: Wed, 14 Jun 2023 20:49:23 GMT  
		Size: 3.3 MB (3329251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b960a271861d2b8bee110ab4afb7ec842665bbbd31f1bb9c1c279cd78d925fc`  
		Last Modified: Tue, 20 Jun 2023 23:22:04 GMT  
		Size: 624.5 KB (624502 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:754fa8e2a433d2589523d839325fd39c00d1a345d3e30234db2d388fdf21d845`  
		Last Modified: Tue, 20 Jun 2023 23:22:08 GMT  
		Size: 34.1 MB (34085876 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e6c2fdac2a73f03934e5e0d484b0746a11e42421db9f59e1eec0e7550b7bf59`  
		Last Modified: Tue, 20 Jun 2023 23:22:04 GMT  
		Size: 365.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:latest` - linux; s390x

```console
$ docker pull traefik@sha256:9b2e7255584bc1bdf07b8ff66cb3c9ce52c952af2009751c311c9e793f3b3040
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.9 MB (39925281 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5eeb14a180e79a1752259e241dc5b9d14fd6eeabdc2776f52e5bca7fd723c5fd`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 15 Jun 2023 05:18:38 GMT
ADD file:a59beca78118ebf4f86cc1685237dc3a29a519401a70668da520beaa3d29eb7a in / 
# Thu, 15 Jun 2023 05:18:38 GMT
CMD ["/bin/sh"]
# Tue, 20 Jun 2023 22:49:13 GMT
RUN apk --no-cache add ca-certificates tzdata
# Tue, 20 Jun 2023 22:49:18 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.10.3/traefik_v2.10.3_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Tue, 20 Jun 2023 22:49:20 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Tue, 20 Jun 2023 22:49:20 GMT
EXPOSE 80
# Tue, 20 Jun 2023 22:49:20 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 20 Jun 2023 22:49:20 GMT
CMD ["traefik"]
# Tue, 20 Jun 2023 22:49:20 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.10.3 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:998cc98447b44e5f0fe799dce691412796ba586ab22eb7c99aebf9d45f34833b`  
		Last Modified: Thu, 15 Jun 2023 05:29:38 GMT  
		Size: 3.2 MB (3213497 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b6fdd3c34275458c3ea0a8688ec24b8c7698ce5a31715673ae57aa8dd5b0844`  
		Last Modified: Tue, 20 Jun 2023 22:49:39 GMT  
		Size: 622.8 KB (622821 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c041a673abae644852705ba64c910a0ebec6c0ea502a06264644f44da6e2e2d`  
		Last Modified: Tue, 20 Jun 2023 22:49:44 GMT  
		Size: 36.1 MB (36088597 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdef234383c44175d81f3fd1a8a0d6970aee17a833bcd7d578a690d36c46efb1`  
		Last Modified: Tue, 20 Jun 2023 22:49:39 GMT  
		Size: 366.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:saintmarcelin`

```console
$ docker pull traefik@sha256:c272e8c32fb7356c2166bc5d170ab0a2c73da7bfec561234c52f255ece1dd07c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; s390x

### `traefik:saintmarcelin` - linux; amd64

```console
$ docker pull traefik@sha256:79c24d0686fa0679cde49f275e694afb7ef6d182b9fe21a219463e2a6bfe4ece
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.2 MB (41246766 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a07d037aae0a48737ff74bbd136e6a809cb25af2fd7754a2168e038a5b9534eb`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 14 Jun 2023 20:41:58 GMT
ADD file:1da756d12551a0e3e793e02ef87432d69d4968937bd11bed0af215db19dd94cd in / 
# Wed, 14 Jun 2023 20:41:59 GMT
CMD ["/bin/sh"]
# Wed, 21 Jun 2023 00:26:12 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 21 Jun 2023 00:26:15 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.10.3/traefik_v2.10.3_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Wed, 21 Jun 2023 00:26:16 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 21 Jun 2023 00:26:16 GMT
EXPOSE 80
# Wed, 21 Jun 2023 00:26:16 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 21 Jun 2023 00:26:16 GMT
CMD ["traefik"]
# Wed, 21 Jun 2023 00:26:16 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.10.3 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:31e352740f534f9ad170f75378a84fe453d6156e40700b882d737a8f4a6988a3`  
		Last Modified: Wed, 14 Jun 2023 20:42:26 GMT  
		Size: 3.4 MB (3397879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b9a9b499d7ae3ed84aef77186cbd2b1ae5418ddc653e721702ec1a35fa324a3`  
		Last Modified: Wed, 21 Jun 2023 00:26:31 GMT  
		Size: 622.2 KB (622241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d581263ee7dc4ec5a72666259aadc3c7072d84df3ef862f3b3737b8392eb09d4`  
		Last Modified: Wed, 21 Jun 2023 00:26:36 GMT  
		Size: 37.2 MB (37226281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5f0f39a1a90d628163b34d2a35ff662ec098d350ce46a3737f1905c7dc2f954`  
		Last Modified: Wed, 21 Jun 2023 00:26:30 GMT  
		Size: 365.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:saintmarcelin` - linux; arm variant v6

```console
$ docker pull traefik@sha256:bf02196efc8a2e8a41c9cba0363d89f7c64d294e70c7f2e36f46d2f7a1405e69
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.8 MB (38806469 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6a8dac0c0e2cda3bc1bdbd21f6b252c8cfb432270813b0e32421cdcd16a40707`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 14 Jun 2023 18:49:20 GMT
ADD file:4213782693bf27a9a6de23bc924ef0c4fb6b2d56010fc07b25f81edeba83b0d4 in / 
# Wed, 14 Jun 2023 18:49:20 GMT
CMD ["/bin/sh"]
# Tue, 20 Jun 2023 22:49:44 GMT
RUN apk --no-cache add ca-certificates tzdata
# Tue, 20 Jun 2023 22:49:48 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.10.3/traefik_v2.10.3_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Tue, 20 Jun 2023 22:49:49 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Tue, 20 Jun 2023 22:49:49 GMT
EXPOSE 80
# Tue, 20 Jun 2023 22:49:49 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 20 Jun 2023 22:49:49 GMT
CMD ["traefik"]
# Tue, 20 Jun 2023 22:49:49 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.10.3 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:7836be94d3024e2042069c1095caba0b391f70c4b3d34a0475a503239d73dfba`  
		Last Modified: Wed, 14 Jun 2023 18:49:46 GMT  
		Size: 3.1 MB (3143353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be273dc11f4147c3910cbabccdb1e28523a1cb24f3f849c4c36c5a2ce46bd092`  
		Last Modified: Tue, 20 Jun 2023 22:50:03 GMT  
		Size: 622.7 KB (622687 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:053ac18b4541fcb4b8456e7b5db6257d6201478c985190a80138c877c6b54962`  
		Last Modified: Tue, 20 Jun 2023 22:50:09 GMT  
		Size: 35.0 MB (35040063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c3b139cedf00b646032b604d4f6a681890378569bb9fff6767c64e2e5d6bdb7`  
		Last Modified: Tue, 20 Jun 2023 22:50:03 GMT  
		Size: 366.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:saintmarcelin` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:3c5daac31719a3158b5ba95d98fa7987ec31a971803c9aca2dca7e02022b23e8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.0 MB (38039994 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:28c14b3be10b718677713d790e913fc0743b8c9703c0dc5d4984a30526cf53f3`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 14 Jun 2023 20:48:58 GMT
ADD file:289c2fac17119508ced527225d445747cd177111b4a0018a6b04948ecb3b5e29 in / 
# Wed, 14 Jun 2023 20:48:58 GMT
CMD ["/bin/sh"]
# Tue, 20 Jun 2023 23:21:47 GMT
RUN apk --no-cache add ca-certificates tzdata
# Tue, 20 Jun 2023 23:21:50 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.10.3/traefik_v2.10.3_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Tue, 20 Jun 2023 23:21:50 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Tue, 20 Jun 2023 23:21:50 GMT
EXPOSE 80
# Tue, 20 Jun 2023 23:21:50 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 20 Jun 2023 23:21:50 GMT
CMD ["traefik"]
# Tue, 20 Jun 2023 23:21:50 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.10.3 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:8c6d1654570f041603f4cef49c320c8f6f3e401324913009d92a19132cbf1ac0`  
		Last Modified: Wed, 14 Jun 2023 20:49:23 GMT  
		Size: 3.3 MB (3329251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b960a271861d2b8bee110ab4afb7ec842665bbbd31f1bb9c1c279cd78d925fc`  
		Last Modified: Tue, 20 Jun 2023 23:22:04 GMT  
		Size: 624.5 KB (624502 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:754fa8e2a433d2589523d839325fd39c00d1a345d3e30234db2d388fdf21d845`  
		Last Modified: Tue, 20 Jun 2023 23:22:08 GMT  
		Size: 34.1 MB (34085876 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e6c2fdac2a73f03934e5e0d484b0746a11e42421db9f59e1eec0e7550b7bf59`  
		Last Modified: Tue, 20 Jun 2023 23:22:04 GMT  
		Size: 365.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:saintmarcelin` - linux; s390x

```console
$ docker pull traefik@sha256:9b2e7255584bc1bdf07b8ff66cb3c9ce52c952af2009751c311c9e793f3b3040
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.9 MB (39925281 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5eeb14a180e79a1752259e241dc5b9d14fd6eeabdc2776f52e5bca7fd723c5fd`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 15 Jun 2023 05:18:38 GMT
ADD file:a59beca78118ebf4f86cc1685237dc3a29a519401a70668da520beaa3d29eb7a in / 
# Thu, 15 Jun 2023 05:18:38 GMT
CMD ["/bin/sh"]
# Tue, 20 Jun 2023 22:49:13 GMT
RUN apk --no-cache add ca-certificates tzdata
# Tue, 20 Jun 2023 22:49:18 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.10.3/traefik_v2.10.3_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Tue, 20 Jun 2023 22:49:20 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Tue, 20 Jun 2023 22:49:20 GMT
EXPOSE 80
# Tue, 20 Jun 2023 22:49:20 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 20 Jun 2023 22:49:20 GMT
CMD ["traefik"]
# Tue, 20 Jun 2023 22:49:20 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.10.3 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:998cc98447b44e5f0fe799dce691412796ba586ab22eb7c99aebf9d45f34833b`  
		Last Modified: Thu, 15 Jun 2023 05:29:38 GMT  
		Size: 3.2 MB (3213497 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b6fdd3c34275458c3ea0a8688ec24b8c7698ce5a31715673ae57aa8dd5b0844`  
		Last Modified: Tue, 20 Jun 2023 22:49:39 GMT  
		Size: 622.8 KB (622821 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c041a673abae644852705ba64c910a0ebec6c0ea502a06264644f44da6e2e2d`  
		Last Modified: Tue, 20 Jun 2023 22:49:44 GMT  
		Size: 36.1 MB (36088597 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdef234383c44175d81f3fd1a8a0d6970aee17a833bcd7d578a690d36c46efb1`  
		Last Modified: Tue, 20 Jun 2023 22:49:39 GMT  
		Size: 366.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:saintmarcelin-windowsservercore-1809`

```console
$ docker pull traefik@sha256:dc03c1897e7fa9697744289086dfd429fc4b22694446bb29881671bd63335f55
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4499; amd64

### `traefik:saintmarcelin-windowsservercore-1809` - windows version 10.0.17763.4499; amd64

```console
$ docker pull traefik@sha256:b61a301ec003fdfb61afa059050468dfd19e329b91adc04b989378307c01e5b9
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.7 GB (1688297643 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c40b4425780339ae5ed986b0312fde45ee26d18c675994fa07879d3ba8ba802f`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Wed, 14 Jun 2023 17:39:58 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 20 Jun 2023 23:18:02 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/traefik/traefik/releases/download/v2.10.3/traefik_v2.10.3_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Tue, 20 Jun 2023 23:18:04 GMT
EXPOSE 80
# Tue, 20 Jun 2023 23:18:05 GMT
ENTRYPOINT ["/traefik"]
# Tue, 20 Jun 2023 23:18:06 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.10.3 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b712a9a082fd391beaa9ca7c8e6c3fda37b0ad8d29cc4663173ed973b961d342`  
		Last Modified: Wed, 14 Jun 2023 18:21:55 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6ae7661d409041f0b91655d0629e3756f67688eabbeb2d46f7c44b9e110614a`  
		Last Modified: Tue, 20 Jun 2023 23:18:40 GMT  
		Size: 37.7 MB (37671801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eda08f2fb0ae872eb7d6aee508ca42acf0aa7d71c4cc8b22b2acd32a8dac9307`  
		Last Modified: Tue, 20 Jun 2023 23:18:30 GMT  
		Size: 1.3 KB (1301 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7fc4c49780e0c6b8e9d6e2577ae7f3597396920dbd9c744ace14c79b3db639e`  
		Last Modified: Tue, 20 Jun 2023 23:18:30 GMT  
		Size: 1.4 KB (1362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7546eab39455c2a7df3171964211f93193cc95597a50435a4c7e5e3ee22b6f2`  
		Last Modified: Tue, 20 Jun 2023 23:18:30 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v2.10`

```console
$ docker pull traefik@sha256:c272e8c32fb7356c2166bc5d170ab0a2c73da7bfec561234c52f255ece1dd07c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; s390x

### `traefik:v2.10` - linux; amd64

```console
$ docker pull traefik@sha256:79c24d0686fa0679cde49f275e694afb7ef6d182b9fe21a219463e2a6bfe4ece
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.2 MB (41246766 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a07d037aae0a48737ff74bbd136e6a809cb25af2fd7754a2168e038a5b9534eb`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 14 Jun 2023 20:41:58 GMT
ADD file:1da756d12551a0e3e793e02ef87432d69d4968937bd11bed0af215db19dd94cd in / 
# Wed, 14 Jun 2023 20:41:59 GMT
CMD ["/bin/sh"]
# Wed, 21 Jun 2023 00:26:12 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 21 Jun 2023 00:26:15 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.10.3/traefik_v2.10.3_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Wed, 21 Jun 2023 00:26:16 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 21 Jun 2023 00:26:16 GMT
EXPOSE 80
# Wed, 21 Jun 2023 00:26:16 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 21 Jun 2023 00:26:16 GMT
CMD ["traefik"]
# Wed, 21 Jun 2023 00:26:16 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.10.3 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:31e352740f534f9ad170f75378a84fe453d6156e40700b882d737a8f4a6988a3`  
		Last Modified: Wed, 14 Jun 2023 20:42:26 GMT  
		Size: 3.4 MB (3397879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b9a9b499d7ae3ed84aef77186cbd2b1ae5418ddc653e721702ec1a35fa324a3`  
		Last Modified: Wed, 21 Jun 2023 00:26:31 GMT  
		Size: 622.2 KB (622241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d581263ee7dc4ec5a72666259aadc3c7072d84df3ef862f3b3737b8392eb09d4`  
		Last Modified: Wed, 21 Jun 2023 00:26:36 GMT  
		Size: 37.2 MB (37226281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5f0f39a1a90d628163b34d2a35ff662ec098d350ce46a3737f1905c7dc2f954`  
		Last Modified: Wed, 21 Jun 2023 00:26:30 GMT  
		Size: 365.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v2.10` - linux; arm variant v6

```console
$ docker pull traefik@sha256:bf02196efc8a2e8a41c9cba0363d89f7c64d294e70c7f2e36f46d2f7a1405e69
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.8 MB (38806469 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6a8dac0c0e2cda3bc1bdbd21f6b252c8cfb432270813b0e32421cdcd16a40707`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 14 Jun 2023 18:49:20 GMT
ADD file:4213782693bf27a9a6de23bc924ef0c4fb6b2d56010fc07b25f81edeba83b0d4 in / 
# Wed, 14 Jun 2023 18:49:20 GMT
CMD ["/bin/sh"]
# Tue, 20 Jun 2023 22:49:44 GMT
RUN apk --no-cache add ca-certificates tzdata
# Tue, 20 Jun 2023 22:49:48 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.10.3/traefik_v2.10.3_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Tue, 20 Jun 2023 22:49:49 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Tue, 20 Jun 2023 22:49:49 GMT
EXPOSE 80
# Tue, 20 Jun 2023 22:49:49 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 20 Jun 2023 22:49:49 GMT
CMD ["traefik"]
# Tue, 20 Jun 2023 22:49:49 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.10.3 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:7836be94d3024e2042069c1095caba0b391f70c4b3d34a0475a503239d73dfba`  
		Last Modified: Wed, 14 Jun 2023 18:49:46 GMT  
		Size: 3.1 MB (3143353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be273dc11f4147c3910cbabccdb1e28523a1cb24f3f849c4c36c5a2ce46bd092`  
		Last Modified: Tue, 20 Jun 2023 22:50:03 GMT  
		Size: 622.7 KB (622687 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:053ac18b4541fcb4b8456e7b5db6257d6201478c985190a80138c877c6b54962`  
		Last Modified: Tue, 20 Jun 2023 22:50:09 GMT  
		Size: 35.0 MB (35040063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c3b139cedf00b646032b604d4f6a681890378569bb9fff6767c64e2e5d6bdb7`  
		Last Modified: Tue, 20 Jun 2023 22:50:03 GMT  
		Size: 366.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v2.10` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:3c5daac31719a3158b5ba95d98fa7987ec31a971803c9aca2dca7e02022b23e8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.0 MB (38039994 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:28c14b3be10b718677713d790e913fc0743b8c9703c0dc5d4984a30526cf53f3`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 14 Jun 2023 20:48:58 GMT
ADD file:289c2fac17119508ced527225d445747cd177111b4a0018a6b04948ecb3b5e29 in / 
# Wed, 14 Jun 2023 20:48:58 GMT
CMD ["/bin/sh"]
# Tue, 20 Jun 2023 23:21:47 GMT
RUN apk --no-cache add ca-certificates tzdata
# Tue, 20 Jun 2023 23:21:50 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.10.3/traefik_v2.10.3_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Tue, 20 Jun 2023 23:21:50 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Tue, 20 Jun 2023 23:21:50 GMT
EXPOSE 80
# Tue, 20 Jun 2023 23:21:50 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 20 Jun 2023 23:21:50 GMT
CMD ["traefik"]
# Tue, 20 Jun 2023 23:21:50 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.10.3 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:8c6d1654570f041603f4cef49c320c8f6f3e401324913009d92a19132cbf1ac0`  
		Last Modified: Wed, 14 Jun 2023 20:49:23 GMT  
		Size: 3.3 MB (3329251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b960a271861d2b8bee110ab4afb7ec842665bbbd31f1bb9c1c279cd78d925fc`  
		Last Modified: Tue, 20 Jun 2023 23:22:04 GMT  
		Size: 624.5 KB (624502 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:754fa8e2a433d2589523d839325fd39c00d1a345d3e30234db2d388fdf21d845`  
		Last Modified: Tue, 20 Jun 2023 23:22:08 GMT  
		Size: 34.1 MB (34085876 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e6c2fdac2a73f03934e5e0d484b0746a11e42421db9f59e1eec0e7550b7bf59`  
		Last Modified: Tue, 20 Jun 2023 23:22:04 GMT  
		Size: 365.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v2.10` - linux; s390x

```console
$ docker pull traefik@sha256:9b2e7255584bc1bdf07b8ff66cb3c9ce52c952af2009751c311c9e793f3b3040
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.9 MB (39925281 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5eeb14a180e79a1752259e241dc5b9d14fd6eeabdc2776f52e5bca7fd723c5fd`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 15 Jun 2023 05:18:38 GMT
ADD file:a59beca78118ebf4f86cc1685237dc3a29a519401a70668da520beaa3d29eb7a in / 
# Thu, 15 Jun 2023 05:18:38 GMT
CMD ["/bin/sh"]
# Tue, 20 Jun 2023 22:49:13 GMT
RUN apk --no-cache add ca-certificates tzdata
# Tue, 20 Jun 2023 22:49:18 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.10.3/traefik_v2.10.3_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Tue, 20 Jun 2023 22:49:20 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Tue, 20 Jun 2023 22:49:20 GMT
EXPOSE 80
# Tue, 20 Jun 2023 22:49:20 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 20 Jun 2023 22:49:20 GMT
CMD ["traefik"]
# Tue, 20 Jun 2023 22:49:20 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.10.3 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:998cc98447b44e5f0fe799dce691412796ba586ab22eb7c99aebf9d45f34833b`  
		Last Modified: Thu, 15 Jun 2023 05:29:38 GMT  
		Size: 3.2 MB (3213497 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b6fdd3c34275458c3ea0a8688ec24b8c7698ce5a31715673ae57aa8dd5b0844`  
		Last Modified: Tue, 20 Jun 2023 22:49:39 GMT  
		Size: 622.8 KB (622821 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c041a673abae644852705ba64c910a0ebec6c0ea502a06264644f44da6e2e2d`  
		Last Modified: Tue, 20 Jun 2023 22:49:44 GMT  
		Size: 36.1 MB (36088597 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdef234383c44175d81f3fd1a8a0d6970aee17a833bcd7d578a690d36c46efb1`  
		Last Modified: Tue, 20 Jun 2023 22:49:39 GMT  
		Size: 366.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v2.10-windowsservercore-1809`

```console
$ docker pull traefik@sha256:dc03c1897e7fa9697744289086dfd429fc4b22694446bb29881671bd63335f55
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4499; amd64

### `traefik:v2.10-windowsservercore-1809` - windows version 10.0.17763.4499; amd64

```console
$ docker pull traefik@sha256:b61a301ec003fdfb61afa059050468dfd19e329b91adc04b989378307c01e5b9
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.7 GB (1688297643 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c40b4425780339ae5ed986b0312fde45ee26d18c675994fa07879d3ba8ba802f`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Wed, 14 Jun 2023 17:39:58 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 20 Jun 2023 23:18:02 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/traefik/traefik/releases/download/v2.10.3/traefik_v2.10.3_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Tue, 20 Jun 2023 23:18:04 GMT
EXPOSE 80
# Tue, 20 Jun 2023 23:18:05 GMT
ENTRYPOINT ["/traefik"]
# Tue, 20 Jun 2023 23:18:06 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.10.3 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b712a9a082fd391beaa9ca7c8e6c3fda37b0ad8d29cc4663173ed973b961d342`  
		Last Modified: Wed, 14 Jun 2023 18:21:55 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6ae7661d409041f0b91655d0629e3756f67688eabbeb2d46f7c44b9e110614a`  
		Last Modified: Tue, 20 Jun 2023 23:18:40 GMT  
		Size: 37.7 MB (37671801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eda08f2fb0ae872eb7d6aee508ca42acf0aa7d71c4cc8b22b2acd32a8dac9307`  
		Last Modified: Tue, 20 Jun 2023 23:18:30 GMT  
		Size: 1.3 KB (1301 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7fc4c49780e0c6b8e9d6e2577ae7f3597396920dbd9c744ace14c79b3db639e`  
		Last Modified: Tue, 20 Jun 2023 23:18:30 GMT  
		Size: 1.4 KB (1362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7546eab39455c2a7df3171964211f93193cc95597a50435a4c7e5e3ee22b6f2`  
		Last Modified: Tue, 20 Jun 2023 23:18:30 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v2.10.3`

```console
$ docker pull traefik@sha256:c272e8c32fb7356c2166bc5d170ab0a2c73da7bfec561234c52f255ece1dd07c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; s390x

### `traefik:v2.10.3` - linux; amd64

```console
$ docker pull traefik@sha256:79c24d0686fa0679cde49f275e694afb7ef6d182b9fe21a219463e2a6bfe4ece
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.2 MB (41246766 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a07d037aae0a48737ff74bbd136e6a809cb25af2fd7754a2168e038a5b9534eb`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 14 Jun 2023 20:41:58 GMT
ADD file:1da756d12551a0e3e793e02ef87432d69d4968937bd11bed0af215db19dd94cd in / 
# Wed, 14 Jun 2023 20:41:59 GMT
CMD ["/bin/sh"]
# Wed, 21 Jun 2023 00:26:12 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 21 Jun 2023 00:26:15 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.10.3/traefik_v2.10.3_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Wed, 21 Jun 2023 00:26:16 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 21 Jun 2023 00:26:16 GMT
EXPOSE 80
# Wed, 21 Jun 2023 00:26:16 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 21 Jun 2023 00:26:16 GMT
CMD ["traefik"]
# Wed, 21 Jun 2023 00:26:16 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.10.3 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:31e352740f534f9ad170f75378a84fe453d6156e40700b882d737a8f4a6988a3`  
		Last Modified: Wed, 14 Jun 2023 20:42:26 GMT  
		Size: 3.4 MB (3397879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b9a9b499d7ae3ed84aef77186cbd2b1ae5418ddc653e721702ec1a35fa324a3`  
		Last Modified: Wed, 21 Jun 2023 00:26:31 GMT  
		Size: 622.2 KB (622241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d581263ee7dc4ec5a72666259aadc3c7072d84df3ef862f3b3737b8392eb09d4`  
		Last Modified: Wed, 21 Jun 2023 00:26:36 GMT  
		Size: 37.2 MB (37226281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5f0f39a1a90d628163b34d2a35ff662ec098d350ce46a3737f1905c7dc2f954`  
		Last Modified: Wed, 21 Jun 2023 00:26:30 GMT  
		Size: 365.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v2.10.3` - linux; arm variant v6

```console
$ docker pull traefik@sha256:bf02196efc8a2e8a41c9cba0363d89f7c64d294e70c7f2e36f46d2f7a1405e69
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.8 MB (38806469 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6a8dac0c0e2cda3bc1bdbd21f6b252c8cfb432270813b0e32421cdcd16a40707`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 14 Jun 2023 18:49:20 GMT
ADD file:4213782693bf27a9a6de23bc924ef0c4fb6b2d56010fc07b25f81edeba83b0d4 in / 
# Wed, 14 Jun 2023 18:49:20 GMT
CMD ["/bin/sh"]
# Tue, 20 Jun 2023 22:49:44 GMT
RUN apk --no-cache add ca-certificates tzdata
# Tue, 20 Jun 2023 22:49:48 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.10.3/traefik_v2.10.3_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Tue, 20 Jun 2023 22:49:49 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Tue, 20 Jun 2023 22:49:49 GMT
EXPOSE 80
# Tue, 20 Jun 2023 22:49:49 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 20 Jun 2023 22:49:49 GMT
CMD ["traefik"]
# Tue, 20 Jun 2023 22:49:49 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.10.3 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:7836be94d3024e2042069c1095caba0b391f70c4b3d34a0475a503239d73dfba`  
		Last Modified: Wed, 14 Jun 2023 18:49:46 GMT  
		Size: 3.1 MB (3143353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be273dc11f4147c3910cbabccdb1e28523a1cb24f3f849c4c36c5a2ce46bd092`  
		Last Modified: Tue, 20 Jun 2023 22:50:03 GMT  
		Size: 622.7 KB (622687 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:053ac18b4541fcb4b8456e7b5db6257d6201478c985190a80138c877c6b54962`  
		Last Modified: Tue, 20 Jun 2023 22:50:09 GMT  
		Size: 35.0 MB (35040063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c3b139cedf00b646032b604d4f6a681890378569bb9fff6767c64e2e5d6bdb7`  
		Last Modified: Tue, 20 Jun 2023 22:50:03 GMT  
		Size: 366.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v2.10.3` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:3c5daac31719a3158b5ba95d98fa7987ec31a971803c9aca2dca7e02022b23e8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.0 MB (38039994 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:28c14b3be10b718677713d790e913fc0743b8c9703c0dc5d4984a30526cf53f3`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 14 Jun 2023 20:48:58 GMT
ADD file:289c2fac17119508ced527225d445747cd177111b4a0018a6b04948ecb3b5e29 in / 
# Wed, 14 Jun 2023 20:48:58 GMT
CMD ["/bin/sh"]
# Tue, 20 Jun 2023 23:21:47 GMT
RUN apk --no-cache add ca-certificates tzdata
# Tue, 20 Jun 2023 23:21:50 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.10.3/traefik_v2.10.3_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Tue, 20 Jun 2023 23:21:50 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Tue, 20 Jun 2023 23:21:50 GMT
EXPOSE 80
# Tue, 20 Jun 2023 23:21:50 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 20 Jun 2023 23:21:50 GMT
CMD ["traefik"]
# Tue, 20 Jun 2023 23:21:50 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.10.3 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:8c6d1654570f041603f4cef49c320c8f6f3e401324913009d92a19132cbf1ac0`  
		Last Modified: Wed, 14 Jun 2023 20:49:23 GMT  
		Size: 3.3 MB (3329251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b960a271861d2b8bee110ab4afb7ec842665bbbd31f1bb9c1c279cd78d925fc`  
		Last Modified: Tue, 20 Jun 2023 23:22:04 GMT  
		Size: 624.5 KB (624502 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:754fa8e2a433d2589523d839325fd39c00d1a345d3e30234db2d388fdf21d845`  
		Last Modified: Tue, 20 Jun 2023 23:22:08 GMT  
		Size: 34.1 MB (34085876 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e6c2fdac2a73f03934e5e0d484b0746a11e42421db9f59e1eec0e7550b7bf59`  
		Last Modified: Tue, 20 Jun 2023 23:22:04 GMT  
		Size: 365.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v2.10.3` - linux; s390x

```console
$ docker pull traefik@sha256:9b2e7255584bc1bdf07b8ff66cb3c9ce52c952af2009751c311c9e793f3b3040
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.9 MB (39925281 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5eeb14a180e79a1752259e241dc5b9d14fd6eeabdc2776f52e5bca7fd723c5fd`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 15 Jun 2023 05:18:38 GMT
ADD file:a59beca78118ebf4f86cc1685237dc3a29a519401a70668da520beaa3d29eb7a in / 
# Thu, 15 Jun 2023 05:18:38 GMT
CMD ["/bin/sh"]
# Tue, 20 Jun 2023 22:49:13 GMT
RUN apk --no-cache add ca-certificates tzdata
# Tue, 20 Jun 2023 22:49:18 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.10.3/traefik_v2.10.3_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Tue, 20 Jun 2023 22:49:20 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Tue, 20 Jun 2023 22:49:20 GMT
EXPOSE 80
# Tue, 20 Jun 2023 22:49:20 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 20 Jun 2023 22:49:20 GMT
CMD ["traefik"]
# Tue, 20 Jun 2023 22:49:20 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.10.3 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:998cc98447b44e5f0fe799dce691412796ba586ab22eb7c99aebf9d45f34833b`  
		Last Modified: Thu, 15 Jun 2023 05:29:38 GMT  
		Size: 3.2 MB (3213497 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b6fdd3c34275458c3ea0a8688ec24b8c7698ce5a31715673ae57aa8dd5b0844`  
		Last Modified: Tue, 20 Jun 2023 22:49:39 GMT  
		Size: 622.8 KB (622821 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c041a673abae644852705ba64c910a0ebec6c0ea502a06264644f44da6e2e2d`  
		Last Modified: Tue, 20 Jun 2023 22:49:44 GMT  
		Size: 36.1 MB (36088597 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdef234383c44175d81f3fd1a8a0d6970aee17a833bcd7d578a690d36c46efb1`  
		Last Modified: Tue, 20 Jun 2023 22:49:39 GMT  
		Size: 366.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v2.10.3-windowsservercore-1809`

```console
$ docker pull traefik@sha256:dc03c1897e7fa9697744289086dfd429fc4b22694446bb29881671bd63335f55
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4499; amd64

### `traefik:v2.10.3-windowsservercore-1809` - windows version 10.0.17763.4499; amd64

```console
$ docker pull traefik@sha256:b61a301ec003fdfb61afa059050468dfd19e329b91adc04b989378307c01e5b9
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.7 GB (1688297643 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c40b4425780339ae5ed986b0312fde45ee26d18c675994fa07879d3ba8ba802f`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Wed, 14 Jun 2023 17:39:58 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 20 Jun 2023 23:18:02 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/traefik/traefik/releases/download/v2.10.3/traefik_v2.10.3_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Tue, 20 Jun 2023 23:18:04 GMT
EXPOSE 80
# Tue, 20 Jun 2023 23:18:05 GMT
ENTRYPOINT ["/traefik"]
# Tue, 20 Jun 2023 23:18:06 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.10.3 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b712a9a082fd391beaa9ca7c8e6c3fda37b0ad8d29cc4663173ed973b961d342`  
		Last Modified: Wed, 14 Jun 2023 18:21:55 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6ae7661d409041f0b91655d0629e3756f67688eabbeb2d46f7c44b9e110614a`  
		Last Modified: Tue, 20 Jun 2023 23:18:40 GMT  
		Size: 37.7 MB (37671801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eda08f2fb0ae872eb7d6aee508ca42acf0aa7d71c4cc8b22b2acd32a8dac9307`  
		Last Modified: Tue, 20 Jun 2023 23:18:30 GMT  
		Size: 1.3 KB (1301 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7fc4c49780e0c6b8e9d6e2577ae7f3597396920dbd9c744ace14c79b3db639e`  
		Last Modified: Tue, 20 Jun 2023 23:18:30 GMT  
		Size: 1.4 KB (1362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7546eab39455c2a7df3171964211f93193cc95597a50435a4c7e5e3ee22b6f2`  
		Last Modified: Tue, 20 Jun 2023 23:18:30 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v3.0`

```console
$ docker pull traefik@sha256:366345ddd7c17a8d273696797a375c5144e3a5242bdb39a2855baaec2bd6851c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; s390x

### `traefik:v3.0` - linux; amd64

```console
$ docker pull traefik@sha256:5f3e471200c36a65618b50719f8f467530a9895a61f87bda0bb437b5718ac327
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.6 MB (40562366 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c08e518a729607ef1142c8a57a82ab9df16bcd47e4e5a6874d07467e07a87dd0`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 14 Jun 2023 20:42:13 GMT
ADD file:4fa8e307f595ecff485113fb0ec6e2320979eaa6fb3eb467d2433771a6f016e6 in / 
# Wed, 14 Jun 2023 20:42:13 GMT
CMD ["/bin/sh"]
# Thu, 15 Jun 2023 06:27:27 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 15 Jun 2023 06:27:31 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v3.0.0-beta2/traefik_v3.0.0-beta2_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 15 Jun 2023 06:27:31 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 15 Jun 2023 06:27:31 GMT
EXPOSE 80
# Thu, 15 Jun 2023 06:27:31 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 15 Jun 2023 06:27:31 GMT
CMD ["traefik"]
# Thu, 15 Jun 2023 06:27:31 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v3.0.0-beta2 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:0cdfa0c98ed79707cd91c5dd7ebd282aa2b976d86a9e699d7fc188cdb6be390e`  
		Last Modified: Wed, 14 Jun 2023 20:42:58 GMT  
		Size: 2.8 MB (2825916 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75174169df6666c22d9a3c3085ea1eacd10478e79c70bbd53abc6cf647134b86`  
		Last Modified: Thu, 15 Jun 2023 06:27:51 GMT  
		Size: 661.2 KB (661203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4920635d165c3cb67e2ee3fd37aec68049e9730086d72999c5d926fd5a2b5bdb`  
		Last Modified: Thu, 15 Jun 2023 06:27:56 GMT  
		Size: 37.1 MB (37074878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:133801879169abc43871a5a32c77fb651e1ae90c3233a0cce11b6ead5c526c79`  
		Last Modified: Thu, 15 Jun 2023 06:27:50 GMT  
		Size: 369.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v3.0` - linux; arm variant v6

```console
$ docker pull traefik@sha256:0e010dd7b60c3960f903b07854cae707e691496f1491f0447ca2635b5a374a6d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.3 MB (38289085 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ee0012c6d54cfd4da66d0da5e01f3dc4f70609eec928ce429e71a5efa02c96b3`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 14 Jun 2023 18:49:32 GMT
ADD file:b987db82fa4ce6e623de49a50612c1fd91c5ab2209a62a5727ab3436c2923e91 in / 
# Wed, 14 Jun 2023 18:49:32 GMT
CMD ["/bin/sh"]
# Wed, 14 Jun 2023 20:12:22 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 14 Jun 2023 20:12:26 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v3.0.0-beta2/traefik_v3.0.0-beta2_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Wed, 14 Jun 2023 20:12:26 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 14 Jun 2023 20:12:26 GMT
EXPOSE 80
# Wed, 14 Jun 2023 20:12:26 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 14 Jun 2023 20:12:26 GMT
CMD ["traefik"]
# Wed, 14 Jun 2023 20:12:26 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v3.0.0-beta2 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:41c5c5b38e13af18def277385607129664fb24993d262d4b601a381e776482a9`  
		Last Modified: Wed, 14 Jun 2023 18:50:19 GMT  
		Size: 2.6 MB (2633060 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:718cfe2cb66c053a8fdb09adf88b20a52f260f22abd38cba68cc2838ee33e73d`  
		Last Modified: Wed, 14 Jun 2023 20:12:46 GMT  
		Size: 666.3 KB (666349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47b2cef5f2c79471c563b3c10376140084b51c097de00e9be0b758219ab95e5c`  
		Last Modified: Wed, 14 Jun 2023 20:12:52 GMT  
		Size: 35.0 MB (34989308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66078e59ed6730404193e57cea654480d0731663c7a068349344e0a681d1c660`  
		Last Modified: Wed, 14 Jun 2023 20:12:46 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v3.0` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:70a1b62539b384a09d98e22bea5212f0120150377a85a599839d35897a55ef3b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.4 MB (37406948 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ebe5414a44cb1b3f5ada2c4d4477d9bb6c73103354707edb71a0adfb2138efb4`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 14 Jun 2023 20:49:10 GMT
ADD file:2b463f242cb7bf946452bb4781838348ecbe80da144fbab09f51d7e050dc68f3 in / 
# Wed, 14 Jun 2023 20:49:11 GMT
CMD ["/bin/sh"]
# Thu, 15 Jun 2023 07:10:02 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 15 Jun 2023 07:10:05 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v3.0.0-beta2/traefik_v3.0.0-beta2_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 15 Jun 2023 07:10:05 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 15 Jun 2023 07:10:05 GMT
EXPOSE 80
# Thu, 15 Jun 2023 07:10:05 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 15 Jun 2023 07:10:06 GMT
CMD ["traefik"]
# Thu, 15 Jun 2023 07:10:06 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v3.0.0-beta2 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:a147224bf413aeffbbfcdcb5104d35c647256a5c32083f4d8134f09a4e74ddeb`  
		Last Modified: Wed, 14 Jun 2023 20:49:52 GMT  
		Size: 2.7 MB (2720801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d273c78104fe60b8d6b0a1d68c0b259293bd972e3ff515bc403a8bfbff6d88a9`  
		Last Modified: Thu, 15 Jun 2023 07:10:24 GMT  
		Size: 662.3 KB (662262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2be3d50287a2f7fba1e120466ee42285469a74914da1378df40803a29c6245f3`  
		Last Modified: Thu, 15 Jun 2023 07:10:28 GMT  
		Size: 34.0 MB (34023516 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:452eba291077ce9af0d14edf868a5522679b04016d43f8a2e05b194d2618d210`  
		Last Modified: Thu, 15 Jun 2023 07:10:24 GMT  
		Size: 369.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v3.0` - linux; s390x

```console
$ docker pull traefik@sha256:feacc7d5c4b3a2d20dcbfc15e95e848cbc3b83820b99cafd9807db1863b65891
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.1 MB (39130249 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:af3c57f022e7ac6f998e72d571ec87f092a10f19341601105cd3f5c2b767d2ad`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 15 Jun 2023 05:22:08 GMT
ADD file:243e0553a1216040e760e1a7ce7119b10b477e081d792fa29e8c17403a8785ff in / 
# Thu, 15 Jun 2023 05:22:08 GMT
CMD ["/bin/sh"]
# Fri, 16 Jun 2023 16:39:46 GMT
RUN apk --no-cache add ca-certificates tzdata
# Fri, 16 Jun 2023 16:39:50 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v3.0.0-beta2/traefik_v3.0.0-beta2_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Fri, 16 Jun 2023 16:39:52 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Fri, 16 Jun 2023 16:39:52 GMT
EXPOSE 80
# Fri, 16 Jun 2023 16:39:52 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 16 Jun 2023 16:39:52 GMT
CMD ["traefik"]
# Fri, 16 Jun 2023 16:39:52 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v3.0.0-beta2 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:66238d49bc5bf7485c63b2671ef3c879dd2015902b151f6f5e7d178cf472c9f2`  
		Last Modified: Thu, 15 Jun 2023 05:32:59 GMT  
		Size: 2.6 MB (2608705 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42d9a3c534bf80ba9a88587c1fd786fafea714685bd2abfac3984c6ddfda55b2`  
		Last Modified: Fri, 16 Jun 2023 16:40:22 GMT  
		Size: 665.7 KB (665740 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72fef4a8a0cc5f1eea5507fd77aa05a9500cb4d1ef385312c7bcbae389046009`  
		Last Modified: Fri, 16 Jun 2023 16:40:28 GMT  
		Size: 35.9 MB (35855437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f5a752b613a2cf39692fa7636be262af8c16ac0a46e8abf8702c047ab934522`  
		Last Modified: Fri, 16 Jun 2023 16:40:22 GMT  
		Size: 367.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v3.0-windowsservercore-1809`

```console
$ docker pull traefik@sha256:468282899a6f9b06f9fca5ebb1a3a5bf030b45e63e0508f36f75ad7792100318
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4499; amd64

### `traefik:v3.0-windowsservercore-1809` - windows version 10.0.17763.4499; amd64

```console
$ docker pull traefik@sha256:58a44dc3d5c4e9816d6873d753a6074c23aa7a462052f72f8fb60172ae00773b
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.7 GB (1688143673 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:01f1804410c439a02c3fbb603e3dc9c1a10922016750389db87aed22db51adb2`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Wed, 14 Jun 2023 17:39:58 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 14 Jun 2023 23:20:14 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/traefik/traefik/releases/download/v3.0.0-beta2/traefik_v3.0.0-beta2_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Wed, 14 Jun 2023 23:20:15 GMT
EXPOSE 80
# Wed, 14 Jun 2023 23:20:15 GMT
ENTRYPOINT ["/traefik"]
# Wed, 14 Jun 2023 23:20:16 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v3.0.0-beta2 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b712a9a082fd391beaa9ca7c8e6c3fda37b0ad8d29cc4663173ed973b961d342`  
		Last Modified: Wed, 14 Jun 2023 18:21:55 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a9b4e4d63720e53bc602ec5afd594ae87dc8d306b5873781d0fd3055f818c16`  
		Last Modified: Wed, 14 Jun 2023 23:21:42 GMT  
		Size: 37.5 MB (37517697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef864bbe2da9a6fc6aba62dc459a1b659d3d46ada2e3a1a04ee8b7c02a6f4e92`  
		Last Modified: Wed, 14 Jun 2023 23:21:33 GMT  
		Size: 1.4 KB (1377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2213ec09fd524be95c6a826c50e14f52e9e639e66c3572d56f438bac3cf98bab`  
		Last Modified: Wed, 14 Jun 2023 23:21:33 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58cd9c99e4865330e999c8136c9600504c563b6c37779e28663ff1421a7ac516`  
		Last Modified: Wed, 14 Jun 2023 23:21:33 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v3.0.0-beta2`

```console
$ docker pull traefik@sha256:366345ddd7c17a8d273696797a375c5144e3a5242bdb39a2855baaec2bd6851c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; s390x

### `traefik:v3.0.0-beta2` - linux; amd64

```console
$ docker pull traefik@sha256:5f3e471200c36a65618b50719f8f467530a9895a61f87bda0bb437b5718ac327
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.6 MB (40562366 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c08e518a729607ef1142c8a57a82ab9df16bcd47e4e5a6874d07467e07a87dd0`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 14 Jun 2023 20:42:13 GMT
ADD file:4fa8e307f595ecff485113fb0ec6e2320979eaa6fb3eb467d2433771a6f016e6 in / 
# Wed, 14 Jun 2023 20:42:13 GMT
CMD ["/bin/sh"]
# Thu, 15 Jun 2023 06:27:27 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 15 Jun 2023 06:27:31 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v3.0.0-beta2/traefik_v3.0.0-beta2_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 15 Jun 2023 06:27:31 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 15 Jun 2023 06:27:31 GMT
EXPOSE 80
# Thu, 15 Jun 2023 06:27:31 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 15 Jun 2023 06:27:31 GMT
CMD ["traefik"]
# Thu, 15 Jun 2023 06:27:31 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v3.0.0-beta2 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:0cdfa0c98ed79707cd91c5dd7ebd282aa2b976d86a9e699d7fc188cdb6be390e`  
		Last Modified: Wed, 14 Jun 2023 20:42:58 GMT  
		Size: 2.8 MB (2825916 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75174169df6666c22d9a3c3085ea1eacd10478e79c70bbd53abc6cf647134b86`  
		Last Modified: Thu, 15 Jun 2023 06:27:51 GMT  
		Size: 661.2 KB (661203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4920635d165c3cb67e2ee3fd37aec68049e9730086d72999c5d926fd5a2b5bdb`  
		Last Modified: Thu, 15 Jun 2023 06:27:56 GMT  
		Size: 37.1 MB (37074878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:133801879169abc43871a5a32c77fb651e1ae90c3233a0cce11b6ead5c526c79`  
		Last Modified: Thu, 15 Jun 2023 06:27:50 GMT  
		Size: 369.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v3.0.0-beta2` - linux; arm variant v6

```console
$ docker pull traefik@sha256:0e010dd7b60c3960f903b07854cae707e691496f1491f0447ca2635b5a374a6d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.3 MB (38289085 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ee0012c6d54cfd4da66d0da5e01f3dc4f70609eec928ce429e71a5efa02c96b3`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 14 Jun 2023 18:49:32 GMT
ADD file:b987db82fa4ce6e623de49a50612c1fd91c5ab2209a62a5727ab3436c2923e91 in / 
# Wed, 14 Jun 2023 18:49:32 GMT
CMD ["/bin/sh"]
# Wed, 14 Jun 2023 20:12:22 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 14 Jun 2023 20:12:26 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v3.0.0-beta2/traefik_v3.0.0-beta2_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Wed, 14 Jun 2023 20:12:26 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 14 Jun 2023 20:12:26 GMT
EXPOSE 80
# Wed, 14 Jun 2023 20:12:26 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 14 Jun 2023 20:12:26 GMT
CMD ["traefik"]
# Wed, 14 Jun 2023 20:12:26 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v3.0.0-beta2 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:41c5c5b38e13af18def277385607129664fb24993d262d4b601a381e776482a9`  
		Last Modified: Wed, 14 Jun 2023 18:50:19 GMT  
		Size: 2.6 MB (2633060 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:718cfe2cb66c053a8fdb09adf88b20a52f260f22abd38cba68cc2838ee33e73d`  
		Last Modified: Wed, 14 Jun 2023 20:12:46 GMT  
		Size: 666.3 KB (666349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47b2cef5f2c79471c563b3c10376140084b51c097de00e9be0b758219ab95e5c`  
		Last Modified: Wed, 14 Jun 2023 20:12:52 GMT  
		Size: 35.0 MB (34989308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66078e59ed6730404193e57cea654480d0731663c7a068349344e0a681d1c660`  
		Last Modified: Wed, 14 Jun 2023 20:12:46 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v3.0.0-beta2` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:70a1b62539b384a09d98e22bea5212f0120150377a85a599839d35897a55ef3b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.4 MB (37406948 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ebe5414a44cb1b3f5ada2c4d4477d9bb6c73103354707edb71a0adfb2138efb4`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 14 Jun 2023 20:49:10 GMT
ADD file:2b463f242cb7bf946452bb4781838348ecbe80da144fbab09f51d7e050dc68f3 in / 
# Wed, 14 Jun 2023 20:49:11 GMT
CMD ["/bin/sh"]
# Thu, 15 Jun 2023 07:10:02 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 15 Jun 2023 07:10:05 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v3.0.0-beta2/traefik_v3.0.0-beta2_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 15 Jun 2023 07:10:05 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 15 Jun 2023 07:10:05 GMT
EXPOSE 80
# Thu, 15 Jun 2023 07:10:05 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 15 Jun 2023 07:10:06 GMT
CMD ["traefik"]
# Thu, 15 Jun 2023 07:10:06 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v3.0.0-beta2 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:a147224bf413aeffbbfcdcb5104d35c647256a5c32083f4d8134f09a4e74ddeb`  
		Last Modified: Wed, 14 Jun 2023 20:49:52 GMT  
		Size: 2.7 MB (2720801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d273c78104fe60b8d6b0a1d68c0b259293bd972e3ff515bc403a8bfbff6d88a9`  
		Last Modified: Thu, 15 Jun 2023 07:10:24 GMT  
		Size: 662.3 KB (662262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2be3d50287a2f7fba1e120466ee42285469a74914da1378df40803a29c6245f3`  
		Last Modified: Thu, 15 Jun 2023 07:10:28 GMT  
		Size: 34.0 MB (34023516 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:452eba291077ce9af0d14edf868a5522679b04016d43f8a2e05b194d2618d210`  
		Last Modified: Thu, 15 Jun 2023 07:10:24 GMT  
		Size: 369.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v3.0.0-beta2` - linux; s390x

```console
$ docker pull traefik@sha256:feacc7d5c4b3a2d20dcbfc15e95e848cbc3b83820b99cafd9807db1863b65891
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.1 MB (39130249 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:af3c57f022e7ac6f998e72d571ec87f092a10f19341601105cd3f5c2b767d2ad`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 15 Jun 2023 05:22:08 GMT
ADD file:243e0553a1216040e760e1a7ce7119b10b477e081d792fa29e8c17403a8785ff in / 
# Thu, 15 Jun 2023 05:22:08 GMT
CMD ["/bin/sh"]
# Fri, 16 Jun 2023 16:39:46 GMT
RUN apk --no-cache add ca-certificates tzdata
# Fri, 16 Jun 2023 16:39:50 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v3.0.0-beta2/traefik_v3.0.0-beta2_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Fri, 16 Jun 2023 16:39:52 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Fri, 16 Jun 2023 16:39:52 GMT
EXPOSE 80
# Fri, 16 Jun 2023 16:39:52 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 16 Jun 2023 16:39:52 GMT
CMD ["traefik"]
# Fri, 16 Jun 2023 16:39:52 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v3.0.0-beta2 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:66238d49bc5bf7485c63b2671ef3c879dd2015902b151f6f5e7d178cf472c9f2`  
		Last Modified: Thu, 15 Jun 2023 05:32:59 GMT  
		Size: 2.6 MB (2608705 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42d9a3c534bf80ba9a88587c1fd786fafea714685bd2abfac3984c6ddfda55b2`  
		Last Modified: Fri, 16 Jun 2023 16:40:22 GMT  
		Size: 665.7 KB (665740 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72fef4a8a0cc5f1eea5507fd77aa05a9500cb4d1ef385312c7bcbae389046009`  
		Last Modified: Fri, 16 Jun 2023 16:40:28 GMT  
		Size: 35.9 MB (35855437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f5a752b613a2cf39692fa7636be262af8c16ac0a46e8abf8702c047ab934522`  
		Last Modified: Fri, 16 Jun 2023 16:40:22 GMT  
		Size: 367.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v3.0.0-beta2-windowsservercore-1809`

```console
$ docker pull traefik@sha256:468282899a6f9b06f9fca5ebb1a3a5bf030b45e63e0508f36f75ad7792100318
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4499; amd64

### `traefik:v3.0.0-beta2-windowsservercore-1809` - windows version 10.0.17763.4499; amd64

```console
$ docker pull traefik@sha256:58a44dc3d5c4e9816d6873d753a6074c23aa7a462052f72f8fb60172ae00773b
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.7 GB (1688143673 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:01f1804410c439a02c3fbb603e3dc9c1a10922016750389db87aed22db51adb2`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Wed, 14 Jun 2023 17:39:58 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 14 Jun 2023 23:20:14 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/traefik/traefik/releases/download/v3.0.0-beta2/traefik_v3.0.0-beta2_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Wed, 14 Jun 2023 23:20:15 GMT
EXPOSE 80
# Wed, 14 Jun 2023 23:20:15 GMT
ENTRYPOINT ["/traefik"]
# Wed, 14 Jun 2023 23:20:16 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v3.0.0-beta2 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b712a9a082fd391beaa9ca7c8e6c3fda37b0ad8d29cc4663173ed973b961d342`  
		Last Modified: Wed, 14 Jun 2023 18:21:55 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a9b4e4d63720e53bc602ec5afd594ae87dc8d306b5873781d0fd3055f818c16`  
		Last Modified: Wed, 14 Jun 2023 23:21:42 GMT  
		Size: 37.5 MB (37517697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef864bbe2da9a6fc6aba62dc459a1b659d3d46ada2e3a1a04ee8b7c02a6f4e92`  
		Last Modified: Wed, 14 Jun 2023 23:21:33 GMT  
		Size: 1.4 KB (1377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2213ec09fd524be95c6a826c50e14f52e9e639e66c3572d56f438bac3cf98bab`  
		Last Modified: Wed, 14 Jun 2023 23:21:33 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58cd9c99e4865330e999c8136c9600504c563b6c37779e28663ff1421a7ac516`  
		Last Modified: Wed, 14 Jun 2023 23:21:33 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:windowsservercore-1809`

```console
$ docker pull traefik@sha256:dc03c1897e7fa9697744289086dfd429fc4b22694446bb29881671bd63335f55
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4499; amd64

### `traefik:windowsservercore-1809` - windows version 10.0.17763.4499; amd64

```console
$ docker pull traefik@sha256:b61a301ec003fdfb61afa059050468dfd19e329b91adc04b989378307c01e5b9
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.7 GB (1688297643 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c40b4425780339ae5ed986b0312fde45ee26d18c675994fa07879d3ba8ba802f`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Wed, 14 Jun 2023 17:39:58 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 20 Jun 2023 23:18:02 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/traefik/traefik/releases/download/v2.10.3/traefik_v2.10.3_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Tue, 20 Jun 2023 23:18:04 GMT
EXPOSE 80
# Tue, 20 Jun 2023 23:18:05 GMT
ENTRYPOINT ["/traefik"]
# Tue, 20 Jun 2023 23:18:06 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.10.3 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b712a9a082fd391beaa9ca7c8e6c3fda37b0ad8d29cc4663173ed973b961d342`  
		Last Modified: Wed, 14 Jun 2023 18:21:55 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6ae7661d409041f0b91655d0629e3756f67688eabbeb2d46f7c44b9e110614a`  
		Last Modified: Tue, 20 Jun 2023 23:18:40 GMT  
		Size: 37.7 MB (37671801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eda08f2fb0ae872eb7d6aee508ca42acf0aa7d71c4cc8b22b2acd32a8dac9307`  
		Last Modified: Tue, 20 Jun 2023 23:18:30 GMT  
		Size: 1.3 KB (1301 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7fc4c49780e0c6b8e9d6e2577ae7f3597396920dbd9c744ace14c79b3db639e`  
		Last Modified: Tue, 20 Jun 2023 23:18:30 GMT  
		Size: 1.4 KB (1362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7546eab39455c2a7df3171964211f93193cc95597a50435a4c7e5e3ee22b6f2`  
		Last Modified: Tue, 20 Jun 2023 23:18:30 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
