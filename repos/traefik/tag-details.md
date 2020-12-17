<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `traefik`

-	[`traefik:1.7`](#traefik17)
-	[`traefik:1.7.26`](#traefik1726)
-	[`traefik:1.7.26-alpine`](#traefik1726-alpine)
-	[`traefik:1.7.26-windowsservercore-1809`](#traefik1726-windowsservercore-1809)
-	[`traefik:1.7-alpine`](#traefik17-alpine)
-	[`traefik:1.7-windowsservercore-1809`](#traefik17-windowsservercore-1809)
-	[`traefik:2.3`](#traefik23)
-	[`traefik:2.3.6`](#traefik236)
-	[`traefik:2.3.6-windowsservercore-1809`](#traefik236-windowsservercore-1809)
-	[`traefik:2.3-windowsservercore-1809`](#traefik23-windowsservercore-1809)
-	[`traefik:2.4`](#traefik24)
-	[`traefik:2.4.0-rc1`](#traefik240-rc1)
-	[`traefik:2.4.0-rc1-windowsservercore-1809`](#traefik240-rc1-windowsservercore-1809)
-	[`traefik:2.4-windowsservercore-1809`](#traefik24-windowsservercore-1809)
-	[`traefik:latest`](#traefiklatest)
-	[`traefik:livarot`](#traefiklivarot)
-	[`traefik:livarot-windowsservercore-1809`](#traefiklivarot-windowsservercore-1809)
-	[`traefik:maroilles`](#traefikmaroilles)
-	[`traefik:maroilles-alpine`](#traefikmaroilles-alpine)
-	[`traefik:maroilles-windowsservercore-1809`](#traefikmaroilles-windowsservercore-1809)
-	[`traefik:picodon`](#traefikpicodon)
-	[`traefik:picodon-windowsservercore-1809`](#traefikpicodon-windowsservercore-1809)
-	[`traefik:v1.7`](#traefikv17)
-	[`traefik:v1.7.26`](#traefikv1726)
-	[`traefik:v1.7.26-alpine`](#traefikv1726-alpine)
-	[`traefik:v1.7.26-windowsservercore-1809`](#traefikv1726-windowsservercore-1809)
-	[`traefik:v1.7-alpine`](#traefikv17-alpine)
-	[`traefik:v1.7-windowsservercore-1809`](#traefikv17-windowsservercore-1809)
-	[`traefik:v2.3`](#traefikv23)
-	[`traefik:v2.3.6`](#traefikv236)
-	[`traefik:v2.3.6-windowsservercore-1809`](#traefikv236-windowsservercore-1809)
-	[`traefik:v2.3-windowsservercore-1809`](#traefikv23-windowsservercore-1809)
-	[`traefik:v2.4`](#traefikv24)
-	[`traefik:v2.4.0-rc1`](#traefikv240-rc1)
-	[`traefik:v2.4.0-rc1-windowsservercore-1809`](#traefikv240-rc1-windowsservercore-1809)
-	[`traefik:v2.4-windowsservercore-1809`](#traefikv24-windowsservercore-1809)
-	[`traefik:windowsservercore-1809`](#traefikwindowsservercore-1809)

## `traefik:1.7`

```console
$ docker pull traefik@sha256:9a53d5dff2c5b474a8560a4af129cc7863fb8932f8bd0e6896f4292445a2bf86
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:1.7` - linux; amd64

```console
$ docker pull traefik@sha256:78a0311203a68b2a9173d8e19b42fc39e5f02f17f1db03c1a06e3fa1c66f4dd7
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **21.6 MB (21563612 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:23b804da420476b5cbcc59bdd26e354e8fa44e4dfe20caf3ac84768dd143b5f2`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Thu, 17 Dec 2020 00:48:11 GMT
COPY file:cd6264d9a7514a8fbc3eb7b400566d36178794d2b757959812cc3abc6f13a97b in /etc/ssl/certs/ 
# Thu, 17 Dec 2020 00:48:11 GMT
COPY dir:83da415af0ff24b3b9d10f857aa8c724a3bc93523f3e047b827e7554fe1f9e08 in /usr/share/ 
# Thu, 17 Dec 2020 00:48:12 GMT
COPY file:8e3cf7c133ac957e81d3eb831160ad827bfde058f356d7ac234b8c5ae307e37a in / 
# Thu, 17 Dec 2020 00:48:12 GMT
EXPOSE 80
# Thu, 17 Dec 2020 00:48:13 GMT
VOLUME [/tmp]
# Thu, 17 Dec 2020 00:48:13 GMT
ENTRYPOINT ["/traefik"]
# Thu, 17 Dec 2020 00:48:13 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.26 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:eca797b3e2d2ac9c3925e07a34654011a4314302362ca0dfe8320d4425bf01f5`  
		Last Modified: Thu, 17 Dec 2020 00:49:22 GMT  
		Size: 21.1 MB (21126329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:1.7` - linux; arm variant v6

```console
$ docker pull traefik@sha256:bb041f9232284130c3646cd4f0d83e032b078ae88a9ab88ea46580df2ee0b991
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **20.2 MB (20210272 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4c618c098e7b6182b45a63ffa8f49bb1656407fb6b666da85775efb87264cf12`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Thu, 17 Dec 2020 00:26:47 GMT
COPY file:cd6264d9a7514a8fbc3eb7b400566d36178794d2b757959812cc3abc6f13a97b in /etc/ssl/certs/ 
# Thu, 17 Dec 2020 00:26:48 GMT
COPY dir:83da415af0ff24b3b9d10f857aa8c724a3bc93523f3e047b827e7554fe1f9e08 in /usr/share/ 
# Thu, 17 Dec 2020 00:26:52 GMT
COPY file:a02ffe991352ee1f8abb077135ea9d27557e8b364fb712a42ccb2865e08df3cc in / 
# Thu, 17 Dec 2020 00:26:53 GMT
EXPOSE 80
# Thu, 17 Dec 2020 00:26:54 GMT
VOLUME [/tmp]
# Thu, 17 Dec 2020 00:26:56 GMT
ENTRYPOINT ["/traefik"]
# Thu, 17 Dec 2020 00:26:57 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.26 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:decc75cc844d668e21a715048cd9c78f2804e625a910fe5568e174c89bd5d8ab`  
		Last Modified: Thu, 17 Dec 2020 00:28:49 GMT  
		Size: 19.8 MB (19772941 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:1.7` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:2dc4a89841d24667bf689a0386eed1525cfe92afd4847039d73204d17e8d77f6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **19.9 MB (19930321 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5993443e6d894e7f4a83e79f4ede7636a3c8b57e7dca57a2dac980bed5a48274`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Thu, 17 Dec 2020 00:27:56 GMT
COPY file:cd6264d9a7514a8fbc3eb7b400566d36178794d2b757959812cc3abc6f13a97b in /etc/ssl/certs/ 
# Thu, 17 Dec 2020 00:27:58 GMT
COPY dir:83da415af0ff24b3b9d10f857aa8c724a3bc93523f3e047b827e7554fe1f9e08 in /usr/share/ 
# Thu, 17 Dec 2020 00:27:59 GMT
COPY file:f592954af2951d1a2538b1945366cb995f49638c7ef8b561b6961e0f8023197a in / 
# Thu, 17 Dec 2020 00:28:00 GMT
EXPOSE 80
# Thu, 17 Dec 2020 00:28:01 GMT
VOLUME [/tmp]
# Thu, 17 Dec 2020 00:28:02 GMT
ENTRYPOINT ["/traefik"]
# Thu, 17 Dec 2020 00:28:03 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.26 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:eda38820bf6e08ea342d37563cf7e4c258c772d4a0576588e8a451209a4534b2`  
		Last Modified: Thu, 17 Dec 2020 00:30:01 GMT  
		Size: 19.5 MB (19492982 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:1.7.26`

```console
$ docker pull traefik@sha256:9a53d5dff2c5b474a8560a4af129cc7863fb8932f8bd0e6896f4292445a2bf86
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:1.7.26` - linux; amd64

```console
$ docker pull traefik@sha256:78a0311203a68b2a9173d8e19b42fc39e5f02f17f1db03c1a06e3fa1c66f4dd7
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **21.6 MB (21563612 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:23b804da420476b5cbcc59bdd26e354e8fa44e4dfe20caf3ac84768dd143b5f2`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Thu, 17 Dec 2020 00:48:11 GMT
COPY file:cd6264d9a7514a8fbc3eb7b400566d36178794d2b757959812cc3abc6f13a97b in /etc/ssl/certs/ 
# Thu, 17 Dec 2020 00:48:11 GMT
COPY dir:83da415af0ff24b3b9d10f857aa8c724a3bc93523f3e047b827e7554fe1f9e08 in /usr/share/ 
# Thu, 17 Dec 2020 00:48:12 GMT
COPY file:8e3cf7c133ac957e81d3eb831160ad827bfde058f356d7ac234b8c5ae307e37a in / 
# Thu, 17 Dec 2020 00:48:12 GMT
EXPOSE 80
# Thu, 17 Dec 2020 00:48:13 GMT
VOLUME [/tmp]
# Thu, 17 Dec 2020 00:48:13 GMT
ENTRYPOINT ["/traefik"]
# Thu, 17 Dec 2020 00:48:13 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.26 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:eca797b3e2d2ac9c3925e07a34654011a4314302362ca0dfe8320d4425bf01f5`  
		Last Modified: Thu, 17 Dec 2020 00:49:22 GMT  
		Size: 21.1 MB (21126329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:1.7.26` - linux; arm variant v6

```console
$ docker pull traefik@sha256:bb041f9232284130c3646cd4f0d83e032b078ae88a9ab88ea46580df2ee0b991
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **20.2 MB (20210272 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4c618c098e7b6182b45a63ffa8f49bb1656407fb6b666da85775efb87264cf12`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Thu, 17 Dec 2020 00:26:47 GMT
COPY file:cd6264d9a7514a8fbc3eb7b400566d36178794d2b757959812cc3abc6f13a97b in /etc/ssl/certs/ 
# Thu, 17 Dec 2020 00:26:48 GMT
COPY dir:83da415af0ff24b3b9d10f857aa8c724a3bc93523f3e047b827e7554fe1f9e08 in /usr/share/ 
# Thu, 17 Dec 2020 00:26:52 GMT
COPY file:a02ffe991352ee1f8abb077135ea9d27557e8b364fb712a42ccb2865e08df3cc in / 
# Thu, 17 Dec 2020 00:26:53 GMT
EXPOSE 80
# Thu, 17 Dec 2020 00:26:54 GMT
VOLUME [/tmp]
# Thu, 17 Dec 2020 00:26:56 GMT
ENTRYPOINT ["/traefik"]
# Thu, 17 Dec 2020 00:26:57 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.26 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:decc75cc844d668e21a715048cd9c78f2804e625a910fe5568e174c89bd5d8ab`  
		Last Modified: Thu, 17 Dec 2020 00:28:49 GMT  
		Size: 19.8 MB (19772941 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:1.7.26` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:2dc4a89841d24667bf689a0386eed1525cfe92afd4847039d73204d17e8d77f6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **19.9 MB (19930321 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5993443e6d894e7f4a83e79f4ede7636a3c8b57e7dca57a2dac980bed5a48274`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Thu, 17 Dec 2020 00:27:56 GMT
COPY file:cd6264d9a7514a8fbc3eb7b400566d36178794d2b757959812cc3abc6f13a97b in /etc/ssl/certs/ 
# Thu, 17 Dec 2020 00:27:58 GMT
COPY dir:83da415af0ff24b3b9d10f857aa8c724a3bc93523f3e047b827e7554fe1f9e08 in /usr/share/ 
# Thu, 17 Dec 2020 00:27:59 GMT
COPY file:f592954af2951d1a2538b1945366cb995f49638c7ef8b561b6961e0f8023197a in / 
# Thu, 17 Dec 2020 00:28:00 GMT
EXPOSE 80
# Thu, 17 Dec 2020 00:28:01 GMT
VOLUME [/tmp]
# Thu, 17 Dec 2020 00:28:02 GMT
ENTRYPOINT ["/traefik"]
# Thu, 17 Dec 2020 00:28:03 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.26 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:eda38820bf6e08ea342d37563cf7e4c258c772d4a0576588e8a451209a4534b2`  
		Last Modified: Thu, 17 Dec 2020 00:30:01 GMT  
		Size: 19.5 MB (19492982 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:1.7.26-alpine`

```console
$ docker pull traefik@sha256:07dce138fe44640f0c52b2f7f4fb2e92fb508ded8ae57f9a7e0fe8fdf6296673
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:1.7.26-alpine` - linux; amd64

```console
$ docker pull traefik@sha256:8759aaeb837cdbbe7d39771b1442b99b182fd9556d0dfa02a4b21d254e125f9e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **24.6 MB (24613437 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6ec9aa2ea8436603df821232711432fc2de244aa083c03e3a23e002cac95549d`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 17 Dec 2020 00:19:49 GMT
ADD file:8ed80010e443da19d72546bcee9a35e0a8d244c72052b1994610bf5939d479c2 in / 
# Thu, 17 Dec 2020 00:19:49 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 00:47:33 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 17 Dec 2020 00:47:52 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/containous/traefik/releases/download/v1.7.26/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Thu, 17 Dec 2020 00:47:52 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 17 Dec 2020 00:47:52 GMT
EXPOSE 80
# Thu, 17 Dec 2020 00:47:52 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 17 Dec 2020 00:47:52 GMT
CMD ["traefik"]
# Thu, 17 Dec 2020 00:47:53 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.26 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:2d44f2e7e74e6943c5aac9ce858b295c6f31e2a0c129a718429a4a99ac1bc23d`  
		Last Modified: Thu, 17 Dec 2020 00:49:08 GMT  
		Size: 21.1 MB (21126507 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ca74d371d4ade4d81c1a76a8c789abb59c301c9b73488bfc9d0b40d3003eddf`  
		Last Modified: Thu, 17 Dec 2020 00:49:05 GMT  
		Size: 369.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:1.7.26-alpine` - linux; arm variant v6

```console
$ docker pull traefik@sha256:0494095125ba05e297b154e0827115ae0618b70d40ccce4b1c496ce1666ce43d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.1 MB (23069021 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b6d3de75d11f16c38ae16a31868fe6680c4f4f196bcab0eab4ca1f85c3d9d6f0`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 16 Dec 2020 23:49:53 GMT
ADD file:e3a6f7566ee3c2ba61d27d801d3522e045a4be64a42f32ee52d933b68338d06f in / 
# Wed, 16 Dec 2020 23:49:55 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 00:25:55 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 17 Dec 2020 00:26:33 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/containous/traefik/releases/download/v1.7.26/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Thu, 17 Dec 2020 00:26:34 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 17 Dec 2020 00:26:35 GMT
EXPOSE 80
# Thu, 17 Dec 2020 00:26:36 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 17 Dec 2020 00:26:37 GMT
CMD ["traefik"]
# Thu, 17 Dec 2020 00:26:39 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.26 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:8bed822566f883c529e4423ed5efb201104f66147671cd72a5a80db2e5609dce`  
		Last Modified: Thu, 17 Dec 2020 00:28:20 GMT  
		Size: 19.8 MB (19772981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a46c867ecec8c478367249ed7ccc513e1c496aa5d628bd9950ed8ad87e604f4d`  
		Last Modified: Thu, 17 Dec 2020 00:28:14 GMT  
		Size: 369.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:1.7.26-alpine` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:91c6f4a7270971b010691e5a21e487ac6d85bfbb85b83237a02dfb5c82f35055
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **22.9 MB (22891964 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f3f47993d5e498f1e77ebd9467c190b17085ea5862b5fb1049ebbaf278fcd434`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 16 Dec 2020 23:40:37 GMT
ADD file:47bb1b85a4eb4d0b355ae89ec5c71c09e2c2b7e21e1851a2896365eb17134f57 in / 
# Wed, 16 Dec 2020 23:40:39 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 00:27:02 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 17 Dec 2020 00:27:42 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/containous/traefik/releases/download/v1.7.26/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Thu, 17 Dec 2020 00:27:43 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 17 Dec 2020 00:27:44 GMT
EXPOSE 80
# Thu, 17 Dec 2020 00:27:45 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 17 Dec 2020 00:27:46 GMT
CMD ["traefik"]
# Thu, 17 Dec 2020 00:27:47 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.26 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:6be00c7721dc4a904b3531bfb7878ea6761d57116b3730c05eac3cb31e726a7e`  
		Last Modified: Thu, 17 Dec 2020 00:29:37 GMT  
		Size: 19.5 MB (19493133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37d0080e4ada531446b01e45e014d2c9983281dc58b873e4162e1adb99b6f3ad`  
		Last Modified: Thu, 17 Dec 2020 00:29:20 GMT  
		Size: 369.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:1.7.26-windowsservercore-1809`

```console
$ docker pull traefik@sha256:2c85e3865465339ff28a47a1511b774491ef43ee5c10e9fce0eed4512dca8e84
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1637; amd64

### `traefik:1.7.26-windowsservercore-1809` - windows version 10.0.17763.1637; amd64

```console
$ docker pull traefik@sha256:ecf2dd6f2cebbfdae3bd25b7ba2a68fea62a623ad337bc401dbfbff0ff03f48f
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2421243323 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c7ae3b3576f87d9dba1f675160af62a993ec7e3a322ac90f9f258497a933fef0`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 04 Dec 2020 02:13:01 GMT
RUN Install update 1809-amd64
# Wed, 09 Dec 2020 13:30:16 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Dec 2020 23:59:07 GMT
RUN Invoke-WebRequest     -Uri "https://github.com/containous/traefik/releases/download/v1.7.26/traefik_windows-amd64.exe"     -OutFile "/traefik.exe"
# Wed, 09 Dec 2020 23:59:09 GMT
EXPOSE 80
# Wed, 09 Dec 2020 23:59:10 GMT
ENTRYPOINT ["/traefik"]
# Wed, 09 Dec 2020 23:59:11 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.26 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:aa4f58cd6da1aaf1a0b44d443bd88e7fbe5b0a6f193995a1a61d6bd63990f314`  
		Size: 672.5 MB (672541583 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a4372d14958dc8a7eaaace9e4774e7f1db524da5eb4474b5e46738848a3a61a5`  
		Last Modified: Wed, 09 Dec 2020 13:54:38 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34300192a929cc8734d3561486bbf20306f0ddf75c3d405112b40a535022d87e`  
		Last Modified: Thu, 10 Dec 2020 00:00:39 GMT  
		Size: 30.4 MB (30364288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bcea0e9edffb70e9148c20ab78ddd79ecb43d454593638a01c8900035a7dfc9`  
		Last Modified: Thu, 10 Dec 2020 00:00:05 GMT  
		Size: 1.1 KB (1132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a53d2ed509732587fa21d4aad5f1ef27c38a85b71e038e15079a978fa5d3114`  
		Last Modified: Thu, 10 Dec 2020 00:00:05 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4118d174807346b7e443506fd438961205a118f2e545f00d509b2a299a92cc06`  
		Last Modified: Thu, 10 Dec 2020 00:00:05 GMT  
		Size: 1.2 KB (1187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:1.7-alpine`

```console
$ docker pull traefik@sha256:07dce138fe44640f0c52b2f7f4fb2e92fb508ded8ae57f9a7e0fe8fdf6296673
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:1.7-alpine` - linux; amd64

```console
$ docker pull traefik@sha256:8759aaeb837cdbbe7d39771b1442b99b182fd9556d0dfa02a4b21d254e125f9e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **24.6 MB (24613437 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6ec9aa2ea8436603df821232711432fc2de244aa083c03e3a23e002cac95549d`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 17 Dec 2020 00:19:49 GMT
ADD file:8ed80010e443da19d72546bcee9a35e0a8d244c72052b1994610bf5939d479c2 in / 
# Thu, 17 Dec 2020 00:19:49 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 00:47:33 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 17 Dec 2020 00:47:52 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/containous/traefik/releases/download/v1.7.26/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Thu, 17 Dec 2020 00:47:52 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 17 Dec 2020 00:47:52 GMT
EXPOSE 80
# Thu, 17 Dec 2020 00:47:52 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 17 Dec 2020 00:47:52 GMT
CMD ["traefik"]
# Thu, 17 Dec 2020 00:47:53 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.26 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:2d44f2e7e74e6943c5aac9ce858b295c6f31e2a0c129a718429a4a99ac1bc23d`  
		Last Modified: Thu, 17 Dec 2020 00:49:08 GMT  
		Size: 21.1 MB (21126507 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ca74d371d4ade4d81c1a76a8c789abb59c301c9b73488bfc9d0b40d3003eddf`  
		Last Modified: Thu, 17 Dec 2020 00:49:05 GMT  
		Size: 369.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:1.7-alpine` - linux; arm variant v6

```console
$ docker pull traefik@sha256:0494095125ba05e297b154e0827115ae0618b70d40ccce4b1c496ce1666ce43d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.1 MB (23069021 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b6d3de75d11f16c38ae16a31868fe6680c4f4f196bcab0eab4ca1f85c3d9d6f0`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 16 Dec 2020 23:49:53 GMT
ADD file:e3a6f7566ee3c2ba61d27d801d3522e045a4be64a42f32ee52d933b68338d06f in / 
# Wed, 16 Dec 2020 23:49:55 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 00:25:55 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 17 Dec 2020 00:26:33 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/containous/traefik/releases/download/v1.7.26/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Thu, 17 Dec 2020 00:26:34 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 17 Dec 2020 00:26:35 GMT
EXPOSE 80
# Thu, 17 Dec 2020 00:26:36 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 17 Dec 2020 00:26:37 GMT
CMD ["traefik"]
# Thu, 17 Dec 2020 00:26:39 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.26 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:8bed822566f883c529e4423ed5efb201104f66147671cd72a5a80db2e5609dce`  
		Last Modified: Thu, 17 Dec 2020 00:28:20 GMT  
		Size: 19.8 MB (19772981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a46c867ecec8c478367249ed7ccc513e1c496aa5d628bd9950ed8ad87e604f4d`  
		Last Modified: Thu, 17 Dec 2020 00:28:14 GMT  
		Size: 369.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:1.7-alpine` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:91c6f4a7270971b010691e5a21e487ac6d85bfbb85b83237a02dfb5c82f35055
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **22.9 MB (22891964 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f3f47993d5e498f1e77ebd9467c190b17085ea5862b5fb1049ebbaf278fcd434`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 16 Dec 2020 23:40:37 GMT
ADD file:47bb1b85a4eb4d0b355ae89ec5c71c09e2c2b7e21e1851a2896365eb17134f57 in / 
# Wed, 16 Dec 2020 23:40:39 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 00:27:02 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 17 Dec 2020 00:27:42 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/containous/traefik/releases/download/v1.7.26/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Thu, 17 Dec 2020 00:27:43 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 17 Dec 2020 00:27:44 GMT
EXPOSE 80
# Thu, 17 Dec 2020 00:27:45 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 17 Dec 2020 00:27:46 GMT
CMD ["traefik"]
# Thu, 17 Dec 2020 00:27:47 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.26 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:6be00c7721dc4a904b3531bfb7878ea6761d57116b3730c05eac3cb31e726a7e`  
		Last Modified: Thu, 17 Dec 2020 00:29:37 GMT  
		Size: 19.5 MB (19493133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37d0080e4ada531446b01e45e014d2c9983281dc58b873e4162e1adb99b6f3ad`  
		Last Modified: Thu, 17 Dec 2020 00:29:20 GMT  
		Size: 369.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:1.7-windowsservercore-1809`

```console
$ docker pull traefik@sha256:2c85e3865465339ff28a47a1511b774491ef43ee5c10e9fce0eed4512dca8e84
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1637; amd64

### `traefik:1.7-windowsservercore-1809` - windows version 10.0.17763.1637; amd64

```console
$ docker pull traefik@sha256:ecf2dd6f2cebbfdae3bd25b7ba2a68fea62a623ad337bc401dbfbff0ff03f48f
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2421243323 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c7ae3b3576f87d9dba1f675160af62a993ec7e3a322ac90f9f258497a933fef0`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 04 Dec 2020 02:13:01 GMT
RUN Install update 1809-amd64
# Wed, 09 Dec 2020 13:30:16 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Dec 2020 23:59:07 GMT
RUN Invoke-WebRequest     -Uri "https://github.com/containous/traefik/releases/download/v1.7.26/traefik_windows-amd64.exe"     -OutFile "/traefik.exe"
# Wed, 09 Dec 2020 23:59:09 GMT
EXPOSE 80
# Wed, 09 Dec 2020 23:59:10 GMT
ENTRYPOINT ["/traefik"]
# Wed, 09 Dec 2020 23:59:11 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.26 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:aa4f58cd6da1aaf1a0b44d443bd88e7fbe5b0a6f193995a1a61d6bd63990f314`  
		Size: 672.5 MB (672541583 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a4372d14958dc8a7eaaace9e4774e7f1db524da5eb4474b5e46738848a3a61a5`  
		Last Modified: Wed, 09 Dec 2020 13:54:38 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34300192a929cc8734d3561486bbf20306f0ddf75c3d405112b40a535022d87e`  
		Last Modified: Thu, 10 Dec 2020 00:00:39 GMT  
		Size: 30.4 MB (30364288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bcea0e9edffb70e9148c20ab78ddd79ecb43d454593638a01c8900035a7dfc9`  
		Last Modified: Thu, 10 Dec 2020 00:00:05 GMT  
		Size: 1.1 KB (1132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a53d2ed509732587fa21d4aad5f1ef27c38a85b71e038e15079a978fa5d3114`  
		Last Modified: Thu, 10 Dec 2020 00:00:05 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4118d174807346b7e443506fd438961205a118f2e545f00d509b2a299a92cc06`  
		Last Modified: Thu, 10 Dec 2020 00:00:05 GMT  
		Size: 1.2 KB (1187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:2.3`

```console
$ docker pull traefik@sha256:6329d060190998d5c9a85f9b812177601a753dc32094195d4e5efbd6bd8f191d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:2.3` - linux; amd64

```console
$ docker pull traefik@sha256:d8faddf331546aca9cfec4091185ef6f0f7654246f5f0656ff5ef53eeae7fd18
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.4 MB (28385315 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:54db2e08f87e0483ab129ec7e400baa38d3616d4821640abbfa740c9398ad864`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 17 Dec 2020 00:19:49 GMT
ADD file:8ed80010e443da19d72546bcee9a35e0a8d244c72052b1994610bf5939d479c2 in / 
# Thu, 17 Dec 2020 00:19:49 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 00:47:33 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 17 Dec 2020 00:47:44 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.3.5/traefik_v2.3.5_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 17 Dec 2020 00:47:44 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 17 Dec 2020 00:47:44 GMT
EXPOSE 80
# Thu, 17 Dec 2020 00:47:45 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 17 Dec 2020 00:47:45 GMT
CMD ["traefik"]
# Thu, 17 Dec 2020 00:47:45 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.3.5 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:9317c0d35096c63079779d328115613d4408f9c4be4c93e3a67fd2631b160854`  
		Last Modified: Thu, 17 Dec 2020 00:48:55 GMT  
		Size: 24.9 MB (24898385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c262a5be356023fa84388e766cd12952112ad0805c10d1316483fd465b668e1`  
		Last Modified: Thu, 17 Dec 2020 00:48:50 GMT  
		Size: 369.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:2.3` - linux; arm variant v6

```console
$ docker pull traefik@sha256:200709b0233fee1951b48edabee5f71c4c143c6883f19349cbeec2fe830d4222
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.5 MB (26482700 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:38d6a862b01e1d5a6b608926e2b099151560a2d809398e048f1ab8987d6913e2`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 16 Dec 2020 23:49:53 GMT
ADD file:e3a6f7566ee3c2ba61d27d801d3522e045a4be64a42f32ee52d933b68338d06f in / 
# Wed, 16 Dec 2020 23:49:55 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 00:25:55 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 17 Dec 2020 00:26:15 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.3.5/traefik_v2.3.5_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 17 Dec 2020 00:26:17 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 17 Dec 2020 00:26:18 GMT
EXPOSE 80
# Thu, 17 Dec 2020 00:26:18 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 17 Dec 2020 00:26:19 GMT
CMD ["traefik"]
# Thu, 17 Dec 2020 00:26:20 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.3.5 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:708a31fe0f367f038f8442997d0200a64291d57caa1d8fcbf8ca6a7bfdeaeab9`  
		Last Modified: Thu, 17 Dec 2020 00:28:01 GMT  
		Size: 23.2 MB (23186660 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff140dbd5ae36d65c765bcdb73f2bfb095918f404c9421eda0b4217f86af0101`  
		Last Modified: Thu, 17 Dec 2020 00:27:53 GMT  
		Size: 369.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:2.3` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:a41ad437600dbfefbdf4bd0c89a6dbe6f178be4f693f1a18d28517fbbe4cf32b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.1 MB (26097249 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1eaf2b0865bc3065f86245d528f1881d0122b7d792620dcbd7f45ff4b4bb060f`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 16 Dec 2020 23:40:37 GMT
ADD file:47bb1b85a4eb4d0b355ae89ec5c71c09e2c2b7e21e1851a2896365eb17134f57 in / 
# Wed, 16 Dec 2020 23:40:39 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 00:27:02 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 17 Dec 2020 00:27:25 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.3.5/traefik_v2.3.5_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 17 Dec 2020 00:27:26 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 17 Dec 2020 00:27:28 GMT
EXPOSE 80
# Thu, 17 Dec 2020 00:27:29 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 17 Dec 2020 00:27:30 GMT
CMD ["traefik"]
# Thu, 17 Dec 2020 00:27:31 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.3.5 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:6e25b961f24a55c5614ba4272f7197b1a40e24999c3113f7a63bafea52304451`  
		Last Modified: Thu, 17 Dec 2020 00:29:06 GMT  
		Size: 22.7 MB (22698418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1383e7238dfb4d957a85710afdfd6389bda4310df784820d996d0d034dabb2c1`  
		Last Modified: Thu, 17 Dec 2020 00:28:58 GMT  
		Size: 369.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:2.3.6`

**does not exist** (yet?)

## `traefik:2.3.6-windowsservercore-1809`

**does not exist** (yet?)

## `traefik:2.3-windowsservercore-1809`

```console
$ docker pull traefik@sha256:e00168af8fd06c5db5810991b63ae9bc32f624cb574998cbe7705bf171d2575b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1637; amd64

### `traefik:2.3-windowsservercore-1809` - windows version 10.0.17763.1637; amd64

```console
$ docker pull traefik@sha256:c86e24a0e106ce1187d55f8ef015cc038ac6fb238890bb24e0e6534752c41075
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2425379374 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b35eb3df56ce0eafb6242f83b0c7170bf0496cd8e220d64148de4c270112992e`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 04 Dec 2020 02:13:01 GMT
RUN Install update 1809-amd64
# Wed, 09 Dec 2020 13:30:16 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Fri, 11 Dec 2020 01:45:44 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/traefik/traefik/releases/download/v2.3.5/traefik_v2.3.5_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Fri, 11 Dec 2020 01:45:48 GMT
EXPOSE 80
# Fri, 11 Dec 2020 01:45:48 GMT
ENTRYPOINT ["/traefik"]
# Fri, 11 Dec 2020 01:45:49 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.3.5 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:aa4f58cd6da1aaf1a0b44d443bd88e7fbe5b0a6f193995a1a61d6bd63990f314`  
		Size: 672.5 MB (672541583 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a4372d14958dc8a7eaaace9e4774e7f1db524da5eb4474b5e46738848a3a61a5`  
		Last Modified: Wed, 09 Dec 2020 13:54:38 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85482ae30bb6c78ecdd6711396f28c8e7d825b0b2fdc5d98b4b7ef1fa55c058a`  
		Last Modified: Fri, 11 Dec 2020 01:46:23 GMT  
		Size: 34.5 MB (34500366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:235692d5c0973ec6d5f726c71422568cbc87ccd6fef238182d05e58450b1a2a8`  
		Last Modified: Fri, 11 Dec 2020 01:46:14 GMT  
		Size: 1.2 KB (1156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5f09935d359b99a157f3caae523bb65efd1975c0d56175dc692646a7262ab6c`  
		Last Modified: Fri, 11 Dec 2020 01:46:14 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ba9ec09cdbc0f0266e3781e8e9d1a12f5440b6847485d9a4f0a20e69579750b`  
		Last Modified: Fri, 11 Dec 2020 01:46:15 GMT  
		Size: 1.1 KB (1132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:2.4`

```console
$ docker pull traefik@sha256:7d8a40698784af9bc56591e7402378deccc31df8ef51f6e09a7e0f4afa1787c1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:2.4` - linux; amd64

```console
$ docker pull traefik@sha256:e72173181d61d6d38147617dc8932f18913eef9b8b016590c987c9601df7156f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.1 MB (29072354 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:77adf581ab54982c064a76d40ab167586a222980aa9818458208cdb9761363fa`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 17 Dec 2020 00:19:49 GMT
ADD file:8ed80010e443da19d72546bcee9a35e0a8d244c72052b1994610bf5939d479c2 in / 
# Thu, 17 Dec 2020 00:19:49 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 00:47:33 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 17 Dec 2020 00:47:36 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.4.0-rc1/traefik_v2.4.0-rc1_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 17 Dec 2020 00:47:36 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 17 Dec 2020 00:47:36 GMT
EXPOSE 80
# Thu, 17 Dec 2020 00:47:36 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 17 Dec 2020 00:47:37 GMT
CMD ["traefik"]
# Thu, 17 Dec 2020 00:47:37 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.4.0-rc1 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:6348b818709856ced463f120a41e43ce15a035508e8cefd7ffcfe67295a783ed`  
		Last Modified: Thu, 17 Dec 2020 00:48:42 GMT  
		Size: 25.6 MB (25585425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc293a73c224168214a62f4c533ab7995c8744665c887eb0a797b53f125dbd60`  
		Last Modified: Thu, 17 Dec 2020 00:48:36 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:2.4` - linux; arm variant v6

```console
$ docker pull traefik@sha256:0464505a5542f0c35a80906488d4f17acc8bc062ac5480abcdba5961e85dedef
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.1 MB (27107202 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0a44b18ddf6ab462a4af8dbedfb58eaca6b7002622164563c3c18128b35078e4`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 16 Dec 2020 23:49:53 GMT
ADD file:e3a6f7566ee3c2ba61d27d801d3522e045a4be64a42f32ee52d933b68338d06f in / 
# Wed, 16 Dec 2020 23:49:55 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 00:25:55 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 17 Dec 2020 00:26:00 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.4.0-rc1/traefik_v2.4.0-rc1_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 17 Dec 2020 00:26:01 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 17 Dec 2020 00:26:02 GMT
EXPOSE 80
# Thu, 17 Dec 2020 00:26:02 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 17 Dec 2020 00:26:03 GMT
CMD ["traefik"]
# Thu, 17 Dec 2020 00:26:04 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.4.0-rc1 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:71a89144d2ec5013a820f4de949514c963d60f1eafac95fc5c0626ac3a5fca49`  
		Last Modified: Thu, 17 Dec 2020 00:27:32 GMT  
		Size: 23.8 MB (23811162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6633878abde02f77de69e78a3868c33a28300c0c47a47f81297473d9186bd156`  
		Last Modified: Thu, 17 Dec 2020 00:27:24 GMT  
		Size: 369.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:2.4` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:e1975275fbaf78b62a8a588b67d3ea3b72acc9ffcd47176cb4e987acf3f73c13
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.7 MB (26736293 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4646b0137cf051fe81afc86b698d2d8849446adda9ab81c8871f01b8c2e52d94`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 16 Dec 2020 23:40:37 GMT
ADD file:47bb1b85a4eb4d0b355ae89ec5c71c09e2c2b7e21e1851a2896365eb17134f57 in / 
# Wed, 16 Dec 2020 23:40:39 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 00:27:02 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 17 Dec 2020 00:27:08 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.4.0-rc1/traefik_v2.4.0-rc1_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 17 Dec 2020 00:27:09 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 17 Dec 2020 00:27:10 GMT
EXPOSE 80
# Thu, 17 Dec 2020 00:27:11 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 17 Dec 2020 00:27:12 GMT
CMD ["traefik"]
# Thu, 17 Dec 2020 00:27:13 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.4.0-rc1 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:a8c978289529e0d75adc45110a61b13d8d3791c39eda7bc74272d02afce9d584`  
		Last Modified: Thu, 17 Dec 2020 00:28:46 GMT  
		Size: 23.3 MB (23337462 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ade89e86f523ff8f8f95973a320cd860a913d5aac0df71602635b88f488a3567`  
		Last Modified: Thu, 17 Dec 2020 00:28:38 GMT  
		Size: 369.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:2.4.0-rc1`

```console
$ docker pull traefik@sha256:7d8a40698784af9bc56591e7402378deccc31df8ef51f6e09a7e0f4afa1787c1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:2.4.0-rc1` - linux; amd64

```console
$ docker pull traefik@sha256:e72173181d61d6d38147617dc8932f18913eef9b8b016590c987c9601df7156f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.1 MB (29072354 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:77adf581ab54982c064a76d40ab167586a222980aa9818458208cdb9761363fa`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 17 Dec 2020 00:19:49 GMT
ADD file:8ed80010e443da19d72546bcee9a35e0a8d244c72052b1994610bf5939d479c2 in / 
# Thu, 17 Dec 2020 00:19:49 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 00:47:33 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 17 Dec 2020 00:47:36 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.4.0-rc1/traefik_v2.4.0-rc1_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 17 Dec 2020 00:47:36 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 17 Dec 2020 00:47:36 GMT
EXPOSE 80
# Thu, 17 Dec 2020 00:47:36 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 17 Dec 2020 00:47:37 GMT
CMD ["traefik"]
# Thu, 17 Dec 2020 00:47:37 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.4.0-rc1 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:6348b818709856ced463f120a41e43ce15a035508e8cefd7ffcfe67295a783ed`  
		Last Modified: Thu, 17 Dec 2020 00:48:42 GMT  
		Size: 25.6 MB (25585425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc293a73c224168214a62f4c533ab7995c8744665c887eb0a797b53f125dbd60`  
		Last Modified: Thu, 17 Dec 2020 00:48:36 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:2.4.0-rc1` - linux; arm variant v6

```console
$ docker pull traefik@sha256:0464505a5542f0c35a80906488d4f17acc8bc062ac5480abcdba5961e85dedef
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.1 MB (27107202 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0a44b18ddf6ab462a4af8dbedfb58eaca6b7002622164563c3c18128b35078e4`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 16 Dec 2020 23:49:53 GMT
ADD file:e3a6f7566ee3c2ba61d27d801d3522e045a4be64a42f32ee52d933b68338d06f in / 
# Wed, 16 Dec 2020 23:49:55 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 00:25:55 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 17 Dec 2020 00:26:00 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.4.0-rc1/traefik_v2.4.0-rc1_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 17 Dec 2020 00:26:01 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 17 Dec 2020 00:26:02 GMT
EXPOSE 80
# Thu, 17 Dec 2020 00:26:02 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 17 Dec 2020 00:26:03 GMT
CMD ["traefik"]
# Thu, 17 Dec 2020 00:26:04 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.4.0-rc1 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:71a89144d2ec5013a820f4de949514c963d60f1eafac95fc5c0626ac3a5fca49`  
		Last Modified: Thu, 17 Dec 2020 00:27:32 GMT  
		Size: 23.8 MB (23811162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6633878abde02f77de69e78a3868c33a28300c0c47a47f81297473d9186bd156`  
		Last Modified: Thu, 17 Dec 2020 00:27:24 GMT  
		Size: 369.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:2.4.0-rc1` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:e1975275fbaf78b62a8a588b67d3ea3b72acc9ffcd47176cb4e987acf3f73c13
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.7 MB (26736293 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4646b0137cf051fe81afc86b698d2d8849446adda9ab81c8871f01b8c2e52d94`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 16 Dec 2020 23:40:37 GMT
ADD file:47bb1b85a4eb4d0b355ae89ec5c71c09e2c2b7e21e1851a2896365eb17134f57 in / 
# Wed, 16 Dec 2020 23:40:39 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 00:27:02 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 17 Dec 2020 00:27:08 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.4.0-rc1/traefik_v2.4.0-rc1_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 17 Dec 2020 00:27:09 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 17 Dec 2020 00:27:10 GMT
EXPOSE 80
# Thu, 17 Dec 2020 00:27:11 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 17 Dec 2020 00:27:12 GMT
CMD ["traefik"]
# Thu, 17 Dec 2020 00:27:13 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.4.0-rc1 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:a8c978289529e0d75adc45110a61b13d8d3791c39eda7bc74272d02afce9d584`  
		Last Modified: Thu, 17 Dec 2020 00:28:46 GMT  
		Size: 23.3 MB (23337462 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ade89e86f523ff8f8f95973a320cd860a913d5aac0df71602635b88f488a3567`  
		Last Modified: Thu, 17 Dec 2020 00:28:38 GMT  
		Size: 369.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:2.4.0-rc1-windowsservercore-1809`

```console
$ docker pull traefik@sha256:c38beba5d61f64ff442e2c8c2e9e7419fb47bdb125b54bbeb0e36b6351d292c1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1637; amd64

### `traefik:2.4.0-rc1-windowsservercore-1809` - windows version 10.0.17763.1637; amd64

```console
$ docker pull traefik@sha256:5be07f9155301dae81e2580ea435677afb018e22df3250d845d1519d9757c9ab
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2426094285 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:69c5a39fe06b07e4794aeffb43f0a1eb437f5f28937a57f4228c090951b2f84a`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 04 Dec 2020 02:13:01 GMT
RUN Install update 1809-amd64
# Wed, 09 Dec 2020 13:30:16 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 17 Dec 2020 00:16:07 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/traefik/traefik/releases/download/v2.4.0-rc1/traefik_v2.4.0-rc1_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Thu, 17 Dec 2020 00:16:11 GMT
EXPOSE 80
# Thu, 17 Dec 2020 00:16:12 GMT
ENTRYPOINT ["/traefik"]
# Thu, 17 Dec 2020 00:16:13 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.4.0-rc1 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:aa4f58cd6da1aaf1a0b44d443bd88e7fbe5b0a6f193995a1a61d6bd63990f314`  
		Size: 672.5 MB (672541583 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a4372d14958dc8a7eaaace9e4774e7f1db524da5eb4474b5e46738848a3a61a5`  
		Last Modified: Wed, 09 Dec 2020 13:54:38 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54167c9a07bde1e13b39ce2bf3c56eaeb33f6466c6a33624dcf3c713b3697e67`  
		Last Modified: Thu, 17 Dec 2020 00:16:59 GMT  
		Size: 35.2 MB (35215314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd6d21c529f31e5de6bfd8d23955872cee397bd7df6332d69b7b97a899868e44`  
		Last Modified: Thu, 17 Dec 2020 00:16:51 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bbf669e97927e7ae7c8ba2a38289f46ec356ed92b648e920c809bbbf8a78fb1`  
		Last Modified: Thu, 17 Dec 2020 00:16:50 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:769f092fb22a8b9cea7104db10bf8b7085aec60d35a3e9938cc433c5861e3744`  
		Last Modified: Thu, 17 Dec 2020 00:16:51 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:2.4-windowsservercore-1809`

```console
$ docker pull traefik@sha256:c38beba5d61f64ff442e2c8c2e9e7419fb47bdb125b54bbeb0e36b6351d292c1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1637; amd64

### `traefik:2.4-windowsservercore-1809` - windows version 10.0.17763.1637; amd64

```console
$ docker pull traefik@sha256:5be07f9155301dae81e2580ea435677afb018e22df3250d845d1519d9757c9ab
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2426094285 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:69c5a39fe06b07e4794aeffb43f0a1eb437f5f28937a57f4228c090951b2f84a`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 04 Dec 2020 02:13:01 GMT
RUN Install update 1809-amd64
# Wed, 09 Dec 2020 13:30:16 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 17 Dec 2020 00:16:07 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/traefik/traefik/releases/download/v2.4.0-rc1/traefik_v2.4.0-rc1_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Thu, 17 Dec 2020 00:16:11 GMT
EXPOSE 80
# Thu, 17 Dec 2020 00:16:12 GMT
ENTRYPOINT ["/traefik"]
# Thu, 17 Dec 2020 00:16:13 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.4.0-rc1 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:aa4f58cd6da1aaf1a0b44d443bd88e7fbe5b0a6f193995a1a61d6bd63990f314`  
		Size: 672.5 MB (672541583 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a4372d14958dc8a7eaaace9e4774e7f1db524da5eb4474b5e46738848a3a61a5`  
		Last Modified: Wed, 09 Dec 2020 13:54:38 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54167c9a07bde1e13b39ce2bf3c56eaeb33f6466c6a33624dcf3c713b3697e67`  
		Last Modified: Thu, 17 Dec 2020 00:16:59 GMT  
		Size: 35.2 MB (35215314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd6d21c529f31e5de6bfd8d23955872cee397bd7df6332d69b7b97a899868e44`  
		Last Modified: Thu, 17 Dec 2020 00:16:51 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bbf669e97927e7ae7c8ba2a38289f46ec356ed92b648e920c809bbbf8a78fb1`  
		Last Modified: Thu, 17 Dec 2020 00:16:50 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:769f092fb22a8b9cea7104db10bf8b7085aec60d35a3e9938cc433c5861e3744`  
		Last Modified: Thu, 17 Dec 2020 00:16:51 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:latest`

```console
$ docker pull traefik@sha256:6329d060190998d5c9a85f9b812177601a753dc32094195d4e5efbd6bd8f191d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:latest` - linux; amd64

```console
$ docker pull traefik@sha256:d8faddf331546aca9cfec4091185ef6f0f7654246f5f0656ff5ef53eeae7fd18
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.4 MB (28385315 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:54db2e08f87e0483ab129ec7e400baa38d3616d4821640abbfa740c9398ad864`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 17 Dec 2020 00:19:49 GMT
ADD file:8ed80010e443da19d72546bcee9a35e0a8d244c72052b1994610bf5939d479c2 in / 
# Thu, 17 Dec 2020 00:19:49 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 00:47:33 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 17 Dec 2020 00:47:44 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.3.5/traefik_v2.3.5_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 17 Dec 2020 00:47:44 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 17 Dec 2020 00:47:44 GMT
EXPOSE 80
# Thu, 17 Dec 2020 00:47:45 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 17 Dec 2020 00:47:45 GMT
CMD ["traefik"]
# Thu, 17 Dec 2020 00:47:45 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.3.5 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:9317c0d35096c63079779d328115613d4408f9c4be4c93e3a67fd2631b160854`  
		Last Modified: Thu, 17 Dec 2020 00:48:55 GMT  
		Size: 24.9 MB (24898385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c262a5be356023fa84388e766cd12952112ad0805c10d1316483fd465b668e1`  
		Last Modified: Thu, 17 Dec 2020 00:48:50 GMT  
		Size: 369.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:latest` - linux; arm variant v6

```console
$ docker pull traefik@sha256:200709b0233fee1951b48edabee5f71c4c143c6883f19349cbeec2fe830d4222
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.5 MB (26482700 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:38d6a862b01e1d5a6b608926e2b099151560a2d809398e048f1ab8987d6913e2`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 16 Dec 2020 23:49:53 GMT
ADD file:e3a6f7566ee3c2ba61d27d801d3522e045a4be64a42f32ee52d933b68338d06f in / 
# Wed, 16 Dec 2020 23:49:55 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 00:25:55 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 17 Dec 2020 00:26:15 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.3.5/traefik_v2.3.5_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 17 Dec 2020 00:26:17 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 17 Dec 2020 00:26:18 GMT
EXPOSE 80
# Thu, 17 Dec 2020 00:26:18 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 17 Dec 2020 00:26:19 GMT
CMD ["traefik"]
# Thu, 17 Dec 2020 00:26:20 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.3.5 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:708a31fe0f367f038f8442997d0200a64291d57caa1d8fcbf8ca6a7bfdeaeab9`  
		Last Modified: Thu, 17 Dec 2020 00:28:01 GMT  
		Size: 23.2 MB (23186660 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff140dbd5ae36d65c765bcdb73f2bfb095918f404c9421eda0b4217f86af0101`  
		Last Modified: Thu, 17 Dec 2020 00:27:53 GMT  
		Size: 369.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:latest` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:a41ad437600dbfefbdf4bd0c89a6dbe6f178be4f693f1a18d28517fbbe4cf32b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.1 MB (26097249 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1eaf2b0865bc3065f86245d528f1881d0122b7d792620dcbd7f45ff4b4bb060f`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 16 Dec 2020 23:40:37 GMT
ADD file:47bb1b85a4eb4d0b355ae89ec5c71c09e2c2b7e21e1851a2896365eb17134f57 in / 
# Wed, 16 Dec 2020 23:40:39 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 00:27:02 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 17 Dec 2020 00:27:25 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.3.5/traefik_v2.3.5_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 17 Dec 2020 00:27:26 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 17 Dec 2020 00:27:28 GMT
EXPOSE 80
# Thu, 17 Dec 2020 00:27:29 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 17 Dec 2020 00:27:30 GMT
CMD ["traefik"]
# Thu, 17 Dec 2020 00:27:31 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.3.5 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:6e25b961f24a55c5614ba4272f7197b1a40e24999c3113f7a63bafea52304451`  
		Last Modified: Thu, 17 Dec 2020 00:29:06 GMT  
		Size: 22.7 MB (22698418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1383e7238dfb4d957a85710afdfd6389bda4310df784820d996d0d034dabb2c1`  
		Last Modified: Thu, 17 Dec 2020 00:28:58 GMT  
		Size: 369.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:livarot`

```console
$ docker pull traefik@sha256:7d8a40698784af9bc56591e7402378deccc31df8ef51f6e09a7e0f4afa1787c1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:livarot` - linux; amd64

```console
$ docker pull traefik@sha256:e72173181d61d6d38147617dc8932f18913eef9b8b016590c987c9601df7156f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.1 MB (29072354 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:77adf581ab54982c064a76d40ab167586a222980aa9818458208cdb9761363fa`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 17 Dec 2020 00:19:49 GMT
ADD file:8ed80010e443da19d72546bcee9a35e0a8d244c72052b1994610bf5939d479c2 in / 
# Thu, 17 Dec 2020 00:19:49 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 00:47:33 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 17 Dec 2020 00:47:36 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.4.0-rc1/traefik_v2.4.0-rc1_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 17 Dec 2020 00:47:36 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 17 Dec 2020 00:47:36 GMT
EXPOSE 80
# Thu, 17 Dec 2020 00:47:36 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 17 Dec 2020 00:47:37 GMT
CMD ["traefik"]
# Thu, 17 Dec 2020 00:47:37 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.4.0-rc1 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:6348b818709856ced463f120a41e43ce15a035508e8cefd7ffcfe67295a783ed`  
		Last Modified: Thu, 17 Dec 2020 00:48:42 GMT  
		Size: 25.6 MB (25585425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc293a73c224168214a62f4c533ab7995c8744665c887eb0a797b53f125dbd60`  
		Last Modified: Thu, 17 Dec 2020 00:48:36 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:livarot` - linux; arm variant v6

```console
$ docker pull traefik@sha256:0464505a5542f0c35a80906488d4f17acc8bc062ac5480abcdba5961e85dedef
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.1 MB (27107202 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0a44b18ddf6ab462a4af8dbedfb58eaca6b7002622164563c3c18128b35078e4`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 16 Dec 2020 23:49:53 GMT
ADD file:e3a6f7566ee3c2ba61d27d801d3522e045a4be64a42f32ee52d933b68338d06f in / 
# Wed, 16 Dec 2020 23:49:55 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 00:25:55 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 17 Dec 2020 00:26:00 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.4.0-rc1/traefik_v2.4.0-rc1_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 17 Dec 2020 00:26:01 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 17 Dec 2020 00:26:02 GMT
EXPOSE 80
# Thu, 17 Dec 2020 00:26:02 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 17 Dec 2020 00:26:03 GMT
CMD ["traefik"]
# Thu, 17 Dec 2020 00:26:04 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.4.0-rc1 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:71a89144d2ec5013a820f4de949514c963d60f1eafac95fc5c0626ac3a5fca49`  
		Last Modified: Thu, 17 Dec 2020 00:27:32 GMT  
		Size: 23.8 MB (23811162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6633878abde02f77de69e78a3868c33a28300c0c47a47f81297473d9186bd156`  
		Last Modified: Thu, 17 Dec 2020 00:27:24 GMT  
		Size: 369.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:livarot` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:e1975275fbaf78b62a8a588b67d3ea3b72acc9ffcd47176cb4e987acf3f73c13
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.7 MB (26736293 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4646b0137cf051fe81afc86b698d2d8849446adda9ab81c8871f01b8c2e52d94`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 16 Dec 2020 23:40:37 GMT
ADD file:47bb1b85a4eb4d0b355ae89ec5c71c09e2c2b7e21e1851a2896365eb17134f57 in / 
# Wed, 16 Dec 2020 23:40:39 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 00:27:02 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 17 Dec 2020 00:27:08 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.4.0-rc1/traefik_v2.4.0-rc1_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 17 Dec 2020 00:27:09 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 17 Dec 2020 00:27:10 GMT
EXPOSE 80
# Thu, 17 Dec 2020 00:27:11 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 17 Dec 2020 00:27:12 GMT
CMD ["traefik"]
# Thu, 17 Dec 2020 00:27:13 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.4.0-rc1 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:a8c978289529e0d75adc45110a61b13d8d3791c39eda7bc74272d02afce9d584`  
		Last Modified: Thu, 17 Dec 2020 00:28:46 GMT  
		Size: 23.3 MB (23337462 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ade89e86f523ff8f8f95973a320cd860a913d5aac0df71602635b88f488a3567`  
		Last Modified: Thu, 17 Dec 2020 00:28:38 GMT  
		Size: 369.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:livarot-windowsservercore-1809`

```console
$ docker pull traefik@sha256:c38beba5d61f64ff442e2c8c2e9e7419fb47bdb125b54bbeb0e36b6351d292c1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1637; amd64

### `traefik:livarot-windowsservercore-1809` - windows version 10.0.17763.1637; amd64

```console
$ docker pull traefik@sha256:5be07f9155301dae81e2580ea435677afb018e22df3250d845d1519d9757c9ab
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2426094285 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:69c5a39fe06b07e4794aeffb43f0a1eb437f5f28937a57f4228c090951b2f84a`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 04 Dec 2020 02:13:01 GMT
RUN Install update 1809-amd64
# Wed, 09 Dec 2020 13:30:16 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 17 Dec 2020 00:16:07 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/traefik/traefik/releases/download/v2.4.0-rc1/traefik_v2.4.0-rc1_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Thu, 17 Dec 2020 00:16:11 GMT
EXPOSE 80
# Thu, 17 Dec 2020 00:16:12 GMT
ENTRYPOINT ["/traefik"]
# Thu, 17 Dec 2020 00:16:13 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.4.0-rc1 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:aa4f58cd6da1aaf1a0b44d443bd88e7fbe5b0a6f193995a1a61d6bd63990f314`  
		Size: 672.5 MB (672541583 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a4372d14958dc8a7eaaace9e4774e7f1db524da5eb4474b5e46738848a3a61a5`  
		Last Modified: Wed, 09 Dec 2020 13:54:38 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54167c9a07bde1e13b39ce2bf3c56eaeb33f6466c6a33624dcf3c713b3697e67`  
		Last Modified: Thu, 17 Dec 2020 00:16:59 GMT  
		Size: 35.2 MB (35215314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd6d21c529f31e5de6bfd8d23955872cee397bd7df6332d69b7b97a899868e44`  
		Last Modified: Thu, 17 Dec 2020 00:16:51 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bbf669e97927e7ae7c8ba2a38289f46ec356ed92b648e920c809bbbf8a78fb1`  
		Last Modified: Thu, 17 Dec 2020 00:16:50 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:769f092fb22a8b9cea7104db10bf8b7085aec60d35a3e9938cc433c5861e3744`  
		Last Modified: Thu, 17 Dec 2020 00:16:51 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:maroilles`

```console
$ docker pull traefik@sha256:9a53d5dff2c5b474a8560a4af129cc7863fb8932f8bd0e6896f4292445a2bf86
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:maroilles` - linux; amd64

```console
$ docker pull traefik@sha256:78a0311203a68b2a9173d8e19b42fc39e5f02f17f1db03c1a06e3fa1c66f4dd7
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **21.6 MB (21563612 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:23b804da420476b5cbcc59bdd26e354e8fa44e4dfe20caf3ac84768dd143b5f2`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Thu, 17 Dec 2020 00:48:11 GMT
COPY file:cd6264d9a7514a8fbc3eb7b400566d36178794d2b757959812cc3abc6f13a97b in /etc/ssl/certs/ 
# Thu, 17 Dec 2020 00:48:11 GMT
COPY dir:83da415af0ff24b3b9d10f857aa8c724a3bc93523f3e047b827e7554fe1f9e08 in /usr/share/ 
# Thu, 17 Dec 2020 00:48:12 GMT
COPY file:8e3cf7c133ac957e81d3eb831160ad827bfde058f356d7ac234b8c5ae307e37a in / 
# Thu, 17 Dec 2020 00:48:12 GMT
EXPOSE 80
# Thu, 17 Dec 2020 00:48:13 GMT
VOLUME [/tmp]
# Thu, 17 Dec 2020 00:48:13 GMT
ENTRYPOINT ["/traefik"]
# Thu, 17 Dec 2020 00:48:13 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.26 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:eca797b3e2d2ac9c3925e07a34654011a4314302362ca0dfe8320d4425bf01f5`  
		Last Modified: Thu, 17 Dec 2020 00:49:22 GMT  
		Size: 21.1 MB (21126329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:maroilles` - linux; arm variant v6

```console
$ docker pull traefik@sha256:bb041f9232284130c3646cd4f0d83e032b078ae88a9ab88ea46580df2ee0b991
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **20.2 MB (20210272 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4c618c098e7b6182b45a63ffa8f49bb1656407fb6b666da85775efb87264cf12`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Thu, 17 Dec 2020 00:26:47 GMT
COPY file:cd6264d9a7514a8fbc3eb7b400566d36178794d2b757959812cc3abc6f13a97b in /etc/ssl/certs/ 
# Thu, 17 Dec 2020 00:26:48 GMT
COPY dir:83da415af0ff24b3b9d10f857aa8c724a3bc93523f3e047b827e7554fe1f9e08 in /usr/share/ 
# Thu, 17 Dec 2020 00:26:52 GMT
COPY file:a02ffe991352ee1f8abb077135ea9d27557e8b364fb712a42ccb2865e08df3cc in / 
# Thu, 17 Dec 2020 00:26:53 GMT
EXPOSE 80
# Thu, 17 Dec 2020 00:26:54 GMT
VOLUME [/tmp]
# Thu, 17 Dec 2020 00:26:56 GMT
ENTRYPOINT ["/traefik"]
# Thu, 17 Dec 2020 00:26:57 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.26 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:decc75cc844d668e21a715048cd9c78f2804e625a910fe5568e174c89bd5d8ab`  
		Last Modified: Thu, 17 Dec 2020 00:28:49 GMT  
		Size: 19.8 MB (19772941 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:maroilles` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:2dc4a89841d24667bf689a0386eed1525cfe92afd4847039d73204d17e8d77f6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **19.9 MB (19930321 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5993443e6d894e7f4a83e79f4ede7636a3c8b57e7dca57a2dac980bed5a48274`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Thu, 17 Dec 2020 00:27:56 GMT
COPY file:cd6264d9a7514a8fbc3eb7b400566d36178794d2b757959812cc3abc6f13a97b in /etc/ssl/certs/ 
# Thu, 17 Dec 2020 00:27:58 GMT
COPY dir:83da415af0ff24b3b9d10f857aa8c724a3bc93523f3e047b827e7554fe1f9e08 in /usr/share/ 
# Thu, 17 Dec 2020 00:27:59 GMT
COPY file:f592954af2951d1a2538b1945366cb995f49638c7ef8b561b6961e0f8023197a in / 
# Thu, 17 Dec 2020 00:28:00 GMT
EXPOSE 80
# Thu, 17 Dec 2020 00:28:01 GMT
VOLUME [/tmp]
# Thu, 17 Dec 2020 00:28:02 GMT
ENTRYPOINT ["/traefik"]
# Thu, 17 Dec 2020 00:28:03 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.26 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:eda38820bf6e08ea342d37563cf7e4c258c772d4a0576588e8a451209a4534b2`  
		Last Modified: Thu, 17 Dec 2020 00:30:01 GMT  
		Size: 19.5 MB (19492982 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:maroilles-alpine`

```console
$ docker pull traefik@sha256:07dce138fe44640f0c52b2f7f4fb2e92fb508ded8ae57f9a7e0fe8fdf6296673
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:maroilles-alpine` - linux; amd64

```console
$ docker pull traefik@sha256:8759aaeb837cdbbe7d39771b1442b99b182fd9556d0dfa02a4b21d254e125f9e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **24.6 MB (24613437 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6ec9aa2ea8436603df821232711432fc2de244aa083c03e3a23e002cac95549d`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 17 Dec 2020 00:19:49 GMT
ADD file:8ed80010e443da19d72546bcee9a35e0a8d244c72052b1994610bf5939d479c2 in / 
# Thu, 17 Dec 2020 00:19:49 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 00:47:33 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 17 Dec 2020 00:47:52 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/containous/traefik/releases/download/v1.7.26/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Thu, 17 Dec 2020 00:47:52 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 17 Dec 2020 00:47:52 GMT
EXPOSE 80
# Thu, 17 Dec 2020 00:47:52 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 17 Dec 2020 00:47:52 GMT
CMD ["traefik"]
# Thu, 17 Dec 2020 00:47:53 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.26 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:2d44f2e7e74e6943c5aac9ce858b295c6f31e2a0c129a718429a4a99ac1bc23d`  
		Last Modified: Thu, 17 Dec 2020 00:49:08 GMT  
		Size: 21.1 MB (21126507 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ca74d371d4ade4d81c1a76a8c789abb59c301c9b73488bfc9d0b40d3003eddf`  
		Last Modified: Thu, 17 Dec 2020 00:49:05 GMT  
		Size: 369.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:maroilles-alpine` - linux; arm variant v6

```console
$ docker pull traefik@sha256:0494095125ba05e297b154e0827115ae0618b70d40ccce4b1c496ce1666ce43d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.1 MB (23069021 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b6d3de75d11f16c38ae16a31868fe6680c4f4f196bcab0eab4ca1f85c3d9d6f0`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 16 Dec 2020 23:49:53 GMT
ADD file:e3a6f7566ee3c2ba61d27d801d3522e045a4be64a42f32ee52d933b68338d06f in / 
# Wed, 16 Dec 2020 23:49:55 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 00:25:55 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 17 Dec 2020 00:26:33 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/containous/traefik/releases/download/v1.7.26/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Thu, 17 Dec 2020 00:26:34 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 17 Dec 2020 00:26:35 GMT
EXPOSE 80
# Thu, 17 Dec 2020 00:26:36 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 17 Dec 2020 00:26:37 GMT
CMD ["traefik"]
# Thu, 17 Dec 2020 00:26:39 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.26 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:8bed822566f883c529e4423ed5efb201104f66147671cd72a5a80db2e5609dce`  
		Last Modified: Thu, 17 Dec 2020 00:28:20 GMT  
		Size: 19.8 MB (19772981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a46c867ecec8c478367249ed7ccc513e1c496aa5d628bd9950ed8ad87e604f4d`  
		Last Modified: Thu, 17 Dec 2020 00:28:14 GMT  
		Size: 369.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:maroilles-alpine` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:91c6f4a7270971b010691e5a21e487ac6d85bfbb85b83237a02dfb5c82f35055
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **22.9 MB (22891964 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f3f47993d5e498f1e77ebd9467c190b17085ea5862b5fb1049ebbaf278fcd434`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 16 Dec 2020 23:40:37 GMT
ADD file:47bb1b85a4eb4d0b355ae89ec5c71c09e2c2b7e21e1851a2896365eb17134f57 in / 
# Wed, 16 Dec 2020 23:40:39 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 00:27:02 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 17 Dec 2020 00:27:42 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/containous/traefik/releases/download/v1.7.26/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Thu, 17 Dec 2020 00:27:43 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 17 Dec 2020 00:27:44 GMT
EXPOSE 80
# Thu, 17 Dec 2020 00:27:45 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 17 Dec 2020 00:27:46 GMT
CMD ["traefik"]
# Thu, 17 Dec 2020 00:27:47 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.26 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:6be00c7721dc4a904b3531bfb7878ea6761d57116b3730c05eac3cb31e726a7e`  
		Last Modified: Thu, 17 Dec 2020 00:29:37 GMT  
		Size: 19.5 MB (19493133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37d0080e4ada531446b01e45e014d2c9983281dc58b873e4162e1adb99b6f3ad`  
		Last Modified: Thu, 17 Dec 2020 00:29:20 GMT  
		Size: 369.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:maroilles-windowsservercore-1809`

```console
$ docker pull traefik@sha256:2c85e3865465339ff28a47a1511b774491ef43ee5c10e9fce0eed4512dca8e84
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1637; amd64

### `traefik:maroilles-windowsservercore-1809` - windows version 10.0.17763.1637; amd64

```console
$ docker pull traefik@sha256:ecf2dd6f2cebbfdae3bd25b7ba2a68fea62a623ad337bc401dbfbff0ff03f48f
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2421243323 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c7ae3b3576f87d9dba1f675160af62a993ec7e3a322ac90f9f258497a933fef0`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 04 Dec 2020 02:13:01 GMT
RUN Install update 1809-amd64
# Wed, 09 Dec 2020 13:30:16 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Dec 2020 23:59:07 GMT
RUN Invoke-WebRequest     -Uri "https://github.com/containous/traefik/releases/download/v1.7.26/traefik_windows-amd64.exe"     -OutFile "/traefik.exe"
# Wed, 09 Dec 2020 23:59:09 GMT
EXPOSE 80
# Wed, 09 Dec 2020 23:59:10 GMT
ENTRYPOINT ["/traefik"]
# Wed, 09 Dec 2020 23:59:11 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.26 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:aa4f58cd6da1aaf1a0b44d443bd88e7fbe5b0a6f193995a1a61d6bd63990f314`  
		Size: 672.5 MB (672541583 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a4372d14958dc8a7eaaace9e4774e7f1db524da5eb4474b5e46738848a3a61a5`  
		Last Modified: Wed, 09 Dec 2020 13:54:38 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34300192a929cc8734d3561486bbf20306f0ddf75c3d405112b40a535022d87e`  
		Last Modified: Thu, 10 Dec 2020 00:00:39 GMT  
		Size: 30.4 MB (30364288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bcea0e9edffb70e9148c20ab78ddd79ecb43d454593638a01c8900035a7dfc9`  
		Last Modified: Thu, 10 Dec 2020 00:00:05 GMT  
		Size: 1.1 KB (1132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a53d2ed509732587fa21d4aad5f1ef27c38a85b71e038e15079a978fa5d3114`  
		Last Modified: Thu, 10 Dec 2020 00:00:05 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4118d174807346b7e443506fd438961205a118f2e545f00d509b2a299a92cc06`  
		Last Modified: Thu, 10 Dec 2020 00:00:05 GMT  
		Size: 1.2 KB (1187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:picodon`

```console
$ docker pull traefik@sha256:6329d060190998d5c9a85f9b812177601a753dc32094195d4e5efbd6bd8f191d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:picodon` - linux; amd64

```console
$ docker pull traefik@sha256:d8faddf331546aca9cfec4091185ef6f0f7654246f5f0656ff5ef53eeae7fd18
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.4 MB (28385315 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:54db2e08f87e0483ab129ec7e400baa38d3616d4821640abbfa740c9398ad864`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 17 Dec 2020 00:19:49 GMT
ADD file:8ed80010e443da19d72546bcee9a35e0a8d244c72052b1994610bf5939d479c2 in / 
# Thu, 17 Dec 2020 00:19:49 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 00:47:33 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 17 Dec 2020 00:47:44 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.3.5/traefik_v2.3.5_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 17 Dec 2020 00:47:44 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 17 Dec 2020 00:47:44 GMT
EXPOSE 80
# Thu, 17 Dec 2020 00:47:45 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 17 Dec 2020 00:47:45 GMT
CMD ["traefik"]
# Thu, 17 Dec 2020 00:47:45 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.3.5 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:9317c0d35096c63079779d328115613d4408f9c4be4c93e3a67fd2631b160854`  
		Last Modified: Thu, 17 Dec 2020 00:48:55 GMT  
		Size: 24.9 MB (24898385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c262a5be356023fa84388e766cd12952112ad0805c10d1316483fd465b668e1`  
		Last Modified: Thu, 17 Dec 2020 00:48:50 GMT  
		Size: 369.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:picodon` - linux; arm variant v6

```console
$ docker pull traefik@sha256:200709b0233fee1951b48edabee5f71c4c143c6883f19349cbeec2fe830d4222
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.5 MB (26482700 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:38d6a862b01e1d5a6b608926e2b099151560a2d809398e048f1ab8987d6913e2`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 16 Dec 2020 23:49:53 GMT
ADD file:e3a6f7566ee3c2ba61d27d801d3522e045a4be64a42f32ee52d933b68338d06f in / 
# Wed, 16 Dec 2020 23:49:55 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 00:25:55 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 17 Dec 2020 00:26:15 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.3.5/traefik_v2.3.5_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 17 Dec 2020 00:26:17 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 17 Dec 2020 00:26:18 GMT
EXPOSE 80
# Thu, 17 Dec 2020 00:26:18 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 17 Dec 2020 00:26:19 GMT
CMD ["traefik"]
# Thu, 17 Dec 2020 00:26:20 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.3.5 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:708a31fe0f367f038f8442997d0200a64291d57caa1d8fcbf8ca6a7bfdeaeab9`  
		Last Modified: Thu, 17 Dec 2020 00:28:01 GMT  
		Size: 23.2 MB (23186660 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff140dbd5ae36d65c765bcdb73f2bfb095918f404c9421eda0b4217f86af0101`  
		Last Modified: Thu, 17 Dec 2020 00:27:53 GMT  
		Size: 369.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:picodon` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:a41ad437600dbfefbdf4bd0c89a6dbe6f178be4f693f1a18d28517fbbe4cf32b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.1 MB (26097249 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1eaf2b0865bc3065f86245d528f1881d0122b7d792620dcbd7f45ff4b4bb060f`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 16 Dec 2020 23:40:37 GMT
ADD file:47bb1b85a4eb4d0b355ae89ec5c71c09e2c2b7e21e1851a2896365eb17134f57 in / 
# Wed, 16 Dec 2020 23:40:39 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 00:27:02 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 17 Dec 2020 00:27:25 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.3.5/traefik_v2.3.5_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 17 Dec 2020 00:27:26 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 17 Dec 2020 00:27:28 GMT
EXPOSE 80
# Thu, 17 Dec 2020 00:27:29 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 17 Dec 2020 00:27:30 GMT
CMD ["traefik"]
# Thu, 17 Dec 2020 00:27:31 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.3.5 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:6e25b961f24a55c5614ba4272f7197b1a40e24999c3113f7a63bafea52304451`  
		Last Modified: Thu, 17 Dec 2020 00:29:06 GMT  
		Size: 22.7 MB (22698418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1383e7238dfb4d957a85710afdfd6389bda4310df784820d996d0d034dabb2c1`  
		Last Modified: Thu, 17 Dec 2020 00:28:58 GMT  
		Size: 369.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:picodon-windowsservercore-1809`

```console
$ docker pull traefik@sha256:e00168af8fd06c5db5810991b63ae9bc32f624cb574998cbe7705bf171d2575b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1637; amd64

### `traefik:picodon-windowsservercore-1809` - windows version 10.0.17763.1637; amd64

```console
$ docker pull traefik@sha256:c86e24a0e106ce1187d55f8ef015cc038ac6fb238890bb24e0e6534752c41075
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2425379374 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b35eb3df56ce0eafb6242f83b0c7170bf0496cd8e220d64148de4c270112992e`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 04 Dec 2020 02:13:01 GMT
RUN Install update 1809-amd64
# Wed, 09 Dec 2020 13:30:16 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Fri, 11 Dec 2020 01:45:44 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/traefik/traefik/releases/download/v2.3.5/traefik_v2.3.5_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Fri, 11 Dec 2020 01:45:48 GMT
EXPOSE 80
# Fri, 11 Dec 2020 01:45:48 GMT
ENTRYPOINT ["/traefik"]
# Fri, 11 Dec 2020 01:45:49 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.3.5 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:aa4f58cd6da1aaf1a0b44d443bd88e7fbe5b0a6f193995a1a61d6bd63990f314`  
		Size: 672.5 MB (672541583 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a4372d14958dc8a7eaaace9e4774e7f1db524da5eb4474b5e46738848a3a61a5`  
		Last Modified: Wed, 09 Dec 2020 13:54:38 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85482ae30bb6c78ecdd6711396f28c8e7d825b0b2fdc5d98b4b7ef1fa55c058a`  
		Last Modified: Fri, 11 Dec 2020 01:46:23 GMT  
		Size: 34.5 MB (34500366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:235692d5c0973ec6d5f726c71422568cbc87ccd6fef238182d05e58450b1a2a8`  
		Last Modified: Fri, 11 Dec 2020 01:46:14 GMT  
		Size: 1.2 KB (1156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5f09935d359b99a157f3caae523bb65efd1975c0d56175dc692646a7262ab6c`  
		Last Modified: Fri, 11 Dec 2020 01:46:14 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ba9ec09cdbc0f0266e3781e8e9d1a12f5440b6847485d9a4f0a20e69579750b`  
		Last Modified: Fri, 11 Dec 2020 01:46:15 GMT  
		Size: 1.1 KB (1132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v1.7`

```console
$ docker pull traefik@sha256:9a53d5dff2c5b474a8560a4af129cc7863fb8932f8bd0e6896f4292445a2bf86
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:v1.7` - linux; amd64

```console
$ docker pull traefik@sha256:78a0311203a68b2a9173d8e19b42fc39e5f02f17f1db03c1a06e3fa1c66f4dd7
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **21.6 MB (21563612 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:23b804da420476b5cbcc59bdd26e354e8fa44e4dfe20caf3ac84768dd143b5f2`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Thu, 17 Dec 2020 00:48:11 GMT
COPY file:cd6264d9a7514a8fbc3eb7b400566d36178794d2b757959812cc3abc6f13a97b in /etc/ssl/certs/ 
# Thu, 17 Dec 2020 00:48:11 GMT
COPY dir:83da415af0ff24b3b9d10f857aa8c724a3bc93523f3e047b827e7554fe1f9e08 in /usr/share/ 
# Thu, 17 Dec 2020 00:48:12 GMT
COPY file:8e3cf7c133ac957e81d3eb831160ad827bfde058f356d7ac234b8c5ae307e37a in / 
# Thu, 17 Dec 2020 00:48:12 GMT
EXPOSE 80
# Thu, 17 Dec 2020 00:48:13 GMT
VOLUME [/tmp]
# Thu, 17 Dec 2020 00:48:13 GMT
ENTRYPOINT ["/traefik"]
# Thu, 17 Dec 2020 00:48:13 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.26 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:eca797b3e2d2ac9c3925e07a34654011a4314302362ca0dfe8320d4425bf01f5`  
		Last Modified: Thu, 17 Dec 2020 00:49:22 GMT  
		Size: 21.1 MB (21126329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v1.7` - linux; arm variant v6

```console
$ docker pull traefik@sha256:bb041f9232284130c3646cd4f0d83e032b078ae88a9ab88ea46580df2ee0b991
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **20.2 MB (20210272 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4c618c098e7b6182b45a63ffa8f49bb1656407fb6b666da85775efb87264cf12`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Thu, 17 Dec 2020 00:26:47 GMT
COPY file:cd6264d9a7514a8fbc3eb7b400566d36178794d2b757959812cc3abc6f13a97b in /etc/ssl/certs/ 
# Thu, 17 Dec 2020 00:26:48 GMT
COPY dir:83da415af0ff24b3b9d10f857aa8c724a3bc93523f3e047b827e7554fe1f9e08 in /usr/share/ 
# Thu, 17 Dec 2020 00:26:52 GMT
COPY file:a02ffe991352ee1f8abb077135ea9d27557e8b364fb712a42ccb2865e08df3cc in / 
# Thu, 17 Dec 2020 00:26:53 GMT
EXPOSE 80
# Thu, 17 Dec 2020 00:26:54 GMT
VOLUME [/tmp]
# Thu, 17 Dec 2020 00:26:56 GMT
ENTRYPOINT ["/traefik"]
# Thu, 17 Dec 2020 00:26:57 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.26 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:decc75cc844d668e21a715048cd9c78f2804e625a910fe5568e174c89bd5d8ab`  
		Last Modified: Thu, 17 Dec 2020 00:28:49 GMT  
		Size: 19.8 MB (19772941 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v1.7` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:2dc4a89841d24667bf689a0386eed1525cfe92afd4847039d73204d17e8d77f6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **19.9 MB (19930321 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5993443e6d894e7f4a83e79f4ede7636a3c8b57e7dca57a2dac980bed5a48274`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Thu, 17 Dec 2020 00:27:56 GMT
COPY file:cd6264d9a7514a8fbc3eb7b400566d36178794d2b757959812cc3abc6f13a97b in /etc/ssl/certs/ 
# Thu, 17 Dec 2020 00:27:58 GMT
COPY dir:83da415af0ff24b3b9d10f857aa8c724a3bc93523f3e047b827e7554fe1f9e08 in /usr/share/ 
# Thu, 17 Dec 2020 00:27:59 GMT
COPY file:f592954af2951d1a2538b1945366cb995f49638c7ef8b561b6961e0f8023197a in / 
# Thu, 17 Dec 2020 00:28:00 GMT
EXPOSE 80
# Thu, 17 Dec 2020 00:28:01 GMT
VOLUME [/tmp]
# Thu, 17 Dec 2020 00:28:02 GMT
ENTRYPOINT ["/traefik"]
# Thu, 17 Dec 2020 00:28:03 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.26 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:eda38820bf6e08ea342d37563cf7e4c258c772d4a0576588e8a451209a4534b2`  
		Last Modified: Thu, 17 Dec 2020 00:30:01 GMT  
		Size: 19.5 MB (19492982 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v1.7.26`

```console
$ docker pull traefik@sha256:9a53d5dff2c5b474a8560a4af129cc7863fb8932f8bd0e6896f4292445a2bf86
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:v1.7.26` - linux; amd64

```console
$ docker pull traefik@sha256:78a0311203a68b2a9173d8e19b42fc39e5f02f17f1db03c1a06e3fa1c66f4dd7
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **21.6 MB (21563612 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:23b804da420476b5cbcc59bdd26e354e8fa44e4dfe20caf3ac84768dd143b5f2`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Thu, 17 Dec 2020 00:48:11 GMT
COPY file:cd6264d9a7514a8fbc3eb7b400566d36178794d2b757959812cc3abc6f13a97b in /etc/ssl/certs/ 
# Thu, 17 Dec 2020 00:48:11 GMT
COPY dir:83da415af0ff24b3b9d10f857aa8c724a3bc93523f3e047b827e7554fe1f9e08 in /usr/share/ 
# Thu, 17 Dec 2020 00:48:12 GMT
COPY file:8e3cf7c133ac957e81d3eb831160ad827bfde058f356d7ac234b8c5ae307e37a in / 
# Thu, 17 Dec 2020 00:48:12 GMT
EXPOSE 80
# Thu, 17 Dec 2020 00:48:13 GMT
VOLUME [/tmp]
# Thu, 17 Dec 2020 00:48:13 GMT
ENTRYPOINT ["/traefik"]
# Thu, 17 Dec 2020 00:48:13 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.26 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:eca797b3e2d2ac9c3925e07a34654011a4314302362ca0dfe8320d4425bf01f5`  
		Last Modified: Thu, 17 Dec 2020 00:49:22 GMT  
		Size: 21.1 MB (21126329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v1.7.26` - linux; arm variant v6

```console
$ docker pull traefik@sha256:bb041f9232284130c3646cd4f0d83e032b078ae88a9ab88ea46580df2ee0b991
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **20.2 MB (20210272 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4c618c098e7b6182b45a63ffa8f49bb1656407fb6b666da85775efb87264cf12`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Thu, 17 Dec 2020 00:26:47 GMT
COPY file:cd6264d9a7514a8fbc3eb7b400566d36178794d2b757959812cc3abc6f13a97b in /etc/ssl/certs/ 
# Thu, 17 Dec 2020 00:26:48 GMT
COPY dir:83da415af0ff24b3b9d10f857aa8c724a3bc93523f3e047b827e7554fe1f9e08 in /usr/share/ 
# Thu, 17 Dec 2020 00:26:52 GMT
COPY file:a02ffe991352ee1f8abb077135ea9d27557e8b364fb712a42ccb2865e08df3cc in / 
# Thu, 17 Dec 2020 00:26:53 GMT
EXPOSE 80
# Thu, 17 Dec 2020 00:26:54 GMT
VOLUME [/tmp]
# Thu, 17 Dec 2020 00:26:56 GMT
ENTRYPOINT ["/traefik"]
# Thu, 17 Dec 2020 00:26:57 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.26 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:decc75cc844d668e21a715048cd9c78f2804e625a910fe5568e174c89bd5d8ab`  
		Last Modified: Thu, 17 Dec 2020 00:28:49 GMT  
		Size: 19.8 MB (19772941 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v1.7.26` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:2dc4a89841d24667bf689a0386eed1525cfe92afd4847039d73204d17e8d77f6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **19.9 MB (19930321 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5993443e6d894e7f4a83e79f4ede7636a3c8b57e7dca57a2dac980bed5a48274`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Thu, 17 Dec 2020 00:27:56 GMT
COPY file:cd6264d9a7514a8fbc3eb7b400566d36178794d2b757959812cc3abc6f13a97b in /etc/ssl/certs/ 
# Thu, 17 Dec 2020 00:27:58 GMT
COPY dir:83da415af0ff24b3b9d10f857aa8c724a3bc93523f3e047b827e7554fe1f9e08 in /usr/share/ 
# Thu, 17 Dec 2020 00:27:59 GMT
COPY file:f592954af2951d1a2538b1945366cb995f49638c7ef8b561b6961e0f8023197a in / 
# Thu, 17 Dec 2020 00:28:00 GMT
EXPOSE 80
# Thu, 17 Dec 2020 00:28:01 GMT
VOLUME [/tmp]
# Thu, 17 Dec 2020 00:28:02 GMT
ENTRYPOINT ["/traefik"]
# Thu, 17 Dec 2020 00:28:03 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.26 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:eda38820bf6e08ea342d37563cf7e4c258c772d4a0576588e8a451209a4534b2`  
		Last Modified: Thu, 17 Dec 2020 00:30:01 GMT  
		Size: 19.5 MB (19492982 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v1.7.26-alpine`

```console
$ docker pull traefik@sha256:07dce138fe44640f0c52b2f7f4fb2e92fb508ded8ae57f9a7e0fe8fdf6296673
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:v1.7.26-alpine` - linux; amd64

```console
$ docker pull traefik@sha256:8759aaeb837cdbbe7d39771b1442b99b182fd9556d0dfa02a4b21d254e125f9e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **24.6 MB (24613437 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6ec9aa2ea8436603df821232711432fc2de244aa083c03e3a23e002cac95549d`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 17 Dec 2020 00:19:49 GMT
ADD file:8ed80010e443da19d72546bcee9a35e0a8d244c72052b1994610bf5939d479c2 in / 
# Thu, 17 Dec 2020 00:19:49 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 00:47:33 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 17 Dec 2020 00:47:52 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/containous/traefik/releases/download/v1.7.26/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Thu, 17 Dec 2020 00:47:52 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 17 Dec 2020 00:47:52 GMT
EXPOSE 80
# Thu, 17 Dec 2020 00:47:52 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 17 Dec 2020 00:47:52 GMT
CMD ["traefik"]
# Thu, 17 Dec 2020 00:47:53 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.26 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:2d44f2e7e74e6943c5aac9ce858b295c6f31e2a0c129a718429a4a99ac1bc23d`  
		Last Modified: Thu, 17 Dec 2020 00:49:08 GMT  
		Size: 21.1 MB (21126507 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ca74d371d4ade4d81c1a76a8c789abb59c301c9b73488bfc9d0b40d3003eddf`  
		Last Modified: Thu, 17 Dec 2020 00:49:05 GMT  
		Size: 369.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v1.7.26-alpine` - linux; arm variant v6

```console
$ docker pull traefik@sha256:0494095125ba05e297b154e0827115ae0618b70d40ccce4b1c496ce1666ce43d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.1 MB (23069021 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b6d3de75d11f16c38ae16a31868fe6680c4f4f196bcab0eab4ca1f85c3d9d6f0`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 16 Dec 2020 23:49:53 GMT
ADD file:e3a6f7566ee3c2ba61d27d801d3522e045a4be64a42f32ee52d933b68338d06f in / 
# Wed, 16 Dec 2020 23:49:55 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 00:25:55 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 17 Dec 2020 00:26:33 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/containous/traefik/releases/download/v1.7.26/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Thu, 17 Dec 2020 00:26:34 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 17 Dec 2020 00:26:35 GMT
EXPOSE 80
# Thu, 17 Dec 2020 00:26:36 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 17 Dec 2020 00:26:37 GMT
CMD ["traefik"]
# Thu, 17 Dec 2020 00:26:39 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.26 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:8bed822566f883c529e4423ed5efb201104f66147671cd72a5a80db2e5609dce`  
		Last Modified: Thu, 17 Dec 2020 00:28:20 GMT  
		Size: 19.8 MB (19772981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a46c867ecec8c478367249ed7ccc513e1c496aa5d628bd9950ed8ad87e604f4d`  
		Last Modified: Thu, 17 Dec 2020 00:28:14 GMT  
		Size: 369.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v1.7.26-alpine` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:91c6f4a7270971b010691e5a21e487ac6d85bfbb85b83237a02dfb5c82f35055
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **22.9 MB (22891964 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f3f47993d5e498f1e77ebd9467c190b17085ea5862b5fb1049ebbaf278fcd434`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 16 Dec 2020 23:40:37 GMT
ADD file:47bb1b85a4eb4d0b355ae89ec5c71c09e2c2b7e21e1851a2896365eb17134f57 in / 
# Wed, 16 Dec 2020 23:40:39 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 00:27:02 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 17 Dec 2020 00:27:42 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/containous/traefik/releases/download/v1.7.26/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Thu, 17 Dec 2020 00:27:43 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 17 Dec 2020 00:27:44 GMT
EXPOSE 80
# Thu, 17 Dec 2020 00:27:45 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 17 Dec 2020 00:27:46 GMT
CMD ["traefik"]
# Thu, 17 Dec 2020 00:27:47 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.26 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:6be00c7721dc4a904b3531bfb7878ea6761d57116b3730c05eac3cb31e726a7e`  
		Last Modified: Thu, 17 Dec 2020 00:29:37 GMT  
		Size: 19.5 MB (19493133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37d0080e4ada531446b01e45e014d2c9983281dc58b873e4162e1adb99b6f3ad`  
		Last Modified: Thu, 17 Dec 2020 00:29:20 GMT  
		Size: 369.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v1.7.26-windowsservercore-1809`

```console
$ docker pull traefik@sha256:2c85e3865465339ff28a47a1511b774491ef43ee5c10e9fce0eed4512dca8e84
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1637; amd64

### `traefik:v1.7.26-windowsservercore-1809` - windows version 10.0.17763.1637; amd64

```console
$ docker pull traefik@sha256:ecf2dd6f2cebbfdae3bd25b7ba2a68fea62a623ad337bc401dbfbff0ff03f48f
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2421243323 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c7ae3b3576f87d9dba1f675160af62a993ec7e3a322ac90f9f258497a933fef0`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 04 Dec 2020 02:13:01 GMT
RUN Install update 1809-amd64
# Wed, 09 Dec 2020 13:30:16 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Dec 2020 23:59:07 GMT
RUN Invoke-WebRequest     -Uri "https://github.com/containous/traefik/releases/download/v1.7.26/traefik_windows-amd64.exe"     -OutFile "/traefik.exe"
# Wed, 09 Dec 2020 23:59:09 GMT
EXPOSE 80
# Wed, 09 Dec 2020 23:59:10 GMT
ENTRYPOINT ["/traefik"]
# Wed, 09 Dec 2020 23:59:11 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.26 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:aa4f58cd6da1aaf1a0b44d443bd88e7fbe5b0a6f193995a1a61d6bd63990f314`  
		Size: 672.5 MB (672541583 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a4372d14958dc8a7eaaace9e4774e7f1db524da5eb4474b5e46738848a3a61a5`  
		Last Modified: Wed, 09 Dec 2020 13:54:38 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34300192a929cc8734d3561486bbf20306f0ddf75c3d405112b40a535022d87e`  
		Last Modified: Thu, 10 Dec 2020 00:00:39 GMT  
		Size: 30.4 MB (30364288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bcea0e9edffb70e9148c20ab78ddd79ecb43d454593638a01c8900035a7dfc9`  
		Last Modified: Thu, 10 Dec 2020 00:00:05 GMT  
		Size: 1.1 KB (1132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a53d2ed509732587fa21d4aad5f1ef27c38a85b71e038e15079a978fa5d3114`  
		Last Modified: Thu, 10 Dec 2020 00:00:05 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4118d174807346b7e443506fd438961205a118f2e545f00d509b2a299a92cc06`  
		Last Modified: Thu, 10 Dec 2020 00:00:05 GMT  
		Size: 1.2 KB (1187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v1.7-alpine`

```console
$ docker pull traefik@sha256:07dce138fe44640f0c52b2f7f4fb2e92fb508ded8ae57f9a7e0fe8fdf6296673
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:v1.7-alpine` - linux; amd64

```console
$ docker pull traefik@sha256:8759aaeb837cdbbe7d39771b1442b99b182fd9556d0dfa02a4b21d254e125f9e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **24.6 MB (24613437 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6ec9aa2ea8436603df821232711432fc2de244aa083c03e3a23e002cac95549d`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 17 Dec 2020 00:19:49 GMT
ADD file:8ed80010e443da19d72546bcee9a35e0a8d244c72052b1994610bf5939d479c2 in / 
# Thu, 17 Dec 2020 00:19:49 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 00:47:33 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 17 Dec 2020 00:47:52 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/containous/traefik/releases/download/v1.7.26/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Thu, 17 Dec 2020 00:47:52 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 17 Dec 2020 00:47:52 GMT
EXPOSE 80
# Thu, 17 Dec 2020 00:47:52 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 17 Dec 2020 00:47:52 GMT
CMD ["traefik"]
# Thu, 17 Dec 2020 00:47:53 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.26 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:2d44f2e7e74e6943c5aac9ce858b295c6f31e2a0c129a718429a4a99ac1bc23d`  
		Last Modified: Thu, 17 Dec 2020 00:49:08 GMT  
		Size: 21.1 MB (21126507 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ca74d371d4ade4d81c1a76a8c789abb59c301c9b73488bfc9d0b40d3003eddf`  
		Last Modified: Thu, 17 Dec 2020 00:49:05 GMT  
		Size: 369.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v1.7-alpine` - linux; arm variant v6

```console
$ docker pull traefik@sha256:0494095125ba05e297b154e0827115ae0618b70d40ccce4b1c496ce1666ce43d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.1 MB (23069021 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b6d3de75d11f16c38ae16a31868fe6680c4f4f196bcab0eab4ca1f85c3d9d6f0`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 16 Dec 2020 23:49:53 GMT
ADD file:e3a6f7566ee3c2ba61d27d801d3522e045a4be64a42f32ee52d933b68338d06f in / 
# Wed, 16 Dec 2020 23:49:55 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 00:25:55 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 17 Dec 2020 00:26:33 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/containous/traefik/releases/download/v1.7.26/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Thu, 17 Dec 2020 00:26:34 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 17 Dec 2020 00:26:35 GMT
EXPOSE 80
# Thu, 17 Dec 2020 00:26:36 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 17 Dec 2020 00:26:37 GMT
CMD ["traefik"]
# Thu, 17 Dec 2020 00:26:39 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.26 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:8bed822566f883c529e4423ed5efb201104f66147671cd72a5a80db2e5609dce`  
		Last Modified: Thu, 17 Dec 2020 00:28:20 GMT  
		Size: 19.8 MB (19772981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a46c867ecec8c478367249ed7ccc513e1c496aa5d628bd9950ed8ad87e604f4d`  
		Last Modified: Thu, 17 Dec 2020 00:28:14 GMT  
		Size: 369.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v1.7-alpine` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:91c6f4a7270971b010691e5a21e487ac6d85bfbb85b83237a02dfb5c82f35055
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **22.9 MB (22891964 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f3f47993d5e498f1e77ebd9467c190b17085ea5862b5fb1049ebbaf278fcd434`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 16 Dec 2020 23:40:37 GMT
ADD file:47bb1b85a4eb4d0b355ae89ec5c71c09e2c2b7e21e1851a2896365eb17134f57 in / 
# Wed, 16 Dec 2020 23:40:39 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 00:27:02 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 17 Dec 2020 00:27:42 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/containous/traefik/releases/download/v1.7.26/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Thu, 17 Dec 2020 00:27:43 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 17 Dec 2020 00:27:44 GMT
EXPOSE 80
# Thu, 17 Dec 2020 00:27:45 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 17 Dec 2020 00:27:46 GMT
CMD ["traefik"]
# Thu, 17 Dec 2020 00:27:47 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.26 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:6be00c7721dc4a904b3531bfb7878ea6761d57116b3730c05eac3cb31e726a7e`  
		Last Modified: Thu, 17 Dec 2020 00:29:37 GMT  
		Size: 19.5 MB (19493133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37d0080e4ada531446b01e45e014d2c9983281dc58b873e4162e1adb99b6f3ad`  
		Last Modified: Thu, 17 Dec 2020 00:29:20 GMT  
		Size: 369.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v1.7-windowsservercore-1809`

```console
$ docker pull traefik@sha256:2c85e3865465339ff28a47a1511b774491ef43ee5c10e9fce0eed4512dca8e84
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1637; amd64

### `traefik:v1.7-windowsservercore-1809` - windows version 10.0.17763.1637; amd64

```console
$ docker pull traefik@sha256:ecf2dd6f2cebbfdae3bd25b7ba2a68fea62a623ad337bc401dbfbff0ff03f48f
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2421243323 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c7ae3b3576f87d9dba1f675160af62a993ec7e3a322ac90f9f258497a933fef0`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 04 Dec 2020 02:13:01 GMT
RUN Install update 1809-amd64
# Wed, 09 Dec 2020 13:30:16 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Dec 2020 23:59:07 GMT
RUN Invoke-WebRequest     -Uri "https://github.com/containous/traefik/releases/download/v1.7.26/traefik_windows-amd64.exe"     -OutFile "/traefik.exe"
# Wed, 09 Dec 2020 23:59:09 GMT
EXPOSE 80
# Wed, 09 Dec 2020 23:59:10 GMT
ENTRYPOINT ["/traefik"]
# Wed, 09 Dec 2020 23:59:11 GMT
LABEL org.opencontainers.image.vendor=Containous org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.26 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:aa4f58cd6da1aaf1a0b44d443bd88e7fbe5b0a6f193995a1a61d6bd63990f314`  
		Size: 672.5 MB (672541583 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a4372d14958dc8a7eaaace9e4774e7f1db524da5eb4474b5e46738848a3a61a5`  
		Last Modified: Wed, 09 Dec 2020 13:54:38 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34300192a929cc8734d3561486bbf20306f0ddf75c3d405112b40a535022d87e`  
		Last Modified: Thu, 10 Dec 2020 00:00:39 GMT  
		Size: 30.4 MB (30364288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bcea0e9edffb70e9148c20ab78ddd79ecb43d454593638a01c8900035a7dfc9`  
		Last Modified: Thu, 10 Dec 2020 00:00:05 GMT  
		Size: 1.1 KB (1132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a53d2ed509732587fa21d4aad5f1ef27c38a85b71e038e15079a978fa5d3114`  
		Last Modified: Thu, 10 Dec 2020 00:00:05 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4118d174807346b7e443506fd438961205a118f2e545f00d509b2a299a92cc06`  
		Last Modified: Thu, 10 Dec 2020 00:00:05 GMT  
		Size: 1.2 KB (1187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v2.3`

```console
$ docker pull traefik@sha256:6329d060190998d5c9a85f9b812177601a753dc32094195d4e5efbd6bd8f191d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:v2.3` - linux; amd64

```console
$ docker pull traefik@sha256:d8faddf331546aca9cfec4091185ef6f0f7654246f5f0656ff5ef53eeae7fd18
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.4 MB (28385315 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:54db2e08f87e0483ab129ec7e400baa38d3616d4821640abbfa740c9398ad864`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 17 Dec 2020 00:19:49 GMT
ADD file:8ed80010e443da19d72546bcee9a35e0a8d244c72052b1994610bf5939d479c2 in / 
# Thu, 17 Dec 2020 00:19:49 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 00:47:33 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 17 Dec 2020 00:47:44 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.3.5/traefik_v2.3.5_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 17 Dec 2020 00:47:44 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 17 Dec 2020 00:47:44 GMT
EXPOSE 80
# Thu, 17 Dec 2020 00:47:45 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 17 Dec 2020 00:47:45 GMT
CMD ["traefik"]
# Thu, 17 Dec 2020 00:47:45 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.3.5 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:9317c0d35096c63079779d328115613d4408f9c4be4c93e3a67fd2631b160854`  
		Last Modified: Thu, 17 Dec 2020 00:48:55 GMT  
		Size: 24.9 MB (24898385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c262a5be356023fa84388e766cd12952112ad0805c10d1316483fd465b668e1`  
		Last Modified: Thu, 17 Dec 2020 00:48:50 GMT  
		Size: 369.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v2.3` - linux; arm variant v6

```console
$ docker pull traefik@sha256:200709b0233fee1951b48edabee5f71c4c143c6883f19349cbeec2fe830d4222
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.5 MB (26482700 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:38d6a862b01e1d5a6b608926e2b099151560a2d809398e048f1ab8987d6913e2`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 16 Dec 2020 23:49:53 GMT
ADD file:e3a6f7566ee3c2ba61d27d801d3522e045a4be64a42f32ee52d933b68338d06f in / 
# Wed, 16 Dec 2020 23:49:55 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 00:25:55 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 17 Dec 2020 00:26:15 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.3.5/traefik_v2.3.5_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 17 Dec 2020 00:26:17 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 17 Dec 2020 00:26:18 GMT
EXPOSE 80
# Thu, 17 Dec 2020 00:26:18 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 17 Dec 2020 00:26:19 GMT
CMD ["traefik"]
# Thu, 17 Dec 2020 00:26:20 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.3.5 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:708a31fe0f367f038f8442997d0200a64291d57caa1d8fcbf8ca6a7bfdeaeab9`  
		Last Modified: Thu, 17 Dec 2020 00:28:01 GMT  
		Size: 23.2 MB (23186660 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff140dbd5ae36d65c765bcdb73f2bfb095918f404c9421eda0b4217f86af0101`  
		Last Modified: Thu, 17 Dec 2020 00:27:53 GMT  
		Size: 369.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v2.3` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:a41ad437600dbfefbdf4bd0c89a6dbe6f178be4f693f1a18d28517fbbe4cf32b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.1 MB (26097249 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1eaf2b0865bc3065f86245d528f1881d0122b7d792620dcbd7f45ff4b4bb060f`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 16 Dec 2020 23:40:37 GMT
ADD file:47bb1b85a4eb4d0b355ae89ec5c71c09e2c2b7e21e1851a2896365eb17134f57 in / 
# Wed, 16 Dec 2020 23:40:39 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 00:27:02 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 17 Dec 2020 00:27:25 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.3.5/traefik_v2.3.5_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 17 Dec 2020 00:27:26 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 17 Dec 2020 00:27:28 GMT
EXPOSE 80
# Thu, 17 Dec 2020 00:27:29 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 17 Dec 2020 00:27:30 GMT
CMD ["traefik"]
# Thu, 17 Dec 2020 00:27:31 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.3.5 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:6e25b961f24a55c5614ba4272f7197b1a40e24999c3113f7a63bafea52304451`  
		Last Modified: Thu, 17 Dec 2020 00:29:06 GMT  
		Size: 22.7 MB (22698418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1383e7238dfb4d957a85710afdfd6389bda4310df784820d996d0d034dabb2c1`  
		Last Modified: Thu, 17 Dec 2020 00:28:58 GMT  
		Size: 369.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v2.3.6`

**does not exist** (yet?)

## `traefik:v2.3.6-windowsservercore-1809`

**does not exist** (yet?)

## `traefik:v2.3-windowsservercore-1809`

```console
$ docker pull traefik@sha256:e00168af8fd06c5db5810991b63ae9bc32f624cb574998cbe7705bf171d2575b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1637; amd64

### `traefik:v2.3-windowsservercore-1809` - windows version 10.0.17763.1637; amd64

```console
$ docker pull traefik@sha256:c86e24a0e106ce1187d55f8ef015cc038ac6fb238890bb24e0e6534752c41075
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2425379374 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b35eb3df56ce0eafb6242f83b0c7170bf0496cd8e220d64148de4c270112992e`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 04 Dec 2020 02:13:01 GMT
RUN Install update 1809-amd64
# Wed, 09 Dec 2020 13:30:16 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Fri, 11 Dec 2020 01:45:44 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/traefik/traefik/releases/download/v2.3.5/traefik_v2.3.5_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Fri, 11 Dec 2020 01:45:48 GMT
EXPOSE 80
# Fri, 11 Dec 2020 01:45:48 GMT
ENTRYPOINT ["/traefik"]
# Fri, 11 Dec 2020 01:45:49 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.3.5 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:aa4f58cd6da1aaf1a0b44d443bd88e7fbe5b0a6f193995a1a61d6bd63990f314`  
		Size: 672.5 MB (672541583 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a4372d14958dc8a7eaaace9e4774e7f1db524da5eb4474b5e46738848a3a61a5`  
		Last Modified: Wed, 09 Dec 2020 13:54:38 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85482ae30bb6c78ecdd6711396f28c8e7d825b0b2fdc5d98b4b7ef1fa55c058a`  
		Last Modified: Fri, 11 Dec 2020 01:46:23 GMT  
		Size: 34.5 MB (34500366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:235692d5c0973ec6d5f726c71422568cbc87ccd6fef238182d05e58450b1a2a8`  
		Last Modified: Fri, 11 Dec 2020 01:46:14 GMT  
		Size: 1.2 KB (1156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5f09935d359b99a157f3caae523bb65efd1975c0d56175dc692646a7262ab6c`  
		Last Modified: Fri, 11 Dec 2020 01:46:14 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ba9ec09cdbc0f0266e3781e8e9d1a12f5440b6847485d9a4f0a20e69579750b`  
		Last Modified: Fri, 11 Dec 2020 01:46:15 GMT  
		Size: 1.1 KB (1132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v2.4`

```console
$ docker pull traefik@sha256:7d8a40698784af9bc56591e7402378deccc31df8ef51f6e09a7e0f4afa1787c1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:v2.4` - linux; amd64

```console
$ docker pull traefik@sha256:e72173181d61d6d38147617dc8932f18913eef9b8b016590c987c9601df7156f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.1 MB (29072354 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:77adf581ab54982c064a76d40ab167586a222980aa9818458208cdb9761363fa`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 17 Dec 2020 00:19:49 GMT
ADD file:8ed80010e443da19d72546bcee9a35e0a8d244c72052b1994610bf5939d479c2 in / 
# Thu, 17 Dec 2020 00:19:49 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 00:47:33 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 17 Dec 2020 00:47:36 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.4.0-rc1/traefik_v2.4.0-rc1_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 17 Dec 2020 00:47:36 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 17 Dec 2020 00:47:36 GMT
EXPOSE 80
# Thu, 17 Dec 2020 00:47:36 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 17 Dec 2020 00:47:37 GMT
CMD ["traefik"]
# Thu, 17 Dec 2020 00:47:37 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.4.0-rc1 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:6348b818709856ced463f120a41e43ce15a035508e8cefd7ffcfe67295a783ed`  
		Last Modified: Thu, 17 Dec 2020 00:48:42 GMT  
		Size: 25.6 MB (25585425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc293a73c224168214a62f4c533ab7995c8744665c887eb0a797b53f125dbd60`  
		Last Modified: Thu, 17 Dec 2020 00:48:36 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v2.4` - linux; arm variant v6

```console
$ docker pull traefik@sha256:0464505a5542f0c35a80906488d4f17acc8bc062ac5480abcdba5961e85dedef
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.1 MB (27107202 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0a44b18ddf6ab462a4af8dbedfb58eaca6b7002622164563c3c18128b35078e4`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 16 Dec 2020 23:49:53 GMT
ADD file:e3a6f7566ee3c2ba61d27d801d3522e045a4be64a42f32ee52d933b68338d06f in / 
# Wed, 16 Dec 2020 23:49:55 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 00:25:55 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 17 Dec 2020 00:26:00 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.4.0-rc1/traefik_v2.4.0-rc1_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 17 Dec 2020 00:26:01 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 17 Dec 2020 00:26:02 GMT
EXPOSE 80
# Thu, 17 Dec 2020 00:26:02 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 17 Dec 2020 00:26:03 GMT
CMD ["traefik"]
# Thu, 17 Dec 2020 00:26:04 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.4.0-rc1 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:71a89144d2ec5013a820f4de949514c963d60f1eafac95fc5c0626ac3a5fca49`  
		Last Modified: Thu, 17 Dec 2020 00:27:32 GMT  
		Size: 23.8 MB (23811162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6633878abde02f77de69e78a3868c33a28300c0c47a47f81297473d9186bd156`  
		Last Modified: Thu, 17 Dec 2020 00:27:24 GMT  
		Size: 369.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v2.4` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:e1975275fbaf78b62a8a588b67d3ea3b72acc9ffcd47176cb4e987acf3f73c13
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.7 MB (26736293 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4646b0137cf051fe81afc86b698d2d8849446adda9ab81c8871f01b8c2e52d94`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 16 Dec 2020 23:40:37 GMT
ADD file:47bb1b85a4eb4d0b355ae89ec5c71c09e2c2b7e21e1851a2896365eb17134f57 in / 
# Wed, 16 Dec 2020 23:40:39 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 00:27:02 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 17 Dec 2020 00:27:08 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.4.0-rc1/traefik_v2.4.0-rc1_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 17 Dec 2020 00:27:09 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 17 Dec 2020 00:27:10 GMT
EXPOSE 80
# Thu, 17 Dec 2020 00:27:11 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 17 Dec 2020 00:27:12 GMT
CMD ["traefik"]
# Thu, 17 Dec 2020 00:27:13 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.4.0-rc1 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:a8c978289529e0d75adc45110a61b13d8d3791c39eda7bc74272d02afce9d584`  
		Last Modified: Thu, 17 Dec 2020 00:28:46 GMT  
		Size: 23.3 MB (23337462 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ade89e86f523ff8f8f95973a320cd860a913d5aac0df71602635b88f488a3567`  
		Last Modified: Thu, 17 Dec 2020 00:28:38 GMT  
		Size: 369.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v2.4.0-rc1`

```console
$ docker pull traefik@sha256:7d8a40698784af9bc56591e7402378deccc31df8ef51f6e09a7e0f4afa1787c1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:v2.4.0-rc1` - linux; amd64

```console
$ docker pull traefik@sha256:e72173181d61d6d38147617dc8932f18913eef9b8b016590c987c9601df7156f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.1 MB (29072354 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:77adf581ab54982c064a76d40ab167586a222980aa9818458208cdb9761363fa`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 17 Dec 2020 00:19:49 GMT
ADD file:8ed80010e443da19d72546bcee9a35e0a8d244c72052b1994610bf5939d479c2 in / 
# Thu, 17 Dec 2020 00:19:49 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 00:47:33 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 17 Dec 2020 00:47:36 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.4.0-rc1/traefik_v2.4.0-rc1_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 17 Dec 2020 00:47:36 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 17 Dec 2020 00:47:36 GMT
EXPOSE 80
# Thu, 17 Dec 2020 00:47:36 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 17 Dec 2020 00:47:37 GMT
CMD ["traefik"]
# Thu, 17 Dec 2020 00:47:37 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.4.0-rc1 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:6348b818709856ced463f120a41e43ce15a035508e8cefd7ffcfe67295a783ed`  
		Last Modified: Thu, 17 Dec 2020 00:48:42 GMT  
		Size: 25.6 MB (25585425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc293a73c224168214a62f4c533ab7995c8744665c887eb0a797b53f125dbd60`  
		Last Modified: Thu, 17 Dec 2020 00:48:36 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v2.4.0-rc1` - linux; arm variant v6

```console
$ docker pull traefik@sha256:0464505a5542f0c35a80906488d4f17acc8bc062ac5480abcdba5961e85dedef
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.1 MB (27107202 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0a44b18ddf6ab462a4af8dbedfb58eaca6b7002622164563c3c18128b35078e4`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 16 Dec 2020 23:49:53 GMT
ADD file:e3a6f7566ee3c2ba61d27d801d3522e045a4be64a42f32ee52d933b68338d06f in / 
# Wed, 16 Dec 2020 23:49:55 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 00:25:55 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 17 Dec 2020 00:26:00 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.4.0-rc1/traefik_v2.4.0-rc1_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 17 Dec 2020 00:26:01 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 17 Dec 2020 00:26:02 GMT
EXPOSE 80
# Thu, 17 Dec 2020 00:26:02 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 17 Dec 2020 00:26:03 GMT
CMD ["traefik"]
# Thu, 17 Dec 2020 00:26:04 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.4.0-rc1 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:71a89144d2ec5013a820f4de949514c963d60f1eafac95fc5c0626ac3a5fca49`  
		Last Modified: Thu, 17 Dec 2020 00:27:32 GMT  
		Size: 23.8 MB (23811162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6633878abde02f77de69e78a3868c33a28300c0c47a47f81297473d9186bd156`  
		Last Modified: Thu, 17 Dec 2020 00:27:24 GMT  
		Size: 369.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v2.4.0-rc1` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:e1975275fbaf78b62a8a588b67d3ea3b72acc9ffcd47176cb4e987acf3f73c13
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.7 MB (26736293 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4646b0137cf051fe81afc86b698d2d8849446adda9ab81c8871f01b8c2e52d94`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 16 Dec 2020 23:40:37 GMT
ADD file:47bb1b85a4eb4d0b355ae89ec5c71c09e2c2b7e21e1851a2896365eb17134f57 in / 
# Wed, 16 Dec 2020 23:40:39 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 00:27:02 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 17 Dec 2020 00:27:08 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.4.0-rc1/traefik_v2.4.0-rc1_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 17 Dec 2020 00:27:09 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 17 Dec 2020 00:27:10 GMT
EXPOSE 80
# Thu, 17 Dec 2020 00:27:11 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 17 Dec 2020 00:27:12 GMT
CMD ["traefik"]
# Thu, 17 Dec 2020 00:27:13 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.4.0-rc1 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:a8c978289529e0d75adc45110a61b13d8d3791c39eda7bc74272d02afce9d584`  
		Last Modified: Thu, 17 Dec 2020 00:28:46 GMT  
		Size: 23.3 MB (23337462 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ade89e86f523ff8f8f95973a320cd860a913d5aac0df71602635b88f488a3567`  
		Last Modified: Thu, 17 Dec 2020 00:28:38 GMT  
		Size: 369.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v2.4.0-rc1-windowsservercore-1809`

```console
$ docker pull traefik@sha256:c38beba5d61f64ff442e2c8c2e9e7419fb47bdb125b54bbeb0e36b6351d292c1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1637; amd64

### `traefik:v2.4.0-rc1-windowsservercore-1809` - windows version 10.0.17763.1637; amd64

```console
$ docker pull traefik@sha256:5be07f9155301dae81e2580ea435677afb018e22df3250d845d1519d9757c9ab
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2426094285 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:69c5a39fe06b07e4794aeffb43f0a1eb437f5f28937a57f4228c090951b2f84a`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 04 Dec 2020 02:13:01 GMT
RUN Install update 1809-amd64
# Wed, 09 Dec 2020 13:30:16 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 17 Dec 2020 00:16:07 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/traefik/traefik/releases/download/v2.4.0-rc1/traefik_v2.4.0-rc1_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Thu, 17 Dec 2020 00:16:11 GMT
EXPOSE 80
# Thu, 17 Dec 2020 00:16:12 GMT
ENTRYPOINT ["/traefik"]
# Thu, 17 Dec 2020 00:16:13 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.4.0-rc1 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:aa4f58cd6da1aaf1a0b44d443bd88e7fbe5b0a6f193995a1a61d6bd63990f314`  
		Size: 672.5 MB (672541583 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a4372d14958dc8a7eaaace9e4774e7f1db524da5eb4474b5e46738848a3a61a5`  
		Last Modified: Wed, 09 Dec 2020 13:54:38 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54167c9a07bde1e13b39ce2bf3c56eaeb33f6466c6a33624dcf3c713b3697e67`  
		Last Modified: Thu, 17 Dec 2020 00:16:59 GMT  
		Size: 35.2 MB (35215314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd6d21c529f31e5de6bfd8d23955872cee397bd7df6332d69b7b97a899868e44`  
		Last Modified: Thu, 17 Dec 2020 00:16:51 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bbf669e97927e7ae7c8ba2a38289f46ec356ed92b648e920c809bbbf8a78fb1`  
		Last Modified: Thu, 17 Dec 2020 00:16:50 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:769f092fb22a8b9cea7104db10bf8b7085aec60d35a3e9938cc433c5861e3744`  
		Last Modified: Thu, 17 Dec 2020 00:16:51 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v2.4-windowsservercore-1809`

```console
$ docker pull traefik@sha256:c38beba5d61f64ff442e2c8c2e9e7419fb47bdb125b54bbeb0e36b6351d292c1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1637; amd64

### `traefik:v2.4-windowsservercore-1809` - windows version 10.0.17763.1637; amd64

```console
$ docker pull traefik@sha256:5be07f9155301dae81e2580ea435677afb018e22df3250d845d1519d9757c9ab
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2426094285 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:69c5a39fe06b07e4794aeffb43f0a1eb437f5f28937a57f4228c090951b2f84a`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 04 Dec 2020 02:13:01 GMT
RUN Install update 1809-amd64
# Wed, 09 Dec 2020 13:30:16 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 17 Dec 2020 00:16:07 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/traefik/traefik/releases/download/v2.4.0-rc1/traefik_v2.4.0-rc1_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Thu, 17 Dec 2020 00:16:11 GMT
EXPOSE 80
# Thu, 17 Dec 2020 00:16:12 GMT
ENTRYPOINT ["/traefik"]
# Thu, 17 Dec 2020 00:16:13 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.4.0-rc1 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:aa4f58cd6da1aaf1a0b44d443bd88e7fbe5b0a6f193995a1a61d6bd63990f314`  
		Size: 672.5 MB (672541583 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a4372d14958dc8a7eaaace9e4774e7f1db524da5eb4474b5e46738848a3a61a5`  
		Last Modified: Wed, 09 Dec 2020 13:54:38 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54167c9a07bde1e13b39ce2bf3c56eaeb33f6466c6a33624dcf3c713b3697e67`  
		Last Modified: Thu, 17 Dec 2020 00:16:59 GMT  
		Size: 35.2 MB (35215314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd6d21c529f31e5de6bfd8d23955872cee397bd7df6332d69b7b97a899868e44`  
		Last Modified: Thu, 17 Dec 2020 00:16:51 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bbf669e97927e7ae7c8ba2a38289f46ec356ed92b648e920c809bbbf8a78fb1`  
		Last Modified: Thu, 17 Dec 2020 00:16:50 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:769f092fb22a8b9cea7104db10bf8b7085aec60d35a3e9938cc433c5861e3744`  
		Last Modified: Thu, 17 Dec 2020 00:16:51 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:windowsservercore-1809`

```console
$ docker pull traefik@sha256:e00168af8fd06c5db5810991b63ae9bc32f624cb574998cbe7705bf171d2575b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1637; amd64

### `traefik:windowsservercore-1809` - windows version 10.0.17763.1637; amd64

```console
$ docker pull traefik@sha256:c86e24a0e106ce1187d55f8ef015cc038ac6fb238890bb24e0e6534752c41075
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2425379374 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b35eb3df56ce0eafb6242f83b0c7170bf0496cd8e220d64148de4c270112992e`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 04 Dec 2020 02:13:01 GMT
RUN Install update 1809-amd64
# Wed, 09 Dec 2020 13:30:16 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Fri, 11 Dec 2020 01:45:44 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/traefik/traefik/releases/download/v2.3.5/traefik_v2.3.5_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Fri, 11 Dec 2020 01:45:48 GMT
EXPOSE 80
# Fri, 11 Dec 2020 01:45:48 GMT
ENTRYPOINT ["/traefik"]
# Fri, 11 Dec 2020 01:45:49 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.3.5 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:aa4f58cd6da1aaf1a0b44d443bd88e7fbe5b0a6f193995a1a61d6bd63990f314`  
		Size: 672.5 MB (672541583 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a4372d14958dc8a7eaaace9e4774e7f1db524da5eb4474b5e46738848a3a61a5`  
		Last Modified: Wed, 09 Dec 2020 13:54:38 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85482ae30bb6c78ecdd6711396f28c8e7d825b0b2fdc5d98b4b7ef1fa55c058a`  
		Last Modified: Fri, 11 Dec 2020 01:46:23 GMT  
		Size: 34.5 MB (34500366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:235692d5c0973ec6d5f726c71422568cbc87ccd6fef238182d05e58450b1a2a8`  
		Last Modified: Fri, 11 Dec 2020 01:46:14 GMT  
		Size: 1.2 KB (1156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5f09935d359b99a157f3caae523bb65efd1975c0d56175dc692646a7262ab6c`  
		Last Modified: Fri, 11 Dec 2020 01:46:14 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ba9ec09cdbc0f0266e3781e8e9d1a12f5440b6847485d9a4f0a20e69579750b`  
		Last Modified: Fri, 11 Dec 2020 01:46:15 GMT  
		Size: 1.1 KB (1132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
