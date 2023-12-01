<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `traefik`

-	[`traefik:2.10`](#traefik210)
-	[`traefik:2.10-windowsservercore-1809`](#traefik210-windowsservercore-1809)
-	[`traefik:2.10.6`](#traefik2106)
-	[`traefik:2.10.6-windowsservercore-1809`](#traefik2106-windowsservercore-1809)
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
-	[`traefik:v2.10.6`](#traefikv2106)
-	[`traefik:v2.10.6-windowsservercore-1809`](#traefikv2106-windowsservercore-1809)
-	[`traefik:v3.0`](#traefikv30)
-	[`traefik:v3.0-windowsservercore-1809`](#traefikv30-windowsservercore-1809)
-	[`traefik:v3.0.0-beta5`](#traefikv300-beta5)
-	[`traefik:v3.0.0-beta5-windowsservercore-1809`](#traefikv300-beta5-windowsservercore-1809)
-	[`traefik:windowsservercore-1809`](#traefikwindowsservercore-1809)

## `traefik:2.10`

```console
$ docker pull traefik@sha256:1957e3314f435c85b3a19f7babd53c630996aa1af65d1f479d75539251b1e112
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; s390x

### `traefik:2.10` - linux; amd64

```console
$ docker pull traefik@sha256:4fa90639a86b7b87d5a4451b683c90e492c1d7bb44e8c16ab8002497c943154c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.2 MB (43230049 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7ec32645961a9f4d5e9d9538fc3514c4d3dbac801ec4aaa96289229441b3fa2c`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 30 Nov 2023 23:22:52 GMT
ADD file:fc714080c3bcbbce7ac746a10d7b4355ffa36293a8d435d62cd5359ea8eb8364 in / 
# Thu, 30 Nov 2023 23:22:52 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 07:48:32 GMT
RUN apk --no-cache add ca-certificates tzdata
# Fri, 01 Dec 2023 07:48:43 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.10.6/traefik_v2.10.6_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Fri, 01 Dec 2023 07:48:44 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Fri, 01 Dec 2023 07:48:44 GMT
EXPOSE 80
# Fri, 01 Dec 2023 07:48:44 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 01 Dec 2023 07:48:44 GMT
CMD ["traefik"]
# Fri, 01 Dec 2023 07:48:44 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.10.6 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:0cb5302170085a0e3b6bccc1b80747fb67e3e7de16de63b49216595635c9413f`  
		Last Modified: Fri, 01 Dec 2023 07:49:20 GMT  
		Size: 39.2 MB (39204940 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6d44d6740486e30a1765db288944de7b12faebce16784306bf9eaf764cfce4e`  
		Last Modified: Fri, 01 Dec 2023 07:49:14 GMT  
		Size: 369.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:2.10` - linux; arm variant v6

```console
$ docker pull traefik@sha256:f8efcf19b182f28245307ab6e5091074d7845a16f80c8a085272caeb80407b0d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.8 MB (40821344 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0bb90430247f6a2ff7e1cb1b59bf9cf11e10f49829ae1ad6b73d43a597b91feb`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 30 Nov 2023 22:49:18 GMT
ADD file:dbf65487d049081dc2d39b3d99d2c64b6c89754e7e2996a46169d3512e59f32a in / 
# Thu, 30 Nov 2023 22:49:18 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 11:16:30 GMT
RUN apk --no-cache add ca-certificates tzdata
# Fri, 01 Dec 2023 11:16:44 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.10.6/traefik_v2.10.6_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Fri, 01 Dec 2023 11:16:45 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Fri, 01 Dec 2023 11:16:45 GMT
EXPOSE 80
# Fri, 01 Dec 2023 11:16:45 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 01 Dec 2023 11:16:45 GMT
CMD ["traefik"]
# Fri, 01 Dec 2023 11:16:45 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.10.6 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:2098f4d6b1552654a7fe1262e0d0e75bce45499077d32a450bc2960b5c6f17d9`  
		Last Modified: Fri, 01 Dec 2023 11:17:23 GMT  
		Size: 37.1 MB (37051398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e0fd89298c613dca9eedd6ca6406c7bb4e696154cf60bffa3cb88f2106ae1ae`  
		Last Modified: Fri, 01 Dec 2023 11:17:17 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:2.10` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:10148f45784e6236f1663cfec56b83724cb3785eb776bc394eb0b5064e00dfdc
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.2 MB (40218357 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ab346e39e7e968375b87bc4491cf3ef3b90ac138f4264e6a3a04d856007c6023`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 30 Nov 2023 23:11:03 GMT
ADD file:d8a30995bbcd627f084912c728fda5483b6ba486de25af588a0956069d0bd7ad in / 
# Thu, 30 Nov 2023 23:11:03 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 09:31:02 GMT
RUN apk --no-cache add ca-certificates tzdata
# Fri, 01 Dec 2023 09:31:11 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.10.6/traefik_v2.10.6_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Fri, 01 Dec 2023 09:31:12 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Fri, 01 Dec 2023 09:31:12 GMT
EXPOSE 80
# Fri, 01 Dec 2023 09:31:12 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 01 Dec 2023 09:31:12 GMT
CMD ["traefik"]
# Fri, 01 Dec 2023 09:31:12 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.10.6 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:e6c0cc073546c2dbdb197249cf4ba88bbfc2e2b9b7d7cb5222879c8d0191d388`  
		Last Modified: Fri, 01 Dec 2023 09:31:44 GMT  
		Size: 36.3 MB (36260436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b71f0cbdc87b5eb493c462520a93ab7dd52b31ab414572a1a15f6584fdeb68b8`  
		Last Modified: Fri, 01 Dec 2023 09:31:40 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:2.10` - linux; s390x

```console
$ docker pull traefik@sha256:02fd705421f50509a35b4c85c0a85432a8b8f2275381586d92b97ea23cb8f620
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **42.1 MB (42053003 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5d1e416a52af492cf639cce18bf0281349f9092f3d66d038e2649964e0f196ce`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 30 Nov 2023 22:42:08 GMT
ADD file:50d6643abf7df167a927decd69d193b980557ff73cca48dce86d57e2ff25ad45 in / 
# Thu, 30 Nov 2023 22:42:09 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 07:15:54 GMT
RUN apk --no-cache add ca-certificates tzdata
# Fri, 01 Dec 2023 07:16:18 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.10.6/traefik_v2.10.6_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Fri, 01 Dec 2023 07:16:23 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Fri, 01 Dec 2023 07:16:23 GMT
EXPOSE 80
# Fri, 01 Dec 2023 07:16:23 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 01 Dec 2023 07:16:23 GMT
CMD ["traefik"]
# Fri, 01 Dec 2023 07:16:24 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.10.6 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:248952b66da9263ca0bb42a1f9af92f04b1028d4adb0225e03f84909823f0264`  
		Last Modified: Fri, 01 Dec 2023 07:17:02 GMT  
		Size: 38.2 MB (38212346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f8191eba9e7d3906f3b7c51f37b7c1631270660c021bdeffb833f0b3ba86932`  
		Last Modified: Fri, 01 Dec 2023 07:16:56 GMT  
		Size: 367.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:2.10-windowsservercore-1809`

```console
$ docker pull traefik@sha256:4009a9c08e8ff3f3a8215cfc2bcce0355913c9800985c58828d1c7cba68572d6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.5122; amd64

### `traefik:2.10-windowsservercore-1809` - windows version 10.0.17763.5122; amd64

```console
$ docker pull traefik@sha256:3f007c45153ec0b2e3abe2b3c7c09b093532d0e198ef4b673e4ddd07bf87ea62
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.1 GB (2098146309 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:84386f59fd9c10dc0607ccebed700b43ed3f66ebfbc4b235398ca2a53bb6dce2`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Thu, 09 Nov 2023 17:56:40 GMT
RUN Install update 10.0.17763.5122
# Thu, 16 Nov 2023 01:37:58 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 29 Nov 2023 02:37:05 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/traefik/traefik/releases/download/v2.10.6/traefik_v2.10.6_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Wed, 29 Nov 2023 02:37:06 GMT
EXPOSE 80
# Wed, 29 Nov 2023 02:37:07 GMT
ENTRYPOINT ["/traefik"]
# Wed, 29 Nov 2023 02:37:08 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.10.6 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f7bb9e009deb881cb90e8b4318258e03882de9bc9b312b763654b59cd13d0bb`  
		Last Modified: Tue, 14 Nov 2023 19:53:30 GMT  
		Size: 406.8 MB (406811201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce7a1cc914f0f5e059bfdf02906a6e052b1c97cebaf91eb6c2fd835cfddebda2`  
		Last Modified: Thu, 16 Nov 2023 02:26:46 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fba9e80c0146453b6de8f35aea2ae18481cf6436bd532c51c90bd2e049433406`  
		Last Modified: Wed, 29 Nov 2023 02:37:46 GMT  
		Size: 40.7 MB (40709104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b54955fdd93b60b49068aadb447e1dbe066720ae5efaa7a315e4592abdd138b0`  
		Last Modified: Wed, 29 Nov 2023 02:37:37 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:463cbb8cb23bb46d13942b85ea410666ef2e97489fb170a77eeaa91dd2f7ae9f`  
		Last Modified: Wed, 29 Nov 2023 02:37:37 GMT  
		Size: 1.4 KB (1391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fb9c1cd767d2004163dd2c4b6bb806605d40ff4f8fa90589edef410642f5e41`  
		Last Modified: Wed, 29 Nov 2023 02:37:37 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:2.10.6`

```console
$ docker pull traefik@sha256:1957e3314f435c85b3a19f7babd53c630996aa1af65d1f479d75539251b1e112
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; s390x

### `traefik:2.10.6` - linux; amd64

```console
$ docker pull traefik@sha256:4fa90639a86b7b87d5a4451b683c90e492c1d7bb44e8c16ab8002497c943154c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.2 MB (43230049 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7ec32645961a9f4d5e9d9538fc3514c4d3dbac801ec4aaa96289229441b3fa2c`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 30 Nov 2023 23:22:52 GMT
ADD file:fc714080c3bcbbce7ac746a10d7b4355ffa36293a8d435d62cd5359ea8eb8364 in / 
# Thu, 30 Nov 2023 23:22:52 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 07:48:32 GMT
RUN apk --no-cache add ca-certificates tzdata
# Fri, 01 Dec 2023 07:48:43 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.10.6/traefik_v2.10.6_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Fri, 01 Dec 2023 07:48:44 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Fri, 01 Dec 2023 07:48:44 GMT
EXPOSE 80
# Fri, 01 Dec 2023 07:48:44 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 01 Dec 2023 07:48:44 GMT
CMD ["traefik"]
# Fri, 01 Dec 2023 07:48:44 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.10.6 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:0cb5302170085a0e3b6bccc1b80747fb67e3e7de16de63b49216595635c9413f`  
		Last Modified: Fri, 01 Dec 2023 07:49:20 GMT  
		Size: 39.2 MB (39204940 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6d44d6740486e30a1765db288944de7b12faebce16784306bf9eaf764cfce4e`  
		Last Modified: Fri, 01 Dec 2023 07:49:14 GMT  
		Size: 369.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:2.10.6` - linux; arm variant v6

```console
$ docker pull traefik@sha256:f8efcf19b182f28245307ab6e5091074d7845a16f80c8a085272caeb80407b0d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.8 MB (40821344 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0bb90430247f6a2ff7e1cb1b59bf9cf11e10f49829ae1ad6b73d43a597b91feb`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 30 Nov 2023 22:49:18 GMT
ADD file:dbf65487d049081dc2d39b3d99d2c64b6c89754e7e2996a46169d3512e59f32a in / 
# Thu, 30 Nov 2023 22:49:18 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 11:16:30 GMT
RUN apk --no-cache add ca-certificates tzdata
# Fri, 01 Dec 2023 11:16:44 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.10.6/traefik_v2.10.6_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Fri, 01 Dec 2023 11:16:45 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Fri, 01 Dec 2023 11:16:45 GMT
EXPOSE 80
# Fri, 01 Dec 2023 11:16:45 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 01 Dec 2023 11:16:45 GMT
CMD ["traefik"]
# Fri, 01 Dec 2023 11:16:45 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.10.6 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:2098f4d6b1552654a7fe1262e0d0e75bce45499077d32a450bc2960b5c6f17d9`  
		Last Modified: Fri, 01 Dec 2023 11:17:23 GMT  
		Size: 37.1 MB (37051398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e0fd89298c613dca9eedd6ca6406c7bb4e696154cf60bffa3cb88f2106ae1ae`  
		Last Modified: Fri, 01 Dec 2023 11:17:17 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:2.10.6` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:10148f45784e6236f1663cfec56b83724cb3785eb776bc394eb0b5064e00dfdc
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.2 MB (40218357 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ab346e39e7e968375b87bc4491cf3ef3b90ac138f4264e6a3a04d856007c6023`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 30 Nov 2023 23:11:03 GMT
ADD file:d8a30995bbcd627f084912c728fda5483b6ba486de25af588a0956069d0bd7ad in / 
# Thu, 30 Nov 2023 23:11:03 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 09:31:02 GMT
RUN apk --no-cache add ca-certificates tzdata
# Fri, 01 Dec 2023 09:31:11 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.10.6/traefik_v2.10.6_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Fri, 01 Dec 2023 09:31:12 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Fri, 01 Dec 2023 09:31:12 GMT
EXPOSE 80
# Fri, 01 Dec 2023 09:31:12 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 01 Dec 2023 09:31:12 GMT
CMD ["traefik"]
# Fri, 01 Dec 2023 09:31:12 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.10.6 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:e6c0cc073546c2dbdb197249cf4ba88bbfc2e2b9b7d7cb5222879c8d0191d388`  
		Last Modified: Fri, 01 Dec 2023 09:31:44 GMT  
		Size: 36.3 MB (36260436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b71f0cbdc87b5eb493c462520a93ab7dd52b31ab414572a1a15f6584fdeb68b8`  
		Last Modified: Fri, 01 Dec 2023 09:31:40 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:2.10.6` - linux; s390x

```console
$ docker pull traefik@sha256:02fd705421f50509a35b4c85c0a85432a8b8f2275381586d92b97ea23cb8f620
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **42.1 MB (42053003 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5d1e416a52af492cf639cce18bf0281349f9092f3d66d038e2649964e0f196ce`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 30 Nov 2023 22:42:08 GMT
ADD file:50d6643abf7df167a927decd69d193b980557ff73cca48dce86d57e2ff25ad45 in / 
# Thu, 30 Nov 2023 22:42:09 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 07:15:54 GMT
RUN apk --no-cache add ca-certificates tzdata
# Fri, 01 Dec 2023 07:16:18 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.10.6/traefik_v2.10.6_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Fri, 01 Dec 2023 07:16:23 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Fri, 01 Dec 2023 07:16:23 GMT
EXPOSE 80
# Fri, 01 Dec 2023 07:16:23 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 01 Dec 2023 07:16:23 GMT
CMD ["traefik"]
# Fri, 01 Dec 2023 07:16:24 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.10.6 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:248952b66da9263ca0bb42a1f9af92f04b1028d4adb0225e03f84909823f0264`  
		Last Modified: Fri, 01 Dec 2023 07:17:02 GMT  
		Size: 38.2 MB (38212346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f8191eba9e7d3906f3b7c51f37b7c1631270660c021bdeffb833f0b3ba86932`  
		Last Modified: Fri, 01 Dec 2023 07:16:56 GMT  
		Size: 367.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:2.10.6-windowsservercore-1809`

```console
$ docker pull traefik@sha256:4009a9c08e8ff3f3a8215cfc2bcce0355913c9800985c58828d1c7cba68572d6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.5122; amd64

### `traefik:2.10.6-windowsservercore-1809` - windows version 10.0.17763.5122; amd64

```console
$ docker pull traefik@sha256:3f007c45153ec0b2e3abe2b3c7c09b093532d0e198ef4b673e4ddd07bf87ea62
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.1 GB (2098146309 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:84386f59fd9c10dc0607ccebed700b43ed3f66ebfbc4b235398ca2a53bb6dce2`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Thu, 09 Nov 2023 17:56:40 GMT
RUN Install update 10.0.17763.5122
# Thu, 16 Nov 2023 01:37:58 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 29 Nov 2023 02:37:05 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/traefik/traefik/releases/download/v2.10.6/traefik_v2.10.6_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Wed, 29 Nov 2023 02:37:06 GMT
EXPOSE 80
# Wed, 29 Nov 2023 02:37:07 GMT
ENTRYPOINT ["/traefik"]
# Wed, 29 Nov 2023 02:37:08 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.10.6 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f7bb9e009deb881cb90e8b4318258e03882de9bc9b312b763654b59cd13d0bb`  
		Last Modified: Tue, 14 Nov 2023 19:53:30 GMT  
		Size: 406.8 MB (406811201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce7a1cc914f0f5e059bfdf02906a6e052b1c97cebaf91eb6c2fd835cfddebda2`  
		Last Modified: Thu, 16 Nov 2023 02:26:46 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fba9e80c0146453b6de8f35aea2ae18481cf6436bd532c51c90bd2e049433406`  
		Last Modified: Wed, 29 Nov 2023 02:37:46 GMT  
		Size: 40.7 MB (40709104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b54955fdd93b60b49068aadb447e1dbe066720ae5efaa7a315e4592abdd138b0`  
		Last Modified: Wed, 29 Nov 2023 02:37:37 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:463cbb8cb23bb46d13942b85ea410666ef2e97489fb170a77eeaa91dd2f7ae9f`  
		Last Modified: Wed, 29 Nov 2023 02:37:37 GMT  
		Size: 1.4 KB (1391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fb9c1cd767d2004163dd2c4b6bb806605d40ff4f8fa90589edef410642f5e41`  
		Last Modified: Wed, 29 Nov 2023 02:37:37 GMT  
		Size: 1.4 KB (1418 bytes)  
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
$ docker pull traefik@sha256:b0c7a98486b0ac8e13a2e2320d452a7464533382cbc252abd449cbb6150737a8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.5122; amd64

### `traefik:3.0-windowsservercore-1809` - windows version 10.0.17763.5122; amd64

```console
$ docker pull traefik@sha256:7e85e697df9033b16fc2f80a00efcb8ac1f717d482f4759a1896ea82b46a1f06
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.1 GB (2099262676 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c790457d2785c38271eccfb5d1a985e2f189d84763d92a8980f1a889f90694f8`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Thu, 09 Nov 2023 17:56:40 GMT
RUN Install update 10.0.17763.5122
# Thu, 16 Nov 2023 01:37:58 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 29 Nov 2023 23:16:56 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/traefik/traefik/releases/download/v3.0.0-beta5/traefik_v3.0.0-beta5_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Wed, 29 Nov 2023 23:16:58 GMT
EXPOSE 80
# Wed, 29 Nov 2023 23:16:58 GMT
ENTRYPOINT ["/traefik"]
# Wed, 29 Nov 2023 23:16:59 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v3.0.0-beta5 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f7bb9e009deb881cb90e8b4318258e03882de9bc9b312b763654b59cd13d0bb`  
		Last Modified: Tue, 14 Nov 2023 19:53:30 GMT  
		Size: 406.8 MB (406811201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce7a1cc914f0f5e059bfdf02906a6e052b1c97cebaf91eb6c2fd835cfddebda2`  
		Last Modified: Thu, 16 Nov 2023 02:26:46 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65d3a54963132deb3b7e269bda91707f12702256902f4c90d487ccb21b9d558a`  
		Last Modified: Wed, 29 Nov 2023 23:17:45 GMT  
		Size: 41.8 MB (41825821 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbce753338c510a600c4f528fabd498bd13a6342d0cd4f58552ee481c98faf41`  
		Last Modified: Wed, 29 Nov 2023 23:17:35 GMT  
		Size: 1.3 KB (1293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41c981bb20ef7dfa9d3f71feb1f2448764c30f56e450431f1c52686bdd4b87de`  
		Last Modified: Wed, 29 Nov 2023 23:17:36 GMT  
		Size: 1.3 KB (1293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b828c19e9a4c0fd32592a6e14895b39c96566702494253d5f316348902749062`  
		Last Modified: Wed, 29 Nov 2023 23:17:35 GMT  
		Size: 1.3 KB (1290 bytes)  
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
$ docker pull traefik@sha256:b0c7a98486b0ac8e13a2e2320d452a7464533382cbc252abd449cbb6150737a8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.5122; amd64

### `traefik:3.0.0-beta5-windowsservercore-1809` - windows version 10.0.17763.5122; amd64

```console
$ docker pull traefik@sha256:7e85e697df9033b16fc2f80a00efcb8ac1f717d482f4759a1896ea82b46a1f06
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.1 GB (2099262676 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c790457d2785c38271eccfb5d1a985e2f189d84763d92a8980f1a889f90694f8`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Thu, 09 Nov 2023 17:56:40 GMT
RUN Install update 10.0.17763.5122
# Thu, 16 Nov 2023 01:37:58 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 29 Nov 2023 23:16:56 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/traefik/traefik/releases/download/v3.0.0-beta5/traefik_v3.0.0-beta5_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Wed, 29 Nov 2023 23:16:58 GMT
EXPOSE 80
# Wed, 29 Nov 2023 23:16:58 GMT
ENTRYPOINT ["/traefik"]
# Wed, 29 Nov 2023 23:16:59 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v3.0.0-beta5 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f7bb9e009deb881cb90e8b4318258e03882de9bc9b312b763654b59cd13d0bb`  
		Last Modified: Tue, 14 Nov 2023 19:53:30 GMT  
		Size: 406.8 MB (406811201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce7a1cc914f0f5e059bfdf02906a6e052b1c97cebaf91eb6c2fd835cfddebda2`  
		Last Modified: Thu, 16 Nov 2023 02:26:46 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65d3a54963132deb3b7e269bda91707f12702256902f4c90d487ccb21b9d558a`  
		Last Modified: Wed, 29 Nov 2023 23:17:45 GMT  
		Size: 41.8 MB (41825821 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbce753338c510a600c4f528fabd498bd13a6342d0cd4f58552ee481c98faf41`  
		Last Modified: Wed, 29 Nov 2023 23:17:35 GMT  
		Size: 1.3 KB (1293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41c981bb20ef7dfa9d3f71feb1f2448764c30f56e450431f1c52686bdd4b87de`  
		Last Modified: Wed, 29 Nov 2023 23:17:36 GMT  
		Size: 1.3 KB (1293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b828c19e9a4c0fd32592a6e14895b39c96566702494253d5f316348902749062`  
		Last Modified: Wed, 29 Nov 2023 23:17:35 GMT  
		Size: 1.3 KB (1290 bytes)  
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
$ docker pull traefik@sha256:b0c7a98486b0ac8e13a2e2320d452a7464533382cbc252abd449cbb6150737a8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.5122; amd64

### `traefik:beaufort-windowsservercore-1809` - windows version 10.0.17763.5122; amd64

```console
$ docker pull traefik@sha256:7e85e697df9033b16fc2f80a00efcb8ac1f717d482f4759a1896ea82b46a1f06
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.1 GB (2099262676 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c790457d2785c38271eccfb5d1a985e2f189d84763d92a8980f1a889f90694f8`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Thu, 09 Nov 2023 17:56:40 GMT
RUN Install update 10.0.17763.5122
# Thu, 16 Nov 2023 01:37:58 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 29 Nov 2023 23:16:56 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/traefik/traefik/releases/download/v3.0.0-beta5/traefik_v3.0.0-beta5_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Wed, 29 Nov 2023 23:16:58 GMT
EXPOSE 80
# Wed, 29 Nov 2023 23:16:58 GMT
ENTRYPOINT ["/traefik"]
# Wed, 29 Nov 2023 23:16:59 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v3.0.0-beta5 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f7bb9e009deb881cb90e8b4318258e03882de9bc9b312b763654b59cd13d0bb`  
		Last Modified: Tue, 14 Nov 2023 19:53:30 GMT  
		Size: 406.8 MB (406811201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce7a1cc914f0f5e059bfdf02906a6e052b1c97cebaf91eb6c2fd835cfddebda2`  
		Last Modified: Thu, 16 Nov 2023 02:26:46 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65d3a54963132deb3b7e269bda91707f12702256902f4c90d487ccb21b9d558a`  
		Last Modified: Wed, 29 Nov 2023 23:17:45 GMT  
		Size: 41.8 MB (41825821 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbce753338c510a600c4f528fabd498bd13a6342d0cd4f58552ee481c98faf41`  
		Last Modified: Wed, 29 Nov 2023 23:17:35 GMT  
		Size: 1.3 KB (1293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41c981bb20ef7dfa9d3f71feb1f2448764c30f56e450431f1c52686bdd4b87de`  
		Last Modified: Wed, 29 Nov 2023 23:17:36 GMT  
		Size: 1.3 KB (1293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b828c19e9a4c0fd32592a6e14895b39c96566702494253d5f316348902749062`  
		Last Modified: Wed, 29 Nov 2023 23:17:35 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:latest`

```console
$ docker pull traefik@sha256:1957e3314f435c85b3a19f7babd53c630996aa1af65d1f479d75539251b1e112
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; s390x

### `traefik:latest` - linux; amd64

```console
$ docker pull traefik@sha256:4fa90639a86b7b87d5a4451b683c90e492c1d7bb44e8c16ab8002497c943154c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.2 MB (43230049 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7ec32645961a9f4d5e9d9538fc3514c4d3dbac801ec4aaa96289229441b3fa2c`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 30 Nov 2023 23:22:52 GMT
ADD file:fc714080c3bcbbce7ac746a10d7b4355ffa36293a8d435d62cd5359ea8eb8364 in / 
# Thu, 30 Nov 2023 23:22:52 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 07:48:32 GMT
RUN apk --no-cache add ca-certificates tzdata
# Fri, 01 Dec 2023 07:48:43 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.10.6/traefik_v2.10.6_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Fri, 01 Dec 2023 07:48:44 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Fri, 01 Dec 2023 07:48:44 GMT
EXPOSE 80
# Fri, 01 Dec 2023 07:48:44 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 01 Dec 2023 07:48:44 GMT
CMD ["traefik"]
# Fri, 01 Dec 2023 07:48:44 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.10.6 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:0cb5302170085a0e3b6bccc1b80747fb67e3e7de16de63b49216595635c9413f`  
		Last Modified: Fri, 01 Dec 2023 07:49:20 GMT  
		Size: 39.2 MB (39204940 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6d44d6740486e30a1765db288944de7b12faebce16784306bf9eaf764cfce4e`  
		Last Modified: Fri, 01 Dec 2023 07:49:14 GMT  
		Size: 369.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:latest` - linux; arm variant v6

```console
$ docker pull traefik@sha256:f8efcf19b182f28245307ab6e5091074d7845a16f80c8a085272caeb80407b0d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.8 MB (40821344 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0bb90430247f6a2ff7e1cb1b59bf9cf11e10f49829ae1ad6b73d43a597b91feb`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 30 Nov 2023 22:49:18 GMT
ADD file:dbf65487d049081dc2d39b3d99d2c64b6c89754e7e2996a46169d3512e59f32a in / 
# Thu, 30 Nov 2023 22:49:18 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 11:16:30 GMT
RUN apk --no-cache add ca-certificates tzdata
# Fri, 01 Dec 2023 11:16:44 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.10.6/traefik_v2.10.6_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Fri, 01 Dec 2023 11:16:45 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Fri, 01 Dec 2023 11:16:45 GMT
EXPOSE 80
# Fri, 01 Dec 2023 11:16:45 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 01 Dec 2023 11:16:45 GMT
CMD ["traefik"]
# Fri, 01 Dec 2023 11:16:45 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.10.6 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:2098f4d6b1552654a7fe1262e0d0e75bce45499077d32a450bc2960b5c6f17d9`  
		Last Modified: Fri, 01 Dec 2023 11:17:23 GMT  
		Size: 37.1 MB (37051398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e0fd89298c613dca9eedd6ca6406c7bb4e696154cf60bffa3cb88f2106ae1ae`  
		Last Modified: Fri, 01 Dec 2023 11:17:17 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:latest` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:10148f45784e6236f1663cfec56b83724cb3785eb776bc394eb0b5064e00dfdc
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.2 MB (40218357 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ab346e39e7e968375b87bc4491cf3ef3b90ac138f4264e6a3a04d856007c6023`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 30 Nov 2023 23:11:03 GMT
ADD file:d8a30995bbcd627f084912c728fda5483b6ba486de25af588a0956069d0bd7ad in / 
# Thu, 30 Nov 2023 23:11:03 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 09:31:02 GMT
RUN apk --no-cache add ca-certificates tzdata
# Fri, 01 Dec 2023 09:31:11 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.10.6/traefik_v2.10.6_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Fri, 01 Dec 2023 09:31:12 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Fri, 01 Dec 2023 09:31:12 GMT
EXPOSE 80
# Fri, 01 Dec 2023 09:31:12 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 01 Dec 2023 09:31:12 GMT
CMD ["traefik"]
# Fri, 01 Dec 2023 09:31:12 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.10.6 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:e6c0cc073546c2dbdb197249cf4ba88bbfc2e2b9b7d7cb5222879c8d0191d388`  
		Last Modified: Fri, 01 Dec 2023 09:31:44 GMT  
		Size: 36.3 MB (36260436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b71f0cbdc87b5eb493c462520a93ab7dd52b31ab414572a1a15f6584fdeb68b8`  
		Last Modified: Fri, 01 Dec 2023 09:31:40 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:latest` - linux; s390x

```console
$ docker pull traefik@sha256:02fd705421f50509a35b4c85c0a85432a8b8f2275381586d92b97ea23cb8f620
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **42.1 MB (42053003 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5d1e416a52af492cf639cce18bf0281349f9092f3d66d038e2649964e0f196ce`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 30 Nov 2023 22:42:08 GMT
ADD file:50d6643abf7df167a927decd69d193b980557ff73cca48dce86d57e2ff25ad45 in / 
# Thu, 30 Nov 2023 22:42:09 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 07:15:54 GMT
RUN apk --no-cache add ca-certificates tzdata
# Fri, 01 Dec 2023 07:16:18 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.10.6/traefik_v2.10.6_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Fri, 01 Dec 2023 07:16:23 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Fri, 01 Dec 2023 07:16:23 GMT
EXPOSE 80
# Fri, 01 Dec 2023 07:16:23 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 01 Dec 2023 07:16:23 GMT
CMD ["traefik"]
# Fri, 01 Dec 2023 07:16:24 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.10.6 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:248952b66da9263ca0bb42a1f9af92f04b1028d4adb0225e03f84909823f0264`  
		Last Modified: Fri, 01 Dec 2023 07:17:02 GMT  
		Size: 38.2 MB (38212346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f8191eba9e7d3906f3b7c51f37b7c1631270660c021bdeffb833f0b3ba86932`  
		Last Modified: Fri, 01 Dec 2023 07:16:56 GMT  
		Size: 367.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:saintmarcelin`

```console
$ docker pull traefik@sha256:1957e3314f435c85b3a19f7babd53c630996aa1af65d1f479d75539251b1e112
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; s390x

### `traefik:saintmarcelin` - linux; amd64

```console
$ docker pull traefik@sha256:4fa90639a86b7b87d5a4451b683c90e492c1d7bb44e8c16ab8002497c943154c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.2 MB (43230049 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7ec32645961a9f4d5e9d9538fc3514c4d3dbac801ec4aaa96289229441b3fa2c`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 30 Nov 2023 23:22:52 GMT
ADD file:fc714080c3bcbbce7ac746a10d7b4355ffa36293a8d435d62cd5359ea8eb8364 in / 
# Thu, 30 Nov 2023 23:22:52 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 07:48:32 GMT
RUN apk --no-cache add ca-certificates tzdata
# Fri, 01 Dec 2023 07:48:43 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.10.6/traefik_v2.10.6_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Fri, 01 Dec 2023 07:48:44 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Fri, 01 Dec 2023 07:48:44 GMT
EXPOSE 80
# Fri, 01 Dec 2023 07:48:44 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 01 Dec 2023 07:48:44 GMT
CMD ["traefik"]
# Fri, 01 Dec 2023 07:48:44 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.10.6 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:0cb5302170085a0e3b6bccc1b80747fb67e3e7de16de63b49216595635c9413f`  
		Last Modified: Fri, 01 Dec 2023 07:49:20 GMT  
		Size: 39.2 MB (39204940 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6d44d6740486e30a1765db288944de7b12faebce16784306bf9eaf764cfce4e`  
		Last Modified: Fri, 01 Dec 2023 07:49:14 GMT  
		Size: 369.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:saintmarcelin` - linux; arm variant v6

```console
$ docker pull traefik@sha256:f8efcf19b182f28245307ab6e5091074d7845a16f80c8a085272caeb80407b0d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.8 MB (40821344 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0bb90430247f6a2ff7e1cb1b59bf9cf11e10f49829ae1ad6b73d43a597b91feb`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 30 Nov 2023 22:49:18 GMT
ADD file:dbf65487d049081dc2d39b3d99d2c64b6c89754e7e2996a46169d3512e59f32a in / 
# Thu, 30 Nov 2023 22:49:18 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 11:16:30 GMT
RUN apk --no-cache add ca-certificates tzdata
# Fri, 01 Dec 2023 11:16:44 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.10.6/traefik_v2.10.6_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Fri, 01 Dec 2023 11:16:45 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Fri, 01 Dec 2023 11:16:45 GMT
EXPOSE 80
# Fri, 01 Dec 2023 11:16:45 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 01 Dec 2023 11:16:45 GMT
CMD ["traefik"]
# Fri, 01 Dec 2023 11:16:45 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.10.6 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:2098f4d6b1552654a7fe1262e0d0e75bce45499077d32a450bc2960b5c6f17d9`  
		Last Modified: Fri, 01 Dec 2023 11:17:23 GMT  
		Size: 37.1 MB (37051398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e0fd89298c613dca9eedd6ca6406c7bb4e696154cf60bffa3cb88f2106ae1ae`  
		Last Modified: Fri, 01 Dec 2023 11:17:17 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:saintmarcelin` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:10148f45784e6236f1663cfec56b83724cb3785eb776bc394eb0b5064e00dfdc
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.2 MB (40218357 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ab346e39e7e968375b87bc4491cf3ef3b90ac138f4264e6a3a04d856007c6023`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 30 Nov 2023 23:11:03 GMT
ADD file:d8a30995bbcd627f084912c728fda5483b6ba486de25af588a0956069d0bd7ad in / 
# Thu, 30 Nov 2023 23:11:03 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 09:31:02 GMT
RUN apk --no-cache add ca-certificates tzdata
# Fri, 01 Dec 2023 09:31:11 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.10.6/traefik_v2.10.6_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Fri, 01 Dec 2023 09:31:12 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Fri, 01 Dec 2023 09:31:12 GMT
EXPOSE 80
# Fri, 01 Dec 2023 09:31:12 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 01 Dec 2023 09:31:12 GMT
CMD ["traefik"]
# Fri, 01 Dec 2023 09:31:12 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.10.6 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:e6c0cc073546c2dbdb197249cf4ba88bbfc2e2b9b7d7cb5222879c8d0191d388`  
		Last Modified: Fri, 01 Dec 2023 09:31:44 GMT  
		Size: 36.3 MB (36260436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b71f0cbdc87b5eb493c462520a93ab7dd52b31ab414572a1a15f6584fdeb68b8`  
		Last Modified: Fri, 01 Dec 2023 09:31:40 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:saintmarcelin` - linux; s390x

```console
$ docker pull traefik@sha256:02fd705421f50509a35b4c85c0a85432a8b8f2275381586d92b97ea23cb8f620
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **42.1 MB (42053003 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5d1e416a52af492cf639cce18bf0281349f9092f3d66d038e2649964e0f196ce`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 30 Nov 2023 22:42:08 GMT
ADD file:50d6643abf7df167a927decd69d193b980557ff73cca48dce86d57e2ff25ad45 in / 
# Thu, 30 Nov 2023 22:42:09 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 07:15:54 GMT
RUN apk --no-cache add ca-certificates tzdata
# Fri, 01 Dec 2023 07:16:18 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.10.6/traefik_v2.10.6_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Fri, 01 Dec 2023 07:16:23 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Fri, 01 Dec 2023 07:16:23 GMT
EXPOSE 80
# Fri, 01 Dec 2023 07:16:23 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 01 Dec 2023 07:16:23 GMT
CMD ["traefik"]
# Fri, 01 Dec 2023 07:16:24 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.10.6 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:248952b66da9263ca0bb42a1f9af92f04b1028d4adb0225e03f84909823f0264`  
		Last Modified: Fri, 01 Dec 2023 07:17:02 GMT  
		Size: 38.2 MB (38212346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f8191eba9e7d3906f3b7c51f37b7c1631270660c021bdeffb833f0b3ba86932`  
		Last Modified: Fri, 01 Dec 2023 07:16:56 GMT  
		Size: 367.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:saintmarcelin-windowsservercore-1809`

```console
$ docker pull traefik@sha256:4009a9c08e8ff3f3a8215cfc2bcce0355913c9800985c58828d1c7cba68572d6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.5122; amd64

### `traefik:saintmarcelin-windowsservercore-1809` - windows version 10.0.17763.5122; amd64

```console
$ docker pull traefik@sha256:3f007c45153ec0b2e3abe2b3c7c09b093532d0e198ef4b673e4ddd07bf87ea62
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.1 GB (2098146309 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:84386f59fd9c10dc0607ccebed700b43ed3f66ebfbc4b235398ca2a53bb6dce2`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Thu, 09 Nov 2023 17:56:40 GMT
RUN Install update 10.0.17763.5122
# Thu, 16 Nov 2023 01:37:58 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 29 Nov 2023 02:37:05 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/traefik/traefik/releases/download/v2.10.6/traefik_v2.10.6_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Wed, 29 Nov 2023 02:37:06 GMT
EXPOSE 80
# Wed, 29 Nov 2023 02:37:07 GMT
ENTRYPOINT ["/traefik"]
# Wed, 29 Nov 2023 02:37:08 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.10.6 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f7bb9e009deb881cb90e8b4318258e03882de9bc9b312b763654b59cd13d0bb`  
		Last Modified: Tue, 14 Nov 2023 19:53:30 GMT  
		Size: 406.8 MB (406811201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce7a1cc914f0f5e059bfdf02906a6e052b1c97cebaf91eb6c2fd835cfddebda2`  
		Last Modified: Thu, 16 Nov 2023 02:26:46 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fba9e80c0146453b6de8f35aea2ae18481cf6436bd532c51c90bd2e049433406`  
		Last Modified: Wed, 29 Nov 2023 02:37:46 GMT  
		Size: 40.7 MB (40709104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b54955fdd93b60b49068aadb447e1dbe066720ae5efaa7a315e4592abdd138b0`  
		Last Modified: Wed, 29 Nov 2023 02:37:37 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:463cbb8cb23bb46d13942b85ea410666ef2e97489fb170a77eeaa91dd2f7ae9f`  
		Last Modified: Wed, 29 Nov 2023 02:37:37 GMT  
		Size: 1.4 KB (1391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fb9c1cd767d2004163dd2c4b6bb806605d40ff4f8fa90589edef410642f5e41`  
		Last Modified: Wed, 29 Nov 2023 02:37:37 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v2.10`

```console
$ docker pull traefik@sha256:1957e3314f435c85b3a19f7babd53c630996aa1af65d1f479d75539251b1e112
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; s390x

### `traefik:v2.10` - linux; amd64

```console
$ docker pull traefik@sha256:4fa90639a86b7b87d5a4451b683c90e492c1d7bb44e8c16ab8002497c943154c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.2 MB (43230049 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7ec32645961a9f4d5e9d9538fc3514c4d3dbac801ec4aaa96289229441b3fa2c`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 30 Nov 2023 23:22:52 GMT
ADD file:fc714080c3bcbbce7ac746a10d7b4355ffa36293a8d435d62cd5359ea8eb8364 in / 
# Thu, 30 Nov 2023 23:22:52 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 07:48:32 GMT
RUN apk --no-cache add ca-certificates tzdata
# Fri, 01 Dec 2023 07:48:43 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.10.6/traefik_v2.10.6_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Fri, 01 Dec 2023 07:48:44 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Fri, 01 Dec 2023 07:48:44 GMT
EXPOSE 80
# Fri, 01 Dec 2023 07:48:44 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 01 Dec 2023 07:48:44 GMT
CMD ["traefik"]
# Fri, 01 Dec 2023 07:48:44 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.10.6 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:0cb5302170085a0e3b6bccc1b80747fb67e3e7de16de63b49216595635c9413f`  
		Last Modified: Fri, 01 Dec 2023 07:49:20 GMT  
		Size: 39.2 MB (39204940 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6d44d6740486e30a1765db288944de7b12faebce16784306bf9eaf764cfce4e`  
		Last Modified: Fri, 01 Dec 2023 07:49:14 GMT  
		Size: 369.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v2.10` - linux; arm variant v6

```console
$ docker pull traefik@sha256:f8efcf19b182f28245307ab6e5091074d7845a16f80c8a085272caeb80407b0d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.8 MB (40821344 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0bb90430247f6a2ff7e1cb1b59bf9cf11e10f49829ae1ad6b73d43a597b91feb`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 30 Nov 2023 22:49:18 GMT
ADD file:dbf65487d049081dc2d39b3d99d2c64b6c89754e7e2996a46169d3512e59f32a in / 
# Thu, 30 Nov 2023 22:49:18 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 11:16:30 GMT
RUN apk --no-cache add ca-certificates tzdata
# Fri, 01 Dec 2023 11:16:44 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.10.6/traefik_v2.10.6_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Fri, 01 Dec 2023 11:16:45 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Fri, 01 Dec 2023 11:16:45 GMT
EXPOSE 80
# Fri, 01 Dec 2023 11:16:45 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 01 Dec 2023 11:16:45 GMT
CMD ["traefik"]
# Fri, 01 Dec 2023 11:16:45 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.10.6 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:2098f4d6b1552654a7fe1262e0d0e75bce45499077d32a450bc2960b5c6f17d9`  
		Last Modified: Fri, 01 Dec 2023 11:17:23 GMT  
		Size: 37.1 MB (37051398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e0fd89298c613dca9eedd6ca6406c7bb4e696154cf60bffa3cb88f2106ae1ae`  
		Last Modified: Fri, 01 Dec 2023 11:17:17 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v2.10` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:10148f45784e6236f1663cfec56b83724cb3785eb776bc394eb0b5064e00dfdc
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.2 MB (40218357 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ab346e39e7e968375b87bc4491cf3ef3b90ac138f4264e6a3a04d856007c6023`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 30 Nov 2023 23:11:03 GMT
ADD file:d8a30995bbcd627f084912c728fda5483b6ba486de25af588a0956069d0bd7ad in / 
# Thu, 30 Nov 2023 23:11:03 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 09:31:02 GMT
RUN apk --no-cache add ca-certificates tzdata
# Fri, 01 Dec 2023 09:31:11 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.10.6/traefik_v2.10.6_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Fri, 01 Dec 2023 09:31:12 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Fri, 01 Dec 2023 09:31:12 GMT
EXPOSE 80
# Fri, 01 Dec 2023 09:31:12 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 01 Dec 2023 09:31:12 GMT
CMD ["traefik"]
# Fri, 01 Dec 2023 09:31:12 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.10.6 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:e6c0cc073546c2dbdb197249cf4ba88bbfc2e2b9b7d7cb5222879c8d0191d388`  
		Last Modified: Fri, 01 Dec 2023 09:31:44 GMT  
		Size: 36.3 MB (36260436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b71f0cbdc87b5eb493c462520a93ab7dd52b31ab414572a1a15f6584fdeb68b8`  
		Last Modified: Fri, 01 Dec 2023 09:31:40 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v2.10` - linux; s390x

```console
$ docker pull traefik@sha256:02fd705421f50509a35b4c85c0a85432a8b8f2275381586d92b97ea23cb8f620
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **42.1 MB (42053003 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5d1e416a52af492cf639cce18bf0281349f9092f3d66d038e2649964e0f196ce`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 30 Nov 2023 22:42:08 GMT
ADD file:50d6643abf7df167a927decd69d193b980557ff73cca48dce86d57e2ff25ad45 in / 
# Thu, 30 Nov 2023 22:42:09 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 07:15:54 GMT
RUN apk --no-cache add ca-certificates tzdata
# Fri, 01 Dec 2023 07:16:18 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.10.6/traefik_v2.10.6_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Fri, 01 Dec 2023 07:16:23 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Fri, 01 Dec 2023 07:16:23 GMT
EXPOSE 80
# Fri, 01 Dec 2023 07:16:23 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 01 Dec 2023 07:16:23 GMT
CMD ["traefik"]
# Fri, 01 Dec 2023 07:16:24 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.10.6 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:248952b66da9263ca0bb42a1f9af92f04b1028d4adb0225e03f84909823f0264`  
		Last Modified: Fri, 01 Dec 2023 07:17:02 GMT  
		Size: 38.2 MB (38212346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f8191eba9e7d3906f3b7c51f37b7c1631270660c021bdeffb833f0b3ba86932`  
		Last Modified: Fri, 01 Dec 2023 07:16:56 GMT  
		Size: 367.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v2.10-windowsservercore-1809`

```console
$ docker pull traefik@sha256:4009a9c08e8ff3f3a8215cfc2bcce0355913c9800985c58828d1c7cba68572d6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.5122; amd64

### `traefik:v2.10-windowsservercore-1809` - windows version 10.0.17763.5122; amd64

```console
$ docker pull traefik@sha256:3f007c45153ec0b2e3abe2b3c7c09b093532d0e198ef4b673e4ddd07bf87ea62
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.1 GB (2098146309 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:84386f59fd9c10dc0607ccebed700b43ed3f66ebfbc4b235398ca2a53bb6dce2`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Thu, 09 Nov 2023 17:56:40 GMT
RUN Install update 10.0.17763.5122
# Thu, 16 Nov 2023 01:37:58 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 29 Nov 2023 02:37:05 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/traefik/traefik/releases/download/v2.10.6/traefik_v2.10.6_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Wed, 29 Nov 2023 02:37:06 GMT
EXPOSE 80
# Wed, 29 Nov 2023 02:37:07 GMT
ENTRYPOINT ["/traefik"]
# Wed, 29 Nov 2023 02:37:08 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.10.6 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f7bb9e009deb881cb90e8b4318258e03882de9bc9b312b763654b59cd13d0bb`  
		Last Modified: Tue, 14 Nov 2023 19:53:30 GMT  
		Size: 406.8 MB (406811201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce7a1cc914f0f5e059bfdf02906a6e052b1c97cebaf91eb6c2fd835cfddebda2`  
		Last Modified: Thu, 16 Nov 2023 02:26:46 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fba9e80c0146453b6de8f35aea2ae18481cf6436bd532c51c90bd2e049433406`  
		Last Modified: Wed, 29 Nov 2023 02:37:46 GMT  
		Size: 40.7 MB (40709104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b54955fdd93b60b49068aadb447e1dbe066720ae5efaa7a315e4592abdd138b0`  
		Last Modified: Wed, 29 Nov 2023 02:37:37 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:463cbb8cb23bb46d13942b85ea410666ef2e97489fb170a77eeaa91dd2f7ae9f`  
		Last Modified: Wed, 29 Nov 2023 02:37:37 GMT  
		Size: 1.4 KB (1391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fb9c1cd767d2004163dd2c4b6bb806605d40ff4f8fa90589edef410642f5e41`  
		Last Modified: Wed, 29 Nov 2023 02:37:37 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v2.10.6`

```console
$ docker pull traefik@sha256:1957e3314f435c85b3a19f7babd53c630996aa1af65d1f479d75539251b1e112
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; s390x

### `traefik:v2.10.6` - linux; amd64

```console
$ docker pull traefik@sha256:4fa90639a86b7b87d5a4451b683c90e492c1d7bb44e8c16ab8002497c943154c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.2 MB (43230049 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7ec32645961a9f4d5e9d9538fc3514c4d3dbac801ec4aaa96289229441b3fa2c`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 30 Nov 2023 23:22:52 GMT
ADD file:fc714080c3bcbbce7ac746a10d7b4355ffa36293a8d435d62cd5359ea8eb8364 in / 
# Thu, 30 Nov 2023 23:22:52 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 07:48:32 GMT
RUN apk --no-cache add ca-certificates tzdata
# Fri, 01 Dec 2023 07:48:43 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.10.6/traefik_v2.10.6_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Fri, 01 Dec 2023 07:48:44 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Fri, 01 Dec 2023 07:48:44 GMT
EXPOSE 80
# Fri, 01 Dec 2023 07:48:44 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 01 Dec 2023 07:48:44 GMT
CMD ["traefik"]
# Fri, 01 Dec 2023 07:48:44 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.10.6 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:0cb5302170085a0e3b6bccc1b80747fb67e3e7de16de63b49216595635c9413f`  
		Last Modified: Fri, 01 Dec 2023 07:49:20 GMT  
		Size: 39.2 MB (39204940 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6d44d6740486e30a1765db288944de7b12faebce16784306bf9eaf764cfce4e`  
		Last Modified: Fri, 01 Dec 2023 07:49:14 GMT  
		Size: 369.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v2.10.6` - linux; arm variant v6

```console
$ docker pull traefik@sha256:f8efcf19b182f28245307ab6e5091074d7845a16f80c8a085272caeb80407b0d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.8 MB (40821344 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0bb90430247f6a2ff7e1cb1b59bf9cf11e10f49829ae1ad6b73d43a597b91feb`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 30 Nov 2023 22:49:18 GMT
ADD file:dbf65487d049081dc2d39b3d99d2c64b6c89754e7e2996a46169d3512e59f32a in / 
# Thu, 30 Nov 2023 22:49:18 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 11:16:30 GMT
RUN apk --no-cache add ca-certificates tzdata
# Fri, 01 Dec 2023 11:16:44 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.10.6/traefik_v2.10.6_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Fri, 01 Dec 2023 11:16:45 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Fri, 01 Dec 2023 11:16:45 GMT
EXPOSE 80
# Fri, 01 Dec 2023 11:16:45 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 01 Dec 2023 11:16:45 GMT
CMD ["traefik"]
# Fri, 01 Dec 2023 11:16:45 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.10.6 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:2098f4d6b1552654a7fe1262e0d0e75bce45499077d32a450bc2960b5c6f17d9`  
		Last Modified: Fri, 01 Dec 2023 11:17:23 GMT  
		Size: 37.1 MB (37051398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e0fd89298c613dca9eedd6ca6406c7bb4e696154cf60bffa3cb88f2106ae1ae`  
		Last Modified: Fri, 01 Dec 2023 11:17:17 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v2.10.6` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:10148f45784e6236f1663cfec56b83724cb3785eb776bc394eb0b5064e00dfdc
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.2 MB (40218357 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ab346e39e7e968375b87bc4491cf3ef3b90ac138f4264e6a3a04d856007c6023`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 30 Nov 2023 23:11:03 GMT
ADD file:d8a30995bbcd627f084912c728fda5483b6ba486de25af588a0956069d0bd7ad in / 
# Thu, 30 Nov 2023 23:11:03 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 09:31:02 GMT
RUN apk --no-cache add ca-certificates tzdata
# Fri, 01 Dec 2023 09:31:11 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.10.6/traefik_v2.10.6_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Fri, 01 Dec 2023 09:31:12 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Fri, 01 Dec 2023 09:31:12 GMT
EXPOSE 80
# Fri, 01 Dec 2023 09:31:12 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 01 Dec 2023 09:31:12 GMT
CMD ["traefik"]
# Fri, 01 Dec 2023 09:31:12 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.10.6 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:e6c0cc073546c2dbdb197249cf4ba88bbfc2e2b9b7d7cb5222879c8d0191d388`  
		Last Modified: Fri, 01 Dec 2023 09:31:44 GMT  
		Size: 36.3 MB (36260436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b71f0cbdc87b5eb493c462520a93ab7dd52b31ab414572a1a15f6584fdeb68b8`  
		Last Modified: Fri, 01 Dec 2023 09:31:40 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v2.10.6` - linux; s390x

```console
$ docker pull traefik@sha256:02fd705421f50509a35b4c85c0a85432a8b8f2275381586d92b97ea23cb8f620
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **42.1 MB (42053003 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5d1e416a52af492cf639cce18bf0281349f9092f3d66d038e2649964e0f196ce`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 30 Nov 2023 22:42:08 GMT
ADD file:50d6643abf7df167a927decd69d193b980557ff73cca48dce86d57e2ff25ad45 in / 
# Thu, 30 Nov 2023 22:42:09 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 07:15:54 GMT
RUN apk --no-cache add ca-certificates tzdata
# Fri, 01 Dec 2023 07:16:18 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.10.6/traefik_v2.10.6_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Fri, 01 Dec 2023 07:16:23 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Fri, 01 Dec 2023 07:16:23 GMT
EXPOSE 80
# Fri, 01 Dec 2023 07:16:23 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 01 Dec 2023 07:16:23 GMT
CMD ["traefik"]
# Fri, 01 Dec 2023 07:16:24 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.10.6 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:248952b66da9263ca0bb42a1f9af92f04b1028d4adb0225e03f84909823f0264`  
		Last Modified: Fri, 01 Dec 2023 07:17:02 GMT  
		Size: 38.2 MB (38212346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f8191eba9e7d3906f3b7c51f37b7c1631270660c021bdeffb833f0b3ba86932`  
		Last Modified: Fri, 01 Dec 2023 07:16:56 GMT  
		Size: 367.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v2.10.6-windowsservercore-1809`

```console
$ docker pull traefik@sha256:4009a9c08e8ff3f3a8215cfc2bcce0355913c9800985c58828d1c7cba68572d6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.5122; amd64

### `traefik:v2.10.6-windowsservercore-1809` - windows version 10.0.17763.5122; amd64

```console
$ docker pull traefik@sha256:3f007c45153ec0b2e3abe2b3c7c09b093532d0e198ef4b673e4ddd07bf87ea62
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.1 GB (2098146309 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:84386f59fd9c10dc0607ccebed700b43ed3f66ebfbc4b235398ca2a53bb6dce2`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Thu, 09 Nov 2023 17:56:40 GMT
RUN Install update 10.0.17763.5122
# Thu, 16 Nov 2023 01:37:58 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 29 Nov 2023 02:37:05 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/traefik/traefik/releases/download/v2.10.6/traefik_v2.10.6_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Wed, 29 Nov 2023 02:37:06 GMT
EXPOSE 80
# Wed, 29 Nov 2023 02:37:07 GMT
ENTRYPOINT ["/traefik"]
# Wed, 29 Nov 2023 02:37:08 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.10.6 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f7bb9e009deb881cb90e8b4318258e03882de9bc9b312b763654b59cd13d0bb`  
		Last Modified: Tue, 14 Nov 2023 19:53:30 GMT  
		Size: 406.8 MB (406811201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce7a1cc914f0f5e059bfdf02906a6e052b1c97cebaf91eb6c2fd835cfddebda2`  
		Last Modified: Thu, 16 Nov 2023 02:26:46 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fba9e80c0146453b6de8f35aea2ae18481cf6436bd532c51c90bd2e049433406`  
		Last Modified: Wed, 29 Nov 2023 02:37:46 GMT  
		Size: 40.7 MB (40709104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b54955fdd93b60b49068aadb447e1dbe066720ae5efaa7a315e4592abdd138b0`  
		Last Modified: Wed, 29 Nov 2023 02:37:37 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:463cbb8cb23bb46d13942b85ea410666ef2e97489fb170a77eeaa91dd2f7ae9f`  
		Last Modified: Wed, 29 Nov 2023 02:37:37 GMT  
		Size: 1.4 KB (1391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fb9c1cd767d2004163dd2c4b6bb806605d40ff4f8fa90589edef410642f5e41`  
		Last Modified: Wed, 29 Nov 2023 02:37:37 GMT  
		Size: 1.4 KB (1418 bytes)  
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
$ docker pull traefik@sha256:b0c7a98486b0ac8e13a2e2320d452a7464533382cbc252abd449cbb6150737a8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.5122; amd64

### `traefik:v3.0-windowsservercore-1809` - windows version 10.0.17763.5122; amd64

```console
$ docker pull traefik@sha256:7e85e697df9033b16fc2f80a00efcb8ac1f717d482f4759a1896ea82b46a1f06
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.1 GB (2099262676 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c790457d2785c38271eccfb5d1a985e2f189d84763d92a8980f1a889f90694f8`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Thu, 09 Nov 2023 17:56:40 GMT
RUN Install update 10.0.17763.5122
# Thu, 16 Nov 2023 01:37:58 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 29 Nov 2023 23:16:56 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/traefik/traefik/releases/download/v3.0.0-beta5/traefik_v3.0.0-beta5_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Wed, 29 Nov 2023 23:16:58 GMT
EXPOSE 80
# Wed, 29 Nov 2023 23:16:58 GMT
ENTRYPOINT ["/traefik"]
# Wed, 29 Nov 2023 23:16:59 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v3.0.0-beta5 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f7bb9e009deb881cb90e8b4318258e03882de9bc9b312b763654b59cd13d0bb`  
		Last Modified: Tue, 14 Nov 2023 19:53:30 GMT  
		Size: 406.8 MB (406811201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce7a1cc914f0f5e059bfdf02906a6e052b1c97cebaf91eb6c2fd835cfddebda2`  
		Last Modified: Thu, 16 Nov 2023 02:26:46 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65d3a54963132deb3b7e269bda91707f12702256902f4c90d487ccb21b9d558a`  
		Last Modified: Wed, 29 Nov 2023 23:17:45 GMT  
		Size: 41.8 MB (41825821 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbce753338c510a600c4f528fabd498bd13a6342d0cd4f58552ee481c98faf41`  
		Last Modified: Wed, 29 Nov 2023 23:17:35 GMT  
		Size: 1.3 KB (1293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41c981bb20ef7dfa9d3f71feb1f2448764c30f56e450431f1c52686bdd4b87de`  
		Last Modified: Wed, 29 Nov 2023 23:17:36 GMT  
		Size: 1.3 KB (1293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b828c19e9a4c0fd32592a6e14895b39c96566702494253d5f316348902749062`  
		Last Modified: Wed, 29 Nov 2023 23:17:35 GMT  
		Size: 1.3 KB (1290 bytes)  
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
$ docker pull traefik@sha256:b0c7a98486b0ac8e13a2e2320d452a7464533382cbc252abd449cbb6150737a8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.5122; amd64

### `traefik:v3.0.0-beta5-windowsservercore-1809` - windows version 10.0.17763.5122; amd64

```console
$ docker pull traefik@sha256:7e85e697df9033b16fc2f80a00efcb8ac1f717d482f4759a1896ea82b46a1f06
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.1 GB (2099262676 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c790457d2785c38271eccfb5d1a985e2f189d84763d92a8980f1a889f90694f8`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Thu, 09 Nov 2023 17:56:40 GMT
RUN Install update 10.0.17763.5122
# Thu, 16 Nov 2023 01:37:58 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 29 Nov 2023 23:16:56 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/traefik/traefik/releases/download/v3.0.0-beta5/traefik_v3.0.0-beta5_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Wed, 29 Nov 2023 23:16:58 GMT
EXPOSE 80
# Wed, 29 Nov 2023 23:16:58 GMT
ENTRYPOINT ["/traefik"]
# Wed, 29 Nov 2023 23:16:59 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v3.0.0-beta5 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f7bb9e009deb881cb90e8b4318258e03882de9bc9b312b763654b59cd13d0bb`  
		Last Modified: Tue, 14 Nov 2023 19:53:30 GMT  
		Size: 406.8 MB (406811201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce7a1cc914f0f5e059bfdf02906a6e052b1c97cebaf91eb6c2fd835cfddebda2`  
		Last Modified: Thu, 16 Nov 2023 02:26:46 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65d3a54963132deb3b7e269bda91707f12702256902f4c90d487ccb21b9d558a`  
		Last Modified: Wed, 29 Nov 2023 23:17:45 GMT  
		Size: 41.8 MB (41825821 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbce753338c510a600c4f528fabd498bd13a6342d0cd4f58552ee481c98faf41`  
		Last Modified: Wed, 29 Nov 2023 23:17:35 GMT  
		Size: 1.3 KB (1293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41c981bb20ef7dfa9d3f71feb1f2448764c30f56e450431f1c52686bdd4b87de`  
		Last Modified: Wed, 29 Nov 2023 23:17:36 GMT  
		Size: 1.3 KB (1293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b828c19e9a4c0fd32592a6e14895b39c96566702494253d5f316348902749062`  
		Last Modified: Wed, 29 Nov 2023 23:17:35 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:windowsservercore-1809`

```console
$ docker pull traefik@sha256:4009a9c08e8ff3f3a8215cfc2bcce0355913c9800985c58828d1c7cba68572d6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.5122; amd64

### `traefik:windowsservercore-1809` - windows version 10.0.17763.5122; amd64

```console
$ docker pull traefik@sha256:3f007c45153ec0b2e3abe2b3c7c09b093532d0e198ef4b673e4ddd07bf87ea62
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.1 GB (2098146309 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:84386f59fd9c10dc0607ccebed700b43ed3f66ebfbc4b235398ca2a53bb6dce2`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Thu, 09 Nov 2023 17:56:40 GMT
RUN Install update 10.0.17763.5122
# Thu, 16 Nov 2023 01:37:58 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 29 Nov 2023 02:37:05 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/traefik/traefik/releases/download/v2.10.6/traefik_v2.10.6_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Wed, 29 Nov 2023 02:37:06 GMT
EXPOSE 80
# Wed, 29 Nov 2023 02:37:07 GMT
ENTRYPOINT ["/traefik"]
# Wed, 29 Nov 2023 02:37:08 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.10.6 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f7bb9e009deb881cb90e8b4318258e03882de9bc9b312b763654b59cd13d0bb`  
		Last Modified: Tue, 14 Nov 2023 19:53:30 GMT  
		Size: 406.8 MB (406811201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce7a1cc914f0f5e059bfdf02906a6e052b1c97cebaf91eb6c2fd835cfddebda2`  
		Last Modified: Thu, 16 Nov 2023 02:26:46 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fba9e80c0146453b6de8f35aea2ae18481cf6436bd532c51c90bd2e049433406`  
		Last Modified: Wed, 29 Nov 2023 02:37:46 GMT  
		Size: 40.7 MB (40709104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b54955fdd93b60b49068aadb447e1dbe066720ae5efaa7a315e4592abdd138b0`  
		Last Modified: Wed, 29 Nov 2023 02:37:37 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:463cbb8cb23bb46d13942b85ea410666ef2e97489fb170a77eeaa91dd2f7ae9f`  
		Last Modified: Wed, 29 Nov 2023 02:37:37 GMT  
		Size: 1.4 KB (1391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fb9c1cd767d2004163dd2c4b6bb806605d40ff4f8fa90589edef410642f5e41`  
		Last Modified: Wed, 29 Nov 2023 02:37:37 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
