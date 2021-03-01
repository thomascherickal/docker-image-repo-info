<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `traefik`

-	[`traefik:1.7`](#traefik17)
-	[`traefik:1.7.28`](#traefik1728)
-	[`traefik:1.7.28-alpine`](#traefik1728-alpine)
-	[`traefik:1.7.28-windowsservercore-1809`](#traefik1728-windowsservercore-1809)
-	[`traefik:1.7-alpine`](#traefik17-alpine)
-	[`traefik:1.7-windowsservercore-1809`](#traefik17-windowsservercore-1809)
-	[`traefik:2.4`](#traefik24)
-	[`traefik:2.4.6`](#traefik246)
-	[`traefik:2.4.6-windowsservercore-1809`](#traefik246-windowsservercore-1809)
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
-	[`traefik:v2.4.6`](#traefikv246)
-	[`traefik:v2.4.6-windowsservercore-1809`](#traefikv246-windowsservercore-1809)
-	[`traefik:v2.4-windowsservercore-1809`](#traefikv24-windowsservercore-1809)
-	[`traefik:windowsservercore-1809`](#traefikwindowsservercore-1809)

## `traefik:1.7`

```console
$ docker pull traefik@sha256:6fcc1a5ef1fc56c7e8ef206407f086feffe155edba2b09e8e2ff51903d5a8af1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:1.7` - linux; amd64

```console
$ docker pull traefik@sha256:70a8743d69121fa77b5d561e3c3dd8cdcafe552467d503bfbb70063289aa7f09
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **21.6 MB (21555688 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a0013bcad7721f151cc49a02c90ad1f8bab70f17fd8cb9b39953e18e251395d6`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Thu, 17 Dec 2020 00:48:11 GMT
COPY file:cd6264d9a7514a8fbc3eb7b400566d36178794d2b757959812cc3abc6f13a97b in /etc/ssl/certs/ 
# Thu, 25 Feb 2021 03:24:27 GMT
COPY dir:379603788862c2a6c57432d70b0a67f561fe00310e1b958c9ecf85381b1c9cd9 in /usr/share/ 
# Thu, 25 Feb 2021 03:24:29 GMT
COPY file:94b9997cc55c7732c9fc173c119f980e4a38eba20b96a90170a3d7fade75f0eb in / 
# Thu, 25 Feb 2021 03:24:29 GMT
EXPOSE 80
# Thu, 25 Feb 2021 03:24:29 GMT
VOLUME [/tmp]
# Thu, 25 Feb 2021 03:24:29 GMT
ENTRYPOINT ["/traefik"]
# Thu, 25 Feb 2021 03:24:30 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.28 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:79de75e85675fa9abbac17b57205d3e0dfcf2bd2fc4cbc194f2aaf917435425e`  
		Last Modified: Thu, 17 Dec 2020 00:49:17 GMT  
		Size: 130.9 KB (130872 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07ccc62f6df1194af0864cbbff567afef1c70d510c6bc4c8e101c6e64def6d70`  
		Last Modified: Thu, 25 Feb 2021 03:25:24 GMT  
		Size: 308.8 KB (308817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff9e7c6f1cdda4e2fd24a670a1af35baae7f2b51de21646bb8088636362f47c5`  
		Last Modified: Thu, 25 Feb 2021 03:25:30 GMT  
		Size: 21.1 MB (21115999 bytes)  
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

## `traefik:1.7.28`

```console
$ docker pull traefik@sha256:6fcc1a5ef1fc56c7e8ef206407f086feffe155edba2b09e8e2ff51903d5a8af1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:1.7.28` - linux; amd64

```console
$ docker pull traefik@sha256:70a8743d69121fa77b5d561e3c3dd8cdcafe552467d503bfbb70063289aa7f09
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **21.6 MB (21555688 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a0013bcad7721f151cc49a02c90ad1f8bab70f17fd8cb9b39953e18e251395d6`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Thu, 17 Dec 2020 00:48:11 GMT
COPY file:cd6264d9a7514a8fbc3eb7b400566d36178794d2b757959812cc3abc6f13a97b in /etc/ssl/certs/ 
# Thu, 25 Feb 2021 03:24:27 GMT
COPY dir:379603788862c2a6c57432d70b0a67f561fe00310e1b958c9ecf85381b1c9cd9 in /usr/share/ 
# Thu, 25 Feb 2021 03:24:29 GMT
COPY file:94b9997cc55c7732c9fc173c119f980e4a38eba20b96a90170a3d7fade75f0eb in / 
# Thu, 25 Feb 2021 03:24:29 GMT
EXPOSE 80
# Thu, 25 Feb 2021 03:24:29 GMT
VOLUME [/tmp]
# Thu, 25 Feb 2021 03:24:29 GMT
ENTRYPOINT ["/traefik"]
# Thu, 25 Feb 2021 03:24:30 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.28 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:79de75e85675fa9abbac17b57205d3e0dfcf2bd2fc4cbc194f2aaf917435425e`  
		Last Modified: Thu, 17 Dec 2020 00:49:17 GMT  
		Size: 130.9 KB (130872 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07ccc62f6df1194af0864cbbff567afef1c70d510c6bc4c8e101c6e64def6d70`  
		Last Modified: Thu, 25 Feb 2021 03:25:24 GMT  
		Size: 308.8 KB (308817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff9e7c6f1cdda4e2fd24a670a1af35baae7f2b51de21646bb8088636362f47c5`  
		Last Modified: Thu, 25 Feb 2021 03:25:30 GMT  
		Size: 21.1 MB (21115999 bytes)  
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
$ docker pull traefik@sha256:f8aa3bcee0d52f8101d2179ed61d34141d263bf2320ceef88ff77e986025a791
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:1.7.28-alpine` - linux; amd64

```console
$ docker pull traefik@sha256:0dcaa21539f6a679eeec2235ef295bf52dc618802a2b86c2bd8f54fb0f918a66
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **24.6 MB (24606031 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3a53b1b425aa4bbaea25bf86763df668237f6261464995a72d1f413b6b8b23ee`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 24 Feb 2021 20:20:11 GMT
ADD file:7eeea546ecde7a036bf634c08719879d32c7ec6ae599708cd91dc1b830735223 in / 
# Wed, 24 Feb 2021 20:20:12 GMT
CMD ["/bin/sh"]
# Thu, 25 Feb 2021 03:23:41 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 25 Feb 2021 03:23:56 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/traefik/traefik/releases/download/v1.7.28/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Thu, 25 Feb 2021 03:23:56 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 25 Feb 2021 03:23:56 GMT
EXPOSE 80
# Thu, 25 Feb 2021 03:23:57 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 25 Feb 2021 03:23:57 GMT
CMD ["traefik"]
# Thu, 25 Feb 2021 03:23:57 GMT
LABEL org.opencontainers.image.vendor=traefik org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.28 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:e95f33c60a645d6d31f52fdc334aecec0d79a1b410789eae37fbf69efcd587ab`  
		Last Modified: Wed, 24 Feb 2021 20:20:43 GMT  
		Size: 2.8 MB (2815313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7caf618c71a94b64d99880ac96da93c76a3931b35dffe57842d5baa964afbb3`  
		Last Modified: Thu, 25 Feb 2021 03:24:54 GMT  
		Size: 674.1 KB (674094 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d86caf1517f080a3c9e8645f69c08191a124a38c59e3c657ecee9dd847a1dcc3`  
		Last Modified: Thu, 25 Feb 2021 03:25:16 GMT  
		Size: 21.1 MB (21116257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49dabb83fefe1e371ad0ad76ea6523ffd2a4e4884a2a88f7e7254bc52dca0000`  
		Last Modified: Thu, 25 Feb 2021 03:25:10 GMT  
		Size: 367.0 B  
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
$ docker pull traefik@sha256:7b6485e1c472dbbe4929740278ebd3a6102f89e5208ad98094f13d366cd7759c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **22.9 MB (22887723 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e433192bfcd73af95a95a11e410a94b1e7792f903ed5b5f89bffd264c1dce2e4`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 24 Feb 2021 20:39:51 GMT
ADD file:f8a47118a2fe92c166c426620bb4ea0090dbf17aed269177989f6dca70438750 in / 
# Wed, 24 Feb 2021 20:39:52 GMT
CMD ["/bin/sh"]
# Thu, 25 Feb 2021 04:18:27 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 25 Feb 2021 04:18:45 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/traefik/traefik/releases/download/v1.7.28/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Thu, 25 Feb 2021 04:18:46 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 25 Feb 2021 04:18:47 GMT
EXPOSE 80
# Thu, 25 Feb 2021 04:18:47 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 25 Feb 2021 04:18:48 GMT
CMD ["traefik"]
# Thu, 25 Feb 2021 04:18:48 GMT
LABEL org.opencontainers.image.vendor=traefik org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.28 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:0328c39aea610966704bee2d2a1c7108816950703f98b4585083cd18f8354380`  
		Last Modified: Wed, 24 Feb 2021 20:40:35 GMT  
		Size: 2.7 MB (2725816 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4961a79823a93d7b581d0d755b544c7ad8e44d35dec7296a3663c7815c9b8e5`  
		Last Modified: Thu, 25 Feb 2021 04:24:33 GMT  
		Size: 675.5 KB (675506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef006d431cee79db31d7d17cf98839851ea3b97f23cff779428c0d801f2e0669`  
		Last Modified: Thu, 25 Feb 2021 04:24:57 GMT  
		Size: 19.5 MB (19486033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a229f0ffeea6995923cfa28b4aa3137adb96ed94f63f8e7fd861c35b76785e2c`  
		Last Modified: Thu, 25 Feb 2021 04:24:51 GMT  
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
$ docker pull traefik@sha256:f8aa3bcee0d52f8101d2179ed61d34141d263bf2320ceef88ff77e986025a791
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:1.7-alpine` - linux; amd64

```console
$ docker pull traefik@sha256:0dcaa21539f6a679eeec2235ef295bf52dc618802a2b86c2bd8f54fb0f918a66
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **24.6 MB (24606031 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3a53b1b425aa4bbaea25bf86763df668237f6261464995a72d1f413b6b8b23ee`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 24 Feb 2021 20:20:11 GMT
ADD file:7eeea546ecde7a036bf634c08719879d32c7ec6ae599708cd91dc1b830735223 in / 
# Wed, 24 Feb 2021 20:20:12 GMT
CMD ["/bin/sh"]
# Thu, 25 Feb 2021 03:23:41 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 25 Feb 2021 03:23:56 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/traefik/traefik/releases/download/v1.7.28/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Thu, 25 Feb 2021 03:23:56 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 25 Feb 2021 03:23:56 GMT
EXPOSE 80
# Thu, 25 Feb 2021 03:23:57 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 25 Feb 2021 03:23:57 GMT
CMD ["traefik"]
# Thu, 25 Feb 2021 03:23:57 GMT
LABEL org.opencontainers.image.vendor=traefik org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.28 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:e95f33c60a645d6d31f52fdc334aecec0d79a1b410789eae37fbf69efcd587ab`  
		Last Modified: Wed, 24 Feb 2021 20:20:43 GMT  
		Size: 2.8 MB (2815313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7caf618c71a94b64d99880ac96da93c76a3931b35dffe57842d5baa964afbb3`  
		Last Modified: Thu, 25 Feb 2021 03:24:54 GMT  
		Size: 674.1 KB (674094 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d86caf1517f080a3c9e8645f69c08191a124a38c59e3c657ecee9dd847a1dcc3`  
		Last Modified: Thu, 25 Feb 2021 03:25:16 GMT  
		Size: 21.1 MB (21116257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49dabb83fefe1e371ad0ad76ea6523ffd2a4e4884a2a88f7e7254bc52dca0000`  
		Last Modified: Thu, 25 Feb 2021 03:25:10 GMT  
		Size: 367.0 B  
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
$ docker pull traefik@sha256:7b6485e1c472dbbe4929740278ebd3a6102f89e5208ad98094f13d366cd7759c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **22.9 MB (22887723 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e433192bfcd73af95a95a11e410a94b1e7792f903ed5b5f89bffd264c1dce2e4`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 24 Feb 2021 20:39:51 GMT
ADD file:f8a47118a2fe92c166c426620bb4ea0090dbf17aed269177989f6dca70438750 in / 
# Wed, 24 Feb 2021 20:39:52 GMT
CMD ["/bin/sh"]
# Thu, 25 Feb 2021 04:18:27 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 25 Feb 2021 04:18:45 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/traefik/traefik/releases/download/v1.7.28/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Thu, 25 Feb 2021 04:18:46 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 25 Feb 2021 04:18:47 GMT
EXPOSE 80
# Thu, 25 Feb 2021 04:18:47 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 25 Feb 2021 04:18:48 GMT
CMD ["traefik"]
# Thu, 25 Feb 2021 04:18:48 GMT
LABEL org.opencontainers.image.vendor=traefik org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.28 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:0328c39aea610966704bee2d2a1c7108816950703f98b4585083cd18f8354380`  
		Last Modified: Wed, 24 Feb 2021 20:40:35 GMT  
		Size: 2.7 MB (2725816 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4961a79823a93d7b581d0d755b544c7ad8e44d35dec7296a3663c7815c9b8e5`  
		Last Modified: Thu, 25 Feb 2021 04:24:33 GMT  
		Size: 675.5 KB (675506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef006d431cee79db31d7d17cf98839851ea3b97f23cff779428c0d801f2e0669`  
		Last Modified: Thu, 25 Feb 2021 04:24:57 GMT  
		Size: 19.5 MB (19486033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a229f0ffeea6995923cfa28b4aa3137adb96ed94f63f8e7fd861c35b76785e2c`  
		Last Modified: Thu, 25 Feb 2021 04:24:51 GMT  
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
$ docker pull traefik@sha256:062dff1b5c54845f34147e04a251a645f3a5318c42da7127bf25a6e0d3c6e4d5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:2.4` - linux; amd64

```console
$ docker pull traefik@sha256:0cba9ff0d0fafa592f96d0ef0de2c1591bbce7c40fabb57dde2038c0ab3f2b73
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.1 MB (29071840 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:da4c4921aee8ad7a7f66870bb726a8fa4d18f9b0b927ab1ef572e06be5241d65`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 24 Feb 2021 20:20:11 GMT
ADD file:7eeea546ecde7a036bf634c08719879d32c7ec6ae599708cd91dc1b830735223 in / 
# Wed, 24 Feb 2021 20:20:12 GMT
CMD ["/bin/sh"]
# Thu, 25 Feb 2021 03:23:41 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 25 Feb 2021 03:23:46 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.4.5/traefik_v2.4.5_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 25 Feb 2021 03:23:46 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 25 Feb 2021 03:23:46 GMT
EXPOSE 80
# Thu, 25 Feb 2021 03:23:46 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 25 Feb 2021 03:23:47 GMT
CMD ["traefik"]
# Thu, 25 Feb 2021 03:23:47 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.4.5 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:e95f33c60a645d6d31f52fdc334aecec0d79a1b410789eae37fbf69efcd587ab`  
		Last Modified: Wed, 24 Feb 2021 20:20:43 GMT  
		Size: 2.8 MB (2815313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7caf618c71a94b64d99880ac96da93c76a3931b35dffe57842d5baa964afbb3`  
		Last Modified: Thu, 25 Feb 2021 03:24:54 GMT  
		Size: 674.1 KB (674094 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fe2d603874139eacbf2d7e18cdfa7eabd27a958eed533d7897ca97e176e2098`  
		Last Modified: Thu, 25 Feb 2021 03:25:00 GMT  
		Size: 25.6 MB (25582065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ae52e7c5a84ee094d3d4cadb9254fe582fb3bf5ee4459db8e0296ed4a7589fd`  
		Last Modified: Thu, 25 Feb 2021 03:24:53 GMT  
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
$ docker pull traefik@sha256:cb015f1dd60e184906c74e18791a4672de286e68d420a1c69f7b6aef3b9e4c16
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.7 MB (26735582 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7f1dc0a165876c6732f35991df0b6ee44a94aee162782d0e65f09d5de023af29`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 24 Feb 2021 20:39:51 GMT
ADD file:f8a47118a2fe92c166c426620bb4ea0090dbf17aed269177989f6dca70438750 in / 
# Wed, 24 Feb 2021 20:39:52 GMT
CMD ["/bin/sh"]
# Thu, 25 Feb 2021 04:18:27 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 25 Feb 2021 04:18:32 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.4.5/traefik_v2.4.5_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 25 Feb 2021 04:18:33 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 25 Feb 2021 04:18:33 GMT
EXPOSE 80
# Thu, 25 Feb 2021 04:18:34 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 25 Feb 2021 04:18:34 GMT
CMD ["traefik"]
# Thu, 25 Feb 2021 04:18:35 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.4.5 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:0328c39aea610966704bee2d2a1c7108816950703f98b4585083cd18f8354380`  
		Last Modified: Wed, 24 Feb 2021 20:40:35 GMT  
		Size: 2.7 MB (2725816 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4961a79823a93d7b581d0d755b544c7ad8e44d35dec7296a3663c7815c9b8e5`  
		Last Modified: Thu, 25 Feb 2021 04:24:33 GMT  
		Size: 675.5 KB (675506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9ab8ff4ffc015f2784025d016e57f87c58b493791912f6032182a23930a4312`  
		Last Modified: Thu, 25 Feb 2021 04:24:40 GMT  
		Size: 23.3 MB (23333893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dceb3bdde5806885fd1ee30d061aaf77bc9abcdff7d0a5cef10797211738765f`  
		Last Modified: Thu, 25 Feb 2021 04:24:33 GMT  
		Size: 367.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:2.4.6`

**does not exist** (yet?)

## `traefik:2.4.6-windowsservercore-1809`

**does not exist** (yet?)

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
$ docker pull traefik@sha256:062dff1b5c54845f34147e04a251a645f3a5318c42da7127bf25a6e0d3c6e4d5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:latest` - linux; amd64

```console
$ docker pull traefik@sha256:0cba9ff0d0fafa592f96d0ef0de2c1591bbce7c40fabb57dde2038c0ab3f2b73
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.1 MB (29071840 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:da4c4921aee8ad7a7f66870bb726a8fa4d18f9b0b927ab1ef572e06be5241d65`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 24 Feb 2021 20:20:11 GMT
ADD file:7eeea546ecde7a036bf634c08719879d32c7ec6ae599708cd91dc1b830735223 in / 
# Wed, 24 Feb 2021 20:20:12 GMT
CMD ["/bin/sh"]
# Thu, 25 Feb 2021 03:23:41 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 25 Feb 2021 03:23:46 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.4.5/traefik_v2.4.5_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 25 Feb 2021 03:23:46 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 25 Feb 2021 03:23:46 GMT
EXPOSE 80
# Thu, 25 Feb 2021 03:23:46 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 25 Feb 2021 03:23:47 GMT
CMD ["traefik"]
# Thu, 25 Feb 2021 03:23:47 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.4.5 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:e95f33c60a645d6d31f52fdc334aecec0d79a1b410789eae37fbf69efcd587ab`  
		Last Modified: Wed, 24 Feb 2021 20:20:43 GMT  
		Size: 2.8 MB (2815313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7caf618c71a94b64d99880ac96da93c76a3931b35dffe57842d5baa964afbb3`  
		Last Modified: Thu, 25 Feb 2021 03:24:54 GMT  
		Size: 674.1 KB (674094 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fe2d603874139eacbf2d7e18cdfa7eabd27a958eed533d7897ca97e176e2098`  
		Last Modified: Thu, 25 Feb 2021 03:25:00 GMT  
		Size: 25.6 MB (25582065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ae52e7c5a84ee094d3d4cadb9254fe582fb3bf5ee4459db8e0296ed4a7589fd`  
		Last Modified: Thu, 25 Feb 2021 03:24:53 GMT  
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
$ docker pull traefik@sha256:cb015f1dd60e184906c74e18791a4672de286e68d420a1c69f7b6aef3b9e4c16
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.7 MB (26735582 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7f1dc0a165876c6732f35991df0b6ee44a94aee162782d0e65f09d5de023af29`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 24 Feb 2021 20:39:51 GMT
ADD file:f8a47118a2fe92c166c426620bb4ea0090dbf17aed269177989f6dca70438750 in / 
# Wed, 24 Feb 2021 20:39:52 GMT
CMD ["/bin/sh"]
# Thu, 25 Feb 2021 04:18:27 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 25 Feb 2021 04:18:32 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.4.5/traefik_v2.4.5_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 25 Feb 2021 04:18:33 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 25 Feb 2021 04:18:33 GMT
EXPOSE 80
# Thu, 25 Feb 2021 04:18:34 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 25 Feb 2021 04:18:34 GMT
CMD ["traefik"]
# Thu, 25 Feb 2021 04:18:35 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.4.5 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:0328c39aea610966704bee2d2a1c7108816950703f98b4585083cd18f8354380`  
		Last Modified: Wed, 24 Feb 2021 20:40:35 GMT  
		Size: 2.7 MB (2725816 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4961a79823a93d7b581d0d755b544c7ad8e44d35dec7296a3663c7815c9b8e5`  
		Last Modified: Thu, 25 Feb 2021 04:24:33 GMT  
		Size: 675.5 KB (675506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9ab8ff4ffc015f2784025d016e57f87c58b493791912f6032182a23930a4312`  
		Last Modified: Thu, 25 Feb 2021 04:24:40 GMT  
		Size: 23.3 MB (23333893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dceb3bdde5806885fd1ee30d061aaf77bc9abcdff7d0a5cef10797211738765f`  
		Last Modified: Thu, 25 Feb 2021 04:24:33 GMT  
		Size: 367.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:livarot`

```console
$ docker pull traefik@sha256:062dff1b5c54845f34147e04a251a645f3a5318c42da7127bf25a6e0d3c6e4d5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:livarot` - linux; amd64

```console
$ docker pull traefik@sha256:0cba9ff0d0fafa592f96d0ef0de2c1591bbce7c40fabb57dde2038c0ab3f2b73
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.1 MB (29071840 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:da4c4921aee8ad7a7f66870bb726a8fa4d18f9b0b927ab1ef572e06be5241d65`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 24 Feb 2021 20:20:11 GMT
ADD file:7eeea546ecde7a036bf634c08719879d32c7ec6ae599708cd91dc1b830735223 in / 
# Wed, 24 Feb 2021 20:20:12 GMT
CMD ["/bin/sh"]
# Thu, 25 Feb 2021 03:23:41 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 25 Feb 2021 03:23:46 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.4.5/traefik_v2.4.5_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 25 Feb 2021 03:23:46 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 25 Feb 2021 03:23:46 GMT
EXPOSE 80
# Thu, 25 Feb 2021 03:23:46 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 25 Feb 2021 03:23:47 GMT
CMD ["traefik"]
# Thu, 25 Feb 2021 03:23:47 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.4.5 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:e95f33c60a645d6d31f52fdc334aecec0d79a1b410789eae37fbf69efcd587ab`  
		Last Modified: Wed, 24 Feb 2021 20:20:43 GMT  
		Size: 2.8 MB (2815313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7caf618c71a94b64d99880ac96da93c76a3931b35dffe57842d5baa964afbb3`  
		Last Modified: Thu, 25 Feb 2021 03:24:54 GMT  
		Size: 674.1 KB (674094 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fe2d603874139eacbf2d7e18cdfa7eabd27a958eed533d7897ca97e176e2098`  
		Last Modified: Thu, 25 Feb 2021 03:25:00 GMT  
		Size: 25.6 MB (25582065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ae52e7c5a84ee094d3d4cadb9254fe582fb3bf5ee4459db8e0296ed4a7589fd`  
		Last Modified: Thu, 25 Feb 2021 03:24:53 GMT  
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
$ docker pull traefik@sha256:cb015f1dd60e184906c74e18791a4672de286e68d420a1c69f7b6aef3b9e4c16
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.7 MB (26735582 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7f1dc0a165876c6732f35991df0b6ee44a94aee162782d0e65f09d5de023af29`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 24 Feb 2021 20:39:51 GMT
ADD file:f8a47118a2fe92c166c426620bb4ea0090dbf17aed269177989f6dca70438750 in / 
# Wed, 24 Feb 2021 20:39:52 GMT
CMD ["/bin/sh"]
# Thu, 25 Feb 2021 04:18:27 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 25 Feb 2021 04:18:32 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.4.5/traefik_v2.4.5_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 25 Feb 2021 04:18:33 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 25 Feb 2021 04:18:33 GMT
EXPOSE 80
# Thu, 25 Feb 2021 04:18:34 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 25 Feb 2021 04:18:34 GMT
CMD ["traefik"]
# Thu, 25 Feb 2021 04:18:35 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.4.5 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:0328c39aea610966704bee2d2a1c7108816950703f98b4585083cd18f8354380`  
		Last Modified: Wed, 24 Feb 2021 20:40:35 GMT  
		Size: 2.7 MB (2725816 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4961a79823a93d7b581d0d755b544c7ad8e44d35dec7296a3663c7815c9b8e5`  
		Last Modified: Thu, 25 Feb 2021 04:24:33 GMT  
		Size: 675.5 KB (675506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9ab8ff4ffc015f2784025d016e57f87c58b493791912f6032182a23930a4312`  
		Last Modified: Thu, 25 Feb 2021 04:24:40 GMT  
		Size: 23.3 MB (23333893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dceb3bdde5806885fd1ee30d061aaf77bc9abcdff7d0a5cef10797211738765f`  
		Last Modified: Thu, 25 Feb 2021 04:24:33 GMT  
		Size: 367.0 B  
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
$ docker pull traefik@sha256:6fcc1a5ef1fc56c7e8ef206407f086feffe155edba2b09e8e2ff51903d5a8af1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:maroilles` - linux; amd64

```console
$ docker pull traefik@sha256:70a8743d69121fa77b5d561e3c3dd8cdcafe552467d503bfbb70063289aa7f09
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **21.6 MB (21555688 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a0013bcad7721f151cc49a02c90ad1f8bab70f17fd8cb9b39953e18e251395d6`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Thu, 17 Dec 2020 00:48:11 GMT
COPY file:cd6264d9a7514a8fbc3eb7b400566d36178794d2b757959812cc3abc6f13a97b in /etc/ssl/certs/ 
# Thu, 25 Feb 2021 03:24:27 GMT
COPY dir:379603788862c2a6c57432d70b0a67f561fe00310e1b958c9ecf85381b1c9cd9 in /usr/share/ 
# Thu, 25 Feb 2021 03:24:29 GMT
COPY file:94b9997cc55c7732c9fc173c119f980e4a38eba20b96a90170a3d7fade75f0eb in / 
# Thu, 25 Feb 2021 03:24:29 GMT
EXPOSE 80
# Thu, 25 Feb 2021 03:24:29 GMT
VOLUME [/tmp]
# Thu, 25 Feb 2021 03:24:29 GMT
ENTRYPOINT ["/traefik"]
# Thu, 25 Feb 2021 03:24:30 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.28 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:79de75e85675fa9abbac17b57205d3e0dfcf2bd2fc4cbc194f2aaf917435425e`  
		Last Modified: Thu, 17 Dec 2020 00:49:17 GMT  
		Size: 130.9 KB (130872 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07ccc62f6df1194af0864cbbff567afef1c70d510c6bc4c8e101c6e64def6d70`  
		Last Modified: Thu, 25 Feb 2021 03:25:24 GMT  
		Size: 308.8 KB (308817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff9e7c6f1cdda4e2fd24a670a1af35baae7f2b51de21646bb8088636362f47c5`  
		Last Modified: Thu, 25 Feb 2021 03:25:30 GMT  
		Size: 21.1 MB (21115999 bytes)  
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
$ docker pull traefik@sha256:f8aa3bcee0d52f8101d2179ed61d34141d263bf2320ceef88ff77e986025a791
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:maroilles-alpine` - linux; amd64

```console
$ docker pull traefik@sha256:0dcaa21539f6a679eeec2235ef295bf52dc618802a2b86c2bd8f54fb0f918a66
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **24.6 MB (24606031 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3a53b1b425aa4bbaea25bf86763df668237f6261464995a72d1f413b6b8b23ee`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 24 Feb 2021 20:20:11 GMT
ADD file:7eeea546ecde7a036bf634c08719879d32c7ec6ae599708cd91dc1b830735223 in / 
# Wed, 24 Feb 2021 20:20:12 GMT
CMD ["/bin/sh"]
# Thu, 25 Feb 2021 03:23:41 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 25 Feb 2021 03:23:56 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/traefik/traefik/releases/download/v1.7.28/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Thu, 25 Feb 2021 03:23:56 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 25 Feb 2021 03:23:56 GMT
EXPOSE 80
# Thu, 25 Feb 2021 03:23:57 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 25 Feb 2021 03:23:57 GMT
CMD ["traefik"]
# Thu, 25 Feb 2021 03:23:57 GMT
LABEL org.opencontainers.image.vendor=traefik org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.28 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:e95f33c60a645d6d31f52fdc334aecec0d79a1b410789eae37fbf69efcd587ab`  
		Last Modified: Wed, 24 Feb 2021 20:20:43 GMT  
		Size: 2.8 MB (2815313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7caf618c71a94b64d99880ac96da93c76a3931b35dffe57842d5baa964afbb3`  
		Last Modified: Thu, 25 Feb 2021 03:24:54 GMT  
		Size: 674.1 KB (674094 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d86caf1517f080a3c9e8645f69c08191a124a38c59e3c657ecee9dd847a1dcc3`  
		Last Modified: Thu, 25 Feb 2021 03:25:16 GMT  
		Size: 21.1 MB (21116257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49dabb83fefe1e371ad0ad76ea6523ffd2a4e4884a2a88f7e7254bc52dca0000`  
		Last Modified: Thu, 25 Feb 2021 03:25:10 GMT  
		Size: 367.0 B  
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
$ docker pull traefik@sha256:7b6485e1c472dbbe4929740278ebd3a6102f89e5208ad98094f13d366cd7759c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **22.9 MB (22887723 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e433192bfcd73af95a95a11e410a94b1e7792f903ed5b5f89bffd264c1dce2e4`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 24 Feb 2021 20:39:51 GMT
ADD file:f8a47118a2fe92c166c426620bb4ea0090dbf17aed269177989f6dca70438750 in / 
# Wed, 24 Feb 2021 20:39:52 GMT
CMD ["/bin/sh"]
# Thu, 25 Feb 2021 04:18:27 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 25 Feb 2021 04:18:45 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/traefik/traefik/releases/download/v1.7.28/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Thu, 25 Feb 2021 04:18:46 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 25 Feb 2021 04:18:47 GMT
EXPOSE 80
# Thu, 25 Feb 2021 04:18:47 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 25 Feb 2021 04:18:48 GMT
CMD ["traefik"]
# Thu, 25 Feb 2021 04:18:48 GMT
LABEL org.opencontainers.image.vendor=traefik org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.28 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:0328c39aea610966704bee2d2a1c7108816950703f98b4585083cd18f8354380`  
		Last Modified: Wed, 24 Feb 2021 20:40:35 GMT  
		Size: 2.7 MB (2725816 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4961a79823a93d7b581d0d755b544c7ad8e44d35dec7296a3663c7815c9b8e5`  
		Last Modified: Thu, 25 Feb 2021 04:24:33 GMT  
		Size: 675.5 KB (675506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef006d431cee79db31d7d17cf98839851ea3b97f23cff779428c0d801f2e0669`  
		Last Modified: Thu, 25 Feb 2021 04:24:57 GMT  
		Size: 19.5 MB (19486033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a229f0ffeea6995923cfa28b4aa3137adb96ed94f63f8e7fd861c35b76785e2c`  
		Last Modified: Thu, 25 Feb 2021 04:24:51 GMT  
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
$ docker pull traefik@sha256:6fcc1a5ef1fc56c7e8ef206407f086feffe155edba2b09e8e2ff51903d5a8af1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:v1.7` - linux; amd64

```console
$ docker pull traefik@sha256:70a8743d69121fa77b5d561e3c3dd8cdcafe552467d503bfbb70063289aa7f09
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **21.6 MB (21555688 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a0013bcad7721f151cc49a02c90ad1f8bab70f17fd8cb9b39953e18e251395d6`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Thu, 17 Dec 2020 00:48:11 GMT
COPY file:cd6264d9a7514a8fbc3eb7b400566d36178794d2b757959812cc3abc6f13a97b in /etc/ssl/certs/ 
# Thu, 25 Feb 2021 03:24:27 GMT
COPY dir:379603788862c2a6c57432d70b0a67f561fe00310e1b958c9ecf85381b1c9cd9 in /usr/share/ 
# Thu, 25 Feb 2021 03:24:29 GMT
COPY file:94b9997cc55c7732c9fc173c119f980e4a38eba20b96a90170a3d7fade75f0eb in / 
# Thu, 25 Feb 2021 03:24:29 GMT
EXPOSE 80
# Thu, 25 Feb 2021 03:24:29 GMT
VOLUME [/tmp]
# Thu, 25 Feb 2021 03:24:29 GMT
ENTRYPOINT ["/traefik"]
# Thu, 25 Feb 2021 03:24:30 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.28 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:79de75e85675fa9abbac17b57205d3e0dfcf2bd2fc4cbc194f2aaf917435425e`  
		Last Modified: Thu, 17 Dec 2020 00:49:17 GMT  
		Size: 130.9 KB (130872 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07ccc62f6df1194af0864cbbff567afef1c70d510c6bc4c8e101c6e64def6d70`  
		Last Modified: Thu, 25 Feb 2021 03:25:24 GMT  
		Size: 308.8 KB (308817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff9e7c6f1cdda4e2fd24a670a1af35baae7f2b51de21646bb8088636362f47c5`  
		Last Modified: Thu, 25 Feb 2021 03:25:30 GMT  
		Size: 21.1 MB (21115999 bytes)  
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

## `traefik:v1.7.28`

```console
$ docker pull traefik@sha256:6fcc1a5ef1fc56c7e8ef206407f086feffe155edba2b09e8e2ff51903d5a8af1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:v1.7.28` - linux; amd64

```console
$ docker pull traefik@sha256:70a8743d69121fa77b5d561e3c3dd8cdcafe552467d503bfbb70063289aa7f09
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **21.6 MB (21555688 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a0013bcad7721f151cc49a02c90ad1f8bab70f17fd8cb9b39953e18e251395d6`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Thu, 17 Dec 2020 00:48:11 GMT
COPY file:cd6264d9a7514a8fbc3eb7b400566d36178794d2b757959812cc3abc6f13a97b in /etc/ssl/certs/ 
# Thu, 25 Feb 2021 03:24:27 GMT
COPY dir:379603788862c2a6c57432d70b0a67f561fe00310e1b958c9ecf85381b1c9cd9 in /usr/share/ 
# Thu, 25 Feb 2021 03:24:29 GMT
COPY file:94b9997cc55c7732c9fc173c119f980e4a38eba20b96a90170a3d7fade75f0eb in / 
# Thu, 25 Feb 2021 03:24:29 GMT
EXPOSE 80
# Thu, 25 Feb 2021 03:24:29 GMT
VOLUME [/tmp]
# Thu, 25 Feb 2021 03:24:29 GMT
ENTRYPOINT ["/traefik"]
# Thu, 25 Feb 2021 03:24:30 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.28 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:79de75e85675fa9abbac17b57205d3e0dfcf2bd2fc4cbc194f2aaf917435425e`  
		Last Modified: Thu, 17 Dec 2020 00:49:17 GMT  
		Size: 130.9 KB (130872 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07ccc62f6df1194af0864cbbff567afef1c70d510c6bc4c8e101c6e64def6d70`  
		Last Modified: Thu, 25 Feb 2021 03:25:24 GMT  
		Size: 308.8 KB (308817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff9e7c6f1cdda4e2fd24a670a1af35baae7f2b51de21646bb8088636362f47c5`  
		Last Modified: Thu, 25 Feb 2021 03:25:30 GMT  
		Size: 21.1 MB (21115999 bytes)  
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
$ docker pull traefik@sha256:f8aa3bcee0d52f8101d2179ed61d34141d263bf2320ceef88ff77e986025a791
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:v1.7.28-alpine` - linux; amd64

```console
$ docker pull traefik@sha256:0dcaa21539f6a679eeec2235ef295bf52dc618802a2b86c2bd8f54fb0f918a66
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **24.6 MB (24606031 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3a53b1b425aa4bbaea25bf86763df668237f6261464995a72d1f413b6b8b23ee`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 24 Feb 2021 20:20:11 GMT
ADD file:7eeea546ecde7a036bf634c08719879d32c7ec6ae599708cd91dc1b830735223 in / 
# Wed, 24 Feb 2021 20:20:12 GMT
CMD ["/bin/sh"]
# Thu, 25 Feb 2021 03:23:41 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 25 Feb 2021 03:23:56 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/traefik/traefik/releases/download/v1.7.28/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Thu, 25 Feb 2021 03:23:56 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 25 Feb 2021 03:23:56 GMT
EXPOSE 80
# Thu, 25 Feb 2021 03:23:57 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 25 Feb 2021 03:23:57 GMT
CMD ["traefik"]
# Thu, 25 Feb 2021 03:23:57 GMT
LABEL org.opencontainers.image.vendor=traefik org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.28 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:e95f33c60a645d6d31f52fdc334aecec0d79a1b410789eae37fbf69efcd587ab`  
		Last Modified: Wed, 24 Feb 2021 20:20:43 GMT  
		Size: 2.8 MB (2815313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7caf618c71a94b64d99880ac96da93c76a3931b35dffe57842d5baa964afbb3`  
		Last Modified: Thu, 25 Feb 2021 03:24:54 GMT  
		Size: 674.1 KB (674094 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d86caf1517f080a3c9e8645f69c08191a124a38c59e3c657ecee9dd847a1dcc3`  
		Last Modified: Thu, 25 Feb 2021 03:25:16 GMT  
		Size: 21.1 MB (21116257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49dabb83fefe1e371ad0ad76ea6523ffd2a4e4884a2a88f7e7254bc52dca0000`  
		Last Modified: Thu, 25 Feb 2021 03:25:10 GMT  
		Size: 367.0 B  
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
$ docker pull traefik@sha256:7b6485e1c472dbbe4929740278ebd3a6102f89e5208ad98094f13d366cd7759c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **22.9 MB (22887723 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e433192bfcd73af95a95a11e410a94b1e7792f903ed5b5f89bffd264c1dce2e4`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 24 Feb 2021 20:39:51 GMT
ADD file:f8a47118a2fe92c166c426620bb4ea0090dbf17aed269177989f6dca70438750 in / 
# Wed, 24 Feb 2021 20:39:52 GMT
CMD ["/bin/sh"]
# Thu, 25 Feb 2021 04:18:27 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 25 Feb 2021 04:18:45 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/traefik/traefik/releases/download/v1.7.28/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Thu, 25 Feb 2021 04:18:46 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 25 Feb 2021 04:18:47 GMT
EXPOSE 80
# Thu, 25 Feb 2021 04:18:47 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 25 Feb 2021 04:18:48 GMT
CMD ["traefik"]
# Thu, 25 Feb 2021 04:18:48 GMT
LABEL org.opencontainers.image.vendor=traefik org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.28 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:0328c39aea610966704bee2d2a1c7108816950703f98b4585083cd18f8354380`  
		Last Modified: Wed, 24 Feb 2021 20:40:35 GMT  
		Size: 2.7 MB (2725816 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4961a79823a93d7b581d0d755b544c7ad8e44d35dec7296a3663c7815c9b8e5`  
		Last Modified: Thu, 25 Feb 2021 04:24:33 GMT  
		Size: 675.5 KB (675506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef006d431cee79db31d7d17cf98839851ea3b97f23cff779428c0d801f2e0669`  
		Last Modified: Thu, 25 Feb 2021 04:24:57 GMT  
		Size: 19.5 MB (19486033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a229f0ffeea6995923cfa28b4aa3137adb96ed94f63f8e7fd861c35b76785e2c`  
		Last Modified: Thu, 25 Feb 2021 04:24:51 GMT  
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
$ docker pull traefik@sha256:f8aa3bcee0d52f8101d2179ed61d34141d263bf2320ceef88ff77e986025a791
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:v1.7-alpine` - linux; amd64

```console
$ docker pull traefik@sha256:0dcaa21539f6a679eeec2235ef295bf52dc618802a2b86c2bd8f54fb0f918a66
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **24.6 MB (24606031 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3a53b1b425aa4bbaea25bf86763df668237f6261464995a72d1f413b6b8b23ee`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 24 Feb 2021 20:20:11 GMT
ADD file:7eeea546ecde7a036bf634c08719879d32c7ec6ae599708cd91dc1b830735223 in / 
# Wed, 24 Feb 2021 20:20:12 GMT
CMD ["/bin/sh"]
# Thu, 25 Feb 2021 03:23:41 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 25 Feb 2021 03:23:56 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/traefik/traefik/releases/download/v1.7.28/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Thu, 25 Feb 2021 03:23:56 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 25 Feb 2021 03:23:56 GMT
EXPOSE 80
# Thu, 25 Feb 2021 03:23:57 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 25 Feb 2021 03:23:57 GMT
CMD ["traefik"]
# Thu, 25 Feb 2021 03:23:57 GMT
LABEL org.opencontainers.image.vendor=traefik org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.28 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:e95f33c60a645d6d31f52fdc334aecec0d79a1b410789eae37fbf69efcd587ab`  
		Last Modified: Wed, 24 Feb 2021 20:20:43 GMT  
		Size: 2.8 MB (2815313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7caf618c71a94b64d99880ac96da93c76a3931b35dffe57842d5baa964afbb3`  
		Last Modified: Thu, 25 Feb 2021 03:24:54 GMT  
		Size: 674.1 KB (674094 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d86caf1517f080a3c9e8645f69c08191a124a38c59e3c657ecee9dd847a1dcc3`  
		Last Modified: Thu, 25 Feb 2021 03:25:16 GMT  
		Size: 21.1 MB (21116257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49dabb83fefe1e371ad0ad76ea6523ffd2a4e4884a2a88f7e7254bc52dca0000`  
		Last Modified: Thu, 25 Feb 2021 03:25:10 GMT  
		Size: 367.0 B  
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
$ docker pull traefik@sha256:7b6485e1c472dbbe4929740278ebd3a6102f89e5208ad98094f13d366cd7759c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **22.9 MB (22887723 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e433192bfcd73af95a95a11e410a94b1e7792f903ed5b5f89bffd264c1dce2e4`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 24 Feb 2021 20:39:51 GMT
ADD file:f8a47118a2fe92c166c426620bb4ea0090dbf17aed269177989f6dca70438750 in / 
# Wed, 24 Feb 2021 20:39:52 GMT
CMD ["/bin/sh"]
# Thu, 25 Feb 2021 04:18:27 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 25 Feb 2021 04:18:45 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/traefik/traefik/releases/download/v1.7.28/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Thu, 25 Feb 2021 04:18:46 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 25 Feb 2021 04:18:47 GMT
EXPOSE 80
# Thu, 25 Feb 2021 04:18:47 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 25 Feb 2021 04:18:48 GMT
CMD ["traefik"]
# Thu, 25 Feb 2021 04:18:48 GMT
LABEL org.opencontainers.image.vendor=traefik org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.28 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:0328c39aea610966704bee2d2a1c7108816950703f98b4585083cd18f8354380`  
		Last Modified: Wed, 24 Feb 2021 20:40:35 GMT  
		Size: 2.7 MB (2725816 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4961a79823a93d7b581d0d755b544c7ad8e44d35dec7296a3663c7815c9b8e5`  
		Last Modified: Thu, 25 Feb 2021 04:24:33 GMT  
		Size: 675.5 KB (675506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef006d431cee79db31d7d17cf98839851ea3b97f23cff779428c0d801f2e0669`  
		Last Modified: Thu, 25 Feb 2021 04:24:57 GMT  
		Size: 19.5 MB (19486033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a229f0ffeea6995923cfa28b4aa3137adb96ed94f63f8e7fd861c35b76785e2c`  
		Last Modified: Thu, 25 Feb 2021 04:24:51 GMT  
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
$ docker pull traefik@sha256:062dff1b5c54845f34147e04a251a645f3a5318c42da7127bf25a6e0d3c6e4d5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:v2.4` - linux; amd64

```console
$ docker pull traefik@sha256:0cba9ff0d0fafa592f96d0ef0de2c1591bbce7c40fabb57dde2038c0ab3f2b73
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.1 MB (29071840 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:da4c4921aee8ad7a7f66870bb726a8fa4d18f9b0b927ab1ef572e06be5241d65`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 24 Feb 2021 20:20:11 GMT
ADD file:7eeea546ecde7a036bf634c08719879d32c7ec6ae599708cd91dc1b830735223 in / 
# Wed, 24 Feb 2021 20:20:12 GMT
CMD ["/bin/sh"]
# Thu, 25 Feb 2021 03:23:41 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 25 Feb 2021 03:23:46 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.4.5/traefik_v2.4.5_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 25 Feb 2021 03:23:46 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 25 Feb 2021 03:23:46 GMT
EXPOSE 80
# Thu, 25 Feb 2021 03:23:46 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 25 Feb 2021 03:23:47 GMT
CMD ["traefik"]
# Thu, 25 Feb 2021 03:23:47 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.4.5 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:e95f33c60a645d6d31f52fdc334aecec0d79a1b410789eae37fbf69efcd587ab`  
		Last Modified: Wed, 24 Feb 2021 20:20:43 GMT  
		Size: 2.8 MB (2815313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7caf618c71a94b64d99880ac96da93c76a3931b35dffe57842d5baa964afbb3`  
		Last Modified: Thu, 25 Feb 2021 03:24:54 GMT  
		Size: 674.1 KB (674094 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fe2d603874139eacbf2d7e18cdfa7eabd27a958eed533d7897ca97e176e2098`  
		Last Modified: Thu, 25 Feb 2021 03:25:00 GMT  
		Size: 25.6 MB (25582065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ae52e7c5a84ee094d3d4cadb9254fe582fb3bf5ee4459db8e0296ed4a7589fd`  
		Last Modified: Thu, 25 Feb 2021 03:24:53 GMT  
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
$ docker pull traefik@sha256:cb015f1dd60e184906c74e18791a4672de286e68d420a1c69f7b6aef3b9e4c16
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.7 MB (26735582 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7f1dc0a165876c6732f35991df0b6ee44a94aee162782d0e65f09d5de023af29`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 24 Feb 2021 20:39:51 GMT
ADD file:f8a47118a2fe92c166c426620bb4ea0090dbf17aed269177989f6dca70438750 in / 
# Wed, 24 Feb 2021 20:39:52 GMT
CMD ["/bin/sh"]
# Thu, 25 Feb 2021 04:18:27 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 25 Feb 2021 04:18:32 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.4.5/traefik_v2.4.5_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 25 Feb 2021 04:18:33 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 25 Feb 2021 04:18:33 GMT
EXPOSE 80
# Thu, 25 Feb 2021 04:18:34 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 25 Feb 2021 04:18:34 GMT
CMD ["traefik"]
# Thu, 25 Feb 2021 04:18:35 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.4.5 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:0328c39aea610966704bee2d2a1c7108816950703f98b4585083cd18f8354380`  
		Last Modified: Wed, 24 Feb 2021 20:40:35 GMT  
		Size: 2.7 MB (2725816 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4961a79823a93d7b581d0d755b544c7ad8e44d35dec7296a3663c7815c9b8e5`  
		Last Modified: Thu, 25 Feb 2021 04:24:33 GMT  
		Size: 675.5 KB (675506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9ab8ff4ffc015f2784025d016e57f87c58b493791912f6032182a23930a4312`  
		Last Modified: Thu, 25 Feb 2021 04:24:40 GMT  
		Size: 23.3 MB (23333893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dceb3bdde5806885fd1ee30d061aaf77bc9abcdff7d0a5cef10797211738765f`  
		Last Modified: Thu, 25 Feb 2021 04:24:33 GMT  
		Size: 367.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v2.4.6`

**does not exist** (yet?)

## `traefik:v2.4.6-windowsservercore-1809`

**does not exist** (yet?)

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
