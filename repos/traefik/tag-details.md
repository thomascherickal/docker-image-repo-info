<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `traefik`

-	[`traefik:1.7`](#traefik17)
-	[`traefik:1.7.28`](#traefik1728)
-	[`traefik:1.7.28-alpine`](#traefik1728-alpine)
-	[`traefik:1.7.28-windowsservercore-1809`](#traefik1728-windowsservercore-1809)
-	[`traefik:1.7-alpine`](#traefik17-alpine)
-	[`traefik:1.7-windowsservercore-1809`](#traefik17-windowsservercore-1809)
-	[`traefik:2.4`](#traefik24)
-	[`traefik:2.4.5`](#traefik245)
-	[`traefik:2.4.5-windowsservercore-1809`](#traefik245-windowsservercore-1809)
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
-	[`traefik:v2.4.5`](#traefikv245)
-	[`traefik:v2.4.5-windowsservercore-1809`](#traefikv245-windowsservercore-1809)
-	[`traefik:v2.4-windowsservercore-1809`](#traefikv24-windowsservercore-1809)
-	[`traefik:windowsservercore-1809`](#traefikwindowsservercore-1809)

## `traefik:1.7`

```console
$ docker pull traefik@sha256:5325e0f4d374b9fd87550465b3145415c24ce90d56f839632e56875ce4072844
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
$ docker pull traefik@sha256:5325e0f4d374b9fd87550465b3145415c24ce90d56f839632e56875ce4072844
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
$ docker pull traefik@sha256:aaf51dc5d08b6aa95894d72fa53f587b3093d4b3cc9626ef42c17d5df630db76
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
$ docker pull traefik@sha256:4b4a41ca1cdc6e1b98793fcd9ba92b1a561c16eddf9c30aa2815feab850205b4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1757; amd64

### `traefik:1.7.28-windowsservercore-1809` - windows version 10.0.17763.1757; amd64

```console
$ docker pull traefik@sha256:697e5dbefbd4bcaef22f89382f30639ed29a3292fdd188cf807bb71546eabeb4
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2469803792 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e71a612ec4fa6c6b261321c8fe09e059ee040cb04218657389bac3c9ce002eed`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 06 Feb 2021 05:03:14 GMT
RUN Install update 1809-amd64
# Wed, 10 Feb 2021 13:14:02 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Feb 2021 20:10:24 GMT
RUN Invoke-WebRequest     -Uri "https://github.com/traefik/traefik/releases/download/v1.7.28/traefik_windows-amd64.exe"     -OutFile "/traefik.exe"
# Wed, 10 Feb 2021 20:10:25 GMT
EXPOSE 80
# Wed, 10 Feb 2021 20:10:26 GMT
ENTRYPOINT ["/traefik"]
# Wed, 10 Feb 2021 20:10:27 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.28 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:db4edcf0861ff3fdc41851a5a218965ecb2ab6cf4ec9448fb80cc4b6792fd46c`  
		Size: 720.9 MB (720933935 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:433d24156d44dde3b3c6c0094ba5824a315286ae537c68f272e464fc426510f6`  
		Last Modified: Wed, 10 Feb 2021 13:40:44 GMT  
		Size: 1.4 KB (1362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:639352e9914386a0227a0fbdfe068f0eecb8206eeb528ebbb1006dc69f155ae8`  
		Last Modified: Wed, 10 Feb 2021 20:11:58 GMT  
		Size: 30.5 MB (30531541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:875bd0eab58c3c0eb449d5641c8d341956ca8df8e79a9960d1b9176d28b7f872`  
		Last Modified: Wed, 10 Feb 2021 20:11:51 GMT  
		Size: 1.3 KB (1349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b14f079b8ee9624c2313d782b2d9a04723215c063eca353822eafbf3ee0a2b59`  
		Last Modified: Wed, 10 Feb 2021 20:11:51 GMT  
		Size: 1.4 KB (1390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3063b85a538300feec077a4ebd3b11960a83a55adb2de40370e013212cfe2e6`  
		Last Modified: Wed, 10 Feb 2021 20:11:51 GMT  
		Size: 1.3 KB (1336 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:1.7-alpine`

```console
$ docker pull traefik@sha256:aaf51dc5d08b6aa95894d72fa53f587b3093d4b3cc9626ef42c17d5df630db76
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
$ docker pull traefik@sha256:4b4a41ca1cdc6e1b98793fcd9ba92b1a561c16eddf9c30aa2815feab850205b4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1757; amd64

### `traefik:1.7-windowsservercore-1809` - windows version 10.0.17763.1757; amd64

```console
$ docker pull traefik@sha256:697e5dbefbd4bcaef22f89382f30639ed29a3292fdd188cf807bb71546eabeb4
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2469803792 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e71a612ec4fa6c6b261321c8fe09e059ee040cb04218657389bac3c9ce002eed`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 06 Feb 2021 05:03:14 GMT
RUN Install update 1809-amd64
# Wed, 10 Feb 2021 13:14:02 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Feb 2021 20:10:24 GMT
RUN Invoke-WebRequest     -Uri "https://github.com/traefik/traefik/releases/download/v1.7.28/traefik_windows-amd64.exe"     -OutFile "/traefik.exe"
# Wed, 10 Feb 2021 20:10:25 GMT
EXPOSE 80
# Wed, 10 Feb 2021 20:10:26 GMT
ENTRYPOINT ["/traefik"]
# Wed, 10 Feb 2021 20:10:27 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.28 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:db4edcf0861ff3fdc41851a5a218965ecb2ab6cf4ec9448fb80cc4b6792fd46c`  
		Size: 720.9 MB (720933935 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:433d24156d44dde3b3c6c0094ba5824a315286ae537c68f272e464fc426510f6`  
		Last Modified: Wed, 10 Feb 2021 13:40:44 GMT  
		Size: 1.4 KB (1362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:639352e9914386a0227a0fbdfe068f0eecb8206eeb528ebbb1006dc69f155ae8`  
		Last Modified: Wed, 10 Feb 2021 20:11:58 GMT  
		Size: 30.5 MB (30531541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:875bd0eab58c3c0eb449d5641c8d341956ca8df8e79a9960d1b9176d28b7f872`  
		Last Modified: Wed, 10 Feb 2021 20:11:51 GMT  
		Size: 1.3 KB (1349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b14f079b8ee9624c2313d782b2d9a04723215c063eca353822eafbf3ee0a2b59`  
		Last Modified: Wed, 10 Feb 2021 20:11:51 GMT  
		Size: 1.4 KB (1390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3063b85a538300feec077a4ebd3b11960a83a55adb2de40370e013212cfe2e6`  
		Last Modified: Wed, 10 Feb 2021 20:11:51 GMT  
		Size: 1.3 KB (1336 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:2.4`

```console
$ docker pull traefik@sha256:4d303938bde19f213ab9888fe48c42138d4ad8392cdd4bc52b5f3f2d226b9c24
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:2.4` - linux; amd64

```console
$ docker pull traefik@sha256:2cec9f638bf256272fc3b7df23f72e84edcbab613aa7aa66c96ff67c90885164
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.1 MB (29068973 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:66c68650f9a1d2203914c7437252596c135158de12607225d9c62c332d6932d6`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 17 Dec 2020 00:19:49 GMT
ADD file:8ed80010e443da19d72546bcee9a35e0a8d244c72052b1994610bf5939d479c2 in / 
# Thu, 17 Dec 2020 00:19:49 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 00:47:33 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 18 Feb 2021 19:21:01 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.4.5/traefik_v2.4.5_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 18 Feb 2021 19:21:01 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 18 Feb 2021 19:21:01 GMT
EXPOSE 80
# Thu, 18 Feb 2021 19:21:01 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 18 Feb 2021 19:21:02 GMT
CMD ["traefik"]
# Thu, 18 Feb 2021 19:21:02 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.4.5 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:7a43eed822408ece4014703bda46018fc52ffc73fe801e045f6ff8dcc67c71c4`  
		Last Modified: Thu, 18 Feb 2021 19:21:30 GMT  
		Size: 25.6 MB (25582044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0383ad4de15380b230a3391b092c22a7efa30b126f7033acdfaa91180dca7e9`  
		Last Modified: Thu, 18 Feb 2021 19:21:26 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:2.4` - linux; arm variant v6

```console
$ docker pull traefik@sha256:51e6acb6b11a005142df938a5c8364906bf46bfc72b336a25816da84a1f97b3f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.1 MB (27118958 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6e41e625833706e636d407ac328f8f6f0a458c3665c50e921be02c2246900373`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 24 Feb 2021 20:50:45 GMT
ADD file:72743cfd9913f13553e700f9d9cfdc17b9dc793ebeeb337fd5fe02dc962d4b63 in / 
# Wed, 24 Feb 2021 20:50:46 GMT
CMD ["/bin/sh"]
# Wed, 24 Feb 2021 23:33:31 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 24 Feb 2021 23:33:37 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.4.5/traefik_v2.4.5_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Wed, 24 Feb 2021 23:33:39 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 24 Feb 2021 23:33:39 GMT
EXPOSE 80
# Wed, 24 Feb 2021 23:33:40 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 24 Feb 2021 23:33:41 GMT
CMD ["traefik"]
# Wed, 24 Feb 2021 23:33:41 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.4.5 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:72e8de7d15c4484a563097a94cbab858afe450985c4b372f94b522b5ea1d8fa6`  
		Last Modified: Wed, 24 Feb 2021 23:35:25 GMT  
		Size: 23.8 MB (23820517 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f48c4b827d0213635a8cc7951840f4390b222dc4556e5e471dfc6f190f71dce`  
		Last Modified: Wed, 24 Feb 2021 23:35:10 GMT  
		Size: 367.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:2.4` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:d192f9f1bbd0e0e799b36f3e923cf4c541d53dfb3af4de5a7ca07f0c666b0c75
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.7 MB (26732718 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f46bc576d13c9ed7dd38a1615fa6e697520634a83a48d35cf19449f180e6a518`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 16 Dec 2020 23:40:37 GMT
ADD file:47bb1b85a4eb4d0b355ae89ec5c71c09e2c2b7e21e1851a2896365eb17134f57 in / 
# Wed, 16 Dec 2020 23:40:39 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 00:27:02 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 18 Feb 2021 19:42:27 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.4.5/traefik_v2.4.5_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 18 Feb 2021 19:42:28 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 18 Feb 2021 19:42:29 GMT
EXPOSE 80
# Thu, 18 Feb 2021 19:42:29 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 18 Feb 2021 19:42:30 GMT
CMD ["traefik"]
# Thu, 18 Feb 2021 19:42:31 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.4.5 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:0cde3dd4acbae4754ea88e0519144e399c757804c4e7cd6c7b981b1c424e9d2e`  
		Last Modified: Thu, 18 Feb 2021 19:43:06 GMT  
		Size: 23.3 MB (23333888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fe295f200a4508af4e26b28b5716ee3afb0cc15b6c8a5472fc9e473e0c02fe1`  
		Last Modified: Thu, 18 Feb 2021 19:42:59 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:2.4.5`

```console
$ docker pull traefik@sha256:4d303938bde19f213ab9888fe48c42138d4ad8392cdd4bc52b5f3f2d226b9c24
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:2.4.5` - linux; amd64

```console
$ docker pull traefik@sha256:2cec9f638bf256272fc3b7df23f72e84edcbab613aa7aa66c96ff67c90885164
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.1 MB (29068973 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:66c68650f9a1d2203914c7437252596c135158de12607225d9c62c332d6932d6`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 17 Dec 2020 00:19:49 GMT
ADD file:8ed80010e443da19d72546bcee9a35e0a8d244c72052b1994610bf5939d479c2 in / 
# Thu, 17 Dec 2020 00:19:49 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 00:47:33 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 18 Feb 2021 19:21:01 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.4.5/traefik_v2.4.5_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 18 Feb 2021 19:21:01 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 18 Feb 2021 19:21:01 GMT
EXPOSE 80
# Thu, 18 Feb 2021 19:21:01 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 18 Feb 2021 19:21:02 GMT
CMD ["traefik"]
# Thu, 18 Feb 2021 19:21:02 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.4.5 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:7a43eed822408ece4014703bda46018fc52ffc73fe801e045f6ff8dcc67c71c4`  
		Last Modified: Thu, 18 Feb 2021 19:21:30 GMT  
		Size: 25.6 MB (25582044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0383ad4de15380b230a3391b092c22a7efa30b126f7033acdfaa91180dca7e9`  
		Last Modified: Thu, 18 Feb 2021 19:21:26 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:2.4.5` - linux; arm variant v6

```console
$ docker pull traefik@sha256:51e6acb6b11a005142df938a5c8364906bf46bfc72b336a25816da84a1f97b3f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.1 MB (27118958 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6e41e625833706e636d407ac328f8f6f0a458c3665c50e921be02c2246900373`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 24 Feb 2021 20:50:45 GMT
ADD file:72743cfd9913f13553e700f9d9cfdc17b9dc793ebeeb337fd5fe02dc962d4b63 in / 
# Wed, 24 Feb 2021 20:50:46 GMT
CMD ["/bin/sh"]
# Wed, 24 Feb 2021 23:33:31 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 24 Feb 2021 23:33:37 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.4.5/traefik_v2.4.5_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Wed, 24 Feb 2021 23:33:39 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 24 Feb 2021 23:33:39 GMT
EXPOSE 80
# Wed, 24 Feb 2021 23:33:40 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 24 Feb 2021 23:33:41 GMT
CMD ["traefik"]
# Wed, 24 Feb 2021 23:33:41 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.4.5 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:72e8de7d15c4484a563097a94cbab858afe450985c4b372f94b522b5ea1d8fa6`  
		Last Modified: Wed, 24 Feb 2021 23:35:25 GMT  
		Size: 23.8 MB (23820517 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f48c4b827d0213635a8cc7951840f4390b222dc4556e5e471dfc6f190f71dce`  
		Last Modified: Wed, 24 Feb 2021 23:35:10 GMT  
		Size: 367.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:2.4.5` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:d192f9f1bbd0e0e799b36f3e923cf4c541d53dfb3af4de5a7ca07f0c666b0c75
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.7 MB (26732718 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f46bc576d13c9ed7dd38a1615fa6e697520634a83a48d35cf19449f180e6a518`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 16 Dec 2020 23:40:37 GMT
ADD file:47bb1b85a4eb4d0b355ae89ec5c71c09e2c2b7e21e1851a2896365eb17134f57 in / 
# Wed, 16 Dec 2020 23:40:39 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 00:27:02 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 18 Feb 2021 19:42:27 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.4.5/traefik_v2.4.5_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 18 Feb 2021 19:42:28 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 18 Feb 2021 19:42:29 GMT
EXPOSE 80
# Thu, 18 Feb 2021 19:42:29 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 18 Feb 2021 19:42:30 GMT
CMD ["traefik"]
# Thu, 18 Feb 2021 19:42:31 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.4.5 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:0cde3dd4acbae4754ea88e0519144e399c757804c4e7cd6c7b981b1c424e9d2e`  
		Last Modified: Thu, 18 Feb 2021 19:43:06 GMT  
		Size: 23.3 MB (23333888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fe295f200a4508af4e26b28b5716ee3afb0cc15b6c8a5472fc9e473e0c02fe1`  
		Last Modified: Thu, 18 Feb 2021 19:42:59 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:2.4.5-windowsservercore-1809`

```console
$ docker pull traefik@sha256:56c556d77094bf8a496466fe0ec56ff819930ef465d252dd4887a68581bbf65b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1757; amd64

### `traefik:2.4.5-windowsservercore-1809` - windows version 10.0.17763.1757; amd64

```console
$ docker pull traefik@sha256:dccfae71811f7f07f664e6e60cb651ecdb00d1cb0754b7d7e920eaa494718111
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2474658912 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:678cdb23a8e3694a9f36cc33974dfcf56d9d68726c676dfdb05fcdc0ceca6dd1`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 06 Feb 2021 05:03:14 GMT
RUN Install update 1809-amd64
# Wed, 10 Feb 2021 13:14:02 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 18 Feb 2021 19:16:05 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/traefik/traefik/releases/download/v2.4.5/traefik_v2.4.5_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Thu, 18 Feb 2021 19:16:07 GMT
EXPOSE 80
# Thu, 18 Feb 2021 19:16:08 GMT
ENTRYPOINT ["/traefik"]
# Thu, 18 Feb 2021 19:16:10 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.4.5 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:db4edcf0861ff3fdc41851a5a218965ecb2ab6cf4ec9448fb80cc4b6792fd46c`  
		Size: 720.9 MB (720933935 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:433d24156d44dde3b3c6c0094ba5824a315286ae537c68f272e464fc426510f6`  
		Last Modified: Wed, 10 Feb 2021 13:40:44 GMT  
		Size: 1.4 KB (1362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1f6a9a190cd76e08337bdbcb4151e2209a8eb869350410b69abc00520909b49`  
		Last Modified: Thu, 18 Feb 2021 19:16:58 GMT  
		Size: 35.4 MB (35386459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3842dc9cd16d601823a69250f2125c318e7c55f63a7a247d9359f2ffe84a662`  
		Last Modified: Thu, 18 Feb 2021 19:16:50 GMT  
		Size: 1.4 KB (1444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dba0a130b3c525c6d7cdd4a3661e9ceaa11bb9287f0823bf8220028c6878d78d`  
		Last Modified: Thu, 18 Feb 2021 19:16:49 GMT  
		Size: 1.4 KB (1402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9924892ced120ed01c98e4f2489c0d44fa78f5258239f969a9910a81ef17c234`  
		Last Modified: Thu, 18 Feb 2021 19:16:49 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:2.4-windowsservercore-1809`

```console
$ docker pull traefik@sha256:56c556d77094bf8a496466fe0ec56ff819930ef465d252dd4887a68581bbf65b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1757; amd64

### `traefik:2.4-windowsservercore-1809` - windows version 10.0.17763.1757; amd64

```console
$ docker pull traefik@sha256:dccfae71811f7f07f664e6e60cb651ecdb00d1cb0754b7d7e920eaa494718111
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2474658912 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:678cdb23a8e3694a9f36cc33974dfcf56d9d68726c676dfdb05fcdc0ceca6dd1`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 06 Feb 2021 05:03:14 GMT
RUN Install update 1809-amd64
# Wed, 10 Feb 2021 13:14:02 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 18 Feb 2021 19:16:05 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/traefik/traefik/releases/download/v2.4.5/traefik_v2.4.5_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Thu, 18 Feb 2021 19:16:07 GMT
EXPOSE 80
# Thu, 18 Feb 2021 19:16:08 GMT
ENTRYPOINT ["/traefik"]
# Thu, 18 Feb 2021 19:16:10 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.4.5 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:db4edcf0861ff3fdc41851a5a218965ecb2ab6cf4ec9448fb80cc4b6792fd46c`  
		Size: 720.9 MB (720933935 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:433d24156d44dde3b3c6c0094ba5824a315286ae537c68f272e464fc426510f6`  
		Last Modified: Wed, 10 Feb 2021 13:40:44 GMT  
		Size: 1.4 KB (1362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1f6a9a190cd76e08337bdbcb4151e2209a8eb869350410b69abc00520909b49`  
		Last Modified: Thu, 18 Feb 2021 19:16:58 GMT  
		Size: 35.4 MB (35386459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3842dc9cd16d601823a69250f2125c318e7c55f63a7a247d9359f2ffe84a662`  
		Last Modified: Thu, 18 Feb 2021 19:16:50 GMT  
		Size: 1.4 KB (1444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dba0a130b3c525c6d7cdd4a3661e9ceaa11bb9287f0823bf8220028c6878d78d`  
		Last Modified: Thu, 18 Feb 2021 19:16:49 GMT  
		Size: 1.4 KB (1402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9924892ced120ed01c98e4f2489c0d44fa78f5258239f969a9910a81ef17c234`  
		Last Modified: Thu, 18 Feb 2021 19:16:49 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:latest`

```console
$ docker pull traefik@sha256:4d303938bde19f213ab9888fe48c42138d4ad8392cdd4bc52b5f3f2d226b9c24
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:latest` - linux; amd64

```console
$ docker pull traefik@sha256:2cec9f638bf256272fc3b7df23f72e84edcbab613aa7aa66c96ff67c90885164
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.1 MB (29068973 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:66c68650f9a1d2203914c7437252596c135158de12607225d9c62c332d6932d6`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 17 Dec 2020 00:19:49 GMT
ADD file:8ed80010e443da19d72546bcee9a35e0a8d244c72052b1994610bf5939d479c2 in / 
# Thu, 17 Dec 2020 00:19:49 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 00:47:33 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 18 Feb 2021 19:21:01 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.4.5/traefik_v2.4.5_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 18 Feb 2021 19:21:01 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 18 Feb 2021 19:21:01 GMT
EXPOSE 80
# Thu, 18 Feb 2021 19:21:01 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 18 Feb 2021 19:21:02 GMT
CMD ["traefik"]
# Thu, 18 Feb 2021 19:21:02 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.4.5 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:7a43eed822408ece4014703bda46018fc52ffc73fe801e045f6ff8dcc67c71c4`  
		Last Modified: Thu, 18 Feb 2021 19:21:30 GMT  
		Size: 25.6 MB (25582044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0383ad4de15380b230a3391b092c22a7efa30b126f7033acdfaa91180dca7e9`  
		Last Modified: Thu, 18 Feb 2021 19:21:26 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:latest` - linux; arm variant v6

```console
$ docker pull traefik@sha256:51e6acb6b11a005142df938a5c8364906bf46bfc72b336a25816da84a1f97b3f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.1 MB (27118958 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6e41e625833706e636d407ac328f8f6f0a458c3665c50e921be02c2246900373`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 24 Feb 2021 20:50:45 GMT
ADD file:72743cfd9913f13553e700f9d9cfdc17b9dc793ebeeb337fd5fe02dc962d4b63 in / 
# Wed, 24 Feb 2021 20:50:46 GMT
CMD ["/bin/sh"]
# Wed, 24 Feb 2021 23:33:31 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 24 Feb 2021 23:33:37 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.4.5/traefik_v2.4.5_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Wed, 24 Feb 2021 23:33:39 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 24 Feb 2021 23:33:39 GMT
EXPOSE 80
# Wed, 24 Feb 2021 23:33:40 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 24 Feb 2021 23:33:41 GMT
CMD ["traefik"]
# Wed, 24 Feb 2021 23:33:41 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.4.5 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:72e8de7d15c4484a563097a94cbab858afe450985c4b372f94b522b5ea1d8fa6`  
		Last Modified: Wed, 24 Feb 2021 23:35:25 GMT  
		Size: 23.8 MB (23820517 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f48c4b827d0213635a8cc7951840f4390b222dc4556e5e471dfc6f190f71dce`  
		Last Modified: Wed, 24 Feb 2021 23:35:10 GMT  
		Size: 367.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:latest` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:d192f9f1bbd0e0e799b36f3e923cf4c541d53dfb3af4de5a7ca07f0c666b0c75
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.7 MB (26732718 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f46bc576d13c9ed7dd38a1615fa6e697520634a83a48d35cf19449f180e6a518`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 16 Dec 2020 23:40:37 GMT
ADD file:47bb1b85a4eb4d0b355ae89ec5c71c09e2c2b7e21e1851a2896365eb17134f57 in / 
# Wed, 16 Dec 2020 23:40:39 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 00:27:02 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 18 Feb 2021 19:42:27 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.4.5/traefik_v2.4.5_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 18 Feb 2021 19:42:28 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 18 Feb 2021 19:42:29 GMT
EXPOSE 80
# Thu, 18 Feb 2021 19:42:29 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 18 Feb 2021 19:42:30 GMT
CMD ["traefik"]
# Thu, 18 Feb 2021 19:42:31 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.4.5 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:0cde3dd4acbae4754ea88e0519144e399c757804c4e7cd6c7b981b1c424e9d2e`  
		Last Modified: Thu, 18 Feb 2021 19:43:06 GMT  
		Size: 23.3 MB (23333888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fe295f200a4508af4e26b28b5716ee3afb0cc15b6c8a5472fc9e473e0c02fe1`  
		Last Modified: Thu, 18 Feb 2021 19:42:59 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:livarot`

```console
$ docker pull traefik@sha256:4d303938bde19f213ab9888fe48c42138d4ad8392cdd4bc52b5f3f2d226b9c24
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:livarot` - linux; amd64

```console
$ docker pull traefik@sha256:2cec9f638bf256272fc3b7df23f72e84edcbab613aa7aa66c96ff67c90885164
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.1 MB (29068973 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:66c68650f9a1d2203914c7437252596c135158de12607225d9c62c332d6932d6`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 17 Dec 2020 00:19:49 GMT
ADD file:8ed80010e443da19d72546bcee9a35e0a8d244c72052b1994610bf5939d479c2 in / 
# Thu, 17 Dec 2020 00:19:49 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 00:47:33 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 18 Feb 2021 19:21:01 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.4.5/traefik_v2.4.5_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 18 Feb 2021 19:21:01 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 18 Feb 2021 19:21:01 GMT
EXPOSE 80
# Thu, 18 Feb 2021 19:21:01 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 18 Feb 2021 19:21:02 GMT
CMD ["traefik"]
# Thu, 18 Feb 2021 19:21:02 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.4.5 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:7a43eed822408ece4014703bda46018fc52ffc73fe801e045f6ff8dcc67c71c4`  
		Last Modified: Thu, 18 Feb 2021 19:21:30 GMT  
		Size: 25.6 MB (25582044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0383ad4de15380b230a3391b092c22a7efa30b126f7033acdfaa91180dca7e9`  
		Last Modified: Thu, 18 Feb 2021 19:21:26 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:livarot` - linux; arm variant v6

```console
$ docker pull traefik@sha256:51e6acb6b11a005142df938a5c8364906bf46bfc72b336a25816da84a1f97b3f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.1 MB (27118958 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6e41e625833706e636d407ac328f8f6f0a458c3665c50e921be02c2246900373`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 24 Feb 2021 20:50:45 GMT
ADD file:72743cfd9913f13553e700f9d9cfdc17b9dc793ebeeb337fd5fe02dc962d4b63 in / 
# Wed, 24 Feb 2021 20:50:46 GMT
CMD ["/bin/sh"]
# Wed, 24 Feb 2021 23:33:31 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 24 Feb 2021 23:33:37 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.4.5/traefik_v2.4.5_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Wed, 24 Feb 2021 23:33:39 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 24 Feb 2021 23:33:39 GMT
EXPOSE 80
# Wed, 24 Feb 2021 23:33:40 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 24 Feb 2021 23:33:41 GMT
CMD ["traefik"]
# Wed, 24 Feb 2021 23:33:41 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.4.5 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:72e8de7d15c4484a563097a94cbab858afe450985c4b372f94b522b5ea1d8fa6`  
		Last Modified: Wed, 24 Feb 2021 23:35:25 GMT  
		Size: 23.8 MB (23820517 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f48c4b827d0213635a8cc7951840f4390b222dc4556e5e471dfc6f190f71dce`  
		Last Modified: Wed, 24 Feb 2021 23:35:10 GMT  
		Size: 367.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:livarot` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:d192f9f1bbd0e0e799b36f3e923cf4c541d53dfb3af4de5a7ca07f0c666b0c75
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.7 MB (26732718 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f46bc576d13c9ed7dd38a1615fa6e697520634a83a48d35cf19449f180e6a518`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 16 Dec 2020 23:40:37 GMT
ADD file:47bb1b85a4eb4d0b355ae89ec5c71c09e2c2b7e21e1851a2896365eb17134f57 in / 
# Wed, 16 Dec 2020 23:40:39 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 00:27:02 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 18 Feb 2021 19:42:27 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.4.5/traefik_v2.4.5_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 18 Feb 2021 19:42:28 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 18 Feb 2021 19:42:29 GMT
EXPOSE 80
# Thu, 18 Feb 2021 19:42:29 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 18 Feb 2021 19:42:30 GMT
CMD ["traefik"]
# Thu, 18 Feb 2021 19:42:31 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.4.5 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:0cde3dd4acbae4754ea88e0519144e399c757804c4e7cd6c7b981b1c424e9d2e`  
		Last Modified: Thu, 18 Feb 2021 19:43:06 GMT  
		Size: 23.3 MB (23333888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fe295f200a4508af4e26b28b5716ee3afb0cc15b6c8a5472fc9e473e0c02fe1`  
		Last Modified: Thu, 18 Feb 2021 19:42:59 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:livarot-windowsservercore-1809`

```console
$ docker pull traefik@sha256:56c556d77094bf8a496466fe0ec56ff819930ef465d252dd4887a68581bbf65b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1757; amd64

### `traefik:livarot-windowsservercore-1809` - windows version 10.0.17763.1757; amd64

```console
$ docker pull traefik@sha256:dccfae71811f7f07f664e6e60cb651ecdb00d1cb0754b7d7e920eaa494718111
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2474658912 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:678cdb23a8e3694a9f36cc33974dfcf56d9d68726c676dfdb05fcdc0ceca6dd1`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 06 Feb 2021 05:03:14 GMT
RUN Install update 1809-amd64
# Wed, 10 Feb 2021 13:14:02 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 18 Feb 2021 19:16:05 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/traefik/traefik/releases/download/v2.4.5/traefik_v2.4.5_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Thu, 18 Feb 2021 19:16:07 GMT
EXPOSE 80
# Thu, 18 Feb 2021 19:16:08 GMT
ENTRYPOINT ["/traefik"]
# Thu, 18 Feb 2021 19:16:10 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.4.5 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:db4edcf0861ff3fdc41851a5a218965ecb2ab6cf4ec9448fb80cc4b6792fd46c`  
		Size: 720.9 MB (720933935 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:433d24156d44dde3b3c6c0094ba5824a315286ae537c68f272e464fc426510f6`  
		Last Modified: Wed, 10 Feb 2021 13:40:44 GMT  
		Size: 1.4 KB (1362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1f6a9a190cd76e08337bdbcb4151e2209a8eb869350410b69abc00520909b49`  
		Last Modified: Thu, 18 Feb 2021 19:16:58 GMT  
		Size: 35.4 MB (35386459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3842dc9cd16d601823a69250f2125c318e7c55f63a7a247d9359f2ffe84a662`  
		Last Modified: Thu, 18 Feb 2021 19:16:50 GMT  
		Size: 1.4 KB (1444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dba0a130b3c525c6d7cdd4a3661e9ceaa11bb9287f0823bf8220028c6878d78d`  
		Last Modified: Thu, 18 Feb 2021 19:16:49 GMT  
		Size: 1.4 KB (1402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9924892ced120ed01c98e4f2489c0d44fa78f5258239f969a9910a81ef17c234`  
		Last Modified: Thu, 18 Feb 2021 19:16:49 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:maroilles`

```console
$ docker pull traefik@sha256:5325e0f4d374b9fd87550465b3145415c24ce90d56f839632e56875ce4072844
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
$ docker pull traefik@sha256:aaf51dc5d08b6aa95894d72fa53f587b3093d4b3cc9626ef42c17d5df630db76
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
$ docker pull traefik@sha256:4b4a41ca1cdc6e1b98793fcd9ba92b1a561c16eddf9c30aa2815feab850205b4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1757; amd64

### `traefik:maroilles-windowsservercore-1809` - windows version 10.0.17763.1757; amd64

```console
$ docker pull traefik@sha256:697e5dbefbd4bcaef22f89382f30639ed29a3292fdd188cf807bb71546eabeb4
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2469803792 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e71a612ec4fa6c6b261321c8fe09e059ee040cb04218657389bac3c9ce002eed`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 06 Feb 2021 05:03:14 GMT
RUN Install update 1809-amd64
# Wed, 10 Feb 2021 13:14:02 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Feb 2021 20:10:24 GMT
RUN Invoke-WebRequest     -Uri "https://github.com/traefik/traefik/releases/download/v1.7.28/traefik_windows-amd64.exe"     -OutFile "/traefik.exe"
# Wed, 10 Feb 2021 20:10:25 GMT
EXPOSE 80
# Wed, 10 Feb 2021 20:10:26 GMT
ENTRYPOINT ["/traefik"]
# Wed, 10 Feb 2021 20:10:27 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.28 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:db4edcf0861ff3fdc41851a5a218965ecb2ab6cf4ec9448fb80cc4b6792fd46c`  
		Size: 720.9 MB (720933935 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:433d24156d44dde3b3c6c0094ba5824a315286ae537c68f272e464fc426510f6`  
		Last Modified: Wed, 10 Feb 2021 13:40:44 GMT  
		Size: 1.4 KB (1362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:639352e9914386a0227a0fbdfe068f0eecb8206eeb528ebbb1006dc69f155ae8`  
		Last Modified: Wed, 10 Feb 2021 20:11:58 GMT  
		Size: 30.5 MB (30531541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:875bd0eab58c3c0eb449d5641c8d341956ca8df8e79a9960d1b9176d28b7f872`  
		Last Modified: Wed, 10 Feb 2021 20:11:51 GMT  
		Size: 1.3 KB (1349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b14f079b8ee9624c2313d782b2d9a04723215c063eca353822eafbf3ee0a2b59`  
		Last Modified: Wed, 10 Feb 2021 20:11:51 GMT  
		Size: 1.4 KB (1390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3063b85a538300feec077a4ebd3b11960a83a55adb2de40370e013212cfe2e6`  
		Last Modified: Wed, 10 Feb 2021 20:11:51 GMT  
		Size: 1.3 KB (1336 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v1.7`

```console
$ docker pull traefik@sha256:5325e0f4d374b9fd87550465b3145415c24ce90d56f839632e56875ce4072844
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
$ docker pull traefik@sha256:5325e0f4d374b9fd87550465b3145415c24ce90d56f839632e56875ce4072844
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
$ docker pull traefik@sha256:aaf51dc5d08b6aa95894d72fa53f587b3093d4b3cc9626ef42c17d5df630db76
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
$ docker pull traefik@sha256:4b4a41ca1cdc6e1b98793fcd9ba92b1a561c16eddf9c30aa2815feab850205b4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1757; amd64

### `traefik:v1.7.28-windowsservercore-1809` - windows version 10.0.17763.1757; amd64

```console
$ docker pull traefik@sha256:697e5dbefbd4bcaef22f89382f30639ed29a3292fdd188cf807bb71546eabeb4
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2469803792 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e71a612ec4fa6c6b261321c8fe09e059ee040cb04218657389bac3c9ce002eed`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 06 Feb 2021 05:03:14 GMT
RUN Install update 1809-amd64
# Wed, 10 Feb 2021 13:14:02 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Feb 2021 20:10:24 GMT
RUN Invoke-WebRequest     -Uri "https://github.com/traefik/traefik/releases/download/v1.7.28/traefik_windows-amd64.exe"     -OutFile "/traefik.exe"
# Wed, 10 Feb 2021 20:10:25 GMT
EXPOSE 80
# Wed, 10 Feb 2021 20:10:26 GMT
ENTRYPOINT ["/traefik"]
# Wed, 10 Feb 2021 20:10:27 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.28 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:db4edcf0861ff3fdc41851a5a218965ecb2ab6cf4ec9448fb80cc4b6792fd46c`  
		Size: 720.9 MB (720933935 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:433d24156d44dde3b3c6c0094ba5824a315286ae537c68f272e464fc426510f6`  
		Last Modified: Wed, 10 Feb 2021 13:40:44 GMT  
		Size: 1.4 KB (1362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:639352e9914386a0227a0fbdfe068f0eecb8206eeb528ebbb1006dc69f155ae8`  
		Last Modified: Wed, 10 Feb 2021 20:11:58 GMT  
		Size: 30.5 MB (30531541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:875bd0eab58c3c0eb449d5641c8d341956ca8df8e79a9960d1b9176d28b7f872`  
		Last Modified: Wed, 10 Feb 2021 20:11:51 GMT  
		Size: 1.3 KB (1349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b14f079b8ee9624c2313d782b2d9a04723215c063eca353822eafbf3ee0a2b59`  
		Last Modified: Wed, 10 Feb 2021 20:11:51 GMT  
		Size: 1.4 KB (1390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3063b85a538300feec077a4ebd3b11960a83a55adb2de40370e013212cfe2e6`  
		Last Modified: Wed, 10 Feb 2021 20:11:51 GMT  
		Size: 1.3 KB (1336 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v1.7-alpine`

```console
$ docker pull traefik@sha256:aaf51dc5d08b6aa95894d72fa53f587b3093d4b3cc9626ef42c17d5df630db76
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
$ docker pull traefik@sha256:4b4a41ca1cdc6e1b98793fcd9ba92b1a561c16eddf9c30aa2815feab850205b4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1757; amd64

### `traefik:v1.7-windowsservercore-1809` - windows version 10.0.17763.1757; amd64

```console
$ docker pull traefik@sha256:697e5dbefbd4bcaef22f89382f30639ed29a3292fdd188cf807bb71546eabeb4
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2469803792 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e71a612ec4fa6c6b261321c8fe09e059ee040cb04218657389bac3c9ce002eed`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 06 Feb 2021 05:03:14 GMT
RUN Install update 1809-amd64
# Wed, 10 Feb 2021 13:14:02 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Feb 2021 20:10:24 GMT
RUN Invoke-WebRequest     -Uri "https://github.com/traefik/traefik/releases/download/v1.7.28/traefik_windows-amd64.exe"     -OutFile "/traefik.exe"
# Wed, 10 Feb 2021 20:10:25 GMT
EXPOSE 80
# Wed, 10 Feb 2021 20:10:26 GMT
ENTRYPOINT ["/traefik"]
# Wed, 10 Feb 2021 20:10:27 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.28 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:db4edcf0861ff3fdc41851a5a218965ecb2ab6cf4ec9448fb80cc4b6792fd46c`  
		Size: 720.9 MB (720933935 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:433d24156d44dde3b3c6c0094ba5824a315286ae537c68f272e464fc426510f6`  
		Last Modified: Wed, 10 Feb 2021 13:40:44 GMT  
		Size: 1.4 KB (1362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:639352e9914386a0227a0fbdfe068f0eecb8206eeb528ebbb1006dc69f155ae8`  
		Last Modified: Wed, 10 Feb 2021 20:11:58 GMT  
		Size: 30.5 MB (30531541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:875bd0eab58c3c0eb449d5641c8d341956ca8df8e79a9960d1b9176d28b7f872`  
		Last Modified: Wed, 10 Feb 2021 20:11:51 GMT  
		Size: 1.3 KB (1349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b14f079b8ee9624c2313d782b2d9a04723215c063eca353822eafbf3ee0a2b59`  
		Last Modified: Wed, 10 Feb 2021 20:11:51 GMT  
		Size: 1.4 KB (1390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3063b85a538300feec077a4ebd3b11960a83a55adb2de40370e013212cfe2e6`  
		Last Modified: Wed, 10 Feb 2021 20:11:51 GMT  
		Size: 1.3 KB (1336 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v2.4`

```console
$ docker pull traefik@sha256:4d303938bde19f213ab9888fe48c42138d4ad8392cdd4bc52b5f3f2d226b9c24
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:v2.4` - linux; amd64

```console
$ docker pull traefik@sha256:2cec9f638bf256272fc3b7df23f72e84edcbab613aa7aa66c96ff67c90885164
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.1 MB (29068973 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:66c68650f9a1d2203914c7437252596c135158de12607225d9c62c332d6932d6`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 17 Dec 2020 00:19:49 GMT
ADD file:8ed80010e443da19d72546bcee9a35e0a8d244c72052b1994610bf5939d479c2 in / 
# Thu, 17 Dec 2020 00:19:49 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 00:47:33 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 18 Feb 2021 19:21:01 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.4.5/traefik_v2.4.5_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 18 Feb 2021 19:21:01 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 18 Feb 2021 19:21:01 GMT
EXPOSE 80
# Thu, 18 Feb 2021 19:21:01 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 18 Feb 2021 19:21:02 GMT
CMD ["traefik"]
# Thu, 18 Feb 2021 19:21:02 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.4.5 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:7a43eed822408ece4014703bda46018fc52ffc73fe801e045f6ff8dcc67c71c4`  
		Last Modified: Thu, 18 Feb 2021 19:21:30 GMT  
		Size: 25.6 MB (25582044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0383ad4de15380b230a3391b092c22a7efa30b126f7033acdfaa91180dca7e9`  
		Last Modified: Thu, 18 Feb 2021 19:21:26 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v2.4` - linux; arm variant v6

```console
$ docker pull traefik@sha256:51e6acb6b11a005142df938a5c8364906bf46bfc72b336a25816da84a1f97b3f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.1 MB (27118958 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6e41e625833706e636d407ac328f8f6f0a458c3665c50e921be02c2246900373`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 24 Feb 2021 20:50:45 GMT
ADD file:72743cfd9913f13553e700f9d9cfdc17b9dc793ebeeb337fd5fe02dc962d4b63 in / 
# Wed, 24 Feb 2021 20:50:46 GMT
CMD ["/bin/sh"]
# Wed, 24 Feb 2021 23:33:31 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 24 Feb 2021 23:33:37 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.4.5/traefik_v2.4.5_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Wed, 24 Feb 2021 23:33:39 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 24 Feb 2021 23:33:39 GMT
EXPOSE 80
# Wed, 24 Feb 2021 23:33:40 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 24 Feb 2021 23:33:41 GMT
CMD ["traefik"]
# Wed, 24 Feb 2021 23:33:41 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.4.5 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:72e8de7d15c4484a563097a94cbab858afe450985c4b372f94b522b5ea1d8fa6`  
		Last Modified: Wed, 24 Feb 2021 23:35:25 GMT  
		Size: 23.8 MB (23820517 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f48c4b827d0213635a8cc7951840f4390b222dc4556e5e471dfc6f190f71dce`  
		Last Modified: Wed, 24 Feb 2021 23:35:10 GMT  
		Size: 367.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v2.4` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:d192f9f1bbd0e0e799b36f3e923cf4c541d53dfb3af4de5a7ca07f0c666b0c75
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.7 MB (26732718 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f46bc576d13c9ed7dd38a1615fa6e697520634a83a48d35cf19449f180e6a518`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 16 Dec 2020 23:40:37 GMT
ADD file:47bb1b85a4eb4d0b355ae89ec5c71c09e2c2b7e21e1851a2896365eb17134f57 in / 
# Wed, 16 Dec 2020 23:40:39 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 00:27:02 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 18 Feb 2021 19:42:27 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.4.5/traefik_v2.4.5_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 18 Feb 2021 19:42:28 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 18 Feb 2021 19:42:29 GMT
EXPOSE 80
# Thu, 18 Feb 2021 19:42:29 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 18 Feb 2021 19:42:30 GMT
CMD ["traefik"]
# Thu, 18 Feb 2021 19:42:31 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.4.5 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:0cde3dd4acbae4754ea88e0519144e399c757804c4e7cd6c7b981b1c424e9d2e`  
		Last Modified: Thu, 18 Feb 2021 19:43:06 GMT  
		Size: 23.3 MB (23333888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fe295f200a4508af4e26b28b5716ee3afb0cc15b6c8a5472fc9e473e0c02fe1`  
		Last Modified: Thu, 18 Feb 2021 19:42:59 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v2.4.5`

```console
$ docker pull traefik@sha256:4d303938bde19f213ab9888fe48c42138d4ad8392cdd4bc52b5f3f2d226b9c24
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:v2.4.5` - linux; amd64

```console
$ docker pull traefik@sha256:2cec9f638bf256272fc3b7df23f72e84edcbab613aa7aa66c96ff67c90885164
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.1 MB (29068973 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:66c68650f9a1d2203914c7437252596c135158de12607225d9c62c332d6932d6`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 17 Dec 2020 00:19:49 GMT
ADD file:8ed80010e443da19d72546bcee9a35e0a8d244c72052b1994610bf5939d479c2 in / 
# Thu, 17 Dec 2020 00:19:49 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 00:47:33 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 18 Feb 2021 19:21:01 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.4.5/traefik_v2.4.5_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 18 Feb 2021 19:21:01 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 18 Feb 2021 19:21:01 GMT
EXPOSE 80
# Thu, 18 Feb 2021 19:21:01 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 18 Feb 2021 19:21:02 GMT
CMD ["traefik"]
# Thu, 18 Feb 2021 19:21:02 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.4.5 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:7a43eed822408ece4014703bda46018fc52ffc73fe801e045f6ff8dcc67c71c4`  
		Last Modified: Thu, 18 Feb 2021 19:21:30 GMT  
		Size: 25.6 MB (25582044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0383ad4de15380b230a3391b092c22a7efa30b126f7033acdfaa91180dca7e9`  
		Last Modified: Thu, 18 Feb 2021 19:21:26 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v2.4.5` - linux; arm variant v6

```console
$ docker pull traefik@sha256:51e6acb6b11a005142df938a5c8364906bf46bfc72b336a25816da84a1f97b3f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.1 MB (27118958 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6e41e625833706e636d407ac328f8f6f0a458c3665c50e921be02c2246900373`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 24 Feb 2021 20:50:45 GMT
ADD file:72743cfd9913f13553e700f9d9cfdc17b9dc793ebeeb337fd5fe02dc962d4b63 in / 
# Wed, 24 Feb 2021 20:50:46 GMT
CMD ["/bin/sh"]
# Wed, 24 Feb 2021 23:33:31 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 24 Feb 2021 23:33:37 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.4.5/traefik_v2.4.5_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Wed, 24 Feb 2021 23:33:39 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 24 Feb 2021 23:33:39 GMT
EXPOSE 80
# Wed, 24 Feb 2021 23:33:40 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 24 Feb 2021 23:33:41 GMT
CMD ["traefik"]
# Wed, 24 Feb 2021 23:33:41 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.4.5 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:72e8de7d15c4484a563097a94cbab858afe450985c4b372f94b522b5ea1d8fa6`  
		Last Modified: Wed, 24 Feb 2021 23:35:25 GMT  
		Size: 23.8 MB (23820517 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f48c4b827d0213635a8cc7951840f4390b222dc4556e5e471dfc6f190f71dce`  
		Last Modified: Wed, 24 Feb 2021 23:35:10 GMT  
		Size: 367.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v2.4.5` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:d192f9f1bbd0e0e799b36f3e923cf4c541d53dfb3af4de5a7ca07f0c666b0c75
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.7 MB (26732718 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f46bc576d13c9ed7dd38a1615fa6e697520634a83a48d35cf19449f180e6a518`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 16 Dec 2020 23:40:37 GMT
ADD file:47bb1b85a4eb4d0b355ae89ec5c71c09e2c2b7e21e1851a2896365eb17134f57 in / 
# Wed, 16 Dec 2020 23:40:39 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 00:27:02 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 18 Feb 2021 19:42:27 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.4.5/traefik_v2.4.5_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 18 Feb 2021 19:42:28 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 18 Feb 2021 19:42:29 GMT
EXPOSE 80
# Thu, 18 Feb 2021 19:42:29 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 18 Feb 2021 19:42:30 GMT
CMD ["traefik"]
# Thu, 18 Feb 2021 19:42:31 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.4.5 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:0cde3dd4acbae4754ea88e0519144e399c757804c4e7cd6c7b981b1c424e9d2e`  
		Last Modified: Thu, 18 Feb 2021 19:43:06 GMT  
		Size: 23.3 MB (23333888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fe295f200a4508af4e26b28b5716ee3afb0cc15b6c8a5472fc9e473e0c02fe1`  
		Last Modified: Thu, 18 Feb 2021 19:42:59 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v2.4.5-windowsservercore-1809`

```console
$ docker pull traefik@sha256:56c556d77094bf8a496466fe0ec56ff819930ef465d252dd4887a68581bbf65b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1757; amd64

### `traefik:v2.4.5-windowsservercore-1809` - windows version 10.0.17763.1757; amd64

```console
$ docker pull traefik@sha256:dccfae71811f7f07f664e6e60cb651ecdb00d1cb0754b7d7e920eaa494718111
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2474658912 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:678cdb23a8e3694a9f36cc33974dfcf56d9d68726c676dfdb05fcdc0ceca6dd1`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 06 Feb 2021 05:03:14 GMT
RUN Install update 1809-amd64
# Wed, 10 Feb 2021 13:14:02 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 18 Feb 2021 19:16:05 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/traefik/traefik/releases/download/v2.4.5/traefik_v2.4.5_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Thu, 18 Feb 2021 19:16:07 GMT
EXPOSE 80
# Thu, 18 Feb 2021 19:16:08 GMT
ENTRYPOINT ["/traefik"]
# Thu, 18 Feb 2021 19:16:10 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.4.5 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:db4edcf0861ff3fdc41851a5a218965ecb2ab6cf4ec9448fb80cc4b6792fd46c`  
		Size: 720.9 MB (720933935 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:433d24156d44dde3b3c6c0094ba5824a315286ae537c68f272e464fc426510f6`  
		Last Modified: Wed, 10 Feb 2021 13:40:44 GMT  
		Size: 1.4 KB (1362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1f6a9a190cd76e08337bdbcb4151e2209a8eb869350410b69abc00520909b49`  
		Last Modified: Thu, 18 Feb 2021 19:16:58 GMT  
		Size: 35.4 MB (35386459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3842dc9cd16d601823a69250f2125c318e7c55f63a7a247d9359f2ffe84a662`  
		Last Modified: Thu, 18 Feb 2021 19:16:50 GMT  
		Size: 1.4 KB (1444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dba0a130b3c525c6d7cdd4a3661e9ceaa11bb9287f0823bf8220028c6878d78d`  
		Last Modified: Thu, 18 Feb 2021 19:16:49 GMT  
		Size: 1.4 KB (1402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9924892ced120ed01c98e4f2489c0d44fa78f5258239f969a9910a81ef17c234`  
		Last Modified: Thu, 18 Feb 2021 19:16:49 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v2.4-windowsservercore-1809`

```console
$ docker pull traefik@sha256:56c556d77094bf8a496466fe0ec56ff819930ef465d252dd4887a68581bbf65b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1757; amd64

### `traefik:v2.4-windowsservercore-1809` - windows version 10.0.17763.1757; amd64

```console
$ docker pull traefik@sha256:dccfae71811f7f07f664e6e60cb651ecdb00d1cb0754b7d7e920eaa494718111
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2474658912 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:678cdb23a8e3694a9f36cc33974dfcf56d9d68726c676dfdb05fcdc0ceca6dd1`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 06 Feb 2021 05:03:14 GMT
RUN Install update 1809-amd64
# Wed, 10 Feb 2021 13:14:02 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 18 Feb 2021 19:16:05 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/traefik/traefik/releases/download/v2.4.5/traefik_v2.4.5_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Thu, 18 Feb 2021 19:16:07 GMT
EXPOSE 80
# Thu, 18 Feb 2021 19:16:08 GMT
ENTRYPOINT ["/traefik"]
# Thu, 18 Feb 2021 19:16:10 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.4.5 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:db4edcf0861ff3fdc41851a5a218965ecb2ab6cf4ec9448fb80cc4b6792fd46c`  
		Size: 720.9 MB (720933935 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:433d24156d44dde3b3c6c0094ba5824a315286ae537c68f272e464fc426510f6`  
		Last Modified: Wed, 10 Feb 2021 13:40:44 GMT  
		Size: 1.4 KB (1362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1f6a9a190cd76e08337bdbcb4151e2209a8eb869350410b69abc00520909b49`  
		Last Modified: Thu, 18 Feb 2021 19:16:58 GMT  
		Size: 35.4 MB (35386459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3842dc9cd16d601823a69250f2125c318e7c55f63a7a247d9359f2ffe84a662`  
		Last Modified: Thu, 18 Feb 2021 19:16:50 GMT  
		Size: 1.4 KB (1444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dba0a130b3c525c6d7cdd4a3661e9ceaa11bb9287f0823bf8220028c6878d78d`  
		Last Modified: Thu, 18 Feb 2021 19:16:49 GMT  
		Size: 1.4 KB (1402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9924892ced120ed01c98e4f2489c0d44fa78f5258239f969a9910a81ef17c234`  
		Last Modified: Thu, 18 Feb 2021 19:16:49 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:windowsservercore-1809`

```console
$ docker pull traefik@sha256:56c556d77094bf8a496466fe0ec56ff819930ef465d252dd4887a68581bbf65b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1757; amd64

### `traefik:windowsservercore-1809` - windows version 10.0.17763.1757; amd64

```console
$ docker pull traefik@sha256:dccfae71811f7f07f664e6e60cb651ecdb00d1cb0754b7d7e920eaa494718111
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2474658912 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:678cdb23a8e3694a9f36cc33974dfcf56d9d68726c676dfdb05fcdc0ceca6dd1`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 06 Feb 2021 05:03:14 GMT
RUN Install update 1809-amd64
# Wed, 10 Feb 2021 13:14:02 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 18 Feb 2021 19:16:05 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/traefik/traefik/releases/download/v2.4.5/traefik_v2.4.5_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Thu, 18 Feb 2021 19:16:07 GMT
EXPOSE 80
# Thu, 18 Feb 2021 19:16:08 GMT
ENTRYPOINT ["/traefik"]
# Thu, 18 Feb 2021 19:16:10 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.4.5 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:db4edcf0861ff3fdc41851a5a218965ecb2ab6cf4ec9448fb80cc4b6792fd46c`  
		Size: 720.9 MB (720933935 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:433d24156d44dde3b3c6c0094ba5824a315286ae537c68f272e464fc426510f6`  
		Last Modified: Wed, 10 Feb 2021 13:40:44 GMT  
		Size: 1.4 KB (1362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1f6a9a190cd76e08337bdbcb4151e2209a8eb869350410b69abc00520909b49`  
		Last Modified: Thu, 18 Feb 2021 19:16:58 GMT  
		Size: 35.4 MB (35386459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3842dc9cd16d601823a69250f2125c318e7c55f63a7a247d9359f2ffe84a662`  
		Last Modified: Thu, 18 Feb 2021 19:16:50 GMT  
		Size: 1.4 KB (1444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dba0a130b3c525c6d7cdd4a3661e9ceaa11bb9287f0823bf8220028c6878d78d`  
		Last Modified: Thu, 18 Feb 2021 19:16:49 GMT  
		Size: 1.4 KB (1402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9924892ced120ed01c98e4f2489c0d44fa78f5258239f969a9910a81ef17c234`  
		Last Modified: Thu, 18 Feb 2021 19:16:49 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
