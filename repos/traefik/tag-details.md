<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `traefik`

-	[`traefik:1.7`](#traefik17)
-	[`traefik:1.7.28`](#traefik1728)
-	[`traefik:1.7.28-alpine`](#traefik1728-alpine)
-	[`traefik:1.7.28-windowsservercore-1809`](#traefik1728-windowsservercore-1809)
-	[`traefik:1.7-alpine`](#traefik17-alpine)
-	[`traefik:1.7-windowsservercore-1809`](#traefik17-windowsservercore-1809)
-	[`traefik:2.4`](#traefik24)
-	[`traefik:2.4.1`](#traefik241)
-	[`traefik:2.4.1-windowsservercore-1809`](#traefik241-windowsservercore-1809)
-	[`traefik:2.4-windowsservercore-1809`](#traefik24-windowsservercore-1809)
-	[`traefik:latest`](#traefiklatest)
-	[`traefik:livarot`](#traefiklivarot)
-	[`traefik:livarot-windowsservercore-1809`](#traefiklivarot-windowsservercore-1809)
-	[`traefik:maroilles`](#traefikmaroilles)
-	[`traefik:maroilles-alpine`](#traefikmaroilles-alpine)
-	[`traefik:maroilles-windowsservercore-1809`](#traefikmaroilles-windowsservercore-1809)
-	[`traefik:v1.7`](#traefikv17)
-	[`traefik:v1.7.28`](#traefikv1728)
-	[`traefik:v1.7.28-alpine`](#traefikv1728-alpine)
-	[`traefik:v1.7.28-windowsservercore-1809`](#traefikv1728-windowsservercore-1809)
-	[`traefik:v1.7-alpine`](#traefikv17-alpine)
-	[`traefik:v1.7-windowsservercore-1809`](#traefikv17-windowsservercore-1809)
-	[`traefik:v2.4`](#traefikv24)
-	[`traefik:v2.4.1`](#traefikv241)
-	[`traefik:v2.4.1-windowsservercore-1809`](#traefikv241-windowsservercore-1809)
-	[`traefik:v2.4-windowsservercore-1809`](#traefikv24-windowsservercore-1809)
-	[`traefik:windowsservercore-1809`](#traefikwindowsservercore-1809)

## `traefik:1.7`

```console
$ docker pull traefik@sha256:998fc0cce3df0fe066005d6e94a7fa8b20749155fb54b4ebd1603e039b842feb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:1.7` - linux; amd64

```console
$ docker pull traefik@sha256:154e065982592220c9355925d9e60348eec6850418754ee76840f83501341b00
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **21.6 MB (21553283 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d2d67ddf1c8b647742ebb1ea0d3edb163dff028640b772832fa325b6b7df830f`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Thu, 17 Dec 2020 00:48:11 GMT
COPY file:cd6264d9a7514a8fbc3eb7b400566d36178794d2b757959812cc3abc6f13a97b in /etc/ssl/certs/ 
# Thu, 17 Dec 2020 00:48:11 GMT
COPY dir:83da415af0ff24b3b9d10f857aa8c724a3bc93523f3e047b827e7554fe1f9e08 in /usr/share/ 
# Wed, 13 Jan 2021 22:29:46 GMT
COPY file:94b9997cc55c7732c9fc173c119f980e4a38eba20b96a90170a3d7fade75f0eb in / 
# Wed, 13 Jan 2021 22:29:47 GMT
EXPOSE 80
# Wed, 13 Jan 2021 22:29:47 GMT
VOLUME [/tmp]
# Wed, 13 Jan 2021 22:29:47 GMT
ENTRYPOINT ["/traefik"]
# Wed, 13 Jan 2021 22:29:47 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.28 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:79de75e85675fa9abbac17b57205d3e0dfcf2bd2fc4cbc194f2aaf917435425e`  
		Last Modified: Thu, 17 Dec 2020 00:49:17 GMT  
		Size: 130.9 KB (130872 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f0e925284bb6370a549da51637ed98a8e574317473e082cc4be745d87327c7f`  
		Last Modified: Thu, 17 Dec 2020 00:49:18 GMT  
		Size: 306.4 KB (306411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81848bd29c493bb51f93a0bf98cf3958436af2128b6890d7a28a35b7dfc352c0`  
		Last Modified: Wed, 13 Jan 2021 22:30:48 GMT  
		Size: 21.1 MB (21116000 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:1.7` - linux; arm variant v6

```console
$ docker pull traefik@sha256:2f69dff9f3e67a011f08fc6a59fc3f72aa26533b5b9c8cd127e1f90948cbaf09
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **20.2 MB (20205544 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:da195dbaa64e13483787db1f21a4e602751bd363ac5c6e594e5e17c1f2420aec`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Thu, 17 Dec 2020 00:26:47 GMT
COPY file:cd6264d9a7514a8fbc3eb7b400566d36178794d2b757959812cc3abc6f13a97b in /etc/ssl/certs/ 
# Thu, 17 Dec 2020 00:26:48 GMT
COPY dir:83da415af0ff24b3b9d10f857aa8c724a3bc93523f3e047b827e7554fe1f9e08 in /usr/share/ 
# Wed, 13 Jan 2021 21:57:06 GMT
COPY file:3d9c1552db5b4c73ac7fe21268eeb20506f000d2e59d7be76697f45a50d32c64 in / 
# Wed, 13 Jan 2021 21:57:07 GMT
EXPOSE 80
# Wed, 13 Jan 2021 21:57:08 GMT
VOLUME [/tmp]
# Wed, 13 Jan 2021 21:57:09 GMT
ENTRYPOINT ["/traefik"]
# Wed, 13 Jan 2021 21:57:09 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.28 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:26c529e82b09c489524aa4f787754320793a95eb7aa7eaf306c517b76818ec25`  
		Last Modified: Thu, 17 Dec 2020 00:28:41 GMT  
		Size: 130.9 KB (130873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4adc6fb65827756c9d95005162623d443b2bd3e445269bcb1a7006e080726d3c`  
		Last Modified: Thu, 17 Dec 2020 00:28:41 GMT  
		Size: 306.5 KB (306458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0280c8ba5c59856146b5130ce0c0eb8b83b9dcc2dea1d69991723680815054f`  
		Last Modified: Wed, 13 Jan 2021 21:58:11 GMT  
		Size: 19.8 MB (19768213 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:1.7` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:468570d210f86c4366e666dac62c34b3054c230ee0b4d61c36e37ed276550b39
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **19.9 MB (19923388 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:13fff7cc610524cb77e4767eb66f534053cc0f45853e096fb250937594f9913d`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Thu, 17 Dec 2020 00:27:56 GMT
COPY file:cd6264d9a7514a8fbc3eb7b400566d36178794d2b757959812cc3abc6f13a97b in /etc/ssl/certs/ 
# Thu, 17 Dec 2020 00:27:58 GMT
COPY dir:83da415af0ff24b3b9d10f857aa8c724a3bc93523f3e047b827e7554fe1f9e08 in /usr/share/ 
# Wed, 13 Jan 2021 21:46:55 GMT
COPY file:6bab4a8fc3d272fc29bc5ff42634cb12785fea9e23b0cf50f077702217bb6c03 in / 
# Wed, 13 Jan 2021 21:46:56 GMT
EXPOSE 80
# Wed, 13 Jan 2021 21:46:56 GMT
VOLUME [/tmp]
# Wed, 13 Jan 2021 21:46:57 GMT
ENTRYPOINT ["/traefik"]
# Wed, 13 Jan 2021 21:46:58 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.28 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:7dccf22d113d483cac839141f2028cbf6ac2e0c6aa4a1716c5e7b575b162028c`  
		Last Modified: Thu, 17 Dec 2020 00:29:55 GMT  
		Size: 130.9 KB (130873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c32c03119dbb32c844511340cb40a21ba5a56b90862cf603dec2e49cf5ab20d`  
		Last Modified: Thu, 17 Dec 2020 00:29:57 GMT  
		Size: 306.5 KB (306466 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41f7f3a967c907bfe4aeb896ba6da80cfaf9bce19fcb39b51a6378b00596760d`  
		Last Modified: Wed, 13 Jan 2021 21:47:50 GMT  
		Size: 19.5 MB (19486049 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:1.7.28`

```console
$ docker pull traefik@sha256:998fc0cce3df0fe066005d6e94a7fa8b20749155fb54b4ebd1603e039b842feb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:1.7.28` - linux; amd64

```console
$ docker pull traefik@sha256:154e065982592220c9355925d9e60348eec6850418754ee76840f83501341b00
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **21.6 MB (21553283 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d2d67ddf1c8b647742ebb1ea0d3edb163dff028640b772832fa325b6b7df830f`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Thu, 17 Dec 2020 00:48:11 GMT
COPY file:cd6264d9a7514a8fbc3eb7b400566d36178794d2b757959812cc3abc6f13a97b in /etc/ssl/certs/ 
# Thu, 17 Dec 2020 00:48:11 GMT
COPY dir:83da415af0ff24b3b9d10f857aa8c724a3bc93523f3e047b827e7554fe1f9e08 in /usr/share/ 
# Wed, 13 Jan 2021 22:29:46 GMT
COPY file:94b9997cc55c7732c9fc173c119f980e4a38eba20b96a90170a3d7fade75f0eb in / 
# Wed, 13 Jan 2021 22:29:47 GMT
EXPOSE 80
# Wed, 13 Jan 2021 22:29:47 GMT
VOLUME [/tmp]
# Wed, 13 Jan 2021 22:29:47 GMT
ENTRYPOINT ["/traefik"]
# Wed, 13 Jan 2021 22:29:47 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.28 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:79de75e85675fa9abbac17b57205d3e0dfcf2bd2fc4cbc194f2aaf917435425e`  
		Last Modified: Thu, 17 Dec 2020 00:49:17 GMT  
		Size: 130.9 KB (130872 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f0e925284bb6370a549da51637ed98a8e574317473e082cc4be745d87327c7f`  
		Last Modified: Thu, 17 Dec 2020 00:49:18 GMT  
		Size: 306.4 KB (306411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81848bd29c493bb51f93a0bf98cf3958436af2128b6890d7a28a35b7dfc352c0`  
		Last Modified: Wed, 13 Jan 2021 22:30:48 GMT  
		Size: 21.1 MB (21116000 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:1.7.28` - linux; arm variant v6

```console
$ docker pull traefik@sha256:2f69dff9f3e67a011f08fc6a59fc3f72aa26533b5b9c8cd127e1f90948cbaf09
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **20.2 MB (20205544 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:da195dbaa64e13483787db1f21a4e602751bd363ac5c6e594e5e17c1f2420aec`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Thu, 17 Dec 2020 00:26:47 GMT
COPY file:cd6264d9a7514a8fbc3eb7b400566d36178794d2b757959812cc3abc6f13a97b in /etc/ssl/certs/ 
# Thu, 17 Dec 2020 00:26:48 GMT
COPY dir:83da415af0ff24b3b9d10f857aa8c724a3bc93523f3e047b827e7554fe1f9e08 in /usr/share/ 
# Wed, 13 Jan 2021 21:57:06 GMT
COPY file:3d9c1552db5b4c73ac7fe21268eeb20506f000d2e59d7be76697f45a50d32c64 in / 
# Wed, 13 Jan 2021 21:57:07 GMT
EXPOSE 80
# Wed, 13 Jan 2021 21:57:08 GMT
VOLUME [/tmp]
# Wed, 13 Jan 2021 21:57:09 GMT
ENTRYPOINT ["/traefik"]
# Wed, 13 Jan 2021 21:57:09 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.28 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:26c529e82b09c489524aa4f787754320793a95eb7aa7eaf306c517b76818ec25`  
		Last Modified: Thu, 17 Dec 2020 00:28:41 GMT  
		Size: 130.9 KB (130873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4adc6fb65827756c9d95005162623d443b2bd3e445269bcb1a7006e080726d3c`  
		Last Modified: Thu, 17 Dec 2020 00:28:41 GMT  
		Size: 306.5 KB (306458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0280c8ba5c59856146b5130ce0c0eb8b83b9dcc2dea1d69991723680815054f`  
		Last Modified: Wed, 13 Jan 2021 21:58:11 GMT  
		Size: 19.8 MB (19768213 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:1.7.28` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:468570d210f86c4366e666dac62c34b3054c230ee0b4d61c36e37ed276550b39
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **19.9 MB (19923388 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:13fff7cc610524cb77e4767eb66f534053cc0f45853e096fb250937594f9913d`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Thu, 17 Dec 2020 00:27:56 GMT
COPY file:cd6264d9a7514a8fbc3eb7b400566d36178794d2b757959812cc3abc6f13a97b in /etc/ssl/certs/ 
# Thu, 17 Dec 2020 00:27:58 GMT
COPY dir:83da415af0ff24b3b9d10f857aa8c724a3bc93523f3e047b827e7554fe1f9e08 in /usr/share/ 
# Wed, 13 Jan 2021 21:46:55 GMT
COPY file:6bab4a8fc3d272fc29bc5ff42634cb12785fea9e23b0cf50f077702217bb6c03 in / 
# Wed, 13 Jan 2021 21:46:56 GMT
EXPOSE 80
# Wed, 13 Jan 2021 21:46:56 GMT
VOLUME [/tmp]
# Wed, 13 Jan 2021 21:46:57 GMT
ENTRYPOINT ["/traefik"]
# Wed, 13 Jan 2021 21:46:58 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.28 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:7dccf22d113d483cac839141f2028cbf6ac2e0c6aa4a1716c5e7b575b162028c`  
		Last Modified: Thu, 17 Dec 2020 00:29:55 GMT  
		Size: 130.9 KB (130873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c32c03119dbb32c844511340cb40a21ba5a56b90862cf603dec2e49cf5ab20d`  
		Last Modified: Thu, 17 Dec 2020 00:29:57 GMT  
		Size: 306.5 KB (306466 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41f7f3a967c907bfe4aeb896ba6da80cfaf9bce19fcb39b51a6378b00596760d`  
		Last Modified: Wed, 13 Jan 2021 21:47:50 GMT  
		Size: 19.5 MB (19486049 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:1.7.28-alpine`

```console
$ docker pull traefik@sha256:d232a757f6c487484b3640973fbb0287e747e6b357bc1dc75faa07b26da14a5f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:1.7.28-alpine` - linux; amd64

```console
$ docker pull traefik@sha256:cb19d2e6f6575fb121eb2181cbd50f783c1995bf515cba8c7bbab7d9b6859949
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **24.6 MB (24603200 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d9ecef4edf395a65a22e7b3c46ec4b16c869c1a5386a1ea0305132dc68266f04`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 17 Dec 2020 00:19:49 GMT
ADD file:8ed80010e443da19d72546bcee9a35e0a8d244c72052b1994610bf5939d479c2 in / 
# Thu, 17 Dec 2020 00:19:49 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 00:47:33 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 13 Jan 2021 22:29:27 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/traefik/traefik/releases/download/v1.7.28/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Wed, 13 Jan 2021 22:29:27 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 13 Jan 2021 22:29:27 GMT
EXPOSE 80
# Wed, 13 Jan 2021 22:29:27 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 13 Jan 2021 22:29:28 GMT
CMD ["traefik"]
# Wed, 13 Jan 2021 22:29:28 GMT
LABEL org.opencontainers.image.vendor=traefik org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.28 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:0a6724ff3fcd51338afdfdc2b1d4ffd04569818e31efad957213d67c29b45101`  
		Last Modified: Thu, 17 Dec 2020 00:20:26 GMT  
		Size: 2.8 MB (2814864 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64d0c2f48fede0de57585b470af3e8e9aa5534db90642859512370fa53ffac21`  
		Last Modified: Thu, 17 Dec 2020 00:48:37 GMT  
		Size: 671.7 KB (671697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce8923725f26216ece246718b634aabb038e3ba78292d388ebb7350cc0d89ba1`  
		Last Modified: Wed, 13 Jan 2021 22:30:25 GMT  
		Size: 21.1 MB (21116271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f8abe3b22d27fbf46de589e10d21107bd248a725e59317b3fc6a78a83e9c940`  
		Last Modified: Wed, 13 Jan 2021 22:30:19 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:1.7.28-alpine` - linux; arm variant v6

```console
$ docker pull traefik@sha256:198e33555ab98a4ea7b448b1f818b9663ab2f8fe98f0966543390a711e55692d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.1 MB (23064299 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:92898625b48315d465f9a4d3ad8e32c8b224bb4617bff335d0840bbd9ce1aced`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 16 Dec 2020 23:49:53 GMT
ADD file:e3a6f7566ee3c2ba61d27d801d3522e045a4be64a42f32ee52d933b68338d06f in / 
# Wed, 16 Dec 2020 23:49:55 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 00:25:55 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 13 Jan 2021 21:56:46 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/traefik/traefik/releases/download/v1.7.28/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Wed, 13 Jan 2021 21:56:47 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 13 Jan 2021 21:56:48 GMT
EXPOSE 80
# Wed, 13 Jan 2021 21:56:48 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 13 Jan 2021 21:56:49 GMT
CMD ["traefik"]
# Wed, 13 Jan 2021 21:56:49 GMT
LABEL org.opencontainers.image.vendor=traefik org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.28 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:56fec67ad66eea034cf5b7d0d0ffd355c0fe87611bad132ac5a952fcaa52138b`  
		Last Modified: Wed, 16 Dec 2020 23:50:34 GMT  
		Size: 2.6 MB (2620769 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab096bb24791df9de14fbfc840265a32c0d9f7be463db3a782da6095c0e6ad5b`  
		Last Modified: Thu, 17 Dec 2020 00:27:24 GMT  
		Size: 674.9 KB (674902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:102471939d830c2c1e2668e0dd48049fc6ce2f332ead14922e8a55086f8816ef`  
		Last Modified: Wed, 13 Jan 2021 21:57:48 GMT  
		Size: 19.8 MB (19768260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29a399e8ce2234a61da5e35bf382eefe32e24435b8c5805b773299d16a01b022`  
		Last Modified: Wed, 13 Jan 2021 21:57:42 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:1.7.28-alpine` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:a144e4ba9554f68e6903986ca95090991e87d3c7a3e45809bfd602a5bda85a3c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **22.9 MB (22884874 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:24c65bf1525b68d03c1cc5d512338cf2608b5742b1e06e6ea57c492e61afee7a`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 16 Dec 2020 23:40:37 GMT
ADD file:47bb1b85a4eb4d0b355ae89ec5c71c09e2c2b7e21e1851a2896365eb17134f57 in / 
# Wed, 16 Dec 2020 23:40:39 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 00:27:02 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 13 Jan 2021 21:46:38 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/traefik/traefik/releases/download/v1.7.28/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Wed, 13 Jan 2021 21:46:39 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 13 Jan 2021 21:46:39 GMT
EXPOSE 80
# Wed, 13 Jan 2021 21:46:40 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 13 Jan 2021 21:46:41 GMT
CMD ["traefik"]
# Wed, 13 Jan 2021 21:46:41 GMT
LABEL org.opencontainers.image.vendor=traefik org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.28 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:20d8a246443a66e74e17f2a0e81a51fe774876ca0c2676691c37ee1b0e4d3cd5`  
		Last Modified: Wed, 16 Dec 2020 23:41:20 GMT  
		Size: 2.7 MB (2725216 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:278abd308a18c136f69dcabbba1dc64486ebdad665d4a2f4ab14d2826ec08b06`  
		Last Modified: Thu, 17 Dec 2020 00:28:38 GMT  
		Size: 673.2 KB (673246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e50dc3ca8b514cac3bfbf2a6303d6be654d1a94f584f6f24d4e62522b80bd36b`  
		Last Modified: Wed, 13 Jan 2021 21:47:33 GMT  
		Size: 19.5 MB (19486044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d4205a3b9bbaa8f65f3bd5780aeb6e4cc761d5f7d6de7cb70588b41ed018c72`  
		Last Modified: Wed, 13 Jan 2021 21:47:27 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:1.7.28-windowsservercore-1809`

```console
$ docker pull traefik@sha256:8f2b9d477c5d31806d427f5dad762d9f448c131bb284641f3977b914e655afd7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1697; amd64

### `traefik:1.7.28-windowsservercore-1809` - windows version 10.0.17763.1697; amd64

```console
$ docker pull traefik@sha256:91b9a8ca83df9afc2b41003518d4b4f9d8e8a21f77880fd74d543670c7ab4da9
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2466262882 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6962de1a7e3fc419a74eb2ea94e4c40359d9f53a93caec6bd1e61f1944ccf282`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 08 Jan 2021 08:50:52 GMT
RUN Install update 1809-amd64
# Wed, 13 Jan 2021 13:13:16 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 14 Jan 2021 01:16:20 GMT
RUN Invoke-WebRequest     -Uri "https://github.com/traefik/traefik/releases/download/v1.7.28/traefik_windows-amd64.exe"     -OutFile "/traefik.exe"
# Thu, 14 Jan 2021 01:16:24 GMT
EXPOSE 80
# Thu, 14 Jan 2021 01:16:25 GMT
ENTRYPOINT ["/traefik"]
# Thu, 14 Jan 2021 01:16:26 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.28 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:4dcc9a9b9e680514ef3fdfcc2ce08a3768f9e412703faa137f4a7c8297600052`  
		Size: 717.4 MB (717439216 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e00081a98bb2679c3c5f469e09d475980133a20987f9cae4cf4f7aedf59f9d8f`  
		Last Modified: Wed, 13 Jan 2021 13:17:19 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84697de3c7d0310176f36e2fe57e5688d23e486eb5b5febf6dbf860e763d1750`  
		Last Modified: Thu, 14 Jan 2021 01:17:09 GMT  
		Size: 30.5 MB (30486249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:069ca4204690196a12b1d26a1b7d9b54c2d8fc7db082a3a4a9e21bfdf55d63d1`  
		Last Modified: Thu, 14 Jan 2021 01:17:02 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adaebdd4a9fa6db73d7167e0d944af020e0ddfe54da3ed92807a14054a53d669`  
		Last Modified: Thu, 14 Jan 2021 01:17:01 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:454fe39b046d9fedbd9e0b3f698556592463406933b790b272dd909d5bd90d53`  
		Last Modified: Thu, 14 Jan 2021 01:17:02 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:1.7-alpine`

```console
$ docker pull traefik@sha256:d232a757f6c487484b3640973fbb0287e747e6b357bc1dc75faa07b26da14a5f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:1.7-alpine` - linux; amd64

```console
$ docker pull traefik@sha256:cb19d2e6f6575fb121eb2181cbd50f783c1995bf515cba8c7bbab7d9b6859949
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **24.6 MB (24603200 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d9ecef4edf395a65a22e7b3c46ec4b16c869c1a5386a1ea0305132dc68266f04`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 17 Dec 2020 00:19:49 GMT
ADD file:8ed80010e443da19d72546bcee9a35e0a8d244c72052b1994610bf5939d479c2 in / 
# Thu, 17 Dec 2020 00:19:49 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 00:47:33 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 13 Jan 2021 22:29:27 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/traefik/traefik/releases/download/v1.7.28/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Wed, 13 Jan 2021 22:29:27 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 13 Jan 2021 22:29:27 GMT
EXPOSE 80
# Wed, 13 Jan 2021 22:29:27 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 13 Jan 2021 22:29:28 GMT
CMD ["traefik"]
# Wed, 13 Jan 2021 22:29:28 GMT
LABEL org.opencontainers.image.vendor=traefik org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.28 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:0a6724ff3fcd51338afdfdc2b1d4ffd04569818e31efad957213d67c29b45101`  
		Last Modified: Thu, 17 Dec 2020 00:20:26 GMT  
		Size: 2.8 MB (2814864 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64d0c2f48fede0de57585b470af3e8e9aa5534db90642859512370fa53ffac21`  
		Last Modified: Thu, 17 Dec 2020 00:48:37 GMT  
		Size: 671.7 KB (671697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce8923725f26216ece246718b634aabb038e3ba78292d388ebb7350cc0d89ba1`  
		Last Modified: Wed, 13 Jan 2021 22:30:25 GMT  
		Size: 21.1 MB (21116271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f8abe3b22d27fbf46de589e10d21107bd248a725e59317b3fc6a78a83e9c940`  
		Last Modified: Wed, 13 Jan 2021 22:30:19 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:1.7-alpine` - linux; arm variant v6

```console
$ docker pull traefik@sha256:198e33555ab98a4ea7b448b1f818b9663ab2f8fe98f0966543390a711e55692d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.1 MB (23064299 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:92898625b48315d465f9a4d3ad8e32c8b224bb4617bff335d0840bbd9ce1aced`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 16 Dec 2020 23:49:53 GMT
ADD file:e3a6f7566ee3c2ba61d27d801d3522e045a4be64a42f32ee52d933b68338d06f in / 
# Wed, 16 Dec 2020 23:49:55 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 00:25:55 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 13 Jan 2021 21:56:46 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/traefik/traefik/releases/download/v1.7.28/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Wed, 13 Jan 2021 21:56:47 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 13 Jan 2021 21:56:48 GMT
EXPOSE 80
# Wed, 13 Jan 2021 21:56:48 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 13 Jan 2021 21:56:49 GMT
CMD ["traefik"]
# Wed, 13 Jan 2021 21:56:49 GMT
LABEL org.opencontainers.image.vendor=traefik org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.28 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:56fec67ad66eea034cf5b7d0d0ffd355c0fe87611bad132ac5a952fcaa52138b`  
		Last Modified: Wed, 16 Dec 2020 23:50:34 GMT  
		Size: 2.6 MB (2620769 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab096bb24791df9de14fbfc840265a32c0d9f7be463db3a782da6095c0e6ad5b`  
		Last Modified: Thu, 17 Dec 2020 00:27:24 GMT  
		Size: 674.9 KB (674902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:102471939d830c2c1e2668e0dd48049fc6ce2f332ead14922e8a55086f8816ef`  
		Last Modified: Wed, 13 Jan 2021 21:57:48 GMT  
		Size: 19.8 MB (19768260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29a399e8ce2234a61da5e35bf382eefe32e24435b8c5805b773299d16a01b022`  
		Last Modified: Wed, 13 Jan 2021 21:57:42 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:1.7-alpine` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:a144e4ba9554f68e6903986ca95090991e87d3c7a3e45809bfd602a5bda85a3c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **22.9 MB (22884874 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:24c65bf1525b68d03c1cc5d512338cf2608b5742b1e06e6ea57c492e61afee7a`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 16 Dec 2020 23:40:37 GMT
ADD file:47bb1b85a4eb4d0b355ae89ec5c71c09e2c2b7e21e1851a2896365eb17134f57 in / 
# Wed, 16 Dec 2020 23:40:39 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 00:27:02 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 13 Jan 2021 21:46:38 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/traefik/traefik/releases/download/v1.7.28/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Wed, 13 Jan 2021 21:46:39 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 13 Jan 2021 21:46:39 GMT
EXPOSE 80
# Wed, 13 Jan 2021 21:46:40 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 13 Jan 2021 21:46:41 GMT
CMD ["traefik"]
# Wed, 13 Jan 2021 21:46:41 GMT
LABEL org.opencontainers.image.vendor=traefik org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.28 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:20d8a246443a66e74e17f2a0e81a51fe774876ca0c2676691c37ee1b0e4d3cd5`  
		Last Modified: Wed, 16 Dec 2020 23:41:20 GMT  
		Size: 2.7 MB (2725216 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:278abd308a18c136f69dcabbba1dc64486ebdad665d4a2f4ab14d2826ec08b06`  
		Last Modified: Thu, 17 Dec 2020 00:28:38 GMT  
		Size: 673.2 KB (673246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e50dc3ca8b514cac3bfbf2a6303d6be654d1a94f584f6f24d4e62522b80bd36b`  
		Last Modified: Wed, 13 Jan 2021 21:47:33 GMT  
		Size: 19.5 MB (19486044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d4205a3b9bbaa8f65f3bd5780aeb6e4cc761d5f7d6de7cb70588b41ed018c72`  
		Last Modified: Wed, 13 Jan 2021 21:47:27 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:1.7-windowsservercore-1809`

```console
$ docker pull traefik@sha256:8f2b9d477c5d31806d427f5dad762d9f448c131bb284641f3977b914e655afd7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1697; amd64

### `traefik:1.7-windowsservercore-1809` - windows version 10.0.17763.1697; amd64

```console
$ docker pull traefik@sha256:91b9a8ca83df9afc2b41003518d4b4f9d8e8a21f77880fd74d543670c7ab4da9
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2466262882 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6962de1a7e3fc419a74eb2ea94e4c40359d9f53a93caec6bd1e61f1944ccf282`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 08 Jan 2021 08:50:52 GMT
RUN Install update 1809-amd64
# Wed, 13 Jan 2021 13:13:16 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 14 Jan 2021 01:16:20 GMT
RUN Invoke-WebRequest     -Uri "https://github.com/traefik/traefik/releases/download/v1.7.28/traefik_windows-amd64.exe"     -OutFile "/traefik.exe"
# Thu, 14 Jan 2021 01:16:24 GMT
EXPOSE 80
# Thu, 14 Jan 2021 01:16:25 GMT
ENTRYPOINT ["/traefik"]
# Thu, 14 Jan 2021 01:16:26 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.28 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:4dcc9a9b9e680514ef3fdfcc2ce08a3768f9e412703faa137f4a7c8297600052`  
		Size: 717.4 MB (717439216 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e00081a98bb2679c3c5f469e09d475980133a20987f9cae4cf4f7aedf59f9d8f`  
		Last Modified: Wed, 13 Jan 2021 13:17:19 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84697de3c7d0310176f36e2fe57e5688d23e486eb5b5febf6dbf860e763d1750`  
		Last Modified: Thu, 14 Jan 2021 01:17:09 GMT  
		Size: 30.5 MB (30486249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:069ca4204690196a12b1d26a1b7d9b54c2d8fc7db082a3a4a9e21bfdf55d63d1`  
		Last Modified: Thu, 14 Jan 2021 01:17:02 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adaebdd4a9fa6db73d7167e0d944af020e0ddfe54da3ed92807a14054a53d669`  
		Last Modified: Thu, 14 Jan 2021 01:17:01 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:454fe39b046d9fedbd9e0b3f698556592463406933b790b272dd909d5bd90d53`  
		Last Modified: Thu, 14 Jan 2021 01:17:02 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:2.4`

```console
$ docker pull traefik@sha256:482a48d4268f6edb38aa6934c74acf5d1f14ec2e7c5e813607ac18c958c62482
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:2.4` - linux; amd64

```console
$ docker pull traefik@sha256:3d2ba657bdec47749235c4a06e0b51d89e6a2a4c72dad70c9fd5f9496c68d871
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.0 MB (29043146 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7dcdc37f2b5f338b1a51a6739a905148dd1c1b189f3d97dd205fced1797f37a0`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 17 Dec 2020 00:19:49 GMT
ADD file:8ed80010e443da19d72546bcee9a35e0a8d244c72052b1994610bf5939d479c2 in / 
# Thu, 17 Dec 2020 00:19:49 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 00:47:33 GMT
RUN apk --no-cache add ca-certificates tzdata
# Mon, 01 Feb 2021 20:36:23 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.4.1/traefik_v2.4.1_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Mon, 01 Feb 2021 20:36:23 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Mon, 01 Feb 2021 20:36:24 GMT
EXPOSE 80
# Mon, 01 Feb 2021 20:36:24 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 01 Feb 2021 20:36:24 GMT
CMD ["traefik"]
# Mon, 01 Feb 2021 20:36:24 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.4.1 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:0a6724ff3fcd51338afdfdc2b1d4ffd04569818e31efad957213d67c29b45101`  
		Last Modified: Thu, 17 Dec 2020 00:20:26 GMT  
		Size: 2.8 MB (2814864 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64d0c2f48fede0de57585b470af3e8e9aa5534db90642859512370fa53ffac21`  
		Last Modified: Thu, 17 Dec 2020 00:48:37 GMT  
		Size: 671.7 KB (671697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1516ade513da1a48f2452fb045c9f59dcb754ec8a45d295fb62c02ca3ce2fa24`  
		Last Modified: Mon, 01 Feb 2021 20:36:56 GMT  
		Size: 25.6 MB (25556218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1646cce883d51cde2f62db17c3ffca7a86fb6b363e190158baacb784df1cd067`  
		Last Modified: Mon, 01 Feb 2021 20:36:51 GMT  
		Size: 367.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:2.4` - linux; arm variant v6

```console
$ docker pull traefik@sha256:a784cf52ea56aea0b24a9906cb19b4b4378a93c7d883df4315cd2274006373ec
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.1 MB (27087182 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:791475a3abf40af6d79e4c48790e71f85dac37a4ff31bfdf59b305585c037bb3`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 16 Dec 2020 23:49:53 GMT
ADD file:e3a6f7566ee3c2ba61d27d801d3522e045a4be64a42f32ee52d933b68338d06f in / 
# Wed, 16 Dec 2020 23:49:55 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 00:25:55 GMT
RUN apk --no-cache add ca-certificates tzdata
# Mon, 01 Feb 2021 20:21:51 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.4.1/traefik_v2.4.1_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Mon, 01 Feb 2021 20:21:52 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Mon, 01 Feb 2021 20:21:54 GMT
EXPOSE 80
# Mon, 01 Feb 2021 20:21:57 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 01 Feb 2021 20:21:59 GMT
CMD ["traefik"]
# Mon, 01 Feb 2021 20:22:00 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.4.1 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:56fec67ad66eea034cf5b7d0d0ffd355c0fe87611bad132ac5a952fcaa52138b`  
		Last Modified: Wed, 16 Dec 2020 23:50:34 GMT  
		Size: 2.6 MB (2620769 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab096bb24791df9de14fbfc840265a32c0d9f7be463db3a782da6095c0e6ad5b`  
		Last Modified: Thu, 17 Dec 2020 00:27:24 GMT  
		Size: 674.9 KB (674902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0eb4fee172158a2a6626c7064a033878a7a6cfc5b3fee45c74d6d44e05bc9370`  
		Last Modified: Mon, 01 Feb 2021 20:22:38 GMT  
		Size: 23.8 MB (23791143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b36a51bbc86a42ed580e716a14368625f925ffe68f228ecaa6c1ee5d7705d560`  
		Last Modified: Mon, 01 Feb 2021 20:22:29 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:2.4` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:7353217d113ec6673f0215e2623b81af6251fbd4f7745078621617b498491b42
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.7 MB (26708518 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6688c1a122c4a87c308f5addeac11defec355c3db5836db65675df5c979340e2`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 16 Dec 2020 23:40:37 GMT
ADD file:47bb1b85a4eb4d0b355ae89ec5c71c09e2c2b7e21e1851a2896365eb17134f57 in / 
# Wed, 16 Dec 2020 23:40:39 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 00:27:02 GMT
RUN apk --no-cache add ca-certificates tzdata
# Mon, 01 Feb 2021 21:04:10 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.4.1/traefik_v2.4.1_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Mon, 01 Feb 2021 21:04:11 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Mon, 01 Feb 2021 21:04:11 GMT
EXPOSE 80
# Mon, 01 Feb 2021 21:04:12 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 01 Feb 2021 21:04:12 GMT
CMD ["traefik"]
# Mon, 01 Feb 2021 21:04:13 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.4.1 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:20d8a246443a66e74e17f2a0e81a51fe774876ca0c2676691c37ee1b0e4d3cd5`  
		Last Modified: Wed, 16 Dec 2020 23:41:20 GMT  
		Size: 2.7 MB (2725216 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:278abd308a18c136f69dcabbba1dc64486ebdad665d4a2f4ab14d2826ec08b06`  
		Last Modified: Thu, 17 Dec 2020 00:28:38 GMT  
		Size: 673.2 KB (673246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76f99e8acab44e0da3e7667fedfc874ddb6f2fa2bf1814aa29cbcd5f97d091c4`  
		Last Modified: Mon, 01 Feb 2021 21:04:49 GMT  
		Size: 23.3 MB (23309688 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f579f772bccf2955a27d99b4778f4f174e3fb78837376c77f98385cdcbe2bdce`  
		Last Modified: Mon, 01 Feb 2021 21:04:43 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:2.4.1`

```console
$ docker pull traefik@sha256:482a48d4268f6edb38aa6934c74acf5d1f14ec2e7c5e813607ac18c958c62482
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:2.4.1` - linux; amd64

```console
$ docker pull traefik@sha256:3d2ba657bdec47749235c4a06e0b51d89e6a2a4c72dad70c9fd5f9496c68d871
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.0 MB (29043146 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7dcdc37f2b5f338b1a51a6739a905148dd1c1b189f3d97dd205fced1797f37a0`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 17 Dec 2020 00:19:49 GMT
ADD file:8ed80010e443da19d72546bcee9a35e0a8d244c72052b1994610bf5939d479c2 in / 
# Thu, 17 Dec 2020 00:19:49 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 00:47:33 GMT
RUN apk --no-cache add ca-certificates tzdata
# Mon, 01 Feb 2021 20:36:23 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.4.1/traefik_v2.4.1_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Mon, 01 Feb 2021 20:36:23 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Mon, 01 Feb 2021 20:36:24 GMT
EXPOSE 80
# Mon, 01 Feb 2021 20:36:24 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 01 Feb 2021 20:36:24 GMT
CMD ["traefik"]
# Mon, 01 Feb 2021 20:36:24 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.4.1 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:0a6724ff3fcd51338afdfdc2b1d4ffd04569818e31efad957213d67c29b45101`  
		Last Modified: Thu, 17 Dec 2020 00:20:26 GMT  
		Size: 2.8 MB (2814864 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64d0c2f48fede0de57585b470af3e8e9aa5534db90642859512370fa53ffac21`  
		Last Modified: Thu, 17 Dec 2020 00:48:37 GMT  
		Size: 671.7 KB (671697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1516ade513da1a48f2452fb045c9f59dcb754ec8a45d295fb62c02ca3ce2fa24`  
		Last Modified: Mon, 01 Feb 2021 20:36:56 GMT  
		Size: 25.6 MB (25556218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1646cce883d51cde2f62db17c3ffca7a86fb6b363e190158baacb784df1cd067`  
		Last Modified: Mon, 01 Feb 2021 20:36:51 GMT  
		Size: 367.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:2.4.1` - linux; arm variant v6

```console
$ docker pull traefik@sha256:a784cf52ea56aea0b24a9906cb19b4b4378a93c7d883df4315cd2274006373ec
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.1 MB (27087182 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:791475a3abf40af6d79e4c48790e71f85dac37a4ff31bfdf59b305585c037bb3`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 16 Dec 2020 23:49:53 GMT
ADD file:e3a6f7566ee3c2ba61d27d801d3522e045a4be64a42f32ee52d933b68338d06f in / 
# Wed, 16 Dec 2020 23:49:55 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 00:25:55 GMT
RUN apk --no-cache add ca-certificates tzdata
# Mon, 01 Feb 2021 20:21:51 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.4.1/traefik_v2.4.1_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Mon, 01 Feb 2021 20:21:52 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Mon, 01 Feb 2021 20:21:54 GMT
EXPOSE 80
# Mon, 01 Feb 2021 20:21:57 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 01 Feb 2021 20:21:59 GMT
CMD ["traefik"]
# Mon, 01 Feb 2021 20:22:00 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.4.1 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:56fec67ad66eea034cf5b7d0d0ffd355c0fe87611bad132ac5a952fcaa52138b`  
		Last Modified: Wed, 16 Dec 2020 23:50:34 GMT  
		Size: 2.6 MB (2620769 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab096bb24791df9de14fbfc840265a32c0d9f7be463db3a782da6095c0e6ad5b`  
		Last Modified: Thu, 17 Dec 2020 00:27:24 GMT  
		Size: 674.9 KB (674902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0eb4fee172158a2a6626c7064a033878a7a6cfc5b3fee45c74d6d44e05bc9370`  
		Last Modified: Mon, 01 Feb 2021 20:22:38 GMT  
		Size: 23.8 MB (23791143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b36a51bbc86a42ed580e716a14368625f925ffe68f228ecaa6c1ee5d7705d560`  
		Last Modified: Mon, 01 Feb 2021 20:22:29 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:2.4.1` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:7353217d113ec6673f0215e2623b81af6251fbd4f7745078621617b498491b42
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.7 MB (26708518 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6688c1a122c4a87c308f5addeac11defec355c3db5836db65675df5c979340e2`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 16 Dec 2020 23:40:37 GMT
ADD file:47bb1b85a4eb4d0b355ae89ec5c71c09e2c2b7e21e1851a2896365eb17134f57 in / 
# Wed, 16 Dec 2020 23:40:39 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 00:27:02 GMT
RUN apk --no-cache add ca-certificates tzdata
# Mon, 01 Feb 2021 21:04:10 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.4.1/traefik_v2.4.1_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Mon, 01 Feb 2021 21:04:11 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Mon, 01 Feb 2021 21:04:11 GMT
EXPOSE 80
# Mon, 01 Feb 2021 21:04:12 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 01 Feb 2021 21:04:12 GMT
CMD ["traefik"]
# Mon, 01 Feb 2021 21:04:13 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.4.1 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:20d8a246443a66e74e17f2a0e81a51fe774876ca0c2676691c37ee1b0e4d3cd5`  
		Last Modified: Wed, 16 Dec 2020 23:41:20 GMT  
		Size: 2.7 MB (2725216 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:278abd308a18c136f69dcabbba1dc64486ebdad665d4a2f4ab14d2826ec08b06`  
		Last Modified: Thu, 17 Dec 2020 00:28:38 GMT  
		Size: 673.2 KB (673246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76f99e8acab44e0da3e7667fedfc874ddb6f2fa2bf1814aa29cbcd5f97d091c4`  
		Last Modified: Mon, 01 Feb 2021 21:04:49 GMT  
		Size: 23.3 MB (23309688 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f579f772bccf2955a27d99b4778f4f174e3fb78837376c77f98385cdcbe2bdce`  
		Last Modified: Mon, 01 Feb 2021 21:04:43 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:2.4.1-windowsservercore-1809`

```console
$ docker pull traefik@sha256:f8a909841f70c259ea7e5c4e4e6711fd047fafa7ca6be1114bc390e0ac69db02
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1697; amd64

### `traefik:2.4.1-windowsservercore-1809` - windows version 10.0.17763.1697; amd64

```console
$ docker pull traefik@sha256:6592087c3b637b852ccb83524da4e563fdbd1aa01c36c7dca55fa4154c908a9f
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2471089030 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1a4da9297c49ca2d742c3719308666352f9a5837f20529b203e86b3490850930`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 08 Jan 2021 08:50:52 GMT
RUN Install update 1809-amd64
# Wed, 13 Jan 2021 13:13:16 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Mon, 01 Feb 2021 20:14:38 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/traefik/traefik/releases/download/v2.4.1/traefik_v2.4.1_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Mon, 01 Feb 2021 20:14:39 GMT
EXPOSE 80
# Mon, 01 Feb 2021 20:14:40 GMT
ENTRYPOINT ["/traefik"]
# Mon, 01 Feb 2021 20:14:41 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.4.1 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:4dcc9a9b9e680514ef3fdfcc2ce08a3768f9e412703faa137f4a7c8297600052`  
		Size: 717.4 MB (717439216 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e00081a98bb2679c3c5f469e09d475980133a20987f9cae4cf4f7aedf59f9d8f`  
		Last Modified: Wed, 13 Jan 2021 13:17:19 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff2522d016390dfd18d8aeb8e2c6aff006cd1f9247bf87ead249db540db5125b`  
		Last Modified: Mon, 01 Feb 2021 20:15:44 GMT  
		Size: 35.3 MB (35311531 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76e10af105fbd4d7ed8322d6268a8e63f903e9d06ff682e3ff1ee966c9663fc0`  
		Last Modified: Mon, 01 Feb 2021 20:15:05 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8e3489a01f3df87bb94b5f1841f336b002617ecfed15c6adfa8e1661322c0c1`  
		Last Modified: Mon, 01 Feb 2021 20:15:05 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ff1204038344324e029d7469e15ec9baa18f1abbc2de83a0ae4a7e295a6eea9`  
		Last Modified: Mon, 01 Feb 2021 20:15:05 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:2.4-windowsservercore-1809`

```console
$ docker pull traefik@sha256:f8a909841f70c259ea7e5c4e4e6711fd047fafa7ca6be1114bc390e0ac69db02
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1697; amd64

### `traefik:2.4-windowsservercore-1809` - windows version 10.0.17763.1697; amd64

```console
$ docker pull traefik@sha256:6592087c3b637b852ccb83524da4e563fdbd1aa01c36c7dca55fa4154c908a9f
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2471089030 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1a4da9297c49ca2d742c3719308666352f9a5837f20529b203e86b3490850930`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 08 Jan 2021 08:50:52 GMT
RUN Install update 1809-amd64
# Wed, 13 Jan 2021 13:13:16 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Mon, 01 Feb 2021 20:14:38 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/traefik/traefik/releases/download/v2.4.1/traefik_v2.4.1_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Mon, 01 Feb 2021 20:14:39 GMT
EXPOSE 80
# Mon, 01 Feb 2021 20:14:40 GMT
ENTRYPOINT ["/traefik"]
# Mon, 01 Feb 2021 20:14:41 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.4.1 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:4dcc9a9b9e680514ef3fdfcc2ce08a3768f9e412703faa137f4a7c8297600052`  
		Size: 717.4 MB (717439216 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e00081a98bb2679c3c5f469e09d475980133a20987f9cae4cf4f7aedf59f9d8f`  
		Last Modified: Wed, 13 Jan 2021 13:17:19 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff2522d016390dfd18d8aeb8e2c6aff006cd1f9247bf87ead249db540db5125b`  
		Last Modified: Mon, 01 Feb 2021 20:15:44 GMT  
		Size: 35.3 MB (35311531 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76e10af105fbd4d7ed8322d6268a8e63f903e9d06ff682e3ff1ee966c9663fc0`  
		Last Modified: Mon, 01 Feb 2021 20:15:05 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8e3489a01f3df87bb94b5f1841f336b002617ecfed15c6adfa8e1661322c0c1`  
		Last Modified: Mon, 01 Feb 2021 20:15:05 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ff1204038344324e029d7469e15ec9baa18f1abbc2de83a0ae4a7e295a6eea9`  
		Last Modified: Mon, 01 Feb 2021 20:15:05 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:latest`

```console
$ docker pull traefik@sha256:482a48d4268f6edb38aa6934c74acf5d1f14ec2e7c5e813607ac18c958c62482
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:latest` - linux; amd64

```console
$ docker pull traefik@sha256:3d2ba657bdec47749235c4a06e0b51d89e6a2a4c72dad70c9fd5f9496c68d871
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.0 MB (29043146 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7dcdc37f2b5f338b1a51a6739a905148dd1c1b189f3d97dd205fced1797f37a0`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 17 Dec 2020 00:19:49 GMT
ADD file:8ed80010e443da19d72546bcee9a35e0a8d244c72052b1994610bf5939d479c2 in / 
# Thu, 17 Dec 2020 00:19:49 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 00:47:33 GMT
RUN apk --no-cache add ca-certificates tzdata
# Mon, 01 Feb 2021 20:36:23 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.4.1/traefik_v2.4.1_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Mon, 01 Feb 2021 20:36:23 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Mon, 01 Feb 2021 20:36:24 GMT
EXPOSE 80
# Mon, 01 Feb 2021 20:36:24 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 01 Feb 2021 20:36:24 GMT
CMD ["traefik"]
# Mon, 01 Feb 2021 20:36:24 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.4.1 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:0a6724ff3fcd51338afdfdc2b1d4ffd04569818e31efad957213d67c29b45101`  
		Last Modified: Thu, 17 Dec 2020 00:20:26 GMT  
		Size: 2.8 MB (2814864 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64d0c2f48fede0de57585b470af3e8e9aa5534db90642859512370fa53ffac21`  
		Last Modified: Thu, 17 Dec 2020 00:48:37 GMT  
		Size: 671.7 KB (671697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1516ade513da1a48f2452fb045c9f59dcb754ec8a45d295fb62c02ca3ce2fa24`  
		Last Modified: Mon, 01 Feb 2021 20:36:56 GMT  
		Size: 25.6 MB (25556218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1646cce883d51cde2f62db17c3ffca7a86fb6b363e190158baacb784df1cd067`  
		Last Modified: Mon, 01 Feb 2021 20:36:51 GMT  
		Size: 367.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:latest` - linux; arm variant v6

```console
$ docker pull traefik@sha256:a784cf52ea56aea0b24a9906cb19b4b4378a93c7d883df4315cd2274006373ec
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.1 MB (27087182 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:791475a3abf40af6d79e4c48790e71f85dac37a4ff31bfdf59b305585c037bb3`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 16 Dec 2020 23:49:53 GMT
ADD file:e3a6f7566ee3c2ba61d27d801d3522e045a4be64a42f32ee52d933b68338d06f in / 
# Wed, 16 Dec 2020 23:49:55 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 00:25:55 GMT
RUN apk --no-cache add ca-certificates tzdata
# Mon, 01 Feb 2021 20:21:51 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.4.1/traefik_v2.4.1_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Mon, 01 Feb 2021 20:21:52 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Mon, 01 Feb 2021 20:21:54 GMT
EXPOSE 80
# Mon, 01 Feb 2021 20:21:57 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 01 Feb 2021 20:21:59 GMT
CMD ["traefik"]
# Mon, 01 Feb 2021 20:22:00 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.4.1 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:56fec67ad66eea034cf5b7d0d0ffd355c0fe87611bad132ac5a952fcaa52138b`  
		Last Modified: Wed, 16 Dec 2020 23:50:34 GMT  
		Size: 2.6 MB (2620769 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab096bb24791df9de14fbfc840265a32c0d9f7be463db3a782da6095c0e6ad5b`  
		Last Modified: Thu, 17 Dec 2020 00:27:24 GMT  
		Size: 674.9 KB (674902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0eb4fee172158a2a6626c7064a033878a7a6cfc5b3fee45c74d6d44e05bc9370`  
		Last Modified: Mon, 01 Feb 2021 20:22:38 GMT  
		Size: 23.8 MB (23791143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b36a51bbc86a42ed580e716a14368625f925ffe68f228ecaa6c1ee5d7705d560`  
		Last Modified: Mon, 01 Feb 2021 20:22:29 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:latest` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:7353217d113ec6673f0215e2623b81af6251fbd4f7745078621617b498491b42
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.7 MB (26708518 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6688c1a122c4a87c308f5addeac11defec355c3db5836db65675df5c979340e2`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 16 Dec 2020 23:40:37 GMT
ADD file:47bb1b85a4eb4d0b355ae89ec5c71c09e2c2b7e21e1851a2896365eb17134f57 in / 
# Wed, 16 Dec 2020 23:40:39 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 00:27:02 GMT
RUN apk --no-cache add ca-certificates tzdata
# Mon, 01 Feb 2021 21:04:10 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.4.1/traefik_v2.4.1_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Mon, 01 Feb 2021 21:04:11 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Mon, 01 Feb 2021 21:04:11 GMT
EXPOSE 80
# Mon, 01 Feb 2021 21:04:12 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 01 Feb 2021 21:04:12 GMT
CMD ["traefik"]
# Mon, 01 Feb 2021 21:04:13 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.4.1 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:20d8a246443a66e74e17f2a0e81a51fe774876ca0c2676691c37ee1b0e4d3cd5`  
		Last Modified: Wed, 16 Dec 2020 23:41:20 GMT  
		Size: 2.7 MB (2725216 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:278abd308a18c136f69dcabbba1dc64486ebdad665d4a2f4ab14d2826ec08b06`  
		Last Modified: Thu, 17 Dec 2020 00:28:38 GMT  
		Size: 673.2 KB (673246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76f99e8acab44e0da3e7667fedfc874ddb6f2fa2bf1814aa29cbcd5f97d091c4`  
		Last Modified: Mon, 01 Feb 2021 21:04:49 GMT  
		Size: 23.3 MB (23309688 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f579f772bccf2955a27d99b4778f4f174e3fb78837376c77f98385cdcbe2bdce`  
		Last Modified: Mon, 01 Feb 2021 21:04:43 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:livarot`

```console
$ docker pull traefik@sha256:482a48d4268f6edb38aa6934c74acf5d1f14ec2e7c5e813607ac18c958c62482
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:livarot` - linux; amd64

```console
$ docker pull traefik@sha256:3d2ba657bdec47749235c4a06e0b51d89e6a2a4c72dad70c9fd5f9496c68d871
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.0 MB (29043146 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7dcdc37f2b5f338b1a51a6739a905148dd1c1b189f3d97dd205fced1797f37a0`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 17 Dec 2020 00:19:49 GMT
ADD file:8ed80010e443da19d72546bcee9a35e0a8d244c72052b1994610bf5939d479c2 in / 
# Thu, 17 Dec 2020 00:19:49 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 00:47:33 GMT
RUN apk --no-cache add ca-certificates tzdata
# Mon, 01 Feb 2021 20:36:23 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.4.1/traefik_v2.4.1_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Mon, 01 Feb 2021 20:36:23 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Mon, 01 Feb 2021 20:36:24 GMT
EXPOSE 80
# Mon, 01 Feb 2021 20:36:24 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 01 Feb 2021 20:36:24 GMT
CMD ["traefik"]
# Mon, 01 Feb 2021 20:36:24 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.4.1 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:0a6724ff3fcd51338afdfdc2b1d4ffd04569818e31efad957213d67c29b45101`  
		Last Modified: Thu, 17 Dec 2020 00:20:26 GMT  
		Size: 2.8 MB (2814864 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64d0c2f48fede0de57585b470af3e8e9aa5534db90642859512370fa53ffac21`  
		Last Modified: Thu, 17 Dec 2020 00:48:37 GMT  
		Size: 671.7 KB (671697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1516ade513da1a48f2452fb045c9f59dcb754ec8a45d295fb62c02ca3ce2fa24`  
		Last Modified: Mon, 01 Feb 2021 20:36:56 GMT  
		Size: 25.6 MB (25556218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1646cce883d51cde2f62db17c3ffca7a86fb6b363e190158baacb784df1cd067`  
		Last Modified: Mon, 01 Feb 2021 20:36:51 GMT  
		Size: 367.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:livarot` - linux; arm variant v6

```console
$ docker pull traefik@sha256:a784cf52ea56aea0b24a9906cb19b4b4378a93c7d883df4315cd2274006373ec
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.1 MB (27087182 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:791475a3abf40af6d79e4c48790e71f85dac37a4ff31bfdf59b305585c037bb3`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 16 Dec 2020 23:49:53 GMT
ADD file:e3a6f7566ee3c2ba61d27d801d3522e045a4be64a42f32ee52d933b68338d06f in / 
# Wed, 16 Dec 2020 23:49:55 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 00:25:55 GMT
RUN apk --no-cache add ca-certificates tzdata
# Mon, 01 Feb 2021 20:21:51 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.4.1/traefik_v2.4.1_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Mon, 01 Feb 2021 20:21:52 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Mon, 01 Feb 2021 20:21:54 GMT
EXPOSE 80
# Mon, 01 Feb 2021 20:21:57 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 01 Feb 2021 20:21:59 GMT
CMD ["traefik"]
# Mon, 01 Feb 2021 20:22:00 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.4.1 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:56fec67ad66eea034cf5b7d0d0ffd355c0fe87611bad132ac5a952fcaa52138b`  
		Last Modified: Wed, 16 Dec 2020 23:50:34 GMT  
		Size: 2.6 MB (2620769 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab096bb24791df9de14fbfc840265a32c0d9f7be463db3a782da6095c0e6ad5b`  
		Last Modified: Thu, 17 Dec 2020 00:27:24 GMT  
		Size: 674.9 KB (674902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0eb4fee172158a2a6626c7064a033878a7a6cfc5b3fee45c74d6d44e05bc9370`  
		Last Modified: Mon, 01 Feb 2021 20:22:38 GMT  
		Size: 23.8 MB (23791143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b36a51bbc86a42ed580e716a14368625f925ffe68f228ecaa6c1ee5d7705d560`  
		Last Modified: Mon, 01 Feb 2021 20:22:29 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:livarot` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:7353217d113ec6673f0215e2623b81af6251fbd4f7745078621617b498491b42
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.7 MB (26708518 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6688c1a122c4a87c308f5addeac11defec355c3db5836db65675df5c979340e2`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 16 Dec 2020 23:40:37 GMT
ADD file:47bb1b85a4eb4d0b355ae89ec5c71c09e2c2b7e21e1851a2896365eb17134f57 in / 
# Wed, 16 Dec 2020 23:40:39 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 00:27:02 GMT
RUN apk --no-cache add ca-certificates tzdata
# Mon, 01 Feb 2021 21:04:10 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.4.1/traefik_v2.4.1_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Mon, 01 Feb 2021 21:04:11 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Mon, 01 Feb 2021 21:04:11 GMT
EXPOSE 80
# Mon, 01 Feb 2021 21:04:12 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 01 Feb 2021 21:04:12 GMT
CMD ["traefik"]
# Mon, 01 Feb 2021 21:04:13 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.4.1 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:20d8a246443a66e74e17f2a0e81a51fe774876ca0c2676691c37ee1b0e4d3cd5`  
		Last Modified: Wed, 16 Dec 2020 23:41:20 GMT  
		Size: 2.7 MB (2725216 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:278abd308a18c136f69dcabbba1dc64486ebdad665d4a2f4ab14d2826ec08b06`  
		Last Modified: Thu, 17 Dec 2020 00:28:38 GMT  
		Size: 673.2 KB (673246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76f99e8acab44e0da3e7667fedfc874ddb6f2fa2bf1814aa29cbcd5f97d091c4`  
		Last Modified: Mon, 01 Feb 2021 21:04:49 GMT  
		Size: 23.3 MB (23309688 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f579f772bccf2955a27d99b4778f4f174e3fb78837376c77f98385cdcbe2bdce`  
		Last Modified: Mon, 01 Feb 2021 21:04:43 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:livarot-windowsservercore-1809`

```console
$ docker pull traefik@sha256:f8a909841f70c259ea7e5c4e4e6711fd047fafa7ca6be1114bc390e0ac69db02
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1697; amd64

### `traefik:livarot-windowsservercore-1809` - windows version 10.0.17763.1697; amd64

```console
$ docker pull traefik@sha256:6592087c3b637b852ccb83524da4e563fdbd1aa01c36c7dca55fa4154c908a9f
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2471089030 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1a4da9297c49ca2d742c3719308666352f9a5837f20529b203e86b3490850930`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 08 Jan 2021 08:50:52 GMT
RUN Install update 1809-amd64
# Wed, 13 Jan 2021 13:13:16 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Mon, 01 Feb 2021 20:14:38 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/traefik/traefik/releases/download/v2.4.1/traefik_v2.4.1_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Mon, 01 Feb 2021 20:14:39 GMT
EXPOSE 80
# Mon, 01 Feb 2021 20:14:40 GMT
ENTRYPOINT ["/traefik"]
# Mon, 01 Feb 2021 20:14:41 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.4.1 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:4dcc9a9b9e680514ef3fdfcc2ce08a3768f9e412703faa137f4a7c8297600052`  
		Size: 717.4 MB (717439216 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e00081a98bb2679c3c5f469e09d475980133a20987f9cae4cf4f7aedf59f9d8f`  
		Last Modified: Wed, 13 Jan 2021 13:17:19 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff2522d016390dfd18d8aeb8e2c6aff006cd1f9247bf87ead249db540db5125b`  
		Last Modified: Mon, 01 Feb 2021 20:15:44 GMT  
		Size: 35.3 MB (35311531 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76e10af105fbd4d7ed8322d6268a8e63f903e9d06ff682e3ff1ee966c9663fc0`  
		Last Modified: Mon, 01 Feb 2021 20:15:05 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8e3489a01f3df87bb94b5f1841f336b002617ecfed15c6adfa8e1661322c0c1`  
		Last Modified: Mon, 01 Feb 2021 20:15:05 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ff1204038344324e029d7469e15ec9baa18f1abbc2de83a0ae4a7e295a6eea9`  
		Last Modified: Mon, 01 Feb 2021 20:15:05 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:maroilles`

```console
$ docker pull traefik@sha256:998fc0cce3df0fe066005d6e94a7fa8b20749155fb54b4ebd1603e039b842feb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:maroilles` - linux; amd64

```console
$ docker pull traefik@sha256:154e065982592220c9355925d9e60348eec6850418754ee76840f83501341b00
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **21.6 MB (21553283 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d2d67ddf1c8b647742ebb1ea0d3edb163dff028640b772832fa325b6b7df830f`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Thu, 17 Dec 2020 00:48:11 GMT
COPY file:cd6264d9a7514a8fbc3eb7b400566d36178794d2b757959812cc3abc6f13a97b in /etc/ssl/certs/ 
# Thu, 17 Dec 2020 00:48:11 GMT
COPY dir:83da415af0ff24b3b9d10f857aa8c724a3bc93523f3e047b827e7554fe1f9e08 in /usr/share/ 
# Wed, 13 Jan 2021 22:29:46 GMT
COPY file:94b9997cc55c7732c9fc173c119f980e4a38eba20b96a90170a3d7fade75f0eb in / 
# Wed, 13 Jan 2021 22:29:47 GMT
EXPOSE 80
# Wed, 13 Jan 2021 22:29:47 GMT
VOLUME [/tmp]
# Wed, 13 Jan 2021 22:29:47 GMT
ENTRYPOINT ["/traefik"]
# Wed, 13 Jan 2021 22:29:47 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.28 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:79de75e85675fa9abbac17b57205d3e0dfcf2bd2fc4cbc194f2aaf917435425e`  
		Last Modified: Thu, 17 Dec 2020 00:49:17 GMT  
		Size: 130.9 KB (130872 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f0e925284bb6370a549da51637ed98a8e574317473e082cc4be745d87327c7f`  
		Last Modified: Thu, 17 Dec 2020 00:49:18 GMT  
		Size: 306.4 KB (306411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81848bd29c493bb51f93a0bf98cf3958436af2128b6890d7a28a35b7dfc352c0`  
		Last Modified: Wed, 13 Jan 2021 22:30:48 GMT  
		Size: 21.1 MB (21116000 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:maroilles` - linux; arm variant v6

```console
$ docker pull traefik@sha256:2f69dff9f3e67a011f08fc6a59fc3f72aa26533b5b9c8cd127e1f90948cbaf09
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **20.2 MB (20205544 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:da195dbaa64e13483787db1f21a4e602751bd363ac5c6e594e5e17c1f2420aec`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Thu, 17 Dec 2020 00:26:47 GMT
COPY file:cd6264d9a7514a8fbc3eb7b400566d36178794d2b757959812cc3abc6f13a97b in /etc/ssl/certs/ 
# Thu, 17 Dec 2020 00:26:48 GMT
COPY dir:83da415af0ff24b3b9d10f857aa8c724a3bc93523f3e047b827e7554fe1f9e08 in /usr/share/ 
# Wed, 13 Jan 2021 21:57:06 GMT
COPY file:3d9c1552db5b4c73ac7fe21268eeb20506f000d2e59d7be76697f45a50d32c64 in / 
# Wed, 13 Jan 2021 21:57:07 GMT
EXPOSE 80
# Wed, 13 Jan 2021 21:57:08 GMT
VOLUME [/tmp]
# Wed, 13 Jan 2021 21:57:09 GMT
ENTRYPOINT ["/traefik"]
# Wed, 13 Jan 2021 21:57:09 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.28 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:26c529e82b09c489524aa4f787754320793a95eb7aa7eaf306c517b76818ec25`  
		Last Modified: Thu, 17 Dec 2020 00:28:41 GMT  
		Size: 130.9 KB (130873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4adc6fb65827756c9d95005162623d443b2bd3e445269bcb1a7006e080726d3c`  
		Last Modified: Thu, 17 Dec 2020 00:28:41 GMT  
		Size: 306.5 KB (306458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0280c8ba5c59856146b5130ce0c0eb8b83b9dcc2dea1d69991723680815054f`  
		Last Modified: Wed, 13 Jan 2021 21:58:11 GMT  
		Size: 19.8 MB (19768213 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:maroilles` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:468570d210f86c4366e666dac62c34b3054c230ee0b4d61c36e37ed276550b39
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **19.9 MB (19923388 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:13fff7cc610524cb77e4767eb66f534053cc0f45853e096fb250937594f9913d`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Thu, 17 Dec 2020 00:27:56 GMT
COPY file:cd6264d9a7514a8fbc3eb7b400566d36178794d2b757959812cc3abc6f13a97b in /etc/ssl/certs/ 
# Thu, 17 Dec 2020 00:27:58 GMT
COPY dir:83da415af0ff24b3b9d10f857aa8c724a3bc93523f3e047b827e7554fe1f9e08 in /usr/share/ 
# Wed, 13 Jan 2021 21:46:55 GMT
COPY file:6bab4a8fc3d272fc29bc5ff42634cb12785fea9e23b0cf50f077702217bb6c03 in / 
# Wed, 13 Jan 2021 21:46:56 GMT
EXPOSE 80
# Wed, 13 Jan 2021 21:46:56 GMT
VOLUME [/tmp]
# Wed, 13 Jan 2021 21:46:57 GMT
ENTRYPOINT ["/traefik"]
# Wed, 13 Jan 2021 21:46:58 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.28 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:7dccf22d113d483cac839141f2028cbf6ac2e0c6aa4a1716c5e7b575b162028c`  
		Last Modified: Thu, 17 Dec 2020 00:29:55 GMT  
		Size: 130.9 KB (130873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c32c03119dbb32c844511340cb40a21ba5a56b90862cf603dec2e49cf5ab20d`  
		Last Modified: Thu, 17 Dec 2020 00:29:57 GMT  
		Size: 306.5 KB (306466 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41f7f3a967c907bfe4aeb896ba6da80cfaf9bce19fcb39b51a6378b00596760d`  
		Last Modified: Wed, 13 Jan 2021 21:47:50 GMT  
		Size: 19.5 MB (19486049 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:maroilles-alpine`

```console
$ docker pull traefik@sha256:d232a757f6c487484b3640973fbb0287e747e6b357bc1dc75faa07b26da14a5f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:maroilles-alpine` - linux; amd64

```console
$ docker pull traefik@sha256:cb19d2e6f6575fb121eb2181cbd50f783c1995bf515cba8c7bbab7d9b6859949
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **24.6 MB (24603200 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d9ecef4edf395a65a22e7b3c46ec4b16c869c1a5386a1ea0305132dc68266f04`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 17 Dec 2020 00:19:49 GMT
ADD file:8ed80010e443da19d72546bcee9a35e0a8d244c72052b1994610bf5939d479c2 in / 
# Thu, 17 Dec 2020 00:19:49 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 00:47:33 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 13 Jan 2021 22:29:27 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/traefik/traefik/releases/download/v1.7.28/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Wed, 13 Jan 2021 22:29:27 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 13 Jan 2021 22:29:27 GMT
EXPOSE 80
# Wed, 13 Jan 2021 22:29:27 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 13 Jan 2021 22:29:28 GMT
CMD ["traefik"]
# Wed, 13 Jan 2021 22:29:28 GMT
LABEL org.opencontainers.image.vendor=traefik org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.28 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:0a6724ff3fcd51338afdfdc2b1d4ffd04569818e31efad957213d67c29b45101`  
		Last Modified: Thu, 17 Dec 2020 00:20:26 GMT  
		Size: 2.8 MB (2814864 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64d0c2f48fede0de57585b470af3e8e9aa5534db90642859512370fa53ffac21`  
		Last Modified: Thu, 17 Dec 2020 00:48:37 GMT  
		Size: 671.7 KB (671697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce8923725f26216ece246718b634aabb038e3ba78292d388ebb7350cc0d89ba1`  
		Last Modified: Wed, 13 Jan 2021 22:30:25 GMT  
		Size: 21.1 MB (21116271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f8abe3b22d27fbf46de589e10d21107bd248a725e59317b3fc6a78a83e9c940`  
		Last Modified: Wed, 13 Jan 2021 22:30:19 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:maroilles-alpine` - linux; arm variant v6

```console
$ docker pull traefik@sha256:198e33555ab98a4ea7b448b1f818b9663ab2f8fe98f0966543390a711e55692d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.1 MB (23064299 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:92898625b48315d465f9a4d3ad8e32c8b224bb4617bff335d0840bbd9ce1aced`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 16 Dec 2020 23:49:53 GMT
ADD file:e3a6f7566ee3c2ba61d27d801d3522e045a4be64a42f32ee52d933b68338d06f in / 
# Wed, 16 Dec 2020 23:49:55 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 00:25:55 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 13 Jan 2021 21:56:46 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/traefik/traefik/releases/download/v1.7.28/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Wed, 13 Jan 2021 21:56:47 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 13 Jan 2021 21:56:48 GMT
EXPOSE 80
# Wed, 13 Jan 2021 21:56:48 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 13 Jan 2021 21:56:49 GMT
CMD ["traefik"]
# Wed, 13 Jan 2021 21:56:49 GMT
LABEL org.opencontainers.image.vendor=traefik org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.28 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:56fec67ad66eea034cf5b7d0d0ffd355c0fe87611bad132ac5a952fcaa52138b`  
		Last Modified: Wed, 16 Dec 2020 23:50:34 GMT  
		Size: 2.6 MB (2620769 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab096bb24791df9de14fbfc840265a32c0d9f7be463db3a782da6095c0e6ad5b`  
		Last Modified: Thu, 17 Dec 2020 00:27:24 GMT  
		Size: 674.9 KB (674902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:102471939d830c2c1e2668e0dd48049fc6ce2f332ead14922e8a55086f8816ef`  
		Last Modified: Wed, 13 Jan 2021 21:57:48 GMT  
		Size: 19.8 MB (19768260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29a399e8ce2234a61da5e35bf382eefe32e24435b8c5805b773299d16a01b022`  
		Last Modified: Wed, 13 Jan 2021 21:57:42 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:maroilles-alpine` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:a144e4ba9554f68e6903986ca95090991e87d3c7a3e45809bfd602a5bda85a3c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **22.9 MB (22884874 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:24c65bf1525b68d03c1cc5d512338cf2608b5742b1e06e6ea57c492e61afee7a`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 16 Dec 2020 23:40:37 GMT
ADD file:47bb1b85a4eb4d0b355ae89ec5c71c09e2c2b7e21e1851a2896365eb17134f57 in / 
# Wed, 16 Dec 2020 23:40:39 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 00:27:02 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 13 Jan 2021 21:46:38 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/traefik/traefik/releases/download/v1.7.28/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Wed, 13 Jan 2021 21:46:39 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 13 Jan 2021 21:46:39 GMT
EXPOSE 80
# Wed, 13 Jan 2021 21:46:40 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 13 Jan 2021 21:46:41 GMT
CMD ["traefik"]
# Wed, 13 Jan 2021 21:46:41 GMT
LABEL org.opencontainers.image.vendor=traefik org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.28 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:20d8a246443a66e74e17f2a0e81a51fe774876ca0c2676691c37ee1b0e4d3cd5`  
		Last Modified: Wed, 16 Dec 2020 23:41:20 GMT  
		Size: 2.7 MB (2725216 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:278abd308a18c136f69dcabbba1dc64486ebdad665d4a2f4ab14d2826ec08b06`  
		Last Modified: Thu, 17 Dec 2020 00:28:38 GMT  
		Size: 673.2 KB (673246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e50dc3ca8b514cac3bfbf2a6303d6be654d1a94f584f6f24d4e62522b80bd36b`  
		Last Modified: Wed, 13 Jan 2021 21:47:33 GMT  
		Size: 19.5 MB (19486044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d4205a3b9bbaa8f65f3bd5780aeb6e4cc761d5f7d6de7cb70588b41ed018c72`  
		Last Modified: Wed, 13 Jan 2021 21:47:27 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:maroilles-windowsservercore-1809`

```console
$ docker pull traefik@sha256:8f2b9d477c5d31806d427f5dad762d9f448c131bb284641f3977b914e655afd7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1697; amd64

### `traefik:maroilles-windowsservercore-1809` - windows version 10.0.17763.1697; amd64

```console
$ docker pull traefik@sha256:91b9a8ca83df9afc2b41003518d4b4f9d8e8a21f77880fd74d543670c7ab4da9
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2466262882 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6962de1a7e3fc419a74eb2ea94e4c40359d9f53a93caec6bd1e61f1944ccf282`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 08 Jan 2021 08:50:52 GMT
RUN Install update 1809-amd64
# Wed, 13 Jan 2021 13:13:16 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 14 Jan 2021 01:16:20 GMT
RUN Invoke-WebRequest     -Uri "https://github.com/traefik/traefik/releases/download/v1.7.28/traefik_windows-amd64.exe"     -OutFile "/traefik.exe"
# Thu, 14 Jan 2021 01:16:24 GMT
EXPOSE 80
# Thu, 14 Jan 2021 01:16:25 GMT
ENTRYPOINT ["/traefik"]
# Thu, 14 Jan 2021 01:16:26 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.28 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:4dcc9a9b9e680514ef3fdfcc2ce08a3768f9e412703faa137f4a7c8297600052`  
		Size: 717.4 MB (717439216 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e00081a98bb2679c3c5f469e09d475980133a20987f9cae4cf4f7aedf59f9d8f`  
		Last Modified: Wed, 13 Jan 2021 13:17:19 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84697de3c7d0310176f36e2fe57e5688d23e486eb5b5febf6dbf860e763d1750`  
		Last Modified: Thu, 14 Jan 2021 01:17:09 GMT  
		Size: 30.5 MB (30486249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:069ca4204690196a12b1d26a1b7d9b54c2d8fc7db082a3a4a9e21bfdf55d63d1`  
		Last Modified: Thu, 14 Jan 2021 01:17:02 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adaebdd4a9fa6db73d7167e0d944af020e0ddfe54da3ed92807a14054a53d669`  
		Last Modified: Thu, 14 Jan 2021 01:17:01 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:454fe39b046d9fedbd9e0b3f698556592463406933b790b272dd909d5bd90d53`  
		Last Modified: Thu, 14 Jan 2021 01:17:02 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v1.7`

```console
$ docker pull traefik@sha256:998fc0cce3df0fe066005d6e94a7fa8b20749155fb54b4ebd1603e039b842feb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:v1.7` - linux; amd64

```console
$ docker pull traefik@sha256:154e065982592220c9355925d9e60348eec6850418754ee76840f83501341b00
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **21.6 MB (21553283 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d2d67ddf1c8b647742ebb1ea0d3edb163dff028640b772832fa325b6b7df830f`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Thu, 17 Dec 2020 00:48:11 GMT
COPY file:cd6264d9a7514a8fbc3eb7b400566d36178794d2b757959812cc3abc6f13a97b in /etc/ssl/certs/ 
# Thu, 17 Dec 2020 00:48:11 GMT
COPY dir:83da415af0ff24b3b9d10f857aa8c724a3bc93523f3e047b827e7554fe1f9e08 in /usr/share/ 
# Wed, 13 Jan 2021 22:29:46 GMT
COPY file:94b9997cc55c7732c9fc173c119f980e4a38eba20b96a90170a3d7fade75f0eb in / 
# Wed, 13 Jan 2021 22:29:47 GMT
EXPOSE 80
# Wed, 13 Jan 2021 22:29:47 GMT
VOLUME [/tmp]
# Wed, 13 Jan 2021 22:29:47 GMT
ENTRYPOINT ["/traefik"]
# Wed, 13 Jan 2021 22:29:47 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.28 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:79de75e85675fa9abbac17b57205d3e0dfcf2bd2fc4cbc194f2aaf917435425e`  
		Last Modified: Thu, 17 Dec 2020 00:49:17 GMT  
		Size: 130.9 KB (130872 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f0e925284bb6370a549da51637ed98a8e574317473e082cc4be745d87327c7f`  
		Last Modified: Thu, 17 Dec 2020 00:49:18 GMT  
		Size: 306.4 KB (306411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81848bd29c493bb51f93a0bf98cf3958436af2128b6890d7a28a35b7dfc352c0`  
		Last Modified: Wed, 13 Jan 2021 22:30:48 GMT  
		Size: 21.1 MB (21116000 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v1.7` - linux; arm variant v6

```console
$ docker pull traefik@sha256:2f69dff9f3e67a011f08fc6a59fc3f72aa26533b5b9c8cd127e1f90948cbaf09
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **20.2 MB (20205544 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:da195dbaa64e13483787db1f21a4e602751bd363ac5c6e594e5e17c1f2420aec`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Thu, 17 Dec 2020 00:26:47 GMT
COPY file:cd6264d9a7514a8fbc3eb7b400566d36178794d2b757959812cc3abc6f13a97b in /etc/ssl/certs/ 
# Thu, 17 Dec 2020 00:26:48 GMT
COPY dir:83da415af0ff24b3b9d10f857aa8c724a3bc93523f3e047b827e7554fe1f9e08 in /usr/share/ 
# Wed, 13 Jan 2021 21:57:06 GMT
COPY file:3d9c1552db5b4c73ac7fe21268eeb20506f000d2e59d7be76697f45a50d32c64 in / 
# Wed, 13 Jan 2021 21:57:07 GMT
EXPOSE 80
# Wed, 13 Jan 2021 21:57:08 GMT
VOLUME [/tmp]
# Wed, 13 Jan 2021 21:57:09 GMT
ENTRYPOINT ["/traefik"]
# Wed, 13 Jan 2021 21:57:09 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.28 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:26c529e82b09c489524aa4f787754320793a95eb7aa7eaf306c517b76818ec25`  
		Last Modified: Thu, 17 Dec 2020 00:28:41 GMT  
		Size: 130.9 KB (130873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4adc6fb65827756c9d95005162623d443b2bd3e445269bcb1a7006e080726d3c`  
		Last Modified: Thu, 17 Dec 2020 00:28:41 GMT  
		Size: 306.5 KB (306458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0280c8ba5c59856146b5130ce0c0eb8b83b9dcc2dea1d69991723680815054f`  
		Last Modified: Wed, 13 Jan 2021 21:58:11 GMT  
		Size: 19.8 MB (19768213 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v1.7` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:468570d210f86c4366e666dac62c34b3054c230ee0b4d61c36e37ed276550b39
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **19.9 MB (19923388 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:13fff7cc610524cb77e4767eb66f534053cc0f45853e096fb250937594f9913d`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Thu, 17 Dec 2020 00:27:56 GMT
COPY file:cd6264d9a7514a8fbc3eb7b400566d36178794d2b757959812cc3abc6f13a97b in /etc/ssl/certs/ 
# Thu, 17 Dec 2020 00:27:58 GMT
COPY dir:83da415af0ff24b3b9d10f857aa8c724a3bc93523f3e047b827e7554fe1f9e08 in /usr/share/ 
# Wed, 13 Jan 2021 21:46:55 GMT
COPY file:6bab4a8fc3d272fc29bc5ff42634cb12785fea9e23b0cf50f077702217bb6c03 in / 
# Wed, 13 Jan 2021 21:46:56 GMT
EXPOSE 80
# Wed, 13 Jan 2021 21:46:56 GMT
VOLUME [/tmp]
# Wed, 13 Jan 2021 21:46:57 GMT
ENTRYPOINT ["/traefik"]
# Wed, 13 Jan 2021 21:46:58 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.28 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:7dccf22d113d483cac839141f2028cbf6ac2e0c6aa4a1716c5e7b575b162028c`  
		Last Modified: Thu, 17 Dec 2020 00:29:55 GMT  
		Size: 130.9 KB (130873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c32c03119dbb32c844511340cb40a21ba5a56b90862cf603dec2e49cf5ab20d`  
		Last Modified: Thu, 17 Dec 2020 00:29:57 GMT  
		Size: 306.5 KB (306466 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41f7f3a967c907bfe4aeb896ba6da80cfaf9bce19fcb39b51a6378b00596760d`  
		Last Modified: Wed, 13 Jan 2021 21:47:50 GMT  
		Size: 19.5 MB (19486049 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v1.7.28`

```console
$ docker pull traefik@sha256:998fc0cce3df0fe066005d6e94a7fa8b20749155fb54b4ebd1603e039b842feb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:v1.7.28` - linux; amd64

```console
$ docker pull traefik@sha256:154e065982592220c9355925d9e60348eec6850418754ee76840f83501341b00
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **21.6 MB (21553283 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d2d67ddf1c8b647742ebb1ea0d3edb163dff028640b772832fa325b6b7df830f`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Thu, 17 Dec 2020 00:48:11 GMT
COPY file:cd6264d9a7514a8fbc3eb7b400566d36178794d2b757959812cc3abc6f13a97b in /etc/ssl/certs/ 
# Thu, 17 Dec 2020 00:48:11 GMT
COPY dir:83da415af0ff24b3b9d10f857aa8c724a3bc93523f3e047b827e7554fe1f9e08 in /usr/share/ 
# Wed, 13 Jan 2021 22:29:46 GMT
COPY file:94b9997cc55c7732c9fc173c119f980e4a38eba20b96a90170a3d7fade75f0eb in / 
# Wed, 13 Jan 2021 22:29:47 GMT
EXPOSE 80
# Wed, 13 Jan 2021 22:29:47 GMT
VOLUME [/tmp]
# Wed, 13 Jan 2021 22:29:47 GMT
ENTRYPOINT ["/traefik"]
# Wed, 13 Jan 2021 22:29:47 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.28 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:79de75e85675fa9abbac17b57205d3e0dfcf2bd2fc4cbc194f2aaf917435425e`  
		Last Modified: Thu, 17 Dec 2020 00:49:17 GMT  
		Size: 130.9 KB (130872 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f0e925284bb6370a549da51637ed98a8e574317473e082cc4be745d87327c7f`  
		Last Modified: Thu, 17 Dec 2020 00:49:18 GMT  
		Size: 306.4 KB (306411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81848bd29c493bb51f93a0bf98cf3958436af2128b6890d7a28a35b7dfc352c0`  
		Last Modified: Wed, 13 Jan 2021 22:30:48 GMT  
		Size: 21.1 MB (21116000 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v1.7.28` - linux; arm variant v6

```console
$ docker pull traefik@sha256:2f69dff9f3e67a011f08fc6a59fc3f72aa26533b5b9c8cd127e1f90948cbaf09
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **20.2 MB (20205544 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:da195dbaa64e13483787db1f21a4e602751bd363ac5c6e594e5e17c1f2420aec`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Thu, 17 Dec 2020 00:26:47 GMT
COPY file:cd6264d9a7514a8fbc3eb7b400566d36178794d2b757959812cc3abc6f13a97b in /etc/ssl/certs/ 
# Thu, 17 Dec 2020 00:26:48 GMT
COPY dir:83da415af0ff24b3b9d10f857aa8c724a3bc93523f3e047b827e7554fe1f9e08 in /usr/share/ 
# Wed, 13 Jan 2021 21:57:06 GMT
COPY file:3d9c1552db5b4c73ac7fe21268eeb20506f000d2e59d7be76697f45a50d32c64 in / 
# Wed, 13 Jan 2021 21:57:07 GMT
EXPOSE 80
# Wed, 13 Jan 2021 21:57:08 GMT
VOLUME [/tmp]
# Wed, 13 Jan 2021 21:57:09 GMT
ENTRYPOINT ["/traefik"]
# Wed, 13 Jan 2021 21:57:09 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.28 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:26c529e82b09c489524aa4f787754320793a95eb7aa7eaf306c517b76818ec25`  
		Last Modified: Thu, 17 Dec 2020 00:28:41 GMT  
		Size: 130.9 KB (130873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4adc6fb65827756c9d95005162623d443b2bd3e445269bcb1a7006e080726d3c`  
		Last Modified: Thu, 17 Dec 2020 00:28:41 GMT  
		Size: 306.5 KB (306458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0280c8ba5c59856146b5130ce0c0eb8b83b9dcc2dea1d69991723680815054f`  
		Last Modified: Wed, 13 Jan 2021 21:58:11 GMT  
		Size: 19.8 MB (19768213 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v1.7.28` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:468570d210f86c4366e666dac62c34b3054c230ee0b4d61c36e37ed276550b39
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **19.9 MB (19923388 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:13fff7cc610524cb77e4767eb66f534053cc0f45853e096fb250937594f9913d`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Thu, 17 Dec 2020 00:27:56 GMT
COPY file:cd6264d9a7514a8fbc3eb7b400566d36178794d2b757959812cc3abc6f13a97b in /etc/ssl/certs/ 
# Thu, 17 Dec 2020 00:27:58 GMT
COPY dir:83da415af0ff24b3b9d10f857aa8c724a3bc93523f3e047b827e7554fe1f9e08 in /usr/share/ 
# Wed, 13 Jan 2021 21:46:55 GMT
COPY file:6bab4a8fc3d272fc29bc5ff42634cb12785fea9e23b0cf50f077702217bb6c03 in / 
# Wed, 13 Jan 2021 21:46:56 GMT
EXPOSE 80
# Wed, 13 Jan 2021 21:46:56 GMT
VOLUME [/tmp]
# Wed, 13 Jan 2021 21:46:57 GMT
ENTRYPOINT ["/traefik"]
# Wed, 13 Jan 2021 21:46:58 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.28 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:7dccf22d113d483cac839141f2028cbf6ac2e0c6aa4a1716c5e7b575b162028c`  
		Last Modified: Thu, 17 Dec 2020 00:29:55 GMT  
		Size: 130.9 KB (130873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c32c03119dbb32c844511340cb40a21ba5a56b90862cf603dec2e49cf5ab20d`  
		Last Modified: Thu, 17 Dec 2020 00:29:57 GMT  
		Size: 306.5 KB (306466 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41f7f3a967c907bfe4aeb896ba6da80cfaf9bce19fcb39b51a6378b00596760d`  
		Last Modified: Wed, 13 Jan 2021 21:47:50 GMT  
		Size: 19.5 MB (19486049 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v1.7.28-alpine`

```console
$ docker pull traefik@sha256:d232a757f6c487484b3640973fbb0287e747e6b357bc1dc75faa07b26da14a5f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:v1.7.28-alpine` - linux; amd64

```console
$ docker pull traefik@sha256:cb19d2e6f6575fb121eb2181cbd50f783c1995bf515cba8c7bbab7d9b6859949
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **24.6 MB (24603200 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d9ecef4edf395a65a22e7b3c46ec4b16c869c1a5386a1ea0305132dc68266f04`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 17 Dec 2020 00:19:49 GMT
ADD file:8ed80010e443da19d72546bcee9a35e0a8d244c72052b1994610bf5939d479c2 in / 
# Thu, 17 Dec 2020 00:19:49 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 00:47:33 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 13 Jan 2021 22:29:27 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/traefik/traefik/releases/download/v1.7.28/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Wed, 13 Jan 2021 22:29:27 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 13 Jan 2021 22:29:27 GMT
EXPOSE 80
# Wed, 13 Jan 2021 22:29:27 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 13 Jan 2021 22:29:28 GMT
CMD ["traefik"]
# Wed, 13 Jan 2021 22:29:28 GMT
LABEL org.opencontainers.image.vendor=traefik org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.28 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:0a6724ff3fcd51338afdfdc2b1d4ffd04569818e31efad957213d67c29b45101`  
		Last Modified: Thu, 17 Dec 2020 00:20:26 GMT  
		Size: 2.8 MB (2814864 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64d0c2f48fede0de57585b470af3e8e9aa5534db90642859512370fa53ffac21`  
		Last Modified: Thu, 17 Dec 2020 00:48:37 GMT  
		Size: 671.7 KB (671697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce8923725f26216ece246718b634aabb038e3ba78292d388ebb7350cc0d89ba1`  
		Last Modified: Wed, 13 Jan 2021 22:30:25 GMT  
		Size: 21.1 MB (21116271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f8abe3b22d27fbf46de589e10d21107bd248a725e59317b3fc6a78a83e9c940`  
		Last Modified: Wed, 13 Jan 2021 22:30:19 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v1.7.28-alpine` - linux; arm variant v6

```console
$ docker pull traefik@sha256:198e33555ab98a4ea7b448b1f818b9663ab2f8fe98f0966543390a711e55692d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.1 MB (23064299 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:92898625b48315d465f9a4d3ad8e32c8b224bb4617bff335d0840bbd9ce1aced`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 16 Dec 2020 23:49:53 GMT
ADD file:e3a6f7566ee3c2ba61d27d801d3522e045a4be64a42f32ee52d933b68338d06f in / 
# Wed, 16 Dec 2020 23:49:55 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 00:25:55 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 13 Jan 2021 21:56:46 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/traefik/traefik/releases/download/v1.7.28/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Wed, 13 Jan 2021 21:56:47 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 13 Jan 2021 21:56:48 GMT
EXPOSE 80
# Wed, 13 Jan 2021 21:56:48 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 13 Jan 2021 21:56:49 GMT
CMD ["traefik"]
# Wed, 13 Jan 2021 21:56:49 GMT
LABEL org.opencontainers.image.vendor=traefik org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.28 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:56fec67ad66eea034cf5b7d0d0ffd355c0fe87611bad132ac5a952fcaa52138b`  
		Last Modified: Wed, 16 Dec 2020 23:50:34 GMT  
		Size: 2.6 MB (2620769 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab096bb24791df9de14fbfc840265a32c0d9f7be463db3a782da6095c0e6ad5b`  
		Last Modified: Thu, 17 Dec 2020 00:27:24 GMT  
		Size: 674.9 KB (674902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:102471939d830c2c1e2668e0dd48049fc6ce2f332ead14922e8a55086f8816ef`  
		Last Modified: Wed, 13 Jan 2021 21:57:48 GMT  
		Size: 19.8 MB (19768260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29a399e8ce2234a61da5e35bf382eefe32e24435b8c5805b773299d16a01b022`  
		Last Modified: Wed, 13 Jan 2021 21:57:42 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v1.7.28-alpine` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:a144e4ba9554f68e6903986ca95090991e87d3c7a3e45809bfd602a5bda85a3c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **22.9 MB (22884874 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:24c65bf1525b68d03c1cc5d512338cf2608b5742b1e06e6ea57c492e61afee7a`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 16 Dec 2020 23:40:37 GMT
ADD file:47bb1b85a4eb4d0b355ae89ec5c71c09e2c2b7e21e1851a2896365eb17134f57 in / 
# Wed, 16 Dec 2020 23:40:39 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 00:27:02 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 13 Jan 2021 21:46:38 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/traefik/traefik/releases/download/v1.7.28/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Wed, 13 Jan 2021 21:46:39 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 13 Jan 2021 21:46:39 GMT
EXPOSE 80
# Wed, 13 Jan 2021 21:46:40 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 13 Jan 2021 21:46:41 GMT
CMD ["traefik"]
# Wed, 13 Jan 2021 21:46:41 GMT
LABEL org.opencontainers.image.vendor=traefik org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.28 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:20d8a246443a66e74e17f2a0e81a51fe774876ca0c2676691c37ee1b0e4d3cd5`  
		Last Modified: Wed, 16 Dec 2020 23:41:20 GMT  
		Size: 2.7 MB (2725216 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:278abd308a18c136f69dcabbba1dc64486ebdad665d4a2f4ab14d2826ec08b06`  
		Last Modified: Thu, 17 Dec 2020 00:28:38 GMT  
		Size: 673.2 KB (673246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e50dc3ca8b514cac3bfbf2a6303d6be654d1a94f584f6f24d4e62522b80bd36b`  
		Last Modified: Wed, 13 Jan 2021 21:47:33 GMT  
		Size: 19.5 MB (19486044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d4205a3b9bbaa8f65f3bd5780aeb6e4cc761d5f7d6de7cb70588b41ed018c72`  
		Last Modified: Wed, 13 Jan 2021 21:47:27 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v1.7.28-windowsservercore-1809`

```console
$ docker pull traefik@sha256:8f2b9d477c5d31806d427f5dad762d9f448c131bb284641f3977b914e655afd7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1697; amd64

### `traefik:v1.7.28-windowsservercore-1809` - windows version 10.0.17763.1697; amd64

```console
$ docker pull traefik@sha256:91b9a8ca83df9afc2b41003518d4b4f9d8e8a21f77880fd74d543670c7ab4da9
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2466262882 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6962de1a7e3fc419a74eb2ea94e4c40359d9f53a93caec6bd1e61f1944ccf282`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 08 Jan 2021 08:50:52 GMT
RUN Install update 1809-amd64
# Wed, 13 Jan 2021 13:13:16 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 14 Jan 2021 01:16:20 GMT
RUN Invoke-WebRequest     -Uri "https://github.com/traefik/traefik/releases/download/v1.7.28/traefik_windows-amd64.exe"     -OutFile "/traefik.exe"
# Thu, 14 Jan 2021 01:16:24 GMT
EXPOSE 80
# Thu, 14 Jan 2021 01:16:25 GMT
ENTRYPOINT ["/traefik"]
# Thu, 14 Jan 2021 01:16:26 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.28 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:4dcc9a9b9e680514ef3fdfcc2ce08a3768f9e412703faa137f4a7c8297600052`  
		Size: 717.4 MB (717439216 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e00081a98bb2679c3c5f469e09d475980133a20987f9cae4cf4f7aedf59f9d8f`  
		Last Modified: Wed, 13 Jan 2021 13:17:19 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84697de3c7d0310176f36e2fe57e5688d23e486eb5b5febf6dbf860e763d1750`  
		Last Modified: Thu, 14 Jan 2021 01:17:09 GMT  
		Size: 30.5 MB (30486249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:069ca4204690196a12b1d26a1b7d9b54c2d8fc7db082a3a4a9e21bfdf55d63d1`  
		Last Modified: Thu, 14 Jan 2021 01:17:02 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adaebdd4a9fa6db73d7167e0d944af020e0ddfe54da3ed92807a14054a53d669`  
		Last Modified: Thu, 14 Jan 2021 01:17:01 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:454fe39b046d9fedbd9e0b3f698556592463406933b790b272dd909d5bd90d53`  
		Last Modified: Thu, 14 Jan 2021 01:17:02 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v1.7-alpine`

```console
$ docker pull traefik@sha256:d232a757f6c487484b3640973fbb0287e747e6b357bc1dc75faa07b26da14a5f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:v1.7-alpine` - linux; amd64

```console
$ docker pull traefik@sha256:cb19d2e6f6575fb121eb2181cbd50f783c1995bf515cba8c7bbab7d9b6859949
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **24.6 MB (24603200 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d9ecef4edf395a65a22e7b3c46ec4b16c869c1a5386a1ea0305132dc68266f04`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 17 Dec 2020 00:19:49 GMT
ADD file:8ed80010e443da19d72546bcee9a35e0a8d244c72052b1994610bf5939d479c2 in / 
# Thu, 17 Dec 2020 00:19:49 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 00:47:33 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 13 Jan 2021 22:29:27 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/traefik/traefik/releases/download/v1.7.28/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Wed, 13 Jan 2021 22:29:27 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 13 Jan 2021 22:29:27 GMT
EXPOSE 80
# Wed, 13 Jan 2021 22:29:27 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 13 Jan 2021 22:29:28 GMT
CMD ["traefik"]
# Wed, 13 Jan 2021 22:29:28 GMT
LABEL org.opencontainers.image.vendor=traefik org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.28 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:0a6724ff3fcd51338afdfdc2b1d4ffd04569818e31efad957213d67c29b45101`  
		Last Modified: Thu, 17 Dec 2020 00:20:26 GMT  
		Size: 2.8 MB (2814864 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64d0c2f48fede0de57585b470af3e8e9aa5534db90642859512370fa53ffac21`  
		Last Modified: Thu, 17 Dec 2020 00:48:37 GMT  
		Size: 671.7 KB (671697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce8923725f26216ece246718b634aabb038e3ba78292d388ebb7350cc0d89ba1`  
		Last Modified: Wed, 13 Jan 2021 22:30:25 GMT  
		Size: 21.1 MB (21116271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f8abe3b22d27fbf46de589e10d21107bd248a725e59317b3fc6a78a83e9c940`  
		Last Modified: Wed, 13 Jan 2021 22:30:19 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v1.7-alpine` - linux; arm variant v6

```console
$ docker pull traefik@sha256:198e33555ab98a4ea7b448b1f818b9663ab2f8fe98f0966543390a711e55692d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.1 MB (23064299 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:92898625b48315d465f9a4d3ad8e32c8b224bb4617bff335d0840bbd9ce1aced`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 16 Dec 2020 23:49:53 GMT
ADD file:e3a6f7566ee3c2ba61d27d801d3522e045a4be64a42f32ee52d933b68338d06f in / 
# Wed, 16 Dec 2020 23:49:55 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 00:25:55 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 13 Jan 2021 21:56:46 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/traefik/traefik/releases/download/v1.7.28/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Wed, 13 Jan 2021 21:56:47 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 13 Jan 2021 21:56:48 GMT
EXPOSE 80
# Wed, 13 Jan 2021 21:56:48 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 13 Jan 2021 21:56:49 GMT
CMD ["traefik"]
# Wed, 13 Jan 2021 21:56:49 GMT
LABEL org.opencontainers.image.vendor=traefik org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.28 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:56fec67ad66eea034cf5b7d0d0ffd355c0fe87611bad132ac5a952fcaa52138b`  
		Last Modified: Wed, 16 Dec 2020 23:50:34 GMT  
		Size: 2.6 MB (2620769 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab096bb24791df9de14fbfc840265a32c0d9f7be463db3a782da6095c0e6ad5b`  
		Last Modified: Thu, 17 Dec 2020 00:27:24 GMT  
		Size: 674.9 KB (674902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:102471939d830c2c1e2668e0dd48049fc6ce2f332ead14922e8a55086f8816ef`  
		Last Modified: Wed, 13 Jan 2021 21:57:48 GMT  
		Size: 19.8 MB (19768260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29a399e8ce2234a61da5e35bf382eefe32e24435b8c5805b773299d16a01b022`  
		Last Modified: Wed, 13 Jan 2021 21:57:42 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v1.7-alpine` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:a144e4ba9554f68e6903986ca95090991e87d3c7a3e45809bfd602a5bda85a3c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **22.9 MB (22884874 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:24c65bf1525b68d03c1cc5d512338cf2608b5742b1e06e6ea57c492e61afee7a`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 16 Dec 2020 23:40:37 GMT
ADD file:47bb1b85a4eb4d0b355ae89ec5c71c09e2c2b7e21e1851a2896365eb17134f57 in / 
# Wed, 16 Dec 2020 23:40:39 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 00:27:02 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 13 Jan 2021 21:46:38 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/traefik/traefik/releases/download/v1.7.28/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Wed, 13 Jan 2021 21:46:39 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 13 Jan 2021 21:46:39 GMT
EXPOSE 80
# Wed, 13 Jan 2021 21:46:40 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 13 Jan 2021 21:46:41 GMT
CMD ["traefik"]
# Wed, 13 Jan 2021 21:46:41 GMT
LABEL org.opencontainers.image.vendor=traefik org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.28 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:20d8a246443a66e74e17f2a0e81a51fe774876ca0c2676691c37ee1b0e4d3cd5`  
		Last Modified: Wed, 16 Dec 2020 23:41:20 GMT  
		Size: 2.7 MB (2725216 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:278abd308a18c136f69dcabbba1dc64486ebdad665d4a2f4ab14d2826ec08b06`  
		Last Modified: Thu, 17 Dec 2020 00:28:38 GMT  
		Size: 673.2 KB (673246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e50dc3ca8b514cac3bfbf2a6303d6be654d1a94f584f6f24d4e62522b80bd36b`  
		Last Modified: Wed, 13 Jan 2021 21:47:33 GMT  
		Size: 19.5 MB (19486044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d4205a3b9bbaa8f65f3bd5780aeb6e4cc761d5f7d6de7cb70588b41ed018c72`  
		Last Modified: Wed, 13 Jan 2021 21:47:27 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v1.7-windowsservercore-1809`

```console
$ docker pull traefik@sha256:8f2b9d477c5d31806d427f5dad762d9f448c131bb284641f3977b914e655afd7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1697; amd64

### `traefik:v1.7-windowsservercore-1809` - windows version 10.0.17763.1697; amd64

```console
$ docker pull traefik@sha256:91b9a8ca83df9afc2b41003518d4b4f9d8e8a21f77880fd74d543670c7ab4da9
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2466262882 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6962de1a7e3fc419a74eb2ea94e4c40359d9f53a93caec6bd1e61f1944ccf282`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 08 Jan 2021 08:50:52 GMT
RUN Install update 1809-amd64
# Wed, 13 Jan 2021 13:13:16 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 14 Jan 2021 01:16:20 GMT
RUN Invoke-WebRequest     -Uri "https://github.com/traefik/traefik/releases/download/v1.7.28/traefik_windows-amd64.exe"     -OutFile "/traefik.exe"
# Thu, 14 Jan 2021 01:16:24 GMT
EXPOSE 80
# Thu, 14 Jan 2021 01:16:25 GMT
ENTRYPOINT ["/traefik"]
# Thu, 14 Jan 2021 01:16:26 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.28 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:4dcc9a9b9e680514ef3fdfcc2ce08a3768f9e412703faa137f4a7c8297600052`  
		Size: 717.4 MB (717439216 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e00081a98bb2679c3c5f469e09d475980133a20987f9cae4cf4f7aedf59f9d8f`  
		Last Modified: Wed, 13 Jan 2021 13:17:19 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84697de3c7d0310176f36e2fe57e5688d23e486eb5b5febf6dbf860e763d1750`  
		Last Modified: Thu, 14 Jan 2021 01:17:09 GMT  
		Size: 30.5 MB (30486249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:069ca4204690196a12b1d26a1b7d9b54c2d8fc7db082a3a4a9e21bfdf55d63d1`  
		Last Modified: Thu, 14 Jan 2021 01:17:02 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adaebdd4a9fa6db73d7167e0d944af020e0ddfe54da3ed92807a14054a53d669`  
		Last Modified: Thu, 14 Jan 2021 01:17:01 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:454fe39b046d9fedbd9e0b3f698556592463406933b790b272dd909d5bd90d53`  
		Last Modified: Thu, 14 Jan 2021 01:17:02 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v2.4`

```console
$ docker pull traefik@sha256:482a48d4268f6edb38aa6934c74acf5d1f14ec2e7c5e813607ac18c958c62482
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:v2.4` - linux; amd64

```console
$ docker pull traefik@sha256:3d2ba657bdec47749235c4a06e0b51d89e6a2a4c72dad70c9fd5f9496c68d871
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.0 MB (29043146 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7dcdc37f2b5f338b1a51a6739a905148dd1c1b189f3d97dd205fced1797f37a0`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 17 Dec 2020 00:19:49 GMT
ADD file:8ed80010e443da19d72546bcee9a35e0a8d244c72052b1994610bf5939d479c2 in / 
# Thu, 17 Dec 2020 00:19:49 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 00:47:33 GMT
RUN apk --no-cache add ca-certificates tzdata
# Mon, 01 Feb 2021 20:36:23 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.4.1/traefik_v2.4.1_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Mon, 01 Feb 2021 20:36:23 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Mon, 01 Feb 2021 20:36:24 GMT
EXPOSE 80
# Mon, 01 Feb 2021 20:36:24 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 01 Feb 2021 20:36:24 GMT
CMD ["traefik"]
# Mon, 01 Feb 2021 20:36:24 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.4.1 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:0a6724ff3fcd51338afdfdc2b1d4ffd04569818e31efad957213d67c29b45101`  
		Last Modified: Thu, 17 Dec 2020 00:20:26 GMT  
		Size: 2.8 MB (2814864 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64d0c2f48fede0de57585b470af3e8e9aa5534db90642859512370fa53ffac21`  
		Last Modified: Thu, 17 Dec 2020 00:48:37 GMT  
		Size: 671.7 KB (671697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1516ade513da1a48f2452fb045c9f59dcb754ec8a45d295fb62c02ca3ce2fa24`  
		Last Modified: Mon, 01 Feb 2021 20:36:56 GMT  
		Size: 25.6 MB (25556218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1646cce883d51cde2f62db17c3ffca7a86fb6b363e190158baacb784df1cd067`  
		Last Modified: Mon, 01 Feb 2021 20:36:51 GMT  
		Size: 367.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v2.4` - linux; arm variant v6

```console
$ docker pull traefik@sha256:a784cf52ea56aea0b24a9906cb19b4b4378a93c7d883df4315cd2274006373ec
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.1 MB (27087182 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:791475a3abf40af6d79e4c48790e71f85dac37a4ff31bfdf59b305585c037bb3`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 16 Dec 2020 23:49:53 GMT
ADD file:e3a6f7566ee3c2ba61d27d801d3522e045a4be64a42f32ee52d933b68338d06f in / 
# Wed, 16 Dec 2020 23:49:55 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 00:25:55 GMT
RUN apk --no-cache add ca-certificates tzdata
# Mon, 01 Feb 2021 20:21:51 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.4.1/traefik_v2.4.1_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Mon, 01 Feb 2021 20:21:52 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Mon, 01 Feb 2021 20:21:54 GMT
EXPOSE 80
# Mon, 01 Feb 2021 20:21:57 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 01 Feb 2021 20:21:59 GMT
CMD ["traefik"]
# Mon, 01 Feb 2021 20:22:00 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.4.1 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:56fec67ad66eea034cf5b7d0d0ffd355c0fe87611bad132ac5a952fcaa52138b`  
		Last Modified: Wed, 16 Dec 2020 23:50:34 GMT  
		Size: 2.6 MB (2620769 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab096bb24791df9de14fbfc840265a32c0d9f7be463db3a782da6095c0e6ad5b`  
		Last Modified: Thu, 17 Dec 2020 00:27:24 GMT  
		Size: 674.9 KB (674902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0eb4fee172158a2a6626c7064a033878a7a6cfc5b3fee45c74d6d44e05bc9370`  
		Last Modified: Mon, 01 Feb 2021 20:22:38 GMT  
		Size: 23.8 MB (23791143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b36a51bbc86a42ed580e716a14368625f925ffe68f228ecaa6c1ee5d7705d560`  
		Last Modified: Mon, 01 Feb 2021 20:22:29 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v2.4` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:7353217d113ec6673f0215e2623b81af6251fbd4f7745078621617b498491b42
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.7 MB (26708518 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6688c1a122c4a87c308f5addeac11defec355c3db5836db65675df5c979340e2`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 16 Dec 2020 23:40:37 GMT
ADD file:47bb1b85a4eb4d0b355ae89ec5c71c09e2c2b7e21e1851a2896365eb17134f57 in / 
# Wed, 16 Dec 2020 23:40:39 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 00:27:02 GMT
RUN apk --no-cache add ca-certificates tzdata
# Mon, 01 Feb 2021 21:04:10 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.4.1/traefik_v2.4.1_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Mon, 01 Feb 2021 21:04:11 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Mon, 01 Feb 2021 21:04:11 GMT
EXPOSE 80
# Mon, 01 Feb 2021 21:04:12 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 01 Feb 2021 21:04:12 GMT
CMD ["traefik"]
# Mon, 01 Feb 2021 21:04:13 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.4.1 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:20d8a246443a66e74e17f2a0e81a51fe774876ca0c2676691c37ee1b0e4d3cd5`  
		Last Modified: Wed, 16 Dec 2020 23:41:20 GMT  
		Size: 2.7 MB (2725216 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:278abd308a18c136f69dcabbba1dc64486ebdad665d4a2f4ab14d2826ec08b06`  
		Last Modified: Thu, 17 Dec 2020 00:28:38 GMT  
		Size: 673.2 KB (673246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76f99e8acab44e0da3e7667fedfc874ddb6f2fa2bf1814aa29cbcd5f97d091c4`  
		Last Modified: Mon, 01 Feb 2021 21:04:49 GMT  
		Size: 23.3 MB (23309688 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f579f772bccf2955a27d99b4778f4f174e3fb78837376c77f98385cdcbe2bdce`  
		Last Modified: Mon, 01 Feb 2021 21:04:43 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v2.4.1`

```console
$ docker pull traefik@sha256:482a48d4268f6edb38aa6934c74acf5d1f14ec2e7c5e813607ac18c958c62482
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:v2.4.1` - linux; amd64

```console
$ docker pull traefik@sha256:3d2ba657bdec47749235c4a06e0b51d89e6a2a4c72dad70c9fd5f9496c68d871
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.0 MB (29043146 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7dcdc37f2b5f338b1a51a6739a905148dd1c1b189f3d97dd205fced1797f37a0`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 17 Dec 2020 00:19:49 GMT
ADD file:8ed80010e443da19d72546bcee9a35e0a8d244c72052b1994610bf5939d479c2 in / 
# Thu, 17 Dec 2020 00:19:49 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 00:47:33 GMT
RUN apk --no-cache add ca-certificates tzdata
# Mon, 01 Feb 2021 20:36:23 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.4.1/traefik_v2.4.1_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Mon, 01 Feb 2021 20:36:23 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Mon, 01 Feb 2021 20:36:24 GMT
EXPOSE 80
# Mon, 01 Feb 2021 20:36:24 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 01 Feb 2021 20:36:24 GMT
CMD ["traefik"]
# Mon, 01 Feb 2021 20:36:24 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.4.1 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:0a6724ff3fcd51338afdfdc2b1d4ffd04569818e31efad957213d67c29b45101`  
		Last Modified: Thu, 17 Dec 2020 00:20:26 GMT  
		Size: 2.8 MB (2814864 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64d0c2f48fede0de57585b470af3e8e9aa5534db90642859512370fa53ffac21`  
		Last Modified: Thu, 17 Dec 2020 00:48:37 GMT  
		Size: 671.7 KB (671697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1516ade513da1a48f2452fb045c9f59dcb754ec8a45d295fb62c02ca3ce2fa24`  
		Last Modified: Mon, 01 Feb 2021 20:36:56 GMT  
		Size: 25.6 MB (25556218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1646cce883d51cde2f62db17c3ffca7a86fb6b363e190158baacb784df1cd067`  
		Last Modified: Mon, 01 Feb 2021 20:36:51 GMT  
		Size: 367.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v2.4.1` - linux; arm variant v6

```console
$ docker pull traefik@sha256:a784cf52ea56aea0b24a9906cb19b4b4378a93c7d883df4315cd2274006373ec
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.1 MB (27087182 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:791475a3abf40af6d79e4c48790e71f85dac37a4ff31bfdf59b305585c037bb3`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 16 Dec 2020 23:49:53 GMT
ADD file:e3a6f7566ee3c2ba61d27d801d3522e045a4be64a42f32ee52d933b68338d06f in / 
# Wed, 16 Dec 2020 23:49:55 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 00:25:55 GMT
RUN apk --no-cache add ca-certificates tzdata
# Mon, 01 Feb 2021 20:21:51 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.4.1/traefik_v2.4.1_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Mon, 01 Feb 2021 20:21:52 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Mon, 01 Feb 2021 20:21:54 GMT
EXPOSE 80
# Mon, 01 Feb 2021 20:21:57 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 01 Feb 2021 20:21:59 GMT
CMD ["traefik"]
# Mon, 01 Feb 2021 20:22:00 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.4.1 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:56fec67ad66eea034cf5b7d0d0ffd355c0fe87611bad132ac5a952fcaa52138b`  
		Last Modified: Wed, 16 Dec 2020 23:50:34 GMT  
		Size: 2.6 MB (2620769 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab096bb24791df9de14fbfc840265a32c0d9f7be463db3a782da6095c0e6ad5b`  
		Last Modified: Thu, 17 Dec 2020 00:27:24 GMT  
		Size: 674.9 KB (674902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0eb4fee172158a2a6626c7064a033878a7a6cfc5b3fee45c74d6d44e05bc9370`  
		Last Modified: Mon, 01 Feb 2021 20:22:38 GMT  
		Size: 23.8 MB (23791143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b36a51bbc86a42ed580e716a14368625f925ffe68f228ecaa6c1ee5d7705d560`  
		Last Modified: Mon, 01 Feb 2021 20:22:29 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v2.4.1` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:7353217d113ec6673f0215e2623b81af6251fbd4f7745078621617b498491b42
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.7 MB (26708518 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6688c1a122c4a87c308f5addeac11defec355c3db5836db65675df5c979340e2`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 16 Dec 2020 23:40:37 GMT
ADD file:47bb1b85a4eb4d0b355ae89ec5c71c09e2c2b7e21e1851a2896365eb17134f57 in / 
# Wed, 16 Dec 2020 23:40:39 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 00:27:02 GMT
RUN apk --no-cache add ca-certificates tzdata
# Mon, 01 Feb 2021 21:04:10 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.4.1/traefik_v2.4.1_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Mon, 01 Feb 2021 21:04:11 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Mon, 01 Feb 2021 21:04:11 GMT
EXPOSE 80
# Mon, 01 Feb 2021 21:04:12 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 01 Feb 2021 21:04:12 GMT
CMD ["traefik"]
# Mon, 01 Feb 2021 21:04:13 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.4.1 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:20d8a246443a66e74e17f2a0e81a51fe774876ca0c2676691c37ee1b0e4d3cd5`  
		Last Modified: Wed, 16 Dec 2020 23:41:20 GMT  
		Size: 2.7 MB (2725216 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:278abd308a18c136f69dcabbba1dc64486ebdad665d4a2f4ab14d2826ec08b06`  
		Last Modified: Thu, 17 Dec 2020 00:28:38 GMT  
		Size: 673.2 KB (673246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76f99e8acab44e0da3e7667fedfc874ddb6f2fa2bf1814aa29cbcd5f97d091c4`  
		Last Modified: Mon, 01 Feb 2021 21:04:49 GMT  
		Size: 23.3 MB (23309688 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f579f772bccf2955a27d99b4778f4f174e3fb78837376c77f98385cdcbe2bdce`  
		Last Modified: Mon, 01 Feb 2021 21:04:43 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v2.4.1-windowsservercore-1809`

```console
$ docker pull traefik@sha256:f8a909841f70c259ea7e5c4e4e6711fd047fafa7ca6be1114bc390e0ac69db02
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1697; amd64

### `traefik:v2.4.1-windowsservercore-1809` - windows version 10.0.17763.1697; amd64

```console
$ docker pull traefik@sha256:6592087c3b637b852ccb83524da4e563fdbd1aa01c36c7dca55fa4154c908a9f
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2471089030 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1a4da9297c49ca2d742c3719308666352f9a5837f20529b203e86b3490850930`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 08 Jan 2021 08:50:52 GMT
RUN Install update 1809-amd64
# Wed, 13 Jan 2021 13:13:16 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Mon, 01 Feb 2021 20:14:38 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/traefik/traefik/releases/download/v2.4.1/traefik_v2.4.1_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Mon, 01 Feb 2021 20:14:39 GMT
EXPOSE 80
# Mon, 01 Feb 2021 20:14:40 GMT
ENTRYPOINT ["/traefik"]
# Mon, 01 Feb 2021 20:14:41 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.4.1 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:4dcc9a9b9e680514ef3fdfcc2ce08a3768f9e412703faa137f4a7c8297600052`  
		Size: 717.4 MB (717439216 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e00081a98bb2679c3c5f469e09d475980133a20987f9cae4cf4f7aedf59f9d8f`  
		Last Modified: Wed, 13 Jan 2021 13:17:19 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff2522d016390dfd18d8aeb8e2c6aff006cd1f9247bf87ead249db540db5125b`  
		Last Modified: Mon, 01 Feb 2021 20:15:44 GMT  
		Size: 35.3 MB (35311531 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76e10af105fbd4d7ed8322d6268a8e63f903e9d06ff682e3ff1ee966c9663fc0`  
		Last Modified: Mon, 01 Feb 2021 20:15:05 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8e3489a01f3df87bb94b5f1841f336b002617ecfed15c6adfa8e1661322c0c1`  
		Last Modified: Mon, 01 Feb 2021 20:15:05 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ff1204038344324e029d7469e15ec9baa18f1abbc2de83a0ae4a7e295a6eea9`  
		Last Modified: Mon, 01 Feb 2021 20:15:05 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v2.4-windowsservercore-1809`

```console
$ docker pull traefik@sha256:f8a909841f70c259ea7e5c4e4e6711fd047fafa7ca6be1114bc390e0ac69db02
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1697; amd64

### `traefik:v2.4-windowsservercore-1809` - windows version 10.0.17763.1697; amd64

```console
$ docker pull traefik@sha256:6592087c3b637b852ccb83524da4e563fdbd1aa01c36c7dca55fa4154c908a9f
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2471089030 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1a4da9297c49ca2d742c3719308666352f9a5837f20529b203e86b3490850930`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 08 Jan 2021 08:50:52 GMT
RUN Install update 1809-amd64
# Wed, 13 Jan 2021 13:13:16 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Mon, 01 Feb 2021 20:14:38 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/traefik/traefik/releases/download/v2.4.1/traefik_v2.4.1_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Mon, 01 Feb 2021 20:14:39 GMT
EXPOSE 80
# Mon, 01 Feb 2021 20:14:40 GMT
ENTRYPOINT ["/traefik"]
# Mon, 01 Feb 2021 20:14:41 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.4.1 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:4dcc9a9b9e680514ef3fdfcc2ce08a3768f9e412703faa137f4a7c8297600052`  
		Size: 717.4 MB (717439216 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e00081a98bb2679c3c5f469e09d475980133a20987f9cae4cf4f7aedf59f9d8f`  
		Last Modified: Wed, 13 Jan 2021 13:17:19 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff2522d016390dfd18d8aeb8e2c6aff006cd1f9247bf87ead249db540db5125b`  
		Last Modified: Mon, 01 Feb 2021 20:15:44 GMT  
		Size: 35.3 MB (35311531 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76e10af105fbd4d7ed8322d6268a8e63f903e9d06ff682e3ff1ee966c9663fc0`  
		Last Modified: Mon, 01 Feb 2021 20:15:05 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8e3489a01f3df87bb94b5f1841f336b002617ecfed15c6adfa8e1661322c0c1`  
		Last Modified: Mon, 01 Feb 2021 20:15:05 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ff1204038344324e029d7469e15ec9baa18f1abbc2de83a0ae4a7e295a6eea9`  
		Last Modified: Mon, 01 Feb 2021 20:15:05 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:windowsservercore-1809`

```console
$ docker pull traefik@sha256:f8a909841f70c259ea7e5c4e4e6711fd047fafa7ca6be1114bc390e0ac69db02
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1697; amd64

### `traefik:windowsservercore-1809` - windows version 10.0.17763.1697; amd64

```console
$ docker pull traefik@sha256:6592087c3b637b852ccb83524da4e563fdbd1aa01c36c7dca55fa4154c908a9f
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2471089030 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1a4da9297c49ca2d742c3719308666352f9a5837f20529b203e86b3490850930`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 08 Jan 2021 08:50:52 GMT
RUN Install update 1809-amd64
# Wed, 13 Jan 2021 13:13:16 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Mon, 01 Feb 2021 20:14:38 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/traefik/traefik/releases/download/v2.4.1/traefik_v2.4.1_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Mon, 01 Feb 2021 20:14:39 GMT
EXPOSE 80
# Mon, 01 Feb 2021 20:14:40 GMT
ENTRYPOINT ["/traefik"]
# Mon, 01 Feb 2021 20:14:41 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.4.1 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:4dcc9a9b9e680514ef3fdfcc2ce08a3768f9e412703faa137f4a7c8297600052`  
		Size: 717.4 MB (717439216 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e00081a98bb2679c3c5f469e09d475980133a20987f9cae4cf4f7aedf59f9d8f`  
		Last Modified: Wed, 13 Jan 2021 13:17:19 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff2522d016390dfd18d8aeb8e2c6aff006cd1f9247bf87ead249db540db5125b`  
		Last Modified: Mon, 01 Feb 2021 20:15:44 GMT  
		Size: 35.3 MB (35311531 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76e10af105fbd4d7ed8322d6268a8e63f903e9d06ff682e3ff1ee966c9663fc0`  
		Last Modified: Mon, 01 Feb 2021 20:15:05 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8e3489a01f3df87bb94b5f1841f336b002617ecfed15c6adfa8e1661322c0c1`  
		Last Modified: Mon, 01 Feb 2021 20:15:05 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ff1204038344324e029d7469e15ec9baa18f1abbc2de83a0ae4a7e295a6eea9`  
		Last Modified: Mon, 01 Feb 2021 20:15:05 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
